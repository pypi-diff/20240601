# Comparing `tmp/coordinax-0.4.3.tar.gz` & `tmp/coordinax-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Apr  2 19:57:40 2024, max compression
+gzip compressed data, last modified: Sat Jun  1 17:04:11 2024, max compression
```

## Comparing `coordinax-0.4.3.tar` & `coordinax-0.5.tar`

### file list

```diff
@@ -1,82 +1,86 @@
--rw-r--r--   0        0        0      373 2024-04-02 19:57:40.000000 coordinax-0.4.3/.copier-answers.yml
--rw-r--r--   0        0        0      125 2024-04-02 19:57:40.000000 coordinax-0.4.3/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-04-02 19:57:40.000000 coordinax-0.4.3/.gitattributes
--rw-r--r--   0        0        0     2558 2024-04-02 19:57:40.000000 coordinax-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-04-02 19:57:40.000000 coordinax-0.4.3/.readthedocs.yml
--rw-r--r--   0        0        0      439 2024-04-02 19:57:40.000000 coordinax-0.4.3/conftest.py
--rw-r--r--   0        0        0     2819 2024-04-02 19:57:40.000000 coordinax-0.4.3/noxfile.py
--rw-r--r--   0        0        0     2386 2024-04-02 19:57:40.000000 coordinax-0.4.3/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-04-02 19:57:40.000000 coordinax-0.4.3/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-04-02 19:57:40.000000 coordinax-0.4.3/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1540 2024-04-02 19:57:40.000000 coordinax-0.4.3/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1655 2024-04-02 19:57:40.000000 coordinax-0.4.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      872 2024-04-02 19:57:40.000000 coordinax-0.4.3/docs/conf.py
--rw-r--r--   0        0        0      196 2024-04-02 19:57:40.000000 coordinax-0.4.3/docs/index.md
--rw-r--r--   0        0        0     1261 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/__init__.py
--rw-r--r--   0        0        0    23716 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_base.py
--rw-r--r--   0        0        0     3937 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_base_dif.py
--rw-r--r--   0        0        0     6663 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_base_vec.py
--rw-r--r--   0        0        0     1379 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_checks.py
--rw-r--r--   0        0        0      460 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_converters.py
--rw-r--r--   0        0        0      209 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_exceptions.py
--rw-r--r--   0        0        0      871 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_typing.py
--rw-r--r--   0        0        0     2424 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_utils.py
--rw-r--r--   0        0        0      411 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_version.py
--rw-r--r--   0        0        0       82 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_version.pyi
--rw-r--r--   0        0        0        0 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/py.typed
--rw-r--r--   0        0        0      217 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/setup_package.py
--rw-r--r--   0        0        0      382 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d1/__init__.py
--rw-r--r--   0        0        0     1990 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d1/base.py
--rw-r--r--   0        0        0     5743 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d1/builtin.py
--rw-r--r--   0        0        0     1118 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d1/compat.py
--rw-r--r--   0        0        0      857 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d1/operate.py
--rw-r--r--   0        0        0     2409 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d1/transform.py
--rw-r--r--   0        0        0      398 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d2/__init__.py
--rw-r--r--   0        0        0     1264 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d2/base.py
--rw-r--r--   0        0        0     7205 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d2/builtin.py
--rw-r--r--   0        0        0     1118 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d2/compat.py
--rw-r--r--   0        0        0      857 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d2/operate.py
--rw-r--r--   0        0        0     2451 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d2/transform.py
--rw-r--r--   0        0        0      454 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d3/__init__.py
--rw-r--r--   0        0        0     1264 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d3/base.py
--rw-r--r--   0        0        0     8200 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d3/builtin.py
--rw-r--r--   0        0        0    28352 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d3/compat.py
--rw-r--r--   0        0        0     2720 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d3/operate.py
--rw-r--r--   0        0        0    16465 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d3/sphere.py
--rw-r--r--   0        0        0    21691 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d3/transform.py
--rw-r--r--   0        0        0      323 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d4/__init__.py
--rw-r--r--   0        0        0      797 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d4/base.py
--rw-r--r--   0        0        0      556 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d4/compat.py
--rw-r--r--   0        0        0     2141 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d4/operate.py
--rw-r--r--   0        0        0     9447 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_d4/spacetime.py
--rw-r--r--   0        0        0      161 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_transform/__init__.py
--rw-r--r--   0        0        0    14040 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_transform/d1.py
--rw-r--r--   0        0        0    11103 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_transform/d2.py
--rw-r--r--   0        0        0    14949 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_transform/d3.py
--rw-r--r--   0        0        0     5927 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/_transform/differentials.py
--rw-r--r--   0        0        0      496 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/operators/__init__.py
--rw-r--r--   0        0        0     3762 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/operators/_base.py
--rw-r--r--   0        0        0     2942 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/operators/_composite.py
--rw-r--r--   0        0        0      897 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/operators/_funcs.py
--rw-r--r--   0        0        0     5051 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/operators/_identity.py
--rw-r--r--   0        0        0     3426 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/operators/_sequential.py
--rw-r--r--   0        0        0      534 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/operators/_galilean/__init__.py
--rw-r--r--   0        0        0      632 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/operators/_galilean/base.py
--rw-r--r--   0        0        0     5265 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/operators/_galilean/boost.py
--rw-r--r--   0        0        0     7319 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/operators/_galilean/composite.py
--rw-r--r--   0        0        0     9090 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/operators/_galilean/rotation.py
--rw-r--r--   0        0        0    17396 2024-04-02 19:57:40.000000 coordinax-0.4.3/src/coordinax/operators/_galilean/translation.py
--rw-r--r--   0        0        0       13 2024-04-02 19:57:40.000000 coordinax-0.4.3/tests/__init__.py
--rw-r--r--   0        0        0     7885 2024-04-02 19:57:40.000000 coordinax-0.4.3/tests/test_base.py
--rw-r--r--   0        0        0    17504 2024-04-02 19:57:40.000000 coordinax-0.4.3/tests/test_d1.py
--rw-r--r--   0        0        0    18195 2024-04-02 19:57:40.000000 coordinax-0.4.3/tests/test_d2.py
--rw-r--r--   0        0        0    42467 2024-04-02 19:57:40.000000 coordinax-0.4.3/tests/test_d3.py
--rw-r--r--   0        0        0      408 2024-04-02 19:57:40.000000 coordinax-0.4.3/tests/test_exceptions.py
--rw-r--r--   0        0        0     1183 2024-04-02 19:57:40.000000 coordinax-0.4.3/tests/test_jax_ops.py
--rw-r--r--   0        0        0      199 2024-04-02 19:57:40.000000 coordinax-0.4.3/tests/test_package.py
--rw-r--r--   0        0        0       36 2024-04-02 19:57:40.000000 coordinax-0.4.3/tests/test_utils.py
--rw-r--r--   0        0        0     2218 2024-04-02 19:57:40.000000 coordinax-0.4.3/.gitignore
--rw-r--r--   0        0        0     1531 2024-04-02 19:57:40.000000 coordinax-0.4.3/LICENSE
--rw-r--r--   0        0        0     1526 2024-04-02 19:57:40.000000 coordinax-0.4.3/README.md
--rw-r--r--   0        0        0     6878 2024-04-02 19:57:40.000000 coordinax-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     5452 2024-04-02 19:57:40.000000 coordinax-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      373 2024-06-01 17:04:11.000000 coordinax-0.5/.copier-answers.yml
+-rw-r--r--   0        0        0      125 2024-06-01 17:04:11.000000 coordinax-0.5/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-06-01 17:04:11.000000 coordinax-0.5/.gitattributes
+-rw-r--r--   0        0        0     2666 2024-06-01 17:04:11.000000 coordinax-0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-06-01 17:04:11.000000 coordinax-0.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      439 2024-06-01 17:04:11.000000 coordinax-0.5/conftest.py
+-rw-r--r--   0        0        0     2903 2024-06-01 17:04:11.000000 coordinax-0.5/noxfile.py
+-rw-r--r--   0        0        0     2386 2024-06-01 17:04:11.000000 coordinax-0.5/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-06-01 17:04:11.000000 coordinax-0.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-06-01 17:04:11.000000 coordinax-0.5/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1682 2024-06-01 17:04:11.000000 coordinax-0.5/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1857 2024-06-01 17:04:11.000000 coordinax-0.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      872 2024-06-01 17:04:11.000000 coordinax-0.5/docs/conf.py
+-rw-r--r--   0        0        0      196 2024-06-01 17:04:11.000000 coordinax-0.5/docs/index.md
+-rw-r--r--   0        0        0     1321 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/__init__.py
+-rw-r--r--   0        0        0    23642 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_base.py
+-rw-r--r--   0        0        0     6672 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_base_pos.py
+-rw-r--r--   0        0        0     5483 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_base_vel.py
+-rw-r--r--   0        0        0     1393 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_checks.py
+-rw-r--r--   0        0        0      460 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_converters.py
+-rw-r--r--   0        0        0      209 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_exceptions.py
+-rw-r--r--   0        0        0      887 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_typing.py
+-rw-r--r--   0        0        0     2412 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_utils.py
+-rw-r--r--   0        0        0      406 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_version.py
+-rw-r--r--   0        0        0       82 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_version.pyi
+-rw-r--r--   0        0        0        0 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/py.typed
+-rw-r--r--   0        0        0      217 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/setup_package.py
+-rw-r--r--   0        0        0      382 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d1/__init__.py
+-rw-r--r--   0        0        0     1964 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d1/base.py
+-rw-r--r--   0        0        0     5826 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d1/builtin.py
+-rw-r--r--   0        0        0     1118 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d1/compat.py
+-rw-r--r--   0        0        0      857 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d1/operate.py
+-rw-r--r--   0        0        0     2426 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d1/transform.py
+-rw-r--r--   0        0        0      398 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d2/__init__.py
+-rw-r--r--   0        0        0     1236 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d2/base.py
+-rw-r--r--   0        0        0     7291 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d2/builtin.py
+-rw-r--r--   0        0        0     1118 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d2/compat.py
+-rw-r--r--   0        0        0      857 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d2/operate.py
+-rw-r--r--   0        0        0     2477 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d2/transform.py
+-rw-r--r--   0        0        0      454 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d3/__init__.py
+-rw-r--r--   0        0        0     1290 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d3/base.py
+-rw-r--r--   0        0        0     8267 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d3/builtin.py
+-rw-r--r--   0        0        0    28424 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d3/compat.py
+-rw-r--r--   0        0        0     2720 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d3/operate.py
+-rw-r--r--   0        0        0    16707 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d3/sphere.py
+-rw-r--r--   0        0        0    21815 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d3/transform.py
+-rw-r--r--   0        0        0      323 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d4/__init__.py
+-rw-r--r--   0        0        0      793 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d4/base.py
+-rw-r--r--   0        0        0      556 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d4/compat.py
+-rw-r--r--   0        0        0     2141 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d4/operate.py
+-rw-r--r--   0        0        0     9435 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_d4/spacetime.py
+-rw-r--r--   0        0        0      267 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_dn/__init__.py
+-rw-r--r--   0        0        0     4595 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_dn/base.py
+-rw-r--r--   0        0        0     7179 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_dn/builtin.py
+-rw-r--r--   0        0        0      784 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_dn/transform.py
+-rw-r--r--   0        0        0      161 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_transform/__init__.py
+-rw-r--r--   0        0        0    14040 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_transform/d1.py
+-rw-r--r--   0        0        0    11103 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_transform/d2.py
+-rw-r--r--   0        0        0    14949 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_transform/d3.py
+-rw-r--r--   0        0        0     6157 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/_transform/differentials.py
+-rw-r--r--   0        0        0      496 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/operators/__init__.py
+-rw-r--r--   0        0        0     3772 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/operators/_base.py
+-rw-r--r--   0        0        0     2952 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/operators/_composite.py
+-rw-r--r--   0        0        0      897 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/operators/_funcs.py
+-rw-r--r--   0        0        0     5061 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/operators/_identity.py
+-rw-r--r--   0        0        0     3426 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/operators/_sequential.py
+-rw-r--r--   0        0        0      534 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/operators/_galilean/__init__.py
+-rw-r--r--   0        0        0      632 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/operators/_galilean/base.py
+-rw-r--r--   0        0        0     5265 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/operators/_galilean/boost.py
+-rw-r--r--   0        0        0     7319 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/operators/_galilean/composite.py
+-rw-r--r--   0        0        0     9090 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/operators/_galilean/rotation.py
+-rw-r--r--   0        0        0    17418 2024-06-01 17:04:11.000000 coordinax-0.5/src/coordinax/operators/_galilean/translation.py
+-rw-r--r--   0        0        0       13 2024-06-01 17:04:11.000000 coordinax-0.5/tests/__init__.py
+-rw-r--r--   0        0        0     7847 2024-06-01 17:04:11.000000 coordinax-0.5/tests/test_base.py
+-rw-r--r--   0        0        0    17492 2024-06-01 17:04:11.000000 coordinax-0.5/tests/test_d1.py
+-rw-r--r--   0        0        0    18181 2024-06-01 17:04:11.000000 coordinax-0.5/tests/test_d2.py
+-rw-r--r--   0        0        0    42375 2024-06-01 17:04:11.000000 coordinax-0.5/tests/test_d3.py
+-rw-r--r--   0        0        0      408 2024-06-01 17:04:11.000000 coordinax-0.5/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1203 2024-06-01 17:04:11.000000 coordinax-0.5/tests/test_jax_ops.py
+-rw-r--r--   0        0        0      199 2024-06-01 17:04:11.000000 coordinax-0.5/tests/test_package.py
+-rw-r--r--   0        0        0       36 2024-06-01 17:04:11.000000 coordinax-0.5/tests/test_utils.py
+-rw-r--r--   0        0        0     2229 2024-06-01 17:04:11.000000 coordinax-0.5/.gitignore
+-rw-r--r--   0        0        0     1069 2024-06-01 17:04:11.000000 coordinax-0.5/LICENSE
+-rw-r--r--   0        0        0     1526 2024-06-01 17:04:11.000000 coordinax-0.5/README.md
+-rw-r--r--   0        0        0     7143 2024-06-01 17:04:11.000000 coordinax-0.5/pyproject.toml
+-rw-r--r--   0        0        0     5477 2024-06-01 17:04:11.000000 coordinax-0.5/PKG-INFO
```

### Comparing `coordinax-0.4.3/.pre-commit-config.yaml` & `coordinax-0.5/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,35 +2,36 @@
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 default_stages: [pre-commit, pre-push]
 
 repos:
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: v3.21.3
+    rev: v3.27.0
     hooks:
       - id: commitizen
       # - id: commitizen-branch
       #   stages: [push]
 
   - repo: meta
     hooks:
       - id: check-useless-excludes
 
   - repo: https://github.com/scientific-python/cookie
