# Comparing `tmp/peakrdl-python-0.7.4.tar.gz` & `tmp/peakrdl_python-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakrdl-python-0.7.4.tar", last modified: Tue Apr  2 13:25:32 2024, max compression
+gzip compressed data, was "peakrdl_python-0.7.5.tar", last modified: Sat Jun  1 17:04:10 2024, max compression
```

## Comparing `peakrdl-python-0.7.4.tar` & `peakrdl_python-0.7.5.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.250208 peakrdl-python-0.7.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.226208 peakrdl-python-0.7.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.230208 peakrdl-python-0.7.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/.github/workflows/action.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42719 2024-04-02 13:25:32.250208 peakrdl-python-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.234208 peakrdl-python-0.7.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/api_components.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/customisation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/design_decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/design_tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14790 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/generated_package.rst
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.226208 peakrdl-python-0.7.4/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.234208 peakrdl-python-0.7.4/example/array_access/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/array_access/array_access.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/array_access/demo_array_access.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.234208 peakrdl-python-0.7.4/example/enumerated_fields/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/enumerated_fields/demo_enumerated_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/enumerated_fields/enumerated_fields.rdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.234208 peakrdl-python-0.7.4/example/optimised_access/
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/optimised_access/demo_optimised_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/optimised_access/demo_optimised_array_access.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/optimised_access/optimised_access.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/optimised_access/optimised_array_access.rdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.234208 peakrdl-python-0.7.4/example/overridden_names/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/overridden_names/over_ridden_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/overridden_names/overridden_names.rdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.234208 peakrdl-python-0.7.4/example/simulating_callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/simulating_callbacks/chip_with_a_GPIO.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/simulating_callbacks/flashing_the_LED.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.234208 peakrdl-python-0.7.4/example/tranversing_address_map/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/tranversing_address_map/chip_with_registers.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/tranversing_address_map/dumping_register_state_to_json_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/tranversing_address_map/reg_dump.json
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/tranversing_address_map/reseting_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10786 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/tranversing_address_map/writing_register_state_from_json_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.238208 peakrdl-python-0.7.4/example/why_ral/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/why_ral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/why_ral/gpio.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/why_ral/hardware_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/why_ral/with_hal.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/why_ral/with_ral.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/example/why_ral/without_ral.py
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/generate_and_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/generate_testcases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:25:32.250208 peakrdl-python-0.7.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.230208 peakrdl-python-0.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.238208 peakrdl-python-0.7.4/src/peakrdl_python/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/__peakrdl__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/_node_walkers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20125 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.242208 peakrdl-python-0.7.4/src/peakrdl_python/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32764 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/async_register.py
--rw-r--r--   0 runner    (1001) docker     (127)    31244 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    28611 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    35122 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    39506 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/lib/utility_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11493 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/safe_name_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/systemrdl_node_utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.242208 peakrdl-python-0.7.4/src/peakrdl_python/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22374 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_field.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_memory.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_register.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_simulation.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_simulation_tb.jinja
--rw-r--r--   0 runner    (1001) docker     (127)    86012 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/baseclass_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/header.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/header_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/src/peakrdl_python/templates/reg_definitions.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.250208 peakrdl-python-0.7.4/src/peakrdl_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42719 2024-04-02 13:25:32.000000 peakrdl-python-0.7.4/src/peakrdl_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-02 13:25:32.000000 peakrdl-python-0.7.4/src/peakrdl_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:25:32.000000 peakrdl-python-0.7.4/src/peakrdl_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 13:25:32.000000 peakrdl-python-0.7.4/src/peakrdl_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 13:25:32.000000 peakrdl-python-0.7.4/src/peakrdl_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 13:25:32.000000 peakrdl-python-0.7.4/src/peakrdl_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.242208 peakrdl-python-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/.mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.242208 peakrdl-python-0.7.4/tests/alternative_template_toml/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/alternative_template_toml/peakrdl.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.246208 peakrdl-python-0.7.4/tests/alternative_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/alternative_templates/header.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/alternative_templates/header_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/pylint.rc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.250208 peakrdl-python-0.7.4/tests/testcases/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/RDLFormatCode_example.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/addr_map.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/all_register_access_types.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/basic.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/block_a.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/block_b.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/different_array_types.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/enum_example.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/example_issue_106.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/field_scope.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/field_with_overridden_reset.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/fields_with_HW_write.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/fields_with_reset_values.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/memories.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/memories_with_registers.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/msb0_and_lsb0.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/multi_block.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/multifile.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/name_clash.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/overridden_python_name.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/parametrised_readonly_and_readwrite.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/regfile_and_arrays.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/same_but_different_enum.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/signals_definitions_at_various_levels.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/simple.rdl
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/simple.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/sizes_registers.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/sizes_registers_array.rdl
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/testcases/write_only_enum_with_undefined_reset.rdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:25:32.250208 peakrdl-python-0.7.4/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/unit_tests/simple_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/unit_tests/test_array_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11899 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/unit_tests/test_optimised_reg_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-04-02 13:25:28.000000 peakrdl-python-0.7.4/tests/unit_tests/test_reg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.791317 peakrdl_python-0.7.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.767317 peakrdl_python-0.7.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.771317 peakrdl_python-0.7.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/.github/workflows/action.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42719 2024-06-01 17:04:10.791317 peakrdl_python-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.775317 peakrdl_python-0.7.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/docs/api_components.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/docs/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/docs/customisation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/docs/design_decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/docs/design_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14790 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/docs/generated_package.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.767317 peakrdl_python-0.7.5/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.775317 peakrdl_python-0.7.5/example/array_access/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/array_access/array_access.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/array_access/demo_array_access.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.775317 peakrdl_python-0.7.5/example/enumerated_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/enumerated_fields/demo_enumerated_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/enumerated_fields/enumerated_fields.rdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.775317 peakrdl_python-0.7.5/example/optimised_access/
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/optimised_access/demo_optimised_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/optimised_access/demo_optimised_array_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/optimised_access/optimised_access.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/optimised_access/optimised_array_access.rdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.775317 peakrdl_python-0.7.5/example/overridden_names/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/overridden_names/over_ridden_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/overridden_names/overridden_names.rdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.775317 peakrdl_python-0.7.5/example/simulating_callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/simulating_callbacks/chip_with_a_GPIO.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/simulating_callbacks/flashing_the_LED.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.775317 peakrdl_python-0.7.5/example/tranversing_address_map/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/tranversing_address_map/chip_with_registers.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/tranversing_address_map/dumping_register_state_to_json_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/tranversing_address_map/reg_dump.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/tranversing_address_map/reseting_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10786 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/tranversing_address_map/writing_register_state_from_json_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.779317 peakrdl_python-0.7.5/example/why_ral/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/why_ral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/why_ral/gpio.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/why_ral/hardware_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/why_ral/with_hal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/why_ral/with_ral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/example/why_ral/without_ral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/generate_and_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/generate_testcases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 17:04:10.791317 peakrdl_python-0.7.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.771317 peakrdl_python-0.7.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.779317 peakrdl_python-0.7.5/src/peakrdl_python/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/__peakrdl__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/_node_walkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20125 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.783317 peakrdl_python-0.7.5/src/peakrdl_python/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35176 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/lib/async_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31244 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/lib/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/lib/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28611 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/lib/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35122 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/lib/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41091 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/lib/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/lib/utility_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11493 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/safe_name_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/systemrdl_node_utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.783317 peakrdl_python-0.7.5/src/peakrdl_python/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22374 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/templates/addrmap.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/templates/addrmap_field.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/templates/addrmap_memory.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/templates/addrmap_register.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/templates/addrmap_simulation.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/templates/addrmap_simulation_tb.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)    86012 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/templates/addrmap_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/templates/baseclass_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/templates/header.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/templates/header_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/src/peakrdl_python/templates/reg_definitions.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.791317 peakrdl_python-0.7.5/src/peakrdl_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42719 2024-06-01 17:04:10.000000 peakrdl_python-0.7.5/src/peakrdl_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-06-01 17:04:10.000000 peakrdl_python-0.7.5/src/peakrdl_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 17:04:10.000000 peakrdl_python-0.7.5/src/peakrdl_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 17:04:10.000000 peakrdl_python-0.7.5/src/peakrdl_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-01 17:04:10.000000 peakrdl_python-0.7.5/src/peakrdl_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-01 17:04:10.000000 peakrdl_python-0.7.5/src/peakrdl_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.783317 peakrdl_python-0.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/.mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.783317 peakrdl_python-0.7.5/tests/alternative_template_toml/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/alternative_template_toml/peakrdl.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.783317 peakrdl_python-0.7.5/tests/alternative_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/alternative_templates/header.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/alternative_templates/header_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/pylint.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.791317 peakrdl_python-0.7.5/tests/testcases/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/RDLFormatCode_example.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/addr_map.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/all_register_access_types.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/basic.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/block_a.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/block_b.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/different_array_types.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/enum_example.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/example_issue_106.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/field_scope.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/field_with_overridden_reset.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/fields_with_HW_write.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/fields_with_reset_values.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/memories.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/memories_with_registers.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/msb0_and_lsb0.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/multi_block.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/multifile.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/name_clash.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/overridden_python_name.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/parametrised_readonly_and_readwrite.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/regfile_and_arrays.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/same_but_different_enum.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/signals_definitions_at_various_levels.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/simple.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/simple.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/sizes_registers.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/sizes_registers_array.rdl
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/testcases/write_only_enum_with_undefined_reset.rdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:04:10.791317 peakrdl_python-0.7.5/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/unit_tests/simple_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/unit_tests/test_array_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11899 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/unit_tests/test_optimised_reg_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21393 2024-06-01 17:04:07.000000 peakrdl_python-0.7.5/tests/unit_tests/test_reg.py
```

### Comparing `peakrdl-python-0.7.4/.github/workflows/action.yaml` & `peakrdl_python-0.7.5/.github/workflows/action.yaml`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/.gitignore` & `peakrdl_python-0.7.5/.gitignore`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/.readthedocs.yaml` & `peakrdl_python-0.7.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/LICENSE` & `peakrdl_python-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/PKG-INFO` & `peakrdl_python-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-python
-Version: 0.7.4
+Version: 0.7.5
 Summary: Generate Python Register Access Layer (RAL) from SystemRDL
 Author: Keith Brady
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `peakrdl-python-0.7.4/README.md` & `peakrdl_python-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/docs/api.rst` & `peakrdl_python-0.7.5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/docs/api_components.rst` & `peakrdl_python-0.7.5/docs/api_components.rst`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     :inherited-members:
 
 .. autoclass:: peakrdl_python.lib.memory.MemoryReadWriteArray
     :members:
     :inherited-members:
 
 Registers
