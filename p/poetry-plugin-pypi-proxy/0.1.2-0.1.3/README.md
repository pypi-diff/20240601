# Comparing `tmp/poetry_plugin_pypi_proxy-0.1.2.tar.gz` & `tmp/poetry_plugin_pypi_proxy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_pypi_proxy-0.1.2.tar", max compression
+gzip compressed data, was "poetry_plugin_pypi_proxy-0.1.3.tar", max compression
```

## Comparing `poetry_plugin_pypi_proxy-0.1.2.tar` & `poetry_plugin_pypi_proxy-0.1.3.tar`

### file list

```diff
@@ -1,110 +1,119 @@
--rw-r--r--   0        0        0     1070 2022-10-20 17:29:12.217273 poetry_plugin_pypi_proxy-0.1.2/LICENSE
--rw-r--r--   0        0        0     1000 2022-10-20 17:29:12.217417 poetry_plugin_pypi_proxy-0.1.2/README.md
--rw-r--r--   0        0        0     1039 2022-10-20 17:29:42.764134 poetry_plugin_pypi_proxy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-20 17:29:12.218618 poetry_plugin_pypi_proxy-0.1.2/src/poetry_plugin_pypi_proxy/__init__.py
--rw-r--r--   0        0        0     3293 2022-10-20 17:29:12.218819 poetry_plugin_pypi_proxy-0.1.2/src/poetry_plugin_pypi_proxy/plugin.py
--rw-r--r--   0        0        0      696 2022-10-20 17:29:12.219056 poetry_plugin_pypi_proxy-0.1.2/src/poetry_plugin_pypi_proxy/utils.py
--rw-r--r--   0        0        0        0 2022-10-20 17:29:12.219269 poetry_plugin_pypi_proxy-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      470 2022-10-20 17:29:12.219501 poetry_plugin_pypi_proxy-0.1.2/tests/console/test_application.py
--rw-r--r--   0        0        0       22 2022-10-20 17:29:12.219807 poetry_plugin_pypi_proxy-0.1.2/tests/fixtures/sample_project/README.rst
--rw-r--r--   0        0        0     1493 2022-10-20 17:29:12.219940 poetry_plugin_pypi_proxy-0.1.2/tests/fixtures/sample_project/pyproject.toml
--rw-r--r--   0        0        0      731 2022-10-20 17:29:12.220239 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/absolute.html
--rw-r--r--   0        0        0      790 2022-10-20 17:29:12.220369 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/black.html
--rw-r--r--   0        0        0     1455 2022-10-20 17:29:12.220543 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/clikit.html
--rw-r--r--   0        0        0      746 2022-10-20 17:29:12.220734 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/discord-py.html
--rw-r--r--   0        0        0      747 2022-10-20 17:29:12.220862 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/futures.html
--rw-r--r--   0        0        0      759 2022-10-20 17:29:12.220986 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/futures_partial_yank.html
--rw-r--r--   0        0        0      625 2022-10-20 17:29:12.221113 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/invalid-version.html
--rw-r--r--   0        0        0     1433 2022-10-20 17:29:12.221235 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/ipython.html
--rw-r--r--   0        0        0      917 2022-10-20 17:29:12.221352 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/isort.html
--rw-r--r--   0        0        0      333 2022-10-20 17:29:12.221521 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/jupyter.html
--rw-r--r--   0        0        0      348 2022-10-20 17:29:12.221730 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/missing-version.html
--rw-r--r--   0        0        0      401 2022-10-20 17:29:12.221963 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/pastel.html
--rw-r--r--   0        0        0      534 2022-10-20 17:29:12.222174 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html
--rw-r--r--   0        0        0      802 2022-10-20 17:29:12.222377 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/pytest.html
--rw-r--r--   0        0        0      467 2022-10-20 17:29:12.222608 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/python-language-server.html
--rw-r--r--   0        0        0      941 2022-10-20 17:29:12.222808 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/pyyaml.html
--rw-r--r--   0        0        0      687 2022-10-20 17:29:12.223029 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/relative.html
--rw-r--r--   0        0        0      473 2022-10-20 17:29:12.223223 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/tomlkit.html
--rw-r--r--   0        0        0    18499 2022-10-20 17:29:12.223774 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz
--rw-r--r--   0        0        0     9634 2022-10-20 17:29:12.224034 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2
--rw-r--r--   0        0        0     1940 2022-10-20 17:29:12.224254 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl
--rw-r--r--   0        0        0     2822 2022-10-20 17:29:12.224468 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl
--rw-r--r--   0        0        0     2329 2022-10-20 17:29:12.224662 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl
--rw-r--r--   0        0        0     2290 2022-10-20 17:29:12.224857 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl
--rw-r--r--   0        0        0    15847 2022-10-20 17:29:12.225132 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl
--rw-r--r--   0        0        0    18359 2022-10-20 17:29:12.225424 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz
--rw-r--r--   0        0        0    23473 2022-10-20 17:29:12.226367 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl
--rw-r--r--   0        0        0    23475 2022-10-20 17:29:12.226682 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl
--rw-r--r--   0        0        0    15795 2022-10-20 17:29:12.226971 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz
--rw-r--r--   0        0        0    22352 2022-10-20 17:29:12.227270 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl
--rw-r--r--   0        0        0    45393 2022-10-20 17:29:12.227785 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl
--rw-r--r--   0        0        0    45352 2022-10-20 17:29:12.228328 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl
--rw-r--r--   0        0        0    56070 2022-10-20 17:29:12.228820 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz
--rw-r--r--   0        0        0     2736 2022-10-20 17:29:12.229087 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0    12916 2022-10-20 17:29:12.229330 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz
--rw-r--r--   0        0        0     4490 2022-10-20 17:29:12.229571 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz
--rw-r--r--   0        0        0     1213 2022-10-20 17:29:12.229849 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl
--rw-r--r--   0        0        0     1218 2022-10-20 17:29:12.230097 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0    54076 2022-10-20 17:29:12.230450 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz
--rw-r--r--   0        0        0    29813 2022-10-20 17:29:12.230806 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz
--rw-r--r--   0        0        0    29864 2022-10-20 17:29:12.231136 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz
--rw-r--r--   0        0        0     3421 2022-10-20 17:29:12.231827 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json
--rw-r--r--   0        0        0      856 2022-10-20 17:29:12.231474 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/attrs.json
--rw-r--r--   0        0        0    62683 2022-10-20 17:29:12.232755 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json
--rw-r--r--   0        0        0     5924 2022-10-20 17:29:12.233030 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json
--rw-r--r--   0        0        0     1709 2022-10-20 17:29:12.232027 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/black.json
--rw-r--r--   0        0        0     2298 2022-10-20 17:29:12.233592 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json
--rw-r--r--   0        0        0     2425 2022-10-20 17:29:12.233235 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/cachecontrol.json
--rw-r--r--   0        0        0     3745 2022-10-20 17:29:12.234377 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json
--rw-r--r--   0        0        0      997 2022-10-20 17:29:12.233802 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/clikit.json
--rw-r--r--   0        0        0     2922 2022-10-20 17:29:12.234925 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json
--rw-r--r--   0        0        0      867 2022-10-20 17:29:12.234617 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/colorama.json
--rw-r--r--   0        0        0     4035 2022-10-20 17:29:12.235353 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json
--rw-r--r--   0        0        0     2944 2022-10-20 17:29:12.235878 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json
--rw-r--r--   0        0        0      867 2022-10-20 17:29:12.235550 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/funcsigs.json
--rw-r--r--   0        0        0     3838 2022-10-20 17:29:12.236458 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json
--rw-r--r--   0        0        0    14437 2022-10-20 17:29:12.236128 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/hbmqtt.json
--rw-r--r--   0        0        0     5984 2022-10-20 17:29:12.236786 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json
--rw-r--r--   0        0        0    21476 2022-10-20 17:29:12.237301 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json
--rw-r--r--   0        0        0     1221 2022-10-20 17:29:12.236986 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/isort.json
--rw-r--r--   0        0        0     3969 2022-10-20 17:29:12.237928 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json
--rw-r--r--   0        0        0     1217 2022-10-20 17:29:12.237589 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/jupyter.json
--rw-r--r--   0        0        0     2931 2022-10-20 17:29:12.238575 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json
--rw-r--r--   0        0        0      871 2022-10-20 17:29:12.238198 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/lockfile.json
--rw-r--r--   0        0        0     3552 2022-10-20 17:29:12.239108 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json
--rw-r--r--   0        0        0     1284 2022-10-20 17:29:12.238794 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/more-itertools.json
--rw-r--r--   0        0        0     2328 2022-10-20 17:29:12.239728 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json
--rw-r--r--   0        0        0      470 2022-10-20 17:29:12.239338 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pluggy.json
--rw-r--r--   0        0        0     3180 2022-10-20 17:29:12.240300 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json
--rw-r--r--   0        0        0     4561 2022-10-20 17:29:12.240013 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/poetry.json
--rw-r--r--   0        0        0     3095 2022-10-20 17:29:12.240931 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json
--rw-r--r--   0        0        0      837 2022-10-20 17:29:12.240540 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/py.json
--rw-r--r--   0        0        0      931 2022-10-20 17:29:12.241169 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json
--rw-r--r--   0        0        0     4469 2022-10-20 17:29:12.241677 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json
--rw-r--r--   0        0        0      495 2022-10-20 17:29:12.241371 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pylev.json
--rw-r--r--   0        0        0     6933 2022-10-20 17:29:12.242260 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json
--rw-r--r--   0        0        0     7555 2022-10-20 17:29:12.242577 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json
--rw-r--r--   0        0        0      857 2022-10-20 17:29:12.241872 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pytest.json
--rw-r--r--   0        0        0    14143 2022-10-20 17:29:12.243184 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json
--rw-r--r--   0        0        0     7805 2022-10-20 17:29:12.242823 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pyyaml.json
--rw-r--r--   0        0        0     3142 2022-10-20 17:29:12.244468 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json
--rw-r--r--   0        0        0    67409 2022-10-20 17:29:12.243891 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/requests.json
--rw-r--r--   0        0        0     5315 2022-10-20 17:29:12.245041 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json
--rw-r--r--   0        0        0      875 2022-10-20 17:29:12.244719 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/setuptools.json
--rw-r--r--   0        0        0     2387 2022-10-20 17:29:12.246017 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json
--rw-r--r--   0        0        0      846 2022-10-20 17:29:12.245316 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/six.json
--rw-r--r--   0        0        0     8870 2022-10-20 17:29:12.246749 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json
--rw-r--r--   0        0        0      484 2022-10-20 17:29:12.246362 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/sqlalchemy.json
--rw-r--r--   0        0        0     6109 2022-10-20 17:29:12.247106 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/toga.json
--rw-r--r--   0        0        0    11126 2022-10-20 17:29:12.247765 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json
--rw-r--r--   0        0        0     1892 2022-10-20 17:29:12.247381 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/tomlkit.json
--rw-r--r--   0        0        0     3184 2022-10-20 17:29:12.248317 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json
--rw-r--r--   0        0        0      838 2022-10-20 17:29:12.247972 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/trackpy.json
--rw-r--r--   0        0        0    11606 2022-10-20 17:29:12.248902 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json
--rw-r--r--   0        0        0      477 2022-10-20 17:29:12.248525 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/twisted.json
--rw-r--r--   0        0        0   224197 2022-10-20 17:29:12.250040 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/search/search.html
--rw-r--r--   0        0        0     1376 2022-10-20 17:29:12.250456 poetry_plugin_pypi_proxy-0.1.2/tests/repositories/test_legacy_proxy_repository.py
--rw-r--r--   0        0        0      565 2022-10-20 17:29:12.250689 poetry_plugin_pypi_proxy-0.1.2/tests/test_utils.py
--rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 poetry_plugin_pypi_proxy-0.1.2/setup.py
--rw-r--r--   0        0        0     1681 1970-01-01 00:00:00.000000 poetry_plugin_pypi_proxy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-10-07 19:05:31.914551 poetry_plugin_pypi_proxy-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1000 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/README.md
+-rw-r--r--   0        0        0     1144 2023-01-03 19:13:53.228064 poetry_plugin_pypi_proxy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/src/poetry_plugin_pypi_proxy/__init__.py
+-rw-r--r--   0        0        0     3914 2022-12-21 03:12:57.515380 poetry_plugin_pypi_proxy-0.1.3/src/poetry_plugin_pypi_proxy/plugin.py
+-rw-r--r--   0        0        0     3033 2022-12-21 03:12:57.515380 poetry_plugin_pypi_proxy-0.1.3/src/poetry_plugin_pypi_proxy/utils.py
+-rw-r--r--   0        0        0        0 2022-10-07 19:05:31.910551 poetry_plugin_pypi_proxy-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      470 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/console/test_application.py
+-rw-r--r--   0        0        0      143 2022-12-21 03:12:57.515380 poetry_plugin_pypi_proxy-0.1.3/tests/e2e/sample-dependency/setup.py
+-rw-r--r--   0        0        0       13 2022-12-21 03:12:57.515380 poetry_plugin_pypi_proxy-0.1.3/tests/e2e/sample-project/README.md
+-rw-r--r--   0        0        0     1183 2022-12-21 03:12:57.515380 poetry_plugin_pypi_proxy-0.1.3/tests/e2e/sample-project/dist/sample_project-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     1035 2022-12-21 03:12:57.515380 poetry_plugin_pypi_proxy-0.1.3/tests/e2e/sample-project/dist/sample_project-0.1.0.tar.gz
+-rw-r--r--   0        0        0      508 2022-12-21 03:12:57.515380 poetry_plugin_pypi_proxy-0.1.3/tests/e2e/sample-project/poetry.lock
+-rw-r--r--   0        0        0       32 2022-12-21 03:12:57.515380 poetry_plugin_pypi_proxy-0.1.3/tests/e2e/sample-project/poetry.toml
+-rw-r--r--   0        0        0      372 2022-12-21 03:12:57.519380 poetry_plugin_pypi_proxy-0.1.3/tests/e2e/sample-project/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-21 03:12:57.519380 poetry_plugin_pypi_proxy-0.1.3/tests/e2e/sample-project/sample_project/__init__.py
+-rw-r--r--   0        0        0     7977 2022-12-21 03:12:57.519380 poetry_plugin_pypi_proxy-0.1.3/tests/e2e/test_e2e.py
+-rw-r--r--   0        0        0       22 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/fixtures/sample_project/README.rst
+-rw-r--r--   0        0        0     1493 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/fixtures/sample_project/pyproject.toml
+-rw-r--r--   0        0        0      731 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/absolute.html
+-rw-r--r--   0        0        0      790 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/black.html
+-rw-r--r--   0        0        0     1455 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/clikit.html
+-rw-r--r--   0        0        0      746 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/discord-py.html
+-rw-r--r--   0        0        0      747 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/futures.html
+-rw-r--r--   0        0        0      759 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/futures_partial_yank.html
+-rw-r--r--   0        0        0      625 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/invalid-version.html
+-rw-r--r--   0        0        0     1433 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/ipython.html
+-rw-r--r--   0        0        0      917 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/isort.html
+-rw-r--r--   0        0        0      333 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/jupyter.html
+-rw-r--r--   0        0        0      348 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/missing-version.html
+-rw-r--r--   0        0        0      401 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/pastel.html
+-rw-r--r--   0        0        0      534 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html
+-rw-r--r--   0        0        0      802 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/pytest.html
+-rw-r--r--   0        0        0      467 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/python-language-server.html
+-rw-r--r--   0        0        0      941 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/pyyaml.html
+-rw-r--r--   0        0        0      687 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/relative.html
+-rw-r--r--   0        0        0      473 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/tomlkit.html
+-rw-r--r--   0        0        0    18499 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz
+-rw-r--r--   0        0        0     9634 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2
+-rw-r--r--   0        0        0     1940 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl
+-rw-r--r--   0        0        0     2822 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl
+-rw-r--r--   0        0        0     2329 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     2290 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0    15847 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl
+-rw-r--r--   0        0        0    18359 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz
+-rw-r--r--   0        0        0    23473 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl
+-rw-r--r--   0        0        0    23475 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0    15795 2022-10-12 13:06:00.655207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz
+-rw-r--r--   0        0        0    22352 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl
+-rw-r--r--   0        0        0    45393 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl
+-rw-r--r--   0        0        0    45352 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl
+-rw-r--r--   0        0        0    56070 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz
+-rw-r--r--   0        0        0     2736 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    12916 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz
+-rw-r--r--   0        0        0     4490 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz
+-rw-r--r--   0        0        0     1213 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl
+-rw-r--r--   0        0        0     1218 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0    54076 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz
+-rw-r--r--   0        0        0    29813 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz
+-rw-r--r--   0        0        0    29864 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz
+-rw-r--r--   0        0        0     3421 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json
+-rw-r--r--   0        0        0      856 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/attrs.json
+-rw-r--r--   0        0        0    62683 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json
+-rw-r--r--   0        0        0     5924 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json
+-rw-r--r--   0        0        0     1709 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/black.json
+-rw-r--r--   0        0        0     2298 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json
+-rw-r--r--   0        0        0     2425 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/cachecontrol.json
+-rw-r--r--   0        0        0     3745 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json
+-rw-r--r--   0        0        0      997 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/clikit.json
+-rw-r--r--   0        0        0     2922 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json
+-rw-r--r--   0        0        0      867 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/colorama.json
+-rw-r--r--   0        0        0     4035 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json
+-rw-r--r--   0        0        0     2944 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json
+-rw-r--r--   0        0        0      867 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/funcsigs.json
+-rw-r--r--   0        0        0     3838 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json
+-rw-r--r--   0        0        0    14437 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/hbmqtt.json
+-rw-r--r--   0        0        0     5984 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json
+-rw-r--r--   0        0        0    21476 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json
+-rw-r--r--   0        0        0     1221 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/isort.json
+-rw-r--r--   0        0        0     3969 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json
+-rw-r--r--   0        0        0     1217 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/jupyter.json
+-rw-r--r--   0        0        0     2931 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json
+-rw-r--r--   0        0        0      871 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/lockfile.json
+-rw-r--r--   0        0        0     3552 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json
+-rw-r--r--   0        0        0     1284 2022-10-12 13:06:00.659207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/more-itertools.json
+-rw-r--r--   0        0        0     2328 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json
+-rw-r--r--   0        0        0      470 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pluggy.json
+-rw-r--r--   0        0        0     3180 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json
+-rw-r--r--   0        0        0     4561 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/poetry.json
+-rw-r--r--   0        0        0     3095 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json
+-rw-r--r--   0        0        0      837 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/py.json
+-rw-r--r--   0        0        0      931 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json
+-rw-r--r--   0        0        0     4469 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json
+-rw-r--r--   0        0        0      495 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pylev.json
+-rw-r--r--   0        0        0     6933 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json
+-rw-r--r--   0        0        0     7555 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json
+-rw-r--r--   0        0        0      857 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pytest.json
+-rw-r--r--   0        0        0    14143 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json
+-rw-r--r--   0        0        0     7805 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pyyaml.json
+-rw-r--r--   0        0        0     3142 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json
+-rw-r--r--   0        0        0    67409 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/requests.json
+-rw-r--r--   0        0        0     5315 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json
+-rw-r--r--   0        0        0      875 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/setuptools.json
+-rw-r--r--   0        0        0     2387 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json
+-rw-r--r--   0        0        0      846 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/six.json
+-rw-r--r--   0        0        0     8870 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json
+-rw-r--r--   0        0        0      484 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/sqlalchemy.json
+-rw-r--r--   0        0        0     6109 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/toga.json
+-rw-r--r--   0        0        0    11126 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json
+-rw-r--r--   0        0        0     1892 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/tomlkit.json
+-rw-r--r--   0        0        0     3184 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json
+-rw-r--r--   0        0        0      838 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/trackpy.json
+-rw-r--r--   0        0        0    11606 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json
+-rw-r--r--   0        0        0      477 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/twisted.json
+-rw-r--r--   0        0        0   224197 2022-10-12 13:06:00.663207 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/search/search.html
+-rw-r--r--   0        0        0     1380 2022-12-21 03:12:57.519380 poetry_plugin_pypi_proxy-0.1.3/tests/repositories/test_legacy_proxy_repository.py
+-rw-r--r--   0        0        0     2104 2022-12-21 03:12:57.519380 poetry_plugin_pypi_proxy-0.1.3/tests/test_utils.py
+-rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 poetry_plugin_pypi_proxy-0.1.3/setup.py
+-rw-r--r--   0        0        0     1681 1970-01-01 00:00:00.000000 poetry_plugin_pypi_proxy-0.1.3/PKG-INFO
```

### Comparing `poetry_plugin_pypi_proxy-0.1.2/LICENSE` & `poetry_plugin_pypi_proxy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/README.md` & `poetry_plugin_pypi_proxy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/pyproject.toml` & `poetry_plugin_pypi_proxy-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-pypi-proxy"
-version = "0.1.2"
+version = "0.1.3"
 description = "Aliases PIP_INDEX_URL silently within Poetry to point at a new repository."
 authors = ["Chad Crawford <chad@cacrawford.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "poetry_plugin_pypi_proxy", from = "src" }
 ]