-    rev: 2024.03.10
+    rev: 2024.04.23
     hooks:
       - id: sp-repo-review
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.5.0"
+    rev: "v4.6.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
+      - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: name-tests-test
         args: ["--pytest-test-first"]
       - id: trailing-whitespace
@@ -39,61 +40,62 @@
     rev: "v1.10.0"
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.1
+    rev: "0.28.4"
     hooks:
       - id: check-dependabot
       - id: check-github-workflows
       - id: check-readthedocs
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.3.5"
+    rev: "v0.4.5"
     hooks:
       # Run the linter
       - id: ruff
         types_or: [python, pyi, jupyter]
         args: ["--fix", "--show-fixes"]
       # Run the formatter
       - id: ruff-format
         types_or: [python, pyi, jupyter]
 
   - repo: https://github.com/adamchainz/blacken-docs
     rev: "1.16.0"
     hooks:
       - id: blacken-docs
-        additional_dependencies: [black==23.*]
+        additional_dependencies: [black==24.*]
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.9.0"
+    rev: "v1.10.0"
     hooks:
       - id: mypy
         files: src
         additional_dependencies:
           - pytest
 
   - repo: https://github.com/codespell-project/codespell
-    rev: "v2.2.6"
+    rev: "v2.3.0"
     hooks:
       - id: codespell
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.16
+    rev: "v0.18"
     hooks:
       - id: validate-pyproject
+        # additional_dependencies: ["validate-pyproject-schema-store[all]"]
 
   - repo: local
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
         language: pygrep
         entry: PyBind|Numpy|Cmake|CCache|Github|PyTest
```

### Comparing `coordinax-0.4.3/noxfile.py` & `coordinax-0.5/noxfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 import shutil
 from pathlib import Path
 
 import nox
 
 DIR = Path(__file__).parent.resolve()
 
+nox.needs_version = ">=2024.3.2"
 nox.options.sessions = ["lint", "pylint", "tests"]
+nox.options.default_venv_backend = "uv|virtualenv"
 
 
 @nox.session
 def lint(session: nox.Session) -> None:
     """Run the linter."""
     session.install("pre-commit")
     session.run(
```

### Comparing `coordinax-0.4.3/.github/CONTRIBUTING.md` & `coordinax-0.5/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/.github/matchers/pylint.json` & `coordinax-0.5/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/.github/workflows/cd.yml` & `coordinax-0.5/.github/workflows/cd.yml`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
       - published
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 env:
+  # Many color libraries just need this to be set to any value, but at least
+  # one distinguishes color depth, where "3" -> "256-bit color".
   FORCE_COLOR: 3
 
 jobs:
   dist:
     name: Distribution build
     runs-on: ubuntu-latest
```

### Comparing `coordinax-0.4.3/.github/workflows/ci.yml` & `coordinax-0.5/.github/workflows/ci.yml`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,16 @@
       - main
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 env:
+  # Many color libraries just need this to be set to any value, but at least
+  # one distinguishes color depth, where "3" -> "256-bit color".
   FORCE_COLOR: 3
 
 jobs:
   pre-commit:
     name: Format
     runs-on: ubuntu-latest
     steps:
@@ -62,8 +64,10 @@
 
       - name: Test package
         run: >-
           python -m pytest src docs tests -ra --cov --cov-report=xml
           --cov-report=term --durations=20 --arraydiff -m"not slow"
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v4.1.1
+        uses: codecov/codecov-action@v4.4.1
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `coordinax-0.4.3/docs/conf.py` & `coordinax-0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/__init__.py` & `coordinax-0.5/src/coordinax/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,65 +5,69 @@
 coordinax: Vectors in JAX
 """
 
 from jaxtyping import install_import_hook
 
 from . import (
     _base,
-    _base_dif,
-    _base_vec,
+    _base_pos,
+    _base_vel,
     _d1,
     _d2,
     _d3,
     _d4,
+    _dn,
     _exceptions,
     _transform,
     _typing,
     _utils,
     operators,
 )
 from ._base import *
-from ._base_dif import *
-from ._base_vec import *
+from ._base_pos import *
+from ._base_vel import *
 from ._d1 import *
 from ._d2 import *
 from ._d3 import *
 from ._d4 import *
+from ._dn import *
 from ._exceptions import *
 from ._transform import *
 from ._typing import *
 from ._utils import *
 from ._version import version as __version__
 from .setup_package import RUNTIME_TYPECHECKER
 
 __all__ = ["__version__", "operators"]
 __all__ += _base.__all__
-__all__ += _base_vec.__all__
-__all__ += _base_dif.__all__
+__all__ += _base_pos.__all__
+__all__ += _base_vel.__all__
 __all__ += _d1.__all__
 __all__ += _d2.__all__
 __all__ += _d3.__all__
 __all__ += _d4.__all__
+__all__ += _dn.__all__
 __all__ += _exceptions.__all__
 __all__ += _transform.__all__
 __all__ += _typing.__all__
 __all__ += _utils.__all__
 
 
 # Runtime Typechecker
 install_import_hook("coordinax", RUNTIME_TYPECHECKER)
 
 # Cleanup
 del (
     _base,
-    _base_dif,
-    _base_vec,
+    _base_vel,
+    _base_pos,
     _exceptions,
     _transform,
     _typing,
     _utils,
     _d1,
     _d2,
     _d3,
     _d4,
+    _dn,
     RUNTIME_TYPECHECKER,
 )
```

### Comparing `coordinax-0.4.3/src/coordinax/_base.py` & `coordinax-0.5/src/coordinax/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Representation of coordinates in different systems."""
 
 __all__ = [
     # vector classes
-    "AbstractVectorBase",
+    "AbstractVector",
     # other
     "ToUnitsOptions",
 ]
 
 from abc import abstractmethod
 from collections.abc import Callable, Mapping
 from dataclasses import fields, replace
@@ -26,39 +26,39 @@
 
 from ._utils import classproperty, dataclass_items, dataclass_values, full_shaped
 from coordinax._typing import Unit
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
-BT = TypeVar("BT", bound="AbstractVectorBase")
+BT = TypeVar("BT", bound="AbstractVector")
 
 
 class ToUnitsOptions(Enum):
     """Options for the units argument of :meth:`AbstractVector.to_units`."""
 
     consistent = "consistent"
     """Convert to consistent units."""
 
 
 # ===================================================================
 
 
-class AbstractVectorBase(eqx.Module):  # type: ignore[misc]
+class AbstractVector(eqx.Module):  # type: ignore[misc]
     """Base class for all vector types.
 
     A vector is a collection of components that can be represented in different
     coordinate systems. This class provides a common interface for all vector
     types. All fields of the vector are expected to be components of the vector.
     """
 
     @classproperty
     @classmethod
     @abstractmethod
-    def _cartesian_cls(cls) -> type["AbstractVectorBase"]:
+    def _cartesian_cls(cls) -> type["AbstractVector"]:
         """Return the corresponding Cartesian vector class.
 
         Examples
         --------
         >>> from coordinax import RadialVector, SphericalVector
 
         >>> RadialVector._cartesian_cls
@@ -73,16 +73,16 @@
 
     # ---------------------------------------------------------------
     # Constructors
 
     @classmethod
     @dispatch
     def constructor(
-        cls: "type[AbstractVectorBase]", obj: Mapping[str, Quantity], /
-    ) -> "AbstractVectorBase":
+        cls: "type[AbstractVector]", obj: Mapping[str, Quantity], /
+    ) -> "AbstractVector":
         """Construct a vector from a mapping.
 
         Parameters
         ----------
         obj : Mapping[str, Any]
             The mapping of components.
 
@@ -113,18 +113,18 @@
 
         """
         return cls(**obj)
 
     @classmethod
     @dispatch
     def constructor(
-        cls: "type[AbstractVectorBase]",
+        cls: "type[AbstractVector]",
         obj: Quantity | u.Quantity,
         /,  # TODO: shape hint
-    ) -> "AbstractVectorBase":
+    ) -> "AbstractVector":
         """Construct a vector from a Quantity array.
 
         The array is expected to have the components as the last dimension.
 
         Parameters
         ----------
         obj : Quantity[Any, (*#batch, N), "..."]
@@ -178,15 +178,15 @@
         Parameters
         ----------
         index : Any
             The slice to apply.
 
         Returns
         -------
-        AbstractVectorBase
+        AbstractVector
             The vector with the slice applied.
 
         Examples
         --------
         We assume the following imports:
 
         >>> from unxt import Quantity
@@ -360,15 +360,15 @@
         Parameters
         ----------
         device : None, Device
             The device to move the vector to.
 
         Returns
         -------
-        AbstractVectorBase
+        AbstractVector
             The vector moved to the new device.
 
         Examples
         --------
         We assume the following imports:
 
         >>> from jax import devices
@@ -410,27 +410,27 @@
             x=Quantity[PhysicalType('length')](value=f32[4], unit=Unit("m")),
             y=Quantity[PhysicalType('length')](value=f32[1], unit=Unit("m"))
         )
 
         """
         return replace(self, **{k: v.flatten() for k, v in dataclass_items(self)})
 
-    def reshape(self, *args: Any, order: str = "C") -> "Self":
+    def reshape(self, *shape: Any, order: str = "C") -> "Self":
         """Reshape the components of the vector.
 
         Parameters
         ----------
-        *args : Any
+        *shape : Any
             The new shape.
         order : str
             The order to use for the reshape.
 
         Returns
         -------
-        AbstractVectorBase
+        AbstractVector
             The vector with the reshaped components.
 
         Examples
         --------
         We assume the following imports:
 
         >>> from unxt import Quantity
@@ -447,15 +447,16 @@
             y=Quantity[PhysicalType('length')](value=f32[4], unit=Unit("m"))
         )
 
         """
         # TODO: enable not needing to make a full-shaped copy
         full = full_shaped(self)
         return replace(
-            self, **{k: v.reshape(*args, order=order) for k, v in dataclass_items(full)}
+            self,
+            **{k: v.reshape(*shape, order=order) for k, v in dataclass_items(full)},
         )
 
     # ===============================================================
     # Collection
 
     def asdict(
         self,
@@ -550,15 +551,15 @@
 
     @abstractmethod
     def represent_as(self, target: type[BT], /, *args: Any, **kwargs: Any) -> BT:
         """Represent the vector as another type."""
         raise NotImplementedError
 
     @dispatch
-    def to_units(self, units: Any) -> "AbstractVectorBase":
+    def to_units(self, units: Any) -> "AbstractVector":
         """Convert the vector to the given units.
 
         Parameters
         ----------
         units : `unxt.AbstractUnitSystem`
             The units to convert to according to the physical type of the
             components.
@@ -588,15 +589,15 @@
                 for k, v in dataclass_items(self)
             },
         )
 
     @dispatch
     def to_units(
         self, units: Mapping[u.PhysicalType | str, Unit | str], /
-    ) -> "AbstractVectorBase":
+    ) -> "AbstractVector":
         """Convert the vector to the given units.
 
         Parameters
         ----------
         units : Mapping[PhysicalType | str, Unit | str]
             The units to convert to according to the physical type of the
             components.
@@ -634,17 +635,15 @@
             **{
                 k: v.to_units(units_[v.unit.physical_type])
                 for k, v in dataclass_items(self)
             },
         )
 
     @dispatch
-    def to_units(
-        self, _: Literal[ToUnitsOptions.consistent], /
-    ) -> "AbstractVectorBase":
+    def to_units(self, _: Literal[ToUnitsOptions.consistent], /) -> "AbstractVector":
         """Convert the vector to a self-consistent set of units.
 
         Parameters
         ----------
         units : Literal[ToUnitsOptions.consistent]
             The vector is converted to consistent units by looking for the first
             quantity with each physical type and converting all components to
@@ -721,23 +720,23 @@
 
 
 # -----------------------------------------------
 # Register additional constructors
 
 
 # TODO: move to the class in py3.11+
-@AbstractVectorBase.constructor._f.register  # type: ignore[attr-defined, misc]  # noqa: SLF001
+@AbstractVector.constructor._f.register  # type: ignore[attr-defined, misc]  # noqa: SLF001
 def constructor(  # noqa: D417
-    cls: type[AbstractVectorBase], obj: AbstractVectorBase, /
-) -> AbstractVectorBase:
+    cls: type[AbstractVector], obj: AbstractVector, /
+) -> AbstractVector:
     """Construct a vector from another vector.
 
     Parameters
     ----------
-    obj : :class:`coordinax.AbstractVectorBase`
+    obj : :class:`coordinax.AbstractVector`
         The vector to construct from.
 
     Examples
     --------
     >>> import jax.numpy as jnp
     >>> from unxt import Quantity
     >>> from coordinax import Cartesian3DVector
```

### Comparing `coordinax-0.4.3/src/coordinax/_base_vec.py` & `coordinax-0.5/src/coordinax/_base_pos.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Representation of coordinates in different systems."""
 
