# Comparing `tmp/pyontoenv-0.1.7a7.tar.gz` & `tmp/pyontoenv-0.1.7a8.tar.gz`

## Comparing `pyontoenv-0.1.7a7.tar` & `pyontoenv-0.1.7a8.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0     1000     1000      776 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/Cargo.toml
--rw-r--r--   0     1000     1000  1689944 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/Brick-1.4-rc1.ttl
--rw-r--r--   0     1000     1000  1599287 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/Brick-1.3.ttl
--rw-r--r--   0     1000     1000     1248 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/model
--rw-r--r--   0     1000     1000      321 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/model.n3
--rw-r--r--   0     1000     1000      537 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/model.nt
--rw-r--r--   0     1000     1000     1248 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/model.ttl
--rw-r--r--   0     1000     1000      789 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/model.xml
--rw-r--r--   0     1000     1000      910 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/SCHEMA-FACADE_QUDT-v2.1.ttl
--rw-r--r--   0     1000     1000   146214 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
--rw-r--r--   0     1000     1000    30521 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
--rw-r--r--   0     1000     1000   163975 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
--rw-r--r--   0     1000     1000    18438 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIX-v2.1.ttl
--rw-r--r--   0     1000     1000    18438 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
--rw-r--r--   0     1000     1000  1323794 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
--rw-r--r--   0     1000     1000    17472 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
--rw-r--r--   0     1000     1000  1456008 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
--rw-r--r--   0     1000     1000   104496 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
--rw-r--r--   0     1000     1000  1255550 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/bacnet.ttl
--rw-r--r--   0     1000     1000    44502 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/brickpatches.ttl
--rw-r--r--   0     1000     1000    94738 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/dash.ttl
--rw-r--r--   0     1000     1000    23951 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/dtype.xml
--rw-r--r--   0     1000     1000    81761 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/rec.ttl
--rw-r--r--   0     1000     1000     4069 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/recimports.ttl
--rw-r--r--   0     1000     1000    11876 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/ref-schema.ttl
--rw-r--r--   0     1000     1000    52899 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/shacl.ttl
--rw-r--r--   0     1000     1000    15906 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/skos.ttl
--rw-r--r--   0     1000     1000    61455 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/vaem.xml
--rw-r--r--   0     1000     1000     1248 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/fileendings/model
--rw-r--r--   0     1000     1000      321 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/fileendings/model.n3
--rw-r--r--   0     1000     1000      537 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/fileendings/model.nt
--rw-r--r--   0     1000     1000     1248 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/fileendings/model.ttl
--rw-r--r--   0     1000     1000      789 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/fileendings/model.xml
--rw-r--r--   0     1000     1000     1160 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/ont1.ttl
--rw-r--r--   0     1000     1000     1132 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/ont2.ttl
--rw-r--r--   0     1000     1000     1135 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/ont3.ttl
--rw-r--r--   0     1000     1000     1106 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/ont4.ttl
--rw-r--r--   0     1000     1000      303 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/rdftest/ontology1.ttl
--rw-r--r--   0     1000     1000      321 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/rdftest/ontology2.ttl
--rw-r--r--   0     1000     1000      370 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/rdftest/ontology3.ttl
--rw-r--r--   0     1000     1000      321 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/rdftest/ontology4.ttl
--rw-r--r--   0     1000     1000      419 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/rdftest/ontology5.ttl
--rw-r--r--   0     1000     1000      370 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/rdftest/ontology6.ttl
--rw-r--r--   0     1000     1000     1160 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/updates/v1/ont1.ttl
--rw-r--r--   0     1000     1000     1132 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/updates/v1/ont2.ttl
--rw-r--r--   0     1000     1000     1135 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/updates/v1/ont3.ttl
--rw-r--r--   0     1000     1000     1106 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/updates/v1/ont4.ttl
--rw-r--r--   0     1000     1000     1135 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/updates/v2/ont3.ttl
--rw-r--r--   0     1000     1000     1129 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/fixtures/updates/v2/ont5.ttl
--rw-r--r--   0     1000     1000     5324 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/src/config.rs
--rw-r--r--   0     1000     1000     2180 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/src/consts.rs
--rw-r--r--   0     1000     1000     3267 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/src/doctor.rs
--rw-r--r--   0     1000     1000      350 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/src/errors.rs
--rw-r--r--   0     1000     1000    31009 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/src/lib.rs
--rw-r--r--   0     1000     1000    14000 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/src/ontology.rs
--rw-r--r--   0     1000     1000     3521 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/src/policy.rs
--rw-r--r--   0     1000     1000     4646 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/src/transform.rs
--rw-r--r--   0     1000     1000     6501 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/src/util.rs
--rw-r--r--   0     1000     1000    17905 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/lib/tests/ontoenv_test.rs
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a7/python/Cargo.toml
--rw-r--r--   0     1000     1000     2886 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/python/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000      686 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/python/.gitignore
--rw-r--r--   0     1000     1000      731 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/python/README.md
--rw-r--r--   0     1000     1000       71 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/python/build.rs
--rw-r--r--   0     1000     1000     5241 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/python/poetry.lock
--rw-r--r--   0     1000     1000       71 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/python/requirements.dev.txt
--rw-r--r--   0     1000     1000    14598 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/python/src/lib.rs
--rw-r--r--   0     1000     1000      694 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/python/test.py
--rw-r--r--   0     1000     1000    73227 2024-05-30 16:37:35.000000 pyontoenv-0.1.7a7/Cargo.lock
--rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a7/Cargo.toml
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a7/pyproject.toml
--rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a7/PKG-INFO
+-rw-r--r--   0     1001      127      776 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/Cargo.toml
+-rw-r--r--   0     1001      127  1689944 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/Brick-1.4-rc1.ttl
+-rw-r--r--   0     1001      127  1599287 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/Brick-1.3.ttl
+-rw-r--r--   0     1001      127     1248 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/model
+-rw-r--r--   0     1001      127      321 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/model.n3
+-rw-r--r--   0     1001      127      537 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/model.nt
+-rw-r--r--   0     1001      127     1248 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/model.ttl
+-rw-r--r--   0     1001      127      789 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/model.xml
+-rw-r--r--   0     1001      127      910 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/SCHEMA-FACADE_QUDT-v2.1.ttl
+-rw-r--r--   0     1001      127   146214 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
+-rw-r--r--   0     1001      127    30521 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
+-rw-r--r--   0     1001      127   163975 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
+-rw-r--r--   0     1001      127    18438 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIX-v2.1.ttl
+-rw-r--r--   0     1001      127    18438 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
+-rw-r--r--   0     1001      127  1323794 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127    17472 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127  1456008 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127   104496 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
+-rw-r--r--   0     1001      127  1255550 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/bacnet.ttl
+-rw-r--r--   0     1001      127    44502 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/brickpatches.ttl
+-rw-r--r--   0     1001      127    94738 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/dash.ttl
+-rw-r--r--   0     1001      127    23951 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/dtype.xml
+-rw-r--r--   0     1001      127    81761 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/rec.ttl
+-rw-r--r--   0     1001      127     4069 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/recimports.ttl
+-rw-r--r--   0     1001      127    11876 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/ref-schema.ttl
+-rw-r--r--   0     1001      127    52899 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/shacl.ttl
+-rw-r--r--   0     1001      127    15906 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/skos.ttl
+-rw-r--r--   0     1001      127    61455 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/vaem.xml
+-rw-r--r--   0     1001      127     1248 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/fileendings/model
+-rw-r--r--   0     1001      127      321 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/fileendings/model.n3
+-rw-r--r--   0     1001      127      537 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/fileendings/model.nt
+-rw-r--r--   0     1001      127     1248 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/fileendings/model.ttl
+-rw-r--r--   0     1001      127      789 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/fileendings/model.xml
+-rw-r--r--   0     1001      127     1148 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/ont1.ttl
+-rw-r--r--   0     1001      127     1144 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/ont2.ttl
+-rw-r--r--   0     1001      127     1135 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/ont3.ttl
+-rw-r--r--   0     1001      127     1106 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/ont4.ttl
+-rw-r--r--   0     1001      127      303 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/rdftest/ontology1.ttl
+-rw-r--r--   0     1001      127      321 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/rdftest/ontology2.ttl
+-rw-r--r--   0     1001      127      370 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/rdftest/ontology3.ttl
+-rw-r--r--   0     1001      127      321 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/rdftest/ontology4.ttl
+-rw-r--r--   0     1001      127      419 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/rdftest/ontology5.ttl
+-rw-r--r--   0     1001      127      370 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/rdftest/ontology6.ttl
+-rw-r--r--   0     1001      127     1160 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/updates/v1/ont1.ttl
+-rw-r--r--   0     1001      127     1132 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/updates/v1/ont2.ttl
+-rw-r--r--   0     1001      127     1135 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/updates/v1/ont3.ttl
+-rw-r--r--   0     1001      127     1106 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/updates/v1/ont4.ttl
+-rw-r--r--   0     1001      127     1135 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/updates/v2/ont3.ttl
+-rw-r--r--   0     1001      127     1129 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/fixtures/updates/v2/ont5.ttl
+-rw-r--r--   0     1001      127     5324 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/src/config.rs
+-rw-r--r--   0     1001      127     2180 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/src/consts.rs
+-rw-r--r--   0     1001      127     3267 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/src/doctor.rs
+-rw-r--r--   0     1001      127      350 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/src/errors.rs
+-rw-r--r--   0     1001      127    32753 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/src/lib.rs
+-rw-r--r--   0     1001      127    14000 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/src/ontology.rs
+-rw-r--r--   0     1001      127     3521 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/src/policy.rs
+-rw-r--r--   0     1001      127     4646 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/src/transform.rs
+-rw-r--r--   0     1001      127     6501 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/src/util.rs
+-rw-r--r--   0     1001      127    17863 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/lib/tests/ontoenv_test.rs
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a8/python/Cargo.toml
+-rw-r--r--   0     1001      127     2886 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/python/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/python/.gitignore
+-rw-r--r--   0     1001      127      731 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/python/README.md
+-rw-r--r--   0     1001      127       71 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/python/build.rs
+-rw-r--r--   0     1001      127     5241 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/python/poetry.lock
+-rw-r--r--   0     1001      127       71 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/python/requirements.dev.txt
+-rw-r--r--   0     1001      127    14597 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/python/src/lib.rs
+-rw-r--r--   0     1001      127      694 2024-06-01 15:57:13.000000 pyontoenv-0.1.7a8/python/test.py
+-rw-r--r--   0     1001      127    73227 2024-06-01 15:57:39.000000 pyontoenv-0.1.7a8/Cargo.lock
+-rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a8/Cargo.toml
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a8/pyproject.toml
+-rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a8/PKG-INFO
```

### Comparing `pyontoenv-0.1.7a7/lib/Cargo.toml` & `pyontoenv-0.1.7a8/lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/Brick-1.4-rc1.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/Brick-1.4-rc1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/Brick-1.3.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/Brick-1.3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/model` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/model.nt` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/model.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/model.xml` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/SCHEMA-FACADE_QUDT-v2.1.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/SCHEMA-FACADE_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/SCHEMA_QUDT_NoOWL-v2.1.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/SCHEMA_QUDT_NoOWL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIX-v2.1.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIX-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIXES-v2.1.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/VOCAB_QUDT-PREFIXES-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/bacnet.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/bacnet.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/brickpatches.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/brickpatches.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/dash.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/dash.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/dtype.xml` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/dtype.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/rec.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/rec.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/recimports.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/recimports.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/ref-schema.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/ref-schema.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/shacl.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/shacl.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/skos.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/skos.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/brick-stuff/support/vaem.xml` & `pyontoenv-0.1.7a8/lib/fixtures/brick-stuff/support/vaem.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/fileendings/model` & `pyontoenv-0.1.7a8/lib/fixtures/fileendings/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/fileendings/model.nt` & `pyontoenv-0.1.7a8/lib/fixtures/fileendings/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/fileendings/model.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/fileendings/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/fileendings/model.xml` & `pyontoenv-0.1.7a8/lib/fixtures/fileendings/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/ont1.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/updates/v1/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/ont2.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/updates/v1/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/ont3.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/ont4.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/updates/v1/ont3.ttl`

 * *Files 4% similar despite different names*

```diff
@@ -16,10 +16,12 @@
 @prefix sosa: <http://www.w3.org/ns/sosa/> .
 @prefix tag: <https://brickschema.org/schema/BrickTag#> .
 @prefix unit: <http://qudt.org/vocab/unit/> .
 @prefix vcard: <http://www.w3.org/2006/vcard/ns#> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix : <urn:ont3/> .
 
