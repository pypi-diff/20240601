# Comparing `tmp/genvarloader-0.3.2.tar.gz` & `tmp/genvarloader-0.3.3.tar.gz`

## Comparing `genvarloader-0.3.2.tar` & `genvarloader-0.3.3.tar`

### file list

```diff
@@ -1,209 +1,211 @@
--rw-r--r--   0        0        0      430 1970-01-01 00:00:00.000000 genvarloader-0.3.2/Cargo.toml
--rw-r--r--   0     1111     7010     2214 2024-04-29 19:03:18.000000 genvarloader-0.3.2/.gitignore
--rw-r--r--   0     1111     7010      432 2024-03-15 17:35:16.000000 genvarloader-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0     1111     7010     1066 2024-02-21 06:02:22.000000 genvarloader-0.3.2/LICENSE.txt
--rw-r--r--   0     1111     7010     2490 2024-02-21 06:02:22.000000 genvarloader-0.3.2/README.md
--rw-r--r--   0     1111     7010      624 2024-02-21 06:02:22.000000 genvarloader-0.3.2/dev-environment.yml
--rw-r--r--   0     1111     7010      365 2024-02-21 06:02:22.000000 genvarloader-0.3.2/environment.yml
--rw-r--r--   0     1111     7010   159221 2024-04-29 18:12:28.000000 genvarloader-0.3.2/poetry.lock
--rw-r--r--   0     1111     7010      912 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/__init__.py
--rw-r--r--   0     1111     7010     3692 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/__main__.py
--rw-r--r--   0     1111     7010     6056 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/bigwig.py
--rw-r--r--   0     1111     7010      974 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/concurrent.py
--rw-r--r--   0     1111     7010    37145 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/dataset/__init__.py
--rw-r--r--   0     1111     7010    34411 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/dataset/genotypes.py
--rw-r--r--   0     1111     7010     5335 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/dataset/intervals.py
--rw-r--r--   0     1111     7010     1679 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/dataset/reference.py
--rw-r--r--   0     1111     7010    15054 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/dataset/tracks.py
--rw-r--r--   0     1111     7010     4110 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/dataset/utils.py
--rw-r--r--   0     1111     7010    15815 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/dataset/write.py
--rw-r--r--   0     1111     7010     8343 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/fasta.py
--rw-r--r--   0     1111     7010      877 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/genvarloader.pyi
--rw-r--r--   0     1111     7010    25831 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/haplotypes.py
--rw-r--r--   0     1111     7010    10153 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/intervals.py
--rw-r--r--   0     1111     7010    48210 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/loader.py
--rw-r--r--   0     1111     7010        0 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/py.typed
--rw-r--r--   0     1111     7010     4215 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/torch.py
--rw-r--r--   0     1111     7010     8437 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/types.py
--rw-r--r--   0     1111     7010    13407 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/utils.py
--rw-r--r--   0     1111     7010     8986 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/variants/__init__.py
--rw-r--r--   0     1111     7010     9120 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/variants/genotypes.py
--rw-r--r--   0     1111     7010    30658 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/variants/records.py
--rw-r--r--   0     1111     7010    10433 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/zarr.py
--rw-r--r--   0     1111     7010     4206 2024-04-29 18:12:28.000000 genvarloader-0.3.2/src/bigwig.rs
--rw-r--r--   0     1111     7010     1325 2024-04-29 18:12:28.000000 genvarloader-0.3.2/src/lib.rs
--rw-r--r--   0     1111     7010     1697 2024-02-21 06:05:07.000000 genvarloader-0.3.2/tests/data/pgen/sample.ends.gvl.arrow
--rw-r--r--   0     1111     7010     2189 2024-02-21 06:05:07.000000 genvarloader-0.3.2/tests/data/pgen/sample.gvl.arrow
--rw-r--r--   0     1111     7010       63 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/pgen/sample.pgen
--rw-r--r--   0     1111     7010       42 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/pgen/sample.psam
--rw-r--r--   0     1111     7010     2241 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/pgen/sample.pvar
--rw-r--r--   0     1111     7010       24 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr0_h1.fa
--rw-r--r--   0     1111     7010       23 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr0_h1.fa.fai
--rw-r--r--   0     1111     7010       24 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr0_h2.fa
--rw-r--r--   0     1111     7010       23 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr0_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr10_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr10_h1.fa.fai
--rw-r--r--   0     1111     7010       33 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr10_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr10_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr11_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr11_h1.fa.fai
--rw-r--r--   0     1111     7010       33 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr11_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr11_h2.fa.fai
--rw-r--r--   0     1111     7010       29 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr1_h1.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr1_h1.fa.fai
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr1_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr1_h2.fa.fai
--rw-r--r--   0     1111     7010       29 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr2_h1.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr2_h1.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr2_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr2_h2.fa.fai
--rw-r--r--   0     1111     7010       29 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr3_h1.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr3_h1.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr3_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr3_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr4_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr4_h1.fa.fai
--rw-r--r--   0     1111     7010      108 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr4_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr4_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr5_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr5_h1.fa.fai
--rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr5_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr5_h2.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr6_h1.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr6_h1.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr6_h2.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr6_h2.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr7_h1.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr7_h1.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr7_h2.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr7_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr8_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr8_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr8_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr8_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr9_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr9_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr9_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr9_h2.fa.fai
--rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr0_h1.fa
--rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr0_h1.fa.fai
--rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr0_h2.fa
--rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr0_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr10_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr10_h1.fa.fai
--rw-r--r--   0     1111     7010       33 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr10_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr10_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr11_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr11_h1.fa.fai
--rw-r--r--   0     1111     7010       33 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr11_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr11_h2.fa.fai
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr1_h1.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr1_h1.fa.fai
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr1_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr1_h2.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr2_h1.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr2_h1.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr2_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr2_h2.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr3_h1.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr3_h1.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr3_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr3_h2.fa.fai
--rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr4_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr4_h1.fa.fai
--rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr4_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr4_h2.fa.fai
--rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr5_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr5_h1.fa.fai
--rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr5_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr5_h2.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr6_h1.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr6_h1.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr6_h2.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr6_h2.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr7_h1.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr7_h1.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr7_h2.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr7_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr8_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr8_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr8_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr8_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr9_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr9_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr9_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr9_h2.fa.fai
--rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr0_h1.fa
--rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr0_h1.fa.fai
--rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr0_h2.fa
--rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr0_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr10_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr10_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr10_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr10_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr11_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr11_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr11_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr11_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr1_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr1_h1.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr1_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr1_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr2_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr2_h1.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr2_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr2_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr3_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr3_h1.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr3_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr3_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr4_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr4_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr4_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr4_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr5_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr5_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr5_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr5_h2.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr6_h1.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr6_h1.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr6_h2.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr6_h2.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr7_h1.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr7_h1.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr7_h2.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr7_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr8_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr8_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr8_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr8_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr9_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr9_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr9_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr9_h2.fa.fai
--rw-r--r--   0     1111     7010     1761 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.ends.gvl.arrow
--rw-r--r--   0     1111     7010     1997 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.gvl.arrow
--rw-r--r--   0     1111     7010      223 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.gvl.genos.zarr/.zarray
--rw-r--r--   0     1111     7010      133 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.gvl.genos.zarr/.zattrs
--rw-r--r--   0     1111     7010    81381 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.gvl.genos.zarr/0.0.0
--rw-r--r--   0     1111     7010     2890 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.vcf
--rw-r--r--   0     1111     7010     1272 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.vcf.gz
--rw-r--r--   0     1111     7010      189 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.vcf.gz.csi
--rw-r--r--   0     1111     7010     6218 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/generate_ground_truth.py
--rw-r--r--   0     1111     7010      212 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/sample.bed
--rw-r--r--   0     1111     7010     2327 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/sample.vcf
--rw-r--r--   0     1111     7010     2136 2024-04-29 18:12:28.000000 genvarloader-0.3.2/tests/dataset/genotypes/test_dense2sparse.py
--rw-r--r--   0     1111     7010     1626 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/test_fasta.py
--rw-r--r--   0     1111     7010     2814 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/test_fasta_variants.py
--rw-r--r--   0     1111     7010     1625 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/test_loader.py
--rw-r--r--   0     1111     7010     3102 2024-04-16 16:39:32.000000 genvarloader-0.3.2/tests/test_max_ends.py
--rw-r--r--   0     1111     7010     5838 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/test_pgen.py
--rw-r--r--   0     1111     7010      391 2024-04-29 18:12:28.000000 genvarloader-0.3.2/tests/test_utils.py
--rw-r--r--   0     1111     7010      633 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/test_variants.py
--rw-r--r--   0     1111     7010     3677 2024-04-29 18:12:28.000000 genvarloader-0.3.2/tests/tracks/bench_cpu_gpu.py
--rw-r--r--   0     1111     7010     3484 2024-04-29 18:12:28.000000 genvarloader-0.3.2/tests/tracks/test_i2t_t2i.py
--rw-r--r--   0     1111     7010     1000 2024-04-29 18:12:28.000000 genvarloader-0.3.2/tests/tracks/test_random_nonoverlapping.py
--rw-r--r--   0     1111     7010     2435 2024-04-29 18:12:28.000000 genvarloader-0.3.2/tests/tracks/utils.py
--rw-r--r--   0     1111     7010    35103 2024-04-29 18:12:28.000000 genvarloader-0.3.2/Cargo.lock
--rw-r--r--   0     1111     7010     1778 2024-04-29 19:04:29.000000 genvarloader-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3355 1970-01-01 00:00:00.000000 genvarloader-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      430 1970-01-01 00:00:00.000000 genvarloader-0.3.3/Cargo.toml
+-rw-r--r--   0     1111     7010     2214 2024-04-29 19:03:18.000000 genvarloader-0.3.3/.gitignore
+-rw-r--r--   0     1111     7010      432 2024-03-15 17:35:16.000000 genvarloader-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0     1111     7010     1066 2024-02-21 06:02:22.000000 genvarloader-0.3.3/LICENSE.txt
+-rw-r--r--   0     1111     7010     2490 2024-02-21 06:02:22.000000 genvarloader-0.3.3/README.md
+-rw-r--r--   0     1111     7010      624 2024-02-21 06:02:22.000000 genvarloader-0.3.3/dev-environment.yml
+-rw-r--r--   0     1111     7010      365 2024-02-21 06:02:22.000000 genvarloader-0.3.3/environment.yml
+-rw-r--r--   0     1111     7010   159221 2024-04-29 18:12:28.000000 genvarloader-0.3.3/poetry.lock
+-rw-r--r--   0     1111     7010      912 2024-04-29 18:12:28.000000 genvarloader-0.3.3/python/genvarloader/__init__.py
+-rw-r--r--   0     1111     7010     3692 2024-04-29 19:03:18.000000 genvarloader-0.3.3/python/genvarloader/__main__.py
+-rw-r--r--   0     1111     7010     6056 2024-04-29 18:12:28.000000 genvarloader-0.3.3/python/genvarloader/bigwig.py
+-rw-r--r--   0     1111     7010      974 2024-04-29 18:12:28.000000 genvarloader-0.3.3/python/genvarloader/concurrent.py
+-rw-r--r--   0     1111     7010    37609 2024-05-31 02:47:46.000000 genvarloader-0.3.3/python/genvarloader/dataset/__init__.py
+-rw-r--r--   0     1111     7010    33937 2024-06-01 17:38:03.000000 genvarloader-0.3.3/python/genvarloader/dataset/genotypes.py
+-rw-r--r--   0     1111     7010     5335 2024-04-29 18:12:28.000000 genvarloader-0.3.3/python/genvarloader/dataset/intervals.py
+-rw-r--r--   0     1111     7010     1679 2024-04-29 18:12:28.000000 genvarloader-0.3.3/python/genvarloader/dataset/reference.py
+-rw-r--r--   0     1111     7010    14850 2024-05-31 20:32:38.000000 genvarloader-0.3.3/python/genvarloader/dataset/tracks.py
+-rw-r--r--   0     1111     7010     4110 2024-04-29 19:03:18.000000 genvarloader-0.3.3/python/genvarloader/dataset/utils.py
+-rw-r--r--   0     1111     7010    16053 2024-06-01 17:54:04.000000 genvarloader-0.3.3/python/genvarloader/dataset/write.py
+-rw-r--r--   0     1111     7010     8343 2024-04-29 19:03:18.000000 genvarloader-0.3.3/python/genvarloader/fasta.py
+-rw-r--r--   0     1111     7010      877 2024-04-29 18:12:28.000000 genvarloader-0.3.3/python/genvarloader/genvarloader.pyi
+-rw-r--r--   0     1111     7010    25831 2024-04-29 18:12:28.000000 genvarloader-0.3.3/python/genvarloader/haplotypes.py
+-rw-r--r--   0     1111     7010    10153 2024-04-29 18:12:28.000000 genvarloader-0.3.3/python/genvarloader/intervals.py
+-rw-r--r--   0     1111     7010    48210 2024-04-29 18:12:28.000000 genvarloader-0.3.3/python/genvarloader/loader.py
+-rw-r--r--   0     1111     7010        0 2024-04-29 18:12:28.000000 genvarloader-0.3.3/python/genvarloader/py.typed
+-rw-r--r--   0     1111     7010     4215 2024-04-29 18:12:28.000000 genvarloader-0.3.3/python/genvarloader/torch.py
+-rw-r--r--   0     1111     7010     8437 2024-04-29 18:12:28.000000 genvarloader-0.3.3/python/genvarloader/types.py
+-rw-r--r--   0     1111     7010    13407 2024-04-29 18:12:28.000000 genvarloader-0.3.3/python/genvarloader/utils.py
+-rw-r--r--   0     1111     7010     9059 2024-05-31 21:27:00.000000 genvarloader-0.3.3/python/genvarloader/variants/__init__.py
+-rw-r--r--   0     1111     7010     9120 2024-04-29 19:03:18.000000 genvarloader-0.3.3/python/genvarloader/variants/genotypes.py
+-rw-r--r--   0     1111     7010    30658 2024-04-29 19:03:18.000000 genvarloader-0.3.3/python/genvarloader/variants/records.py
+-rw-r--r--   0     1111     7010    10433 2024-04-29 18:12:28.000000 genvarloader-0.3.3/python/genvarloader/zarr.py
+-rw-r--r--   0     1111     7010     4206 2024-04-29 18:12:28.000000 genvarloader-0.3.3/src/bigwig.rs
+-rw-r--r--   0     1111     7010     1325 2024-04-29 18:12:28.000000 genvarloader-0.3.3/src/lib.rs
+-rw-r--r--   0     1111     7010     1697 2024-02-21 06:05:07.000000 genvarloader-0.3.3/tests/data/pgen/sample.ends.gvl.arrow
+-rw-r--r--   0     1111     7010     2189 2024-02-21 06:05:07.000000 genvarloader-0.3.3/tests/data/pgen/sample.gvl.arrow
+-rw-r--r--   0     1111     7010       63 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/pgen/sample.pgen
+-rw-r--r--   0     1111     7010       42 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/pgen/sample.psam
+-rw-r--r--   0     1111     7010     2241 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/pgen/sample.pvar
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr0_h1.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr0_h1.fa.fai
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr0_h2.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr0_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr10_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr10_h1.fa.fai
+-rw-r--r--   0     1111     7010       33 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr10_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr10_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr11_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr11_h1.fa.fai
+-rw-r--r--   0     1111     7010       33 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr11_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr11_h2.fa.fai
+-rw-r--r--   0     1111     7010       29 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr1_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr1_h1.fa.fai
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr1_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr1_h2.fa.fai
+-rw-r--r--   0     1111     7010       29 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr2_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr2_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr2_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr2_h2.fa.fai
+-rw-r--r--   0     1111     7010       29 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr3_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr3_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr3_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr3_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr4_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr4_h1.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr4_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr4_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr5_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr5_h1.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr5_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr5_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr6_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr6_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr6_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr6_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr7_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr7_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr7_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr7_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr8_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr8_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr8_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr8_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr9_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr9_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr9_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00001_nr9_h2.fa.fai
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr0_h1.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr0_h1.fa.fai
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr0_h2.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr0_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr10_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr10_h1.fa.fai
+-rw-r--r--   0     1111     7010       33 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr10_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr10_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr11_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr11_h1.fa.fai
+-rw-r--r--   0     1111     7010       33 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr11_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr11_h2.fa.fai
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr1_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr1_h1.fa.fai
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr1_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr1_h2.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr2_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr2_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr2_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr2_h2.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr3_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr3_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr3_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr3_h2.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr4_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr4_h1.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr4_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr4_h2.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr5_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr5_h1.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr5_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr5_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr6_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr6_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr6_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr6_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr7_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr7_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr7_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr7_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr8_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr8_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr8_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr8_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr9_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr9_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr9_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00002_nr9_h2.fa.fai
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr0_h1.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr0_h1.fa.fai
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr0_h2.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr0_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr10_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr10_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr10_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr10_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr11_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr11_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr11_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr11_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr1_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr1_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr1_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr1_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr2_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr2_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr2_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr2_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr3_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr3_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr3_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr3_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr4_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr4_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr4_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr4_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr5_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr5_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr5_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr5_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr6_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr6_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr6_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr6_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr7_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr7_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr7_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr7_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr8_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr8_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr8_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr8_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr9_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr9_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr9_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/consensus/sample_NA00003_nr9_h2.fa.fai
+-rw-r--r--   0     1111     7010     1761 2024-02-27 06:15:30.000000 genvarloader-0.3.3/tests/data/vcf/filtered_sample.ends.gvl.arrow
+-rw-r--r--   0     1111     7010     1997 2024-02-27 06:15:30.000000 genvarloader-0.3.3/tests/data/vcf/filtered_sample.gvl.arrow
+-rw-r--r--   0     1111     7010      223 2024-02-27 06:15:30.000000 genvarloader-0.3.3/tests/data/vcf/filtered_sample.gvl.genos.zarr/.zarray
+-rw-r--r--   0     1111     7010      133 2024-02-27 06:15:30.000000 genvarloader-0.3.3/tests/data/vcf/filtered_sample.gvl.genos.zarr/.zattrs
+-rw-r--r--   0     1111     7010    81381 2024-02-27 06:15:30.000000 genvarloader-0.3.3/tests/data/vcf/filtered_sample.gvl.genos.zarr/0.0.0
+-rw-r--r--   0     1111     7010     2890 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/filtered_sample.vcf
+-rw-r--r--   0     1111     7010     1272 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/filtered_sample.vcf.gz
+-rw-r--r--   0     1111     7010      189 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/filtered_sample.vcf.gz.csi
+-rw-r--r--   0     1111     7010     6218 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/generate_ground_truth.py
+-rw-r--r--   0     1111     7010      212 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/sample.bed
+-rw-r--r--   0     1111     7010     2327 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/data/vcf/sample.vcf
+-rw-r--r--   0     1111     7010     3808 2024-06-01 01:33:54.000000 genvarloader-0.3.3/tests/dataset/genotypes/test_dense2sparse.py
+-rw-r-----   0     1111     7010     4348 2024-05-31 21:08:26.000000 genvarloader-0.3.3/tests/dataset/genotypes/test_reconstruct.py
+-rw-r-----   0     1111     7010     3642 2024-05-31 21:09:30.000000 genvarloader-0.3.3/tests/dataset/test_realign.py
+-rw-r--r--   0     1111     7010     1626 2024-02-27 06:15:30.000000 genvarloader-0.3.3/tests/test_fasta.py
+-rw-r--r--   0     1111     7010     2814 2024-02-27 06:15:30.000000 genvarloader-0.3.3/tests/test_fasta_variants.py
+-rw-r--r--   0     1111     7010     1625 2024-02-27 06:15:30.000000 genvarloader-0.3.3/tests/test_loader.py
+-rw-r--r--   0     1111     7010     3102 2024-04-16 16:39:32.000000 genvarloader-0.3.3/tests/test_max_ends.py
+-rw-r--r--   0     1111     7010     5838 2024-02-21 06:02:23.000000 genvarloader-0.3.3/tests/test_pgen.py
+-rw-r--r--   0     1111     7010      391 2024-04-29 18:12:28.000000 genvarloader-0.3.3/tests/test_utils.py
+-rw-r--r--   0     1111     7010      633 2024-02-27 06:15:30.000000 genvarloader-0.3.3/tests/test_variants.py
+-rw-r--r--   0     1111     7010     3677 2024-04-29 18:12:28.000000 genvarloader-0.3.3/tests/tracks/bench_cpu_gpu.py
+-rw-r--r--   0     1111     7010     3484 2024-04-29 18:12:28.000000 genvarloader-0.3.3/tests/tracks/test_i2t_t2i.py
+-rw-r--r--   0     1111     7010     1000 2024-04-29 18:12:28.000000 genvarloader-0.3.3/tests/tracks/test_random_nonoverlapping.py
+-rw-r--r--   0     1111     7010     2435 2024-04-29 18:12:28.000000 genvarloader-0.3.3/tests/tracks/utils.py
+-rw-r--r--   0     1111     7010    35103 2024-04-29 18:12:28.000000 genvarloader-0.3.3/Cargo.lock
+-rw-r--r--   0     1111     7010     1779 2024-06-01 17:54:27.000000 genvarloader-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3355 1970-01-01 00:00:00.000000 genvarloader-0.3.3/PKG-INFO
```