-__all__ = ["AbstractVector"]
+__all__ = ["AbstractPosition"]
 
 import operator
 import warnings
 from abc import abstractmethod
 from dataclasses import replace
 from functools import partial
 from inspect import isabstract
@@ -12,43 +12,43 @@
 
 import jax
 from jaxtyping import ArrayLike
 from plum import dispatch
 
 from unxt import Quantity
 
-from ._base import AbstractVectorBase
+from ._base import AbstractVector
 from ._utils import classproperty, dataclass_items
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
-VT = TypeVar("VT", bound="AbstractVector")
+VT = TypeVar("VT", bound="AbstractPosition")
 
-VECTOR_CLASSES: list[type["AbstractVector"]] = []
+VECTOR_CLASSES: set[type["AbstractPosition"]] = set()
 
 
-class AbstractVector(AbstractVectorBase):  # pylint: disable=abstract-method
+class AbstractPosition(AbstractVector):  # pylint: disable=abstract-method
     """Abstract representation of coordinates in different systems."""
 
     def __init_subclass__(cls, **kwargs: Any) -> None:
         """Initialize the subclass.
 
         The subclass is registered if it is not an abstract class.
         """
         # TODO: a more robust check using equinox.
         if isabstract(cls) or cls.__name__.startswith("Abstract"):
             return
 
-        VECTOR_CLASSES.append(cls)
+        VECTOR_CLASSES.add(cls)
 
     @classproperty
     @classmethod
     @abstractmethod
-    def differential_cls(cls) -> type["AbstractVectorDifferential"]:
+    def differential_cls(cls) -> type["AbstractVelocity"]:
         """Return the corresponding differential vector class.
 
         Examples
         --------
         >>> from coordinax import RadialVector, SphericalVector
 
         >>> RadialVector.differential_cls.__name__
@@ -75,86 +75,86 @@
         return (-cart).represent_as(type(self))
 
     # -----------------------------------------------------
     # Binary arithmetic operations
 
     def __add__(self, other: Any) -> "Self":
         """Add another object to this vector."""
-        if not isinstance(other, AbstractVector):
+        if not isinstance(other, AbstractPosition):
             return NotImplemented
 
         # The base implementation is to convert to Cartesian and perform the
         # operation.  Cartesian coordinates do not have any branch cuts or
         # singularities or ranges that need to be handled, so this is a safe
         # default.
         return operator.add(
             self.represent_as(self._cartesian_cls),
             other.represent_as(self._cartesian_cls),
         ).represent_as(type(self))
 
     def __sub__(self, other: Any) -> "Self":
         """Add another object to this vector."""
-        if not isinstance(other, AbstractVector):
+        if not isinstance(other, AbstractPosition):
             return NotImplemented
 
         # The base implementation is to convert to Cartesian and perform the
         # operation.  Cartesian coordinates do not have any branch cuts or
         # singularities or ranges that need to be handled, so this is a safe
         # default.
         return operator.sub(
             self.represent_as(self._cartesian_cls),
             other.represent_as(self._cartesian_cls),
         ).represent_as(type(self))
 
     @dispatch
-    def __mul__(self: "AbstractVector", other: Any) -> Any:
+    def __mul__(self: "AbstractPosition", other: Any) -> Any:
         return NotImplemented
 
     @dispatch
-    def __mul__(self: "AbstractVector", other: ArrayLike) -> Any:
+    def __mul__(self: "AbstractPosition", other: ArrayLike) -> Any:
         return replace(self, **{k: v * other for k, v in dataclass_items(self)})
 
     @dispatch
-    def __truediv__(self: "AbstractVector", other: Any) -> Any:
+    def __truediv__(self: "AbstractPosition", other: Any) -> Any:
         return NotImplemented
 
     @dispatch
-    def __truediv__(self: "AbstractVector", other: ArrayLike) -> Any:
+    def __truediv__(self: "AbstractPosition", other: ArrayLike) -> Any:
         return replace(self, **{k: v / other for k, v in dataclass_items(self)})
 
     # ---------------------------------
     # Reverse binary operations
 
     @dispatch
-    def __rmul__(self: "AbstractVector", other: Any) -> Any:
+    def __rmul__(self: "AbstractPosition", other: Any) -> Any:
         return NotImplemented
 
     @dispatch
-    def __rmul__(self: "AbstractVector", other: ArrayLike) -> Any:
+    def __rmul__(self: "AbstractPosition", other: ArrayLike) -> Any:
         return replace(self, **{k: other * v for k, v in dataclass_items(self)})
 
     # ===============================================================
     # Convenience methods
 
     @partial(jax.jit, static_argnums=1)
     def represent_as(self, target: type[VT], /, *args: Any, **kwargs: Any) -> VT:
         """Represent the vector as another type.
 
         Parameters
         ----------
-        target : type[AbstractVector]
+        target : type[AbstractPosition]
             The type to represent the vector as.
         *args : Any
             Extra arguments. Raises a warning if any are given.
         **kwargs : Any
             Extra keyword arguments.
 
         Returns
         -------
-        AbstractVector
+        AbstractPosition
             The vector represented as the target type.
 
         Warns
         -----
         UserWarning
             If extra arguments are given.
```

### Comparing `coordinax-0.4.3/src/coordinax/_checks.py` & `coordinax-0.5/src/coordinax/_checks.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,41 +13,41 @@
 _0m = Quantity(0, "meter")
 _0d = Quantity(0, "rad")
 _pid = Quantity(180, "deg")
 _2pid = Quantity(360, "deg")
 
 
 def check_r_non_negative(
-    r: BatchableLength, _lower: Quantity["length"] = _0m
+    r: BatchableLength, /, _lower: Quantity["length"] = _0m
 ) -> BatchableLength:
     """Check that the radial distance is non-negative."""
     return eqx.error_if(
-        r,
-        xp.any(r < _lower),
-        "The radial distance must be non-negative.",
+        r, xp.any(r < _lower), "The radial distance must be non-negative."
     )
 
 
 def check_azimuth_range(
     phi: BatchableAngle,
+    /,
     _lower: Quantity["angle"] = _0d,
     _upper: Quantity["angle"] = _2pid,
 ) -> BatchableAngle:
     """Check that the polar angle is in the range [0, 2pi)."""
     return eqx.error_if(
         phi,
         xp.any((phi < _lower) | (phi >= _upper)),
         "The azimuthal (polar) angle must be in the range [0, 2pi).",
     )
 
 
 def check_polar_range(
     theta: BatchableAngle,
+    /,
     _lower: Quantity["angle"] = _0d,
     _upper: Quantity["angle"] = _pid,
 ) -> BatchableAngle:
     """Check that the inclination angle is in the range [0, pi]."""
     return eqx.error_if(
         theta,
-        xp.any((theta < _lower) | (theta > _upper)),
+        xp.any(xp.logical_or((theta < _lower), (theta > _upper))),
         "The inclination angle must be in the range [0, pi].",
     )
```

### Comparing `coordinax-0.4.3/src/coordinax/_typing.py` & `coordinax-0.5/src/coordinax/_typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 __all__: list[str] = []
 
 from typing import TypeAlias
 
 import astropy.units as u
 from jaxtyping import Float, Int, Shaped
 
-from unxt import Distance, Quantity
+from unxt import AbstractDistance, Quantity
 
 Unit: TypeAlias = u.Unit | u.UnitBase | u.CompositeUnit
 
 FloatScalarQ = Float[Quantity, ""]
 BatchFloatScalarQ = Shaped[FloatScalarQ, "*batch"]
 BatchableFloatScalarQ = Shaped[FloatScalarQ, "*#batch"]
 
 ScalarTime = Float[Quantity["time"], ""] | Int[Quantity["time"], ""]
 
 BatchableAngle = Shaped[Quantity["angle"], "*#batch"]
 BatchableLength = Shaped[Quantity["length"], "*#batch"]
-BatchableDistance = Shaped[Distance, "*#batch"]
+BatchableDistance = Shaped[AbstractDistance, "*#batch"]
 BatchableSpeed = Shaped[Quantity["speed"], "*#batch"]
 BatchableTime = Shaped[Quantity["time"], "*#batch"]
 BatchableAngularSpeed = Shaped[Quantity["angular speed"], "*#batch"]
 
 
 TimeBatchOrScalar = ScalarTime | BatchableTime
```

### Comparing `coordinax-0.4.3/src/coordinax/_utils.py` & `coordinax-0.5/src/coordinax/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     TypeVar,
     runtime_checkable,
 )
 
 import quaxed.array_api as xp
 
 if TYPE_CHECKING:
-    from coordinax._base import AbstractVectorBase
+    from coordinax._base import AbstractVector
 
 
 ################################################################################
 
 
 @runtime_checkable
 class DataclassInstance(Protocol):
@@ -36,15 +36,15 @@
 
 
 def dataclass_items(obj: "DataclassInstance") -> Iterator[tuple[str, Any]]:
     """Return the field names and values of a dataclass instance."""
     yield from ((f.name, getattr(obj, f.name)) for f in fields(obj))
 
 
-def full_shaped(obj: "AbstractVectorBase", /) -> "AbstractVectorBase":
+def full_shaped(obj: "AbstractVector", /) -> "AbstractVector":
     """Return the vector, fully broadcasting all components."""
     arrays = xp.broadcast_arrays(*dataclass_values(obj))
     return replace(obj, **dict(zip(obj.components, arrays, strict=True)))
 
 
 ################################################################################
```

### Comparing `coordinax-0.4.3/src/coordinax/_d1/base.py` & `coordinax-0.5/src/coordinax/_d1/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 from abc import abstractmethod
 from dataclasses import fields
 
 from jaxtyping import Shaped
 
 from unxt import Quantity
 
-from coordinax._base import AbstractVectorBase
-from coordinax._base_dif import AbstractVectorDifferential
-from coordinax._base_vec import AbstractVector
+from coordinax._base import AbstractVector
+from coordinax._base_pos import AbstractPosition
+from coordinax._base_vel import AbstractVelocity
 from coordinax._utils import classproperty
 
 
-class Abstract1DVector(AbstractVector):
+class Abstract1DVector(AbstractPosition):
     """Abstract representation of 1D coordinates in different systems."""
 
     @classproperty
     @classmethod
-    def _cartesian_cls(cls) -> type[AbstractVectorBase]:
+    def _cartesian_cls(cls) -> type[AbstractVector]:
         from .builtin import Cartesian1DVector
 
         return Cartesian1DVector
 
     @classproperty
     @classmethod
     @abstractmethod
     def differential_cls(cls) -> type["Abstract1DVectorDifferential"]:
         raise NotImplementedError
 
 
 # TODO: move to the class in py3.11+
-@AbstractVector.constructor._f.dispatch  # type: ignore[attr-defined, misc]  # noqa: SLF001
+@AbstractPosition.constructor._f.dispatch  # type: ignore[attr-defined, misc]  # noqa: SLF001
 def constructor(
     cls: "type[Abstract1DVector]", x: Shaped[Quantity["length"], ""], /
 ) -> "Abstract1DVector":
     """Construct a 1D vector.
 
     Examples
     --------
@@ -51,20 +51,20 @@
         x=Quantity[PhysicalType('length')](value=f32[1], unit=Unit("kpc"))
     )
 
     """
     return cls(**{fields(cls)[0].name: x.reshape(1)})
 
 
-class Abstract1DVectorDifferential(AbstractVectorDifferential):
+class Abstract1DVectorDifferential(AbstractVelocity):
     """Abstract representation of 1D differentials in different systems."""
 
     @classproperty
     @classmethod
-    def _cartesian_cls(cls) -> type[AbstractVectorBase]:
+    def _cartesian_cls(cls) -> type[AbstractVector]:
         from .builtin import CartesianDifferential1D
 
         return CartesianDifferential1D
 
     @classproperty
     @classmethod
     @abstractmethod
```

### Comparing `coordinax-0.4.3/src/coordinax/_d1/builtin.py` & `coordinax-0.5/src/coordinax/_d1/builtin.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from functools import partial
 from typing import Any, final
 
 import equinox as eqx
 import jax
 
 import quaxed.array_api as xp
-from unxt import Distance, Quantity
+from unxt import AbstractDistance, Distance, Quantity
 
 import coordinax._typing as ct
 from .base import Abstract1DVector, Abstract1DVectorDifferential
-from coordinax._base_vec import AbstractVector
+from coordinax._base_pos import AbstractPosition
 from coordinax._checks import check_r_non_negative
 from coordinax._utils import classproperty
 
 ##############################################################################
 # Position
 
 
@@ -80,15 +80,15 @@
         Cartesian1DVector(
            x=Quantity[PhysicalType('length')](value=f32[], unit=Unit("kpc"))
         )
         >>> qpr.x
         Quantity['length'](Array(2., dtype=float32), unit='kpc')
 
         """
-        if not isinstance(other, AbstractVector):
+        if not isinstance(other, AbstractPosition):
             msg = f"Cannot add {Cartesian1DVector!r} and {type(other)!r}."
             raise TypeError(msg)
 
         cart = other.represent_as(Cartesian1DVector)
         return replace(self, x=self.x + cart.x)
 
     def __sub__(self, other: Any, /) -> "Cartesian1DVector":
@@ -106,15 +106,15 @@
         Cartesian1DVector(
            x=Quantity[PhysicalType('length')](value=f32[], unit=Unit("kpc"))
         )
         >>> qmr.x
         Quantity['length'](Array(0., dtype=float32), unit='kpc')
 
         """
-        if not isinstance(other, AbstractVector):
+        if not isinstance(other, AbstractPosition):
             msg = f"Cannot subtract {Cartesian1DVector!r} and {type(other)!r}."
             raise TypeError(msg)
 
         cart = other.represent_as(Cartesian1DVector)
         return replace(self, x=self.x - cart.x)
 
     @partial(jax.jit)