-<urn:ont4> a owl:Ontology .
+<urn:ont3> a owl:Ontology ;
+    owl:imports <urn:ont4> .
+
+:Setpoint a owl:Class .
 
-:Parameter a owl:Class .
```

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/updates/v1/ont1.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/ont2.ttl`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,13 @@
 @prefix sh: <http://www.w3.org/ns/shacl#> .
 @prefix skos: <http://www.w3.org/2004/02/skos/core#> .
 @prefix sosa: <http://www.w3.org/ns/sosa/> .
 @prefix tag: <https://brickschema.org/schema/BrickTag#> .
 @prefix unit: <http://qudt.org/vocab/unit/> .
 @prefix vcard: <http://www.w3.org/2006/vcard/ns#> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix : <urn:ont1/> .
+@prefix : <urn:ont2/> .
 
-<urn:ont1> a owl:Ontology ;
-    owl:imports <urn:ont2>, <urn:ont3> .
+<urn:ont2> a owl:Ontology ;
+    owl:imports <urn:ont3>, <urn:ont4> .
 
-:VAV a owl:Class .
-:AHU a owl:Class .
+:Sensor a owl:Class .
```

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/updates/v1/ont2.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/ont1.ttl`

 * *Files 6% similar despite different names*

```diff
@@ -14,13 +14,14 @@
 @prefix sh: <http://www.w3.org/ns/shacl#> .
 @prefix skos: <http://www.w3.org/2004/02/skos/core#> .
 @prefix sosa: <http://www.w3.org/ns/sosa/> .
 @prefix tag: <https://brickschema.org/schema/BrickTag#> .
 @prefix unit: <http://qudt.org/vocab/unit/> .
 @prefix vcard: <http://www.w3.org/2006/vcard/ns#> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix : <urn:ont2/> .
+@prefix : <urn:ont1/> .
 
-<urn:ont2> a owl:Ontology ;
-    owl:imports <urn:ont4> .
+<urn:ont1> a owl:Ontology ;
+    owl:imports <urn:ont3> .
 
-:Sensor a owl:Class .
+:VAV a owl:Class .
+:AHU a owl:Class .
```

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/updates/v1/ont3.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/updates/v2/ont3.ttl`

 * *Files 1% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 @prefix tag: <https://brickschema.org/schema/BrickTag#> .
 @prefix unit: <http://qudt.org/vocab/unit/> .
 @prefix vcard: <http://www.w3.org/2006/vcard/ns#> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix : <urn:ont3/> .
 
 <urn:ont3> a owl:Ontology ;
-    owl:imports <urn:ont4> .
+    owl:imports <urn:ont5> .
 
 :Setpoint a owl:Class .
```

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/updates/v1/ont4.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/updates/v2/ont3.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/updates/v2/ont5.ttl`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,13 @@
 @prefix sh: <http://www.w3.org/ns/shacl#> .
 @prefix skos: <http://www.w3.org/2004/02/skos/core#> .
 @prefix sosa: <http://www.w3.org/ns/sosa/> .
 @prefix tag: <https://brickschema.org/schema/BrickTag#> .
 @prefix unit: <http://qudt.org/vocab/unit/> .
 @prefix vcard: <http://www.w3.org/2006/vcard/ns#> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix : <urn:ont3/> .
+@prefix : <urn:ont5/> .
 
-<urn:ont3> a owl:Ontology ;
-    owl:imports <urn:ont5> .
-
-:Setpoint a owl:Class .
+<urn:ont5> a owl:Ontology .
 
+:Test1 a brick:Sensor .
+:Test2 a brick:Sensor .
```

