# Comparing `tmp/emmet-api-0.83.6rc3.tar.gz` & `tmp/emmet-api-0.83.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmet-api-0.83.6rc3.tar", last modified: Tue May 21 23:05:59 2024, max compression
+gzip compressed data, was "emmet-api-0.83.7.tar", last modified: Fri May 31 23:09:47 2024, max compression
```

## Comparing `emmet-api-0.83.6rc3.tar` & `emmet-api-0.83.7.tar`

### file list

```diff
@@ -1,348 +1,348 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.651682 emmet-api-0.83.6rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-21 23:05:59.651682 emmet-api-0.83.6rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.607682 emmet-api-0.83.6rc3/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.615682 emmet-api-0.83.6rc3/emmet/api/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.615682 emmet-api-0.83.6rc3/emmet/api/core/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.615682 emmet-api-0.83.6rc3/emmet/api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (127)    21390 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/core/global_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.615682 emmet-api-0.83.6rc3/emmet/api/routes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.615682 emmet-api-0.83.6rc3/emmet/api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.619682 emmet-api-0.83.6rc3/emmet/api/routes/_general_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/_general_store/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/_general_store/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.619682 emmet-api-0.83.6rc3/emmet/api/routes/_messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/_messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/_messages/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/_messages/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.619682 emmet-api-0.83.6rc3/emmet/api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.619682 emmet-api-0.83.6rc3/emmet/api/routes/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.619682 emmet-api-0.83.6rc3/emmet/api/routes/legacy/jcesr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/legacy/jcesr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/legacy/jcesr/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/legacy/jcesr/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.619682 emmet-api-0.83.6rc3/emmet/api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.619682 emmet-api-0.83.6rc3/emmet/api/routes/materials/absorption/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/absorption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/absorption/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.619682 emmet-api-0.83.6rc3/emmet/api/routes/materials/alloys/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/alloys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/alloys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/alloys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.619682 emmet-api-0.83.6rc3/emmet/api/routes/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.619682 emmet-api-0.83.6rc3/emmet/api/routes/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.619682 emmet-api-0.83.6rc3/emmet/api/routes/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/chemenv/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/chemenv/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.623682 emmet-api-0.83.6rc3/emmet/api/routes/materials/conversion_electrodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/conversion_electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/conversion_electrodes/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.623682 emmet-api-0.83.6rc3/emmet/api/routes/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.623682 emmet-api-0.83.6rc3/emmet/api/routes/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.623682 emmet-api-0.83.6rc3/emmet/api/routes/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.623682 emmet-api-0.83.6rc3/emmet/api/routes/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.623682 emmet-api-0.83.6rc3/emmet/api/routes/materials/fermi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.623682 emmet-api-0.83.6rc3/emmet/api/routes/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.623682 emmet-api-0.83.6rc3/emmet/api/routes/materials/insertion_electrodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/insertion_electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/insertion_electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/insertion_electrodes/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/insertion_electrodes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.623682 emmet-api-0.83.6rc3/emmet/api/routes/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.627682 emmet-api-0.83.6rc3/emmet/api/routes/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13458 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.627682 emmet-api-0.83.6rc3/emmet/api/routes/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.627682 emmet-api-0.83.6rc3/emmet/api/routes/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.627682 emmet-api-0.83.6rc3/emmet/api/routes/materials/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.627682 emmet-api-0.83.6rc3/emmet/api/routes/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.627682 emmet-api-0.83.6rc3/emmet/api/routes/materials/provenance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.627682 emmet-api-0.83.6rc3/emmet/api/routes/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.627682 emmet-api-0.83.6rc3/emmet/api/routes/materials/similarity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.627682 emmet-api-0.83.6rc3/emmet/api/routes/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.627682 emmet-api-0.83.6rc3/emmet/api/routes/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.631682 emmet-api-0.83.6rc3/emmet/api/routes/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.631682 emmet-api-0.83.6rc3/emmet/api/routes/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.631682 emmet-api-0.83.6rc3/emmet/api/routes/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.631682 emmet-api-0.83.6rc3/emmet/api/routes/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.631682 emmet-api-0.83.6rc3/emmet/api/routes/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/materials/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.631682 emmet-api-0.83.6rc3/emmet/api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.631682 emmet-api-0.83.6rc3/emmet/api/routes/molecules/association/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/association/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.631682 emmet-api-0.83.6rc3/emmet/api/routes/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.635682 emmet-api-0.83.6rc3/emmet/api/routes/molecules/metal_binding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/metal_binding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/metal_binding/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/metal_binding/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.635682 emmet-api-0.83.6rc3/emmet/api/routes/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/molecules/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    14682 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.635682 emmet-api-0.83.6rc3/emmet/api/routes/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19385 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/orbitals/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/orbitals/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.635682 emmet-api-0.83.6rc3/emmet/api/routes/molecules/partial_charges/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/partial_charges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/partial_charges/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.635682 emmet-api-0.83.6rc3/emmet/api/routes/molecules/partial_spins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/partial_spins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/partial_spins/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.635682 emmet-api-0.83.6rc3/emmet/api/routes/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/redox/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/redox/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.635682 emmet-api-0.83.6rc3/emmet/api/routes/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.635682 emmet-api-0.83.6rc3/emmet/api/routes/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.635682 emmet-api-0.83.6rc3/emmet/api/routes/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/thermo/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.639682 emmet-api-0.83.6rc3/emmet/api/routes/molecules/vibrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/vibrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/emmet/api/routes/molecules/vibrations/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.639682 emmet-api-0.83.6rc3/emmet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-21 23:05:59.000000 emmet-api-0.83.6rc3/emmet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-05-21 23:05:59.000000 emmet-api-0.83.6rc3/emmet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 23:05:59.000000 emmet-api-0.83.6rc3/emmet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 23:05:59.000000 emmet-api-0.83.6rc3/emmet_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 23:05:59.000000 emmet-api-0.83.6rc3/emmet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 23:05:59.000000 emmet-api-0.83.6rc3/emmet_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13875 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/material_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/molecule_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.639682 emmet-api-0.83.6rc3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9777 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/requirements/ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/requirements/ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 23:05:59.651682 emmet-api-0.83.6rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.639682 emmet-api-0.83.6rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.639682 emmet-api-0.83.6rc3/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.639682 emmet-api-0.83.6rc3/tests/_general_store/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/_general_store/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.639682 emmet-api-0.83.6rc3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.611682 emmet-api-0.83.6rc3/tests/legacy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.639682 emmet-api-0.83.6rc3/tests/legacy/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/legacy/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/legacy/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.615682 emmet-api-0.83.6rc3/tests/materials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.639682 emmet-api-0.83.6rc3/tests/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.643682 emmet-api-0.83.6rc3/tests/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.643682 emmet-api-0.83.6rc3/tests/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/chemenv/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.643682 emmet-api-0.83.6rc3/tests/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.643682 emmet-api-0.83.6rc3/tests/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.643682 emmet-api-0.83.6rc3/tests/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/electrodes/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/electrodes/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.643682 emmet-api-0.83.6rc3/tests/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.643682 emmet-api-0.83.6rc3/tests/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.643682 emmet-api-0.83.6rc3/tests/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.643682 emmet-api-0.83.6rc3/tests/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.643682 emmet-api-0.83.6rc3/tests/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.643682 emmet-api-0.83.6rc3/tests/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.643682 emmet-api-0.83.6rc3/tests/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.643682 emmet-api-0.83.6rc3/tests/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.643682 emmet-api-0.83.6rc3/tests/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.647682 emmet-api-0.83.6rc3/tests/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.647682 emmet-api-0.83.6rc3/tests/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.647682 emmet-api-0.83.6rc3/tests/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.647682 emmet-api-0.83.6rc3/tests/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.647682 emmet-api-0.83.6rc3/tests/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.647682 emmet-api-0.83.6rc3/tests/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.647682 emmet-api-0.83.6rc3/tests/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/materials/xas/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.647682 emmet-api-0.83.6rc3/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.647682 emmet-api-0.83.6rc3/tests/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.647682 emmet-api-0.83.6rc3/tests/molecules/metal_binding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/metal_binding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/metal_binding/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.647682 emmet-api-0.83.6rc3/tests/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/molecules/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.651682 emmet-api-0.83.6rc3/tests/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/orbitals/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.651682 emmet-api-0.83.6rc3/tests/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/redox/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.651682 emmet-api-0.83.6rc3/tests/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.651682 emmet-api-0.83.6rc3/tests/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/tasks/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:59.651682 emmet-api-0.83.6rc3/tests/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-21 23:05:52.000000 emmet-api-0.83.6rc3/tests/molecules/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.543336 emmet-api-0.83.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-31 23:09:41.000000 emmet-api-0.83.7/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-31 23:09:47.543336 emmet-api-0.83.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-31 23:09:41.000000 emmet-api-0.83.7/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.503337 emmet-api-0.83.7/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.511336 emmet-api-0.83.7/emmet/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.511336 emmet-api-0.83.7/emmet/api/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.511336 emmet-api-0.83.7/emmet/api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21390 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/core/global_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.511336 emmet-api-0.83.7/emmet/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.511336 emmet-api-0.83.7/emmet/api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.515337 emmet-api-0.83.7/emmet/api/routes/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/_general_store/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/_general_store/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.515337 emmet-api-0.83.7/emmet/api/routes/_messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/_messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/_messages/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/_messages/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.515337 emmet-api-0.83.7/emmet/api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.515337 emmet-api-0.83.7/emmet/api/routes/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.515337 emmet-api-0.83.7/emmet/api/routes/legacy/jcesr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/legacy/jcesr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/legacy/jcesr/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/legacy/jcesr/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.515337 emmet-api-0.83.7/emmet/api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.515337 emmet-api-0.83.7/emmet/api/routes/materials/absorption/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/absorption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/absorption/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.515337 emmet-api-0.83.7/emmet/api/routes/materials/alloys/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/alloys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/alloys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/alloys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.515337 emmet-api-0.83.7/emmet/api/routes/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.515337 emmet-api-0.83.7/emmet/api/routes/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.515337 emmet-api-0.83.7/emmet/api/routes/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/chemenv/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/chemenv/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.515337 emmet-api-0.83.7/emmet/api/routes/materials/conversion_electrodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/conversion_electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/conversion_electrodes/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.519337 emmet-api-0.83.7/emmet/api/routes/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.519337 emmet-api-0.83.7/emmet/api/routes/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.519337 emmet-api-0.83.7/emmet/api/routes/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.519337 emmet-api-0.83.7/emmet/api/routes/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.519337 emmet-api-0.83.7/emmet/api/routes/materials/fermi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.519337 emmet-api-0.83.7/emmet/api/routes/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.519337 emmet-api-0.83.7/emmet/api/routes/materials/insertion_electrodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/insertion_electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12790 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/insertion_electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/insertion_electrodes/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/insertion_electrodes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.519337 emmet-api-0.83.7/emmet/api/routes/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.519337 emmet-api-0.83.7/emmet/api/routes/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13458 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.519337 emmet-api-0.83.7/emmet/api/routes/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.523337 emmet-api-0.83.7/emmet/api/routes/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.523337 emmet-api-0.83.7/emmet/api/routes/materials/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.523337 emmet-api-0.83.7/emmet/api/routes/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.523337 emmet-api-0.83.7/emmet/api/routes/materials/provenance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.523337 emmet-api-0.83.7/emmet/api/routes/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.523337 emmet-api-0.83.7/emmet/api/routes/materials/similarity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.523337 emmet-api-0.83.7/emmet/api/routes/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.523337 emmet-api-0.83.7/emmet/api/routes/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.523337 emmet-api-0.83.7/emmet/api/routes/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.527336 emmet-api-0.83.7/emmet/api/routes/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.527336 emmet-api-0.83.7/emmet/api/routes/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.527336 emmet-api-0.83.7/emmet/api/routes/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.527336 emmet-api-0.83.7/emmet/api/routes/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/materials/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.527336 emmet-api-0.83.7/emmet/api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.527336 emmet-api-0.83.7/emmet/api/routes/molecules/association/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/association/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.527336 emmet-api-0.83.7/emmet/api/routes/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.527336 emmet-api-0.83.7/emmet/api/routes/molecules/metal_binding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/metal_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/metal_binding/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/metal_binding/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.527336 emmet-api-0.83.7/emmet/api/routes/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/molecules/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14682 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.527336 emmet-api-0.83.7/emmet/api/routes/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19385 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/orbitals/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/orbitals/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.531337 emmet-api-0.83.7/emmet/api/routes/molecules/partial_charges/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/partial_charges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/partial_charges/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.531337 emmet-api-0.83.7/emmet/api/routes/molecules/partial_spins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/partial_spins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/partial_spins/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.531337 emmet-api-0.83.7/emmet/api/routes/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/redox/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/redox/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.531337 emmet-api-0.83.7/emmet/api/routes/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.531337 emmet-api-0.83.7/emmet/api/routes/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.531337 emmet-api-0.83.7/emmet/api/routes/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/thermo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.531337 emmet-api-0.83.7/emmet/api/routes/molecules/vibrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/vibrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-31 23:09:41.000000 emmet-api-0.83.7/emmet/api/routes/molecules/vibrations/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.531337 emmet-api-0.83.7/emmet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-31 23:09:47.000000 emmet-api-0.83.7/emmet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-05-31 23:09:47.000000 emmet-api-0.83.7/emmet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 23:09:47.000000 emmet-api-0.83.7/emmet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 23:09:47.000000 emmet-api-0.83.7/emmet_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-31 23:09:47.000000 emmet-api-0.83.7/emmet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 23:09:47.000000 emmet-api-0.83.7/emmet_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13875 2024-05-31 23:09:41.000000 emmet-api-0.83.7/material_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-31 23:09:41.000000 emmet-api-0.83.7/molecule_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.535337 emmet-api-0.83.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-31 23:09:41.000000 emmet-api-0.83.7/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-31 23:09:41.000000 emmet-api-0.83.7/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-05-31 23:09:41.000000 emmet-api-0.83.7/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-31 23:09:41.000000 emmet-api-0.83.7/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-05-31 23:09:41.000000 emmet-api-0.83.7/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-05-31 23:09:41.000000 emmet-api-0.83.7/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-05-31 23:09:41.000000 emmet-api-0.83.7/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 23:09:47.543336 emmet-api-0.83.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-31 23:09:41.000000 emmet-api-0.83.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-31 23:09:41.000000 emmet-api-0.83.7/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.535337 emmet-api-0.83.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.535337 emmet-api-0.83.7/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.535337 emmet-api-0.83.7/tests/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/_general_store/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.535337 emmet-api-0.83.7/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.507336 emmet-api-0.83.7/tests/legacy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.535337 emmet-api-0.83.7/tests/legacy/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/legacy/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/legacy/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.511336 emmet-api-0.83.7/tests/materials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.535337 emmet-api-0.83.7/tests/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.535337 emmet-api-0.83.7/tests/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.535337 emmet-api-0.83.7/tests/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/chemenv/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.535337 emmet-api-0.83.7/tests/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.535337 emmet-api-0.83.7/tests/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.535337 emmet-api-0.83.7/tests/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/electrodes/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/electrodes/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.535337 emmet-api-0.83.7/tests/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.535337 emmet-api-0.83.7/tests/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.539337 emmet-api-0.83.7/tests/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.539337 emmet-api-0.83.7/tests/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.539337 emmet-api-0.83.7/tests/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.539337 emmet-api-0.83.7/tests/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.539337 emmet-api-0.83.7/tests/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.539337 emmet-api-0.83.7/tests/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.539337 emmet-api-0.83.7/tests/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.539337 emmet-api-0.83.7/tests/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.539337 emmet-api-0.83.7/tests/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.539337 emmet-api-0.83.7/tests/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.539337 emmet-api-0.83.7/tests/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.539337 emmet-api-0.83.7/tests/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.543336 emmet-api-0.83.7/tests/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.543336 emmet-api-0.83.7/tests/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/materials/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.543336 emmet-api-0.83.7/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.543336 emmet-api-0.83.7/tests/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.543336 emmet-api-0.83.7/tests/molecules/metal_binding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/metal_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/metal_binding/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.543336 emmet-api-0.83.7/tests/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/molecules/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.543336 emmet-api-0.83.7/tests/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/orbitals/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.543336 emmet-api-0.83.7/tests/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/redox/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.543336 emmet-api-0.83.7/tests/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.543336 emmet-api-0.83.7/tests/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/tasks/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:47.543336 emmet-api-0.83.7/tests/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-31 23:09:41.000000 emmet-api-0.83.7/tests/molecules/thermo/test_query_operators.py
```

### Comparing `emmet-api-0.83.6rc3/Dockerfile` & `emmet-api-0.83.7/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM materialsproject/devops:python-3.1013.8 as base
+FROM materialsproject/devops:python-3.1013.10 as base
 RUN apt-get update && apt-get install -y --no-install-recommends libopenblas-dev libjpeg62 && apt-get clean
 
 FROM base as builder
 RUN apt-get update && apt-get install -y --no-install-recommends gcc git g++ cmake make libsnappy-dev wget && apt-get clean
 ENV PATH /root/.local/bin:$PATH
 WORKDIR /emmet-api
 ENV PIP_FLAGS "--user --no-cache-dir --compile"