@@ -135,15 +135,17 @@
 
 
 @final
 class RadialVector(Abstract1DVector):
     """Radial vector representation."""
 
     r: ct.BatchableDistance = eqx.field(
-        converter=partial(Distance.constructor, dtype=float)
+        converter=lambda x: x
+        if isinstance(x, AbstractDistance)
+        else Distance.constructor(x, dtype=float)
     )
     r"""Radial distance :math:`r \in [0,+\infty)`."""
 
     def __check_init__(self) -> None:
         """Check the initialization."""
         check_r_non_negative(self.r)
 
@@ -175,15 +177,15 @@
 
         Examples
         --------
         >>> from unxt import Quantity
         >>> from coordinax import CartesianDifferential1D
         >>> q = CartesianDifferential1D.constructor(Quantity([-1], "km/s"))
         >>> q.norm()
-        Quantity['speed'](Array(1., dtype=float32), unit='km / s')
+        Quantity['speed'](Array(1, dtype=int32), unit='km / s')
 
         """
         return xp.abs(self.d_x)
 
 
 @final
 class RadialDifferential(Abstract1DVectorDifferential):
```

### Comparing `coordinax-0.4.3/src/coordinax/_d1/compat.py` & `coordinax-0.5/src/coordinax/_d1/compat.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/_d1/operate.py` & `coordinax-0.5/src/coordinax/_d1/operate.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/_d1/transform.py` & `coordinax-0.5/src/coordinax/_d1/transform.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .base import Abstract1DVector, Abstract1DVectorDifferential
 from .builtin import (
     Cartesian1DVector,
     CartesianDifferential1D,
     RadialDifferential,
     RadialVector,
 )
-from coordinax._base_vec import AbstractVector
+from coordinax._base_pos import AbstractPosition
 
 ###############################################################################
 # 1D
 
 
 @dispatch(precedence=1)
 def represent_as(
@@ -44,21 +44,21 @@
     This is the base case for the transformation of 1D vectors.
     """
     cart1d = represent_as(current, Cartesian1DVector)
     return represent_as(cart1d, target)
 
 
 @dispatch.multi(
-    (CartesianDifferential1D, type[CartesianDifferential1D], AbstractVector),
-    (RadialDifferential, type[RadialDifferential], AbstractVector),
+    (CartesianDifferential1D, type[CartesianDifferential1D], AbstractPosition),
+    (RadialDifferential, type[RadialDifferential], AbstractPosition),
 )
 def represent_as(
     current: Abstract1DVectorDifferential,
     target: type[Abstract1DVectorDifferential],
-    position: AbstractVector,
+    position: AbstractPosition,
     /,
     **kwargs: Any,
 ) -> Abstract1DVectorDifferential:
     """Self transform of 1D Differentials."""
     return current
 
 
@@ -85,8 +85,8 @@
 def represent_as(
     current: RadialVector, target: type[Cartesian1DVector], /, **kwargs: Any
 ) -> Cartesian1DVector:
     """RadialVector -> Cartesian1DVector.
 
     The `r` coordinate is converted to the `x` coordinate of the 1D system.
     """
-    return target(x=current.r)
+    return target(x=current.r.distance)
```

### Comparing `coordinax-0.4.3/src/coordinax/_d2/base.py` & `coordinax-0.5/src/coordinax/_d2/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """Representation of coordinates in different systems."""
 
 __all__ = ["Abstract2DVector", "Abstract2DVectorDifferential"]
 
 
 from abc import abstractmethod
 
-from coordinax._base import AbstractVectorBase
-from coordinax._base_dif import AbstractVectorDifferential
-from coordinax._base_vec import AbstractVector
+from coordinax._base import AbstractVector
+from coordinax._base_pos import AbstractPosition
+from coordinax._base_vel import AbstractVelocity
 from coordinax._utils import classproperty
 
 
-class Abstract2DVector(AbstractVector):
+class Abstract2DVector(AbstractPosition):
     """Abstract representation of 2D coordinates in different systems."""
 
     @classproperty
     @classmethod
-    def _cartesian_cls(cls) -> type[AbstractVectorBase]:
+    def _cartesian_cls(cls) -> type[AbstractVector]:
         from .builtin import Cartesian2DVector
 
         return Cartesian2DVector
 
     @classproperty
     @classmethod
     @abstractmethod
     def differential_cls(cls) -> type["Abstract2DVectorDifferential"]:
         raise NotImplementedError
 
 
-class Abstract2DVectorDifferential(AbstractVectorDifferential):
+class Abstract2DVectorDifferential(AbstractVelocity):
     """Abstract representation of 2D vector differentials."""
 
     @classproperty
     @classmethod
-    def _cartesian_cls(cls) -> type[AbstractVectorBase]:
+    def _cartesian_cls(cls) -> type[AbstractVector]:
         from .builtin import CartesianDifferential2D
 
         return CartesianDifferential2D
 
     @classproperty
     @classmethod
     @abstractmethod
```

### Comparing `coordinax-0.4.3/src/coordinax/_d2/builtin.py` & `coordinax-0.5/src/coordinax/_d2/builtin.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from functools import partial
 from typing import Any, final
 
 import equinox as eqx
 import jax
 
 import quaxed.array_api as xp
-from unxt import Distance, Quantity
+from unxt import AbstractDistance, Distance, Quantity
 
 import coordinax._typing as ct
 from .base import Abstract2DVector, Abstract2DVectorDifferential
-from coordinax._base_vec import AbstractVector
+from coordinax._base_pos import AbstractPosition
 from coordinax._checks import check_azimuth_range, check_r_non_negative
 from coordinax._converters import converter_azimuth_to_range
 from coordinax._utils import classproperty
 
 # =============================================================================
 # 2D
 
@@ -80,15 +80,15 @@
         >>> cart = Cartesian2DVector.constructor(Quantity([1, 2], "kpc"))
         >>> polr = PolarVector(r=Quantity(3, "kpc"), phi=Quantity(90, "deg"))
 
         >>> (cart + polr).x
         Quantity['length'](Array(0.9999999, dtype=float32), unit='kpc')
 
         """
-        if not isinstance(other, AbstractVector):
+        if not isinstance(other, AbstractPosition):
             msg = f"Cannot add {Cartesian2DVector!r} and {type(other)!r}."
             raise TypeError(msg)
 
         cart = other.represent_as(Cartesian2DVector)
         return replace(self, x=self.x + cart.x, y=self.y + cart.y)
 
     def __sub__(self, other: Any, /) -> "Cartesian2DVector":
@@ -101,15 +101,15 @@
         >>> cart = Cartesian2DVector.constructor(Quantity([1, 2], "kpc"))
         >>> polr = PolarVector(r=Quantity(3, "kpc"), phi=Quantity(90, "deg"))
 
         >>> (cart - polr).x
         Quantity['length'](Array(1.0000001, dtype=float32), unit='kpc')
 
         """
-        if not isinstance(other, AbstractVector):
+        if not isinstance(other, AbstractPosition):
             msg = f"Cannot subtract {Cartesian2DVector!r} and {type(other)!r}."
             raise TypeError(msg)
 
         cart = other.represent_as(Cartesian2DVector)
         return replace(self, x=self.x - cart.x, y=self.y - cart.y)
 
     @partial(jax.jit)
@@ -139,15 +139,17 @@
     phi : BatchableAngle
         Polar angle :math:`\phi \in [0,2\pi)`.  We use the symbol `phi` to
         adhere to the ISO standard 31-11.
 
     """
 
     r: ct.BatchableDistance = eqx.field(
-        converter=partial(Distance.constructor, dtype=float)
+        converter=lambda x: x
+        if isinstance(x, AbstractDistance)
+        else Distance.constructor(x, dtype=float)
     )
     r"""Radial distance :math:`r \in [0,+\infty)`."""
 
     phi: ct.BatchableAngle = eqx.field(
         converter=lambda x: converter_azimuth_to_range(
             Quantity["angle"].constructor(x, dtype=float)  # pylint: disable=E1120
         )
```

### Comparing `coordinax-0.4.3/src/coordinax/_d2/compat.py` & `coordinax-0.5/src/coordinax/_d2/compat.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/_d2/operate.py` & `coordinax-0.5/src/coordinax/_d2/operate.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/_d2/transform.py` & `coordinax-0.5/src/coordinax/_d2/transform.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .base import Abstract2DVector, Abstract2DVectorDifferential
 from .builtin import (
     Cartesian2DVector,
     CartesianDifferential2D,
     PolarDifferential,
     PolarVector,
 )
-from coordinax._base_vec import AbstractVector
+from coordinax._base_pos import AbstractPosition
 
 
 @dispatch
 def represent_as(
     current: Abstract2DVector, target: type[Abstract2DVector], /, **kwargs: Any
 ) -> Abstract2DVector:
     """Abstract2DVector -> Cartesian2D -> Abstract2DVector.
@@ -37,21 +37,21 @@
     current: Abstract2DVector, target: type[Abstract2DVector], /, **kwargs: Any
 ) -> Abstract2DVector:
     """Self transform of 2D vectors."""
     return current
 
 
 @dispatch.multi(
-    (CartesianDifferential2D, type[CartesianDifferential2D], AbstractVector),
-    (PolarDifferential, type[PolarDifferential], AbstractVector),
+    (CartesianDifferential2D, type[CartesianDifferential2D], AbstractPosition),
+    (PolarDifferential, type[PolarDifferential], AbstractPosition),
 )
 def represent_as(
     current: Abstract2DVectorDifferential,
     target: type[Abstract2DVectorDifferential],
-    position: AbstractVector,
+    position: AbstractPosition,
     /,
     **kwargs: Any,
 ) -> Abstract2DVectorDifferential:
     """Self transform of 2D Differentials."""
     return current
 
 
@@ -84,10 +84,10 @@
 
 
 @dispatch
 def represent_as(
     current: PolarVector, target: type[Cartesian2DVector], /, **kwargs: Any
 ) -> Cartesian2DVector:
     """PolarVector -> Cartesian2DVector."""
-    x = current.r * xp.cos(current.phi)
-    y = current.r * xp.sin(current.phi)
+    x = current.r.distance * xp.cos(current.phi)
+    y = current.r.distance * xp.sin(current.phi)
     return target(x=x, y=y)
```

### Comparing `coordinax-0.4.3/src/coordinax/_d3/base.py` & `coordinax-0.5/src/coordinax/_d4/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,30 @@
 """Representation of coordinates in different systems."""
 
-__all__ = ["Abstract3DVector", "Abstract3DVectorDifferential"]
+__all__ = ["Abstract4DVector"]
 
 
 from abc import abstractmethod
+from typing import TYPE_CHECKING
 
-from coordinax._base import AbstractVectorBase
-from coordinax._base_dif import AbstractVectorDifferential
-from coordinax._base_vec import AbstractVector
+from coordinax._base import AbstractVector
+from coordinax._base_pos import AbstractPosition
 from coordinax._utils import classproperty
 
+if TYPE_CHECKING:
+    from typing_extensions import Never
 
-class Abstract3DVector(AbstractVector):
-    """Abstract representation of 3D coordinates in different systems."""
 
-    @classproperty
-    @classmethod
-    def _cartesian_cls(cls) -> type[AbstractVectorBase]:
-        from .builtin import Cartesian3DVector
-
-        return Cartesian3DVector
+class Abstract4DVector(AbstractPosition):
+    """Abstract representation of 4D coordinates in different systems."""
 
     @classproperty
     @classmethod
-    @abstractmethod
-    def differential_cls(cls) -> type["Abstract3DVectorDifferential"]:
+    def _cartesian_cls(cls) -> type[AbstractVector]:
         raise NotImplementedError
 
-
-class Abstract3DVectorDifferential(AbstractVectorDifferential):
-    """Abstract representation of 3D vector differentials."""
-
-    @classproperty
-    @classmethod
-    def _cartesian_cls(cls) -> type[AbstractVectorBase]:
-        from .builtin import CartesianDifferential3D
-
-        return CartesianDifferential3D
-
     @classproperty
     @classmethod
     @abstractmethod
-    def integral_cls(cls) -> type[Abstract3DVector]:
-        raise NotImplementedError
+    def differential_cls(cls) -> "Never":  # type: ignore[override]
+        msg = "Not yet implemented"
+        raise NotImplementedError(msg)
```

### Comparing `coordinax-0.4.3/src/coordinax/_d3/builtin.py` & `coordinax-0.5/src/coordinax/_d3/builtin.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 import jax
 
 import quaxed.array_api as xp
 from unxt import Quantity
 
 import coordinax._typing as ct
 from .base import Abstract3DVector, Abstract3DVectorDifferential
-from coordinax._base_vec import AbstractVector
+from coordinax._base_pos import AbstractPosition
+from coordinax._base_vel import AdditionMixin
 from coordinax._checks import check_azimuth_range, check_r_non_negative
 from coordinax._converters import converter_azimuth_to_range
 from coordinax._utils import classproperty
 
 ##############################################################################
 # Position
 
@@ -84,15 +85,15 @@
         >>> q = Cartesian3DVector.constructor(Quantity([1, 2, 3], "kpc"))
         >>> s = SphericalVector(r=Quantity(1, "kpc"), theta=Quantity(90, "deg"),
         ...                     phi=Quantity(0, "deg"))
         >>> (q + s).x
         Quantity['length'](Array(2., dtype=float32), unit='kpc')
 
         """
-        if not isinstance(other, AbstractVector):
+        if not isinstance(other, AbstractPosition):
             msg = f"Cannot add {self._cartesian_cls!r} and {type(other)!r}."
             raise TypeError(msg)
 
         cart = other.represent_as(Cartesian3DVector)
         return replace(self, x=self.x + cart.x, y=self.y + cart.y, z=self.z + cart.z)
 
     def __sub__(self, other: Any, /) -> "Cartesian3DVector":
@@ -105,15 +106,15 @@
         >>> q = Cartesian3DVector.constructor(Quantity([1, 2, 3], "kpc"))
         >>> s = SphericalVector(r=Quantity(1, "kpc"), theta=Quantity(90, "deg"),
         ...                     phi=Quantity(0, "deg"))
         >>> (q - s).x
         Quantity['length'](Array(0., dtype=float32), unit='kpc')
 
         """