### Comparing `genvarloader-0.3.2/.gitignore` & `genvarloader-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/LICENSE.txt` & `genvarloader-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/README.md` & `genvarloader-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/dev-environment.yml` & `genvarloader-0.3.3/dev-environment.yml`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/poetry.lock` & `genvarloader-0.3.3/poetry.lock`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/__init__.py` & `genvarloader-0.3.3/python/genvarloader/__init__.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/__main__.py` & `genvarloader-0.3.3/python/genvarloader/__main__.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/bigwig.py` & `genvarloader-0.3.3/python/genvarloader/bigwig.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/concurrent.py` & `genvarloader-0.3.3/python/genvarloader/concurrent.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/dataset/__init__.py` & `genvarloader-0.3.3/python/genvarloader/dataset/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -872,15 +872,15 @@
         diffs = get_diffs_sparse(
             geno_offset_idx,
             self.genotypes.variant_idxs,
             self.genotypes.offsets,
             self.variants.sizes,
         )
         # (b p)
-        shifts = self.rng.integers(0, diffs + 1, dtype=np.int32)
+        shifts = self.rng.integers(0, -diffs.clip(max=0) + 1, dtype=np.int32)
         return shifts
 
     def get_haplotypes(
         self,
         geno_offset_idx: NDArray[np.intp],
         region_idx: NDArray[np.intp],
         shifts: NDArray[np.int32],
@@ -1014,10 +1014,25 @@
             raise ImportError(
                 "Could not import PyTorch. Please install PyTorch to use torch features."
             )
 
     def __len__(self) -> int:
         return len(self.dataset)
 
-    def __getitem__(self, idx: Idx) -> Union[NDArray, Tuple[NDArray, ...]]:
+    def __getitem__(
+        self, idx: Idx
+    ) -> Union["torch.Tensor", Tuple["torch.Tensor", ...], Any]:
         batch = self.dataset[idx]
+        if isinstance(batch, np.ndarray):
+            batch = _tensor_from_maybe_bytes(batch)
+        elif isinstance(batch, tuple):
+            batch = tuple(_tensor_from_maybe_bytes(b) for b in batch)
         return batch
+
+
+def _tensor_from_maybe_bytes(array: NDArray) -> "torch.Tensor":
+    if TYPE_CHECKING:
+        import torch
+
+    if array.dtype == np.bytes_:
+        array = array.view(np.uint8)
+    return torch.from_numpy(array)
```

### Comparing `genvarloader-0.3.2/python/genvarloader/dataset/genotypes.py` & `genvarloader-0.3.3/python/genvarloader/dataset/genotypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Tuple, cast
+from typing import Tuple
 
 import numba as nb
 import numpy as np
 from attrs import define
 from numpy.typing import NDArray
 
 from ..types import ListIdx
 from ..utils import lengths_to_offsets
-from .utils import padded_slice, reduceat_offsets
+from .utils import padded_slice
 
 
 @define
 class DenseGenotypes:
     """Dense genotypes. In this format, genotypes are stored as a special case of a ragged 3D array where
     each sample has the same number of variants, but each region may have a different number of variants.
     Thus, the first variant indices are the same for every sample, and the offsets are readily computed
@@ -28,16 +28,16 @@
     offsets : NDArray[np.uint32]
         Shape = (n_regions + 1,) Offsets into genos.
     n_samples : int
         Number of samples.
     """
 
     genos: NDArray[np.int8]  # (n_samples * n_variants, ploidy)
-    first_v_idxs: NDArray[np.uint32]  # (n_regions)
-    offsets: NDArray[np.uint32]  # (n_regions + 1)
+    first_v_idxs: NDArray[np.int32]  # (n_regions)
+    offsets: NDArray[np.int32]  # (n_regions + 1)
     n_samples: int
 
     @property
     def n_regions(self) -> int:
         return len(self.first_v_idxs)
 
     @property
@@ -239,15 +239,15 @@
             positions,
             ilens,
             starts,
             length,
         )
         # (r)
         max_ends: NDArray[np.int32] = starts + length - min_ilens.clip(max=0)