```

### Comparing `emmet-api-0.83.6rc3/app.py` & `emmet-api-0.83.7/app.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/core/api.py` & `emmet-api-0.83.7/emmet/api/core/api.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/core/assets/mp_logo.svg` & `emmet-api-0.83.7/emmet/api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/core/assets/mp_logo_small.png` & `emmet-api-0.83.7/emmet/api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/core/documentation.py` & `emmet-api-0.83.7/emmet/api/core/documentation.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/core/global_header.py` & `emmet-api-0.83.7/emmet/api/core/global_header.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/core/settings.py` & `emmet-api-0.83.7/emmet/api/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/_consumer/query_operator.py` & `emmet-api-0.83.7/emmet/api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/_consumer/resources.py` & `emmet-api-0.83.7/emmet/api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/_general_store/query_operator.py` & `emmet-api-0.83.7/emmet/api/routes/_general_store/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/_general_store/resources.py` & `emmet-api-0.83.7/emmet/api/routes/_general_store/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/_messages/query_operator.py` & `emmet-api-0.83.7/emmet/api/routes/_messages/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/_messages/resources.py` & `emmet-api-0.83.7/emmet/api/routes/_messages/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/dois/resources.py` & `emmet-api-0.83.7/emmet/api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/legacy/jcesr/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/legacy/jcesr/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/legacy/jcesr/resources.py` & `emmet-api-0.83.7/emmet/api/routes/legacy/jcesr/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/absorption/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/absorption/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/alloys/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/alloys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/alloys/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/alloys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/bonds/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/bonds/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/charge_density/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/charge_density/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/charge_density/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/chemenv/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/chemenv/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/chemenv/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/chemenv/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/conversion_electrodes/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/conversion_electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/dielectric/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/dielectric/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/dielectric/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/elasticity/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/elasticity/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/elasticity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/electronic_structure/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/electronic_structure/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/electronic_structure/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/eos/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/eos/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/fermi/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/fermi/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/grain_boundary/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/grain_boundary/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/grain_boundary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/insertion_electrodes/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/insertion_electrodes/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/insertion_electrodes/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/insertion_electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/insertion_electrodes/utils.py` & `emmet-api-0.83.7/emmet/api/routes/materials/insertion_electrodes/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/magnetism/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/magnetism/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/magnetism/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/materials/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/materials/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/materials/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/materials/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/materials/utils.py` & `emmet-api-0.83.7/emmet/api/routes/materials/materials/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/mpcomplete/query_operator.py` & `emmet-api-0.83.7/emmet/api/routes/materials/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/mpcomplete/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/mpcomplete/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/oxidation_states/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/oxidation_states/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/oxidation_states/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/phonon/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/phonon/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/phonon/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/piezo/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/piezo/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/piezo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/provenance/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/provenance/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/robocrys/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/robocrys/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/robocrys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/similarity/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/similarity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/substrates/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/substrates/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/substrates/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/summary/hint_scheme.py` & `emmet-api-0.83.7/emmet/api/routes/materials/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/summary/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/summary/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/surface_properties/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/surface_properties/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/surface_properties/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/synthesis/data_adaptor.py` & `emmet-api-0.83.7/emmet/api/routes/materials/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py` & `emmet-api-0.83.7/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/synthesis/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/synthesis/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/synthesis/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/synthesis/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/synthesis/utils.py` & `emmet-api-0.83.7/emmet/api/routes/materials/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/tasks/hint_scheme.py` & `emmet-api-0.83.7/emmet/api/routes/materials/tasks/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/tasks/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/tasks/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/tasks/utils.py` & `emmet-api-0.83.7/emmet/api/routes/materials/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/thermo/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/thermo/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/xas/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/materials/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/materials/xas/resources.py` & `emmet-api-0.83.7/emmet/api/routes/materials/xas/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/association/resources.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/association/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/bonds/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/bonds/resources.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/metal_binding/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/metal_binding/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/metal_binding/resources.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/metal_binding/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/molecules/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/molecules/resources.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/orbitals/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/orbitals/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/orbitals/resources.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/orbitals/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/partial_charges/resources.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/partial_charges/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/partial_spins/resources.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/partial_spins/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/redox/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/redox/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/redox/resources.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/redox/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/summary/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/summary/resources.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/tasks/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/tasks/resources.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/tasks/utils.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/thermo/query_operators.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/thermo/resources.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/utils.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet/api/routes/molecules/vibrations/resources.py` & `emmet-api-0.83.7/emmet/api/routes/molecules/vibrations/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/emmet_api.egg-info/SOURCES.txt` & `emmet-api-0.83.7/emmet_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/material_resources.py` & `emmet-api-0.83.7/material_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/molecule_resources.py` & `emmet-api-0.83.7/molecule_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/requirements/deployment.txt` & `emmet-api-0.83.7/requirements/deployment.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --output-file=emmet/emmet-api/requirements/deployment.txt emmet/emmet-api/setup.py python/requirements.txt
 #
 aioitertools==0.11.0
     # via maggma