-        if not isinstance(other, AbstractVector):
+        if not isinstance(other, AbstractPosition):
             msg = f"Cannot subtract {self._cartesian_cls!r} and {type(other)!r}."
             raise TypeError(msg)
 
         cart = other.represent_as(Cartesian3DVector)
         return replace(self, x=self.x - cart.x, y=self.y - cart.y, z=self.z - cart.z)
 
     @partial(jax.jit)
@@ -185,15 +186,15 @@
 
 
 ##############################################################################
 # Differential
 
 
 @final
-class CartesianDifferential3D(Abstract3DVectorDifferential):
+class CartesianDifferential3D(Abstract3DVectorDifferential, AdditionMixin):
     """Cartesian differential representation."""
 
     d_x: ct.BatchableSpeed = eqx.field(
         converter=partial(Quantity["speed"].constructor, dtype=float)
     )
     r"""X speed :math:`dx/dt \in [-\infty, \infty]."""
```

### Comparing `coordinax-0.4.3/src/coordinax/_d3/compat.py` & `coordinax-0.5/src/coordinax/_d3/compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,17 @@
     Distance(Array(1., dtype=float32), unit='kpc')
 
     """
     obj = obj.represent_as(apyc.SphericalRepresentation)
     return cls(distance=obj.distance, lon=obj.lon, lat=obj.lat)
 
 
+# -------------------------------------------------------------------
+
+
 @CartesianDifferential3D.constructor._f.register  # noqa: SLF001
 def constructor(
     cls: type[CartesianDifferential3D], obj: apyc.CartesianDifferential
 ) -> CartesianDifferential3D:
     """Construct from a :class:`astropy.coordinates.CartesianDifferential`.
 
     Examples
```

### Comparing `coordinax-0.4.3/src/coordinax/_d3/operate.py` & `coordinax-0.5/src/coordinax/_d3/operate.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/_d3/sphere.py` & `coordinax-0.5/src/coordinax/_d3/sphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from typing import final
 
 import equinox as eqx
 import jax
 
 import quaxed.array_api as xp
 import quaxed.lax as qlax
-from unxt import Distance, Quantity
+from unxt import AbstractDistance, Distance, Quantity
 
 import coordinax._typing as ct
 from .base import Abstract3DVector, Abstract3DVectorDifferential
 from coordinax._checks import (
     check_azimuth_range,
     check_polar_range,
     check_r_non_negative,
@@ -68,15 +68,17 @@
         Polar angle [0, 180] [deg] where 0 is the z-axis.
     phi : Quantity['angle']
         Azimuthal angle [0, 360) [deg] where 0 is the x-axis.
 
     """
 
     r: ct.BatchableDistance = eqx.field(
-        converter=partial(Distance.constructor, dtype=float)
+        converter=lambda x: x
+        if isinstance(x, AbstractDistance)
+        else Distance.constructor(x, dtype=float)
     )
     r"""Radial distance :math:`r \in [0,+\infty)`."""
 
     theta: ct.BatchableAngle = eqx.field(
         converter=partial(Quantity["angle"].constructor, dtype=float)
     )
     r"""Inclination angle :math:`\theta \in [0,180]`."""
@@ -132,15 +134,17 @@
         Azimuthal angle [0, 360) [deg] where 0 is the x-axis.
     phi : Quantity['angle']
         Polar angle [0, 180] [deg] where 0 is the z-axis.
 
     """
 
     r: ct.BatchableDistance = eqx.field(
-        converter=partial(Distance.constructor, dtype=float)
+        converter=lambda x: x
+        if isinstance(x, AbstractDistance)
+        else Distance.constructor(x, dtype=float)
     )
     r"""Radial distance :math:`r \in [0,+\infty)`."""
 
     theta: ct.BatchableAngle = eqx.field(
         converter=lambda x: converter_azimuth_to_range(
             Quantity["angle"].constructor(x, dtype=float)  # pylint: disable=E1120
         )
@@ -221,23 +225,27 @@
     ...                                lat=Quantity(90, "deg"),
     ...                                distance=Quantity(3, "kpc"))
     >>> vec.lon
     Quantity['angle'](Array(5., dtype=float32), unit='deg')
 
     The latitude is not wrapped, but it is checked to be in the [-90, 90] degrees range.
 
+    .. skip: next
+
     >>> try:
     ...     cx.LonLatSphericalVector(lon=Quantity(0, "deg"), lat=Quantity(100, "deg"),
     ...                              distance=Quantity(3, "kpc"))
     ... except Exception as e:
     ...     print(e)
     The inclination angle must be in the range [0, pi]...
 
     Likewise, the radial distance is checked to be non-negative.
 
+    .. skip: next
+
     >>> try:
     ...     cx.LonLatSphericalVector(lon=Quantity(0, "deg"), lat=Quantity(0, "deg"),
     ...                              distance=Quantity(-3, "kpc"))
     ... except Exception as e:
     ...     print(e)
     The radial distance must be non-negative...
 
@@ -252,15 +260,17 @@
 
     lat: ct.BatchableAngle = eqx.field(
         converter=lambda x: Quantity["angle"].constructor(x, dtype=float)  # pylint: disable=E1120
     )
     r"""Latitude (polar) angle :math:`\in [-90,90]`."""
 
     distance: ct.BatchableDistance = eqx.field(
-        converter=partial(Distance.constructor, dtype=float)
+        converter=lambda x: x
+        if isinstance(x, AbstractDistance)
+        else Distance.constructor(x, dtype=float)
     )
     r"""Radial distance :math:`r \in [0,+\infty)`."""
 
     def __check_init__(self) -> None:
         """Check the validity of the initialization."""
         check_azimuth_range(self.lon)
         check_polar_range(self.lat, -Quantity(90, "deg"), Quantity(90, "deg"))
```

### Comparing `coordinax-0.4.3/src/coordinax/_d3/transform.py` & `coordinax-0.5/src/coordinax/_d3/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     LonLatSphericalDifferential,
     LonLatSphericalVector,
     MathSphericalDifferential,
     MathSphericalVector,
     SphericalDifferential,
     SphericalVector,
 )
-from coordinax._base_vec import AbstractVector
+from coordinax._base_pos import AbstractPosition
 
 ###############################################################################
 # 3D
 
 
 @dispatch
 def represent_as(
@@ -92,29 +92,29 @@
     True
 
     """
     return current
 
 
 @dispatch.multi(
-    (CartesianDifferential3D, type[CartesianDifferential3D], AbstractVector),
-    (CylindricalDifferential, type[CylindricalDifferential], AbstractVector),
-    (SphericalDifferential, type[SphericalDifferential], AbstractVector),
-    (LonLatSphericalDifferential, type[LonLatSphericalDifferential], AbstractVector),
+    (CartesianDifferential3D, type[CartesianDifferential3D], AbstractPosition),
+    (CylindricalDifferential, type[CylindricalDifferential], AbstractPosition),
+    (SphericalDifferential, type[SphericalDifferential], AbstractPosition),
+    (LonLatSphericalDifferential, type[LonLatSphericalDifferential], AbstractPosition),
     (
         LonCosLatSphericalDifferential,
         type[LonCosLatSphericalDifferential],
-        AbstractVector,
+        AbstractPosition,
     ),
-    (MathSphericalDifferential, type[MathSphericalDifferential], AbstractVector),
+    (MathSphericalDifferential, type[MathSphericalDifferential], AbstractPosition),
 )
 def represent_as(
     current: Abstract3DVectorDifferential,
     target: type[Abstract3DVectorDifferential],
-    position: AbstractVector,
+    position: AbstractPosition,
     /,
     **kwargs: Any,
 ) -> Abstract3DVectorDifferential:
     """Self transforms for 3D differentials.
 
     Examples
     --------
@@ -351,17 +351,17 @@
     >>> vec = cx.SphericalVector(r=Quantity(1., "kpc"), theta=Quantity(90, "deg"),
     ...                          phi=Quantity(90, "deg"))
     >>> print(cx.represent_as(vec, cx.Cartesian3DVector))
     <Cartesian3DVector (x[kpc], y[kpc], z[kpc])
         [-4.371e-08  1.000e+00 -4.371e-08]>
 
     """
-    x = current.r * xp.sin(current.theta) * xp.cos(current.phi)
-    y = current.r * xp.sin(current.theta) * xp.sin(current.phi)
-    z = current.r * xp.cos(current.theta)
+    x = current.r.distance * xp.sin(current.theta) * xp.cos(current.phi)
+    y = current.r.distance * xp.sin(current.theta) * xp.sin(current.phi)
+    z = current.r.distance * xp.cos(current.theta)
     return target(x=x, y=y, z=z)
 
 
 @dispatch
 def represent_as(
     current: SphericalVector, target: type[CylindricalVector], /, **kwargs: Any
 ) -> CylindricalVector:
@@ -375,16 +375,16 @@
     >>> vec = cx.SphericalVector(r=Quantity(1., "kpc"), theta=Quantity(90, "deg"),
     ...                          phi=Quantity(90, "deg"))
     >>> print(cx.represent_as(vec, cx.CylindricalVector))
     <CylindricalVector (rho[kpc], phi[deg], z[kpc])
         [ 1.000e+00  9.000e+01 -4.371e-08]>
 
     """
-    rho = xp.abs(current.r * xp.sin(current.theta))
-    z = current.r * xp.cos(current.theta)
+    rho = xp.abs(current.r.distance * xp.sin(current.theta))
+    z = current.r.distance * xp.cos(current.theta)
     return target(rho=rho, phi=current.phi, z=z)
 
 
 @dispatch
 def represent_as(
     current: SphericalVector, target: type[LonLatSphericalVector], /, **kwargs: Any
 ) -> LonLatSphericalVector:
@@ -515,17 +515,17 @@
     >>> vec = cx.MathSphericalVector(r=Quantity(1., "kpc"), theta=Quantity(90, "deg"),
     ...                              phi=Quantity(90, "deg"))
     >>> print(cx.represent_as(vec, cx.Cartesian3DVector))
     <Cartesian3DVector (x[kpc], y[kpc], z[kpc])
         [-4.371e-08  1.000e+00 -4.371e-08]>
 
     """
-    x = current.r * xp.sin(current.phi) * xp.cos(current.theta)
-    y = current.r * xp.sin(current.phi) * xp.sin(current.theta)
-    z = current.r * xp.cos(current.phi)
+    x = current.r.distance * xp.sin(current.phi) * xp.cos(current.theta)
+    y = current.r.distance * xp.sin(current.phi) * xp.sin(current.theta)
+    z = current.r.distance * xp.cos(current.phi)
     return target(x=x, y=y, z=z)
 
 
 @dispatch
 def represent_as(
     current: MathSphericalVector, target: type[CylindricalVector], /, **kwargs: Any
 ) -> CylindricalVector:
@@ -539,16 +539,16 @@
     >>> vec = cx.MathSphericalVector(r=Quantity(1., "kpc"), theta=Quantity(90, "deg"),
     ...                              phi=Quantity(90, "deg"))
     >>> print(cx.represent_as(vec, cx.CylindricalVector))
     <CylindricalVector (rho[kpc], phi[deg], z[kpc])
         [ 1.000e+00  9.000e+01 -4.371e-08]>
 
     """
-    rho = xp.abs(current.r * xp.sin(current.phi))
-    z = current.r * xp.cos(current.phi)
+    rho = xp.abs(current.r.distance * xp.sin(current.phi))
+    z = current.r.distance * xp.cos(current.phi)
     return target(rho=rho, phi=current.theta, z=z)
 
 
 @dispatch
 def represent_as(
     current: MathSphericalVector, target: type[SphericalVector], /, **kwargs: Any
 ) -> SphericalVector:
@@ -573,15 +573,15 @@
 # LonLatSphericalDifferential
 
 
 @dispatch
 def represent_as(
     current: Abstract3DVectorDifferential,
     target: type[LonCosLatSphericalDifferential],
-    position: AbstractVector | Quantity["length"],
+    position: AbstractPosition | Quantity["length"],
     /,
     **kwargs: Any,
 ) -> LonCosLatSphericalDifferential:
     """Abstract3DVectorDifferential -> LonCosLatSphericalDifferential.
 
     Examples
     --------
@@ -602,16 +602,16 @@
       d_distance=Quantity[...]( value=f32[], unit=Unit("km / s") )
     )
 
     >>> newdif.d_lon_coslat / xp.cos(vec.lat)  # float32 imprecision
     Quantity['angular frequency'](Array(6.9999995, dtype=float32), unit='mas / yr')
 
     """
-    # Parse the position to an AbstractVector
-    if isinstance(position, AbstractVector):
+    # Parse the position to an AbstractPosition
+    if isinstance(position, AbstractPosition):
         posvec = position
     else:  # Q -> Cart<X>D
         posvec = current.integral_cls._cartesian_cls.constructor(  # noqa: SLF001
             position
         )
 
     # Transform the differential to LonLatSphericalDifferential
@@ -628,21 +628,21 @@
     )
 
 
 @dispatch
 def represent_as(
     current: LonCosLatSphericalDifferential,
     target: type[LonLatSphericalDifferential],
-    position: AbstractVector | Quantity["length"],
+    position: AbstractPosition | Quantity["length"],
     /,
     **kwargs: Any,
 ) -> LonLatSphericalDifferential:
     """LonCosLatSphericalDifferential -> LonLatSphericalDifferential."""
-    # Parse the position to an AbstractVector
-    if isinstance(position, AbstractVector):
+    # Parse the position to an AbstractPosition
+    if isinstance(position, AbstractPosition):
         posvec = position
     else:  # Q -> Cart<X>D
         posvec = current.integral_cls._cartesian_cls.constructor(  # noqa: SLF001
             position
         )
 
     # Transform the position to the required type