### Comparing `pyontoenv-0.1.7a7/lib/fixtures/updates/v2/ont5.ttl` & `pyontoenv-0.1.7a8/lib/fixtures/updates/v1/ont4.ttl`

 * *Files 20% similar despite different names*

```diff
@@ -14,13 +14,12 @@
 @prefix sh: <http://www.w3.org/ns/shacl#> .
 @prefix skos: <http://www.w3.org/2004/02/skos/core#> .
 @prefix sosa: <http://www.w3.org/ns/sosa/> .
 @prefix tag: <https://brickschema.org/schema/BrickTag#> .
 @prefix unit: <http://qudt.org/vocab/unit/> .
 @prefix vcard: <http://www.w3.org/2006/vcard/ns#> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
-@prefix : <urn:ont5/> .
+@prefix : <urn:ont4/> .
 
-<urn:ont5> a owl:Ontology .
+<urn:ont4> a owl:Ontology .
 
-:Test1 a brick:Sensor .
-:Test2 a brick:Sensor .
+:Parameter a owl:Class .
```

### Comparing `pyontoenv-0.1.7a7/lib/src/config.rs` & `pyontoenv-0.1.7a8/lib/src/config.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/src/consts.rs` & `pyontoenv-0.1.7a8/lib/src/consts.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/src/doctor.rs` & `pyontoenv-0.1.7a8/lib/src/doctor.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/src/lib.rs` & `pyontoenv-0.1.7a8/lib/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,16 @@
     #[serde(skip)]
     read_only: bool,
 }
 
 // probably need some graph "identifier" that incorporates location and version..
 
 impl OntoEnv {
+    /// Create a new OntoEnv with the given configuration. Will error if the
+    /// environment already exists and recreate is false.
     pub fn new(config: Config, recreate: bool) -> Result<Self> {
         // create the config.root/.ontoenv directory so it exists before the store
         // is created
         let ontoenv_dir = config.root.join(".ontoenv");
 
         // if recreate is False, raise an error if the directory already exists
         if ontoenv_dir.exists() && !recreate {
@@ -101,59 +103,68 @@
                 .map_err(|e| anyhow::anyhow!("Could not open store: {}", e));
         }
         Store::open(ontoenv_dir.join("store.db"))
             .or_else(|_| Store::open_read_only(ontoenv_dir.join("store.db")))
             .map_err(|e| anyhow::anyhow!("Could not open store: {}", e))
     }
 
+    /// Close the environment and release any resources
     pub fn close(self) {}
 
     //TODO: add import_graph which imports a single graph into a given graph
 
+    /// Returns the number of graphs in the environment
     pub fn num_graphs(&self) -> usize {
         self.ontologies.len()
     }
 
+    /// Returns the number of triples in the environment
     pub fn num_triples(&self) -> Result<usize> {
         // this construction coerces the error the the correct type
         Ok(self.store()?.len()?)
     }
 
+    /// Returns an Ontology with the given name. Uses the provided policy to resolve
+    /// the ontology if there are multiple ontologies with the same name.
     pub fn get_ontology_with_policy(
         &self,
         name: NamedNodeRef,
         policy: &dyn policy::ResolutionPolicy,
     ) -> Option<Ontology> {
         let ontologies = self.ontologies.values().collect::<Vec<&Ontology>>();
         policy
             .resolve(name.as_str(), ontologies.as_slice())
             .cloned()
     }
 
+    /// Returns the first ontology with the given name
     pub fn get_ontology_by_name(&self, name: NamedNodeRef) -> Option<&Ontology> {
         // choose the first ontology with the given name
         self.ontologies
             .values()
             .find(|&ontology| ontology.name() == name)
     }
 
+    /// Returns the first graph with the given name
     pub fn get_graph_by_name(&self, name: NamedNodeRef) -> Result<Graph> {
         let ontology = self
             .get_ontology_by_name(name)
             .ok_or(anyhow::anyhow!("Ontology not found"))?;
         self.get_graph(ontology.id())
     }
 
+    /// Returns the first ontology with the given location
     pub fn get_ontology_by_location(&self, location: &OntologyLocation) -> Option<&Ontology> {
         // choose the first ontology with the given location
         self.ontologies
             .values()
             .find(|&ontology| ontology.location() == Some(location))
     }
 
+    /// Load an OntoEnv from the given path
     pub fn from_file(path: &Path, read_only: bool) -> Result<Self> {
         let file = std::fs::File::open(path)?;
         let reader = BufReader::new(file);
         let env: OntoEnv = serde_json::from_reader(reader)?;
         Ok(Self { read_only, ..env })
     }
 
@@ -195,23 +206,24 @@
             let ont = self
                 .ontologies
                 .get(&ontology)
                 .ok_or(anyhow::anyhow!("Ontology not found"))?;
             let imports = &ont.imports.clone();
             for import in imports {
                 // check to see if we have a file defining this ontology first
-                if let Some(imp) = self.get_ontology_by_name(import.into()) {
+                let location = if let Some(imp) = self.get_ontology_by_name(import.into()) {
                     // if we have already re-visited it, skip
                     if seen.contains(imp.id()) || stack.contains(imp.id()) {
                         continue;
                     }
-                }
-
-                // otherwise, try to find the ontology by location
-                let location = OntologyLocation::from_str(import.as_str())?;
+                    imp.location().ok_or(anyhow::anyhow!("Ontology location not found"))?.clone()
+                } else {
+                    // otherwise, try to find the ontology by location
+                    OntologyLocation::from_str(import.as_str())?
+                };
                 let imp = match self.add_or_update_ontology_from_location(location) {
                     Ok(imp) => imp,
                     Err(e) => {
                         if self.config.strict {
                             return Err(e);
                         } else {
                             error!("Failed to read ontology file {}: {}", import.as_str(), e);
@@ -219,14 +231,17 @@
                         }
                     }
                 };
                 stack.push_back(imp);
             }
         }
 