-annotated-types==0.6.0
+annotated-types==0.7.0
     # via pydantic
-anyio==4.3.0
+anyio==4.4.0
     # via
     #   httpx
     #   starlette
     #   watchfiles
 asgi-logger==0.1.0
     # via emmet-api (emmet/emmet-api/setup.py)
 asgiref==3.8.1
@@ -23,19 +23,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.3
     # via paramiko
 blinker==1.8.2
     # via flask
-boto3==1.34.108
+boto3==1.34.113
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
-botocore==1.34.108
+botocore==1.34.113
     # via
     #   boto3
     #   s3transfer
 bytecode==0.15.1
     # via ddtrace
 cattrs==23.2.3
     # via ddtrace
@@ -87,15 +87,15 @@
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
 fastapi-cli==0.0.4
     # via fastapi
 flask==3.0.3
     # via mongogrant
-fonttools==4.51.0
+fonttools==4.52.1
     # via matplotlib
 future==1.0.0
     # via uncertainties
 gunicorn==22.0.0
     # via emmet-api (emmet/emmet-api/setup.py)
 h11==0.14.0
     # via
@@ -149,15 +149,15 @@
     #   pymatgen
 mdurl==0.1.2
     # via markdown-it-py
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2024.5.15
+monty==2024.5.24
     # via
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
@@ -195,15 +195,15 @@
     #   pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pillow==10.3.0
     # via matplotlib
 plotly==5.22.0
     # via pymatgen
