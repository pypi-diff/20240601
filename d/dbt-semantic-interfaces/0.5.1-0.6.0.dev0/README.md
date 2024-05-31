# Comparing `tmp/dbt_semantic_interfaces-0.5.1.tar.gz` & `tmp/dbt_semantic_interfaces-0.6.0.dev0.tar.gz`

## Comparing `dbt_semantic_interfaces-0.5.1.tar` & `dbt_semantic_interfaces-0.6.0.dev0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/Makefile
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dsi_pydantic_shim.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/__init__.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/call_parameter_sets.py
--rw-r--r--   0        0        0    18184 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/dataclass_serialization.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/enum_extension.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/errors.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/pretty_print.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/py.typed
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/references.py
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/__init__.py
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/base.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/export.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/metadata.py
--rw-r--r--   0        0        0     8643 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/metric.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/project_configuration.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/saved_query.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/semantic_manifest.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/semantic_model.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/semantic_version.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/elements/__init__.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/elements/dimension.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/elements/entity.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/elements/measure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/filters/__init__.py
--rw-r--r--   0        0        0     6590 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/filters/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/naming/__init__.py
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/naming/dundered.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/naming/keywords.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/__init__.py
--rw-r--r--   0        0        0    16345 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/dir_to_model.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/generate_json_schema_file.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/objects.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/schema_validator.py
--rw-r--r--   0        0        0    13881 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/schemas.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/yaml_loader.py
--rw-r--r--   0        0        0    21357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/where_filter/parameter_set_factory.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/where_filter/where_filter_dimension.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/where_filter/where_filter_entity.py
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/where_filter/where_filter_parser.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/where_filter/where_filter_time_dimension.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/__init__.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/dimension.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/entity.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/export.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/measure.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/metadata.py
--rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/metric.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/project_configuration.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/protocol_hint.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/query_interface.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/saved_query.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/semantic_manifest.py
--rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/semantic_model.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/semantic_version.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/time_spine_configuration.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/__init__.py
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/boolean_measure.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/convert_count.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/convert_median.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/names.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/proxy_measure.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/rule_set.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/transform_rule.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/type_enums/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/type_enums/aggregation_type.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/type_enums/conversion_calculation_type.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/type_enums/date_part.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/type_enums/dimension_type.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/type_enums/entity_type.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/type_enums/export_destination_type.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/type_enums/metric_type.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/type_enums/semantic_manifest_node_type.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/type_enums/time_granularity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/__init__.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/agg_time_dimension.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/common_entities.py
--rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/dimension_const.py
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/element_const.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/entities.py
--rw-r--r--   0        0        0     8971 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/labels.py
--rw-r--r--   0        0        0    28374 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/measures.py
--rw-r--r--   0        0        0    22911 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/metrics.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/non_empty.py
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/primary_entity.py
--rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/reserved_keywords.py
--rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/saved_query.py
--rw-r--r--   0        0        0     6627 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
--rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/semantic_models.py
--rw-r--r--   0        0        0    13193 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/unique_valid_name.py
--rw-r--r--   0        0        0    16109 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/validator_helpers.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/LICENSE
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/README.md
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/CHANGELOG.md
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/Makefile
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dsi_pydantic_shim.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/__init__.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/call_parameter_sets.py
+-rw-r--r--   0        0        0    18184 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/dataclass_serialization.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/enum_extension.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/errors.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/pretty_print.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/py.typed
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/references.py
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/__init__.py
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/base.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/export.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/metadata.py
+-rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/metric.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/project_configuration.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/saved_query.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/semantic_manifest.py
+-rw-r--r--   0        0        0     7959 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/semantic_model.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/semantic_version.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/elements/__init__.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/elements/dimension.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/elements/entity.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/elements/measure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/filters/__init__.py
+-rw-r--r--   0        0        0     6590 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/filters/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/naming/__init__.py
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/naming/dundered.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/naming/keywords.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/__init__.py
+-rw-r--r--   0        0        0    16345 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/dir_to_model.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/generate_json_schema_file.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/objects.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/schema_validator.py
+-rw-r--r--   0        0        0    14575 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/schemas.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/yaml_loader.py
+-rw-r--r--   0        0        0    22379 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/where_filter/parameter_set_factory.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/where_filter/where_filter_dimension.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/where_filter/where_filter_entity.py
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/where_filter/where_filter_parser.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/where_filter/where_filter_time_dimension.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/dimension.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/entity.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/export.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/measure.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/metadata.py
+-rw-r--r--   0        0        0     8404 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/metric.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/project_configuration.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/protocol_hint.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/query_interface.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/saved_query.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/semantic_manifest.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/semantic_model.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/semantic_version.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/time_spine_configuration.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/__init__.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/boolean_measure.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/convert_count.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/convert_median.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/names.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/proxy_measure.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/pydantic_rule_set.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/rule_set.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/transform_rule.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/type_enums/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/type_enums/aggregation_type.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/type_enums/conversion_calculation_type.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/type_enums/date_part.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/type_enums/dimension_type.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/type_enums/entity_type.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/type_enums/export_destination_type.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/type_enums/metric_type.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/type_enums/semantic_manifest_node_type.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/type_enums/time_granularity.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/__init__.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/agg_time_dimension.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/common_entities.py
+-rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/dimension_const.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/element_const.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/entities.py
+-rw-r--r--   0        0        0     8971 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/labels.py
+-rw-r--r--   0        0        0    28374 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/measures.py
+-rw-r--r--   0        0        0    25160 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/metrics.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/non_empty.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/primary_entity.py
+-rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/reserved_keywords.py
+-rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/saved_query.py
+-rw-r--r--   0        0        0     6627 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/semantic_manifest_validator.py
+-rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/semantic_models.py
+-rw-r--r--   0        0        0    13193 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/unique_valid_name.py
+-rw-r--r--   0        0        0    16109 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/validator_helpers.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/LICENSE
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/README.md
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.6.0.dev0/PKG-INFO
```

### Comparing `dbt_semantic_interfaces-0.5.1/Makefile` & `dbt_semantic_interfaces-0.6.0.dev0/Makefile`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dsi_pydantic_shim.py` & `dbt_semantic_interfaces-0.6.0.dev0/dsi_pydantic_shim.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/call_parameter_sets.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/call_parameter_sets.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/dataclass_serialization.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/dataclass_serialization.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/enum_extension.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/enum_extension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/errors.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/errors.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/pretty_print.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/pretty_print.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/references.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/references.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/test_utils.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/base.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/base.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/export.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/export.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/metric.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
-from typing import List, Optional, Sequence
+from typing import Any, Dict, List, Optional, Sequence
+
+from typing_extensions import override
 
 from dbt_semantic_interfaces.enum_extension import assert_values_exhausted
 from dbt_semantic_interfaces.errors import ParsingException
 from dbt_semantic_interfaces.implementations.base import (
     HashableBaseModel,
     ModelWithMetadataParsing,
     PydanticCustomInputParser,
     PydanticParseableValueType,
 )
 from dbt_semantic_interfaces.implementations.filters.where_filter import (
     PydanticWhereFilterIntersection,
 )
 from dbt_semantic_interfaces.implementations.metadata import PydanticMetadata
+from dbt_semantic_interfaces.protocols import MetricConfig, ProtocolHint
 from dbt_semantic_interfaces.references import MeasureReference, MetricReference
 from dbt_semantic_interfaces.type_enums import (
     ConversionCalculationType,
     MetricType,
     TimeGranularity,
 )
 from dsi_pydantic_shim import Field
@@ -166,24 +169,33 @@
     grain_to_date: Optional[TimeGranularity]
     metrics: Optional[List[PydanticMetricInput]]
     conversion_type_params: Optional[PydanticConversionTypeParams]
 
     input_measures: List[PydanticMetricInputMeasure] = Field(default_factory=list)
 
 
+class PydanticMetricConfig(HashableBaseModel, ProtocolHint[MetricConfig]):  # noqa: D
+    @override
+    def _implements_protocol(self) -> MetricConfig:  # noqa: D
+        return self
+
+    meta: Dict[str, Any] = Field(default_factory=dict)
+
+
 class PydanticMetric(HashableBaseModel, ModelWithMetadataParsing):
     """Describes a metric."""
 
     name: str
     description: Optional[str]
     type: MetricType
     type_params: PydanticMetricTypeParams
     filter: Optional[PydanticWhereFilterIntersection]
     metadata: Optional[PydanticMetadata]
     label: Optional[str] = None
+    config: Optional[PydanticMetricConfig]
 
     @property
     def input_measures(self) -> Sequence[PydanticMetricInputMeasure]:
         """Return the complete list of input measure configurations for this metric."""
         return self.type_params.input_measures
 
     @property
```

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/project_configuration.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/project_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/saved_query.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/saved_query.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/semantic_manifest.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/semantic_model.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/semantic_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from __future__ import annotations
 