-        # tuple s p v
+        # (r s p)
         n_per_rsp = get_n_per_rsp(keep, offsets, n_regions)
         sparse_offsets = lengths_to_offsets(n_per_rsp.ravel(), np.int32)
         variant_idxs = keep_mask_to_rsp_v_idx(
             keep, first_v_idxs, offsets, sparse_offsets, n_regions, n_samples, ploidy
         )
         sparse_genos = cls(
             variant_idxs=variant_idxs,
@@ -255,31 +255,14 @@
             n_regions=n_regions,
             n_samples=n_samples,
             ploidy=ploidy,
         )
         return sparse_genos, max_ends
 
 
-def get_haplotype_ilens(
-    genos: NDArray[np.int8],
-    first_v_idxs: NDArray[np.int32],
-    offsets: NDArray[np.int32],
-    ilens: NDArray[np.int32],
-):
-    # (r)
-    n_per_region = np.diff(offsets)
-    # (v)
-    dense_v_idxs = first_v_idxs_to_all_v_idxs(first_v_idxs, n_per_region)
-    # (s p v)
-    spv_ilens = cast(NDArray[np.int32], np.where(genos == 1, ilens[dense_v_idxs], 0))
-    # (s p r)
-    r_ilens = reduceat_offsets(np.add, spv_ilens, offsets, -1)
-    return spv_ilens, r_ilens
-
-
 @nb.njit(parallel=True, nogil=True, cache=True)
 def get_haplotype_region_ilens(
     genos: NDArray[np.int8],
     first_v_idxs: NDArray[np.int32],
     offsets: NDArray[np.int32],
     ilens: NDArray[np.int32],
 ):