-protobuf==5.26.1
+protobuf==5.27.0
     # via ddtrace
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pycparser==2.22
     # via cffi
@@ -257,15 +257,15 @@
     #   uvicorn
 pyzmq==26.0.3
     # via maggma
 referencing==0.35.1
     # via
     #   jsonschema
     #   jsonschema-specifications
-requests==2.32.0
+requests==2.32.2
     # via
     #   mongogrant
     #   pymatgen
 rich==13.7.1
     # via typer
 rpds-py==0.18.1
     # via
@@ -275,15 +275,15 @@
     # via
     #   maggma
     #   pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 s3transfer==0.10.1
     # via boto3
-scipy==1.13.0
+scipy==1.13.1
     # via
     #   -r python/requirements.txt
     #   pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (emmet/emmet-api/setup.py)
@@ -319,15 +319,15 @@
     # via plotly
 tqdm==4.66.4
     # via
     #   maggma
     #   pymatgen
 typer==0.12.3
     # via fastapi-cli
-typing-extensions==4.11.0
+typing-extensions==4.12.0
     # via
     #   anyio
     #   asgiref
     #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
@@ -348,22 +348,22 @@
     #   requests
 uvicorn[standard]==0.29.0
     # via
     #   fastapi
     #   maggma
 uvloop==0.19.0
     # via uvicorn
-watchfiles==0.21.0
+watchfiles==0.22.0
     # via uvicorn
 websockets==12.0
     # via uvicorn
 werkzeug==3.0.3
     # via flask
 wrapt==1.16.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.18.2
+zipp==3.19.0
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.83.6rc3/requirements/ubuntu-latest_py3.10.txt` & `emmet-api-0.83.7/requirements/ubuntu-latest_py3.11.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.11.txt
 #
 aioitertools==0.11.0
     # via maggma
-annotated-types==0.6.0
+annotated-types==0.7.0
     # via pydantic
 anyio==4.3.0
     # via
     #   httpx
     #   starlette
     #   watchfiles
 asgi-logger==0.1.0
@@ -23,19 +23,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.3
     # via paramiko
 blinker==1.8.2
     # via flask
-boto3==1.34.99
+boto3==1.34.112
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.99
+botocore==1.34.112
     # via
     #   boto3
     #   s3transfer
 bytecode==0.15.1
     # via ddtrace
 cattrs==23.2.3
     # via ddtrace
@@ -60,39 +60,34 @@
     # via matplotlib
 cryptography==42.0.7
     # via paramiko
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.8.4
+ddtrace==2.8.5
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.6.1
     # via
     #   email-validator
     #   maggma
     #   pymongo
 email-validator==2.1.1
     # via fastapi
 emmet-core==0.83.6
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
-exceptiongroup==1.2.1
-    # via
-    #   anyio
-    #   cattrs
 fastapi==0.111.0
     # via
     #   emmet-api (setup.py)
-    #   fastapi-cli
     #   maggma
-fastapi-cli==0.0.2
+fastapi-cli==0.0.4
     # via fastapi
 flask==3.0.3
     # via mongogrant
 fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
@@ -132,31 +127,31 @@
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
-maggma==0.66.0
+maggma==0.67.0
     # via emmet-api (setup.py)
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via
     #   jinja2
     #   werkzeug
-matplotlib==3.8.4
+matplotlib==3.9.0
     # via pymatgen
 mdurl==0.1.2
     # via markdown-it-py
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2024.4.17
+monty==2024.5.15
     # via
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
@@ -191,15 +186,15 @@
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pillow==10.3.0
     # via matplotlib
 plotly==5.22.0
     # via pymatgen
-protobuf==5.26.1
+protobuf==5.27.0
     # via ddtrace
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pycparser==2.22
     # via cffi
@@ -221,15 +216,15 @@
     # via rich
 pymatgen==2024.5.1
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
-pymongo==4.7.1
+pymongo==4.7.2
     # via
     #   maggma
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.1.2
     # via matplotlib
@@ -253,15 +248,15 @@
     #   uvicorn
 pyzmq==26.0.3
     # via maggma
 referencing==0.35.1
     # via
     #   jsonschema
     #   jsonschema-specifications
-requests==2.31.0
+requests==2.32.2
     # via
     #   mongogrant
     #   pymatgen
 rich==13.7.1
     # via typer
 rpds-py==0.18.1
     # via
@@ -271,15 +266,15 @@
     # via
     #   maggma
     #   pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 s3transfer==0.10.1
     # via boto3
-scipy==1.13.0
+scipy==1.13.1
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
 shapely==2.0.4
     # via
@@ -315,50 +310,45 @@
     # via
     #   maggma
     #   pymatgen
 typer==0.12.3
     # via fastapi-cli
 typing-extensions==4.11.0
     # via
-    #   anyio
-    #   asgiref
-    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   pydantic
     #   pydantic-core
     #   pydash
     #   typer
-    #   uvicorn
 tzdata==2024.1
     # via pandas
-ujson==5.9.0
+ujson==5.10.0
     # via fastapi
 uncertainties==3.1.7
     # via pymatgen
 urllib3==2.2.1
     # via
     #   botocore
     #   requests
 uvicorn[standard]==0.29.0
     # via
     #   fastapi