-from typing import Any, List, Optional, Sequence
+from typing import Any, Dict, List, Optional, Sequence
 
 from typing_extensions import override
 
 from dbt_semantic_interfaces.implementations.base import (
     HashableBaseModel,
     ModelWithMetadataParsing,
 )
 from dbt_semantic_interfaces.implementations.elements.dimension import PydanticDimension
 from dbt_semantic_interfaces.implementations.elements.entity import PydanticEntity
 from dbt_semantic_interfaces.implementations.elements.measure import PydanticMeasure
 from dbt_semantic_interfaces.implementations.metadata import PydanticMetadata
 from dbt_semantic_interfaces.protocols import (
     ProtocolHint,
     SemanticModel,
+    SemanticModelConfig,
     SemanticModelDefaults,
 )
 from dbt_semantic_interfaces.references import (
     EntityReference,
     LinkableElementReference,
     MeasureReference,
     SemanticModelReference,
     TimeDimensionReference,
 )
-from dsi_pydantic_shim import validator
+from dsi_pydantic_shim import Field, validator
 
 
 class NodeRelation(HashableBaseModel):
     """Path object to where the data should be."""
 
     alias: str
     schema_name: str
@@ -72,14 +73,22 @@
     @override
     def _implements_protocol(self) -> SemanticModelDefaults:  # noqa: D
         return self
 
     agg_time_dimension: Optional[str]
 
 