-^^^^^^^^^
+=========
 
 .. autoclass:: peakrdl_python.lib.register.RegReadOnly
     :members:
     :inherited-members:
 
 .. autoclass:: peakrdl_python.lib.register.RegWriteOnly
     :members:
@@ -89,14 +89,15 @@
 
 .. autoclass:: peakrdl_python.lib.register.RegReadWriteArray
     :members:
     :inherited-members:
 
 Register Fields
 ^^^^^^^^^^^^^^^
+A register will always have fields within it
 
 .. autoclass:: peakrdl_python.lib.fields.FieldReadOnly
     :members:
     :inherited-members:
 
 .. autoclass:: peakrdl_python.lib.fields.FieldWriteOnly
     :members:
@@ -112,8 +113,8 @@
 
 .. autoclass:: peakrdl_python.lib.fields.FieldEnumWriteOnly
     :members:
     :inherited-members:
 
 .. autoclass:: peakrdl_python.lib.fields.FieldEnumReadWrite
     :members:
-    :inherited-members:
+    :inherited-members:
```

### Comparing `peakrdl-python-0.7.4/docs/conf.py` & `peakrdl_python-0.7.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/docs/customisation.rst` & `peakrdl_python-0.7.5/docs/customisation.rst`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/docs/design_decisions.rst` & `peakrdl_python-0.7.5/docs/design_decisions.rst`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/docs/generated_package.rst` & `peakrdl_python-0.7.5/docs/generated_package.rst`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/docs/index.rst` & `peakrdl_python-0.7.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/docs/installation.rst` & `peakrdl_python-0.7.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/array_access/demo_array_access.py` & `peakrdl_python-0.7.5/example/array_access/demo_array_access.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/enumerated_fields/demo_enumerated_fields.py` & `peakrdl_python-0.7.5/example/enumerated_fields/demo_enumerated_fields.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/enumerated_fields/enumerated_fields.rdl` & `peakrdl_python-0.7.5/example/enumerated_fields/enumerated_fields.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/optimised_access/demo_optimised_access.py` & `peakrdl_python-0.7.5/example/optimised_access/demo_optimised_access.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/optimised_access/demo_optimised_array_access.py` & `peakrdl_python-0.7.5/example/optimised_access/demo_optimised_array_access.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/optimised_access/optimised_access.rdl` & `peakrdl_python-0.7.5/example/optimised_access/optimised_access.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/overridden_names/over_ridden_names.py` & `peakrdl_python-0.7.5/example/overridden_names/over_ridden_names.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/simulating_callbacks/chip_with_a_GPIO.rdl` & `peakrdl_python-0.7.5/example/simulating_callbacks/chip_with_a_GPIO.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/simulating_callbacks/flashing_the_LED.py` & `peakrdl_python-0.7.5/example/simulating_callbacks/flashing_the_LED.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/tranversing_address_map/dumping_register_state_to_json_file.py` & `peakrdl_python-0.7.5/example/tranversing_address_map/dumping_register_state_to_json_file.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/tranversing_address_map/reg_dump.json` & `peakrdl_python-0.7.5/example/tranversing_address_map/reg_dump.json`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/tranversing_address_map/reseting_registers.py` & `peakrdl_python-0.7.5/example/tranversing_address_map/reseting_registers.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/tranversing_address_map/writing_register_state_from_json_file.py` & `peakrdl_python-0.7.5/example/tranversing_address_map/writing_register_state_from_json_file.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/why_ral/gpio.rdl` & `peakrdl_python-0.7.5/example/why_ral/gpio.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/why_ral/hardware_sim.py` & `peakrdl_python-0.7.5/example/why_ral/hardware_sim.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/why_ral/with_hal.py` & `peakrdl_python-0.7.5/example/why_ral/with_hal.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/why_ral/with_ral.py` & `peakrdl_python-0.7.5/example/why_ral/with_ral.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/example/why_ral/without_ral.py` & `peakrdl_python-0.7.5/example/why_ral/without_ral.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/generate_and_test.py` & `peakrdl_python-0.7.5/generate_and_test.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/generate_testcases.py` & `peakrdl_python-0.7.5/generate_testcases.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/pyproject.toml` & `peakrdl_python-0.7.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/.coveragerc` & `peakrdl_python-0.7.5/src/peakrdl_python/.coveragerc`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/__about__.py` & `peakrdl_python-0.7.5/src/peakrdl_python/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Variables that describes the peakrdl-python Package
 """
-__version__ = "0.7.4"
+__version__ = "0.7.5"
```

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/__init__.py` & `peakrdl_python-0.7.5/src/peakrdl_python/__init__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/__peakrdl__.py` & `peakrdl_python-0.7.5/src/peakrdl_python/__peakrdl__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/_node_walkers.py` & `peakrdl_python-0.7.5/src/peakrdl_python/_node_walkers.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/exporter.py` & `peakrdl_python-0.7.5/src/peakrdl_python/exporter.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/lib/__init__.py` & `peakrdl_python-0.7.5/src/peakrdl_python/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/lib/async_register.py` & `peakrdl_python-0.7.5/src/peakrdl_python/lib/async_register.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from enum import Enum
 from typing import List, Union, Iterator, TYPE_CHECKING, Tuple, cast, Optional, Dict, TypeVar
 from typing import AsyncGenerator
 from abc import ABC, abstractmethod
 from contextlib import asynccontextmanager
 from array import array as Array
 import sys