-    #   fastapi-cli
     #   maggma
 uvloop==0.19.0
     # via uvicorn
 watchfiles==0.21.0
     # via uvicorn
 websockets==12.0
     # via uvicorn
 werkzeug==3.0.3
     # via flask
 wrapt==1.16.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.18.1
+zipp==3.18.2
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.83.6rc3/requirements/ubuntu-latest_py3.10_extras.txt` & `emmet-api-0.83.7/requirements/ubuntu-latest_py3.11_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.11_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
-annotated-types==0.6.0
+annotated-types==0.7.0
     # via pydantic
 anyio==4.3.0
     # via
     #   httpx
     #   starlette
     #   watchfiles
 asgi-logger==0.1.0
@@ -23,19 +23,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.3
     # via paramiko
 blinker==1.8.2
     # via flask
-boto3==1.34.99
+boto3==1.34.112
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.99
+botocore==1.34.112
     # via
     #   boto3
     #   s3transfer
 bracex==2.4
     # via wcmatch
 bytecode==0.15.1
     # via ddtrace
@@ -72,15 +72,15 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.8.4
+ddtrace==2.8.5
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.8
     # via virtualenv
 dnspython==2.6.1
     # via
@@ -89,39 +89,33 @@
     #   pymongo
 email-validator==2.1.1
     # via fastapi
 emmet-core==0.83.6
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
-exceptiongroup==1.2.1
-    # via
-    #   anyio
-    #   cattrs
-    #   pytest
 fastapi==0.111.0
     # via
     #   emmet-api (setup.py)
-    #   fastapi-cli
     #   maggma
-fastapi-cli==0.0.2
+fastapi-cli==0.0.4
     # via fastapi
 filelock==3.14.0
     # via virtualenv
 flake8==7.0.0
     # via emmet-api (setup.py)
 flask==3.0.3
     # via mongogrant
 fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.44.0
+griffe==0.45.2
     # via mkdocstrings-python
 gunicorn==22.0.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via
     #   httpcore
     #   uvicorn
@@ -169,15 +163,15 @@
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.66.0
+maggma==0.67.0
     # via emmet-api (setup.py)
 markdown==3.6
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -187,15 +181,15 @@
 markupsafe==2.1.5
     # via
     #   jinja2
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocstrings
     #   werkzeug
-matplotlib==3.8.4
+matplotlib==3.9.0
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via
@@ -226,21 +220,21 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.8.0
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.25.1
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.10.0
+mkdocstrings-python==1.10.3
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2024.4.17
+monty==2024.5.15
     # via
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
@@ -287,26 +281,26 @@
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pathspec==0.12.1
     # via mkdocs
 pillow==10.3.0
     # via matplotlib
-platformdirs==4.2.1
+platformdirs==4.2.2
     # via
     #   mkdocs-get-deps
     #   mkdocstrings
     #   virtualenv
 plotly==5.22.0
     # via pymatgen
 pluggy==1.5.0
     # via pytest
-pre-commit==3.7.0
+pre-commit==3.7.1
     # via emmet-api (setup.py)
-protobuf==5.26.1
+protobuf==5.27.0
     # via ddtrace
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pycodestyle==2.11.1
     # via
@@ -332,33 +326,33 @@
     # via emmet-api (setup.py)
 pyflakes==3.2.0
     # via flake8
 pygments==2.18.0
     # via
     #   mkdocs-material
     #   rich
-pymatgen==2024.4.13
+pymatgen==2024.5.1
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
 pymdown-extensions==10.8.1
     # via
     #   mkdocs-material
     #   mkdocstrings
-pymongo==4.7.1
+pymongo==4.7.2
     # via
     #   maggma
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.1.2
     # via matplotlib
-pytest==8.2.0
+pytest==8.2.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
 pytest-cov==5.0.0
     # via emmet-api (setup.py)
 python-dateutil==2.9.0.post0
     # via
@@ -389,15 +383,15 @@
     # via mkdocs
 pyzmq==26.0.3
     # via maggma
 referencing==0.35.1
     # via
     #   jsonschema
     #   jsonschema-specifications
-requests==2.31.0
+requests==2.32.2
     # via
     #   mongogrant
     #   pymatgen
 rich==13.7.1
     # via typer
 rpds-py==0.18.1
     # via
@@ -407,15 +401,15 @@
     # via
     #   maggma
     #   pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 s3transfer==0.10.1
     # via boto3
-scipy==1.13.0
+scipy==1.13.1
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
 shapely==2.0.4
     # via
@@ -446,79 +440,69 @@
     # via fastapi
 sympy==1.12
     # via pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.3.0
     # via plotly
-tomli==2.0.1
-    # via
-    #   coverage
-    #   mypy
-    #   pytest
 tornado==6.4
     # via livereload
 tqdm==4.66.4
     # via
     #   maggma
     #   pymatgen
 typer==0.12.3
     # via fastapi-cli
-types-requests==2.31.0.20240406
+types-requests==2.32.0.20240523
     # via emmet-api (setup.py)
-types-setuptools==69.5.0.20240423
+types-setuptools==70.0.0.20240523
     # via emmet-api (setup.py)
 typing-extensions==4.11.0
     # via
-    #   anyio
-    #   asgiref
-    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   mypy
     #   pydantic
     #   pydantic-core
     #   pydash
     #   typer
-    #   uvicorn
 tzdata==2024.1
     # via pandas
-ujson==5.9.0
+ujson==5.10.0
     # via fastapi
 uncertainties==3.1.7
     # via pymatgen
 urllib3==2.2.1
     # via
     #   botocore
     #   requests
     #   types-requests
 uvicorn[standard]==0.29.0
     # via
     #   fastapi
-    #   fastapi-cli
     #   maggma
 uvloop==0.19.0
     # via uvicorn
-virtualenv==20.26.1
+virtualenv==20.26.2
     # via pre-commit
-watchdog==4.0.0
+watchdog==4.0.1
     # via mkdocs
 watchfiles==0.21.0
     # via uvicorn
-wcmatch==8.5.1
+wcmatch==8.5.2
     # via mkdocs-awesome-pages-plugin
 websockets==12.0
     # via uvicorn
 werkzeug==3.0.3
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.16.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.18.1
+zipp==3.18.2
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.83.6rc3/requirements/ubuntu-latest_py3.11.txt` & `emmet-api-0.83.7/requirements/ubuntu-latest_py3.10.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.11.txt
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt
 #
 aioitertools==0.11.0
     # via maggma
-annotated-types==0.6.0
+annotated-types==0.7.0
     # via pydantic
 anyio==4.3.0
     # via
     #   httpx
     #   starlette
     #   watchfiles
 asgi-logger==0.1.0
@@ -23,19 +23,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.3
     # via paramiko
 blinker==1.8.2
     # via flask
-boto3==1.34.99
+boto3==1.34.112
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.99
+botocore==1.34.112
     # via
     #   boto3
     #   s3transfer
 bytecode==0.15.1
     # via ddtrace
 cattrs==23.2.3
     # via ddtrace
@@ -60,35 +60,38 @@
     # via matplotlib
 cryptography==42.0.7
     # via paramiko
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.8.4
+ddtrace==2.8.5
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.6.1
     # via
     #   email-validator
     #   maggma
     #   pymongo
 email-validator==2.1.1
     # via fastapi
 emmet-core==0.83.6
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
+exceptiongroup==1.2.1
+    # via
+    #   anyio
+    #   cattrs
 fastapi==0.111.0
     # via
     #   emmet-api (setup.py)