+class PydanticSemanticModelConfig(HashableBaseModel, ProtocolHint[SemanticModelConfig]):  # noqa: D
+    @override
+    def _implements_protocol(self) -> SemanticModelConfig:  # noqa: D
+        return self
+
+    meta: Dict[str, Any] = Field(default_factory=dict)
+
+
 class PydanticSemanticModel(HashableBaseModel, ModelWithMetadataParsing, ProtocolHint[SemanticModel]):
     """Describes a semantic model."""
 
     @override
     def _implements_protocol(self) -> SemanticModel:
         return self
 
@@ -91,14 +100,15 @@
     primary_entity: Optional[str]
     entities: Sequence[PydanticEntity] = []
     measures: Sequence[PydanticMeasure] = []
     dimensions: Sequence[PydanticDimension] = []
     label: Optional[str] = None
 
     metadata: Optional[PydanticMetadata]
+    config: Optional[PydanticSemanticModelConfig]
 
     @property
     def entity_references(self) -> List[LinkableElementReference]:  # noqa: D
         return [i.reference for i in self.entities]
 
     @property
     def dimension_references(self) -> List[LinkableElementReference]:  # noqa: D
```

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/semantic_version.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/semantic_version.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/time_spine_table_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/elements/dimension.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/elements/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/elements/entity.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/elements/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/elements/measure.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/elements/measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/implementations/filters/where_filter.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/implementations/filters/where_filter.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/naming/dundered.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/naming/dundered.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 element_name=name_parts[-1],
             )
 
     @property
     def dundered_name(self) -> str:
         """Return the full name form. e.g. ds or listing__ds__month."""
         items = [entity_reference.element_name for entity_reference in self.entity_links] + [self.element_name]
-        if self.time_granularity and self.time_granularity != TimeGranularity.DAY:
+        if self.time_granularity:
             items.append(self.time_granularity.value)
         return DUNDER.join(items)
 
     @property
     def dundered_name_without_granularity(self) -> str:
         """Return the name without the time granularity. e.g. listing__ds__month -> listing__ds."""
         return DUNDER.join(
```

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/dir_to_model.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/dir_to_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/generate_json_schema_file.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/generate_json_schema_file.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/objects.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/objects.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/schema_validator.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/schema_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/schemas.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,28 +248,38 @@
             "required": ["type"],
         },
     },
     "additionalProperties": False,
     "required": ["name", "type"],
 }
 