+from warnings import warn
 
 from .utility_functions import get_array_typecode
 from .base import AsyncAddressMap, AsyncRegFile
 from .register import BaseReg, BaseRegArray, RegisterWriteVerifyError
 from .memory import  MemoryAsyncReadOnly, MemoryAsyncWriteOnly, MemoryAsyncReadWrite, \
     AsyncMemory, ReadableAsyncMemory, WritableAsyncMemory
 from .callbacks import AsyncCallbackSet
@@ -123,22 +124,24 @@
     # pylint: enable=too-many-arguments, duplicate-code
 
     @asynccontextmanager
     async def single_read(self) -> AsyncGenerator[Self, None]:
         """
         Context manager to allow multiple field accesses to be performed with a single
         read of the register
-
-        Returns:
-
         """
         self.__register_state = await self.read()
+        # pylint: disable=duplicate-code
         self.__in_context_manager = True
-        yield self
-        self.__in_context_manager = False
+        # this try/finally is needed to make sure that in the event of an exception
+        # the state flags are not left incorrectly set
+        try:
+            yield self
+        finally:
+            self.__in_context_manager = False
 
     async def read(self) -> int:
         """Asynchronously read value from the register
 
         Returns:
             The value from register
 
@@ -288,15 +291,16 @@
 
 
 class RegAsyncReadWrite(RegAsyncReadOnly, RegAsyncWriteOnly, ABC):
     """
     class for an async read and write only register
 
     """
-    __slots__: List[str] = ['__in_context_manager', '__register_state']
+    __slots__: List[str] = ['__in_read_write_context_manager', '__in_read_context_manager',
+                            '__register_state']
 
     # pylint: disable=too-many-arguments, duplicate-code
     def __init__(self, *,
                  address: int,
                  width: int,
                  accesswidth: int,
                  logger_handle: str,
@@ -304,15 +308,16 @@
                  parent: Union[AsyncAddressMap, AsyncRegFile, MemoryAsyncReadWrite]):
 
         super().__init__(address=address,
                          logger_handle=logger_handle,
                          inst_name=inst_name,
                          parent=parent, width=width, accesswidth=accesswidth)
 
-        self.__in_context_manager: bool = False
+        self.__in_read_write_context_manager: bool = False
+        self.__in_read_context_manager: bool = False
         self.__register_state: Optional[int] = None
 
     # pylint: enable=too-many-arguments, duplicate-code
 
     @asynccontextmanager
     async def single_read_modify_write(self, verify: bool = False, skip_write: bool = False) -> \
         AsyncGenerator[Self, None]:
@@ -320,27 +325,61 @@
         Context manager to allow multiple field reads/write to be done with a single set of
         field operations
 
         Args:
             verify (bool): very the write with a read afterwards
             skip_write (bool): skip the write back at the end
 
-        Returns:
-
         """
