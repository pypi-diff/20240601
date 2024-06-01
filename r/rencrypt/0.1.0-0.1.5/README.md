# Comparing `tmp/REncrypt-0.1.0.tar.gz` & `tmp/REncrypt-0.1.5.tar.gz`

## Comparing `REncrypt-0.1.0.tar` & `REncrypt-0.1.5.tar`

### file list

```diff
@@ -1,574 +1,574 @@
--rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 REncrypt-0.1.0/Cargo.toml
--rw-r--r--   0     1001     1001        0 2024-05-31 16:07:30.000000 REncrypt-0.1.0/.SRCINFO
--rw-r--r--   0     1001     1001        4 2024-06-01 02:11:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/REncrypt-0.1.0.dist-info/INSTALLER
--rw-r--r--   0     1001     1001    25143 2024-06-01 02:11:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/REncrypt-0.1.0.dist-info/METADATA
--rw-r--r--   0     1001     1001      829 2024-06-01 02:11:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/REncrypt-0.1.0.dist-info/RECORD
--rw-r--r--   0     1001     1001        0 2024-06-01 02:11:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/REncrypt-0.1.0.dist-info/REQUESTED
--rw-r--r--   0     1001     1001       99 2024-06-01 02:11:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/REncrypt-0.1.0.dist-info/WHEEL
--rw-r--r--   0     1001     1001       99 2024-06-01 02:11:13.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/REncrypt-0.1.0.dist-info/direct_url.json
--rw-r--r--   0     1001     1001    11357 2024-06-01 02:11:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/REncrypt-0.1.0.dist-info/license_files/LICENSE
--rw-r--r--   0     1001     1001     6703 2024-06-01 02:10:28.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/maturin/__init__.py
--rw-r--r--   0     1001     1001      987 2024-06-01 02:10:28.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/maturin/__main__.py
--rw-r--r--   0     1001     1001     5602 2024-06-01 02:10:28.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/maturin/import_hook.py
--rw-r--r--   0     1001     1001        4 2024-06-01 02:10:28.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/maturin-1.5.1.dist-info/INSTALLER
--rw-r--r--   0     1001     1001    18241 2024-06-01 02:10:28.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/maturin-1.5.1.dist-info/METADATA
--rw-r--r--   0     1001     1001      849 2024-06-01 02:10:28.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/maturin-1.5.1.dist-info/RECORD
--rw-r--r--   0     1001     1001        0 2024-06-01 02:10:28.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/maturin-1.5.1.dist-info/REQUESTED
--rw-r--r--   0     1001     1001      147 2024-06-01 02:10:28.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/maturin-1.5.1.dist-info/WHEEL
--rw-r--r--   0     1001     1001      355 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/__init__.py
--rw-r--r--   0     1001     1001      854 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/__main__.py
--rw-r--r--   0     1001     1001     1444 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/__pip-runner__.py
--rw-r--r--   0     1001     1001      515 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/__init__.py
--rw-r--r--   0     1001     1001    10243 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/build_env.py
--rw-r--r--   0     1001     1001    10370 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cache.py
--rw-r--r--   0     1001     1001      132 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0     1001     1001     6690 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0     1001     1001     8733 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0     1001     1001    30064 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0     1001     1001      774 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0     1001     1001     2816 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0     1001     1001     4338 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0     1001     1001    10781 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0     1001     1001     1968 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0     1001     1001    18369 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0     1001     1001     5118 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0     1001     1001      116 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0     1001     1001     3882 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0     1001     1001     7944 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0     1001     1001     1782 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0     1001     1001     4287 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0     1001     1001     9766 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0     1001     1001     6777 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0     1001     1001     5335 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0     1001     1001     3172 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0     1001     1001     1703 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0     1001     1001     1132 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0     1001     1001     4775 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0     1001     1001     3188 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0     1001     1001    28782 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0     1001     1001    12450 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0     1001     1001     5697 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0     1001     1001     6419 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0     1001     1001     3886 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0     1001     1001     6476 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0     1001     1001    14006 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/configuration.py
--rw-r--r--   0     1001     1001      858 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0     1001     1001     1743 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0     1001     1001      842 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0     1001     1001     6709 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0     1001     1001     1277 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0     1001     1001    23634 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0     1001     1001       30 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0     1001     1001    16590 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0     1001     1001    37843 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0     1001     1001     8688 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0     1001     1001    15365 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0     1001     1001     6009 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0     1001     1001     7680 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0     1001     1001     2556 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0     1001     1001      340 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/main.py
--rw-r--r--   0     1001     1001     4339 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0     1001     1001     2627 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0     1001     1001    25907 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0     1001     1001      135 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0     1001     1001     1882 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0     1001     1001     8297 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0     1001     1001     7456 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0     1001     1001    10035 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0     1001     1001       63 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0     1001     1001      931 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0     1001     1001     6889 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0     1001     1001     2486 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0     1001     1001     1030 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/index.py
--rw-r--r--   0     1001     1001     2818 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0     1001     1001    20777 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/link.py
--rw-r--r--   0     1001     1001      738 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0     1001     1001     4643 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0     1001     1001     1907 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0     1001     1001     4272 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0     1001     1001     3600 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0     1001     1001       50 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0     1001     1001    20541 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0     1001     1001     3935 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0     1001     1001     6086 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/network/download.py
--rw-r--r--   0     1001     1001     7638 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0     1001     1001    18698 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/network/session.py
--rw-r--r--   0     1001     1001     4073 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0     1001     1001     1838 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0     1001     1001     4832 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0     1001     1001     1422 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0     1001     1001     1474 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0     1001     1001     2198 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0     1001     1001     1075 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0     1001     1001     1417 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0     1001     1001     3064 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0     1001     1001     6806 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0     1001     1001     9816 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0     1001     1001       51 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0     1001     1001     1282 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0     1001     1001    27311 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0     1001     1001    28128 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0     1001     1001     7152 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0     1001     1001     2738 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0     1001     1001    19018 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0     1001     1001    17790 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0     1001     1001    35460 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0     1001     1001     4704 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0     1001     1001    24551 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0     1001     1001      583 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0     1001     1001    24025 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0     1001     1001     5173 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0     1001     1001    21052 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0     1001     1001    32292 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0     1001     1001     5705 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0     1001     1001     9824 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0     1001     1001     3100 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0     1001     1001     5696 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0     1001     1001    12592 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0     1001     1001     8378 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0     1001     1001     3351 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-r--r--   0     1001     1001     1015 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0     1001     1001     1665 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0     1001     1001     1884 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0     1001     1001     5377 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0     1001     1001      242 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0     1001     1001     3627 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0     1001     1001     3206 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0     1001     1001     2463 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0     1001     1001     1169 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0     1001     1001     3064 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0     1001     1001     5122 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0     1001     1001      716 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0     1001     1001     3113 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0     1001     1001     5118 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0     1001     1001    11603 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0     1001     1001    23623 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0     1001     1001     1193 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0     1001     1001     2108 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0     1001     1001     4435 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0     1001     1001     9207 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0     1001     1001     9312 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0     1001     1001     8821 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0     1001     1001     1759 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0     1001     1001     3456 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0     1001     1001     4499 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0     1001     1001      596 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0     1001     1001     3519 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0     1001     1001    18121 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0     1001     1001     5249 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0     1001     1001    11729 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0     1001     1001    22787 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0     1001     1001    11801 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0     1001     1001     4993 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0     1001     1001      676 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0     1001     1001     1737 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0     1001     1001     6392 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0     1001     1001     1952 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0     1001     1001      303 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0     1001     1001     5352 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0     1001     1001     1386 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0     1001     1001    18384 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0     1001     1001     4292 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0     1001     1001     4828 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/py.typed
--rw-r--r--   0     1001     1001     7173 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0     1001     1001     1417 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0     1001     1001       94 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0     1001     1001      255 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0     1001     1001   281617 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0     1001     1001     4279 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/certifi/py.typed
--rw-r--r--   0     1001     1001     4797 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0     1001     1001    31274 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0     1001     1001     1763 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0     1001     1001    10032 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0     1001     1001     3915 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0     1001     1001     5420 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0     1001     1001     3242 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0     1001     1001     3732 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0     1001     1001      542 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0     1001     1001     1860 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0     1001     1001     1683 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0     1001     1001     4006 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0     1001     1001    12176 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0     1001     1001     3934 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0     1001     1001    13566 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0     1001     1001     1753 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0     1001     1001    36913 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0     1001     1001     1753 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0     1001     1001    20735 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0     1001     1001     1759 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0     1001     1001    14537 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0     1001     1001    25796 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0     1001     1001    42498 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0     1001     1001     1752 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0     1001     1001    27055 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0     1001     1001   104562 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0     1001     1001    98484 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0     1001     1001    98196 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0     1001     1001   101363 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0     1001     1001   128035 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0     1001     1001   102774 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0     1001     1001    95372 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0     1001     1001     5380 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0     1001     1001     6077 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0     1001     1001     3715 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0     1001     1001     2131 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0     1001     1001    30391 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0     1001     1001    13560 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/py.typed
--rw-r--r--   0     1001     1001      402 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0     1001     1001     6400 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0     1001     1001     4137 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0     1001     1001     4007 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0     1001     1001    14848 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0     1001     1001     8505 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0     1001     1001     2812 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0     1001     1001      244 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0     1001     1001      266 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0     1001     1001     2522 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0     1001     1001    11128 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0     1001     1001     3325 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0     1001     1001       75 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0     1001     1001     2839 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0     1001     1001    10678 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0     1001     1001     6741 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0     1001     1001     1866 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0     1001     1001     1079 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0     1001     1001     3709 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0     1001     1001     6181 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0     1001     1001     7134 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0     1001     1001      625 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0     1001     1001    41487 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0     1001     1001    51965 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0     1001     1001    20797 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0     1001     1001    51767 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0     1001     1001    14168 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0     1001     1001     5268 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0     1001     1001    39693 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0     1001     1001    10820 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0     1001     1001    18315 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0     1001     1001    97792 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/t32.exe
--rw-r--r--   0     1001     1001   182784 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/t64-arm.exe
--rw-r--r--   0     1001     1001   108032 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0     1001     1001    67530 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0     1001     1001    23747 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0     1001     1001    91648 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/w32.exe
--rw-r--r--   0     1001     1001   168448 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/w64-arm.exe
--rw-r--r--   0     1001     1001   101888 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0     1001     1001    43958 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0     1001     1001      981 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0     1001     1001       64 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0     1001     1001    49330 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distro/py.typed
--rw-r--r--   0     1001     1001      849 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0     1001     1001     3374 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0     1001     1001      321 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0     1001     1001    12950 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0     1001     1001    44375 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0     1001     1001     1881 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0     1001     1001       21 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/idna/py.typed
--rw-r--r--   0     1001     1001   206539 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0     1001     1001     1132 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0     1001     1001     1081 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0     1001     1001     6079 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0     1001     1001    34544 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0     1001     1001      661 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0     1001     1001      497 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0     1001     1001    11488 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0     1001     1001     4378 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0     1001     1001     1431 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0     1001     1001     8487 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/py.typed
--rw-r--r--   0     1001     1001     4676 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0     1001     1001    30110 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0     1001     1001    15699 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0     1001     1001     4200 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0     1001     1001    14665 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0     1001     1001   109364 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0     1001     1001    20155 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0     1001     1001     1476 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0     1001     1001     7211 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0     1001     1001     7132 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0     1001     1001     3678 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/py.typed
--rw-r--r--   0     1001     1001     8809 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0     1001     1001      160 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0     1001     1001     9573 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0     1001     1001     2983 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0     1001     1001      353 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0     1001     1001    23685 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0     1001     1001     1697 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0     1001     1001     1938 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0     1001     1001    40386 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0     1001     1001     4178 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0     1001     1001     5424 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0     1001     1001     4176 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0     1001     1001     3314 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0     1001     1001     5094 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0     1001     1001    35610 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0     1001     1001    21938 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0     1001     1001     4981 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0     1001     1001    19351 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0     1001     1001     5073 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0     1001     1001     2212 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0     1001     1001     5014 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0     1001     1001     7335 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0     1001     1001     4674 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0     1001     1001    11753 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0     1001     1001    34618 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0     1001     1001    12130 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0     1001     1001    72281 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0     1001     1001    53424 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0     1001     1001      986 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0     1001     1001     2591 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0     1001     1001     3072 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0     1001     1001     3092 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0     1001     1001     6882 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0     1001     1001     6257 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0     1001     1001     3700 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0     1001     1001     6184 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0     1001     1001    63223 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0     1001     1001    10230 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0     1001     1001     9116 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0     1001     1001     6567 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0     1001     1001    13387 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0     1001     1001   224445 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0     1001     1001    24215 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0     1001     1001     9523 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0     1001     1001    38646 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/py.typed
--rw-r--r--   0     1001     1001    26692 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0     1001     1001    13488 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0     1001     1001    10646 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0     1001     1001     8670 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0     1001     1001      491 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0     1001     1001      138 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0     1001     1001    11920 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0     1001     1001      546 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0     1001     1001    10927 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0     1001     1001     5169 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0     1001     1001      435 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0     1001     1001     1495 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0     1001     1001    19697 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0     1001     1001     6449 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0     1001     1001    10187 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0     1001     1001      575 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0     1001     1001     1286 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0     1001     1001    18560 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0     1001     1001     3823 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0     1001     1001     3879 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0     1001     1001      733 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0     1001     1001    35288 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0     1001     1001      695 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0     1001     1001    30373 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0     1001     1001     4235 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0     1001     1001     2912 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0     1001     1001    33460 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0     1001     1001      537 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0     1001     1001      156 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0     1001     1001     5871 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/py.typed
--rw-r--r--   0     1001     1001     1601 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0     1001     1001    20511 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0     1001     1001     4963 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0     1001     1001     6090 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0     1001     1001     8478 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0     1001     1001    10096 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0     1001     1001   140235 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0     1001     1001     1064 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0     1001     1001     2100 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0     1001     1001      265 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0     1001     1001      799 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_fileno.py
--rw-r--r--   0     1001     1001     9695 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0     1001     1001     3225 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0     1001     1001     1236 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0     1001     1001     1387 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0     1001     1001     7063 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0     1001     1001      423 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0     1001     1001     5472 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0     1001     1001    19919 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0     1001     1001      351 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0     1001     1001      417 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0     1001     1001    22820 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0     1001     1001     1926 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0     1001     1001     2783 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0     1001     1001     1840 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0     1001     1001      890 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0     1001     1001    10368 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0     1001     1001     6906 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0     1001     1001     3264 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0     1001     1001     9842 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0     1001     1001     4509 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0     1001     1001    18224 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0     1001     1001     1054 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0     1001     1001     7131 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0     1001     1001    99218 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0     1001     1001     1288 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0     1001     1001     5497 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0     1001     1001     6630 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0     1001     1001     8082 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0     1001     1001      972 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0     1001     1001     2501 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0     1001     1001      642 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0     1001     1001     1683 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0     1001     1001     2508 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0     1001     1001     9584 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0     1001     1001     5032 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0     1001     1001     3252 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0     1001     1001    14007 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0     1001     1001    14273 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0     1001     1001     3667 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0     1001     1001    11903 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0     1001     1001     8198 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0     1001     1001     5305 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0     1001     1001     4970 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0     1001     1001      828 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0     1001     1001     3396 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0     1001     1001    10574 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0     1001     1001    35852 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0     1001     1001    59706 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0     1001     1001     8165 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0     1001     1001    11303 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0     1001     1001     1391 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/py.typed
--rw-r--r--   0     1001     1001      166 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0     1001     1001     4431 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0     1001     1001     4602 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0     1001     1001     2843 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0     1001     1001     1591 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0     1001     1001    24247 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0     1001     1001     4339 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0     1001     1001     4425 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0     1001     1001    27073 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0     1001     1001     1258 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0     1001     1001    35173 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0     1001     1001    39684 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0     1001     1001     3370 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0     1001     1001    45525 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0     1001     1001     3777 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0     1001     1001      102 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0     1001     1001    29604 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0     1001     1001     9169 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0     1001     1001    34549 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/six.py
--rw-r--r--   0     1001     1001    20493 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0     1001     1001     3551 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0     1001     1001     2179 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0     1001     1001     1682 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0     1001     1001     1562 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0     1001     1001     2372 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0     1001     1001     1383 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/py.typed
--rw-r--r--   0     1001     1001     8746 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0     1001     1001     3086 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0     1001     1001     2142 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0     1001     1001     8024 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0     1001     1001      396 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0     1001     1001    22633 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0     1001     1001     2943 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0     1001     1001      254 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0     1001     1001       26 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tomli/py.typed
--rw-r--r--   0     1001     1001      403 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/__init__.py
--rw-r--r--   0     1001     1001     9893 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_api.py
--rw-r--r--   0     1001     1001    17694 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_macos.py
--rw-r--r--   0     1001     1001     2324 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_openssl.py
--rw-r--r--   0     1001     1001     1130 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_ssl_constants.py
--rw-r--r--   0     1001     1001    17468 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_windows.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/py.typed
--rw-r--r--   0     1001     1001   111130 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0     1001     1001     3333 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0     1001     1001    10811 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0     1001     1001       64 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0     1001     1001    20300 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0     1001     1001    39990 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0     1001     1001      957 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0     1001     1001    17632 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0     1001     1001    13922 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0     1001     1001    11036 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0     1001     1001     4528 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0     1001     1001    17081 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0     1001     1001    34448 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0     1001     1001     7097 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0     1001     1001     8217 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0     1001     1001     8579 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0     1001     1001     2440 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0     1001     1001     1417 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0     1001     1001     5343 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
--rw-r--r--   0     1001     1001    34665 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0     1001     1001    19752 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0     1001     1001     6691 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0     1001     1001    30641 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0     1001     1001     1155 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0     1001     1001     4901 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0     1001     1001     1605 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0     1001     1001      498 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0     1001     1001     3997 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0     1001     1001     3510 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0     1001     1001    22013 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0     1001     1001    17177 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0     1001     1001     5758 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0     1001     1001     6895 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0     1001     1001    10168 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0     1001     1001    14296 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0     1001     1001     5403 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0     1001     1001      493 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0     1001     1001    10579 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0     1001     1001     8979 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0     1001     1001     1305 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0     1001     1001     6563 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0     1001     1001     4307 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0     1001     1001      286 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/py.typed
--rw-r--r--   0     1001     1001    10388 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/AUTHORS.txt
--rw-r--r--   0     1001     1001        4 2024-06-01 02:01:13.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/INSTALLER
--rw-r--r--   0     1001     1001     1093 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/LICENSE.txt
--rw-r--r--   0     1001     1001     3581 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/METADATA
--rw-r--r--   0     1001     1001    78936 2024-06-01 02:01:13.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/RECORD
--rw-r--r--   0     1001     1001        0 2024-06-01 02:01:13.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/REQUESTED
--rw-r--r--   0     1001     1001       92 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/WHEEL
--rw-r--r--   0     1001     1001      125 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/entry_points.txt
--rw-r--r--   0     1001     1001        4 2024-06-01 02:01:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/top_level.txt
--rw-r--r--   0     1001     1001      115 2024-06-01 07:31:00.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/procmaps/__init__.py
--rw-r--r--   0     1001     1001        4 2024-06-01 07:31:00.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/INSTALLER
--rw-r--r--   0     1001     1001     1781 2024-06-01 07:31:00.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/METADATA
--rw-r--r--   0     1001     1001      706 2024-06-01 07:31:00.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/RECORD
--rw-r--r--   0     1001     1001        0 2024-06-01 07:31:00.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/REQUESTED
--rw-r--r--   0     1001     1001      127 2024-06-01 07:31:00.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/WHEEL
--rw-r--r--   0     1001     1001     1109 2024-06-01 07:31:00.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/license_files/LICENSE
--rw-r--r--   0     1001     1001      115 2024-06-01 02:11:12.000000 REncrypt-0.1.0/.env/lib64/python3.12/site-packages/rencrypt/__init__.py
--rw-r--r--   0     1001     1001      192 2024-06-01 02:01:10.000000 REncrypt-0.1.0/.env/pyvenv.cfg
--rw-r--r--   0     1001     1001     4344 2024-06-01 07:59:53.000000 REncrypt-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001     1001      686 2024-05-28 14:37:57.000000 REncrypt-0.1.0/.gitignore
--rw-r--r--   0     1001     1001      394 2024-05-30 03:48:14.000000 REncrypt-0.1.0/.gitpod.yml
--rw-r--r--   0     1001     1001    11357 2024-05-29 01:36:25.000000 REncrypt-0.1.0/LICENSE
--rw-r--r--   0     1001     1001    25614 2024-06-01 06:40:27.000000 REncrypt-0.1.0/README.md
--rw-r--r--   0     1001     1001    15170 2024-06-01 06:51:44.000000 REncrypt-0.1.0/bench.py
--rw-r--r--   0     1001     1001     1107 2024-05-29 16:10:51.000000 REncrypt-0.1.0/benches/parallel_copy.rs
--rw-r--r--   0     1001     1001     1768 2024-06-01 06:39:09.000000 REncrypt-0.1.0/examples/encrypt.py
--rw-r--r--   0     1001     1001     3041 2024-06-01 06:38:49.000000 REncrypt-0.1.0/examples/encrypt_file.py
--rw-r--r--   0     1001     1001      965 2024-06-01 06:38:57.000000 REncrypt-0.1.0/examples/encrypt_from.py
--rw-r--r--   0     1001     1001     1372 2024-06-01 06:39:04.000000 REncrypt-0.1.0/examples/encrypt_into.py
--rw-r--r--   0     1001     1001    51365 2024-05-30 20:11:14.000000 REncrypt-0.1.0/resources/charts/decrypt-all.png
--rw-r--r--   0     1001     1001    30475 2024-06-01 05:23:25.000000 REncrypt-0.1.0/resources/charts/decrypt-file.png
--rw-r--r--   0     1001     1001    30645 2024-05-30 19:57:33.000000 REncrypt-0.1.0/resources/charts/decrypt.png
--rw-r--r--   0     1001     1001    51749 2024-05-30 20:18:23.000000 REncrypt-0.1.0/resources/charts/encrypt-all.png
--rw-r--r--   0     1001     1001    31716 2024-06-01 00:14:33.000000 REncrypt-0.1.0/resources/charts/encrypt-file.png
--rw-r--r--   0     1001     1001    29936 2024-05-30 19:58:10.000000 REncrypt-0.1.0/resources/charts/encrypt.png
--rw-r--r--   0     1001     1001    28627 2024-06-01 01:10:14.000000 REncrypt-0.1.0/resources/charts/speed-throughput.png
--rw-r--r--   0     1001     1001    29720 2024-06-01 07:45:06.000000 REncrypt-0.1.0/src/lib.rs
--rw-r--r--   0     1001     1001    23698 2024-06-01 07:59:21.000000 REncrypt-0.1.0/Cargo.lock
--rw-r--r--   0     1001     1001      904 2024-06-01 08:57:34.000000 REncrypt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    26423 1970-01-01 00:00:00.000000 REncrypt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 REncrypt-0.1.5/Cargo.toml
+-rw-r--r--   0     1001     1001        0 2024-05-31 16:07:30.000000 REncrypt-0.1.5/.SRCINFO
+-rw-r--r--   0     1001     1001        4 2024-06-01 09:02:41.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/REncrypt-0.1.5.dist-info/INSTALLER
+-rw-r--r--   0     1001     1001    26878 2024-06-01 09:02:41.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/REncrypt-0.1.5.dist-info/METADATA
+-rw-r--r--   0     1001     1001      829 2024-06-01 09:02:41.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/REncrypt-0.1.5.dist-info/RECORD
+-rw-r--r--   0     1001     1001        0 2024-06-01 09:02:41.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/REncrypt-0.1.5.dist-info/REQUESTED
+-rw-r--r--   0     1001     1001       99 2024-06-01 09:02:41.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/REncrypt-0.1.5.dist-info/WHEEL
+-rw-r--r--   0     1001     1001       99 2024-06-01 09:02:42.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/REncrypt-0.1.5.dist-info/direct_url.json
+-rw-r--r--   0     1001     1001    11357 2024-06-01 09:02:41.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/REncrypt-0.1.5.dist-info/license_files/LICENSE
+-rw-r--r--   0     1001     1001     6703 2024-06-01 02:10:28.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/maturin/__init__.py
+-rw-r--r--   0     1001     1001      987 2024-06-01 02:10:28.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/maturin/__main__.py
+-rw-r--r--   0     1001     1001     5602 2024-06-01 02:10:28.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/maturin/import_hook.py
+-rw-r--r--   0     1001     1001        4 2024-06-01 02:10:28.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/maturin-1.5.1.dist-info/INSTALLER
+-rw-r--r--   0     1001     1001    18241 2024-06-01 02:10:28.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/maturin-1.5.1.dist-info/METADATA
+-rw-r--r--   0     1001     1001      849 2024-06-01 02:10:28.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/maturin-1.5.1.dist-info/RECORD
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:10:28.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/maturin-1.5.1.dist-info/REQUESTED
+-rw-r--r--   0     1001     1001      147 2024-06-01 02:10:28.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/maturin-1.5.1.dist-info/WHEEL
+-rw-r--r--   0     1001     1001      355 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/__init__.py
+-rw-r--r--   0     1001     1001      854 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/__main__.py
+-rw-r--r--   0     1001     1001     1444 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0     1001     1001      515 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0     1001     1001    10243 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0     1001     1001    10370 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cache.py
+-rw-r--r--   0     1001     1001      132 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0     1001     1001     6690 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0     1001     1001     8733 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0     1001     1001    30064 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0     1001     1001      774 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0     1001     1001     2816 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0     1001     1001     4338 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0     1001     1001    10781 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0     1001     1001     1968 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0     1001     1001    18369 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0     1001     1001     5118 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0     1001     1001      116 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0     1001     1001     3882 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0     1001     1001     7944 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0     1001     1001     1782 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0     1001     1001     4287 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0     1001     1001     9766 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0     1001     1001     6777 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0     1001     1001     5335 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0     1001     1001     3172 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0     1001     1001     1703 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0     1001     1001     1132 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0     1001     1001     4775 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0     1001     1001     3188 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0     1001     1001    28782 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0     1001     1001    12450 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0     1001     1001     5697 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0     1001     1001     6419 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0     1001     1001     3886 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0     1001     1001     6476 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0     1001     1001    14006 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0     1001     1001      858 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0     1001     1001     1743 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0     1001     1001      842 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0     1001     1001     6709 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0     1001     1001     1277 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0     1001     1001    23634 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0     1001     1001       30 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0     1001     1001    16590 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0     1001     1001    37843 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0     1001     1001     8688 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0     1001     1001    15365 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0     1001     1001     6009 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0     1001     1001     7680 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0     1001     1001     2556 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0     1001     1001      340 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/main.py
+-rw-r--r--   0     1001     1001     4339 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0     1001     1001     2627 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0     1001     1001    25907 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0     1001     1001      135 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0     1001     1001     1882 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0     1001     1001     8297 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0     1001     1001     7456 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0     1001     1001    10035 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0     1001     1001       63 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0     1001     1001      931 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0     1001     1001     6889 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0     1001     1001     2486 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0     1001     1001     1030 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0     1001     1001     2818 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0     1001     1001    20777 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0     1001     1001      738 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0     1001     1001     4643 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0     1001     1001     1907 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0     1001     1001     4272 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0     1001     1001     3600 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0     1001     1001       50 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0     1001     1001    20541 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0     1001     1001     3935 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0     1001     1001     6086 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0     1001     1001     7638 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0     1001     1001    18698 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0     1001     1001     4073 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0     1001     1001     1838 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0     1001     1001     4832 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0     1001     1001     1422 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0     1001     1001     1474 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0     1001     1001     2198 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0     1001     1001     1075 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0     1001     1001     1417 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0     1001     1001     3064 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0     1001     1001     6806 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0     1001     1001     9816 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0     1001     1001       51 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0     1001     1001     1282 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0     1001     1001    27311 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0     1001     1001    28128 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0     1001     1001     7152 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0     1001     1001     2738 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0     1001     1001    19018 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0     1001     1001    17790 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0     1001     1001    35460 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0     1001     1001     4704 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0     1001     1001    24551 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0     1001     1001      583 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0     1001     1001    24025 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0     1001     1001     5173 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0     1001     1001    21052 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0     1001     1001    32292 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0     1001     1001     5705 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0     1001     1001     9824 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0     1001     1001     3100 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0     1001     1001     5696 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0     1001     1001    12592 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0     1001     1001     8378 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0     1001     1001     3351 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-r--r--   0     1001     1001     1015 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0     1001     1001     1665 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0     1001     1001     1884 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0     1001     1001     5377 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0     1001     1001      242 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0     1001     1001     3627 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0     1001     1001     3206 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0     1001     1001     2463 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0     1001     1001     1169 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0     1001     1001     3064 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0     1001     1001     5122 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0     1001     1001      716 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0     1001     1001     3113 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0     1001     1001     5118 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0     1001     1001    11603 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0     1001     1001    23623 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0     1001     1001     1193 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0     1001     1001     2108 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0     1001     1001     4435 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0     1001     1001     9207 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0     1001     1001     9312 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0     1001     1001     8821 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0     1001     1001     1759 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0     1001     1001     3456 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0     1001     1001     4499 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0     1001     1001      596 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0     1001     1001     3519 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0     1001     1001    18121 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0     1001     1001     5249 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0     1001     1001    11729 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0     1001     1001    22787 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0     1001     1001    11801 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0     1001     1001     4993 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0     1001     1001      676 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0     1001     1001     1737 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0     1001     1001     6392 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0     1001     1001     1952 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0     1001     1001      303 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0     1001     1001     5352 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0     1001     1001     1386 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0     1001     1001    18384 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0     1001     1001     4292 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0     1001     1001     4828 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/py.typed
+-rw-r--r--   0     1001     1001     7173 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0     1001     1001     1417 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0     1001     1001       94 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0     1001     1001      255 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0     1001     1001   281617 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0     1001     1001     4279 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/certifi/py.typed
+-rw-r--r--   0     1001     1001     4797 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0     1001     1001    31274 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0     1001     1001     1763 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0     1001     1001    10032 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0     1001     1001     3915 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0     1001     1001     5420 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0     1001     1001     3242 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0     1001     1001     3732 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0     1001     1001      542 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0     1001     1001     1860 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0     1001     1001     1683 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0     1001     1001     4006 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0     1001     1001    12176 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0     1001     1001     3934 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0     1001     1001    13566 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0     1001     1001     1753 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0     1001     1001    36913 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0     1001     1001     1753 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0     1001     1001    20735 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0     1001     1001     1759 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0     1001     1001    14537 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0     1001     1001    25796 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0     1001     1001    42498 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0     1001     1001     1752 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0     1001     1001    27055 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0     1001     1001   104562 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0     1001     1001    98484 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0     1001     1001    98196 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0     1001     1001   101363 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0     1001     1001   128035 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0     1001     1001   102774 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0     1001     1001    95372 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0     1001     1001     5380 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0     1001     1001     6077 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0     1001     1001     3715 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0     1001     1001     2131 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0     1001     1001    30391 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0     1001     1001    13560 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/py.typed
+-rw-r--r--   0     1001     1001      402 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0     1001     1001     6400 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0     1001     1001     4137 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0     1001     1001     4007 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0     1001     1001    14848 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0     1001     1001     8505 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0     1001     1001     2812 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0     1001     1001      244 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0     1001     1001      266 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0     1001     1001     2522 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0     1001     1001    11128 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0     1001     1001     3325 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0     1001     1001       75 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0     1001     1001     2839 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0     1001     1001    10678 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0     1001     1001     6741 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0     1001     1001     1866 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0     1001     1001     1079 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0     1001     1001     3709 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0     1001     1001     6181 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0     1001     1001     7134 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0     1001     1001      625 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0     1001     1001    41487 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0     1001     1001    51965 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0     1001     1001    20797 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0     1001     1001    51767 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0     1001     1001    14168 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0     1001     1001     5268 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0     1001     1001    39693 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0     1001     1001    10820 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0     1001     1001    18315 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0     1001     1001    97792 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/t32.exe
+-rw-r--r--   0     1001     1001   182784 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rw-r--r--   0     1001     1001   108032 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0     1001     1001    67530 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0     1001     1001    23747 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0     1001     1001    91648 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/w32.exe
+-rw-r--r--   0     1001     1001   168448 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rw-r--r--   0     1001     1001   101888 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0     1001     1001    43958 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0     1001     1001      981 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0     1001     1001       64 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0     1001     1001    49330 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distro/py.typed
+-rw-r--r--   0     1001     1001      849 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0     1001     1001     3374 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0     1001     1001      321 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0     1001     1001    12950 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0     1001     1001    44375 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0     1001     1001     1881 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0     1001     1001       21 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/idna/py.typed
+-rw-r--r--   0     1001     1001   206539 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0     1001     1001     1132 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0     1001     1001     1081 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0     1001     1001     6079 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0     1001     1001    34544 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0     1001     1001      661 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0     1001     1001      497 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0     1001     1001    11488 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0     1001     1001     4378 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0     1001     1001     1431 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0     1001     1001     8487 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/py.typed
+-rw-r--r--   0     1001     1001     4676 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0     1001     1001    30110 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0     1001     1001    15699 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0     1001     1001     4200 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0     1001     1001    14665 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0     1001     1001   109364 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0     1001     1001    20155 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0     1001     1001     1476 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0     1001     1001     7211 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0     1001     1001     7132 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0     1001     1001     3678 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/py.typed
+-rw-r--r--   0     1001     1001     8809 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0     1001     1001      160 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0     1001     1001     9573 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0     1001     1001     2983 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0     1001     1001      353 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0     1001     1001    23685 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0     1001     1001     1697 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0     1001     1001     1938 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0     1001     1001    40386 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0     1001     1001     4178 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0     1001     1001     5424 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0     1001     1001     4176 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0     1001     1001     3314 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0     1001     1001     5094 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0     1001     1001    35610 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0     1001     1001    21938 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0     1001     1001     4981 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0     1001     1001    19351 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0     1001     1001     5073 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0     1001     1001     2212 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0     1001     1001     5014 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0     1001     1001     7335 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0     1001     1001     4674 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0     1001     1001    11753 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0     1001     1001    34618 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0     1001     1001    12130 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0     1001     1001    72281 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0     1001     1001    53424 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0     1001     1001      986 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0     1001     1001     2591 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0     1001     1001     3072 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0     1001     1001     3092 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0     1001     1001     6882 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0     1001     1001     6257 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0     1001     1001     3700 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0     1001     1001     6184 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0     1001     1001    63223 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0     1001     1001    10230 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0     1001     1001     9116 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0     1001     1001     6567 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0     1001     1001    13387 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0     1001     1001   224445 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0     1001     1001    24215 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0     1001     1001     9523 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0     1001     1001    38646 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/py.typed
+-rw-r--r--   0     1001     1001    26692 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0     1001     1001    13488 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0     1001     1001    10646 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0     1001     1001     8670 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0     1001     1001      491 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0     1001     1001      138 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0     1001     1001    11920 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0     1001     1001      546 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0     1001     1001    10927 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0     1001     1001     5169 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0     1001     1001      435 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0     1001     1001     1495 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0     1001     1001    19697 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0     1001     1001     6449 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0     1001     1001    10187 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0     1001     1001      575 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0     1001     1001     1286 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0     1001     1001    18560 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0     1001     1001     3823 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0     1001     1001     3879 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0     1001     1001      733 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0     1001     1001    35288 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0     1001     1001      695 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0     1001     1001    30373 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0     1001     1001     4235 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0     1001     1001     2912 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0     1001     1001    33460 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0     1001     1001      537 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0     1001     1001      156 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0     1001     1001     5871 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/py.typed
+-rw-r--r--   0     1001     1001     1601 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0     1001     1001    20511 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0     1001     1001     4963 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0     1001     1001     6090 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0     1001     1001     8478 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0     1001     1001    10096 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0     1001     1001   140235 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0     1001     1001     1064 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0     1001     1001     2100 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0     1001     1001      265 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0     1001     1001      799 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_fileno.py
+-rw-r--r--   0     1001     1001     9695 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0     1001     1001     3225 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0     1001     1001     1236 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0     1001     1001     1387 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0     1001     1001     7063 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0     1001     1001      423 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0     1001     1001     5472 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0     1001     1001    19919 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0     1001     1001      351 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0     1001     1001      417 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0     1001     1001    22820 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0     1001     1001     1926 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0     1001     1001     2783 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0     1001     1001     1840 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0     1001     1001      890 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0     1001     1001    10368 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0     1001     1001     6906 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0     1001     1001     3264 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0     1001     1001     9842 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0     1001     1001     4509 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0     1001     1001    18224 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0     1001     1001     1054 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0     1001     1001     7131 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0     1001     1001    99218 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0     1001     1001     1288 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0     1001     1001     5497 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0     1001     1001     6630 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0     1001     1001     8082 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0     1001     1001      972 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0     1001     1001     2501 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0     1001     1001      642 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0     1001     1001     1683 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0     1001     1001     2508 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0     1001     1001     9584 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0     1001     1001     5032 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0     1001     1001     3252 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0     1001     1001    14007 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0     1001     1001    14273 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0     1001     1001     3667 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0     1001     1001    11903 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0     1001     1001     8198 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0     1001     1001     5305 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0     1001     1001     4970 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0     1001     1001      828 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0     1001     1001     3396 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0     1001     1001    10574 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0     1001     1001    35852 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0     1001     1001    59706 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0     1001     1001     8165 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0     1001     1001    11303 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0     1001     1001     1391 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/py.typed
+-rw-r--r--   0     1001     1001      166 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0     1001     1001     4431 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0     1001     1001     4602 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0     1001     1001     2843 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0     1001     1001     1591 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0     1001     1001    24247 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0     1001     1001     4339 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0     1001     1001     4425 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0     1001     1001    27073 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0     1001     1001     1258 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0     1001     1001    35173 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0     1001     1001    39684 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0     1001     1001     3370 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0     1001     1001    45525 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0     1001     1001     3777 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0     1001     1001      102 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0     1001     1001    29604 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0     1001     1001     9169 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0     1001     1001    34549 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/six.py
+-rw-r--r--   0     1001     1001    20493 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0     1001     1001     3551 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0     1001     1001     2179 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0     1001     1001     1682 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0     1001     1001     1562 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0     1001     1001     2372 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0     1001     1001     1383 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/py.typed
+-rw-r--r--   0     1001     1001     8746 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0     1001     1001     3086 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0     1001     1001     2142 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0     1001     1001     8024 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0     1001     1001      396 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0     1001     1001    22633 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0     1001     1001     2943 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0     1001     1001      254 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0     1001     1001       26 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tomli/py.typed
+-rw-r--r--   0     1001     1001      403 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/__init__.py
+-rw-r--r--   0     1001     1001     9893 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_api.py
+-rw-r--r--   0     1001     1001    17694 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_macos.py
+-rw-r--r--   0     1001     1001     2324 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_openssl.py
+-rw-r--r--   0     1001     1001     1130 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_ssl_constants.py
+-rw-r--r--   0     1001     1001    17468 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_windows.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/py.typed
+-rw-r--r--   0     1001     1001   111130 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0     1001     1001     3333 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0     1001     1001    10811 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0     1001     1001       64 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0     1001     1001    20300 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0     1001     1001    39990 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0     1001     1001      957 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0     1001     1001    17632 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0     1001     1001    13922 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0     1001     1001    11036 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0     1001     1001     4528 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0     1001     1001    17081 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0     1001     1001    34448 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0     1001     1001     7097 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0     1001     1001     8217 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0     1001     1001     8579 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0     1001     1001     2440 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0     1001     1001     1417 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0     1001     1001     5343 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
+-rw-r--r--   0     1001     1001    34665 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0     1001     1001    19752 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0     1001     1001     6691 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0     1001     1001    30641 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0     1001     1001     1155 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0     1001     1001     4901 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0     1001     1001     1605 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0     1001     1001      498 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0     1001     1001     3997 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0     1001     1001     3510 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0     1001     1001    22013 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0     1001     1001    17177 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0     1001     1001     5758 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0     1001     1001     6895 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0     1001     1001    10168 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0     1001     1001    14296 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0     1001     1001     5403 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0     1001     1001      493 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0     1001     1001    10579 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0     1001     1001     8979 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0     1001     1001     1305 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0     1001     1001     6563 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0     1001     1001     4307 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0     1001     1001      286 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/py.typed
+-rw-r--r--   0     1001     1001    10388 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/AUTHORS.txt
+-rw-r--r--   0     1001     1001        4 2024-06-01 02:01:13.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/INSTALLER
+-rw-r--r--   0     1001     1001     1093 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/LICENSE.txt
+-rw-r--r--   0     1001     1001     3581 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/METADATA
+-rw-r--r--   0     1001     1001    78936 2024-06-01 02:01:13.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/RECORD
+-rw-r--r--   0     1001     1001        0 2024-06-01 02:01:13.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/REQUESTED
+-rw-r--r--   0     1001     1001       92 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/WHEEL
+-rw-r--r--   0     1001     1001      125 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/entry_points.txt
+-rw-r--r--   0     1001     1001        4 2024-06-01 02:01:12.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/top_level.txt
+-rw-r--r--   0     1001     1001      115 2024-06-01 07:31:00.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/procmaps/__init__.py
+-rw-r--r--   0     1001     1001        4 2024-06-01 07:31:00.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/INSTALLER
+-rw-r--r--   0     1001     1001     1781 2024-06-01 07:31:00.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/METADATA
+-rw-r--r--   0     1001     1001      706 2024-06-01 07:31:00.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/RECORD
+-rw-r--r--   0     1001     1001        0 2024-06-01 07:31:00.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/REQUESTED
+-rw-r--r--   0     1001     1001      127 2024-06-01 07:31:00.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/WHEEL
+-rw-r--r--   0     1001     1001     1109 2024-06-01 07:31:00.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/license_files/LICENSE
+-rw-r--r--   0     1001     1001      115 2024-06-01 09:02:41.000000 REncrypt-0.1.5/.env/lib64/python3.12/site-packages/rencrypt/__init__.py
+-rw-r--r--   0     1001     1001      192 2024-06-01 02:01:10.000000 REncrypt-0.1.5/.env/pyvenv.cfg
+-rw-r--r--   0     1001     1001     4344 2024-06-01 07:59:53.000000 REncrypt-0.1.5/.github/workflows/CI.yml
+-rw-r--r--   0     1001     1001      686 2024-05-28 14:37:57.000000 REncrypt-0.1.5/.gitignore
+-rw-r--r--   0     1001     1001      394 2024-05-30 03:48:14.000000 REncrypt-0.1.5/.gitpod.yml
+-rw-r--r--   0     1001     1001    11357 2024-05-29 01:36:25.000000 REncrypt-0.1.5/LICENSE
+-rw-r--r--   0     1001     1001    26069 2024-06-01 09:01:17.000000 REncrypt-0.1.5/README.md
+-rw-r--r--   0     1001     1001    15170 2024-06-01 06:51:44.000000 REncrypt-0.1.5/bench.py
+-rw-r--r--   0     1001     1001     1107 2024-05-29 16:10:51.000000 REncrypt-0.1.5/benches/parallel_copy.rs
+-rw-r--r--   0     1001     1001     1768 2024-06-01 06:39:09.000000 REncrypt-0.1.5/examples/encrypt.py
+-rw-r--r--   0     1001     1001     3041 2024-06-01 06:38:49.000000 REncrypt-0.1.5/examples/encrypt_file.py
+-rw-r--r--   0     1001     1001      965 2024-06-01 06:38:57.000000 REncrypt-0.1.5/examples/encrypt_from.py
+-rw-r--r--   0     1001     1001     1372 2024-06-01 06:39:04.000000 REncrypt-0.1.5/examples/encrypt_into.py
+-rw-r--r--   0     1001     1001    51365 2024-05-30 20:11:14.000000 REncrypt-0.1.5/resources/charts/decrypt-all.png
+-rw-r--r--   0     1001     1001    30475 2024-06-01 05:23:25.000000 REncrypt-0.1.5/resources/charts/decrypt-file.png
+-rw-r--r--   0     1001     1001    30645 2024-05-30 19:57:33.000000 REncrypt-0.1.5/resources/charts/decrypt.png
+-rw-r--r--   0     1001     1001    51749 2024-05-30 20:18:23.000000 REncrypt-0.1.5/resources/charts/encrypt-all.png
+-rw-r--r--   0     1001     1001    31716 2024-06-01 00:14:33.000000 REncrypt-0.1.5/resources/charts/encrypt-file.png
+-rw-r--r--   0     1001     1001    29936 2024-05-30 19:58:10.000000 REncrypt-0.1.5/resources/charts/encrypt.png
+-rw-r--r--   0     1001     1001    28627 2024-06-01 01:10:14.000000 REncrypt-0.1.5/resources/charts/speed-throughput.png
+-rw-r--r--   0     1001     1001    29720 2024-06-01 07:45:06.000000 REncrypt-0.1.5/src/lib.rs
+-rw-r--r--   0     1001     1001    23698 2024-06-01 09:02:30.000000 REncrypt-0.1.5/Cargo.lock
+-rw-r--r--   0     1001     1001      904 2024-06-01 08:57:34.000000 REncrypt-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    26878 1970-01-01 00:00:00.000000 REncrypt-0.1.5/PKG-INFO
```

