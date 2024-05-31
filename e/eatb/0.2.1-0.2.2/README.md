# Comparing `tmp/eatb-0.2.1.tar.gz` & `tmp/eatb-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eatb-0.2.1.tar", last modified: Fri Apr 12 11:11:54 2024, max compression
+gzip compressed data, was "eatb-0.2.2.tar", last modified: Fri May 31 22:44:55 2024, max compression
```

## Comparing `eatb-0.2.1.tar` & `eatb-0.2.2.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:54.500496 eatb-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-12 11:11:49.000000 eatb-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-12 11:11:49.000000 eatb-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-12 11:11:54.500496 eatb-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-12 11:11:49.000000 eatb-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:54.484496 eatb-0.2.1/eatb/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/csip_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/file_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/ipstate.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/logging_config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:54.488496 eatb-0.2.1/eatb/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/metadata/dip_parsed_premis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/metadata/ead.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/metadata/mets.py
--rw-r--r--   0 runner    (1001) docker     (127)    26379 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/metadata/mets_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/metadata/mets_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/metadata/parsed_dcat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/metadata/parsed_ead.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/metadata/parsed_mets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/metadata/parsed_premis.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/metadata/premis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/metadata/premis_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13294 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/metadata/premis_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46968 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/oais_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/package_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)    15251 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/pairtree_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:54.488496 eatb-0.2.1/eatb/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/resources/default_commands.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:54.492496 eatb-0.2.1/eatb/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/resources/schemas/DILCISExtensionMETS.xsd
--rwxr-xr-x   0 runner    (1001) docker     (127)     2033 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/resources/schemas/DILCISExtensionMETS.xsd.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)   125569 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/resources/schemas/E-ARK-CSIP-v2-0-4.xml
--rw-r--r--   0 runner    (1001) docker     (127)   145565 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/resources/schemas/IP.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/resources/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/resources/schemas/csip.xsd
--rwxr-xr-x   0 runner    (1001) docker     (127)   133920 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/resources/schemas/mets.xsd
--rw-r--r--   0 runner    (1001) docker     (127)   133018 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/resources/schemas/mets_1_11.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    65126 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/resources/schemas/premis-v2-2.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/resources/schemas/xlink.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/resources/validation_rules.xml
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/settings.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:54.492496 eatb-0.2.1/eatb/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/utils/XmlHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/utils/dictutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/utils/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)    18051 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/utils/fileutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/utils/listhandling.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/utils/randomutils.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/utils/reporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/utils/stringutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/utils/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-04-12 11:11:49.000000 eatb-0.2.1/eatb/utils/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:54.500496 eatb-0.2.1/eatb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-12 11:11:54.000000 eatb-0.2.1/eatb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-12 11:11:54.000000 eatb-0.2.1/eatb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:11:54.000000 eatb-0.2.1/eatb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:11:54.000000 eatb-0.2.1/eatb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 11:11:54.000000 eatb-0.2.1/eatb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-12 11:11:54.500496 eatb-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-12 11:11:49.000000 eatb-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:54.496496 eatb-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/dip_premis_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_csip_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_filehandling.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_formatidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_metadata_dcat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_metadata_ead.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_mets_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_mets_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    15220 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_mets_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_pairtreestorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_parsed_mets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_premis_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_premis_manipulate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_stringutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_tarentryreader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_unzip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-12 11:11:49.000000 eatb-0.2.1/tests/test_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:44:55.236808 eatb-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-31 22:44:50.000000 eatb-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-31 22:44:50.000000 eatb-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-31 22:44:55.236808 eatb-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-31 22:44:50.000000 eatb-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:44:55.220808 eatb-0.2.2/eatb/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/csip_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/file_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/ipstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/logging_config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:44:55.224808 eatb-0.2.2/eatb/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/metadata/dip_parsed_premis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/metadata/ead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/metadata/mets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26379 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/metadata/mets_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/metadata/mets_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/metadata/parsed_dcat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/metadata/parsed_ead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/metadata/parsed_mets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/metadata/parsed_premis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/metadata/premis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/metadata/premis_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13294 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/metadata/premis_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46968 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/oais_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/package_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15251 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/pairtree_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:44:55.224808 eatb-0.2.2/eatb/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/resources/default_commands.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:44:55.228808 eatb-0.2.2/eatb/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/resources/schemas/DILCISExtensionMETS.xsd
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2033 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/resources/schemas/DILCISExtensionMETS.xsd.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   125569 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/resources/schemas/E-ARK-CSIP-v2-0-4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   145565 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/resources/schemas/IP.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/resources/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/resources/schemas/csip.xsd
+-rwxr-xr-x   0 runner    (1001) docker     (127)   133920 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/resources/schemas/mets.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)   133018 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/resources/schemas/mets_1_11.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    65126 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/resources/schemas/premis-v2-2.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    52845 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/resources/schemas/premis-v3-0.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/resources/schemas/xlink.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/resources/validation_rules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/settings.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:44:55.228808 eatb-0.2.2/eatb/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/utils/XmlHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/utils/dictutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/utils/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18226 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/utils/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/utils/listhandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/utils/randomutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/utils/reporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/utils/stringutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/utils/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-31 22:44:50.000000 eatb-0.2.2/eatb/utils/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:44:55.232808 eatb-0.2.2/eatb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-31 22:44:55.000000 eatb-0.2.2/eatb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-31 22:44:55.000000 eatb-0.2.2/eatb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:44:55.000000 eatb-0.2.2/eatb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:44:55.000000 eatb-0.2.2/eatb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 22:44:55.000000 eatb-0.2.2/eatb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-31 22:44:55.236808 eatb-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-31 22:44:50.000000 eatb-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:44:55.232808 eatb-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/dip_premis_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_csip_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_filehandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_formatidentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_metadata_dcat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_metadata_ead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_mets_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_mets_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15220 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_mets_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_pairtreestorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_parsed_mets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_premis_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_premis_manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_stringutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_tarentryreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_unzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-31 22:44:50.000000 eatb-0.2.2/tests/test_xml.py
```

### Comparing `eatb-0.2.1/LICENSE` & `eatb-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/PKG-INFO` & `eatb-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eatb
-Version: 0.2.1
+Version: 0.2.2
 Summary: A suite of tools for the creation of information packages for archival purposes.
 Home-page: https://www.e-ark-foundation.eu/e-ark-software-eatb
 Author: E-ARK Foundation
 Author-email: admin@e-ark-foundation.eu
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eatb-0.2.1/README.md` & `eatb-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/checksum.py` & `eatb-0.2.2/eatb/checksum.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/cli.py` & `eatb-0.2.2/eatb/cli.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/csip_validation.py` & `eatb-0.2.2/eatb/csip_validation.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/file_format.py` & `eatb-0.2.2/eatb/file_format.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/ipstate.py` & `eatb-0.2.2/eatb/ipstate.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/metadata/__init__.py` & `eatb-0.2.2/eatb/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/metadata/dip_parsed_premis.py` & `eatb-0.2.2/eatb/metadata/dip_parsed_premis.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/metadata/ead.py` & `eatb-0.2.2/eatb/metadata/ead.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/metadata/mets.py` & `eatb-0.2.2/eatb/metadata/mets.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/metadata/mets_generator.py` & `eatb-0.2.2/eatb/metadata/mets_generator.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/metadata/mets_validation.py` & `eatb-0.2.2/eatb/metadata/mets_validation.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/metadata/parsed_dcat.py` & `eatb-0.2.2/eatb/metadata/parsed_dcat.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/metadata/parsed_ead.py` & `eatb-0.2.2/eatb/metadata/parsed_ead.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/metadata/parsed_mets.py` & `eatb-0.2.2/eatb/metadata/parsed_mets.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/metadata/parsed_premis.py` & `eatb-0.2.2/eatb/metadata/parsed_premis.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/metadata/premis.py` & `eatb-0.2.2/eatb/metadata/premis.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/metadata/premis_creator.py` & `eatb-0.2.2/eatb/metadata/premis_creator.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/metadata/premis_generator.py` & `eatb-0.2.2/eatb/metadata/premis_generator.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/oais_ip.py` & `eatb-0.2.2/eatb/oais_ip.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/package_creator.py` & `eatb-0.2.2/eatb/package_creator.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/packaging.py` & `eatb-0.2.2/eatb/packaging.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/pairtree_storage.py` & `eatb-0.2.2/eatb/pairtree_storage.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/resources/default_commands.cfg` & `eatb-0.2.2/eatb/resources/default_commands.cfg`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/resources/schemas/DILCISExtensionMETS.xsd` & `eatb-0.2.2/eatb/resources/schemas/DILCISExtensionMETS.xsd`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/resources/schemas/DILCISExtensionMETS.xsd.xml` & `eatb-0.2.2/eatb/resources/schemas/DILCISExtensionMETS.xsd.xml`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/resources/schemas/E-ARK-CSIP-v2-0-4.xml` & `eatb-0.2.2/eatb/resources/schemas/E-ARK-CSIP-v2-0-4.xml`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/resources/schemas/IP.xsd` & `eatb-0.2.2/eatb/resources/schemas/IP.xsd`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/resources/schemas/csip.xsd` & `eatb-0.2.2/eatb/resources/schemas/csip.xsd`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/resources/schemas/mets.xsd` & `eatb-0.2.2/eatb/resources/schemas/mets.xsd`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/resources/schemas/mets_1_11.xsd` & `eatb-0.2.2/eatb/resources/schemas/mets_1_11.xsd`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/resources/schemas/premis-v2-2.xsd` & `eatb-0.2.2/eatb/resources/schemas/premis-v2-2.xsd`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/resources/schemas/xlink.xsd` & `eatb-0.2.2/eatb/resources/schemas/xlink.xsd`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/resources/validation_rules.xml` & `eatb-0.2.2/eatb/resources/validation_rules.xml`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/settings.cfg` & `eatb-0.2.2/eatb/settings.cfg`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/settings.py` & `eatb-0.2.2/eatb/settings.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/storage.py` & `eatb-0.2.2/eatb/storage.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/utils/datetime.py` & `eatb-0.2.2/eatb/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/utils/dictutils.py` & `eatb-0.2.2/eatb/utils/dictutils.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/utils/encrypt.py` & `eatb-0.2.2/eatb/utils/encrypt.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/utils/fileutils.py` & `eatb-0.2.2/eatb/utils/fileutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -492,24 +492,26 @@
 
 def from_safe_filename(uri):
     """
     Convert URI to safe filename
     :param uri: URI
     :return: safe file name
     """