+        // what are the current ontologies in the environment?
+        let current_ontologies: HashSet<GraphIdentifier> = self.ontologies.keys().cloned().collect();
+
         // put the dependency graph into self.dependency_graph
         let mut indexes: HashMap<GraphIdentifier, NodeIndex> = HashMap::new();
         let mut graph: DiGraph<GraphIdentifier, (), petgraph::Directed> = DiGraph::new();
         // add all ontologies in self.ontologies to the graph
         for ontology in self.ontologies.keys() {
             let index = graph.add_node(ontology.clone());
             indexes.insert(ontology.clone(), index);
@@ -241,15 +256,18 @@
                     continue;
                 }
             };
             for import in &ont.imports {
                 let graph_id = match self.get_ontology_by_name(import.into()) {
                     Some(imp) => imp.id(),
                     None => {
-                        error!("Import not found: {}", import);
+                        if self.config.strict {
+                            return Err(anyhow::anyhow!("Import not found: {}", import));
+                        }
+                        warn!("Import not found: {}", import);
                         continue;
                     }
                 };
                 let import_index = indexes.get(graph_id).unwrap();
                 graph.add_edge(*index, *import_index, ());
             }
         }
@@ -475,14 +493,16 @@
                     files.push(OntologyLocation::File(entry.path().to_path_buf()));
                 }
             }
         }
         Ok(files)
     }
 