-    #   fastapi-cli
     #   maggma
-fastapi-cli==0.0.2
+fastapi-cli==0.0.4
     # via fastapi
 flask==3.0.3
     # via mongogrant
 fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
@@ -128,31 +131,31 @@
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
-maggma==0.66.0
+maggma==0.67.0
     # via emmet-api (setup.py)
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via
     #   jinja2
     #   werkzeug
-matplotlib==3.8.4
+matplotlib==3.9.0
     # via pymatgen
 mdurl==0.1.2
     # via markdown-it-py
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2024.4.17
+monty==2024.5.15
     # via
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
@@ -187,15 +190,15 @@
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pillow==10.3.0
     # via matplotlib
 plotly==5.22.0
     # via pymatgen
-protobuf==5.26.1
+protobuf==5.27.0
     # via ddtrace
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pycparser==2.22
     # via cffi
@@ -217,15 +220,15 @@
     # via rich
 pymatgen==2024.5.1
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
-pymongo==4.7.1
+pymongo==4.7.2
     # via
     #   maggma
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.1.2
     # via matplotlib
@@ -249,15 +252,15 @@
     #   uvicorn
 pyzmq==26.0.3
     # via maggma
 referencing==0.35.1
     # via
     #   jsonschema
     #   jsonschema-specifications
-requests==2.31.0
+requests==2.32.2
     # via
     #   mongogrant
     #   pymatgen
 rich==13.7.1
     # via typer
 rpds-py==0.18.1
     # via
@@ -267,15 +270,15 @@
     # via
     #   maggma
     #   pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 s3transfer==0.10.1
     # via boto3
-scipy==1.13.0
+scipy==1.13.1
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
 shapely==2.0.4
     # via
@@ -311,46 +314,49 @@
     # via
     #   maggma
     #   pymatgen
 typer==0.12.3
     # via fastapi-cli
 typing-extensions==4.11.0
     # via
+    #   anyio
+    #   asgiref
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   pydantic
     #   pydantic-core
     #   pydash
     #   typer
+    #   uvicorn
 tzdata==2024.1
     # via pandas
-ujson==5.9.0
+ujson==5.10.0
     # via fastapi
 uncertainties==3.1.7
     # via pymatgen
 urllib3==2.2.1
     # via
     #   botocore
     #   requests
 uvicorn[standard]==0.29.0
     # via
     #   fastapi
-    #   fastapi-cli
     #   maggma
 uvloop==0.19.0
     # via uvicorn
 watchfiles==0.21.0
     # via uvicorn
 websockets==12.0
     # via uvicorn
 werkzeug==3.0.3
     # via flask
 wrapt==1.16.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.18.1
+zipp==3.18.2
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.83.6rc3/requirements/ubuntu-latest_py3.11_extras.txt` & `emmet-api-0.83.7/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.11_extras.txt
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
-annotated-types==0.6.0
+annotated-types==0.7.0
     # via pydantic
 anyio==4.3.0
     # via
     #   httpx
     #   starlette
     #   watchfiles
 asgi-logger==0.1.0
@@ -23,19 +23,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.3
     # via paramiko
 blinker==1.8.2
     # via flask
-boto3==1.34.99
+boto3==1.34.112
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.99
+botocore==1.34.112
     # via
     #   boto3
     #   s3transfer
 bracex==2.4
     # via wcmatch
 bytecode==0.15.1
     # via ddtrace
@@ -72,15 +72,15 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.8.4
+ddtrace==2.8.5
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.8
     # via virtualenv
 dnspython==2.6.1
     # via
@@ -89,34 +89,38 @@
     #   pymongo
 email-validator==2.1.1
     # via fastapi
 emmet-core==0.83.6
     # via emmet-api (setup.py)
 envier==0.5.1
     # via ddtrace
+exceptiongroup==1.2.1
+    # via
+    #   anyio
+    #   cattrs
+    #   pytest
 fastapi==0.111.0
     # via
     #   emmet-api (setup.py)
-    #   fastapi-cli
     #   maggma
-fastapi-cli==0.0.2
+fastapi-cli==0.0.4
     # via fastapi
 filelock==3.14.0
     # via virtualenv
 flake8==7.0.0
     # via emmet-api (setup.py)
 flask==3.0.3
     # via mongogrant
 fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.44.0
+griffe==0.45.2
     # via mkdocstrings-python
 gunicorn==22.0.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via
     #   httpcore
     #   uvicorn
@@ -164,15 +168,15 @@
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.66.0
+maggma==0.67.0
     # via emmet-api (setup.py)
 markdown==3.6
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -182,15 +186,15 @@
 markupsafe==2.1.5
     # via
     #   jinja2
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocstrings
     #   werkzeug
-matplotlib==3.8.4
+matplotlib==3.9.0
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via
@@ -221,21 +225,21 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.8.0
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.25.1
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.10.0
+mkdocstrings-python==1.10.3
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2024.4.17
+monty==2024.5.15
     # via
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
@@ -282,26 +286,26 @@
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pathspec==0.12.1
     # via mkdocs
 pillow==10.3.0
     # via matplotlib
-platformdirs==4.2.1
+platformdirs==4.2.2
     # via
     #   mkdocs-get-deps
     #   mkdocstrings
     #   virtualenv
 plotly==5.22.0
     # via pymatgen
 pluggy==1.5.0
     # via pytest
-pre-commit==3.7.0
+pre-commit==3.7.1
     # via emmet-api (setup.py)
-protobuf==5.26.1
+protobuf==5.27.0
     # via ddtrace
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pycodestyle==2.11.1
     # via
@@ -327,33 +331,33 @@
     # via emmet-api (setup.py)
 pyflakes==3.2.0
     # via flake8
 pygments==2.18.0
     # via
     #   mkdocs-material
     #   rich
-pymatgen==2024.4.13
+pymatgen==2024.5.1
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
 pymdown-extensions==10.8.1
     # via
     #   mkdocs-material
     #   mkdocstrings
-pymongo==4.7.1
+pymongo==4.7.2
     # via
     #   maggma
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.1.2
     # via matplotlib
-pytest==8.2.0
+pytest==8.2.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
 pytest-cov==5.0.0
     # via emmet-api (setup.py)
 python-dateutil==2.9.0.post0
     # via
@@ -384,15 +388,15 @@
     # via mkdocs
 pyzmq==26.0.3
     # via maggma
 referencing==0.35.1
     # via
     #   jsonschema
     #   jsonschema-specifications
-requests==2.31.0
+requests==2.32.2
     # via
     #   mongogrant
     #   pymatgen
 rich==13.7.1
     # via typer
 rpds-py==0.18.1
     # via
@@ -402,15 +406,15 @@
     # via
     #   maggma
     #   pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 s3transfer==0.10.1
     # via boto3
-scipy==1.13.0
+scipy==1.13.1
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
 shapely==2.0.4
     # via
@@ -441,70 +445,78 @@
     # via fastapi
 sympy==1.12
     # via pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.3.0
     # via plotly
+tomli==2.0.1
+    # via
+    #   coverage
+    #   mypy
+    #   pytest
 tornado==6.4
     # via livereload
 tqdm==4.66.4
     # via
     #   maggma
     #   pymatgen
 typer==0.12.3
     # via fastapi-cli