@@ -656,21 +656,21 @@
     )
 
 
 @dispatch
 def represent_as(
     current: LonCosLatSphericalDifferential,
     target: type[Abstract3DVectorDifferential],
-    position: AbstractVector | Quantity["length"],
+    position: AbstractPosition | Quantity["length"],
     /,
     **kwargs: Any,
 ) -> Abstract3DVectorDifferential:
     """LonCosLatSphericalDifferential -> Abstract3DVectorDifferential."""
-    # Parse the position to an AbstractVector
-    if isinstance(position, AbstractVector):
+    # Parse the position to an AbstractPosition
+    if isinstance(position, AbstractPosition):
         posvec = position
     else:  # Q -> Cart<X>D
         posvec = current.integral_cls._cartesian_cls.constructor(  # noqa: SLF001
             position
         )
     # Transform the differential to LonLatSphericalDifferential
     current = represent_as(current, LonLatSphericalDifferential, posvec)
```

### Comparing `coordinax-0.4.3/src/coordinax/_d4/compat.py` & `coordinax-0.5/src/coordinax/_d4/compat.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/_d4/operate.py` & `coordinax-0.5/src/coordinax/_d4/operate.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/_d4/spacetime.py` & `coordinax-0.5/src/coordinax/_d4/spacetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import jax.numpy as jnp
 from jaxtyping import Shaped
 
 import quaxed.array_api as xp
 from unxt import Quantity
 
 from .base import Abstract4DVector
-from coordinax._base import AbstractVectorBase
+from coordinax._base import AbstractVector
 from coordinax._d3.base import Abstract3DVector
 from coordinax._d3.builtin import Cartesian3DVector
 from coordinax._typing import BatchableLength, BatchableTime, ScalarTime
 from coordinax._utils import classproperty
 
 if TYPE_CHECKING:
     from typing_extensions import Never
@@ -98,15 +98,15 @@
             msg = "t and q must be broadcastable to the same shape."
             raise ValueError(msg)
 
     # ---------------------------------------------------------------
     # Constructors
 
     @classmethod
-    @AbstractVectorBase.constructor._f.dispatch  # type: ignore[attr-defined, misc]  # noqa: SLF001
+    @AbstractVector.constructor._f.dispatch  # type: ignore[attr-defined, misc]  # noqa: SLF001
     def constructor(
         cls: "type[FourVector]",
         obj: Quantity | u.Quantity,
         /,  # TODO: shape hint
     ) -> "FourVector":
         """Construct a vector from a Quantity array.
 
@@ -175,15 +175,15 @@
         """
         return getattr(self.q, name)
 
     # -------------------------------------------
 
     @classproperty
     @classmethod
-    def _cartesian_cls(cls) -> type[AbstractVectorBase]:
+    def _cartesian_cls(cls) -> type[AbstractVector]:
         msg = "Not yet implemented"
         raise NotImplementedError(msg)
 
     @classproperty
     @classmethod
     def differential_cls(cls) -> "Never":  # type: ignore[override]
         msg = "Not yet implemented"
```

### Comparing `coordinax-0.4.3/src/coordinax/_transform/d1.py` & `coordinax-0.5/src/coordinax/_transform/d1.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/_transform/d2.py` & `coordinax-0.5/src/coordinax/_transform/d2.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/_transform/d3.py` & `coordinax-0.5/src/coordinax/_transform/d3.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/_transform/differentials.py` & `coordinax-0.5/src/coordinax/_transform/differentials.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 """Transformations between representations."""
 
 __all__ = ["represent_as"]
 
+from dataclasses import replace
 from math import prod
 from typing import Any
 
 import jax
 from plum import dispatch
 
 import quaxed.array_api as xp
-from unxt import Quantity
+from unxt import AbstractDistance, Quantity
 
-from coordinax._base_dif import AbstractVectorDifferential
-from coordinax._base_vec import AbstractVector
+from coordinax._base_pos import AbstractPosition
+from coordinax._base_vel import AbstractVelocity
 from coordinax._d1.base import Abstract1DVectorDifferential
 from coordinax._d2.base import Abstract2DVectorDifferential
 from coordinax._d3.base import Abstract3DVectorDifferential
 from coordinax._utils import dataclass_items
 
 
 # TODO: implement for cross-representations
 @dispatch.multi(  # type: ignore[misc]
     # N-D -> N-D
     (
         Abstract1DVectorDifferential,
         type[Abstract1DVectorDifferential],  # type: ignore[misc]
-        AbstractVector | Quantity["length"],
+        AbstractPosition | Quantity["length"],
     ),
     (
         Abstract2DVectorDifferential,
         type[Abstract2DVectorDifferential],  # type: ignore[misc]
-        AbstractVector | Quantity["length"],
+        AbstractPosition | Quantity["length"],
     ),
     (
         Abstract3DVectorDifferential,
         type[Abstract3DVectorDifferential],  # type: ignore[misc]
-        AbstractVector | Quantity["length"],
+        AbstractPosition | Quantity["length"],
     ),
 )
 def represent_as(
-    current: AbstractVectorDifferential,
-    target: type[AbstractVectorDifferential],
-    position: AbstractVector | Quantity["length"],
+    current: AbstractVelocity,
+    target: type[AbstractVelocity],
+    position: AbstractPosition | Quantity["length"],
     /,
     **kwargs: Any,
-) -> AbstractVectorDifferential:
-    """AbstractVectorDifferential -> Cartesian -> AbstractVectorDifferential.
+) -> AbstractVelocity:
+    """AbstractVelocity -> Cartesian -> AbstractVelocity.
 
     This is the base case for the transformation of vector differentials.
 
     Parameters
     ----------
-    current : AbstractVectorDifferential
+    current : AbstractVelocity
         The vector differential to transform.
-    target : type[AbstractVectorDifferential]
+    target : type[AbstractVelocity]
         The target type of the vector differential.
-    position : AbstractVector
+    position : AbstractPosition
         The position vector used to transform the differential.
     **kwargs : Any
         Additional keyword arguments.
 
     Examples
     --------
     >>> import coordinax as cx
@@ -105,27 +106,36 @@
     )
 
     """
     # TODO: not require the shape munging / support more shapes
     shape = current.shape
     flat_shape = prod(shape)
 
-    # Parse the position to an AbstractVector
-    if isinstance(position, AbstractVector):
+    # Parse the position to an AbstractPosition
+    if isinstance(position, AbstractPosition):
         posvec = position
     else:  # Q -> Cart<X>D
         posvec = current.integral_cls._cartesian_cls.constructor(  # noqa: SLF001
             position
         )
 
     posvec = posvec.reshape(flat_shape)  # flattened
 
     # Start by transforming the position to the type required by the
     # differential to construct the Jacobian.
     current_pos = represent_as(posvec, current.integral_cls, **kwargs)
+    # TODO: not need to cast to distance
+    current_pos = replace(
+        current_pos,
+        **{
+            k: v.distance
+            for k, v in dataclass_items(current_pos)
+            if isinstance(v, AbstractDistance)
+        },
+    )
 
     # Takes the Jacobian through the representation transformation function.  This
     # returns a representation of the target type, where the value of each field the
     # corresponding row of the Jacobian. The value of the field is a Quantity with
     # the correct numerator unit (of the Jacobian row). The value is a Vector of the
     # original type, with fields that are the columns of that row, but with only the
     # denomicator's units.
```

### Comparing `coordinax-0.4.3/src/coordinax/operators/_base.py` & `coordinax-0.5/src/coordinax/operators/_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import TYPE_CHECKING, Any
 
 import equinox as eqx
 from plum import dispatch
 
 from unxt import Quantity
 
-from coordinax._base_vec import AbstractVector
+from coordinax._base_pos import AbstractPosition
 from coordinax._utils import dataclass_items
 
 if TYPE_CHECKING:
     from ._sequential import OperatorSequence
 
 
 class AbstractOperator(eqx.Module):  # type: ignore[misc]
@@ -52,28 +52,28 @@
         return cls(**obj)
 
     # -------------------------------------------
 
     @dispatch.abstract
     def __call__(
         self: "AbstractOperator",
-        x: AbstractVector,  # noqa: ARG002
+        x: AbstractPosition,  # noqa: ARG002
         /,
-    ) -> AbstractVector:
+    ) -> AbstractPosition:
         """Apply the operator to the coordinates `x`."""
         msg = "implement this method in the subclass"
         raise TypeError(msg)
 
     @dispatch.abstract
     def __call__(
         self: "AbstractOperator",
-        x: AbstractVector,  # noqa: ARG002
+        x: AbstractPosition,  # noqa: ARG002
         t: Quantity["time"],  # noqa: ARG002
         /,
-    ) -> AbstractVector:
+    ) -> AbstractPosition:
         """Apply the operator to the coordinates `x` at a time `t`."""
         msg = "implement this method in the subclass"
         raise TypeError(msg)
 
     # -------------------------------------------
 
     @property
```

### Comparing `coordinax-0.4.3/src/coordinax/operators/_composite.py` & `coordinax-0.5/src/coordinax/operators/_composite.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from collections.abc import Iterator
 from dataclasses import replace
 from typing import TYPE_CHECKING, Protocol, overload, runtime_checkable
 
 from unxt import Quantity
 
 from ._base import AbstractOperator, op_call_dispatch
-from coordinax._base_vec import AbstractVector
+from coordinax._base_pos import AbstractPosition
 from coordinax._utils import DataclassInstance
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
 
 @runtime_checkable
@@ -39,30 +39,30 @@
     # Operator
 
     # TODO: how to have the `operators` attribute in a way that allows for both
     # writeable (in the constructor) and read-only (as a property) subclasses.
 
     @op_call_dispatch(precedence=1)
     def __call__(
-        self: "AbstractCompositeOperator", x: AbstractVector, /
-    ) -> AbstractVector:
+        self: "AbstractCompositeOperator", x: AbstractPosition, /
+    ) -> AbstractPosition:
         """Apply the operator to the coordinates.
 
         This is the default implementation, which applies the operators in
         sequence.
         """
         # TODO: with lax.scan?
         for op in self.operators:
             x = op(x)
         return x
 
     @op_call_dispatch(precedence=1)
     def __call__(
-        self: "AbstractCompositeOperator", x: AbstractVector, t: Quantity["time"], /
-    ) -> tuple[AbstractVector, Quantity["time"]]:
+        self: "AbstractCompositeOperator", x: AbstractPosition, t: Quantity["time"], /
+    ) -> tuple[AbstractPosition, Quantity["time"]]:
         """Apply the operator to the coordinates."""
         # TODO: with lax.scan?
         for op in self.operators:
             x, t = op(x, t)
         return x, t
 
     @property
```

### Comparing `coordinax-0.4.3/src/coordinax/operators/_funcs.py` & `coordinax-0.5/src/coordinax/operators/_funcs.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/operators/_identity.py` & `coordinax-0.5/src/coordinax/operators/_identity.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Literal, final
 
 from jaxtyping import Shaped
 
 from unxt import Quantity
 
 from ._base import AbstractOperator, op_call_dispatch
-from coordinax._base_vec import AbstractVector
+from coordinax._base_pos import AbstractPosition
 
 
 @final
 class IdentityOperator(AbstractOperator):
     """Identity operation.
 
     This is the identity operation, which does nothing to the input.
@@ -129,15 +129,15 @@
         return self
 
     # -------------------------------------------
     # Dispatched call signatures
     # More call signatures are registered in the `coordinax._d<X>.operate` modules.
 
     @op_call_dispatch(precedence=1)
-    def __call__(self: "IdentityOperator", x: AbstractVector, /) -> AbstractVector:
+    def __call__(self: "IdentityOperator", x: AbstractPosition, /) -> AbstractPosition:
         """Apply the Identity operation.
 
         This is the identity operation, which does nothing to the input.
 
         Examples
         --------
         >>> from unxt import Quantity
@@ -171,16 +171,16 @@
         True
 
         """
         return x
 
     @op_call_dispatch(precedence=1)
     def __call__(
-        self: "IdentityOperator", x: AbstractVector, t: Quantity["time"], /
-    ) -> tuple[AbstractVector, Quantity["time"]]:
+        self: "IdentityOperator", x: AbstractPosition, t: Quantity["time"], /
+    ) -> tuple[AbstractPosition, Quantity["time"]]:
         """Apply the Identity operation."""  # TODO: docstring
         return x, t
 
     @op_call_dispatch(precedence=1)
     def __call__(
         self: "IdentityOperator", x: Shaped[Quantity, "*shape"], t: Quantity["time"], /
     ) -> tuple[Shaped[Quantity, "*shape"], Quantity["time"]]:
```

### Comparing `coordinax-0.4.3/src/coordinax/operators/_sequential.py` & `coordinax-0.5/src/coordinax/operators/_sequential.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/operators/_galilean/__init__.py` & `coordinax-0.5/src/coordinax/operators/_galilean/__init__.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/operators/_galilean/base.py` & `coordinax-0.5/src/coordinax/operators/_galilean/base.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/operators/_galilean/boost.py` & `coordinax-0.5/src/coordinax/operators/_galilean/boost.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/operators/_galilean/composite.py` & `coordinax-0.5/src/coordinax/operators/_galilean/composite.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/operators/_galilean/rotation.py` & `coordinax-0.5/src/coordinax/operators/_galilean/rotation.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/src/coordinax/operators/_galilean/translation.py` & `coordinax-0.5/src/coordinax/operators/_galilean/translation.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,34 +11,34 @@
 import jax.numpy as jnp
 from plum import convert
 
 import quaxed.array_api as xp
 from unxt import Quantity
 
 from .base import AbstractGalileanOperator
-from coordinax._base_vec import AbstractVector
+from coordinax._base_pos import AbstractPosition
 from coordinax._d1.builtin import Cartesian1DVector
 from coordinax._d2.builtin import Cartesian2DVector
 from coordinax._d3.base import Abstract3DVector
 from coordinax._d3.builtin import Cartesian3DVector
 from coordinax._d4.spacetime import FourVector
 from coordinax.operators._base import AbstractOperator, op_call_dispatch
 from coordinax.operators._funcs import simplify_op
 from coordinax.operators._identity import IdentityOperator
 
 ##############################################################################
 # Spatial Translations
 
 