-    return uri.replace("+", ":")
+    return uri.replace("+", ":").replace("=", "/").replace(",", ".")
 
 
 def to_safe_filename(uri):
     """
     Convert URI to safe filename
     :param uri: URI
     :return: safe file name
     """
-    return uri.replace(" ", "").replace(":", "+")
+    # https://www.ietf.org/archive/id/draft-kunze-pairtree-01.txt
+    # 3.  Identifier string cleaning
+    return uri.replace(" ", "").replace(":", "+").replace("/", "=").replace(".", ",")
 
 
 class FileBinaryDataChunks(object):
     """
     Generator to iteratively read binary chunks of a large file
     """
```

### Comparing `eatb-0.2.1/eatb/utils/stringutils.py` & `eatb-0.2.2/eatb/utils/stringutils.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/utils/terminal.py` & `eatb-0.2.2/eatb/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb/utils/xmlutils.py` & `eatb-0.2.2/eatb/utils/xmlutils.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/eatb.egg-info/PKG-INFO` & `eatb-0.2.2/eatb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eatb
-Version: 0.2.1
+Version: 0.2.2
 Summary: A suite of tools for the creation of information packages for archival purposes.
 Home-page: https://www.e-ark-foundation.eu/e-ark-software-eatb
 Author: E-ARK Foundation
 Author-email: admin@e-ark-foundation.eu
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eatb-0.2.1/eatb.egg-info/SOURCES.txt` & `eatb-0.2.2/eatb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 eatb/resources/schemas/E-ARK-CSIP-v2-0-4.xml
 eatb/resources/schemas/IP.xsd
 eatb/resources/schemas/__init__.py
 eatb/resources/schemas/csip.xsd
 eatb/resources/schemas/mets.xsd
 eatb/resources/schemas/mets_1_11.xsd
 eatb/resources/schemas/premis-v2-2.xsd