+        # pylint: disable=duplicate-code
+        if self.__in_read_context_manager:
+            raise RuntimeError('using the `single_read_modify_write` context manager within the '
+                               'single_read` is not permitted')
+
+        if skip_write is True:
+            warn('The `skip_write` argument will be removed in the future, use `single_read`'
+                 ' instead',
+                 DeprecationWarning, stacklevel=2)
+        # pylint: enable=duplicate-code
+
         self.__register_state = await self.read()
-        self.__in_context_manager = True
-        yield self
-        self.__in_context_manager = False
+
+        # pylint: disable=duplicate-code
+        self.__in_read_write_context_manager = True
+        # this try/finally is needed to make sure that in the event of an exception
+        # the state flags are not left incorrectly set
+        try:
+            yield self
+        finally:
+            self.__in_read_write_context_manager = False
+        # pylint: enable=duplicate-code
         if not skip_write:
             await self.write(self.__register_state, verify)
 
         # clear the register states at the end of the context manager
         self.__register_state = None
 
+    @asynccontextmanager
+    async def single_read(self) -> \
+            AsyncGenerator[Self, None]:
+        """
+        Context manager to allow multiple field reads with a single register read
+        """
+        # pylint: disable=duplicate-code
+        if self.__in_read_write_context_manager:
+            raise RuntimeError('using the `single_read` context manager within the '
+                               'single_read_modify_write` is not permitted')
+        self.__in_read_context_manager = True
+        # pylint: enable=duplicate-code
+        try:
+            async with super().single_read() as reg:
+                yield reg
+        finally:
+            self.__in_read_context_manager = False
+
     async def write(self, data: int, verify: bool = False) -> None:
         """
         Writes a value to the register
 
         Args:
             data: data to be written
             verify: set to True to read back the register to verify the read has occurred correctly
@@ -348,49 +387,53 @@
         Raises:
             ValueError: if the value provided is outside the range of the
                         permissible values for the register
             TypeError: if the type of data is wrong
             RegisterWriteVerifyError: the read back data after the write does not match the
                                       expected value
         """
-        if self.__in_context_manager:
+        if self.__in_read_context_manager:
+            raise RuntimeError('writes within the single read context manager are not permitted')
+
+        if self.__in_read_write_context_manager:
             # pylint: disable=duplicate-code
             if self.__register_state is None:
                 raise RuntimeError('The internal register state should never be None in the '
                                    'context manager')
             self.__register_state = data
         else:
             await super().write(data)
             if verify:
                 read_back = await self.read()
                 if read_back != data:
                     raise RegisterWriteVerifyError(f'Readback {read_back:X} '
                                                    f'after writing {data:X}')
 
     async def read(self) -> int:
-        """Asynchronously read value from the register
-
-        Returns:
-            The value from register
         """
-        if self.__in_context_manager:
+        Asynchronously read value from the register
+        """
+        if self.__in_read_write_context_manager:
             # pylint: disable=duplicate-code
             if self.__register_state is None:
                 raise RuntimeError('The internal register state should never be None in the '
                                    'context manager')
             return self.__register_state
 
+        # the single read context manager is handled in the base class so does need any
+        # handling here
+
         return await super().read()
 
     async def read_fields(self) -> Dict['str', Union[bool, Enum, int]]:
         """
         asynchronously read the register and return a dictionary of the field values
         """
         return_dict: Dict['str', Union[bool, Enum, int]] = {}
-        async with self.single_read_modify_write(skip_write=True) as reg:
+        async with self.single_read() as reg:
             for field in reg.readable_fields:
                 return_dict[field.inst_name] = await field.read()
 
         return return_dict
 
     async def write_fields(self, **kwargs) -> None:  # type: ignore[no-untyped-def]
         """
@@ -550,15 +593,16 @@
         Validate the data provided and determine the cache entry
 
         Args:
             addr: Address to write to
             width: Width of the register in bits
             accesswidth: Minimum access width of the register in bits
 