### Comparing `REncrypt-0.1.0/Cargo.toml` & `REncrypt-0.1.5/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rencrypt"
-version = "0.1.0"
+version = "0.1.5"
 edition = "2021"
 
 [lib]
 name = "rencrypt"
 crate-type = ["cdylib"]
 
 [profile.dev]
```

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/REncrypt-0.1.0.dist-info/METADATA` & `REncrypt-0.1.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,26 @@
-Metadata-Version: 2.3
-Name: REncrypt
-Version: 0.1.0
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: License :: Apache-2.0 license
-License-File: LICENSE
-Summary: A Python encryption library implemented in Rust. It supports AEAD with AES-GCM and ChaCha20Poly1305. It uses ring crate to handle encryption.
-Keywords: cryptography,encryption,security,rust,speed
-Author-email: Radu Marias <radumarias@gmail.com>
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Homepage, https://github.com/radumarias/rencrypt-python
-Project-URL: Issues, https://github.com/radumarias/rencrypt-python/issues
-
 # REncrypt
 
 A Python encryption library implemented in Rust. It supports `AEAD` with `AES-GCM` and `ChaCha20Poly1305`. It uses [ring](https://crates.io/crates/ring) to handle encryption.  
-If offers slightly higher speed compared to other Python libs, especially for smaller chunks of data. The API also tries to be easy to use but it's more optimized for speed than usability.
+If offers slightly higher speed compared to other Python libs, especially for small chunks of data. The API also tries to be easy to use but it's more optimized for speed than usability.
 
 So if you want to achieve the highest possible encryption speed, consider giving it a try.
 
 # Benchmark
 
 Some benchmarks comparing to [PyFLocker](https://github.com/arunanshub/pyflocker), which, from other implementations, I found to be the fastest. After this there is also comparison with other implementations.
 
 ## Buffer in memory
 
 This is useful when you keep a buffer, set your plaintext/ciphertext in there, and then encrypt/decrypt in-place that buffer. This is the most performant way to use it, because it does't copy any bytes nor allocate new memory.  
 `REncrypt` is faster on small buffers, less than few MB, `PyFLocker` is comming closer for larger buffers.
 
-| Encrypt | Decrypt |
-| ------- | ------- |
-| ![Encrypt buffer](resources/charts/encrypt.png) | ![Decrypt buffer](resources/charts/decrypt.png) |
+| Encrypt seconds | Decrypt seconds |
+| --------------- | --------------- |
+| ![Encrypt buffer](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/encrypt.png?raw=true) | ![Decrypt buffer](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/decrypt.png?raw=true) |
 
 
 <table>
     <thead>
         <tr>
             <th rowspan=2>MB</th>
             <th colspan=2>Encrypt seconds</th>
@@ -161,20 +145,19 @@
             <td>0.24953</td>
             <td>0.25377</td>
             <td>0.42581</td>
         </tr>
     </tbody>
 </table>
 
-
 ## File
 
-| Encrypt | Decrypt |
-| ------- | ------- |
-| ![Encrypt file](resources/charts/encrypt-file.png) | ![Decrypt buffer](resources/charts/encrypt-file.png) |
+| Encrypt seconds | Decrypt seconds |
+| --------------- | --------------- |
+| ![Encrypt file](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/encrypt-file.png?raw=true) | ![Decrypt buffer](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/decrypt-file.png?raw=true) |
 
 <table>
     <thead>
         <tr>
             <th rowspan=2>MB</th>
             <th colspan=2>Encrypt seconds</th>
             <th colspan=2>Decrypt seconds</th>
@@ -237,15 +220,15 @@
             <td>0.00363</td>
         </tr>
         <tr>
             <td>4</td>
             <td>0.00361</td>
             <td>0.00765</td>
             <td>0.00301</td>
-            <td>0.00550</td>
+            <td>0.00736</td>
         </tr>
         <tr>
             <td>8</td>
             <td>0.00688</td>
             <td>0.01190</td>
             <td>0.00621</td>
             <td>0.00876</td>
@@ -306,47 +289,47 @@
             <td>1.69471</td>
             <td>2.99210</td>
         </tr>
         <tr>
             <td>4096</td>
             <td>4.85395</td>
             <td>4.69722</td>
-            <td>6.72873</td>
-            <td>4.50009</td>
+            <td>5.40580</td>
+            <td>8.73779</td>
         </tr>
         <tr>
             <td>8192</td>
             <td>10.76984</td>
             <td>11.76741</td>
-            <td>14.27756</td>
-            <td>9.66436</td>
+            <td>10.29253</td>
+            <td>21.00636</td>
         </tr>
         <tr>
             <td>16384</td>
             <td>21.84490</td>
             <td>26.27385</td>
-            <td>28.98916</td>
-            <td>19.08575</td>
+            <td>39.56230</td>
+            <td>43.55530</td>
         </tr>
     </tbody>
 </table>
 
 # Usage
 
 There are three ways in which you can use the lib, the main difference is the speed, some offers an easier way to use it sacrificing performance.
 
 1. **With a buffer in memory**: using `encrypt()`/`decrypt()`, is useful when you keep a buffer (or have it from somewhere), set your plaintext/ciphertext in there, and then encrypt/decrypt in-place that buffer. This is the most performant way to use it, because it does't copy any bytes nor allocate new memory. If you can directly collect the data to that buffer, like `buffered_reader.read_into()`, **this is the preffered way to go**.
-2. **From some bytes to the buffer**: using `encrypt_into()`/`decrypt_to_buf()`, when you have some arbitrary `bytes` that you want to work with. It will first copy those bytes to the buffer then do the operation in-place in buffer. This is a bit slower, especially for large data, because it needs to copy the bytes to the buffer.
+2. **From some bytes to the buffer**: using `encrypt_into()`/`decrypt_into()`, when you have some arbitrary `bytes` that you want to work with. It will first copy those bytes to the buffer then do the operation in-place in buffer. This is a bit slower, especially for large data, because it needs to copy the bytes to the buffer.
 3. **From some bytes to another new bytes**: using `encrypt_from()`/`decrypt_from()`, it doesn't use the buffer at all, you just got some bytes you want to work with and you receive back another new bytes. This is the slowest one because it needs to first allocate a buffer, copy the data to the buffer, perform the operation then return that buffer as bytes. It's the easiest to use but is not so performant.
 
 # Examples
 
 You can see more in [examples](https://github.com/radumarias/rencrypt-python/tree/main/examples) directory and in [bench.py](https://github.com/radumarias/rencrypt-python/tree/main/bench.py) which has some benchmarks. Here are few simple examples:
 
-## Encrypt and decrypt with a buffer in memory `encrypt`/`decrypt`
+## Encrypt and decrypt with a buffer in memory `encrypt()`/`decrypt()`
 
 This is the most performant way to use it as it will not copy bytes to the buffer nor allocate new memory for plaintext and ciphertext.
 
 ```python
 from rencrypt import REncrypt, Cipher
 import os
 