-def _converter_spatialtranslation(x: Any) -> AbstractVector:
+def _converter_spatialtranslation(x: Any) -> AbstractPosition:
     """Convert to a spatial translation vector."""
-    out: AbstractVector | None = None
+    out: AbstractPosition | None = None
     if isinstance(x, GalileanSpatialTranslationOperator):
         out = x.translation
-    elif isinstance(x, AbstractVector):
+    elif isinstance(x, AbstractPosition):
         out = x
     elif isinstance(x, Quantity):
         shape: tuple[int, ...] = x.shape
         match shape:
             case (1,):
                 out = Cartesian1DVector.constructor(x)
             case (2,):
@@ -99,15 +99,15 @@
     >>> shift = SphericalVector(r=Quantity(1.0, "kpc"),
     ...                         theta=Quantity(xp.pi/2, "rad"),
     ...                         phi=Quantity(0, "rad"))
     >>> op = cx.operators.GalileanSpatialTranslationOperator(shift)
     >>> op
     GalileanSpatialTranslationOperator( translation=SphericalVector( ... ) )
 
-    Translation operators can be applied to :class:`vector.AbstractVector`:
+    Translation operators can be applied to :class:`vector.AbstractPosition`:
 
     >>> q = cx.Cartesian3DVector.constructor(Quantity([0, 0, 0], "kpc"))
     >>> op(q)
     Cartesian3DVector( ... )
 
     And to :class:`~unxt.Quantity`:
 
@@ -162,15 +162,15 @@
 
     >>> t = Quantity(0, "Gyr")
     >>> op(q, t)[1] is t
     True
 
     """
 
-    translation: AbstractVector = eqx.field(converter=_converter_spatialtranslation)
+    translation: AbstractPosition = eqx.field(converter=_converter_spatialtranslation)
     """The spatial translation.
 
     This parameters accepts either a :class:`vector.AbstracVector` instance or
     uses a Cartesian vector constructor to enable a variety of more convenient
     input types to create a Cartesian vector. See
     :class:`vector.Cartesian3DVector.constructor` for an example when doing a 3D
     translation.
@@ -219,16 +219,16 @@
         """
         return GalileanSpatialTranslationOperator(-self.translation)
 
     # -------------------------------------------
 
     @op_call_dispatch(precedence=1)
     def __call__(
-        self: "GalileanSpatialTranslationOperator", q: AbstractVector, /
-    ) -> AbstractVector:
+        self: "GalileanSpatialTranslationOperator", q: AbstractPosition, /
+    ) -> AbstractPosition:
         """Apply the translation to the coordinates.
 
         Examples
         --------
         >>> from unxt import Quantity
         >>> from coordinax import Cartesian3DVector
         >>> from coordinax.operators import GalileanSpatialTranslationOperator
@@ -244,18 +244,18 @@
 
         """
         return q + self.translation
 
     @op_call_dispatch(precedence=1)
     def __call__(
         self: "GalileanSpatialTranslationOperator",
-        q: AbstractVector,
+        q: AbstractPosition,
         t: Quantity["time"],
         /,
-    ) -> tuple[AbstractVector, Quantity["time"]]:
+    ) -> tuple[AbstractPosition, Quantity["time"]]:
         """Apply the translation to the coordinates.
 
         Examples
         --------
         >>> from unxt import Quantity
         >>> from coordinax import Cartesian3DVector
         >>> from coordinax.operators import GalileanSpatialTranslationOperator
@@ -276,15 +276,15 @@
 
         """
         return q + self.translation, t
 
     @op_call_dispatch(precedence=1)
     def __call__(
         self: "GalileanSpatialTranslationOperator", v4: FourVector, /
-    ) -> AbstractVector:
+    ) -> AbstractPosition:
         """Apply the translation to the coordinates."""  # TODO: docstring
         return replace(v4, q=v4.q + self.translation)
 
 
 @simplify_op.register
 def _simplify_op_spatialtranslation(
     op: GalileanSpatialTranslationOperator, /, **kwargs: Any
```

### Comparing `coordinax-0.4.3/tests/test_base.py` & `coordinax-0.5/tests/test_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from coordinax import (
     Abstract1DVector,
     Abstract1DVectorDifferential,
     Abstract2DVector,
     Abstract2DVectorDifferential,
     Abstract3DVector,
     Abstract3DVectorDifferential,
-    AbstractVector,
-    AbstractVectorDifferential,
+    AbstractPosition,
+    AbstractVelocity,
     Cartesian1DVector,
     Cartesian2DVector,
     Cartesian3DVector,
     CartesianDifferential1D,
     CartesianDifferential2D,
     CartesianDifferential3D,
     CylindricalDifferential,
@@ -66,15 +66,15 @@
     CartesianDifferential3D,
     SphericalDifferential,
     CylindricalDifferential,
 ]
 
 
 def context_dimension_reduction(
-    vector: AbstractVector, target: type[AbstractVector]
+    vector: AbstractPosition, target: type[AbstractPosition]
 ) -> AbstractContextManager[Any]:
     """Return a context manager that checks for dimensionality reduction."""
     context: AbstractContextManager[Any]
     if (
         isinstance(vector, Abstract2DVector) and issubclass(target, Abstract1DVector)
     ) or (
         isinstance(vector, Abstract3DVector)
@@ -82,16 +82,16 @@
     ):
         context = pytest.warns(IrreversibleDimensionChange)
     else:
         context = nullcontext()
     return context
 
 
-class AbstractVectorBaseTest:
-    """Test :class:`coordinax.AbstractVectorBase`."""
+class AbstractVectorTest:
+    """Test :class:`coordinax.AbstractVector`."""
 
     # ===============================================================
     # Array
 
     def test_shape(self, vector):
         """Test :meth:`AbstractVector.shape`."""
         shape = vector.shape
@@ -179,54 +179,54 @@
         # Simple test
         shapes = vector.shapes
         assert isinstance(shapes, MappingProxyType)
         assert set(shapes.keys()) == set(vector.components)
         assert all(v == getattr(vector, k).shape for k, v in shapes.items())
 
 
-class AbstractVectorTest(AbstractVectorBaseTest):
-    """Test :class:`coordinax.AbstractVector`."""
+class AbstractPositionTest(AbstractVectorTest):
+    """Test :class:`coordinax.AbstractPosition`."""
 
     @pytest.fixture(scope="class")
-    def vector(self) -> AbstractVector:  # noqa: PT004
+    def vector(self) -> AbstractPosition:  # noqa: PT004
         """Return a vector."""
         raise NotImplementedError
 
     @pytest.mark.parametrize("target", BUILTIN_VECTORS)
     def test_represent_as(self, vector, target):
-        """Test :meth:`AbstractVector.represent_as`.
+        """Test :meth:`AbstractPosition.represent_as`.
 
         This just tests that the machiner works.
         """
         # Perform the conversion.
         # Detecting whether the conversion reduces the dimensionality.
         with context_dimension_reduction(vector, target):
             newvec = vector.represent_as(target)
 
         # Test
         assert isinstance(newvec, target)
 
 
-class AbstractVectorDifferentialTest(AbstractVectorBaseTest):
-    """Test :class:`coordinax.AbstractVectorDifferential`."""
+class AbstractVelocityTest(AbstractVectorTest):
+    """Test :class:`coordinax.AbstractVelocity`."""
 
     @pytest.fixture(scope="class")
-    def vector(self) -> AbstractVector:  # noqa: PT004
+    def vector(self) -> AbstractPosition:  # noqa: PT004
         """Return a vector."""
         raise NotImplementedError
 
     @pytest.fixture(scope="class")
-    def difntl(self) -> AbstractVectorDifferential:  # noqa: PT004
+    def difntl(self) -> AbstractVelocity:  # noqa: PT004
         """Return a vector."""
         raise NotImplementedError
 
     @pytest.mark.parametrize("target", BUILTIN_DIFFERENTIALS)
     @pytest.mark.filterwarnings("ignore:Explicitly requested dtype")
     def test_represent_as(self, difntl, target, vector):
