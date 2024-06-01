# Comparing `tmp/omniduct-1.2.1.tar.gz` & `tmp/omniduct-1.2.2.tar.gz`

## Comparing `omniduct-1.2.1.tar` & `omniduct-1.2.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 omniduct-1.2.1/MANIFEST.in
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/Makefile
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/conf.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/contributions.rst
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/deployment.rst
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/extensions.rst
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/index.rst
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/installation.rst
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/make.bat
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/protocols.rst
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/python_deps.txt
--rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/quickstart.rst
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/core.rst
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/overview.rst
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/registry.rst
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/caches/overview.rst
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/caches/reference/filesystem.rst
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/databases/overview.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/databases/reference/druid.rst
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/databases/reference/hiveserver2.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/databases/reference/neo4j.rst
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/databases/reference/presto.rst
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/databases/reference/pyspark.rst
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/databases/reference/sqlalchemy.rst
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/filesystems/overview.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/filesystems/reference/local.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/filesystems/reference/s3.rst
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/filesystems/reference/webhdfs.rst
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/remotes/overview.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/remotes/reference/ssh.rst
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/remotes/reference/ssh_paramiko.rst
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 omniduct-1.2.1/example_wrapper/MANIFEST.in
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 omniduct-1.2.1/example_wrapper/README.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 omniduct-1.2.1/example_wrapper/setup.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 omniduct-1.2.1/example_wrapper/example_wrapper/__init__.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 omniduct-1.2.1/example_wrapper/example_wrapper/_version.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 omniduct-1.2.1/example_wrapper/example_wrapper/services.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 omniduct-1.2.1/example_wrapper/example_wrapper/services.yml
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/__init__.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/_version.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/_version_info.py
--rw-r--r--   0        0        0    23348 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/duct.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/errors.py
--rw-r--r--   0        0        0    21834 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/logo.png
--rw-r--r--   0        0        0    53763 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/logo.svg
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/protocols.py
--rw-r--r--   0        0        0    12051 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/caches/__init__.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/caches/_serializers.py
--rw-r--r--   0        0        0    20694 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/caches/base.py
--rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/caches/filesystem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/__init__.py
--rw-r--r--   0        0        0     7224 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/_cursor_formatters.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/_cursor_serializer.py
--rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/_namespaces.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/_pandas.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/_schemas.py
--rw-r--r--   0        0        0    41077 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/base.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/druid.py
--rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/exasol.py
--rw-r--r--   0        0        0    24756 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/hiveserver2.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/neo4j.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/presto.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/pyspark.py
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/sqlalchemy.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/stub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/__init__.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/_pyarrow_compat.py
--rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/_webhdfs_helpers.py
--rw-r--r--   0        0        0    35915 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/base.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/local.py
--rw-r--r--   0        0        0    10569 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/s3.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/stub.py
--rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/webhdfs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/remotes/__init__.py
--rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/remotes/base.py
--rw-r--r--   0        0        0    21990 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/remotes/ssh.py
--rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/remotes/ssh_paramiko.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/remotes/stub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/restful/__init__.py
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/restful/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/__init__.py
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/about.py
--rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/config.py
--rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/debug.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/decorators.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/dependencies.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/magics.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/ports.py
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/processes.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/proxies.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/storage.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/submodules.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/tests/__init__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 omniduct-1.2.1/tests/test_restful.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/tests/databases/__init__.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 omniduct-1.2.1/tests/databases/test__namespaces.py
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 omniduct-1.2.1/tests/databases/test_base.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omniduct-1.2.1/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 omniduct-1.2.1/LICENSE
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 omniduct-1.2.1/README.md
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 omniduct-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 omniduct-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 omniduct-1.2.2/MANIFEST.in
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/Makefile
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/conf.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/contributions.rst
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/deployment.rst
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/extensions.rst
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/index.rst
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/installation.rst
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/make.bat
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/protocols.rst
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/python_deps.txt
+-rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/quickstart.rst
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/core.rst
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/overview.rst
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/registry.rst
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/caches/overview.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/caches/reference/filesystem.rst
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/databases/overview.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/databases/reference/druid.rst
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/databases/reference/hiveserver2.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/databases/reference/neo4j.rst
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/databases/reference/presto.rst
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/databases/reference/pyspark.rst
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/databases/reference/sqlalchemy.rst
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/filesystems/overview.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/filesystems/reference/local.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/filesystems/reference/s3.rst
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/filesystems/reference/webhdfs.rst
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/remotes/overview.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/remotes/reference/ssh.rst
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 omniduct-1.2.2/docs/api/remotes/reference/ssh_paramiko.rst
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 omniduct-1.2.2/example_wrapper/MANIFEST.in
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 omniduct-1.2.2/example_wrapper/README.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 omniduct-1.2.2/example_wrapper/setup.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 omniduct-1.2.2/example_wrapper/example_wrapper/__init__.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 omniduct-1.2.2/example_wrapper/example_wrapper/_version.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 omniduct-1.2.2/example_wrapper/example_wrapper/services.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 omniduct-1.2.2/example_wrapper/example_wrapper/services.yml
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/__init__.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/_version.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/_version_info.py
+-rw-r--r--   0        0        0    23348 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/duct.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/errors.py
+-rw-r--r--   0        0        0    21834 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/logo.png
+-rw-r--r--   0        0        0    53763 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/logo.svg
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/protocols.py
+-rw-r--r--   0        0        0    12051 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/caches/__init__.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/caches/_serializers.py
+-rw-r--r--   0        0        0    20694 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/caches/base.py
+-rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/caches/filesystem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/databases/__init__.py
+-rw-r--r--   0        0        0     7224 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/databases/_cursor_formatters.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/databases/_cursor_serializer.py
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/databases/_namespaces.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/databases/_pandas.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/databases/_schemas.py
+-rw-r--r--   0        0        0    41077 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/databases/base.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/databases/druid.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/databases/exasol.py
+-rw-r--r--   0        0        0    24756 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/databases/hiveserver2.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/databases/neo4j.py
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/databases/presto.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/databases/pyspark.py
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/databases/sqlalchemy.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/databases/stub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/filesystems/__init__.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/filesystems/_pyarrow_compat.py
+-rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/filesystems/_webhdfs_helpers.py
+-rw-r--r--   0        0        0    35915 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/filesystems/base.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/filesystems/local.py
+-rw-r--r--   0        0        0    10569 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/filesystems/s3.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/filesystems/stub.py
+-rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/filesystems/webhdfs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/remotes/__init__.py
+-rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/remotes/base.py
+-rw-r--r--   0        0        0    21990 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/remotes/ssh.py
+-rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/remotes/ssh_paramiko.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/remotes/stub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/restful/__init__.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/restful/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/utils/__init__.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/utils/about.py
+-rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/utils/config.py
+-rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/utils/debug.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/utils/decorators.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/utils/dependencies.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/utils/magics.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/utils/ports.py
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/utils/processes.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/utils/proxies.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/utils/storage.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 omniduct-1.2.2/omniduct/utils/submodules.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 omniduct-1.2.2/tests/test_restful.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.2/tests/databases/__init__.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 omniduct-1.2.2/tests/databases/test__namespaces.py
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 omniduct-1.2.2/tests/databases/test_base.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omniduct-1.2.2/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 omniduct-1.2.2/LICENSE
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 omniduct-1.2.2/README.md
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 omniduct-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 omniduct-1.2.2/PKG-INFO
```

### Comparing `omniduct-1.2.1/docs/Makefile` & `omniduct-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/docs/conf.py` & `omniduct-1.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/docs/deployment.rst` & `omniduct-1.2.2/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/docs/extensions.rst` & `omniduct-1.2.2/docs/extensions.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/docs/index.rst` & `omniduct-1.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/docs/installation.rst` & `omniduct-1.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/docs/make.bat` & `omniduct-1.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/docs/protocols.rst` & `omniduct-1.2.2/docs/protocols.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/docs/quickstart.rst` & `omniduct-1.2.2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/docs/api/core.rst` & `omniduct-1.2.2/docs/api/core.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/docs/api/overview.rst` & `omniduct-1.2.2/docs/api/overview.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/docs/api/caches/overview.rst` & `omniduct-1.2.2/docs/api/caches/overview.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/docs/api/databases/overview.rst` & `omniduct-1.2.2/docs/api/databases/overview.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/docs/api/filesystems/overview.rst` & `omniduct-1.2.2/docs/api/filesystems/overview.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/docs/api/remotes/overview.rst` & `omniduct-1.2.2/docs/api/remotes/overview.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/example_wrapper/README.md` & `omniduct-1.2.2/example_wrapper/README.md`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/example_wrapper/setup.py` & `omniduct-1.2.2/example_wrapper/setup.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/example_wrapper/example_wrapper/__init__.py` & `omniduct-1.2.2/example_wrapper/example_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/example_wrapper/example_wrapper/services.py` & `omniduct-1.2.2/example_wrapper/example_wrapper/services.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/example_wrapper/example_wrapper/services.yml` & `omniduct-1.2.2/example_wrapper/example_wrapper/services.yml`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/__init__.py` & `omniduct-1.2.2/omniduct/__init__.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/_version.py` & `omniduct-1.2.2/omniduct/_version.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/duct.py` & `omniduct-1.2.2/omniduct/duct.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/logo.png` & `omniduct-1.2.2/omniduct/logo.png`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/logo.svg` & `omniduct-1.2.2/omniduct/logo.svg`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/protocols.py` & `omniduct-1.2.2/omniduct/protocols.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/registry.py` & `omniduct-1.2.2/omniduct/registry.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/caches/_serializers.py` & `omniduct-1.2.2/omniduct/caches/_serializers.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/caches/base.py` & `omniduct-1.2.2/omniduct/caches/base.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/caches/filesystem.py` & `omniduct-1.2.2/omniduct/caches/filesystem.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/databases/_cursor_formatters.py` & `omniduct-1.2.2/omniduct/databases/_cursor_formatters.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/databases/_cursor_serializer.py` & `omniduct-1.2.2/omniduct/databases/_cursor_serializer.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/databases/_namespaces.py` & `omniduct-1.2.2/omniduct/databases/_namespaces.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/databases/_pandas.py` & `omniduct-1.2.2/omniduct/databases/_pandas.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/databases/_schemas.py` & `omniduct-1.2.2/omniduct/databases/_schemas.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/databases/base.py` & `omniduct-1.2.2/omniduct/databases/base.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/databases/druid.py` & `omniduct-1.2.2/omniduct/databases/druid.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/databases/exasol.py` & `omniduct-1.2.2/omniduct/databases/exasol.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/databases/hiveserver2.py` & `omniduct-1.2.2/omniduct/databases/hiveserver2.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/databases/neo4j.py` & `omniduct-1.2.2/omniduct/databases/neo4j.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/databases/presto.py` & `omniduct-1.2.2/omniduct/databases/presto.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,15 +72,14 @@
             Passed through to the pyhive Cursor which supports custom requests sessions for advanced usage
             such as custom headers, cookie values, retry logic, etc.
         """
         self.catalog = catalog
         self.schema = schema
         self.server_protocol = server_protocol
         self.source = source
-        self.__presto = None
         self.connection_fields += ("catalog", "schema")
         self._requests_session = requests_session
 
     @property
     def source(self):
         return self._source
 
@@ -99,26 +98,19 @@
         self._sqlalchemy_engine = create_engine(
             f"presto://{self.host}:{self.port}/{self.catalog}/{self.schema}"
         )
         self._sqlalchemy_metadata = MetaData(self._sqlalchemy_engine)
 
     @override
     def _is_connected(self):
-        try:
-            return self.__presto is not None
-        except:  # pylint: disable=bare-except
-            return False
+        return True
 
     @override
     def _disconnect(self):
         logger.info("Disconnecting from Presto coordinator...")
-        try:
-            self.__presto.close()
-        except:  # pylint: disable=bare-except
-            pass
         self._sqlalchemy_engine = None
         self._sqlalchemy_metadata = None
         self._schemas = None  # pylint: disable=attribute-defined-outside-init
 
     # Querying
     @override
     def _execute(self, statement, cursor, wait, session_properties):
@@ -158,18 +150,14 @@
                             4,
                         )
                         logger.progress(pct_complete * 100)
                     status = cursor.poll()
                 logger.progress(100, complete=True)
             return cursor
         except (DatabaseError, pandas.io.sql.DatabaseError) as e:
-            # Attempt to parse database error, before ultimately reraising the same
-            # exception, maintaining the full stacktrace.
-            exception, exception_args, traceback = sys.exc_info()
-
             try:
                 message = e.args[0]
                 if isinstance(message, str):
                     message = ast.literal_eval(
                         re.match("[^{]*({.*})[^}]*$", message).group(1)
                     )
 
@@ -187,49 +175,49 @@
                             for ln in range(
                                 max(linenumber - 1, 0), min(linenumber + 2, len(splt))
                             )
                         ]
                     )
                 )
 
-                class ErrContext:
-                    def __repr__(self):
-                        return context
-
-                # logged twice so that both notebook and console users see the error context
-                exception_args.args = [exception_args, ErrContext()]
                 logger.error(context)
             except:  # pylint: disable=bare-except
                 logger.warn(
                     (
                         "Omniduct was unable to parse the database error messages. Refer to the "
                         "traceback below for full error details."
                     )
                 )
 
-            if isinstance(exception, type):
-                exception = exception(exception_args)
-
-            raise exception.with_traceback(traceback)
+            raise
 
     @override
     def _query_to_table(self, statement, table, if_exists, **kwargs):
+        from pyhive.exc import DatabaseError
+
         statements = []
 
-        if if_exists == "fail" and self.table_exists(table):
-            raise RuntimeError(f"Table {table} already exists!")
         if if_exists == "replace":
             statements.append(f"DROP TABLE IF EXISTS {table};\n")
         elif if_exists == "append":
             raise NotImplementedError(
                 f"Append operations have not been implemented for {self.__class__.__name__}."
             )
 
         statements.append(f"CREATE TABLE {table} AS ({statement})")
-        return self.execute("\n".join(statements), **kwargs)
+
+        try:
+            return self.execute("\n".join(statements), **kwargs)
+        except DatabaseError as e:
+            if (
+                isinstance(e.args, dict)
+                and e.args.get("errorName") == "TABLE_ALREADY_EXISTS"
+            ):
+                raise RuntimeError(f"Table {table} already exists!") from e
+            raise
 
     @override
     def _dataframe_to_table(self, df, table, if_exists="fail", **kwargs):
         """
         If if the schema namespace is not specified, `table.schema` will be
         defaulted to your username. Catalog overrides will be ignored, and will
         default to `self.catalog`.