-        Returns: cache entry
+        Returns:
+            cache entry
 
         """
         if not isinstance(width, int):
             raise TypeError(f'Width should be an int byt got {type(width)}')
         if width != self.width:
             raise ValueError('Requested Read width does not match the expected value')
         if not isinstance(accesswidth, int):
@@ -633,26 +677,28 @@
         Context manager to allow multiple field reads/write to be done with a single set of
         field operations
 
         Args:
             verify (bool): very the write with a read afterwards
             skip_write (bool): skip the write back at the end
 
-        Returns:
-
         """
         self.__register_address_array = \
             [self.address + (i * (self.width >> 3)) for i in range(self.__number_cache_entries)]
         if skip_initial_read:
             self.__register_array_cache = self.__empty_array_cache
         else:
             self.__register_array_cache = await self.__block_read()
         self.__in_context_manager = True
-        yield self
-        self.__in_context_manager = False
+        # this try/finally is needed to make sure that in the event of an exception
+        # the state flags are not left incorrectly set
+        try:
+            yield self
+        finally:
+            self.__in_context_manager = False
         if not skip_write:
             await self.__block_write(self.__register_array_cache, verify)
 
         # clear the register states at the end of the context manager
         self.__register_address_array = None
         self.__register_array_cache = None
 
@@ -707,15 +753,15 @@
         Args:
 
 
         Returns:
 
         """
         async with self._cached_access(verify=False, skip_write=True,
-                                 skip_initial_read=False) as reg_array:
+                                       skip_initial_read=False) as reg_array:
             yield reg_array
 
     @property
     def _is_readable(self) -> bool:
         return True
 
     @property
@@ -814,16 +860,21 @@
         Args:
             verify (bool): very the write with a read afterwards
             skip_write (bool): skip the write back at the end
 
         Returns:
 
         """
+        if skip_write is True:
+            warn('The `skip_write` argument will be removed in the future, use `single_read`'
+                 ' instead',
+                 DeprecationWarning, stacklevel=2)
+
         async with self._cached_access(verify=verify, skip_write=skip_write,
-                                  skip_initial_read=False) as reg_array:
+                                       skip_initial_read=False) as reg_array:
             yield reg_array
 
     @property
     def _is_readable(self) -> bool:
         return True
 
     @property