@@ -332,34 +315,36 @@
     length : int
         Length of haplotypes.
     """
     n_samples = genos.shape[0]
     ploidy = genos.shape[1]
     n_regions = len(starts)
     keep = np.empty_like(genos, np.bool_)
-    min_ilens = np.empty(n_regions, np.int32)
+    min_ilens = np.zeros(n_regions, np.int32)
     for r in nb.prange(n_regions):
         o_s, o_e = offsets[r], offsets[r + 1]
         n_variants = o_e - o_s
         if n_variants == 0:
             continue
         r_start = starts[r]
+        _ilens = np.empty((n_samples, ploidy), np.int32)
         for s in nb.prange(n_samples):
             for p in nb.prange(ploidy):
                 cum_ilen = 0
                 for v in range(o_s, o_e):
                     v_idx = first_v_idxs[r] + v - o_s
                     rel_pos = positions[v_idx] - r_start
                     ilen = ilens[v_idx]
                     if rel_pos + cum_ilen + ilen < length and genos[s, p, v] == 1:
                         cum_ilen += ilen
                         keep[s, p, v] = True
                     else:
                         keep[s, p, v] = False
-                min_ilens[r] = min(min_ilens[r], cum_ilen)
+                _ilens[s, p] = cum_ilen
+        min_ilens[r] = _ilens.min()
     return keep, min_ilens
 
 
 @nb.njit(parallel=True, nogil=True, cache=True)
 def get_n_per_rsp(keep: NDArray[np.bool_], offsets: NDArray[np.int32], n_regions: int):
     n_samples, ploidy, _ = keep.shape
     n_per_rsp = np.empty((n_regions, n_samples, ploidy), np.int32)
@@ -776,34 +761,33 @@
     n_regions = out.shape[0]
     ploidy = out.shape[1]
     for query in nb.prange(n_regions):
         q = regions[query]
         c_idx = q[0]
         c_s = ref_offsets[c_idx]
         c_e = ref_offsets[c_idx + 1]
-        ref_s = q[1]
-        ref_e = q[2]
-        _ref = padded_slice(ref[c_s:c_e], ref_s, ref_e, pad_char)
+        ref_start = q[1]
+        _reference = ref[c_s:c_e]
 
         for hap in nb.prange(ploidy):
             o_idx = offset_idx[query, hap]
             _out = out[query, hap]
-            _shifts = shifts[query, hap]
+            shift = shifts[query, hap]
 
             reconstruct_haplotype_from_sparse(
                 o_idx,
                 sparse_genos,
                 offsets,
                 positions,
                 sizes,
-                _shifts,
+                shift,
                 alt_alleles,
                 alt_offsets,
-                _ref,
-                ref_s,
+                _reference,
+                ref_start + shift,  # shift ref_start as well
                 _out,
                 pad_char,
             )
 
 
 @nb.njit(nogil=True, cache=True)
 def reconstruct_haplotype_from_sparse(
@@ -811,120 +795,101 @@
     variant_idxs: NDArray[np.int32],
     offsets: NDArray[np.int32],
     positions: NDArray[np.int32],
     sizes: NDArray[np.int32],
     shift: int,
     alt_alleles: NDArray[np.uint8],  # full set
     alt_offsets: NDArray[np.uintp],  # full set
-    ref: NDArray[np.uint8],
-    ref_start: int,
+    ref: NDArray[np.uint8],  # full contig
+    ref_start: int,  # may be negative
     out: NDArray[np.uint8],
     pad_char: int,
 ):
     """Reconstruct a haplotype from reference sequence and variants.
 
     Parameters
     ----------