+eatb/resources/schemas/premis-v3-0.xsd
 eatb/resources/schemas/xlink.xsd
 eatb/utils/XmlHelper.py
 eatb/utils/__init__.py
 eatb/utils/datetime.py
 eatb/utils/dictutils.py
 eatb/utils/encrypt.py
 eatb/utils/fileutils.py
```

### Comparing `eatb-0.2.1/setup.py` & `eatb-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="eatb",
-    version="0.2.1",
+    version="0.2.2",
     author="E-ARK Foundation",
     author_email="admin@e-ark-foundation.eu",
     license='MIT',
     description="A suite of tools for the creation of information packages for archival purposes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.e-ark-foundation.eu/e-ark-software-eatb",
```

### Comparing `eatb-0.2.1/tests/dip_premis_test.py` & `eatb-0.2.2/tests/dip_premis_test.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_checksum.py` & `eatb-0.2.2/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_cli.py` & `eatb-0.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_csip_validation.py` & `eatb-0.2.2/tests/test_csip_validation.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_datetime.py` & `eatb-0.2.2/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_encryption.py` & `eatb-0.2.2/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_extract.py` & `eatb-0.2.2/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_filehandling.py` & `eatb-0.2.2/tests/test_filehandling.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_formatidentification.py` & `eatb-0.2.2/tests/test_formatidentification.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_metadata_dcat.py` & `eatb-0.2.2/tests/test_metadata_dcat.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_metadata_ead.py` & `eatb-0.2.2/tests/test_metadata_ead.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_mets_generator.py` & `eatb-0.2.2/tests/test_mets_generator.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_mets_util.py` & `eatb-0.2.2/tests/test_mets_util.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_mets_validation.py` & `eatb-0.2.2/tests/test_mets_validation.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_pairtreestorage.py` & `eatb-0.2.2/tests/test_pairtreestorage.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_parsed_mets.py` & `eatb-0.2.2/tests/test_parsed_mets.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_premis_generation.py` & `eatb-0.2.2/tests/test_premis_generation.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_premis_manipulate.py` & `eatb-0.2.2/tests/test_premis_manipulate.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_stringutils.py` & `eatb-0.2.2/tests/test_stringutils.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_tarentryreader.py` & `eatb-0.2.2/tests/test_tarentryreader.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_unzip.py` & `eatb-0.2.2/tests/test_unzip.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_utils.py` & `eatb-0.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `eatb-0.2.1/tests/test_xml.py` & `eatb-0.2.2/tests/test_xml.py`

 * *Files identical despite different names*