-        """Test :meth:`AbstractVector.represent_as`.
+        """Test :meth:`AbstractPosition.represent_as`.
 
         This just tests that the machiner works.
         """
         # TODO: have all the conversions
         if (
             (
                 isinstance(difntl, Abstract1DVectorDifferential)
```

### Comparing `coordinax-0.4.3/tests/test_d1.py` & `coordinax-0.5/tests/test_d1.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 import pytest
 
 import quaxed.numpy as qnp
 from unxt import Quantity
 
 import coordinax as cx
-from .test_base import AbstractVectorDifferentialTest, AbstractVectorTest
+from .test_base import AbstractPositionTest, AbstractVelocityTest
 
 
-class Abstract1DVectorTest(AbstractVectorTest):
+class Abstract1DVectorTest(AbstractPositionTest):
     """Test :class:`coordinax.Abstract1DVector`."""
 
     # TODO: Add tests
 
 
 class TestCartesian1DVector(Abstract1DVectorTest):
     """Test :class:`coordinax.Cartesian1DVector`."""
 
     @pytest.fixture(scope="class")
-    def vector(self) -> cx.AbstractVector:
+    def vector(self) -> cx.AbstractPosition:
         """Return a vector."""
         return cx.Cartesian1DVector(x=Quantity([1, 2, 3, 4], "kpc"))
 
     # ==========================================================================
     # represent_as
 
     def test_cartesian1d_to_cartesian1d(self, vector):
@@ -101,15 +101,15 @@
         assert qnp.array_equal(cylindrical.z, Quantity([4, 5, 6, 7], "m"))
 
 
 class TestRadialVector(Abstract1DVectorTest):
     """Test :class:`coordinax.RadialVector`."""
 
     @pytest.fixture(scope="class")
-    def vector(self) -> cx.AbstractVector:
+    def vector(self) -> cx.AbstractPosition:
         """Return a vector."""
         return cx.RadialVector(r=Quantity([1, 2, 3, 4], "kpc"))
 
     # ==========================================================================
     # represent_as
 
     def test_radial_to_cartesian1d(self, vector):
@@ -183,15 +183,15 @@
 
         assert isinstance(cylindrical, cx.CylindricalVector)
         assert qnp.array_equal(cylindrical.rho, Quantity([1, 2, 3, 4], "kpc"))
         assert qnp.array_equal(cylindrical.phi, Quantity([0, 1, 2, 3], "rad"))
         assert qnp.array_equal(cylindrical.z, Quantity([4, 5, 6, 7], "m"))
 
 
-class Abstract1DVectorDifferentialTest(AbstractVectorDifferentialTest):
+class Abstract1DVectorDifferentialTest(AbstractVelocityTest):
     """Test :class:`coordinax.Abstract1DVectorDifferential`."""
 
 
 class TestCartesianDifferential1D(Abstract1DVectorDifferentialTest):
     """Test :class:`coordinax.CartesianDifferential1D`."""
 
     @pytest.fixture(scope="class")
```

### Comparing `coordinax-0.4.3/tests/test_d2.py` & `coordinax-0.5/tests/test_d2.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import pytest
 
 import quaxed.array_api as xp
 import quaxed.numpy as qnp
 from unxt import Quantity
 
 import coordinax as cx
-from .test_base import AbstractVectorDifferentialTest, AbstractVectorTest
+from .test_base import AbstractPositionTest, AbstractVelocityTest
 
 
-class Abstract2DVectorTest(AbstractVectorTest):
+class Abstract2DVectorTest(AbstractPositionTest):
     """Test :class:`coordinax.Abstract2DVector`."""
 
 
 class TestCartesian2DVector:
     """Test :class:`coordinax.Cartesian2DVector`."""
 
     @pytest.fixture(scope="class")
@@ -113,15 +113,15 @@
         assert qnp.array_equal(cylindrical.z, Quantity([9, 10, 11, 12], "m"))
 
 
 class TestPolarVector:
     """Test :class:`coordinax.PolarVector`."""
 
     @pytest.fixture(scope="class")
-    def vector(self) -> cx.AbstractVector:
+    def vector(self) -> cx.AbstractPosition:
         """Return a vector."""
         return cx.PolarVector(
             r=Quantity([1, 2, 3, 4], "kpc"), phi=Quantity([0, 1, 2, 3], "rad")
         )
 
     # ==========================================================================
     # represent_as
@@ -211,15 +211,15 @@
 
         assert isinstance(cylindrical, cx.CylindricalVector)
         assert qnp.array_equal(cylindrical.rho, Quantity([1, 2, 3, 4], "kpc"))
         assert qnp.array_equal(cylindrical.phi, Quantity([0, 1, 2, 3], "rad"))
         assert qnp.array_equal(cylindrical.z, Quantity([9, 10, 11, 12], "m"))
 
 
-class Abstract2DVectorDifferentialTest(AbstractVectorDifferentialTest):
+class Abstract2DVectorDifferentialTest(AbstractVelocityTest):
     """Test :class:`coordinax.Abstract2DVectorDifferential`."""
 
 
 class TestCartesianDifferential2D(Abstract2DVectorDifferentialTest):
     """Test :class:`coordinax.CartesianDifferential2D`."""
 
     @pytest.fixture(scope="class")
```

### Comparing `coordinax-0.4.3/tests/test_d3.py` & `coordinax-0.5/tests/test_d3.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 from plum import convert
 
 import quaxed.array_api as xp
 import quaxed.numpy as qnp
 from unxt import Quantity
 
 import coordinax as cx
-from .test_base import AbstractVectorDifferentialTest, AbstractVectorTest
+from .test_base import AbstractPositionTest, AbstractVelocityTest
 
 
-class Abstract3DVectorTest(AbstractVectorTest):
+class Abstract3DVectorTest(AbstractPositionTest):
     """Test :class:`coordinax.Abstract3DVector`."""
 
     # ==========================================================================
     # Unary operations
 
     def test_neg_compare_apy(
-        self, vector: cx.AbstractVector, apyvector: apyc.BaseRepresentation
+        self, vector: cx.AbstractPosition, apyvector: apyc.BaseRepresentation
     ):
         """Test negation."""
         # To take the negative, Vector converts to Cartesian coordinates, takes
         # the negative, then converts back to the original representation.
         # This can result in equivalent but different angular coordinates than
         # Astropy. AFAIK this only happens at the poles.
         cart = convert(-vector, type(apyvector)).represent_as(
@@ -55,24 +55,24 @@
         #     )
 
 
 class TestCartesian3DVector(Abstract3DVectorTest):
     """Test :class:`coordinax.Cartesian3DVector`."""
 
     @pytest.fixture(scope="class")
-    def vector(self) -> cx.AbstractVector:
+    def vector(self) -> cx.AbstractPosition:
         """Return a vector."""
         return cx.Cartesian3DVector(
             x=Quantity([1, 2, 3, 4], "kpc"),
             y=Quantity([5, 6, 7, 8], "kpc"),
             z=Quantity([9, 10, 11, 12], "kpc"),
         )
 
     @pytest.fixture(scope="class")
-    def apyvector(self, vector: cx.AbstractVector) -> apyc.CartesianRepresentation:
+    def apyvector(self, vector: cx.AbstractPosition) -> apyc.CartesianRepresentation:
         """Return an Astropy vector."""
         return convert(vector, apyc.CartesianRepresentation)
 
     # ==========================================================================
     # represent_as
 
     @pytest.mark.filterwarnings("ignore:Irreversible dimension change")
@@ -181,24 +181,24 @@
         assert np.allclose(convert(cyl.z, APYQuantity), apycyl.z)
 
 
 class TestCylindricalVector(Abstract3DVectorTest):
     """Test :class:`coordinax.CylindricalVector`."""
 
     @pytest.fixture(scope="class")
-    def vector(self) -> cx.AbstractVector:
+    def vector(self) -> cx.AbstractPosition:
         """Return a vector."""
         return cx.CylindricalVector(
             rho=Quantity([1, 2, 3, 4], "kpc"),
             phi=Quantity([0, 1, 2, 3], "rad"),
             z=Quantity([9, 10, 11, 12], "m"),
         )
 
     @pytest.fixture(scope="class")
-    def apyvector(self, vector: cx.AbstractVector):
+    def apyvector(self, vector: cx.AbstractPosition):
         """Return an Astropy vector."""
         return convert(vector, apyc.CylindricalRepresentation)
 
     # ==========================================================================
     # represent_as
 
     @pytest.mark.filterwarnings("ignore:Irreversible dimension change")
@@ -311,15 +311,15 @@
         return cx.SphericalVector(
             r=Quantity([1, 2, 3, 4], "kpc"),
             theta=Quantity([0, 36, 142, 180], "deg"),
             phi=Quantity([0, 65, 135, 270], "deg"),
         )
 
     @pytest.fixture(scope="class")
-    def apyvector(self, vector: cx.AbstractVector):
+    def apyvector(self, vector: cx.AbstractPosition):
         """Return an Astropy vector."""
         return convert(vector, apyc.PhysicsSphericalRepresentation)
 
     # ==========================================================================
     # represent_as
 
     @pytest.mark.filterwarnings("ignore:Irreversible dimension change")
@@ -413,22 +413,21 @@
     def test_spherical_to_cylindrical_astropy(self, vector, apyvector):
         """Test ``coordinax.represent_as(CylindricalVector)``."""
         cyl = vector.represent_as(
             cx.CylindricalVector, z=Quantity([9, 10, 11, 12], "m")
         )
 
         apycyl = apyvector.represent_as(apyc.CylindricalRepresentation)
-        assert np.allclose(convert(cyl.rho, APYQuantity), apycyl.rho)
-        assert np.allclose(convert(cyl.z, APYQuantity), apycyl.z)
+        # There's a 'bug' in Astropy where rho can be negative.
+        with pytest.raises(AssertionError):
+            assert convert(cyl.rho[-1], APYQuantity) == apycyl.rho[-1]
+        assert np.allclose(convert(cyl.rho, APYQuantity), np.abs(apycyl.rho))
 
-        assert np.allclose(convert(cyl.phi[:-1], APYQuantity), apycyl.phi[:-1])
-        # There's a 'bug' in Astropy where at the origin phi is always 90, or at
-        # least doesn't keep its value.
-        with pytest.raises(AssertionError):  # TODO: Fix this
-            assert np.allclose(convert(cyl.phi[-1], APYQuantity), apycyl.phi[-1])
+        assert np.allclose(convert(cyl.z, APYQuantity), apycyl.z)
+        assert np.allclose(convert(cyl.phi, APYQuantity), apycyl.phi)
 
     def test_spherical_to_spherical(self, vector):
         """Test ``coordinax.represent_as(SphericalVector)``."""
         # Jit can copy
         newvec = vector.represent_as(cx.SphericalVector)
         assert newvec == vector
 
@@ -469,22 +468,22 @@
 
         apycart3 = apyvector.represent_as(apyc.SphericalRepresentation)
         assert np.allclose(convert(llsph.distance, APYQuantity), apycart3.distance)
         assert np.allclose(convert(llsph.lon, APYQuantity), apycart3.lon)
         assert np.allclose(convert(llsph.lat, APYQuantity), apycart3.lat)
 
 
-class Abstract3DVectorDifferentialTest(AbstractVectorDifferentialTest):
+class Abstract3DVectorDifferentialTest(AbstractVelocityTest):
     """Test :class:`coordinax.Abstract2DVectorDifferential`."""
 
     # ==========================================================================
     # Unary operations
 
     def test_neg_compare_apy(
-        self, difntl: cx.AbstractVector, apydifntl: apyc.BaseRepresentation
+        self, difntl: cx.AbstractVelocity, apydifntl: apyc.BaseDifferential
     ):
         """Test negation."""
         assert all(representation_equal(convert(-difntl, type(apydifntl)), -apydifntl))
 
 
 class TestCartesianDifferential3D(Abstract3DVectorDifferentialTest):
     """Test :class:`coordinax.CartesianDifferential3D`."""
```

### Comparing `coordinax-0.4.3/tests/test_jax_ops.py` & `coordinax-0.5/tests/test_jax_ops.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,36 +5,38 @@
 import astropy.units as u
 import jax
 import pytest
 
 from unxt import AbstractQuantity, Quantity
 
 import coordinax as cx
-from coordinax._base_vec import VECTOR_CLASSES
+from coordinax._base_pos import VECTOR_CLASSES
 from coordinax._utils import dataclass_items
 
 VECTOR_CLASSES_3D = [c for c in VECTOR_CLASSES if issubclass(c, cx.Abstract3DVector)]
 
 
 # TODO: cycle through all representations
 @pytest.fixture(params=VECTOR_CLASSES_3D)
-def q(request) -> cx.AbstractVector:
+def q(request) -> cx.AbstractPosition:
     """Fixture for 3D Vectors."""
     q = cx.Cartesian3DVector.constructor(Quantity([1, 2, 3], unit=u.kpc))
     return q.represent_as(request.param)
 
 
 @partial(jax.jit, static_argnums=(1,))
-def func(q: cx.AbstractVector, target: type[cx.AbstractVector]) -> cx.AbstractVector:
+def func(
+    q: cx.AbstractPosition, target: type[cx.AbstractPosition]
+) -> cx.AbstractPosition:
     return q.represent_as(target)
 
 
 @pytest.mark.parametrize("target", VECTOR_CLASSES_3D)
 def test_jax_through_representation(
-    q: cx.AbstractVector, target: type[cx.AbstractVector]
+    q: cx.AbstractPosition, target: type[cx.AbstractPosition]
 ) -> None:
     """Test using Jax operations through representation."""
     newq = func(q, target)
 
-    assert isinstance(newq, cx.AbstractVector)
+    assert isinstance(newq, cx.AbstractPosition)
     for k, f in dataclass_items(newq):
         assert isinstance(f, AbstractQuantity), k
```

### Comparing `coordinax-0.4.3/.gitignore` & `coordinax-0.5/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 
 # PyBuilder
 .pybuilder/
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
+notebooks/
 
 # IPython
 profile_default/
 ipython_config.py
 
 # pyenv
 #   For a library or package, you might want to ignore these files since the code is
```

### Comparing `coordinax-0.4.3/README.md` & `coordinax-0.5/README.md`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.3/pyproject.toml` & `coordinax-0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     "astropy",
     "equinox",
     "jax",
     "jaxlib",
     "jaxtyping",
     "plum-dispatch>=2.3.3",
     "quax>=0.0.3",
-    "quaxed >= 0.3",
-    "unxt >= 0.8",
+    "quaxed >= 0.4",
+    "unxt >= 0.10",
   ]
   description = "Vectors in JAX"
   dynamic = ["version"]
   license.file = "LICENSE"
   name = "coordinax"
   readme = "README.md"
   requires-python = ">=3.10"
@@ -194,30 +194,34 @@
       known-first-party = ["quaxed", "unxt"]
       known-local-folder = ["coordinax"]
 
 
 [tool.pylint]
   ignore-paths = [".*/_version.py"]
   messages_control.disable = [
+    "abstract-method",            # pylint doesn't like ABC hierarchies
     "cyclic-import",              # broken?
     "design",
     "duplicate-code",
     "import-outside-toplevel",    # handled by ruff
     "fixme",
     "function-redefined",         # plum-dispatch
     "invalid-name",               # handled by ruff
     "invalid-unary-operand-type", # pylint doesn't understand dataclass fields
+    "isinstance-second-argument-not-valid-type", # pylint doesn't understand _cartesian_cls
     "line-too-long",
     "missing-function-docstring", # TODO: resolve
+    "missing-kwoa",               # plum-dispatch
     "missing-module-docstring",
     "no-member",                  # handled by mypy
     "no-value-for-parameter",     # pylint doesn't understand multiple dispatch
     "not-a-mapping",              # pylint doesn't understand dataclass fields
     "protected-access",           # handled by ruff
     "redefined-builtin",          # handled by ruff
+    "too-many-function-args",     # plum-dispatch
     "unnecessary-ellipsis",       # I like my ellipses in ABCs and Protocols
     "unsubscriptable-object",     # handled by mypy
     "unused-argument",            # handled by ruff
     "wrong-import-position",
     "wrong-import-order",         # handled by ruff
   ]
   py-version = "3.10"
```

### Comparing `coordinax-0.4.3/PKG-INFO` & `coordinax-0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,35 @@
 Metadata-Version: 2.3
 Name: coordinax
-Version: 0.4.3
+Version: 0.5
 Summary: Vectors in JAX
 Project-URL: Bug Tracker, https://github.com/GalacticDynamics/coordinax/issues
 Project-URL: Changelog, https://github.com/GalacticDynamics/coordinax/releases
 Project-URL: Discussions, https://github.com/GalacticDynamics/coordinax/discussions
 Project-URL: Homepage, https://github.com/GalacticDynamics/coordinax
 Author-email: Nathaniel Starkman <nstarman@users.noreply.github.com>
-License: BSD 3-Clause License
+License: Copyright 2024 Galactic Dynamics maintainers
         
-        Copyright (c) 2023, Nathaniel Starkman.
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        * Redistributions of source code must retain the above copyright notice, this
-          list of conditions and the following disclaimer.
-        
-        * Redistributions in binary form must reproduce the above copyright notice,
-          this list of conditions and the following disclaimer in the documentation
-          and/or other materials provided with the distribution.
-        
-        * Neither the name of the coordinax package developers nor the names of its
-          contributors may be used to endorse or promote products derived from
-          this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        Permission is hereby granted, free of charge, to any person obtaining a copy of
+        this software and associated documentation files (the "Software"), to deal in
+        the Software without restriction, including without limitation the rights to
+        use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+        of the Software, and to permit persons to whom the Software is furnished to do
+        so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
 License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -54,22 +44,35 @@
 Requires-Dist: astropy
 Requires-Dist: equinox
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: jaxtyping
 Requires-Dist: plum-dispatch>=2.3.3
 Requires-Dist: quax>=0.0.3
-Requires-Dist: quaxed>=0.3
-Requires-Dist: unxt>=0.8
+Requires-Dist: quaxed>=0.4
+Requires-Dist: unxt>=0.10
 Provides-Extra: all
-Requires-Dist: coordinax[dev]; extra == 'all'
-Requires-Dist: coordinax[docs]; extra == 'all'
-Requires-Dist: coordinax[test]; extra == 'all'
+Requires-Dist: furo>=2023.08.17; extra == 'all'
+Requires-Dist: hypothesis[numpy]; extra == 'all'
+Requires-Dist: myst-parser>=0.13; extra == 'all'
+Requires-Dist: nox; extra == 'all'
+Requires-Dist: pytest-arraydiff; extra == 'all'
+Requires-Dist: pytest-cov>=3; extra == 'all'
+Requires-Dist: pytest>=6; extra == 'all'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'all'
+Requires-Dist: sphinx-copybutton; extra == 'all'
+Requires-Dist: sphinx>=7.0; extra == 'all'
+Requires-Dist: sybil; extra == 'all'
 Provides-Extra: dev
-Requires-Dist: coordinax[test]; extra == 'dev'
+Requires-Dist: hypothesis[numpy]; extra == 'dev'
+Requires-Dist: nox; extra == 'dev'
+Requires-Dist: pytest-arraydiff; extra == 'dev'
+Requires-Dist: pytest-cov>=3; extra == 'dev'
+Requires-Dist: pytest>=6; extra == 'dev'
+Requires-Dist: sybil; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo>=2023.08.17; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx>=7.0; extra == 'docs'
 Provides-Extra: test
```