-    sample_idx : int
-        Sample index.
-    ploid : int
-        Ploidy.
-    region_idx : int
-        Region index.
-    variant_idxs : NDArray[np.int8]
-        Shape = (variants) Genotypes of variants.
+    offset_idx : int
+        Index for `offsets` for where to find the offsets into variant_idxs.
+    variant_idxs : int
+        Index of alt variants for all samples and variants.
     offsets : NDArray[np.int32]
         Shape = (samples*ploidy*regions + 1) Offsets into variant indices.
     positions : NDArray[np.int32]
         Shape = (total_variants) Positions of variants.
     sizes : NDArray[np.int32]
         Shape = (total_variants) Sizes of variants.
     shift : int
-        Shift amount.
+        Total amount to shift by.
     alt_alleles : NDArray[np.uint8]
         Shape = (total_alt_length) ALT alleles.
     alt_offsets : NDArray[np.uintp]
         Shape = (total_variants + 1) Offsets of ALT alleles.
     ref : NDArray[np.uint8]
-        Shape = (ref_length) Reference sequence. ref_length >= out_length
+        Shape = (ref_length) Reference sequence for the whole contig. ref_length >= out_length
     ref_start : int
-        Start position of reference sequence.
+        Start position of reference sequence, may be negative.
     out : NDArray[np.uint8]
         Shape = (out_length) Output array.
     pad_char : int
         Padding character.
     """
     _variant_idxs = variant_idxs[offsets[offset_idx] : offsets[offset_idx + 1]]
     length = len(out)
     n_variants = len(_variant_idxs)
-    if n_variants == 0:
-        out[:] = ref[:length]
-        return
 
     # where to get next reference subsequence
-    ref_idx = 0
+    ref_idx = ref_start
     # where to put next subsequence
     out_idx = 0
-    # total amount to shift by
-    shift = shift
     # how much we've shifted
     shifted = 0
 
-    # first variant is a DEL spanning start
-    v_rel_pos = positions[_variant_idxs[0]] - ref_start
-    v_diff = sizes[_variant_idxs[0]]
-    if v_rel_pos < 0:
-        # diff of v(-1) has been normalized to consider where ref is
-        # otherwise, ref_idx = v_rel_pos - v_diff + 1
-        # e.g. a -10 diff became -3 if v_rel_pos = -7
-        ref_idx = v_rel_pos - v_diff + 1
-        # increment the variant index
-        start_idx = 1
-    else:
-        start_idx = 0
-
-    for v in range(start_idx, n_variants):
+    for v in range(n_variants):
         variant: np.int32 = _variant_idxs[v]
-        # position of variant relative to ref from fetch(contig, start, q_end)
-        # i.e. has been put into same coordinate system as ref_idx
-        v_rel_pos = positions[variant] - ref_start
+        v_pos = positions[variant]
+        v_diff = sizes[variant]
+
+        # if first variant is a DEL spanning start of query
+        if v == 0 and v_pos < ref_start and v_diff < 0:
+            ref_idx = v_pos - v_diff + 1
+            continue
 
         # overlapping variants
         # v_rel_pos < ref_idx only if we see an ALT at a given position a second
         # time or more. We'll do what bcftools consensus does and only use the
         # first ALT variant we find.
-        if v_rel_pos < ref_idx:
+        if v_pos < ref_idx:
             continue
 
-        v_diff = sizes[variant]
         allele = alt_alleles[alt_offsets[variant] : alt_offsets[variant + 1]]
         v_len = len(allele)
 
         # handle shift
         if shifted < shift:
-            ref_shift_dist = v_rel_pos - ref_idx
+            ref_shift_dist = v_pos - ref_idx
             # not enough distance to finish the shift even with the variant
             if shifted + ref_shift_dist + v_len < shift:
                 # consume ref up to the end of the variant
-                ref_idx = v_rel_pos + 1
+                ref_idx = v_pos + 1
                 # add the length of skipped ref and size of the variant to the shift
                 shifted += ref_shift_dist + v_len
                 # skip the variant
                 continue
             # enough distance between ref_idx and variant to finish shift
             elif shifted + ref_shift_dist >= shift:
                 ref_idx += shift - shifted
                 shifted = shift
                 # can still use the variant and whatever ref is left between
                 # ref_idx and the variant
             # ref + (some of) variant is enough to finish shift
             else:
                 # consume ref up to beginning of variant
                 # ref_idx will be moved to end of variant after using the variant
-                ref_idx = v_rel_pos
+                ref_idx = v_pos
                 # how much left to shift - amount of ref we can use
                 allele_start_idx = shift - shifted - ref_shift_dist
                 #! without if statement, parallel=True can cause a SystemError!
                 # * parallel jit cannot handle changes in array dimension.
                 # * without this, allele can change from a 1D array to a 0D
                 # * array.
                 # enough dist with variant to complete shift
@@ -932,40 +897,54 @@
                     continue
                 allele = allele[allele_start_idx:]
                 v_len = len(allele)
                 # done shifting
                 shifted = shift
 
         # add reference sequence
-        ref_len = v_rel_pos - ref_idx
+        ref_len = v_pos - ref_idx
         if out_idx + ref_len >= length:
             # ref will get written by final clause
             # handles case where extraneous variants downstream of the haplotype were provided
             break
+        if ref_idx < 0:
+            pad_len = -ref_idx
+            out[out_idx : out_idx + pad_len] = pad_char
+            out_idx += pad_len
+            ref_idx = 0
+            ref_len -= pad_len
         out[out_idx : out_idx + ref_len] = ref[ref_idx : ref_idx + ref_len]
         out_idx += ref_len
 
         # insertions + substitions
         writable_length = min(v_len, length - out_idx)
         out[out_idx : out_idx + writable_length] = allele[:writable_length]
         out_idx += writable_length
         # +1 because ALT alleles always replace 1 nt of reference for a
         # normalized VCF
-        ref_idx = v_rel_pos + 1
+        ref_idx = v_pos + 1
 
         # deletions, move ref to end of deletion
         if v_diff < 0:
             ref_idx -= v_diff
 
         if out_idx >= length:
             break
 
     # fill rest with reference sequence and pad with Ns
     unfilled_length = length - out_idx
     if unfilled_length > 0:
+        # if ref_idx is negative, we need to pad the beginning of the haplotype
+        # can occur if there are 0 variants and the start of the query is < 0
+        if ref_idx < 0:
+            pad_len = -ref_idx
+            out[out_idx : out_idx + pad_len] = pad_char
+            out_idx += pad_len
+            ref_idx = 0
+
         writable_ref = min(unfilled_length, len(ref) - ref_idx)
         out_end_idx = out_idx + writable_ref
         ref_end_idx = ref_idx + writable_ref
         out[out_idx:out_end_idx] = ref[ref_idx:ref_end_idx]
 
         if out_end_idx < length:
             out[out_end_idx:] = pad_char
```

### Comparing `genvarloader-0.3.2/python/genvarloader/dataset/intervals.py` & `genvarloader-0.3.3/python/genvarloader/dataset/intervals.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/dataset/reference.py` & `genvarloader-0.3.3/python/genvarloader/dataset/reference.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/dataset/tracks.py` & `genvarloader-0.3.3/python/genvarloader/dataset/tracks.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,52 +304,45 @@
     out : NDArray[np.uint8]
         Shape = (out_length) Shifted and re-aligned track.
     """
     _variant_idxs = variant_idxs[offsets[offset_idx] : offsets[offset_idx + 1]]
     length = len(out)
     n_variants = len(_variant_idxs)
     if n_variants == 0:
-        out[:] = track[:length]
+        # track must have length >= max(shif0)t + length
+        out[:] = track[shift : shift + length]
         return
     # where to get next reference subsequence
     track_idx = 0
     # where to put next subsequence
     out_idx = 0
     # how much we've shifted
     shifted = 0
 
-    # first variant is a DEL spanning start
-    v_rel_pos = positions[_variant_idxs[0]] - query_start
-    v_diff = sizes[_variant_idxs[0]]
-    if v_rel_pos < 0:
-        # diff of v(-1) has been normalized to consider where ref is
-        # otherwise, ref_idx = v_rel_pos - v_diff + 1
-        # e.g. a -10 diff became -3 if v_rel_pos = -7
-        track_idx = v_rel_pos - v_diff + 1
-        # increment the variant index
-        start_idx = 1
-    else:
-        start_idx = 0
-
-    for v in range(start_idx, n_variants):
+    for v in range(n_variants):
         variant: np.int32 = _variant_idxs[v]
 
         # position of variant relative to ref from fetch(contig, start, q_end)
         # i.e. has been put into same coordinate system as ref_idx
         v_rel_pos = positions[variant] - query_start
+        v_diff = sizes[variant]
+
+        # first variant is a DEL spanning start
+        if v == 0 and v_rel_pos < 0 and v_diff < 0:
+            track_idx = v_rel_pos - v_diff + 1
+            continue
 
         # overlapping variants
         # v_rel_pos < ref_idx only if we see an ALT at a given position a second
         # time or more. We'll do what bcftools consensus does and only use the
         # first ALT variant we find.
         if v_rel_pos < track_idx:
             continue
 