-types-requests==2.31.0.20240406
+types-requests==2.32.0.20240523
     # via emmet-api (setup.py)
-types-setuptools==69.5.0.20240423
+types-setuptools==70.0.0.20240523
     # via emmet-api (setup.py)
 typing-extensions==4.11.0
     # via
+    #   anyio
+    #   asgiref
+    #   cattrs
     #   ddtrace
     #   emmet-core
     #   fastapi
     #   mypy
     #   pydantic
     #   pydantic-core
     #   pydash
     #   typer
+    #   uvicorn
 tzdata==2024.1
     # via pandas
-ujson==5.9.0
+ujson==5.10.0
     # via fastapi
 uncertainties==3.1.7
     # via pymatgen
 urllib3==2.2.1
     # via
     #   botocore
     #   requests
     #   types-requests
 uvicorn[standard]==0.29.0
     # via
     #   fastapi
-    #   fastapi-cli
     #   maggma
 uvloop==0.19.0
     # via uvicorn
-virtualenv==20.26.1
+virtualenv==20.26.2
     # via pre-commit
-watchdog==4.0.0
+watchdog==4.0.1
     # via mkdocs
 watchfiles==0.21.0
     # via uvicorn
-wcmatch==8.5.1
+wcmatch==8.5.2
     # via mkdocs-awesome-pages-plugin
 websockets==12.0
     # via uvicorn
 werkzeug==3.0.3
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.16.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.18.1
+zipp==3.18.2
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.83.6rc3/requirements/ubuntu-latest_py3.9.txt` & `emmet-api-0.83.7/requirements/ubuntu-latest_py3.9.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt
 #
 aioitertools==0.11.0
     # via maggma
-annotated-types==0.6.0
+annotated-types==0.7.0
     # via pydantic
 anyio==4.3.0
     # via
     #   httpx
     #   starlette
     #   watchfiles
 asgi-logger==0.1.0
@@ -23,19 +23,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.3
     # via paramiko
 blinker==1.8.2
     # via flask
-boto3==1.34.99
+boto3==1.34.112
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.99
+botocore==1.34.112
     # via
     #   boto3
     #   s3transfer
 bytecode==0.15.1
     # via ddtrace
 cattrs==23.2.3
     # via ddtrace
@@ -60,15 +60,15 @@
     # via matplotlib
 cryptography==42.0.7
     # via paramiko
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.8.4
+ddtrace==2.8.5
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.6.1
     # via
     #   email-validator
     #   maggma
@@ -82,17 +82,16 @@
 exceptiongroup==1.2.1
     # via
     #   anyio
     #   cattrs
 fastapi==0.111.0
     # via
     #   emmet-api (setup.py)
-    #   fastapi-cli
     #   maggma
-fastapi-cli==0.0.2
+fastapi-cli==0.0.4
     # via fastapi
 flask==3.0.3
     # via mongogrant
 fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
@@ -138,31 +137,31 @@
     # via maggma
 jsonschema-specifications==2023.12.1
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
-maggma==0.66.0
+maggma==0.67.0
     # via emmet-api (setup.py)
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via
     #   jinja2
     #   werkzeug
-matplotlib==3.8.4
+matplotlib==3.9.0
     # via pymatgen
 mdurl==0.1.2
     # via markdown-it-py
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2024.4.17
+monty==2024.5.15
     # via
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
@@ -197,15 +196,15 @@
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pillow==10.3.0
     # via matplotlib
 plotly==5.22.0
     # via pymatgen
-protobuf==5.26.1
+protobuf==5.27.0
     # via ddtrace
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pycparser==2.22
     # via cffi
@@ -227,15 +226,15 @@
     # via rich
 pymatgen==2024.5.1
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
-pymongo==4.7.1
+pymongo==4.7.2
     # via
     #   maggma
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.1.2
     # via matplotlib
@@ -259,15 +258,15 @@
     #   uvicorn
 pyzmq==26.0.3
     # via maggma
 referencing==0.35.1
     # via
     #   jsonschema
     #   jsonschema-specifications
-requests==2.31.0
+requests==2.32.2
     # via
     #   mongogrant
     #   pymatgen
 rich==13.7.1
     # via typer
 rpds-py==0.18.1
     # via
@@ -277,15 +276,15 @@
     # via
     #   maggma
     #   pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 s3transfer==0.10.1
     # via boto3
-scipy==1.13.0
+scipy==1.13.1
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
 shapely==2.0.4
     # via
@@ -337,39 +336,38 @@
     #   pydantic-core
     #   pydash
     #   starlette
     #   typer
     #   uvicorn
 tzdata==2024.1
     # via pandas
-ujson==5.9.0
+ujson==5.10.0
     # via fastapi
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.18
     # via
     #   botocore
     #   requests
 uvicorn[standard]==0.29.0
     # via
     #   fastapi
-    #   fastapi-cli
     #   maggma
 uvloop==0.19.0
     # via uvicorn
 watchfiles==0.21.0
     # via uvicorn
 websockets==12.0
     # via uvicorn
 werkzeug==3.0.3
     # via flask
 wrapt==1.16.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.18.1
+zipp==3.18.2
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.83.6rc3/requirements/ubuntu-latest_py3.9_extras.txt` & `emmet-api-0.83.7/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt
 #
 aioitertools==0.11.0
     # via maggma
-annotated-types==0.6.0
+annotated-types==0.7.0
     # via pydantic
 anyio==4.3.0
     # via
     #   httpx
     #   starlette
     #   watchfiles
 asgi-logger==0.1.0
@@ -23,19 +23,19 @@
     #   ddtrace
     #   jsonschema
     #   referencing
 bcrypt==4.1.3
     # via paramiko
 blinker==1.8.2
     # via flask
-boto3==1.34.99
+boto3==1.34.112
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.34.99
+botocore==1.34.112
     # via
     #   boto3
     #   s3transfer
 bracex==2.4
     # via wcmatch
 bytecode==0.15.1
     # via ddtrace
@@ -72,15 +72,15 @@
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.12.1
     # via matplotlib
 ddsketch==3.0.1
     # via ddtrace
-ddtrace==2.8.4
+ddtrace==2.8.5
     # via emmet-api (setup.py)
 deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.8
     # via virtualenv
 dnspython==2.6.1
     # via
@@ -97,31 +97,30 @@
     # via
     #   anyio
     #   cattrs
     #   pytest
 fastapi==0.111.0
     # via
     #   emmet-api (setup.py)
-    #   fastapi-cli
     #   maggma
-fastapi-cli==0.0.2
+fastapi-cli==0.0.4
     # via fastapi
 filelock==3.14.0
     # via virtualenv
 flake8==7.0.0
     # via emmet-api (setup.py)
 flask==3.0.3
     # via mongogrant
 fonttools==4.51.0
     # via matplotlib
 future==1.0.0
     # via uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.44.0
+griffe==0.45.2
     # via mkdocstrings-python
 gunicorn==22.0.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via
     #   httpcore
     #   uvicorn
@@ -179,15 +178,15 @@
     # via jsonschema
 kiwisolver==1.4.5
     # via matplotlib
 latexcodec==3.0.0
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.66.0
+maggma==0.67.0
     # via emmet-api (setup.py)
 markdown==3.6
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -197,15 +196,15 @@
 markupsafe==2.1.5
     # via
     #   jinja2
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocstrings
     #   werkzeug