+metric_config_schema = {
+    "$id": "metric_config_schema",
+    "type": "object",
+    "properties": {
+        "meta": {"type": "object", "propertyNames": {"type": "string"}},
+    },
+    "additionalProperties": False,
+}
+
 # Top level object schemas
 metric_schema = {
     "$id": "metric_schema",
     "type": "object",
     "properties": {
         "name": {
             "type": "string",
             "pattern": TRANSFORM_OBJECT_NAME_PATTERN,
         },
         "type": {"enum": metric_types_enum_values},
         "type_params": {"$ref": "metric_type_params"},
         "filter": {"$ref": "filter_schema"},
         "description": {"type": "string"},
         "label": {"type": "string"},
+        "config": {"$ref": "metric_config_schema"},
     },
     "additionalProperties": False,
     "required": ["name", "type", "type_params"],
 }
 
 node_relation_schema = {
     "$id": "node_relation_schema",
@@ -374,14 +384,23 @@
         "label": {"type": "string"},
         "exports": {"type": "array", "items": {"$ref": "export_schema"}},
     },
     "required": ["name", "query_params"],
     "additionalProperties": False,
 }
 
+semantic_model_config_schema = {
+    "$id": "semantic_model_config_schema",
+    "type": "object",
+    "properties": {
+        "meta": {"type": "object", "propertyNames": {"type": "string"}},
+    },
+    "additionalProperties": False,
+}
+
 semantic_model_schema = {
     "$id": "semantic_model_schema",
     "type": "object",
     "properties": {
         "name": {
             "type": "string",
             "pattern": TRANSFORM_OBJECT_NAME_PATTERN,
@@ -392,14 +411,15 @@
             "type": "string",
         },
         "entities": {"type": "array", "items": {"$ref": "entity_schema"}},
         "measures": {"type": "array", "items": {"$ref": "measure_schema"}},
         "dimensions": {"type": "array", "items": {"$ref": "dimension_schema"}},
         "description": {"type": "string"},
         "label": {"type": "string"},
+        "config": {"$ref": "semantic_model_config_schema"},
     },
     "additionalProperties": False,
     "required": ["name"],
 }
 
 
 schema_store = {
@@ -424,14 +444,16 @@
     metric_input_schema["$id"]: metric_input_schema,
     node_relation_schema["$id"]: node_relation_schema,
     semantic_model_defaults_schema["$id"]: semantic_model_defaults_schema,
     time_spine_table_configuration_schema["$id"]: time_spine_table_configuration_schema,
     export_schema["$id"]: export_schema,
     export_config_schema["$id"]: export_config_schema,
     saved_query_query_params_schema["$id"]: saved_query_query_params_schema,
+    semantic_model_config_schema["$id"]: semantic_model_config_schema,
+    metric_config_schema["$id"]: metric_config_schema,
 }
 
 resources: List[Tuple[str, Resource]] = [(str(k), DRAFT7.create_resource(v)) for k, v in schema_store.items()]
 registry: Registry = Registry().with_resources(resources)
 semantic_model_validator = SchemaValidator(semantic_model_schema, registry=registry)
 metric_validator = SchemaValidator(metric_schema, registry=registry)
 project_configuration_validator = SchemaValidator(project_configuration_schema, registry=registry)