-        v_diff = sizes[variant]
-        # ok to do this before shift because there must be at least one nonzero diff if shift > 0
+        # ok to do this before shift because there must be at least one positive diff since 0 < shift < sum(v_diff)
         if v_diff == 0:
             continue
         v_len = max(1, v_diff + 1)
         value = track[v_rel_pos]
 
         # handle shift
         if shifted < shift:
@@ -390,23 +383,23 @@
         if out_idx + track_len >= length:
             # track will get written by final clause
             # handles case where extraneous variants downstream of the haplotype were provided
             break
         out[out_idx : out_idx + track_len] = track[track_idx : track_idx + track_len]
         out_idx += track_len
 
-        # insertions + substitions
+        # insertions (substitutions are skipped above)
         writable_length = min(v_len, length - out_idx)
         out[out_idx : out_idx + writable_length] = value
         out_idx += writable_length
         # +1 because ALT alleles always replace 1 nt of reference for a
         # normalized VCF
         track_idx = v_rel_pos + 1
 
-        # deletions, move ref to end of deletion
+        # deletions, move track to end of deletion
         if v_diff < 0:
             track_idx -= v_diff
 
         if out_idx >= length:
             break
 
     # fill rest with track and pad with 0
```

### Comparing `genvarloader-0.3.2/python/genvarloader/dataset/utils.py` & `genvarloader-0.3.3/python/genvarloader/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/dataset/write.py` & `genvarloader-0.3.3/python/genvarloader/dataset/write.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
         if isinstance(variants.genotypes, VCFGenos):
             variants.genotypes.close()
         metadata["ploidy"] = variants.ploidy
         # free memory
         del variants
         gc.collect()
 
+    logger.info("Writing regions.")
     write_regions(path, bed, contigs)
 
     if bigwigs is not None:
         logger.info("Writing BigWig intervals.")
         for bw in bigwigs:
             write_bigwigs(path, bed, bw, samples)
 
@@ -307,44 +308,46 @@
     return bed
 
 
 def read_variants_chunk(
     contig: Optional[str],
     starts: NDArray[np.int32],
     ends: NDArray[np.int32],
-    rel_s_idx: NDArray[np.int32],
-    rel_e_idx: NDArray[np.int32],
+    rel_s_idxs: NDArray[np.int32],
+    rel_e_idxs: NDArray[np.int32],
     variants: Variants,
     region_length: int,
     samples: List[str],
-    sample_idx: Optional[NDArray[np.intp]],
+    sample_idxs: Optional[NDArray[np.intp]],
 ):
     if contig is None:
         genos = SparseGenotypes.empty(
-            n_regions=len(rel_s_idx), n_samples=len(samples), ploidy=variants.ploidy
+            n_regions=len(rel_s_idxs), n_samples=len(samples), ploidy=variants.ploidy
         )
         chunk_max_ends = ends
     else:
         first = True
         while True:
             logger.debug(f"region length {ends[0] - starts[0]}")
             if not first:
-                rel_e_idx = variants.records.find_relative_end_idx(contig, ends)
-            s_idx = variants.records.contig_offsets[contig] + rel_s_idx
-            e_idx = variants.records.contig_offsets[contig] + rel_e_idx
+                rel_e_idxs = variants.records.find_relative_end_idx(contig, ends)
+            s_idx = variants.records.contig_offsets[contig] + rel_s_idxs
+            e_idx = variants.records.contig_offsets[contig] + rel_e_idxs
             # (s p v)
             logger.debug("read genotypes")
-            genos = variants.genotypes.read(contig, s_idx, e_idx, sample_idx=sample_idx)
+            genos = variants.genotypes.read(
+                contig, s_idx, e_idx, sample_idx=sample_idxs
+            )
             n_per_region = e_idx - s_idx
             offsets = lengths_to_offsets(n_per_region)
 
             logger.debug("get haplotype region ilens")
             # (s p r)
             haplotype_ilens = get_haplotype_region_ilens(
-                genos, rel_s_idx, offsets, variants.records.v_diffs[contig]
+                genos, rel_s_idxs, offsets, variants.records.v_diffs[contig]
             )
             haplotype_lengths = ends - starts + haplotype_ilens
             logger.debug(f"average haplotype length {haplotype_lengths.mean()}")
             # (s p r)
             missing_length = region_length - haplotype_lengths
             logger.debug(f"max missing length {missing_length.max()}")
 
@@ -355,21 +358,23 @@
             ends += np.ceil(
                 EXTEND_END_MULTIPLIER * missing_length.max((0, 1)).clip(min=0)
             ).astype(np.int32)
 
         logger.debug("sparsify genotypes")
         genos, chunk_max_ends = SparseGenotypes.from_dense_with_length(
             genos=genos,
-            first_v_idxs=rel_s_idx,
+            first_v_idxs=rel_s_idxs,
             offsets=offsets,
             ilens=variants.records.v_diffs[contig],
             positions=variants.records.v_starts[contig],
             starts=starts,
             length=region_length,
         )