```

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/lib/base.py` & `peakrdl_python-0.7.5/src/peakrdl_python/lib/base.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/lib/callbacks.py` & `peakrdl_python-0.7.5/src/peakrdl_python/lib/callbacks.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/lib/fields.py` & `peakrdl_python-0.7.5/src/peakrdl_python/lib/fields.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/lib/memory.py` & `peakrdl_python-0.7.5/src/peakrdl_python/lib/memory.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/lib/register.py` & `peakrdl_python-0.7.5/src/peakrdl_python/lib/register.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from enum import Enum
 from typing import List, Union, Iterator, TYPE_CHECKING, Tuple, cast, Optional, Dict, TypeVar, Type
 from typing import Generator
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from array import array as Array
 import sys
+from warnings import warn
 
 from .base import Node, AddressMap, RegFile, NodeArray
 from .utility_functions import get_array_typecode
 from .base import AsyncAddressMap, AsyncRegFile
 from .memory import  MemoryReadOnly, MemoryWriteOnly, MemoryReadWrite, \
     BaseMemory, Memory, ReadableMemory, WritableMemory
 from .callbacks import NormalCallbackSet
@@ -89,15 +90,16 @@
         if accesswidth not in (8, 16, 32, 64):
             raise ValueError(f'currently only support 8, 16, 32 or 64 accesswidth, got {width:d}')
         self.__accesswidth = accesswidth
     # pylint: enable=too-many-arguments,duplicate-code
 
     @property
     def max_value(self) -> int:
-        """maximum unsigned integer value that can be stored in the register
+        """
+        maximum unsigned integer value that can be stored in the register
 
         For example:
 
         * 8-bit register returns 0xFF (255)
         * 16-bit register returns 0xFFFF (65535)
         * 32-bit register returns 0xFFFF_FFFF (4294967295)
 
@@ -117,47 +119,42 @@
         if data < 0:
             raise ValueError('data out of range')
 
     @property
     def width(self) -> int:
         """
         The width of the register in bits, this uses the `regwidth` systemRDL property
-
-        Returns: register width
-
         """
         return self.__width
 
     @property
     def accesswidth(self) -> int:
         """
         The access width of the register in bits, this uses the `accesswidth` systemRDL property
-
-        Returns: register access width
         """
         return self.__accesswidth
 
     @property
     def size(self) -> int:
         """
         Total Number of bytes of address the node occupies
         """
         return self.__width >> 3
 
-
     @property
     @abstractmethod
     def _is_readable(self) -> bool:
         ...
 
     @property
     @abstractmethod
     def _is_writeable(self) -> bool:
         ...
 
+
 class Reg(BaseReg, ABC):
     """
         base class of non-async register wrappers
 
         Note:
             It is not expected that this class will be instantiated under normal
             circumstances however, it is useful for type checking
@@ -238,40 +235,34 @@
                          parent=parent, address=address,
                          stride=stride, dimensions=dimensions, elements=elements)
 
     @property
     def width(self) -> int:
         """
         The width of the register in bits, this uses the `regwidth` systemRDL property
-
-        Returns: register width
-
         """
         return self.__width
 
     @property
     def accesswidth(self) -> int:
         """
         The access width of the register in bits, this uses the `accesswidth` systemRDL property
-
-        Returns: register access width
         """
         return self.__accesswidth
 
     def _build_element(self, indices: Tuple[int, ...]) -> BaseRegArrayElementType:
 
         return self._element_datatype(
             logger_handle=self._build_element_logger_handle(indices=indices),
             address=self._address_calculator(indices),
             inst_name=self._build_element_inst_name(indices=indices),
             width=self.width,
             accesswidth=self.accesswidth,
             parent=self)
 
-
     def _sub_instance(self, elements: Dict[Tuple[int, ...], BaseRegArrayElementType]) ->\
             NodeArray[BaseRegArrayElementType]:
         if not isinstance(self.parent, (AddressMap, AsyncAddressMap, RegFile,
                                         AsyncRegFile, BaseMemory)):
             raise RuntimeError('Parent of a Node Array must be Node')
         return self.__class__(logger_handle=self._logger.name,
                               inst_name=self.inst_name,
@@ -427,15 +418,16 @@
         Validate the data provided and determine the cache entry
 
         Args:
             addr: Address to write to
             width: Width of the register in bits
             accesswidth: Minimum access width of the register in bits
 
-        Returns: cache entry
+        Returns:
+            cache entry
 
         """
         if not isinstance(width, int):
             raise TypeError(f'Width should be an int byt got {type(width)}')
         if width != self.width:
             raise ValueError('Requested Read width does not match the expected value')
         if not isinstance(accesswidth, int):
@@ -468,16 +460,14 @@
         """
         if self.__register_array_cache is None:
             raise RuntimeError('The cache array should be initialised')
         return self.__register_array_cache[self.__cache_entry(addr=addr,
                                                               width=width,
                                                               accesswidth=accesswidth)]
 
-
-
     def __cache_write(self, addr: int, width: int, accesswidth: int, data: int) -> None:
         """
         Used to replace the normal callbacks with those that access the cache
 
         Args:
             addr: Address to write to
             width: Width of the register in bits
@@ -491,49 +481,48 @@
             raise TypeError(f'Data should be an int byt got {type(data)}')
         if self.__register_array_cache is None:
             raise RuntimeError('The cache array should be initialised')
         self.__register_array_cache[self.__cache_entry(addr=addr,
                                                        width=width,
                                                        accesswidth=accesswidth)] = data
 
-
     @property
     def __cache_callbacks(self) -> NormalCallbackSet:
         return NormalCallbackSet(read_callback=self.__cache_read,
                                  write_callback=self.__cache_write)
 
-
     @property
     def __number_cache_entries(self) -> int:
         return self.size // (self.width >> 3)
 
     @contextmanager
     def _cached_access(self, verify: bool = False, skip_write: bool = False,
-                                   skip_initial_read: bool = False) -> \
+                       skip_initial_read: bool = False) -> \
             Generator[Self, None, None]:
         """
         Context manager to allow multiple field reads/write to be done with a single set of
         field operations
 
         Args:
             verify (bool): very the write with a read afterwards
             skip_write (bool): skip the write back at the end
-
-        Returns:
-
         """
         self.__register_address_array = \
             [self.address + (i * (self.width >> 3)) for i in range(self.__number_cache_entries)]
         if skip_initial_read:
             self.__register_array_cache = self.__empty_array_cache
         else:
             self.__register_array_cache = self.__block_read()
         self.__in_context_manager = True
-        yield self
-        self.__in_context_manager = False
+        # this try/finally is needed to make sure that in the event of an exception
+        # the state flags are not left incorrectly set
+        try:
+            yield self
+        finally:
+            self.__in_context_manager = False
         if not skip_write:
             self.__block_write(self.__register_array_cache, verify)
 
         # clear the register states at the end of the context manager
         self.__register_address_array = None
         self.__register_array_cache = None
 
@@ -545,14 +534,15 @@
 
         if self.parent is None:
             raise RuntimeError('Parent must be set')
         # This cast is OK because the type was checked in the __init__
         # pylint: disable-next=protected-access
         return cast(NormalCallbackSet, self.parent._callbacks)
 
+
 class RegReadOnly(Reg, ABC):
     """
     class for a read only register
 
     Args:
         callbacks: set of callback to be used for accessing the hardware or simulator
         address: address of the register
@@ -585,29 +575,27 @@
     # pylint: enable=too-many-arguments, duplicate-code
 
     @contextmanager
     def single_read(self) -> Generator[Self, None, None]:
         """
         Context manager to allow multiple field accesses to be performed with a single
         read of the register
-
-        Returns:
-
         """
         self.__register_state = self.read()
         self.__in_context_manager = True
-        yield self
-        self.__in_context_manager = False
+        # this try/finally is needed to make sure that in the event of an exception
+        # the state flags are not left incorrectly set
+        try:
+            yield self
+        finally:
+            self.__in_context_manager = False
 
     def read(self) -> int:
-        """Read value from the register
-
-        Returns:
-            The value from register
-
+        """
+        Read value from the register
         """
         if self.__in_context_manager:
             return self.__register_state
 
         read_block_callback = self._callbacks.read_block_callback
         read_callback = self._callbacks.read_callback
 
@@ -744,15 +732,16 @@
 
 
 class RegReadWrite(RegReadOnly, RegWriteOnly, ABC):
     """
     class for a read and write only register
 
     """
-    __slots__: List[str] = ['__in_context_manager', '__register_state']
+    __slots__: List[str] = ['__in_read_write_context_manager', '__in_read_context_manager',
+                            '__register_state']
 
     # pylint: disable=too-many-arguments, duplicate-code
     def __init__(self, *,
                  address: int,
                  width: int,
                  accesswidth: int,
                  logger_handle: str,
@@ -760,15 +749,16 @@
                  parent: Union[AddressMap, RegFile, MemoryReadWrite]):
 
         super().__init__(address=address,
                          logger_handle=logger_handle,
                          inst_name=inst_name,
                          parent=parent, width=width, accesswidth=accesswidth)
 
-        self.__in_context_manager: bool = False
+        self.__in_read_write_context_manager: bool = False
+        self.__in_read_context_manager: bool = False
         self.__register_state: Optional[int] = None
 
     # pylint: enable=too-many-arguments, duplicate-code
 
     @contextmanager
     def single_read_modify_write(self, verify: bool = False, skip_write: bool = False) -> \
             Generator[Self, None, None]:
@@ -776,27 +766,55 @@
         Context manager to allow multiple field reads/write to be done with a single set of
         field operations
 
         Args:
             verify (bool): very the write with a read afterwards
             skip_write (bool): skip the write back at the end
 
-        Returns:
-
         """
+        if self.__in_read_context_manager:
+            raise RuntimeError('using the `single_read_modify_write` context manager within the '
+                               'single_read` is not permitted')
+
+        if skip_write is True:
+            warn('The `skip_write` argument will be removed in the future, use `single_read`'
+                 ' instead',
+                 DeprecationWarning, stacklevel=2)
+
         self.__register_state = self.read()