```

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/yaml_loader.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/generated_json_schemas/default_explicit_schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9922609890109889%*

 * *Differences: {"'definitions'": "{'metric_schema': {'properties': {'config': OrderedDict([('$ref', "*

 * *                  "'#/definitions/metric_config_schema')])}}, 'semantic_model_schema': "*

 * *                  "{'properties': {'config': OrderedDict([('$ref', "*

 * *                  "'#/definitions/semantic_model_config_schema')])}}, 'metric_config_schema': "*

 * *                  "OrderedDict([('$id', 'metric_config_schema'), ('additionalProperties', False), "*

 * *                  "('properties', OrderedDict([('meta', OrderedDict([(' […]*

```diff
@@ -324,14 +324,27 @@
             },
             "required": [
                 "name",
                 "agg"
             ],
             "type": "object"
         },
+        "metric_config_schema": {
+            "$id": "metric_config_schema",
+            "additionalProperties": false,
+            "properties": {
+                "meta": {
+                    "propertyNames": {
+                        "type": "string"
+                    },
+                    "type": "object"
+                }
+            },
+            "type": "object"
+        },
         "metric_input_measure_schema": {
             "$id": "metric_input_measure_schema",
             "oneOf": [
                 {
                     "type": "string"
                 },
                 {
@@ -379,14 +392,17 @@
             },
             "type": "object"
         },
         "metric_schema": {
             "$id": "metric_schema",
             "additionalProperties": false,
             "properties": {
+                "config": {
+                    "$ref": "#/definitions/metric_config_schema"
+                },
                 "description": {
                     "type": "string"
                 },
                 "filter": {
                     "$ref": "#/definitions/filter_schema"
                 },
                 "label": {
@@ -574,14 +590,27 @@
             },
             "required": [
                 "name",
                 "query_params"
             ],
             "type": "object"
         },
+        "semantic_model_config_schema": {
+            "$id": "semantic_model_config_schema",
+            "additionalProperties": false,
+            "properties": {
+                "meta": {
+                    "propertyNames": {
+                        "type": "string"
+                    },
+                    "type": "object"
+                }
+            },
+            "type": "object"
+        },
         "semantic_model_defaults_schema": {
             "$id": "semantic_model_defaults_schema",
             "additionalProperties": false,
             "properties": {
                 "agg_time_dimension": {
                     "type": "string"
                 }
@@ -589,14 +618,17 @@
             "required": [],
             "type": "object"
         },
         "semantic_model_schema": {
             "$id": "semantic_model_schema",
             "additionalProperties": false,
             "properties": {
+                "config": {
+                    "$ref": "#/definitions/semantic_model_config_schema"
+                },
                 "defaults": {
                     "$ref": "#/definitions/semantic_model_defaults_schema"
                 },
                 "description": {
                     "type": "string"
                 },
                 "dimensions": {
```

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/where_filter/parameter_set_factory.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/where_filter/parameter_set_factory.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/where_filter/where_filter_dimension.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/where_filter/where_filter_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/where_filter/where_filter_entity.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/where_filter/where_filter_entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/where_filter/where_filter_parser.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/where_filter/where_filter_parser.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/parsing/where_filter/where_filter_time_dimension.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/parsing/where_filter/where_filter_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/__init__.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,29 @@
     NonAdditiveDimensionParameters,
 )
 from dbt_semantic_interfaces.protocols.metadata import FileSlice, Metadata  # noqa:F401
 from dbt_semantic_interfaces.protocols.metric import (  # noqa:F401
     ConstantPropertyInput,
     ConversionTypeParams,
     Metric,
+    MetricConfig,
     MetricInput,
     MetricInputMeasure,
     MetricTimeWindow,
     MetricTypeParams,
 )
 from dbt_semantic_interfaces.protocols.protocol_hint import ProtocolHint  # noqa:F401
 from dbt_semantic_interfaces.protocols.saved_query import SavedQuery  # noqa:F401
 from dbt_semantic_interfaces.protocols.semantic_manifest import (  # noqa:F401
     SemanticManifest,
     SemanticManifestT,
 )
 from dbt_semantic_interfaces.protocols.semantic_model import (  # noqa:F401
     SemanticModel,
+    SemanticModelConfig,
     SemanticModelDefaults,
     SemanticModelT,
 )
 from dbt_semantic_interfaces.protocols.where_filter import (  # noqa:F401
     WhereFilter,
     WhereFilterIntersection,
 )
```

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/dimension.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/entity.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/export.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/export.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/measure.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/metadata.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/metric.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from abc import abstractmethod
-from typing import Optional, Protocol, Sequence
+from typing import Any, Dict, Optional, Protocol, Sequence
 
 from dbt_semantic_interfaces.protocols.metadata import Metadata
 from dbt_semantic_interfaces.protocols.where_filter import WhereFilterIntersection
 from dbt_semantic_interfaces.references import MeasureReference, MetricReference
 from dbt_semantic_interfaces.type_enums import (
     ConversionCalculationType,
     MetricType,
@@ -224,14 +224,24 @@
 
     @property
     @abstractmethod
     def conversion_type_params(self) -> Optional[ConversionTypeParams]:  # noqa: D
         pass
 
 
+class MetricConfig(Protocol):  # noqa: D
+    """The config property allows you to configure additional resources/metadata."""
+
+    @property
+    @abstractmethod
+    def meta(self) -> Dict[str, Any]:
+        """The meta field can be used to set metadata for a resource."""
+        pass
+
+
 class Metric(Protocol):
     """Describes a metric."""
 
     @property
     @abstractmethod
     def name(self) -> str:  # noqa: D
         pass
@@ -278,10 +288,15 @@
     @property
     @abstractmethod
     def metadata(self) -> Optional[Metadata]:  # noqa: D
         pass
 
     @property
     @abstractmethod
+    def config(self) -> Optional[MetricConfig]:  # noqa: D
+        pass
+
+    @property
+    @abstractmethod
     def label(self) -> Optional[str]:
         """Returns a string representing a human readable label for the metric."""
         pass
```

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/project_configuration.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/project_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/protocol_hint.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/protocol_hint.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/query_interface.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/query_interface.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/saved_query.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/saved_query.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/semantic_manifest.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/semantic_model.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/semantic_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from abc import abstractmethod
-from typing import Optional, Protocol, Sequence, TypeVar
+from typing import Any, Dict, Optional, Protocol, Sequence, TypeVar
 
 from dbt_semantic_interfaces.protocols.dimension import Dimension
 from dbt_semantic_interfaces.protocols.entity import Entity
 from dbt_semantic_interfaces.protocols.measure import Measure
 from dbt_semantic_interfaces.protocols.metadata import Metadata
 from dbt_semantic_interfaces.references import (
     EntityReference,
@@ -46,14 +46,24 @@
     @property
     @abstractmethod
     def agg_time_dimension(self) -> Optional[str]:
         """The aggregation time dimension to use for a measure if one was not specified."""
         pass
 
 
+class SemanticModelConfig(Protocol):  # noqa: D
+    """The config property allows you to configure additional resources/metadata."""
+
+    @property
+    @abstractmethod
+    def meta(self) -> Dict[str, Any]:
+        """The meta field can be used to set metadata for a resource."""
+        pass
+
+
 class SemanticModel(Protocol):
     """Describes a semantic model."""
 
     @property
     @abstractmethod
     def name(self) -> str:  # noqa: D
         pass
@@ -155,14 +165,19 @@
         ...
 
     @property
     @abstractmethod
     def metadata(self) -> Optional[Metadata]:  # noqa: D
         pass
 
+    @property
+    @abstractmethod
+    def config(self) -> Optional[SemanticModelConfig]:  # noqa: D
+        pass
+
     @abstractmethod
     def checked_agg_time_dimension_for_measure(self, measure_reference: MeasureReference) -> TimeDimensionReference:
         """Returns the `TimeDimensionReference` what a measure should use for it's `agg_time_dimension`.
 
         Should raise an exception if a TimeDimensionReference cannot be built
         """
         ...
```

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/time_spine_configuration.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/time_spine_configuration.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/protocols/where_filter.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/protocols/where_filter.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/add_input_metric_measures.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/add_input_metric_measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/boolean_measure.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/boolean_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/convert_count.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/convert_count.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/convert_median.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/convert_median.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/names.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/names.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/proxy_measure.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/proxy_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/pydantic_rule_set.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/pydantic_rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/rule_set.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/rule_set.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/semantic_manifest_transformer.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/transformations/transform_rule.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/transformations/transform_rule.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/type_enums/__init__.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/type_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/type_enums/date_part.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/type_enums/date_part.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/agg_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/common_entities.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/common_entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/dimension_const.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/dimension_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/element_const.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/element_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/entities.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/labels.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/labels.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/measures.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/metrics.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,16 +83,17 @@
         issues: List[ValidationIssue] = []
 
         if metric.type == MetricType.DERIVED:
             metric_context = MetricContext(
                 file_context=FileContext.from_metadata(metadata=metric.metadata),
                 metric=MetricModelReference(metric_name=metric.name),
             )
-            used_names = {input_metric.name for input_metric in metric.input_metrics}
-            for input_metric in metric.input_metrics:
+            input_metrics = metric.type_params.metrics or []
+            used_names = {input_metric.name for input_metric in input_metrics}
+            for input_metric in input_metrics:
                 if input_metric.alias:
                     issues += UniqueAndValidNameRule.check_valid_name(input_metric.alias, metric_context)
                     if input_metric.alias in used_names:
                         issues.append(
                             ValidationError(
                                 context=metric_context,
                                 message=f"Alias '{input_metric.alias}' for input metric: '{input_metric.name}' is "
@@ -105,35 +106,44 @@
     @staticmethod
     @validate_safely(whats_being_done="checking that the input metrics exist")
     def _validate_input_metrics_exist(semantic_manifest: SemanticManifest) -> List[ValidationIssue]:
         issues: List[ValidationIssue] = []
 
         all_metrics = {m.name for m in semantic_manifest.metrics}
         for metric in semantic_manifest.metrics:
+            metric_context = MetricContext(
+                file_context=FileContext.from_metadata(metadata=metric.metadata),
+                metric=MetricModelReference(metric_name=metric.name),
+            )
             if metric.type == MetricType.DERIVED:
-                for input_metric in metric.input_metrics:
+                if not metric.type_params.metrics:
+                    issues.append(
+                        ValidationError(
+                            context=metric_context,
+                            message=f"No input metrics found for derived metric '{metric.name}'. "
+                            "Please add metrics to type_params.metrics.",
+                        )
+                    )
+                for input_metric in metric.type_params.metrics or []:
                     if input_metric.name not in all_metrics:
                         issues.append(
                             ValidationError(
-                                context=MetricContext(
-                                    file_context=FileContext.from_metadata(metadata=metric.metadata),
-                                    metric=MetricModelReference(metric_name=metric.name),
-                                ),
+                                context=metric_context,
                                 message=f"For metric: {metric.name}, input metric: '{input_metric.name}' does not "
                                 "exist as a configured metric in the model.",
                             )
                         )
         return issues
 
     @staticmethod
     @validate_safely(whats_being_done="checking that input metric time offset params are valid")
     def _validate_time_offset_params(metric: Metric) -> List[ValidationIssue]:
         issues: List[ValidationIssue] = []
 
-        for input_metric in metric.input_metrics or []:
+        for input_metric in metric.type_params.metrics or []:
             if input_metric.offset_window and input_metric.offset_to_grain:
                 issues.append(
                     ValidationError(
                         context=MetricContext(
                             file_context=FileContext.from_metadata(metadata=metric.metadata),
                             metric=MetricModelReference(metric_name=metric.name),
                         ),
@@ -141,24 +151,59 @@
                         f"input metric '{input_metric.name}'. Please set one or the other.",
                     )
                 )
 
         return issues
 
     @staticmethod
+    @validate_safely(whats_being_done="checking that the expr field uses the input metrics")
+    def _validate_expr(metric: Metric) -> List[ValidationIssue]:
+        issues: List[ValidationIssue] = []
+
+        if metric.type == MetricType.DERIVED:
+            if not metric.type_params.expr:
+                issues.append(
+                    ValidationError(
+                        context=MetricContext(
+                            file_context=FileContext.from_metadata(metadata=metric.metadata),
+                            metric=MetricModelReference(metric_name=metric.name),
+                        ),
+                        message=f"No expr set for derived metric {metric.name}. "
+                        "Please add an expr that references all input metrics.",
+                    )
+                )
+            else:
+                for input_metric in metric.type_params.metrics or []:
+                    name = input_metric.alias or input_metric.name
+                    if name not in metric.type_params.expr:
+                        issues.append(
+                            ValidationError(
+                                context=MetricContext(
+                                    file_context=FileContext.from_metadata(metadata=metric.metadata),
+                                    metric=MetricModelReference(metric_name=metric.name),
+                                ),
+                                message=f"Input metric '{name}' is not used in expr: '{metric.type_params.expr}' for "
+                                f"derived metric '{metric.name}'. Please update the expr or remove the input metric.",
+                            )
+                        )
+
+        return issues
+
+    @staticmethod
     @validate_safely(
         whats_being_done="running model validation ensuring derived metrics properties are configured properly"
     )
     def validate_manifest(semantic_manifest: SemanticManifestT) -> Sequence[ValidationIssue]:  # noqa: D
         issues: List[ValidationIssue] = []
 
         issues += DerivedMetricRule._validate_input_metrics_exist(semantic_manifest=semantic_manifest)
         for metric in semantic_manifest.metrics or []:
             issues += DerivedMetricRule._validate_alias_collision(metric=metric)
             issues += DerivedMetricRule._validate_time_offset_params(metric=metric)
+            issues += DerivedMetricRule._validate_expr(metric=metric)
         return issues
 
 
 class WhereFiltersAreParseable(SemanticManifestValidationRule[SemanticManifestT], Generic[SemanticManifestT]):
     """Validates that all Metric WhereFilters are parseable."""
 
     @staticmethod
```

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/non_empty.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/non_empty.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/primary_entity.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/primary_entity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/reserved_keywords.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/saved_query.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/saved_query.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/semantic_manifest_validator.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/semantic_manifest_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/semantic_models.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/semantic_models.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/unique_valid_name.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/unique_valid_name.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/dbt_semantic_interfaces/validations/validator_helpers.py` & `dbt_semantic_interfaces-0.6.0.dev0/dbt_semantic_interfaces/validations/validator_helpers.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/.gitignore` & `dbt_semantic_interfaces-0.6.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/LICENSE` & `dbt_semantic_interfaces-0.6.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/README.md` & `dbt_semantic_interfaces-0.6.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.5.1/pyproject.toml` & `dbt_semantic_interfaces-0.6.0.dev0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbt-semantic-interfaces"
-version = "0.5.1"
+version = "0.6.0dev0"
 description = 'The shared semantic layer definitions that dbt-core and MetricFlow use'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "dbt Labs", email = "info@dbtlabs.com" },
```

### Comparing `dbt_semantic_interfaces-0.5.1/PKG-INFO` & `dbt_semantic_interfaces-0.6.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dbt-semantic-interfaces
-Version: 0.5.1
+Version: 0.6.0.dev0
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs <info@dbtlabs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.3 Name: dbt-semantic-interfaces Version: 0.5.1 Summary: The
-shared semantic layer definitions that dbt-core and MetricFlow use Author-
-email: dbt Labs
+Metadata-Version: 2.3 Name: dbt-semantic-interfaces Version: 0.6.0.dev0
+Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
+Author-email: dbt Labs
 dbtlabs.com> License-Expression: Apache-2.0 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
```