@@ -374,25 +357,28 @@
 # decrypt it
 # if you need to copy ciphertext to buffer, we don't need to do it now as it's already in the buffer
 # enc.copy_slice(ciphertext, buf[:len(ciphertext)])
 print("decryping...")
 plaintext_len = enc.decrypt(buf, ciphertext_len, 42, aad)
 plaintext2 = buf[:plaintext_len]
 assert plaintext == plaintext2
+# best practice, you should always zeroize the plaintext and key after you are done with them
 print("bye!")
 ```
 
 You can use other ciphers like `cipher = Cipher.ChaCha20Poly1305`.
 
 ## Encrypt and decrypt a file
 
 ```python
 import errno
 import io
 import os
+from pathlib import Path
+import shutil
 from rencrypt import REncrypt, Cipher
 import hashlib
 
 
 def read_file_in_chunks(file_path, buf):
     with open(file_path, "rb") as file:
         buffered_reader = io.BufferedReader(file, buffer_size=len(buf))
@@ -419,63 +405,93 @@
     try:
         os.remove(filename)
     except OSError as e:  # this would be "except OSError, e:" before Python 2.6
         if e.errno != errno.ENOENT:  # errno.ENOENT = no such file or directory
             raise  # re-raise exception if a different error occurred
 
 
-path_in = "/tmp/fin"
-path_out = "/tmp/fout.enc"
+def create_directory_in_home(dir_name):
+    # Get the user's home directory
+    home_dir = Path.home()
+
+    # Create the full path for the new directory
+    new_dir_path = home_dir / dir_name
+
+    # Create the directory
+    try:
+        new_dir_path.mkdir(parents=True, exist_ok=True)
+    except Exception as e:
+        print(f"Error creating directory: {e}")
 