+        logger.debug(f"maximum needed length {(chunk_max_ends - starts).max()}")
+        logger.debug(f"minimum needed length {(chunk_max_ends - starts).min()}")
 
         # make indices absolute
         genos.variant_idxs += variants.records.contig_offsets[contig]
     return genos, chunk_max_ends
 
 
 def write_variants_chunk(
```

### Comparing `genvarloader-0.3.2/python/genvarloader/fasta.py` & `genvarloader-0.3.3/python/genvarloader/fasta.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/genvarloader.pyi` & `genvarloader-0.3.3/python/genvarloader/genvarloader.pyi`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/haplotypes.py` & `genvarloader-0.3.3/python/genvarloader/haplotypes.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/intervals.py` & `genvarloader-0.3.3/python/genvarloader/intervals.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/loader.py` & `genvarloader-0.3.3/python/genvarloader/loader.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/torch.py` & `genvarloader-0.3.3/python/genvarloader/torch.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/types.py` & `genvarloader-0.3.3/python/genvarloader/types.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/utils.py` & `genvarloader-0.3.3/python/genvarloader/utils.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/variants/__init__.py` & `genvarloader-0.3.3/python/genvarloader/variants/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from pathlib import Path
 from typing import Dict, Optional, Tuple, Union
 
 import numpy as np
 import polars as pl
 from attrs import define
 from numpy.typing import ArrayLike, NDArray
@@ -62,15 +63,17 @@
     def from_file(cls, path: Union[str, Path, Dict[str, Path]]):
         if isinstance(path, (str, Path)):
             path = Path(path)
             first_path = path
         elif isinstance(path, dict):
             first_path = next(iter(path.values()))
 
-        if first_path.suffix == ".vcf":
+        vcf_suffix = re.compile(r"\.[vb]cf(\.gz)?$")
+
+        if vcf_suffix.search(first_path.suffix):
             return cls.from_vcf(path)
         elif first_path.suffix == ".pgen":
             return cls.from_pgen(path)
         else:
             raise ValueError("Unsupported file type.")
 
     @property
```

### Comparing `genvarloader-0.3.2/python/genvarloader/variants/genotypes.py` & `genvarloader-0.3.3/python/genvarloader/variants/genotypes.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/variants/records.py` & `genvarloader-0.3.3/python/genvarloader/variants/records.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/python/genvarloader/zarr.py` & `genvarloader-0.3.3/python/genvarloader/zarr.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/src/bigwig.rs` & `genvarloader-0.3.3/src/bigwig.rs`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/src/lib.rs` & `genvarloader-0.3.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/data/pgen/sample.ends.gvl.arrow` & `genvarloader-0.3.3/tests/data/pgen/sample.ends.gvl.arrow`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/data/pgen/sample.gvl.arrow` & `genvarloader-0.3.3/tests/data/pgen/sample.gvl.arrow`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/data/pgen/sample.pvar` & `genvarloader-0.3.3/tests/data/pgen/sample.pvar`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/data/vcf/filtered_sample.ends.gvl.arrow` & `genvarloader-0.3.3/tests/data/vcf/filtered_sample.ends.gvl.arrow`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/data/vcf/filtered_sample.gvl.arrow` & `genvarloader-0.3.3/tests/data/vcf/filtered_sample.gvl.arrow`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/data/vcf/filtered_sample.gvl.genos.zarr/0.0.0` & `genvarloader-0.3.3/tests/data/vcf/filtered_sample.gvl.genos.zarr/0.0.0`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/data/vcf/filtered_sample.vcf` & `genvarloader-0.3.3/tests/data/vcf/filtered_sample.vcf`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/data/vcf/filtered_sample.vcf.gz` & `genvarloader-0.3.3/tests/data/vcf/filtered_sample.vcf.gz`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/data/vcf/generate_ground_truth.py` & `genvarloader-0.3.3/tests/data/vcf/generate_ground_truth.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/data/vcf/sample.vcf` & `genvarloader-0.3.3/tests/data/vcf/sample.vcf`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/test_fasta.py` & `genvarloader-0.3.3/tests/test_fasta.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/test_fasta_variants.py` & `genvarloader-0.3.3/tests/test_fasta_variants.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/test_loader.py` & `genvarloader-0.3.3/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/test_max_ends.py` & `genvarloader-0.3.3/tests/test_max_ends.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/test_pgen.py` & `genvarloader-0.3.3/tests/test_pgen.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/test_variants.py` & `genvarloader-0.3.3/tests/test_variants.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/tracks/bench_cpu_gpu.py` & `genvarloader-0.3.3/tests/tracks/bench_cpu_gpu.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/tracks/test_i2t_t2i.py` & `genvarloader-0.3.3/tests/tracks/test_i2t_t2i.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/tracks/test_random_nonoverlapping.py` & `genvarloader-0.3.3/tests/tracks/test_random_nonoverlapping.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/tests/tracks/utils.py` & `genvarloader-0.3.3/tests/tracks/utils.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/Cargo.lock` & `genvarloader-0.3.3/Cargo.lock`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.2/pyproject.toml` & `genvarloader-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "genvarloader"
-version = "0.3.2"
+version = "0.3.3"
 description = "Pipeline for efficient genomic data processing."
 authors = [
     { name = "David Laub", email = "dlaub@ucsd.edu" },
     { name = "Aaron Ho", email = "aho@salk.edu" },
 ]
 readme = "README.md"
 repository = "https://github.com/mcvickerlab/genome-loader"
@@ -46,15 +46,15 @@
     "py-spy>=0.3.14",
     "icecream>=2.1.3",
     "pytest-cases>=3.8.0",
     "pytest-cov>=4.1.0",
     "ruff>=0.0.292",
     "pre-commit>=3.5.0",
     "pytest-benchmark>=4.0.0",
-    "filelock>=3.13.1"
+    "filelock>=3.13.1",
 ]
 
 [tool.mypy]
 plugins = ["numpy.typing.mypy_plugin", "pandera.mypy"]
 
 [tool.ruff]
 lint.ignore = ["E501"]
```

### Comparing `genvarloader-0.3.2/PKG-INFO` & `genvarloader-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: genvarloader
-Version: 0.3.2
+Version: 0.3.3
 Requires-Dist: pytest >=7.4.2 ; extra == 'dev'
 Requires-Dist: mypy >=1.6.0 ; extra == 'dev'
 Requires-Dist: memray >=1.10.0 ; extra == 'dev'
 Requires-Dist: py-spy >=0.3.14 ; extra == 'dev'
 Requires-Dist: icecream >=2.1.3 ; extra == 'dev'
 Requires-Dist: pytest-cases >=3.8.0 ; extra == 'dev'
 Requires-Dist: pytest-cov >=4.1.0 ; extra == 'dev'
```