-        self.__in_context_manager = True
-        yield self
-        self.__in_context_manager = False
+        self.__in_read_write_context_manager = True
+        try:
+            yield self
+        finally:
+            # need to make sure the state flag is cleared even if an exception occurs within
+            # the context
+            self.__in_read_write_context_manager = False
+
         if not skip_write:
             self.write(self.__register_state, verify)
 
         # clear the register states at the end of the context manager
         self.__register_state = None
 
+    @contextmanager
+    def single_read(self) -> \
+            Generator[Self, None, None]:
+        """
+        Context manager to allow multiple field reads with a single register read
+        """
+        if self.__in_read_write_context_manager:
+            raise RuntimeError('using the `single_read` context manager within the '
+                               'single_read_modify_write` is not permitted')
+        self.__in_read_context_manager = True
+        try:
+            with super().single_read() as reg:
+                yield reg
+        finally:
+            self.__in_read_context_manager = False
+
     def write(self, data: int, verify: bool = False) -> None:  # pylint: disable=arguments-differ
         """
         Writes a value to the register
 
         Args:
             data: data to be written
             verify: set to True to read back the register to verify the read has occurred correctly
@@ -804,39 +822,43 @@
         Raises:
             ValueError: if the value provided is outside the range of the
                         permissible values for the register
             TypeError: if the type of data is wrong
             RegisterWriteVerifyError: the read back data after the write does not match the
                                       expected value
         """
-        if self.__in_context_manager:
+        if self.__in_read_context_manager:
+            raise RuntimeError('writes within the single read context manager are not permitted')
+
+        if self.__in_read_write_context_manager:
             if self.__register_state is None:
                 raise RuntimeError('The internal register state should never be None in the '
                                    'context manager')
             self.__register_state = data
         else:
             super().write(data)
             if verify:
                 read_back = self.read()
                 if read_back != data:
                     raise RegisterWriteVerifyError(f'Readback {read_back:X} '
                                                    f'after writing {data:X}')
 
     def read(self) -> int:
-        """Read value from the register
-
-        Returns:
-            The value from register
         """
-        if self.__in_context_manager:
+        Read value from the register
+        """
+        if self.__in_read_write_context_manager:
             if self.__register_state is None:
                 raise RuntimeError('The internal register state should never be None in the '
                                    'context manager')
             return self.__register_state
 
+        # the single read context manager is handled in the base class so does need any
+        # handling here
+
         return super().read()
 
     def write_fields(self, **kwargs) -> None:  # type: ignore[no-untyped-def]
         """
         Do a read-modify-write to the register, updating any field included in
         the arguments
         """
@@ -852,15 +874,15 @@
                 field.write(field_value)
 
     def read_fields(self) -> Dict['str', Union[bool, Enum, int]]:
         """
         read the register and return a dictionary of the field values
         """
         return_dict: Dict['str', Union[bool, Enum, int]] = {}
-        with self.single_read_modify_write(skip_write=True) as reg:
+        with self.single_read() as reg:
             for field in reg.readable_fields:
                 return_dict[field.inst_name] = field.read()
 
         return return_dict
 
     @property
     def _is_readable(self) -> bool:
@@ -868,17 +890,19 @@
         return True
 
     @property
     def _is_writeable(self) -> bool:
         # pylint: disable=duplicate-code
         return True
 
+
 ReadableRegister = Union[RegReadOnly, RegReadWrite]
 WritableRegister = Union[RegWriteOnly, RegReadWrite]
 
+
 class RegReadOnlyArray(RegArray, ABC):
     """
     base class for a array of read only registers
     """
     __slots__: List[str] = []
 
     # pylint: disable=too-many-arguments,duplicate-code
@@ -907,20 +931,14 @@
 
     @contextmanager
     def single_read(self) -> \
             Generator[Self, None, None]:
         """
         Context manager to allow multiple field reads/write to be done with a single set of
         field operations
-
-        Args:
-
-
-        Returns:
-
         """
         with self._cached_access(verify=False, skip_write=True,
                                  skip_initial_read=False) as reg_array:
             yield reg_array
 
     @property
     def _is_readable(self) -> bool:
@@ -928,14 +946,15 @@
         return True
 
     @property
     def _is_writeable(self) -> bool:
         # pylint: disable=duplicate-code
         return False
 
+
 class RegWriteOnlyArray(RegArray, ABC):
     """
     base class for a array of write only registers
     """
     __slots__: List[str] = []
 
     # pylint: disable=too-many-arguments,duplicate-code
@@ -964,20 +983,14 @@
 
     @contextmanager
     def single_write(self) -> \
             Generator[Self, None, None]:
         """
         Context manager to allow multiple field reads/write to be done with a single set of
         field operations