-matplotlib==3.8.4
+matplotlib==3.9.0
     # via pymatgen
 mccabe==0.7.0
     # via flake8
 mdurl==0.1.2
     # via markdown-it-py
 mergedeep==1.3.4
     # via
@@ -236,21 +235,21 @@
     #   mkdocs-material
 mkdocs-minify-plugin==0.8.0
     # via emmet-api (setup.py)
 mkdocstrings[python]==0.25.1
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.10.0
+mkdocstrings-python==1.10.3
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
-monty==2024.4.17
+monty==2024.5.15
     # via
     #   emmet-core
     #   maggma
     #   pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
@@ -297,26 +296,26 @@
     # via pymatgen
 paramiko==3.4.0
     # via sshtunnel
 pathspec==0.12.1
     # via mkdocs
 pillow==10.3.0
     # via matplotlib
-platformdirs==4.2.1
+platformdirs==4.2.2
     # via
     #   mkdocs-get-deps
     #   mkdocstrings
     #   virtualenv
 plotly==5.22.0
     # via pymatgen
 pluggy==1.5.0
     # via pytest
-pre-commit==3.7.0
+pre-commit==3.7.1
     # via emmet-api (setup.py)
-protobuf==5.26.1
+protobuf==5.27.0
     # via ddtrace
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
 pycodestyle==2.11.1
     # via
@@ -342,33 +341,33 @@
     # via emmet-api (setup.py)
 pyflakes==3.2.0
     # via flake8
 pygments==2.18.0
     # via
     #   mkdocs-material
     #   rich
-pymatgen==2024.4.13
+pymatgen==2024.5.1
     # via
     #   emmet-core
     #   pymatgen-analysis-alloys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-api (setup.py)
 pymdown-extensions==10.8.1
     # via
     #   mkdocs-material
     #   mkdocstrings
-pymongo==4.7.1
+pymongo==4.7.2
     # via
     #   maggma
     #   mongogrant
 pynacl==1.5.0
     # via paramiko
 pyparsing==3.1.2
     # via matplotlib
-pytest==8.2.0
+pytest==8.2.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
 pytest-cov==5.0.0
     # via emmet-api (setup.py)
 python-dateutil==2.9.0.post0
     # via
@@ -399,15 +398,15 @@
     # via mkdocs
 pyzmq==26.0.3
     # via maggma
 referencing==0.35.1
     # via
     #   jsonschema
     #   jsonschema-specifications
-requests==2.31.0
+requests==2.32.2
     # via
     #   mongogrant
     #   pymatgen
 rich==13.7.1
     # via typer
 rpds-py==0.18.1
     # via
@@ -417,15 +416,15 @@
     # via
     #   maggma
     #   pymatgen
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
 s3transfer==0.10.1
     # via boto3
-scipy==1.13.0
+scipy==1.13.1
     # via pymatgen
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.3
     # via emmet-api (setup.py)
 shapely==2.0.4
     # via
@@ -471,15 +470,15 @@
     # via
     #   maggma
     #   pymatgen
 typer==0.12.3
     # via fastapi-cli
 types-requests==2.31.0.6
     # via emmet-api (setup.py)
-types-setuptools==69.5.0.20240423
+types-setuptools==70.0.0.20240523
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.14
     # via types-requests
 typing-extensions==4.11.0
     # via
     #   aioitertools
     #   anyio
@@ -495,47 +494,46 @@
     #   pydantic-core
     #   pydash
     #   starlette
     #   typer
     #   uvicorn
 tzdata==2024.1
     # via pandas
-ujson==5.9.0
+ujson==5.10.0
     # via fastapi
 uncertainties==3.1.7
     # via pymatgen
 urllib3==1.26.18
     # via
     #   botocore
     #   requests
 uvicorn[standard]==0.29.0
     # via
     #   fastapi
-    #   fastapi-cli
     #   maggma
 uvloop==0.19.0
     # via uvicorn
-virtualenv==20.26.1
+virtualenv==20.26.2
     # via pre-commit
-watchdog==4.0.0
+watchdog==4.0.1
     # via mkdocs
 watchfiles==0.21.0
     # via uvicorn
-wcmatch==8.5.1
+wcmatch==8.5.2
     # via mkdocs-awesome-pages-plugin
 websockets==12.0
     # via uvicorn
 werkzeug==3.0.3
     # via flask
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.16.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
-zipp==3.18.1
+zipp==3.18.2
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.83.6rc3/setup.py` & `emmet-api-0.83.7/setup.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/start.sh` & `emmet-api-0.83.7/start.sh`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/_consumer/test_query_operators.py` & `emmet-api-0.83.7/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/_general_store/test_query_operators.py` & `emmet-api-0.83.7/tests/_general_store/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/core/test_mapi.py` & `emmet-api-0.83.7/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/legacy/molecules/test_query_operators.py` & `emmet-api-0.83.7/tests/legacy/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/bonds/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/charge_density/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/charge_density/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/chemenv/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/chemenv/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/dielectric/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/dielectric/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/elasticity/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/elasticity/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/electrodes/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/electrodes/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/electrodes/test_utils.py` & `emmet-api-0.83.7/tests/materials/electrodes/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/electronic_structure/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/electronic_structure/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/grain_boundary/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/grain_boundary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/magnetism/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/magnetism/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/materials/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/materials/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/materials/test_utils.py` & `emmet-api-0.83.7/tests/materials/materials/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/mpcomplete/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/mpcomplete/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/oxidation_states/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/oxidation_states/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/piezo/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/piezo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/robocrys/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/robocrys/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/substrates/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/substrates/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/summary/test_hint_scheme.py` & `emmet-api-0.83.7/tests/materials/summary/test_hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/summary/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/surface_properties/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/surface_properties/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/synthesis/test_adaptor.py` & `emmet-api-0.83.7/tests/materials/synthesis/test_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/synthesis/test_adaptor_synpro.py` & `emmet-api-0.83.7/tests/materials/synthesis/test_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/synthesis/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/synthesis/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/synthesis/test_utils.py` & `emmet-api-0.83.7/tests/materials/synthesis/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/tasks/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/tasks/test_utils.py` & `emmet-api-0.83.7/tests/materials/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/materials/xas/test_query_operators.py` & `emmet-api-0.83.7/tests/materials/xas/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/molecules/bonds/test_query_operators.py` & `emmet-api-0.83.7/tests/molecules/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/molecules/metal_binding/test_query_operators.py` & `emmet-api-0.83.7/tests/molecules/metal_binding/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/molecules/molecules/test_query_operators.py` & `emmet-api-0.83.7/tests/molecules/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/molecules/orbitals/test_query_operators.py` & `emmet-api-0.83.7/tests/molecules/orbitals/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/molecules/redox/test_query_operators.py` & `emmet-api-0.83.7/tests/molecules/redox/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/molecules/summary/test_query_operators.py` & `emmet-api-0.83.7/tests/molecules/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/molecules/tasks/test_query_operators.py` & `emmet-api-0.83.7/tests/molecules/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/molecules/tasks/test_utils.py` & `emmet-api-0.83.7/tests/molecules/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.83.6rc3/tests/molecules/thermo/test_query_operators.py` & `emmet-api-0.83.7/tests/molecules/thermo/test_query_operators.py`

 * *Files identical despite different names*