-chunk_len = 128 * 1024
+    return new_dir_path.absolute().__str__()
+
+
+def create_file_with_size(file_path_str, size_in_bytes):
+    with open(file_path_str, "wb") as f:
+        for _ in range(size_in_bytes // 4096):
+            f.write(os.urandom(4096))
+
+
+def delete_dir(path):
+    if os.path.exists(path):
+        shutil.rmtree(path)
+    else:
+        print(f"Directory {path} does not exist.")
+
+
+tmp_dir = create_directory_in_home("rencrypt_tmp")
+fin = tmp_dir + "/" + "fin"
+fout = tmp_dir + "/" + "fout.enc"
+create_file_with_size(fin, 42 * 1024 * 1024)
+
+chunk_len = 256 * 1024
 
 key = os.urandom(32)
 
 cipher = Cipher.AES256GCM
 key = cipher.generate_key()
 enc = REncrypt(cipher, key)
 plaintext_len, _, buf = enc.create_buf(chunk_len)
 
 aad = b"AAD"
 
 # encrypt
 print("encryping...")
-silentremove(path_out)
-with open(path_out, "wb", buffering=plaintext_len) as file_out:
+with open(fout, "wb", buffering=plaintext_len) as file_out:
     i = 0
-    for read in read_file_in_chunks(path_in, buf[:plaintext_len]):
+    for read in read_file_in_chunks(fin, buf[:plaintext_len]):
         ciphertext_len = enc.encrypt(buf, read, i, aad)
         file_out.write(buf[:ciphertext_len])
         i += 1
     file_out.flush()
 
 # decrypt
 print("decryping...")
-tmp_path = "/tmp/fout.dec"
-with open(tmp_path, "wb", buffering=plaintext_len) as file_out:
+tmp = fout + ".dec"
+with open(tmp, "wb", buffering=plaintext_len) as file_out:
     i = 0
-    for read in read_file_in_chunks(path_out, buf):
+    for read in read_file_in_chunks(fout, buf):
         plaintext_len2 = enc.decrypt(buf, read, i, aad)
         file_out.write(buf[:plaintext_len2])
         i += 1
     file_out.flush()
 
-compare_files_by_hash(path_in, tmp_path)
+compare_files_by_hash(fin, tmp)
 
-silentremove(tmp_path)
-silentremove(path_out)
+delete_dir(tmp_dir)
+# best practice, you should always zeroize the plaintext and key after you are done with them
 
 print("bye!")
 ```
 
-## Encrypt and decrypt from some bytes to the buffer `encrypt_into`/`decrypt_into` or `encrypt_into1`/`decrypt_into1`
+## Encrypt and decrypt from some bytes to the buffer `encrypt_into()`/`decrypt_into()` or `encrypt_into1()`/`decrypt_into1()`
 
 This is a bit slower than handling data only via the buffer, especially for large plaintext, but there are situations when you can't directly collect the data to the buffer but have some `bytes` from somewhere else.
 
-For `encrypt_into`/`encrypt_into` the plaintext is `bytes`.
+For `encrypt_into()`/`decrypt_into()` the plaintext is `bytes`.
 
 ```python
 from rencrypt import REncrypt, Cipher
 import os
 
 # You can use also other ciphers like `cipher = Cipher.ChaCha20Poly1305`.
 cipher = Cipher.AES256GCM
@@ -495,25 +511,26 @@
 cipertext = bytes(buf[:ciphertext_len])
 
 # decrypt it
 print("decryping...")
 plaintext_len = enc.decrypt_into(cipertext, buf, 42, aad)
 plaintext2 = buf[:plaintext_len]
 assert plaintext == plaintext2
+# best practice, you should always zeroize the plaintext and key after you are done with them
 print("bye!")
 ```
 
-For `encrypt_into1`/`encrypt_into1` the only difference is that the plaintext is `bytearray`.
+For `encrypt_into1()`/`decrypt_into1()` the only difference is that the input is `bytearray`.
 
 
-## Encrypt and decrypt from some bytes to another new bytes, without using the buffer  `encrypt_from`/`decrypt_from` or `encrypt_from2`/`decrypt_from2`
+## Encrypt and decrypt from some bytes to another new bytes, without using the buffer  `encrypt_from()`/`decrypt_from()` or `encrypt_from1()`/`decrypt_from1()`
 
 This is the slowest option, especially for large plaintext, because it allocates new memory for the ciphertext on encrypt and plaintext on decrypt.
 
-For `encrypt_from`/`decrypt_from` the plaintext is `bytes`.
+For `encrypt_from()`/`decrypt_from()` the plaintext is `bytes`.
 
 ```python
 from rencrypt import REncrypt, Cipher
 import os
 
 # You can use also other ciphers like `cipher = Cipher.ChaCha20Poly1305`.# You can use also other ciphers like `cipher = Cipher.ChaCha20Poly1305`.
 cipher = Cipher.AES256GCM
@@ -528,18 +545,19 @@
  print("encryping...")
 ciphertext = enc.encrypt_from(plaintext, 42, aad)
 
 # decrypt it
 print("decryping...")
 plaintext2 = enc.decrypt_from(ciphertext, 42, aad)
 assert plaintext == plaintext2
+# best practice, you should always zeroize the plaintext and key after you are done with them
 print("bye!")
 ```
 
-For `encrypt_from2`/`decrypt_from2` the only difference is that the plaintext is `bytearray`.
+For `encrypt_from1()`/`decrypt_from1()` the only difference is that the input is `bytearray`.
 
 # Building from source
 
 ## Browser
 
 [![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/radumarias/rencrypt-python)
 
@@ -563,24 +581,24 @@
 . "$HOME/.cargo/env"
 ```
 ```
 python -m venv .env
 source .env/bin/activate
 pip install maturin
 maturin develop
-python python bench.py
+python bench.py
 ```
 
 # More benchmarks
 
 ## Different ways to use the lib
 
 | Encrypt | Decrypt |
 | ------- | ------- |
-| ![Encrypt buffer](resources/charts/encrypt-all.png) | ![Decrypt buffer](resources/charts/decrypt-all.png) |
+| ![Encrypt buffer](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/encrypt-all.png?raw=true) | ![Decrypt buffer](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/decrypt-all.png?raw=true) |
 
 
 <table>
     <thead>
         <tr>
             <th rowspan=2>MB</th>
             <th colspan=5>Encrypt seconds</th>
@@ -812,15 +830,15 @@
 </table>
 
 ## Speed throughput
 
 `256KB` seems to be the sweet spot for buffer size that offers the max `MB/s` speed for encryption, on benchmarks that seem to be the case.
 We performed `10.000` encryption operations for each size varying from `1KB` to `16MB`.
 
-![Speed throughput](resources/charts/speed-throughput.png)
+![Speed throughput](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/speed-throughput.png?raw=true)
 
 | MB    | MB/s |
 | ----- | ------- |
 | 0.0009765625 | 1083 |
 | 0.001953125 | 1580 |
 | 0.00390625 | 2158 |
 | 0.0078125 | 2873 |
@@ -842,8 +860,7 @@
 - Add other encryption providers like [RustCrypto](https://github.com/RustCrypto/traits) and [libsodium](https://crates.io/crates/sodiumoxide)
 - Maybe add support for `RSA` and `Elliptic-curve cryptography`
 - Saving and loading keys from file
 
 # Considerations
 
 This lib hasn't been audited, but it mostly wraps `ring` crate which is a well known library, so in principle it should offer the same level of security.
-
```

#### html2text {}

```diff
@@ -1,33 +1,25 @@
-Metadata-Version: 2.3 Name: REncrypt Version: 0.1.0 Classifier: Programming
-Language :: Rust Classifier: Programming Language :: Python :: Implementation
-:: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: License :: Apache-2.0 license License-File: LICENSE Summary: A
-Python encryption library implemented in Rust. It supports AEAD with AES-GCM
-and ChaCha20Poly1305. It uses ring crate to handle encryption. Keywords:
-cryptography,encryption,security,rust,speed Author-email: Radu Marias
-gmail.com> Requires-Python: >=3.8 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Project-URL: Homepage, https://github.com/
-radumarias/rencrypt-python Project-URL: Issues, https://github.com/radumarias/
-rencrypt-python/issues # REncrypt A Python encryption library implemented in
-Rust. It supports `AEAD` with `AES-GCM` and `ChaCha20Poly1305`. It uses [ring]
-(https://crates.io/crates/ring) to handle encryption. If offers slightly higher
-speed compared to other Python libs, especially for smaller chunks of data. The
-API also tries to be easy to use but it's more optimized for speed than
-usability. So if you want to achieve the highest possible encryption speed,
-consider giving it a try. # Benchmark Some benchmarks comparing to [PyFLocker]
-(https://github.com/arunanshub/pyflocker), which, from other implementations, I
-found to be the fastest. After this there is also comparison with other
-implementations. ## Buffer in memory This is useful when you keep a buffer, set
-your plaintext/ciphertext in there, and then encrypt/decrypt in-place that
-buffer. This is the most performant way to use it, because it does't copy any
-bytes nor allocate new memory. `REncrypt` is faster on small buffers, less than
-few MB, `PyFLocker` is comming closer for larger buffers. | Encrypt | Decrypt |
-| ------- | ------- | | ![Encrypt buffer](resources/charts/encrypt.png) | !
-[Decrypt buffer](resources/charts/decrypt.png) |
+# REncrypt A Python encryption library implemented in Rust. It supports `AEAD`
+with `AES-GCM` and `ChaCha20Poly1305`. It uses [ring](https://crates.io/crates/
+ring) to handle encryption. If offers slightly higher speed compared to other
+Python libs, especially for small chunks of data. The API also tries to be easy
+to use but it's more optimized for speed than usability. So if you want to
+achieve the highest possible encryption speed, consider giving it a try. #
+Benchmark Some benchmarks comparing to [PyFLocker](https://github.com/
+arunanshub/pyflocker), which, from other implementations, I found to be the
+fastest. After this there is also comparison with other implementations. ##
+Buffer in memory This is useful when you keep a buffer, set your plaintext/
+ciphertext in there, and then encrypt/decrypt in-place that buffer. This is the
+most performant way to use it, because it does't copy any bytes nor allocate
+new memory. `REncrypt` is faster on small buffers, less than few MB,
+`PyFLocker` is comming closer for larger buffers. | Encrypt seconds | Decrypt
+seconds | | --------------- | --------------- | | ![Encrypt buffer](https://
+github.com/radumarias/rencrypt-python/blob/main/resources/charts/
+encrypt.png?raw=true) | ![Decrypt buffer](https://github.com/radumarias/
+rencrypt-python/blob/main/resources/charts/decrypt.png?raw=true) |
 MMBB      EEnnccrryypptt sseeccoonnddss    DDeeccrryypptt sseeccoonnddss
         RREEnnccrryypptt PPyyFFLLoocckkeerr RREEnnccrryypptt PPyyFFLLoocckkeerr
 0.03125 0.00001  0.00091   0.00001  0.00004
 0.0625  0.00001  0.00005   0.00001  0.00004
 0.125   0.00002  0.00005   0.00003  0.00005
 0.25    0.00004  0.00008   0.00005  0.00009
 0.5     0.00010  0.00014   0.00011  0.00015
@@ -38,61 +30,63 @@
 16      0.00353  0.00393   0.00367  0.00617
 32      0.00678  0.00748   0.00749  0.01348
 64      0.01361  0.01461   0.01460  0.02697
 128     0.02923  0.03027   0.03134  0.05410
 256     0.06348  0.06188   0.06136  0.10417
 512     0.11782  0.13463   0.12090  0.21114
 1024    0.25001  0.24953   0.25377  0.42581
-## File | Encrypt | Decrypt | | ------- | ------- | | ![Encrypt file]
-(resources/charts/encrypt-file.png) | ![Decrypt buffer](resources/charts/
-encrypt-file.png) |
+## File | Encrypt seconds | Decrypt seconds | | --------------- | -------------
+-- | | ![Encrypt file](https://github.com/radumarias/rencrypt-python/blob/main/
+resources/charts/encrypt-file.png?raw=true) | ![Decrypt buffer](https://
+github.com/radumarias/rencrypt-python/blob/main/resources/charts/decrypt-
+file.png?raw=true) |
 MMBB       EEnnccrryypptt sseeccoonnddss    DDeeccrryypptt sseeccoonnddss
          RREEnnccrryypptt PPyyFFLLoocckkeerr RREEnnccrryypptt PPyyFFLLoocckkeerr
 0.031251 0.00010  0.00280   0.00004  0.00479
 0.062501 0.00009  0.00218   0.00005  0.00143
 0.125    0.00020  0.00212   0.00014  0.00129
 0.25     0.00034  0.00232   0.00020  0.00165
 0.5      0.00050  0.00232   0.00035  0.00181
 1        0.00087  0.00356   0.00065  0.00248
 2        0.00215  0.00484   0.00154  0.00363
-4        0.00361  0.00765   0.00301  0.00550
+4        0.00361  0.00765   0.00301  0.00736
 8        0.00688  0.01190   0.00621  0.00876
 16       0.01503  0.02097   0.01202  0.01583
 32       0.02924  0.03642   0.02563  0.02959
 64       0.05737  0.06473   0.04431  0.05287
 128      0.11098  0.12646   0.08944  0.09926
 256      0.22964  0.24716   0.17402  0.19420
 512      0.43506  0.46444   0.38143  0.38242
 1024     0.97147  0.95803   0.78137  0.87363
 2048     2.07143  2.10766   1.69471  2.99210
-4096     4.85395  4.69722   6.72873  4.50009
-8192     10.76984 11.76741  14.27756 9.66436
-16384    21.84490 26.27385  28.98916 19.08575
+4096     4.85395  4.69722   5.40580  8.73779
+8192     10.76984 11.76741  10.29253 21.00636
+16384    21.84490 26.27385  39.56230 43.55530
 # Usage There are three ways in which you can use the lib, the main difference
 is the speed, some offers an easier way to use it sacrificing performance. 1.
 **With a buffer in memory**: using `encrypt()`/`decrypt()`, is useful when you
 keep a buffer (or have it from somewhere), set your plaintext/ciphertext in
 there, and then encrypt/decrypt in-place that buffer. This is the most
 performant way to use it, because it does't copy any bytes nor allocate new
 memory. If you can directly collect the data to that buffer, like
 `buffered_reader.read_into()`, **this is the preffered way to go**. 2. **From
-some bytes to the buffer**: using `encrypt_into()`/`decrypt_to_buf()`, when you
+some bytes to the buffer**: using `encrypt_into()`/`decrypt_into()`, when you
 have some arbitrary `bytes` that you want to work with. It will first copy
 those bytes to the buffer then do the operation in-place in buffer. This is a
 bit slower, especially for large data, because it needs to copy the bytes to
 the buffer. 3. **From some bytes to another new bytes**: using `encrypt_from
 ()`/`decrypt_from()`, it doesn't use the buffer at all, you just got some bytes
 you want to work with and you receive back another new bytes. This is the
 slowest one because it needs to first allocate a buffer, copy the data to the
 buffer, perform the operation then return that buffer as bytes. It's the
 easiest to use but is not so performant. # Examples You can see more in
 [examples](https://github.com/radumarias/rencrypt-python/tree/main/examples)
 directory and in [bench.py](https://github.com/radumarias/rencrypt-python/tree/
 main/bench.py) which has some benchmarks. Here are few simple examples: ##
-Encrypt and decrypt with a buffer in memory `encrypt`/`decrypt` This is the
+Encrypt and decrypt with a buffer in memory `encrypt()`/`decrypt()` This is the
 most performant way to use it as it will not copy bytes to the buffer nor
 allocate new memory for plaintext and ciphertext. ```python from rencrypt
 import REncrypt, Cipher import os # You can use also other ciphers like `cipher
 = Cipher.ChaCha20Poly1305`. cipher = Cipher.AES256GCM key = cipher.generate_key
 () enc = REncrypt(cipher, key) # we get a buffer based on block len 4096
 plaintext # the actual buffer will be 28 bytes larger as in ciphertext we also
 include the tag and nonce plaintext_len, ciphertext_len, buf = enc.create_buf
@@ -104,86 +98,102 @@
 the data in parallel enc.copy_slice(plaintext, buf) # encrypt it, this will
 encrypt in-place the data in the buffer print("encryping...") ciphertext_len =
 enc.encrypt(buf, plaintext_len, 42, aad) cipertext = buf[:ciphertext_len] # you
 can do something with the ciphertext # decrypt it # if you need to copy
 ciphertext to buffer, we don't need to do it now as it's already in the buffer
 # enc.copy_slice(ciphertext, buf[:len(ciphertext)]) print("decryping...")
 plaintext_len = enc.decrypt(buf, ciphertext_len, 42, aad) plaintext2 = buf[:
-plaintext_len] assert plaintext == plaintext2 print("bye!") ``` You can use
-other ciphers like `cipher = Cipher.ChaCha20Poly1305`. ## Encrypt and decrypt a
-file ```python import errno import io import os from rencrypt import REncrypt,
-Cipher import hashlib def read_file_in_chunks(file_path, buf): with open
-(file_path, "rb") as file: buffered_reader = io.BufferedReader(file,
-buffer_size=len(buf)) while True: read = buffered_reader.readinto(buf) if read
-== 0: break yield read def calculate_file_hash(file_path): hash_algo =
-hashlib.sha256() with open(file_path, "rb") as f: for chunk in iter(lambda:
-f.read(4096), b""): hash_algo.update(chunk) return hash_algo.hexdigest() def
-compare_files_by_hash(file1, file2): return calculate_file_hash(file1) ==
-calculate_file_hash(file2) def silentremove(filename): try: os.remove(filename)
-except OSError as e: # this would be "except OSError, e:" before Python 2.6 if
-e.errno != errno.ENOENT: # errno.ENOENT = no such file or directory raise # re-
-raise exception if a different error occurred path_in = "/tmp/fin" path_out =
-"/tmp/fout.enc" chunk_len = 128 * 1024 key = os.urandom(32) cipher =
-Cipher.AES256GCM key = cipher.generate_key() enc = REncrypt(cipher, key)
-plaintext_len, _, buf = enc.create_buf(chunk_len) aad = b"AAD" # encrypt print
-("encryping...") silentremove(path_out) with open(path_out, "wb",
+plaintext_len] assert plaintext == plaintext2 # best practice, you should
+always zeroize the plaintext and key after you are done with them print("bye!")
+``` You can use other ciphers like `cipher = Cipher.ChaCha20Poly1305`. ##
+Encrypt and decrypt a file ```python import errno import io import os from
+pathlib import Path import shutil from rencrypt import REncrypt, Cipher import
+hashlib def read_file_in_chunks(file_path, buf): with open(file_path, "rb") as
+file: buffered_reader = io.BufferedReader(file, buffer_size=len(buf)) while
+True: read = buffered_reader.readinto(buf) if read == 0: break yield read def
+calculate_file_hash(file_path): hash_algo = hashlib.sha256() with open
+(file_path, "rb") as f: for chunk in iter(lambda: f.read(4096), b""):
+hash_algo.update(chunk) return hash_algo.hexdigest() def compare_files_by_hash
+(file1, file2): return calculate_file_hash(file1) == calculate_file_hash(file2)
+def silentremove(filename): try: os.remove(filename) except OSError as e: #
+this would be "except OSError, e:" before Python 2.6 if e.errno !=
+errno.ENOENT: # errno.ENOENT = no such file or directory raise # re-raise
+exception if a different error occurred def create_directory_in_home(dir_name):
+# Get the user's home directory home_dir = Path.home() # Create the full path
+for the new directory new_dir_path = home_dir / dir_name # Create the directory
+try: new_dir_path.mkdir(parents=True, exist_ok=True) except Exception as e:
+print(f"Error creating directory: {e}") return new_dir_path.absolute().__str__
+() def create_file_with_size(file_path_str, size_in_bytes): with open
+(file_path_str, "wb") as f: for _ in range(size_in_bytes // 4096): f.write
+(os.urandom(4096)) def delete_dir(path): if os.path.exists(path): shutil.rmtree
+(path) else: print(f"Directory {path} does not exist.") tmp_dir =
+create_directory_in_home("rencrypt_tmp") fin = tmp_dir + "/" + "fin" fout =
+tmp_dir + "/" + "fout.enc" create_file_with_size(fin, 42 * 1024 * 1024)
+chunk_len = 256 * 1024 key = os.urandom(32) cipher = Cipher.AES256GCM key =
+cipher.generate_key() enc = REncrypt(cipher, key) plaintext_len, _, buf =
+enc.create_buf(chunk_len) aad = b"AAD" # encrypt print("encryping...") with
+open(fout, "wb", buffering=plaintext_len) as file_out: i = 0 for read in
+read_file_in_chunks(fin, buf[:plaintext_len]): ciphertext_len = enc.encrypt
+(buf, read, i, aad) file_out.write(buf[:ciphertext_len]) i += 1 file_out.flush
+() # decrypt print("decryping...") tmp = fout + ".dec" with open(tmp, "wb",
 buffering=plaintext_len) as file_out: i = 0 for read in read_file_in_chunks
-(path_in, buf[:plaintext_len]): ciphertext_len = enc.encrypt(buf, read, i, aad)
-file_out.write(buf[:ciphertext_len]) i += 1 file_out.flush() # decrypt print
-("decryping...") tmp_path = "/tmp/fout.dec" with open(tmp_path, "wb",
-buffering=plaintext_len) as file_out: i = 0 for read in read_file_in_chunks
-(path_out, buf): plaintext_len2 = enc.decrypt(buf, read, i, aad) file_out.write
-(buf[:plaintext_len2]) i += 1 file_out.flush() compare_files_by_hash(path_in,
-tmp_path) silentremove(tmp_path) silentremove(path_out) print("bye!") ``` ##
-Encrypt and decrypt from some bytes to the buffer `encrypt_into`/`decrypt_into`
-or `encrypt_into1`/`decrypt_into1` This is a bit slower than handling data only
-via the buffer, especially for large plaintext, but there are situations when
-you can't directly collect the data to the buffer but have some `bytes` from
-somewhere else. For `encrypt_into`/`encrypt_into` the plaintext is `bytes`.
-```python from rencrypt import REncrypt, Cipher import os # You can use also
-other ciphers like `cipher = Cipher.ChaCha20Poly1305`. cipher =
+(fout, buf): plaintext_len2 = enc.decrypt(buf, read, i, aad) file_out.write(buf
+[:plaintext_len2]) i += 1 file_out.flush() compare_files_by_hash(fin, tmp)
+delete_dir(tmp_dir) # best practice, you should always zeroize the plaintext
+and key after you are done with them print("bye!") ``` ## Encrypt and decrypt
+from some bytes to the buffer `encrypt_into()`/`decrypt_into()` or
+`encrypt_into1()`/`decrypt_into1()` This is a bit slower than handling data
+only via the buffer, especially for large plaintext, but there are situations
+when you can't directly collect the data to the buffer but have some `bytes`
+from somewhere else. For `encrypt_into()`/`decrypt_into()` the plaintext is
+`bytes`. ```python from rencrypt import REncrypt, Cipher import os # You can
+use also other ciphers like `cipher = Cipher.ChaCha20Poly1305`. cipher =
 Cipher.AES256GCM key = cipher.generate_key() enc = REncrypt(cipher, key) # we
 get a buffer based on block len 4096 plaintext # the actual buffer will be 28
 bytes larger as in ciphertext we also include the tag and nonce plaintext_len,
 ciphertext_len, buf = enc.create_buf(4096) aad = b"AAD" plaintext = bytes
 (os.urandom(plaintext_len)) # encrypt it, after this will have the ciphertext
 in the buffer print("encryping...") ciphertext_len = enc.encrypt_into
 (plaintext, buf, 42, aad) cipertext = bytes(buf[:ciphertext_len]) # decrypt it
 print("decryping...") plaintext_len = enc.decrypt_into(cipertext, buf, 42, aad)
-plaintext2 = buf[:plaintext_len] assert plaintext == plaintext2 print("bye!")
-``` For `encrypt_into1`/`encrypt_into1` the only difference is that the
-plaintext is `bytearray`. ## Encrypt and decrypt from some bytes to another new
-bytes, without using the buffer `encrypt_from`/`decrypt_from` or
-`encrypt_from2`/`decrypt_from2` This is the slowest option, especially for
-large plaintext, because it allocates new memory for the ciphertext on encrypt
-and plaintext on decrypt. For `encrypt_from`/`decrypt_from` the plaintext is
-`bytes`. ```python from rencrypt import REncrypt, Cipher import os # You can
-use also other ciphers like `cipher = Cipher.ChaCha20Poly1305`.# You can use
-also other ciphers like `cipher = Cipher.ChaCha20Poly1305`. cipher =
-Cipher.AES256GCM key = cipher.generate_key() enc = REncrypt(cipher, key) aad =
-b"AAD" plaintext = os.urandom(4096) # encrypt it, this will return the
-ciphertext print("encryping...") ciphertext = enc.encrypt_from(plaintext, 42,
-aad) # decrypt it print("decryping...") plaintext2 = enc.decrypt_from
-(ciphertext, 42, aad) assert plaintext == plaintext2 print("bye!") ``` For
-`encrypt_from2`/`decrypt_from2` the only difference is that the plaintext is
-`bytearray`. # Building from source ## Browser [![Open in Gitpod](https://
-gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/
-radumarias/rencrypt-python) [![Open Rustlings On Codespaces](https://
-github.com/codespaces/badge.svg)](https://github.com/codespaces/new/
-?repo=radumarias%2Frencrypt-python&ref=main) ## Geting sources from GitHub
-```bash git clone https://github.com/radumarias/rencrypt-python && cd rencrypt-
-python ``` ## Compile and run ```bash curl --proto '=https' --tlsv1.2 -sSf
-https://sh.rustup.rs | sh ``` To configure your current shell, you need to
-source the corresponding env file under $HOME/.cargo. This is usually done by
-running one of the following (note the leading DOT): ```bash . "$HOME/.cargo/
-env" ``` ``` python -m venv .env source .env/bin/activate pip install maturin
-maturin develop python python bench.py ``` # More benchmarks ## Different ways
-to use the lib | Encrypt | Decrypt | | ------- | ------- | | ![Encrypt buffer]
-(resources/charts/encrypt-all.png) | ![Decrypt buffer](resources/charts/
-decrypt-all.png) |
+plaintext2 = buf[:plaintext_len] assert plaintext == plaintext2 # best
+practice, you should always zeroize the plaintext and key after you are done
+with them print("bye!") ``` For `encrypt_into1()`/`decrypt_into1()` the only
+difference is that the input is `bytearray`. ## Encrypt and decrypt from some
+bytes to another new bytes, without using the buffer `encrypt_from()`/
+`decrypt_from()` or `encrypt_from1()`/`decrypt_from1()` This is the slowest
+option, especially for large plaintext, because it allocates new memory for the
+ciphertext on encrypt and plaintext on decrypt. For `encrypt_from()`/
+`decrypt_from()` the plaintext is `bytes`. ```python from rencrypt import
+REncrypt, Cipher import os # You can use also other ciphers like `cipher =
+Cipher.ChaCha20Poly1305`.# You can use also other ciphers like `cipher =
+Cipher.ChaCha20Poly1305`. cipher = Cipher.AES256GCM key = cipher.generate_key()
+enc = REncrypt(cipher, key) aad = b"AAD" plaintext = os.urandom(4096) # encrypt
+it, this will return the ciphertext print("encryping...") ciphertext =
+enc.encrypt_from(plaintext, 42, aad) # decrypt it print("decryping...")
+plaintext2 = enc.decrypt_from(ciphertext, 42, aad) assert plaintext ==
+plaintext2 # best practice, you should always zeroize the plaintext and key
+after you are done with them print("bye!") ``` For `encrypt_from1()`/
+`decrypt_from1()` the only difference is that the input is `bytearray`. #
+Building from source ## Browser [![Open in Gitpod](https://gitpod.io/button/
+open-in-gitpod.svg)](https://gitpod.io/#https://github.com/radumarias/rencrypt-
+python) [![Open Rustlings On Codespaces](https://github.com/codespaces/
+badge.svg)](https://github.com/codespaces/new/?repo=radumarias%2Frencrypt-
+python&ref=main) ## Geting sources from GitHub ```bash git clone https://
+github.com/radumarias/rencrypt-python && cd rencrypt-python ``` ## Compile and
+run ```bash curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh ```
+To configure your current shell, you need to source the corresponding env file
+under $HOME/.cargo. This is usually done by running one of the following (note
+the leading DOT): ```bash . "$HOME/.cargo/env" ``` ``` python -m venv .env
+source .env/bin/activate pip install maturin maturin develop python bench.py
+``` # More benchmarks ## Different ways to use the lib | Encrypt | Decrypt | |
+------- | ------- | | ![Encrypt buffer](https://github.com/radumarias/rencrypt-
+python/blob/main/resources/charts/encrypt-all.png?raw=true) | ![Decrypt buffer]
+(https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/
+decrypt-all.png?raw=true) |
         EEnnccrryypptt sseeccoonnddss                                          DDeeccrryypptt sseeccoonnddss
 MMBB      RREEnnccrryypptt PPyyFFLLoocckkeerr   RREEnnccrryypptt     RREEnnccrryypptt     PPyyFFLLoocckkeerr RREEnnccrryypptt PPyyFFLLoocckkeerr   RREEnnccrryypptt     RREEnnccrryypptt     PPyyFFLLoocckkeerr
         eennccrryypptt  uuppddaattee__iinnttoo eennccrryypptt__iinnttoo eennccrryypptt__ffrroomm uuppddaattee    ddeeccrryypptt  uuppddaattee__iinnttoo ddeeccrryypptt__iinnttoo ddeeccrryypptt__ffrroomm uuppddaattee
 0.03125 0.00001  0.00091     0.00001      0.00002      0.00009   0.00001  0.00004     0.00001      0.00003      0.00005
 0.0625  0.00001  0.00005     0.00002      0.00002      0.00005   0.00001  0.00004     0.00002      0.00004      0.00008
 0.125   0.00002  0.00005     0.00003      0.00005      0.00011   0.00003  0.00005     0.00003      0.00007      0.00013
 0.25    0.00004  0.00008     0.00007      0.00009      0.00019   0.00005  0.00009     0.00007      0.00016      0.00023
@@ -198,19 +208,20 @@
 128     0.02923  0.03027     0.03343      0.06805      0.10362   0.03134  0.05410     0.03558      0.06955      0.11380
 256     0.06348  0.06188     0.07303      0.13003      0.20911   0.06136  0.10417     0.07572      0.13733      0.20828
 512     0.11782  0.13463     0.14283      0.26799      0.41929   0.12090  0.21114     0.14434      0.25771      0.41463
 1024    0.25001  0.24953     0.28912      0.51228      0.82370   0.25377  0.42581     0.29795      0.53807      0.82588
 ## Speed throughput `256KB` seems to be the sweet spot for buffer size that
 offers the max `MB/s` speed for encryption, on benchmarks that seem to be the
 case. We performed `10.000` encryption operations for each size varying from
-`1KB` to `16MB`. ![Speed throughput](resources/charts/speed-throughput.png) |
-MB | MB/s | | ----- | ------- | | 0.0009765625 | 1083 | | 0.001953125 | 1580 |
-| 0.00390625 | 2158 | | 0.0078125 | 2873 | | 0.015625 | 3348 | | 0.03125 | 3731
-| | 0.0625 | 4053 | | 0.125 | 4156 | | 0.25 | 4247 | | 0.5 | 4182 | | 1.0 |
-3490 | | 2.0 | 3539 | | 4.0 | 3684 | | 8.0 | 3787 | | 16.0 | 3924 | # For the
-future - Add more `AES` ciphers like `AES128-GCM` and `AES-GCM-SIV` - Add other
-encryption providers like [RustCrypto](https://github.com/RustCrypto/traits)
-and [libsodium](https://crates.io/crates/sodiumoxide) - Maybe add support for
-`RSA` and `Elliptic-curve cryptography` - Saving and loading keys from file #
+`1KB` to `16MB`. ![Speed throughput](https://github.com/radumarias/rencrypt-
+python/blob/main/resources/charts/speed-throughput.png?raw=true) | MB | MB/s |
+| ----- | ------- | | 0.0009765625 | 1083 | | 0.001953125 | 1580 | | 0.00390625
+| 2158 | | 0.0078125 | 2873 | | 0.015625 | 3348 | | 0.03125 | 3731 | | 0.0625 |
+4053 | | 0.125 | 4156 | | 0.25 | 4247 | | 0.5 | 4182 | | 1.0 | 3490 | | 2.0 |
+3539 | | 4.0 | 3684 | | 8.0 | 3787 | | 16.0 | 3924 | # For the future - Add
+more `AES` ciphers like `AES128-GCM` and `AES-GCM-SIV` - Add other encryption
+providers like [RustCrypto](https://github.com/RustCrypto/traits) and
+[libsodium](https://crates.io/crates/sodiumoxide) - Maybe add support for `RSA`
+and `Elliptic-curve cryptography` - Saving and loading keys from file #
 Considerations This lib hasn't been audited, but it mostly wraps `ring` crate
 which is a well known library, so in principle it should offer the same level
 of security.
```

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/REncrypt-0.1.0.dist-info/license_files/LICENSE` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/REncrypt-0.1.5.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/maturin/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/maturin/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/maturin/__main__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/maturin/__main__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/maturin/import_hook.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/maturin/import_hook.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/maturin-1.5.1.dist-info/METADATA` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/maturin-1.5.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/maturin-1.5.1.dist-info/RECORD` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/maturin-1.5.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/__main__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/__pip-runner__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/build_env.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cache.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/autocompletion.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/base_command.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/cmdoptions.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/command_context.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/main.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/main_parser.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/parser.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/progress_bars.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/req_command.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/cli/spinners.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/cache.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/check.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/completion.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/configuration.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/debug.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/download.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/freeze.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/hash.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/help.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/index.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/inspect.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/install.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/list.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/search.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/show.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/uninstall.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/commands/wheel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/configuration.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/distributions/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/distributions/base.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/distributions/installed.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/distributions/sdist.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/distributions/wheel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/exceptions.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/index/collector.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/index/package_finder.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/index/sources.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/locations/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/locations/_distutils.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/locations/_sysconfig.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/locations/base.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/metadata/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/metadata/_json.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/metadata/base.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/metadata/importlib/_compat.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/metadata/importlib/_dists.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/metadata/importlib/_envs.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/metadata/pkg_resources.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/candidate.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/direct_url.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/format_control.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/index.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/installation_report.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/link.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/scheme.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/search_scope.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/selection_prefs.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/target_python.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/models/wheel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/network/auth.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/network/cache.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/network/download.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/network/lazy_wheel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/network/session.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/network/utils.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/network/xmlrpc.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/build_tracker.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/metadata.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/metadata_editable.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/wheel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/wheel_editable.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/check.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/freeze.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/install/editable_legacy.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/install/wheel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/operations/prepare.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/pyproject.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/req/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/req/constructors.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/req/req_file.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/req/req_install.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/req/req_set.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/req/req_uninstall.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/base.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/legacy/resolver.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/base.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/self_outdated_check.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/_jaraco_text.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/_log.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/appdirs.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/compat.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/compatibility_tags.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/deprecation.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/direct_url_helpers.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/egg_link.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/encoding.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/entrypoints.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/filesystem.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/filetypes.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/glibc.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/hashes.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/logging.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/misc.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/models.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/packaging.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/setuptools_build.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/subprocess.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/temp_dir.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/unpacking.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/urls.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/virtualenv.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/utils/wheel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/vcs/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/vcs/bazaar.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/vcs/git.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/vcs/mercurial.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/vcs/subversion.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/vcs/versioncontrol.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_internal/wheel_builder.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/adapter.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/cache.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/controller.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/serialize.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/certifi/cacert.pem` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/certifi/core.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/big5freq.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/big5prober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/chardistribution.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/charsetprober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/cp949prober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/enums.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/escprober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/escsm.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/eucjpprober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euckrfreq.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euckrprober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euctwfreq.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euctwprober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/gb2312freq.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/gb2312prober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/hebrewprober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/jisfreq.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/johabfreq.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/johabprober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/jpcntx.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langthaimodel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/latin1prober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/macromanprober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/mbcssm.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/metadata/languages.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/sjisprober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/universaldetector.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/utf1632prober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/utf8prober.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/ansi.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/ansitowin32.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/initialise.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/utils.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/win32.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/winterm.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/compat.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/database.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/index.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/locators.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/manifest.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/markers.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/metadata.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/resources.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/scripts.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/t32.exe` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/t64-arm.exe` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/t64.exe` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/util.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/version.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/w32.exe` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/w64-arm.exe` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/w64.exe` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/wheel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distro/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/distro/distro.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/idna/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/idna/codec.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/idna/core.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/idna/idnadata.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/idna/intranges.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/idna/uts46data.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/exceptions.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/ext.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/fallback.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/__about__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/_manylinux.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/_musllinux.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/_structures.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/markers.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/requirements.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/specifiers.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/tags.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/utils.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/version.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pkg_resources/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/__main__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/android.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/api.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/macos.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/unix.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/windows.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/cmdline.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/console.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/filter.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/filters/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatter.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/groff.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/html.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/img.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/irc.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/latex.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/other.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/svg.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexer.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexers/python.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/modeline.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/plugin.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/regexopt.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/scanner.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/sphinxext.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/style.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/styles/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/token.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/unistring.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/util.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/actions.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/common.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/core.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/exceptions.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/helpers.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/results.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/testing.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/unicode.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/util.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/_internal_utils.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/adapters.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/api.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/auth.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/certs.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/compat.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/cookies.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/exceptions.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/help.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/hooks.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/models.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/packages.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/sessions.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/status_codes.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/structures.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/requests/utils.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/providers.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/reporters.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/resolvers.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/structs.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/__main__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_cell_widths.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_emoji_codes.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_emoji_replace.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_export_format.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_fileno.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_inspect.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_log_render.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_loop.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_null_file.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_palettes.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_ratio.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_spinners.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_win32_console.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_windows.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_windows_renderer.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_wrap.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/abc.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/align.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/ansi.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/bar.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/box.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/cells.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/color.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/color_triplet.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/columns.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/console.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/constrain.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/containers.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/control.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/default_styles.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/diagnose.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/emoji.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/errors.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/file_proxy.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/filesize.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/highlighter.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/json.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/jupyter.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/layout.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/live.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/live_render.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/logging.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/markup.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/measure.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/padding.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/pager.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/palette.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/panel.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/pretty.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/progress.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/progress_bar.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/prompt.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/protocol.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/repr.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/rule.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/scope.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/screen.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/segment.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/spinner.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/status.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/style.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/styled.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/syntax.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/table.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/terminal_theme.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/text.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/theme.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/traceback.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/rich/tree.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/six.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/_asyncio.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/_utils.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/after.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/before.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/before_sleep.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/nap.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/retry.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/stop.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/wait.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tomli/_parser.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/tomli/_re.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_api.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_api.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_macos.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_macos.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_openssl.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_openssl.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_ssl_constants.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_ssl_constants.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_windows.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/truststore/_windows.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/typing_extensions.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/_collections.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/connection.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/connectionpool.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/exceptions.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/fields.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/filepost.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/six.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/poolmanager.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/request.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/response.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/connection.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/proxy.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/request.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/response.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/retry.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/timeout.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/url.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/wait.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/__init__.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/labels.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/mklabels.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/tests.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/AUTHORS.txt` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/LICENSE.txt` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/METADATA` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/RECORD` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/pip-24.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/METADATA` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/RECORD` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/license_files/LICENSE` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/procmaps-0.6.5.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.github/workflows/CI.yml` & `REncrypt-0.1.5/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/.gitignore` & `REncrypt-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/LICENSE` & `REncrypt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/README.md` & `REncrypt-0.1.5/.env/lib64/python3.12/site-packages/REncrypt-0.1.5.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.3
+Name: REncrypt
+Version: 0.1.5
+Classifier: Programming Language :: Rust
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: License :: OSI Approved :: Apache Software License
+License-File: LICENSE
+Summary: A Python encryption library implemented in Rust. It supports AEAD with AES-GCM and ChaCha20Poly1305. It uses ring crate to handle encryption.
+Keywords: cryptography,encryption,security,rust,speed
+Author-email: Radu Marias <radumarias@gmail.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Homepage, https://github.com/radumarias/rencrypt-python
+Project-URL: Issues, https://github.com/radumarias/rencrypt-python/issues
+
 # REncrypt
 
 A Python encryption library implemented in Rust. It supports `AEAD` with `AES-GCM` and `ChaCha20Poly1305`. It uses [ring](https://crates.io/crates/ring) to handle encryption.  
 If offers slightly higher speed compared to other Python libs, especially for small chunks of data. The API also tries to be easy to use but it's more optimized for speed than usability.
 
 So if you want to achieve the highest possible encryption speed, consider giving it a try.
 
@@ -12,15 +28,15 @@
 ## Buffer in memory
 
 This is useful when you keep a buffer, set your plaintext/ciphertext in there, and then encrypt/decrypt in-place that buffer. This is the most performant way to use it, because it does't copy any bytes nor allocate new memory.  
 `REncrypt` is faster on small buffers, less than few MB, `PyFLocker` is comming closer for larger buffers.
 
 | Encrypt seconds | Decrypt seconds |
 | --------------- | --------------- |
-| ![Encrypt buffer](resources/charts/encrypt.png) | ![Decrypt buffer](resources/charts/decrypt.png) |
+| ![Encrypt buffer](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/encrypt.png?raw=true) | ![Decrypt buffer](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/decrypt.png?raw=true) |
 
 
 <table>
     <thead>
         <tr>
             <th rowspan=2>MB</th>
             <th colspan=2>Encrypt seconds</th>
@@ -149,15 +165,15 @@
     </tbody>
 </table>
 
 ## File
 
 | Encrypt seconds | Decrypt seconds |
 | --------------- | --------------- |
-| ![Encrypt file](resources/charts/encrypt-file.png) | ![Decrypt buffer](resources/charts/decrypt-file.png) |
+| ![Encrypt file](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/encrypt-file.png?raw=true) | ![Decrypt buffer](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/decrypt-file.png?raw=true) |
 
 <table>
     <thead>
         <tr>
             <th rowspan=2>MB</th>
             <th colspan=2>Encrypt seconds</th>
             <th colspan=2>Decrypt seconds</th>
@@ -590,15 +606,15 @@
 
 # More benchmarks
 
 ## Different ways to use the lib
 
 | Encrypt | Decrypt |
 | ------- | ------- |
-| ![Encrypt buffer](resources/charts/encrypt-all.png) | ![Decrypt buffer](resources/charts/decrypt-all.png) |
+| ![Encrypt buffer](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/encrypt-all.png?raw=true) | ![Decrypt buffer](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/decrypt-all.png?raw=true) |
 
 
 <table>
     <thead>
         <tr>
             <th rowspan=2>MB</th>
             <th colspan=5>Encrypt seconds</th>
@@ -830,15 +846,15 @@
 </table>
 
 ## Speed throughput
 
 `256KB` seems to be the sweet spot for buffer size that offers the max `MB/s` speed for encryption, on benchmarks that seem to be the case.
 We performed `10.000` encryption operations for each size varying from `1KB` to `16MB`.
 
-![Speed throughput](resources/charts/speed-throughput.png)
+![Speed throughput](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/speed-throughput.png?raw=true)
 
 | MB    | MB/s |
 | ----- | ------- |
 | 0.0009765625 | 1083 |
 | 0.001953125 | 1580 |
 | 0.00390625 | 2158 |
 | 0.0078125 | 2873 |
@@ -860,7 +876,8 @@
 - Add other encryption providers like [RustCrypto](https://github.com/RustCrypto/traits) and [libsodium](https://crates.io/crates/sodiumoxide)
 - Maybe add support for `RSA` and `Elliptic-curve cryptography`
 - Saving and loading keys from file
 
 # Considerations
 
 This lib hasn't been audited, but it mostly wraps `ring` crate which is a well known library, so in principle it should offer the same level of security.
+
```

#### html2text {}

```diff
@@ -1,23 +1,36 @@
-# REncrypt A Python encryption library implemented in Rust. It supports `AEAD`
-with `AES-GCM` and `ChaCha20Poly1305`. It uses [ring](https://crates.io/crates/
-ring) to handle encryption. If offers slightly higher speed compared to other
-Python libs, especially for small chunks of data. The API also tries to be easy
-to use but it's more optimized for speed than usability. So if you want to
-achieve the highest possible encryption speed, consider giving it a try. #
-Benchmark Some benchmarks comparing to [PyFLocker](https://github.com/
-arunanshub/pyflocker), which, from other implementations, I found to be the
-fastest. After this there is also comparison with other implementations. ##
-Buffer in memory This is useful when you keep a buffer, set your plaintext/
-ciphertext in there, and then encrypt/decrypt in-place that buffer. This is the
-most performant way to use it, because it does't copy any bytes nor allocate
-new memory. `REncrypt` is faster on small buffers, less than few MB,
-`PyFLocker` is comming closer for larger buffers. | Encrypt seconds | Decrypt
-seconds | | --------------- | --------------- | | ![Encrypt buffer](resources/
-charts/encrypt.png) | ![Decrypt buffer](resources/charts/decrypt.png) |
+Metadata-Version: 2.3 Name: REncrypt Version: 0.1.5 Classifier: Programming
+Language :: Rust Classifier: Programming Language :: Python :: Implementation
+:: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: License :: OSI Approved :: Apache Software License License-File:
+LICENSE Summary: A Python encryption library implemented in Rust. It supports
+AEAD with AES-GCM and ChaCha20Poly1305. It uses ring crate to handle
+encryption. Keywords: cryptography,encryption,security,rust,speed Author-email:
+Radu Marias
+gmail.com> Requires-Python: >=3.8 Description-Content-Type: text/markdown;
+charset=UTF-8; variant=GFM Project-URL: Homepage, https://github.com/
+radumarias/rencrypt-python Project-URL: Issues, https://github.com/radumarias/
+rencrypt-python/issues # REncrypt A Python encryption library implemented in
+Rust. It supports `AEAD` with `AES-GCM` and `ChaCha20Poly1305`. It uses [ring]
+(https://crates.io/crates/ring) to handle encryption. If offers slightly higher
+speed compared to other Python libs, especially for small chunks of data. The
+API also tries to be easy to use but it's more optimized for speed than
+usability. So if you want to achieve the highest possible encryption speed,
+consider giving it a try. # Benchmark Some benchmarks comparing to [PyFLocker]
+(https://github.com/arunanshub/pyflocker), which, from other implementations, I
+found to be the fastest. After this there is also comparison with other
+implementations. ## Buffer in memory This is useful when you keep a buffer, set
+your plaintext/ciphertext in there, and then encrypt/decrypt in-place that
+buffer. This is the most performant way to use it, because it does't copy any
+bytes nor allocate new memory. `REncrypt` is faster on small buffers, less than
+few MB, `PyFLocker` is comming closer for larger buffers. | Encrypt seconds |
+Decrypt seconds | | --------------- | --------------- | | ![Encrypt buffer]
+(https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/
+encrypt.png?raw=true) | ![Decrypt buffer](https://github.com/radumarias/
+rencrypt-python/blob/main/resources/charts/decrypt.png?raw=true) |
 MMBB      EEnnccrryypptt sseeccoonnddss    DDeeccrryypptt sseeccoonnddss
         RREEnnccrryypptt PPyyFFLLoocckkeerr RREEnnccrryypptt PPyyFFLLoocckkeerr
 0.03125 0.00001  0.00091   0.00001  0.00004
 0.0625  0.00001  0.00005   0.00001  0.00004
 0.125   0.00002  0.00005   0.00003  0.00005
 0.25    0.00004  0.00008   0.00005  0.00009
 0.5     0.00010  0.00014   0.00011  0.00015
@@ -29,16 +42,18 @@
 32      0.00678  0.00748   0.00749  0.01348
 64      0.01361  0.01461   0.01460  0.02697
 128     0.02923  0.03027   0.03134  0.05410
 256     0.06348  0.06188   0.06136  0.10417
 512     0.11782  0.13463   0.12090  0.21114
 1024    0.25001  0.24953   0.25377  0.42581
 ## File | Encrypt seconds | Decrypt seconds | | --------------- | -------------
--- | | ![Encrypt file](resources/charts/encrypt-file.png) | ![Decrypt buffer]
-(resources/charts/decrypt-file.png) |
+-- | | ![Encrypt file](https://github.com/radumarias/rencrypt-python/blob/main/
+resources/charts/encrypt-file.png?raw=true) | ![Decrypt buffer](https://
+github.com/radumarias/rencrypt-python/blob/main/resources/charts/decrypt-
+file.png?raw=true) |
 MMBB       EEnnccrryypptt sseeccoonnddss    DDeeccrryypptt sseeccoonnddss
          RREEnnccrryypptt PPyyFFLLoocckkeerr RREEnnccrryypptt PPyyFFLLoocckkeerr
 0.031251 0.00010  0.00280   0.00004  0.00479
 0.062501 0.00009  0.00218   0.00005  0.00143
 0.125    0.00020  0.00212   0.00014  0.00129
 0.25     0.00034  0.00232   0.00020  0.00165
 0.5      0.00050  0.00232   0.00035  0.00181
@@ -178,16 +193,18 @@
 github.com/radumarias/rencrypt-python && cd rencrypt-python ``` ## Compile and
 run ```bash curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh ```
 To configure your current shell, you need to source the corresponding env file
 under $HOME/.cargo. This is usually done by running one of the following (note
 the leading DOT): ```bash . "$HOME/.cargo/env" ``` ``` python -m venv .env
 source .env/bin/activate pip install maturin maturin develop python bench.py
 ``` # More benchmarks ## Different ways to use the lib | Encrypt | Decrypt | |
-------- | ------- | | ![Encrypt buffer](resources/charts/encrypt-all.png) | !
-[Decrypt buffer](resources/charts/decrypt-all.png) |
+------- | ------- | | ![Encrypt buffer](https://github.com/radumarias/rencrypt-
+python/blob/main/resources/charts/encrypt-all.png?raw=true) | ![Decrypt buffer]
+(https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/
+decrypt-all.png?raw=true) |
         EEnnccrryypptt sseeccoonnddss                                          DDeeccrryypptt sseeccoonnddss
 MMBB      RREEnnccrryypptt PPyyFFLLoocckkeerr   RREEnnccrryypptt     RREEnnccrryypptt     PPyyFFLLoocckkeerr RREEnnccrryypptt PPyyFFLLoocckkeerr   RREEnnccrryypptt     RREEnnccrryypptt     PPyyFFLLoocckkeerr
         eennccrryypptt  uuppddaattee__iinnttoo eennccrryypptt__iinnttoo eennccrryypptt__ffrroomm uuppddaattee    ddeeccrryypptt  uuppddaattee__iinnttoo ddeeccrryypptt__iinnttoo ddeeccrryypptt__ffrroomm uuppddaattee
 0.03125 0.00001  0.00091     0.00001      0.00002      0.00009   0.00001  0.00004     0.00001      0.00003      0.00005
 0.0625  0.00001  0.00005     0.00002      0.00002      0.00005   0.00001  0.00004     0.00002      0.00004      0.00008
 0.125   0.00002  0.00005     0.00003      0.00005      0.00011   0.00003  0.00005     0.00003      0.00007      0.00013
 0.25    0.00004  0.00008     0.00007      0.00009      0.00019   0.00005  0.00009     0.00007      0.00016      0.00023
@@ -202,19 +219,20 @@
 128     0.02923  0.03027     0.03343      0.06805      0.10362   0.03134  0.05410     0.03558      0.06955      0.11380
 256     0.06348  0.06188     0.07303      0.13003      0.20911   0.06136  0.10417     0.07572      0.13733      0.20828
 512     0.11782  0.13463     0.14283      0.26799      0.41929   0.12090  0.21114     0.14434      0.25771      0.41463
 1024    0.25001  0.24953     0.28912      0.51228      0.82370   0.25377  0.42581     0.29795      0.53807      0.82588
 ## Speed throughput `256KB` seems to be the sweet spot for buffer size that
 offers the max `MB/s` speed for encryption, on benchmarks that seem to be the
 case. We performed `10.000` encryption operations for each size varying from
-`1KB` to `16MB`. ![Speed throughput](resources/charts/speed-throughput.png) |
-MB | MB/s | | ----- | ------- | | 0.0009765625 | 1083 | | 0.001953125 | 1580 |
-| 0.00390625 | 2158 | | 0.0078125 | 2873 | | 0.015625 | 3348 | | 0.03125 | 3731
-| | 0.0625 | 4053 | | 0.125 | 4156 | | 0.25 | 4247 | | 0.5 | 4182 | | 1.0 |
-3490 | | 2.0 | 3539 | | 4.0 | 3684 | | 8.0 | 3787 | | 16.0 | 3924 | # For the
-future - Add more `AES` ciphers like `AES128-GCM` and `AES-GCM-SIV` - Add other
-encryption providers like [RustCrypto](https://github.com/RustCrypto/traits)
-and [libsodium](https://crates.io/crates/sodiumoxide) - Maybe add support for
-`RSA` and `Elliptic-curve cryptography` - Saving and loading keys from file #
+`1KB` to `16MB`. ![Speed throughput](https://github.com/radumarias/rencrypt-
+python/blob/main/resources/charts/speed-throughput.png?raw=true) | MB | MB/s |
+| ----- | ------- | | 0.0009765625 | 1083 | | 0.001953125 | 1580 | | 0.00390625
+| 2158 | | 0.0078125 | 2873 | | 0.015625 | 3348 | | 0.03125 | 3731 | | 0.0625 |
+4053 | | 0.125 | 4156 | | 0.25 | 4247 | | 0.5 | 4182 | | 1.0 | 3490 | | 2.0 |
+3539 | | 4.0 | 3684 | | 8.0 | 3787 | | 16.0 | 3924 | # For the future - Add
+more `AES` ciphers like `AES128-GCM` and `AES-GCM-SIV` - Add other encryption
+providers like [RustCrypto](https://github.com/RustCrypto/traits) and
+[libsodium](https://crates.io/crates/sodiumoxide) - Maybe add support for `RSA`
+and `Elliptic-curve cryptography` - Saving and loading keys from file #
 Considerations This lib hasn't been audited, but it mostly wraps `ring` crate
 which is a well known library, so in principle it should offer the same level
 of security.
```

### Comparing `REncrypt-0.1.0/bench.py` & `REncrypt-0.1.5/bench.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/benches/parallel_copy.rs` & `REncrypt-0.1.5/benches/parallel_copy.rs`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/examples/encrypt.py` & `REncrypt-0.1.5/examples/encrypt.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/examples/encrypt_file.py` & `REncrypt-0.1.5/examples/encrypt_file.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/examples/encrypt_from.py` & `REncrypt-0.1.5/examples/encrypt_from.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/examples/encrypt_into.py` & `REncrypt-0.1.5/examples/encrypt_into.py`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/resources/charts/decrypt-all.png` & `REncrypt-0.1.5/resources/charts/decrypt-all.png`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/resources/charts/decrypt-file.png` & `REncrypt-0.1.5/resources/charts/decrypt-file.png`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/resources/charts/decrypt.png` & `REncrypt-0.1.5/resources/charts/decrypt.png`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/resources/charts/encrypt-all.png` & `REncrypt-0.1.5/resources/charts/encrypt-all.png`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/resources/charts/encrypt-file.png` & `REncrypt-0.1.5/resources/charts/encrypt-file.png`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/resources/charts/encrypt.png` & `REncrypt-0.1.5/resources/charts/encrypt.png`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/resources/charts/speed-throughput.png` & `REncrypt-0.1.5/resources/charts/speed-throughput.png`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/src/lib.rs` & `REncrypt-0.1.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/Cargo.lock` & `REncrypt-0.1.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -589,15 +589,15 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rencrypt"
-version = "0.1.0"
+version = "0.1.5"
 dependencies = [
  "blake3",
  "criterion",
  "hex",
  "pyo3",
  "rand",
  "rand_chacha",
```

### Comparing `REncrypt-0.1.0/pyproject.toml` & `REncrypt-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `REncrypt-0.1.0/PKG-INFO` & `REncrypt-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: REncrypt
-Version: 0.1.0
+Version: 0.1.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: Apache Software License
 License-File: LICENSE
 Summary: A Python encryption library implemented in Rust. It supports AEAD with AES-GCM and ChaCha20Poly1305. It uses ring crate to handle encryption.
 Keywords: cryptography,encryption,security,rust,speed
@@ -28,15 +28,15 @@
 ## Buffer in memory
 
 This is useful when you keep a buffer, set your plaintext/ciphertext in there, and then encrypt/decrypt in-place that buffer. This is the most performant way to use it, because it does't copy any bytes nor allocate new memory.  
 `REncrypt` is faster on small buffers, less than few MB, `PyFLocker` is comming closer for larger buffers.
 
 | Encrypt seconds | Decrypt seconds |
 | --------------- | --------------- |
-| ![Encrypt buffer](resources/charts/encrypt.png) | ![Decrypt buffer](resources/charts/decrypt.png) |
+| ![Encrypt buffer](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/encrypt.png?raw=true) | ![Decrypt buffer](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/decrypt.png?raw=true) |
 
 
 <table>
     <thead>
         <tr>
             <th rowspan=2>MB</th>
             <th colspan=2>Encrypt seconds</th>
@@ -165,15 +165,15 @@
     </tbody>
 </table>
 
 ## File
 
 | Encrypt seconds | Decrypt seconds |
 | --------------- | --------------- |
-| ![Encrypt file](resources/charts/encrypt-file.png) | ![Decrypt buffer](resources/charts/decrypt-file.png) |
+| ![Encrypt file](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/encrypt-file.png?raw=true) | ![Decrypt buffer](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/decrypt-file.png?raw=true) |
 
 <table>
     <thead>
         <tr>
             <th rowspan=2>MB</th>
             <th colspan=2>Encrypt seconds</th>
             <th colspan=2>Decrypt seconds</th>
@@ -606,15 +606,15 @@
 
 # More benchmarks
 
 ## Different ways to use the lib
 
 | Encrypt | Decrypt |
 | ------- | ------- |
-| ![Encrypt buffer](resources/charts/encrypt-all.png) | ![Decrypt buffer](resources/charts/decrypt-all.png) |
+| ![Encrypt buffer](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/encrypt-all.png?raw=true) | ![Decrypt buffer](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/decrypt-all.png?raw=true) |
 
 
 <table>
     <thead>
         <tr>
             <th rowspan=2>MB</th>
             <th colspan=5>Encrypt seconds</th>
@@ -846,15 +846,15 @@
 </table>
 
 ## Speed throughput
 
 `256KB` seems to be the sweet spot for buffer size that offers the max `MB/s` speed for encryption, on benchmarks that seem to be the case.
 We performed `10.000` encryption operations for each size varying from `1KB` to `16MB`.
 
-![Speed throughput](resources/charts/speed-throughput.png)
+![Speed throughput](https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/speed-throughput.png?raw=true)
 
 | MB    | MB/s |
 | ----- | ------- |
 | 0.0009765625 | 1083 |
 | 0.001953125 | 1580 |
 | 0.00390625 | 2158 |
 | 0.0078125 | 2873 |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: REncrypt Version: 0.1.0 Classifier: Programming
+Metadata-Version: 2.3 Name: REncrypt Version: 0.1.5 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: Apache Software License License-File:
 LICENSE Summary: A Python encryption library implemented in Rust. It supports
 AEAD with AES-GCM and ChaCha20Poly1305. It uses ring crate to handle
 encryption. Keywords: cryptography,encryption,security,rust,speed Author-email:
 Radu Marias
@@ -20,16 +20,17 @@
 found to be the fastest. After this there is also comparison with other
 implementations. ## Buffer in memory This is useful when you keep a buffer, set
 your plaintext/ciphertext in there, and then encrypt/decrypt in-place that
 buffer. This is the most performant way to use it, because it does't copy any
 bytes nor allocate new memory. `REncrypt` is faster on small buffers, less than
 few MB, `PyFLocker` is comming closer for larger buffers. | Encrypt seconds |
 Decrypt seconds | | --------------- | --------------- | | ![Encrypt buffer]
-(resources/charts/encrypt.png) | ![Decrypt buffer](resources/charts/
-decrypt.png) |
+(https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/
+encrypt.png?raw=true) | ![Decrypt buffer](https://github.com/radumarias/
+rencrypt-python/blob/main/resources/charts/decrypt.png?raw=true) |
 MMBB      EEnnccrryypptt sseeccoonnddss    DDeeccrryypptt sseeccoonnddss
         RREEnnccrryypptt PPyyFFLLoocckkeerr RREEnnccrryypptt PPyyFFLLoocckkeerr
 0.03125 0.00001  0.00091   0.00001  0.00004
 0.0625  0.00001  0.00005   0.00001  0.00004
 0.125   0.00002  0.00005   0.00003  0.00005
 0.25    0.00004  0.00008   0.00005  0.00009
 0.5     0.00010  0.00014   0.00011  0.00015
@@ -41,16 +42,18 @@
 32      0.00678  0.00748   0.00749  0.01348
 64      0.01361  0.01461   0.01460  0.02697
 128     0.02923  0.03027   0.03134  0.05410
 256     0.06348  0.06188   0.06136  0.10417
 512     0.11782  0.13463   0.12090  0.21114
 1024    0.25001  0.24953   0.25377  0.42581
 ## File | Encrypt seconds | Decrypt seconds | | --------------- | -------------
--- | | ![Encrypt file](resources/charts/encrypt-file.png) | ![Decrypt buffer]
-(resources/charts/decrypt-file.png) |
+-- | | ![Encrypt file](https://github.com/radumarias/rencrypt-python/blob/main/
+resources/charts/encrypt-file.png?raw=true) | ![Decrypt buffer](https://
+github.com/radumarias/rencrypt-python/blob/main/resources/charts/decrypt-
+file.png?raw=true) |
 MMBB       EEnnccrryypptt sseeccoonnddss    DDeeccrryypptt sseeccoonnddss
          RREEnnccrryypptt PPyyFFLLoocckkeerr RREEnnccrryypptt PPyyFFLLoocckkeerr
 0.031251 0.00010  0.00280   0.00004  0.00479
 0.062501 0.00009  0.00218   0.00005  0.00143
 0.125    0.00020  0.00212   0.00014  0.00129
 0.25     0.00034  0.00232   0.00020  0.00165
 0.5      0.00050  0.00232   0.00035  0.00181
@@ -190,16 +193,18 @@
 github.com/radumarias/rencrypt-python && cd rencrypt-python ``` ## Compile and
 run ```bash curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh ```
 To configure your current shell, you need to source the corresponding env file
 under $HOME/.cargo. This is usually done by running one of the following (note
 the leading DOT): ```bash . "$HOME/.cargo/env" ``` ``` python -m venv .env
 source .env/bin/activate pip install maturin maturin develop python bench.py
 ``` # More benchmarks ## Different ways to use the lib | Encrypt | Decrypt | |
-------- | ------- | | ![Encrypt buffer](resources/charts/encrypt-all.png) | !
-[Decrypt buffer](resources/charts/decrypt-all.png) |
+------- | ------- | | ![Encrypt buffer](https://github.com/radumarias/rencrypt-
+python/blob/main/resources/charts/encrypt-all.png?raw=true) | ![Decrypt buffer]
+(https://github.com/radumarias/rencrypt-python/blob/main/resources/charts/
+decrypt-all.png?raw=true) |
         EEnnccrryypptt sseeccoonnddss                                          DDeeccrryypptt sseeccoonnddss
 MMBB      RREEnnccrryypptt PPyyFFLLoocckkeerr   RREEnnccrryypptt     RREEnnccrryypptt     PPyyFFLLoocckkeerr RREEnnccrryypptt PPyyFFLLoocckkeerr   RREEnnccrryypptt     RREEnnccrryypptt     PPyyFFLLoocckkeerr
         eennccrryypptt  uuppddaattee__iinnttoo eennccrryypptt__iinnttoo eennccrryypptt__ffrroomm uuppddaattee    ddeeccrryypptt  uuppddaattee__iinnttoo ddeeccrryypptt__iinnttoo ddeeccrryypptt__ffrroomm uuppddaattee
 0.03125 0.00001  0.00091     0.00001      0.00002      0.00009   0.00001  0.00004     0.00001      0.00003      0.00005
 0.0625  0.00001  0.00005     0.00002      0.00002      0.00005   0.00001  0.00004     0.00002      0.00004      0.00008
 0.125   0.00002  0.00005     0.00003      0.00005      0.00011   0.00003  0.00005     0.00003      0.00007      0.00013
 0.25    0.00004  0.00008     0.00007      0.00009      0.00019   0.00005  0.00009     0.00007      0.00016      0.00023
@@ -214,19 +219,20 @@
 128     0.02923  0.03027     0.03343      0.06805      0.10362   0.03134  0.05410     0.03558      0.06955      0.11380
 256     0.06348  0.06188     0.07303      0.13003      0.20911   0.06136  0.10417     0.07572      0.13733      0.20828
 512     0.11782  0.13463     0.14283      0.26799      0.41929   0.12090  0.21114     0.14434      0.25771      0.41463
 1024    0.25001  0.24953     0.28912      0.51228      0.82370   0.25377  0.42581     0.29795      0.53807      0.82588
 ## Speed throughput `256KB` seems to be the sweet spot for buffer size that
 offers the max `MB/s` speed for encryption, on benchmarks that seem to be the
 case. We performed `10.000` encryption operations for each size varying from
-`1KB` to `16MB`. ![Speed throughput](resources/charts/speed-throughput.png) |
-MB | MB/s | | ----- | ------- | | 0.0009765625 | 1083 | | 0.001953125 | 1580 |
-| 0.00390625 | 2158 | | 0.0078125 | 2873 | | 0.015625 | 3348 | | 0.03125 | 3731
-| | 0.0625 | 4053 | | 0.125 | 4156 | | 0.25 | 4247 | | 0.5 | 4182 | | 1.0 |
-3490 | | 2.0 | 3539 | | 4.0 | 3684 | | 8.0 | 3787 | | 16.0 | 3924 | # For the
-future - Add more `AES` ciphers like `AES128-GCM` and `AES-GCM-SIV` - Add other
-encryption providers like [RustCrypto](https://github.com/RustCrypto/traits)
-and [libsodium](https://crates.io/crates/sodiumoxide) - Maybe add support for
-`RSA` and `Elliptic-curve cryptography` - Saving and loading keys from file #
+`1KB` to `16MB`. ![Speed throughput](https://github.com/radumarias/rencrypt-
+python/blob/main/resources/charts/speed-throughput.png?raw=true) | MB | MB/s |
+| ----- | ------- | | 0.0009765625 | 1083 | | 0.001953125 | 1580 | | 0.00390625
+| 2158 | | 0.0078125 | 2873 | | 0.015625 | 3348 | | 0.03125 | 3731 | | 0.0625 |
+4053 | | 0.125 | 4156 | | 0.25 | 4247 | | 0.5 | 4182 | | 1.0 | 3490 | | 2.0 |
+3539 | | 4.0 | 3684 | | 8.0 | 3787 | | 16.0 | 3924 | # For the future - Add
+more `AES` ciphers like `AES128-GCM` and `AES-GCM-SIV` - Add other encryption
+providers like [RustCrypto](https://github.com/RustCrypto/traits) and
+[libsodium](https://crates.io/crates/sodiumoxide) - Maybe add support for `RSA`
+and `Elliptic-curve cryptography` - Saving and loading keys from file #
 Considerations This lib hasn't been audited, but it mostly wraps `ring` crate
 which is a well known library, so in principle it should offer the same level
 of security.
```