```

### Comparing `omniduct-1.2.1/omniduct/databases/pyspark.py` & `omniduct-1.2.2/omniduct/databases/pyspark.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/databases/sqlalchemy.py` & `omniduct-1.2.2/omniduct/databases/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/databases/stub.py` & `omniduct-1.2.2/omniduct/databases/stub.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/filesystems/_pyarrow_compat.py` & `omniduct-1.2.2/omniduct/filesystems/_pyarrow_compat.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/filesystems/_webhdfs_helpers.py` & `omniduct-1.2.2/omniduct/filesystems/_webhdfs_helpers.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/filesystems/base.py` & `omniduct-1.2.2/omniduct/filesystems/base.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/filesystems/local.py` & `omniduct-1.2.2/omniduct/filesystems/local.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/filesystems/s3.py` & `omniduct-1.2.2/omniduct/filesystems/s3.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/filesystems/stub.py` & `omniduct-1.2.2/omniduct/filesystems/stub.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/filesystems/webhdfs.py` & `omniduct-1.2.2/omniduct/filesystems/webhdfs.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/remotes/base.py` & `omniduct-1.2.2/omniduct/remotes/base.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/remotes/ssh.py` & `omniduct-1.2.2/omniduct/remotes/ssh.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/remotes/ssh_paramiko.py` & `omniduct-1.2.2/omniduct/remotes/ssh_paramiko.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/remotes/stub.py` & `omniduct-1.2.2/omniduct/remotes/stub.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/restful/base.py` & `omniduct-1.2.2/omniduct/restful/base.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/utils/about.py` & `omniduct-1.2.2/omniduct/utils/about.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/utils/config.py` & `omniduct-1.2.2/omniduct/utils/config.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/utils/debug.py` & `omniduct-1.2.2/omniduct/utils/debug.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/utils/decorators.py` & `omniduct-1.2.2/omniduct/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/utils/dependencies.py` & `omniduct-1.2.2/omniduct/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/utils/magics.py` & `omniduct-1.2.2/omniduct/utils/magics.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/utils/ports.py` & `omniduct-1.2.2/omniduct/utils/ports.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/utils/processes.py` & `omniduct-1.2.2/omniduct/utils/processes.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/omniduct/utils/proxies.py` & `omniduct-1.2.2/omniduct/utils/proxies.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/tests/databases/test__namespaces.py` & `omniduct-1.2.2/tests/databases/test__namespaces.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/tests/databases/test_base.py` & `omniduct-1.2.2/tests/databases/test_base.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/.gitignore` & `omniduct-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/LICENSE` & `omniduct-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/README.md` & `omniduct-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/pyproject.toml` & `omniduct-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.1/PKG-INFO` & `omniduct-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: omniduct
-Version: 1.2.1
+Version: 1.2.2
 Summary: A toolkit providing a uniform interface for connecting to and extracting data from a wide variety of (potentially remote) data stores (including HDFS, Hive, Presto, MySQL, etc).
 Project-URL: Homepage, https://github.com/airbnb/omniduct
 Author-email: Matthew Wardrop <mpwardrop@gmail.com>, Dan Frank <danfrankj@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