+    /// Add the ontology from the given location to the environment. If the ontology
+    /// already exists in the environment, it is overwritten.
     pub fn add(&mut self, location: OntologyLocation) -> Result<GraphIdentifier> {
         info!("Adding ontology from location: {:?}", location);
         self.add_or_update_ontology_from_location(location)
     }
 
     /// Add or update the ontology from the given location. Overwrites the ontology
     /// if it already exists in the environment.
@@ -556,18 +576,20 @@
             );
             store.insert(q)?;
         }
 
         Ok(id)
     }
 
+    /// Return a list of all graph identifiers in the environment
     pub fn graph_ids(&self) -> Vec<GraphIdentifier> {
         self.ontologies.keys().cloned().collect()
     }
 
+    /// Return a list of all ontologies in the environment
     pub fn ontologies(&self) -> &HashMap<GraphIdentifier, Ontology> {
         &self.ontologies
     }
 
     /// returns a list of all graphs in the environment that provide a definition
     /// for the given IRI (using owl:Ontology)
     pub fn get_graphs_by_name(&self, name: NamedNodeRef) -> Vec<GraphIdentifier> {
@@ -576,14 +598,15 @@
             if ontology.name() == name {
                 graphs.push(ontology.id().clone());
             }
         }
         graphs
     }
 