@@ -12,29 +12,36 @@
     { path = "tests", format = "sdist" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 poetry = "^1.2.0"
 
+
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.3"
+pytest-mock = "^3.10.0"
+wheel = "^0.38.4"
+pytest-httpserver = "^1.0.6"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^0.982"
+types-setuptools = "^65.6.0.2"
+
 
 [tool.isort]
 py_version = 37
 profile = "black"
 
 [tool.black]
-target-version = ['py37']
+target-version = ["py37"]
 preview = true
 
 [tool.mypy]
 files = ["src", "tests"]
 
 [[tool.mypy.overrides]]
 module = [
```

### Comparing `poetry_plugin_pypi_proxy-0.1.2/src/poetry_plugin_pypi_proxy/plugin.py` & `poetry_plugin_pypi_proxy-0.1.3/src/poetry_plugin_pypi_proxy/plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,20 +2,24 @@
 
 import copy
 import os
 
 from cleo.io.io import IO
 from cleo.io.outputs.output import Verbosity
 from poetry.core.packages.package import Package
-from poetry.core.semver.version import Version
 from poetry.plugins.plugin import Plugin
 from poetry.poetry import Poetry
 from poetry.repositories.legacy_repository import LegacyRepository
 
-from poetry_plugin_pypi_proxy.utils import get_repo_id, parse_url
+from poetry_plugin_pypi_proxy.utils import (
+    POETRY_VERSION,
+    Version,
+    generate_poetry_auth_config,
+    get_repo_id,
+)
 
 
 class LegacyProxyRepository(LegacyRepository):
     """
     Alternative repository that strips URL information from packages.
 
     Mainly used to ensure the lockfile looks as if it were pulled
@@ -62,41 +66,53 @@
             io.write_line(
                 "No PIP_INDEX_URL set, so no Pypi proxy will be configured.",
                 verbosity=Verbosity.VERBOSE,
             )
             return
 
         # Parse the proper for PIP_INDEX_URL but not for publishing.
-        proxy_url = parse_url(proxy_url)
+        auth_config = generate_poetry_auth_config(proxy_url)
+        proxy_url = auth_config.url
 
         # Add debug message so that users are certain the substitution happens
         io.write_line(
             f"Disabling Pypi and substituting with proxy server at {proxy_url}.",
             verbosity=Verbosity.VERBOSE,
         )
 
         # Generate unique string for project root
         proxy_id = get_repo_id(proxy_url)
 
+        # Create entries in the config for the repo and Auth if we have it
+        poetry.config._config["repositories"] = {proxy_id: {"url": auth_config.url}}
+        if auth_config.http_auth is not None:
+            poetry.config._config["http-basic"] = poetry.config._config.get(
+                "http-basic", {}
+            )
+            poetry.config._config["http-basic"][proxy_id] = {
+                "username": auth_config.http_auth.username,
+                "password": auth_config.http_auth.password,
+            }
+
         # Set up the proxy as the default, remove
         poetry.pool._default = False
-        poetry.pool.remove_repository("pypi")
+        if poetry.pool.has_repository("pypi"):
+            poetry.pool.remove_repository("pypi")
 
         # resolve bug in old Poetry
-        if "pypi" in poetry.pool._lookup:
-            del poetry.pool._lookup["pypi"]
+        if POETRY_VERSION < (1, 2, 1):
+            if "pypi" in poetry.pool._lookup:
+                del poetry.pool._lookup["pypi"]
 
         # Add default repository
         poetry.pool.add_repository(
             LegacyProxyRepository(
-                name=proxy_id,
-                url=f"{proxy_url}simple/",
+                name=proxy_id, url=f"{proxy_url}/simple/", config=poetry.config
             ),
             default=True,
         )
 
         # If this is a publish command to Pypi, we'll silenly redirect to the proxy
         if io.input.arguments["command"] == "publish" and not io.input.option(
             "repository"
         ):
             io.input.set_option("repository", proxy_id)
-            poetry.config._config["repositories"] = {proxy_id: {"url": proxy_url}}
```

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/fixtures/sample_project/pyproject.toml` & `poetry_plugin_pypi_proxy-0.1.3/tests/fixtures/sample_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/absolute.html` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/absolute.html`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/black.html` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/black.html`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/clikit.html` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/clikit.html`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/discord-py.html` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/discord-py.html`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/futures.html` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/futures.html`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/futures_partial_yank.html` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/futures_partial_yank.html`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/invalid-version.html` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/invalid-version.html`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/ipython.html` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/ipython.html`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/isort.html` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/isort.html`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/poetry-test-py2-py3-metadata-merge.html`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/pytest.html` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/pytest.html`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/pyyaml.html` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/pyyaml.html`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/legacy/relative.html` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/legacy/relative.html`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/SQLAlchemy-1.2.12.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/Twisted-18.9.0.tar.bz2`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/black-19.10b0-py36-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/black-21.11b0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/clikit-0.2.4-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/discord.py-2.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/futures-3.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/ipython-5.7.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/ipython-7.5.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/isort-4.3.4.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/jupyter-1.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/pastel-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/poetry_test_py2_py3_metadata_merge-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/python-language-server-0.21.2.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.2.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/dists/tomlkit-0.5.3.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/attrs/17.4.0.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/attrs.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/attrs.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/black/19.10b0.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/black/21.11b0.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/black.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/black.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/cachecontrol/0.12.5.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/cachecontrol.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/cachecontrol.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/clikit/0.2.4.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/clikit.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/clikit.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/colorama/0.3.9.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/colorama.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/colorama.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/discord-py/2.0.0.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/funcsigs/1.0.2.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/funcsigs.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/funcsigs.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/hbmqtt/0.9.6.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/hbmqtt.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/hbmqtt.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/ipython/4.1.0rc1.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/isort/4.3.4.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/isort.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/isort.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/jupyter/1.0.0.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/jupyter.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/jupyter.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/lockfile/0.12.2.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/lockfile.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/lockfile.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/more-itertools/4.1.0.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/more-itertools.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/more-itertools.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pluggy/0.6.0.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/poetry/0.12.4.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/poetry.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/poetry.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/py/1.5.3.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/py.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/py.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pygame-music-grid.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pylev/1.3.0.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pytest/3.5.0.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pytest/3.5.1.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pytest.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pytest.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pyyaml/3.13.0.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/pyyaml.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/pyyaml.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/requests/2.18.4.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/requests.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/requests.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/setuptools/39.2.0.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/setuptools.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/setuptools.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/six/1.11.0.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/six.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/six.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/sqlalchemy/1.2.12.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/toga.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/toga.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/tomlkit/0.5.3.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/tomlkit.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/tomlkit.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/trackpy/0.4.1.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/trackpy.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/trackpy.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/json/twisted/18.9.0.json`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/fixtures/pypi.org/search/search.html` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/fixtures/pypi.org/search/search.html`

 * *Files identical despite different names*

### Comparing `poetry_plugin_pypi_proxy-0.1.2/tests/repositories/test_legacy_proxy_repository.py` & `poetry_plugin_pypi_proxy-0.1.3/tests/repositories/test_legacy_proxy_repository.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import shutil
 import urllib.parse as urlparse
 from pathlib import Path
 
-from poetry.core.semver.version import Version
 from poetry.repositories.link_sources.html import SimpleRepositoryPage
 
 from poetry_plugin_pypi_proxy.plugin import LegacyProxyRepository
+from poetry_plugin_pypi_proxy.utils import Version
 
 
 class MockRepository(LegacyProxyRepository):
     FIXTURES = Path(__file__).parent / "fixtures" / "legacy"
 
     def __init__(self) -> None:
         super().__init__("proxy", url="http://legacy.foo.bar", disable_cache=True)
```

### Comparing `poetry_plugin_pypi_proxy-0.1.2/setup.py` & `poetry_plugin_pypi_proxy-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 entry_points = \
 {'poetry.plugin': ['poetry-pypi-proxy = '
                    'poetry_plugin_pypi_proxy.plugin:PypiProxyPlugin']}
 
 setup_kwargs = {
     'name': 'poetry-plugin-pypi-proxy',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Aliases PIP_INDEX_URL silently within Poetry to point at a new repository.',
     'long_description': '# poetry-plugin-pypi-proxy\n\nThis is a plugin that enables developers who use internal proxies of\nPypi to integrate their projects seamlessly with Poetry without\nneeding to build custom configurations for their proxy server.\n\nThe plugin operates intuitively -- users can onboard to this tooling\nby installing the plugin and then setting `PIP_INDEX_URL` before\nrunning Poetry commands.\n\nIt also runs silently, i.e., it will not pollute your `poetry.lock`\nwith the URL of your proxy server and `poetry publish` is\nautomatically redirected to the proxy as well.\n\n## Usage\n\nStart by installing Poetry with pipx:\n\n    pipx install poetry\n    pipx runpip poetry install poetry-plugin-pypi-proxy\n\nIf you have already installed poetry, you only need to run the second command.\n\nNow, any Poetry project will automatically use the proxy server\nspecified by `PIP_INDEX_URL`. You may add this to your `rc` file\n(`.bashrc`, `.zshrc`, `.envrc` with direnv, etc) or simply export it\nin your terminal to get started.\n',
     'author': 'Chad Crawford',
     'author_email': 'chad@cacrawford.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `poetry_plugin_pypi_proxy-0.1.2/PKG-INFO` & `poetry_plugin_pypi_proxy-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-pypi-proxy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Aliases PIP_INDEX_URL silently within Poetry to point at a new repository.
 License: MIT
 Author: Chad Crawford
 Author-email: chad@cacrawford.org
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