-
-        Args:
-
-
-        Returns:
-
         """
         with self._cached_access(verify=False, skip_write=False,
                                   skip_initial_read=True) as reg_array:
             yield reg_array
 
     @property
     def _is_readable(self) -> bool:
@@ -1014,33 +1027,29 @@
         if not isinstance(parent._callbacks, NormalCallbackSet):
             raise TypeError(f'callback set type is wrong, got {type(parent._callbacks)}')
 
         super().__init__(logger_handle=logger_handle, inst_name=inst_name,
                          parent=parent, address=address, width=width, accesswidth=accesswidth,
                          stride=stride, dimensions=dimensions, elements=elements)
 
-
     # pylint: enable=too-many-arguments,duplicate-code
 
     @contextmanager
     def single_read_modify_write(self, verify: bool = False, skip_write: bool = False) -> \
             Generator[Self, None, None]:
         """
         Context manager to allow multiple field reads/write to be done with a single set of
         field operations
 
         Args:
             verify (bool): very the write with a read afterwards
             skip_write (bool): skip the write back at the end
-
-        Returns:
-
         """
         with self._cached_access(verify=verify, skip_write=skip_write,
-                                  skip_initial_read=False) as reg_array:
+                                 skip_initial_read=False) as reg_array:
             yield reg_array
 
     @property
     def _is_readable(self) -> bool:
         # pylint: disable=duplicate-code
         return True
```

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/lib/utility_functions.py` & `peakrdl_python-0.7.5/src/peakrdl_python/lib/utility_functions.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/safe_name_utility.py` & `peakrdl_python-0.7.5/src/peakrdl_python/safe_name_utility.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/systemrdl_node_utility_functions.py` & `peakrdl_python-0.7.5/src/peakrdl_python/systemrdl_node_utility_functions.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/templates/__init__.py` & `peakrdl_python-0.7.5/src/peakrdl_python/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap.py.jinja` & `peakrdl_python-0.7.5/src/peakrdl_python/templates/addrmap.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_field.py.jinja` & `peakrdl_python-0.7.5/src/peakrdl_python/templates/addrmap_field.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_memory.py.jinja` & `peakrdl_python-0.7.5/src/peakrdl_python/templates/addrmap_memory.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_register.py.jinja` & `peakrdl_python-0.7.5/src/peakrdl_python/templates/addrmap_register.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_simulation.py.jinja` & `peakrdl_python-0.7.5/src/peakrdl_python/templates/addrmap_simulation.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_simulation_tb.jinja` & `peakrdl_python-0.7.5/src/peakrdl_python/templates/addrmap_simulation_tb.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/templates/addrmap_tb.py.jinja` & `peakrdl_python-0.7.5/src/peakrdl_python/templates/addrmap_tb.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/templates/baseclass_tb.py.jinja` & `peakrdl_python-0.7.5/src/peakrdl_python/templates/baseclass_tb.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/templates/header.py.jinja` & `peakrdl_python-0.7.5/src/peakrdl_python/templates/header.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/templates/header_tb.py.jinja` & `peakrdl_python-0.7.5/src/peakrdl_python/templates/header_tb.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python/templates/reg_definitions.py.jinja` & `peakrdl_python-0.7.5/src/peakrdl_python/templates/reg_definitions.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python.egg-info/PKG-INFO` & `peakrdl_python-0.7.5/src/peakrdl_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-python
-Version: 0.7.4
+Version: 0.7.5
 Summary: Generate Python Register Access Layer (RAL) from SystemRDL
 Author: Keith Brady
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `peakrdl-python-0.7.4/src/peakrdl_python.egg-info/SOURCES.txt` & `peakrdl_python-0.7.5/src/peakrdl_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/pylint.rc` & `peakrdl_python-0.7.5/tests/pylint.rc`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/addr_map.rdl` & `peakrdl_python-0.7.5/tests/testcases/addr_map.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/basic.rdl` & `peakrdl_python-0.7.5/tests/testcases/basic.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/block_a.xml` & `peakrdl_python-0.7.5/tests/testcases/block_a.xml`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/block_b.xml` & `peakrdl_python-0.7.5/tests/testcases/block_b.xml`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/different_array_types.rdl` & `peakrdl_python-0.7.5/tests/testcases/different_array_types.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/enum_example.rdl` & `peakrdl_python-0.7.5/tests/testcases/enum_example.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/example_issue_106.rdl` & `peakrdl_python-0.7.5/tests/testcases/example_issue_106.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/field_with_overridden_reset.rdl` & `peakrdl_python-0.7.5/tests/testcases/field_with_overridden_reset.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/fields_with_reset_values.rdl` & `peakrdl_python-0.7.5/tests/testcases/fields_with_reset_values.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/memories.rdl` & `peakrdl_python-0.7.5/tests/testcases/memories.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/msb0_and_lsb0.rdl` & `peakrdl_python-0.7.5/tests/testcases/msb0_and_lsb0.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/name_clash.rdl` & `peakrdl_python-0.7.5/tests/testcases/name_clash.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/overridden_python_name.rdl` & `peakrdl_python-0.7.5/tests/testcases/overridden_python_name.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/regfile_and_arrays.rdl` & `peakrdl_python-0.7.5/tests/testcases/regfile_and_arrays.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/same_but_different_enum.rdl` & `peakrdl_python-0.7.5/tests/testcases/same_but_different_enum.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/signals_definitions_at_various_levels.rdl` & `peakrdl_python-0.7.5/tests/testcases/signals_definitions_at_various_levels.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/simple.xml` & `peakrdl_python-0.7.5/tests/testcases/simple.xml`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/testcases/sizes_registers.rdl` & `peakrdl_python-0.7.5/tests/testcases/sizes_registers.rdl`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/unit_tests/simple_components.py` & `peakrdl_python-0.7.5/tests/unit_tests/simple_components.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/unit_tests/test_array_indexing.py` & `peakrdl_python-0.7.5/tests/unit_tests/test_array_indexing.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.7.4/tests/unit_tests/test_optimised_reg_array.py` & `peakrdl_python-0.7.5/tests/unit_tests/test_optimised_reg_array.py`

 * *Files identical despite different names*