+    /// Returns the graph for the given graph identifier
     pub fn get_graph(&self, id: &GraphIdentifier) -> Result<Graph> {
         let mut graph = Graph::new();
         let name = id.graphname()?;
         let store = self.store()?;
         for quad in store.quads_for_pattern(None, None, None, Some(name.as_ref())) {
             graph.insert(quad?.as_ref());
         }
@@ -624,15 +647,18 @@
                 .get(&graph)
                 .ok_or(anyhow::anyhow!("Ontology not found"))?;
             for import in &ontology.imports {
                 // get graph identifier for import
                 let import = match self.get_ontology_by_name(import.into()) {
                     Some(imp) => imp.id().clone(),
                     None => {
-                        error!("Import not found: {}", import);
+                        if self.config.strict {
+                            return Err(anyhow::anyhow!("Import not found: {}", import));
+                        }
+                        warn!("Import not found: {}", import);
                         continue;
                     }
                 };
                 if !closure.contains(&import) {
                     stack.push_back(import);
                 }
             }
@@ -713,14 +739,16 @@
             println!("Problem: {}", message);
             for location in locations {
                 println!("  - {}", location);
             }
         }
     }
 
+    /// Outputs a human-readable dump of the environment, including all ontologies
+    /// and their metadata and imports
     pub fn dump(&self) {
         let mut ontologies = self.ontologies.clone();
         let mut groups: HashMap<NamedNode, Vec<Ontology>> = HashMap::new();
         for ontology in ontologies.values_mut() {
             let name = ontology.name();
             groups.entry(name).or_default().push(ontology.clone());
         }
```

### Comparing `pyontoenv-0.1.7a7/lib/src/ontology.rs` & `pyontoenv-0.1.7a8/lib/src/ontology.rs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 use log::{debug, info, warn};
 use oxigraph::model::{
     Graph as OxigraphGraph, GraphName, NamedNode, NamedNodeRef, Subject, SubjectRef, TermRef,
 };
 use serde::{Deserialize, Deserializer, Serialize, Serializer};
 use serde_with::{serde_as, DeserializeAs, SerializeAs};
 use std::collections::HashMap;
-use std::path::PathBuf;
 use std::hash::Hash;
+use std::path::PathBuf;
 //
 // custom derive for NamedNode
 fn namednode_ser<S>(namednode: &NamedNode, serializer: S) -> Result<S::Ok, S::Error>
 where
     S: serde::Serializer,
 {
     serializer.serialize_str(namednode.as_str())
```

### Comparing `pyontoenv-0.1.7a7/lib/src/policy.rs` & `pyontoenv-0.1.7a8/lib/src/policy.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/src/transform.rs` & `pyontoenv-0.1.7a8/lib/src/transform.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/src/util.rs` & `pyontoenv-0.1.7a8/lib/src/util.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/lib/tests/ontoenv_test.rs` & `pyontoenv-0.1.7a8/lib/tests/ontoenv_test.rs`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
         // Check the contents of the temporary directory
         for entry in fs::read_dir(dir.path()).expect("Failed to read directory") {
             let entry = entry.expect("Failed to read entry");
             let file_name = entry.file_name().into_string().expect("Failed to convert filename to string");
 
             if !provided_files.contains(file_name.as_str()) && entry.file_type().expect("Failed to get file type").is_file() {
-                println!("Warning: extra file {} found in directory", file_name);
                 // remove it
                 fs::remove_file(entry.path()).expect("Failed to remove file");
             }
         }
     }};
 }
 
@@ -105,22 +104,15 @@
 fn test_ontoenv_scans() -> Result<()> {
     let dir = TempDir::new("ontoenv")?;
     setup!(&dir, { "fixtures/ont1.ttl" => "ont1.ttl", 
                    "fixtures/ont2.ttl" => "ont2.ttl",
                    "fixtures/ont3.ttl" => "ont3.ttl",
                    "fixtures/ont4.ttl" => "ont4.ttl" });
     // print the files in dir
-    println!("listing files");
-    for entry in std::fs::read_dir(dir.path())? {
-        let entry = entry?;
-        println!("inside> {:?}", entry.file_name());
-    }
-
     let cfg = default_config(&dir);
-    println!("config: {:?}", cfg);
     let mut env = OntoEnv::new(cfg, false)?;
     env.update()?;
     assert_eq!(env.num_graphs(), 4);
     teardown(dir);
     Ok(())
 }
 
@@ -185,18 +177,18 @@
     assert_eq!(env.num_graphs(), 4);
 
     // updating again shouldn't add anything
     env.update()?;
     assert_eq!(env.num_graphs(), 4);
     assert_eq!(env.num_triples()?, old_num_triples);
 
-    // remove ont4.ttl
+    // remove ont2.ttl
     setup!(&dir, { "fixtures/ont1.ttl" => "ont1.ttl", 
-                   "fixtures/ont2.ttl" => "ont2.ttl",
-                   "fixtures/ont3.ttl" => "ont3.ttl"});
+                   "fixtures/ont3.ttl" => "ont3.ttl",
+                   "fixtures/ont4.ttl" => "ont4.ttl"});
 
     env.update()?;
     assert_eq!(env.num_graphs(), 3);
 
     // copy ont4.ttl back
     setup!(&dir, { "fixtures/ont1.ttl" => "ont1.ttl", 
                    "fixtures/ont2.ttl" => "ont2.ttl",
@@ -241,14 +233,21 @@
     let mut env = OntoEnv::new(cfg, false)?;
     env.update()?;
 
     let ont1 = NamedNodeRef::new("urn:ont1")?;
     let ont = env
         .get_ontology_by_name(ont1)
         .ok_or(anyhow::anyhow!("Ontology not found"))?;
+    assert_eq!(ont.imports.len(), 1);
+    assert!(ont.location().unwrap().is_file());
+
+    let ont2 = NamedNodeRef::new("urn:ont2")?;
+    let ont = env
+        .get_ontology_by_name(ont2)
+        .ok_or(anyhow::anyhow!("Ontology not found"))?;
     assert_eq!(ont.imports.len(), 2);
     assert!(ont.location().unwrap().is_file());
     teardown(dir);
     Ok(())
 }
 
 #[test]
@@ -267,15 +266,15 @@
         ont1_path
             .to_str()
             .ok_or(anyhow::anyhow!("Failed to convert to string"))?,
     )?;
     let ont = env
         .get_ontology_by_location(&loc)
         .ok_or(anyhow::anyhow!("Ontology not found"))?;
-    assert_eq!(ont.imports.len(), 2);
+    assert_eq!(ont.imports.len(), 1);
     assert!(ont
         .location()
         .ok_or(anyhow::anyhow!("Location not found"))?
         .is_file());
     teardown(dir);
     Ok(())
 }
```

### Comparing `pyontoenv-0.1.7a7/python/Cargo.toml` & `pyontoenv-0.1.7a8/python/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/python/.github/workflows/CI.yml` & `pyontoenv-0.1.7a8/python/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/python/.gitignore` & `pyontoenv-0.1.7a8/python/.gitignore`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/python/README.md` & `pyontoenv-0.1.7a8/python/README.md`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/python/poetry.lock` & `pyontoenv-0.1.7a8/python/poetry.lock`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/python/src/lib.rs` & `pyontoenv-0.1.7a8/python/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,15 @@
     }
 
     fn import_dependencies(&self, py: Python, graph: &Bound<'_, PyAny>) -> PyResult<()> {
         let rdflib = py.import_bound("rdflib")?;
         let py_rdf_type = term_to_python(py, &rdflib, Term::NamedNode(TYPE.into()))?;
         let py_ontology = term_to_python(py, &rdflib, Term::NamedNode(ONTOLOGY.into()))?;
         let value_fun: Py<PyAny> = graph.getattr("value")?.into();
-        let kwargs =  [("predicate", py_rdf_type), ("object", py_ontology)].into_py_dict_bound(py);
+        let kwargs = [("predicate", py_rdf_type), ("object", py_ontology)].into_py_dict_bound(py);
         let ontology = value_fun.call_bound(py, (), Some(&kwargs))?;
 
         if ontology.is_none(py) {
             return Ok(());
         }
 
         let ontology = ontology.to_string();
```

### Comparing `pyontoenv-0.1.7a7/python/test.py` & `pyontoenv-0.1.7a8/python/test.py`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a7/Cargo.lock` & `pyontoenv-0.1.7a8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1375,15 +1375,15 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "ontoenv"
-version = "0.1.7-a7"
+version = "0.1.7-a8"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "derive_builder",
  "env_logger",
  "glob",
@@ -1401,15 +1401,15 @@
  "tempdir",
  "tempfile",
  "walkdir",
 ]
 
 [[package]]
 name = "ontoenv-cli"
-version = "0.1.7-a7"
+version = "0.1.7-a8"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "env_logger",
  "ontoenv",
  "oxigraph",
@@ -1719,15 +1719,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyontoenv"
-version = "0.1.7-a7"
+version = "0.1.7-a8"
 dependencies = [
  "anyhow",
  "env_logger",
  "log",
  "ontoenv",
  "oxigraph",
  "pyo3",
```

### Comparing `pyontoenv-0.1.7a7/Cargo.toml` & `pyontoenv-0.1.7a8/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["python"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.7-a7"
+version = "0.1.7-a8"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 license = "BSD-3-Clause"
 edition = "2021"
 rust-version = "1.70"
 repository = "https://github.com/gtfierro/ontoenv-rs"
 homepage = "https://github.com/gtfierro/ontoenv-rs"
 description = "A tool for managing ontologies and their dependencies"
@@ -27,8 +27,8 @@
 glob = "0.3.1"
 chrono = { version = "0.4.33", features = ["serde"] }
 petgraph = { version = "0.6.4", features = ["serde-1"] }
 clap = { version = "4.4.18", features = ["derive"] }
 derive_builder = "0.13.0"
 oxigraph = "0.3.22"
 
-ontoenv = { version = "0.1.7-a7", path = "lib" }
+ontoenv = { version = "0.1.7-a8", path = "lib" }
```

### Comparing `pyontoenv-0.1.7a7/pyproject.toml` & `pyontoenv-0.1.7a8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 manifest-path = "python/Cargo.toml"
 
 [tool.poetry]
 name = "ontoenv"
-version = "0.1.7a7"
+version = "0.1.7a8"
 description = "Python bindings for the OntoEnv Rust library. Manages ontology-based environments for building knowledge graphs."
 license = "bsd-3-clause"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pyontoenv-0.1.7a7/PKG-INFO` & `pyontoenv-0.1.7a8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyontoenv
-Version: 0.1.7a7
+Version: 0.1.7a8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Command line tool to manage ontologies and their imports in a local environment
 Home-Page: https://github.com/gtfierro/ontoenv-rs
 Author: Gabe Fierro <gtfierro@mines.edu>
 Author-email: Gabe Fierro <gtfierro@mines.edu>
```

