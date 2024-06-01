# Comparing `tmp/oaklib-0.6.6.tar.gz` & `tmp/oaklib-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaklib-0.6.6.tar", max compression
+gzip compressed data, was "oaklib-0.6.7.tar", max compression
```

## Comparing `oaklib-0.6.6.tar` & `oaklib-0.6.7.tar`

### file list

```diff
@@ -1,316 +1,319 @@
--rw-r--r--   0        0        0    11357 2024-05-09 23:39:19.984135 oaklib-0.6.6/LICENSE
--rw-r--r--   0        0        0     7258 2024-05-09 23:39:19.984135 oaklib-0.6.6/README.md
--rw-r--r--   0        0        0     3599 2024-05-09 23:39:53.832227 oaklib-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      272 2024-05-09 23:39:20.152136 oaklib-0.6.6/src/oaklib/__init__.py
--rw-r--r--   0        0        0   231525 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/cli.py
--rw-r--r--   0        0        0       64 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/__init__.py
--rw-r--r--   0        0        0      372 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/go-human-input-spec.yaml
--rw-r--r--   0        0        0      162 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/go-pombase-input-spec.yaml
--rw-r--r--   0        0        0      109 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/hpoa-g2p-input-spec.yaml
--rw-r--r--   0        0        0      106 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/hpoa-input-spec.yaml
--rw-r--r--   0        0        0     1903 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
--rw-r--r--   0        0        0     1011 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/mondo-g2d-input-spec.yaml
--rw-r--r--   0        0        0      109 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/mondo-gencc-input-spec.yaml
--rw-r--r--   0        0        0      529 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml
--rw-r--r--   0        0        0      118 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
--rw-r--r--   0        0        0     4730 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/obograph-style.json
--rw-r--r--   0        0        0      256 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/omo-to-skos.sssom.tsv
--rw-r--r--   0        0        0      131 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/conf/value-set-expander.conf.yaml
--rw-r--r--   0        0        0      149 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/constants.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/converters/__init__.py
--rw-r--r--   0        0        0     1461 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/converters/data_model_converter.py
--rw-r--r--   0        0        0     2547 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/converters/logical_definition_flattener.py
--rw-r--r--   0        0        0     2446 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/converters/obo_graph_to_cx_converter.py
--rw-r--r--   0        0        0    12105 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/converters/obo_graph_to_fhir_converter.py
--rw-r--r--   0        0        0     7719 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/converters/obo_graph_to_obo_format_converter.py
--rw-r--r--   0        0        0     6100 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
--rw-r--r--   0        0        0       60 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/__init__.py
--rw-r--r--   0        0        0     4034 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/association.owl.ttl
--rw-r--r--   0        0        0    38339 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/association.py
--rw-r--r--   0        0        0    13058 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/association.yaml
--rw-r--r--   0        0        0     6165 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/class_enrichment.owl.ttl
--rw-r--r--   0        0        0    13288 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/class_enrichment.py
--rw-r--r--   0        0        0     3262 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/class_enrichment.yaml
--rw-r--r--   0        0        0    19083 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
--rw-r--r--   0        0        0    24250 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/cross_ontology_diff.py
--rw-r--r--   0        0        0    10687 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/cross_ontology_diff.yaml
--rw-r--r--   0        0        0    29418 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/cx.py
--rw-r--r--   0        0        0     6314 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/cx.yaml
--rw-r--r--   0        0        0    15826 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/fhir.owl.ttl
--rw-r--r--   0        0        0    35746 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/fhir.py
--rw-r--r--   0        0        0     5064 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/fhir.yaml
--rw-r--r--   0        0        0    14566 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/input_specification.py
--rw-r--r--   0        0        0     3560 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/input_specification.yaml
--rw-r--r--   0        0        0    15776 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/item_list.py
--rw-r--r--   0        0        0     6339 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/item_list.yaml
--rw-r--r--   0        0        0     8984 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/lexical_index.owl.ttl
--rw-r--r--   0        0        0    17296 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/lexical_index.py
--rw-r--r--   0        0        0     6429 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/lexical_index.schema.json
--rw-r--r--   0        0        0     4016 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/lexical_index.yaml
--rw-r--r--   0        0        0    26474 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/mapping_cluster_datamodel.py
--rw-r--r--   0        0        0     7317 2024-05-09 23:39:20.156136 oaklib-0.6.6/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
--rw-r--r--   0        0        0   226115 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
--rw-r--r--   0        0        0    33955 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.py
--rw-r--r--   0        0        0    12889 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
--rw-r--r--   0        0        0     4155 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.yaml
--rw-r--r--   0        0        0    25354 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/obograph.owl.ttl
--rw-r--r--   0        0        0    51109 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/obograph.py
--rw-r--r--   0        0        0    22375 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/obograph.schema.json
--rw-r--r--   0        0        0    19600 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/obograph.yaml
--rw-r--r--   0        0        0    59793 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.owl.ttl
--rw-r--r--   0        0        0   116914 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.py
--rw-r--r--   0        0        0    95288 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.schema.json
--rw-r--r--   0        0        0    31452 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.yaml
--rw-r--r--   0        0        0    14759 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/oxo.owl.ttl
--rw-r--r--   0        0        0    21914 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/oxo.py
--rw-r--r--   0        0        0     4392 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/oxo.yaml
--rw-r--r--   0        0        0     3348 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/search.py
--rw-r--r--   0        0        0    16948 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/search_datamodel.owl.ttl
--rw-r--r--   0        0        0    25157 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/search_datamodel.py
--rw-r--r--   0        0        0     6684 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/search_datamodel.yaml
--rw-r--r--   0        0        0      287 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/settings.py
--rw-r--r--   0        0        0    12826 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/similarity.owl.ttl
--rw-r--r--   0        0        0    22645 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/similarity.py
--rw-r--r--   0        0        0     5690 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/similarity.yaml
--rw-r--r--   0        0        0    31217 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
--rw-r--r--   0        0        0    50743 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.py
--rw-r--r--   0        0        0    21176 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
--rw-r--r--   0        0        0    16246 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.yaml
--rw-r--r--   0        0        0    23481 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/synonymizer_datamodel.py
--rw-r--r--   0        0        0     2476 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/synonymizer_datamodel.yaml
--rw-r--r--   0        0        0     9909 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/taxon_constraints.owl.ttl
--rw-r--r--   0        0        0    18432 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/taxon_constraints.py
--rw-r--r--   0        0        0     5880 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/taxon_constraints.yaml
--rw-r--r--   0        0        0    11599 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/text_annotator.owl.ttl
--rw-r--r--   0        0        0    21645 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/text_annotator.py
--rw-r--r--   0        0        0     2464 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/text_annotator.schema.json
--rw-r--r--   0        0        0     4996 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/text_annotator.yaml
--rw-r--r--   0        0        0    13670 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.owl.ttl
--rw-r--r--   0        0        0    33912 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.py
--rw-r--r--   0        0        0    10783 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.schema.json
--rw-r--r--   0        0        0     9005 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.yaml
--rw-r--r--   0        0        0     6640 2024-05-09 23:39:20.160136 oaklib-0.6.6/src/oaklib/datamodels/value_set_configuration.owl.ttl
--rw-r--r--   0        0        0     8458 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/datamodels/value_set_configuration.py
--rw-r--r--   0        0        0     2276 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/datamodels/value_set_configuration.yaml
--rw-r--r--   0        0        0     6549 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/datamodels/vocabulary.py
--rw-r--r--   0        0        0     6452 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/aggregator/__init__.py
--rw-r--r--   0        0        0     6377 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/aggregator/aggregator_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/agrkb/__init__.py
--rw-r--r--   0        0        0     8848 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/agrkb/agrkb_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/amigo/__init__.py
--rw-r--r--   0        0        0    16195 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/amigo/amigo_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/cx/__init__.py
--rw-r--r--   0        0        0     1985 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/cx/cx_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/eutils/__init__.py
--rw-r--r--   0        0        0     2180 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/eutils/eutils_implementation.py
--rw-r--r--   0        0        0     1055 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/eutils/pubmed_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/fhir/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/funowl/__init__.py
--rw-r--r--   0        0        0     8473 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/funowl/funowl_implementation.py
--rw-r--r--   0        0        0     3565 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/gilda.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/kgx/__init__.py
--rw-r--r--   0        0        0    30523 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/kgx/kgx_implementation.py
--rw-r--r--   0        0        0    28777 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/llm_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/monarch/__init__.py
--rw-r--r--   0        0        0     7034 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/monarch/monarch_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ncbi/__init__.py
--rw-r--r--   0        0        0     7034 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/neo4j/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/obograph/__init__.py
--rw-r--r--   0        0        0    17122 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/obograph/obograph_implementation.py
--rw-r--r--   0        0        0      267 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ols/__init__.py
--rw-r--r--   0        0        0      132 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ols/constants.py
--rw-r--r--   0        0        0     8071 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ols/ols_implementation.py
--rw-r--r--   0        0        0      686 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ols/oxo_utils.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontobee/__init__.py
--rw-r--r--   0        0        0     2641 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontobee/ontobee_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontoportal/__init__.py
--rw-r--r--   0        0        0      382 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontoportal/agroportal_implementation.py
--rw-r--r--   0        0        0     1250 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontoportal/bioportal_implementation.py
--rw-r--r--   0        0        0      378 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
--rw-r--r--   0        0        0      378 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontoportal/matportal_implementation.py
--rw-r--r--   0        0        0    13670 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/owlery/__init__.py
--rw-r--r--   0        0        0      427 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/owlery/owlery_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/pantherdb/__init__.py
--rw-r--r--   0        0        0    12625 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/pantherdb/pantherdb_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/pronto/__init__.py
--rw-r--r--   0        0        0    37863 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/pronto/pronto_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/robot/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/scigraph/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/semsimian/__init__.py
--rw-r--r--   0        0        0      247 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/semsimian/profiler.py
--rw-r--r--   0        0        0    11605 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/semsimian/semsimian_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/simpleobo/__init__.py
--rw-r--r--   0        0        0    46328 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
--rw-r--r--   0        0        0    23081 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/simpleobo/simple_obo_parser.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/skos/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/solor/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/solr/__init__.py
--rw-r--r--   0        0        0       96 2024-05-09 23:39:20.164136 oaklib-0.6.6/src/oaklib/implementations/sparql/__init__.py
--rw-r--r--   0        0        0    38067 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
--rw-r--r--   0        0        0      885 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sparql/lov_implementation.py
--rw-r--r--   0        0        0     1721 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
--rw-r--r--   0        0        0     2658 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sparql/sparql_implementation.py
--rw-r--r--   0        0        0     2325 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sparql/sparql_query.py
--rw-r--r--   0        0        0       96 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sqldb/__init__.py
--rw-r--r--   0        0        0   115796 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sqldb/sql_implementation.py
--rw-r--r--   0        0        0     1903 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/sqldb/sqlite_utils.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/tabular/__init__.py
--rw-r--r--   0        0        0    19432 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/tabular/robot_template_implementation.py
--rw-r--r--   0        0        0     3279 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/tabular/tabular_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/tccm/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/translator/__init__.py
--rw-r--r--   0        0        0     5442 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/translator/translator_implementation.py
--rw-r--r--   0        0        0      108 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/ubergraph/__init__.py
--rw-r--r--   0        0        0    20090 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/umls/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/uniprot/__init__.py
--rw-r--r--   0        0        0    14740 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/uniprot/uniprot_implementation.py
--rw-r--r--   0        0        0       96 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/wikidata/__init__.py
--rw-r--r--   0        0        0    17267 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/implementations/wikidata/wikidata_implementation.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/indexes/__init__.py
--rw-r--r--   0        0        0     3089 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/indexes/edge_index.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/inference/__init__.py
--rw-r--r--   0        0        0      748 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/inference/owl_reasoner.py
--rw-r--r--   0        0        0      105 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/inference/reasoner.py
--rw-r--r--   0        0        0     6960 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/inference/relation_graph_reasoner.py
--rw-r--r--   0        0        0      913 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/__init__.py
--rw-r--r--   0        0        0    28686 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/association_provider_interface.py
--rw-r--r--   0        0        0    55465 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/basic_ontology_interface.py
--rw-r--r--   0        0        0     9243 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/class_enrichment_calculation_interface.py
--rw-r--r--   0        0        0    21219 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/differ_interface.py
--rw-r--r--   0        0        0     3222 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/dumper_interface.py
--rw-r--r--   0        0        0      788 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/embedding_provider_interface.py
--rw-r--r--   0        0        0    13680 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/mapping_provider_interface.py
--rw-r--r--   0        0        0     3262 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/merge_interface.py
--rw-r--r--   0        0        0     3103 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/metadata_interface.py
--rw-r--r--   0        0        0    24049 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/obograph_interface.py
--rw-r--r--   0        0        0     1003 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/obolegacy_interface.py
--rw-r--r--   0        0        0      786 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/ontology_generator_interface.py
--rw-r--r--   0        0        0      784 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/ontology_interface.py
--rw-r--r--   0        0        0    13645 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/owl_interface.py
--rw-r--r--   0        0        0     8606 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/patcher_interface.py
--rw-r--r--   0        0        0     1955 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/rdf_interface.py
--rw-r--r--   0        0        0     2287 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/relation_graph_interface.py
--rw-r--r--   0        0        0     3759 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/search_interface.py
--rw-r--r--   0        0        0    16173 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/semsim_interface.py
--rw-r--r--   0        0        0     1063 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/skos_interface.py
--rw-r--r--   0        0        0     2113 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/subsetter_interface.py
--rw-r--r--   0        0        0    10140 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/summary_statistics_interface.py
--rw-r--r--   0        0        0    18295 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/taxon_constraint_interface.py
--rw-r--r--   0        0        0    10076 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/text_annotator_interface.py
--rw-r--r--   0        0        0    12915 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/interfaces/validator_interface.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/__init__.py
--rw-r--r--   0        0        0     2091 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/heatmap_writer.py
--rw-r--r--   0        0        0     1698 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/html_writer.py
--rw-r--r--   0        0        0     1565 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/obograph_writer.py
--rw-r--r--   0        0        0     3444 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/rollup_report_writer.py
--rw-r--r--   0        0        0      739 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/streaming_axiom_writer.py
--rw-r--r--   0        0        0     9012 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/streaming_csv_writer.py
--rw-r--r--   0        0        0     1284 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/streaming_fhir_writer.py
--rw-r--r--   0        0        0     2524 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/streaming_info_writer.py
--rw-r--r--   0        0        0      785 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/streaming_json_lines_writer.py
--rw-r--r--   0        0        0     1806 2024-05-09 23:39:20.168136 oaklib-0.6.6/src/oaklib/io/streaming_json_writer.py
--rw-r--r--   0        0        0      741 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_kgcl_writer.py
--rw-r--r--   0        0        0     2672 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_markdown_writer.py
--rw-r--r--   0        0        0     1152 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_nl_writer.py
--rw-r--r--   0        0        0     1117 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_obo_json_writer.py
--rw-r--r--   0        0        0     3485 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_obo_writer.py
--rw-r--r--   0        0        0     1270 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_owl_functional_writer.py
--rw-r--r--   0        0        0     2244 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_rdf_writer.py
--rw-r--r--   0        0        0     5101 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_writer.py
--rw-r--r--   0        0        0     1318 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/io/streaming_yaml_writer.py
--rw-r--r--   0        0        0      113 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/mappers/__init__.py
--rw-r--r--   0        0        0     3956 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/mappers/base_mapper.py
--rw-r--r--   0        0        0     1979 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/mappers/ontology_metadata_mapper.py
--rw-r--r--   0        0        0     2363 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/__init__.py
--rw-r--r--   0        0        0     1525 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/association_parser.py
--rw-r--r--   0        0        0      522 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/association_parser_factory.py
--rw-r--r--   0        0        0     4732 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/boomer_parser.py
--rw-r--r--   0        0        0     2148 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/gaf_association_parser.py
--rw-r--r--   0        0        0     2101 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/gencc_association_parser.py
--rw-r--r--   0        0        0     1131 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/hpoa_association_parser.py
--rw-r--r--   0        0        0     1673 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/hpoa_g2d_association_parser.py
--rw-r--r--   0        0        0      603 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/hpoa_g2p_association_parser.py
--rw-r--r--   0        0        0      654 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/kgx_association_parser.py
--rw-r--r--   0        0        0     1672 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/mim2gene_association_parser.py
--rw-r--r--   0        0        0      526 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/pairwise_association_parser.py
--rw-r--r--   0        0        0     1433 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/parser_base.py
--rw-r--r--   0        0        0      708 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/phaf_association_parser.py
--rw-r--r--   0        0        0     8681 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/parsers/xaf_association_parser.py
--rw-r--r--   0        0        0     2210 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/resource.py
--rw-r--r--   0        0        0    15958 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/selector.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/__init__.py
--rw-r--r--   0        0        0      589 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/chained_ontology_transformer.py
--rw-r--r--   0        0        0     2757 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/edge_filter_transformer.py
--rw-r--r--   0        0        0     1257 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/graph_transformer.py
--rw-r--r--   0        0        0     1804 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/node_filter_transformer.py
--rw-r--r--   0        0        0      470 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/ontology_transformer.py
--rw-r--r--   0        0        0     6353 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/sep_transformer.py
--rw-r--r--   0        0        0     1768 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/transformers/transformers_factory.py
--rw-r--r--   0        0        0      177 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/types.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/__init__.py
--rw-r--r--   0        0        0     1613 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/apikey_manager.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/associations/__init__.py
--rw-r--r--   0        0        0    13441 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/associations/association_differ.py
--rw-r--r--   0        0        0     3427 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/associations/association_index.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/axioms/__init__.py
--rw-r--r--   0        0        0     7694 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py
--rw-r--r--   0        0        0     4093 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/axioms/logical_definition_analyzer.py
--rw-r--r--   0        0        0     8829 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/axioms/logical_definition_summarizer.py
--rw-r--r--   0        0        0     2436 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/axioms/logical_definition_utilities.py
--rw-r--r--   0        0        0     1540 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/basic_utils.py
--rw-r--r--   0        0        0     1356 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/format_utilities.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/graph/__init__.py
--rw-r--r--   0        0        0     2491 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/graph/networkx_bridge.py
--rw-r--r--   0        0        0     2857 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/graph/relationship_walker.py
--rw-r--r--   0        0        0      993 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/identifier_utils.py
--rw-r--r--   0        0        0      999 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/iterator_utils.py
--rw-r--r--   0        0        0     1015 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/keyval_cache.py
--rw-r--r--   0        0        0     3425 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/kgcl_utilities.py
--rw-r--r--   0        0        0      850 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/label_utilities.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/lexical/__init__.py
--rw-r--r--   0        0        0    19249 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/lexical/lexical_indexer.py
--rw-r--r--   0        0        0    10235 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/lexical/patternizer.py
--rw-r--r--   0        0        0     6881 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/lexical/synonymizer.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/mapping/__init__.py
--rw-r--r--   0        0        0    14422 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/mapping/boomer_utils.py
--rw-r--r--   0        0        0    15527 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/mapping/cross_ontology_diffs.py
--rw-r--r--   0        0        0      751 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/mapping/mapping_propagator.py
--rw-r--r--   0        0        0    10929 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/mapping/mapping_validation.py
--rw-r--r--   0        0        0     2558 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/mapping/sssom_utils.py
--rw-r--r--   0        0        0      690 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/ner_utilities.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/nlp/__init__.py
--rw-r--r--   0        0        0     3358 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/nlp/natual_language_generation.py
--rw-r--r--   0        0        0      136 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/oboformat_utils.py
--rw-r--r--   0        0        0    30409 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/obograph_utils.py
--rw-r--r--   0        0        0     2275 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/ontology_builder.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/publication_utils/__init__.py
--rw-r--r--   0        0        0     5283 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/publication_utils/doi_wrapper.py
--rw-r--r--   0        0        0      960 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/publication_utils/pubdb_wrapper.py
--rw-r--r--   0        0        0     6575 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/publication_utils/pubmed_wrapper.py
--rw-r--r--   0        0        0      380 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/rate_limiter.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/reasoning/__init__.py
--rw-r--r--   0        0        0      569 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/reasoning/relation_graph.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/semsim/__init__.py
--rw-r--r--   0        0        0     2545 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/semsim/similarity_utils.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.172136 oaklib-0.6.6/src/oaklib/utilities/stats/__init__.py
--rw-r--r--   0        0        0     1511 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/stats/hypergeometric.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/subsets/__init__.py
--rw-r--r--   0        0        0     2819 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/subsets/slimmer_utils.py
--rw-r--r--   0        0        0     4701 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/subsets/subset_analysis.py
--rw-r--r--   0        0        0    12015 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/subsets/value_set_expander.py
--rw-r--r--   0        0        0    18045 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/table_filler.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/taxon/__init__.py
--rw-r--r--   0        0        0     1743 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/taxon/taxon_constraint_utils.py
--rw-r--r--   0        0        0        0 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/validation/__init__.py
--rw-r--r--   0        0        0    11118 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/validation/definition_ontology_rule.py
--rw-r--r--   0        0        0     7492 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/validation/disjointness_rule.py
--rw-r--r--   0        0        0     1729 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/validation/lint_utils.py
--rw-r--r--   0        0        0     1402 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/validation/ontology_rule.py
--rw-r--r--   0        0        0     1275 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/validation/rule_runner.py
--rw-r--r--   0        0        0      122 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/writers/__init__.py
--rw-r--r--   0        0        0    15885 2024-05-09 23:39:20.176136 oaklib-0.6.6/src/oaklib/utilities/writers/change_handler.py
--rw-r--r--   0        0        0     9214 1970-01-01 00:00:00.000000 oaklib-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-06-01 00:03:35.016946 oaklib-0.6.7/LICENSE
+-rw-r--r--   0        0        0     7258 2024-06-01 00:03:35.016946 oaklib-0.6.7/README.md
+-rw-r--r--   0        0        0     3618 2024-06-01 00:04:08.517318 oaklib-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0      334 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/__init__.py
+-rw-r--r--   0        0        0   219900 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/cli.py
+-rw-r--r--   0        0        0       64 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/conf/__init__.py
+-rw-r--r--   0        0        0      372 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/conf/go-human-input-spec.yaml
+-rw-r--r--   0        0        0      162 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/conf/go-pombase-input-spec.yaml
+-rw-r--r--   0        0        0      109 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/conf/hpoa-g2p-input-spec.yaml
+-rw-r--r--   0        0        0      106 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/conf/hpoa-input-spec.yaml
+-rw-r--r--   0        0        0     1903 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
+-rw-r--r--   0        0        0     1011 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/conf/mondo-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      109 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/conf/mondo-gencc-input-spec.yaml
+-rw-r--r--   0        0        0      529 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      118 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
+-rw-r--r--   0        0        0     4904 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/conf/obograph-style.json
+-rw-r--r--   0        0        0      256 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/conf/omo-to-skos.sssom.tsv
+-rw-r--r--   0        0        0      131 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/conf/value-set-expander.conf.yaml
+-rw-r--r--   0        0        0      149 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/constants.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/converters/__init__.py
+-rw-r--r--   0        0        0     1461 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/converters/data_model_converter.py
+-rw-r--r--   0        0        0     2547 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/converters/logical_definition_flattener.py
+-rw-r--r--   0        0        0     2446 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/converters/obo_graph_to_cx_converter.py
+-rw-r--r--   0        0        0    12105 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/converters/obo_graph_to_fhir_converter.py
+-rw-r--r--   0        0        0     7719 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/converters/obo_graph_to_obo_format_converter.py
+-rw-r--r--   0        0        0     6100 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
+-rw-r--r--   0        0        0       60 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/__init__.py
+-rw-r--r--   0        0        0     4034 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/association.owl.ttl
+-rw-r--r--   0        0        0    38339 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/association.py
+-rw-r--r--   0        0        0    13058 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/association.yaml
+-rw-r--r--   0        0        0     6165 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/class_enrichment.owl.ttl
+-rw-r--r--   0        0        0    13288 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/class_enrichment.py
+-rw-r--r--   0        0        0     3262 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/class_enrichment.yaml
+-rw-r--r--   0        0        0    19083 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
+-rw-r--r--   0        0        0    24250 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/cross_ontology_diff.py
+-rw-r--r--   0        0        0    10687 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/cross_ontology_diff.yaml
+-rw-r--r--   0        0        0    29418 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/cx.py
+-rw-r--r--   0        0        0     6314 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/cx.yaml
+-rw-r--r--   0        0        0    15826 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/fhir.owl.ttl
+-rw-r--r--   0        0        0    35746 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/fhir.py
+-rw-r--r--   0        0        0     5064 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/fhir.yaml
+-rw-r--r--   0        0        0    14566 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/input_specification.py
+-rw-r--r--   0        0        0     3560 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/input_specification.yaml
+-rw-r--r--   0        0        0    15776 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/item_list.py
+-rw-r--r--   0        0        0     6339 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/item_list.yaml
+-rw-r--r--   0        0        0     8984 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/lexical_index.owl.ttl
+-rw-r--r--   0        0        0    17296 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/lexical_index.py
+-rw-r--r--   0        0        0     6429 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/lexical_index.schema.json
+-rw-r--r--   0        0        0     4016 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/lexical_index.yaml
+-rw-r--r--   0        0        0    26474 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/mapping_cluster_datamodel.py
+-rw-r--r--   0        0        0     7317 2024-06-01 00:03:35.196948 oaklib-0.6.7/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
+-rw-r--r--   0        0        0   226115 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
+-rw-r--r--   0        0        0    33955 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/mapping_rules_datamodel.py
+-rw-r--r--   0        0        0    12889 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
+-rw-r--r--   0        0        0     4155 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/mapping_rules_datamodel.yaml
+-rw-r--r--   0        0        0    25354 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/obograph.owl.ttl
+-rw-r--r--   0        0        0    51109 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/obograph.py
+-rw-r--r--   0        0        0    22375 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/obograph.schema.json
+-rw-r--r--   0        0        0    19600 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/obograph.yaml
+-rw-r--r--   0        0        0    59793 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/ontology_metadata.owl.ttl
+-rw-r--r--   0        0        0   116914 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/ontology_metadata.py
+-rw-r--r--   0        0        0    95288 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/ontology_metadata.schema.json
+-rw-r--r--   0        0        0    31452 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/ontology_metadata.yaml
+-rw-r--r--   0        0        0    14759 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/oxo.owl.ttl
+-rw-r--r--   0        0        0    21914 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/oxo.py
+-rw-r--r--   0        0        0     4392 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/oxo.yaml
+-rw-r--r--   0        0        0     3348 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/search.py
+-rw-r--r--   0        0        0    16948 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/search_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25157 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/search_datamodel.py
+-rw-r--r--   0        0        0     6684 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/search_datamodel.yaml
+-rw-r--r--   0        0        0      287 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/settings.py
+-rw-r--r--   0        0        0    12826 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/similarity.owl.ttl
+-rw-r--r--   0        0        0    22645 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/similarity.py
+-rw-r--r--   0        0        0     5690 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/similarity.yaml
+-rw-r--r--   0        0        0    31217 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
+-rw-r--r--   0        0        0    50743 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/summary_statistics_datamodel.py
+-rw-r--r--   0        0        0    21176 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
+-rw-r--r--   0        0        0    16246 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/summary_statistics_datamodel.yaml
+-rw-r--r--   0        0        0    23481 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/synonymizer_datamodel.py
+-rw-r--r--   0        0        0     2476 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/synonymizer_datamodel.yaml
+-rw-r--r--   0        0        0     9909 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/taxon_constraints.owl.ttl
+-rw-r--r--   0        0        0    18432 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/taxon_constraints.py
+-rw-r--r--   0        0        0     5880 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/taxon_constraints.yaml
+-rw-r--r--   0        0        0    11599 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/text_annotator.owl.ttl
+-rw-r--r--   0        0        0    21645 2024-06-01 00:03:35.200948 oaklib-0.6.7/src/oaklib/datamodels/text_annotator.py
+-rw-r--r--   0        0        0     2464 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/datamodels/text_annotator.schema.json
+-rw-r--r--   0        0        0     4996 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/datamodels/text_annotator.yaml
+-rw-r--r--   0        0        0    13670 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/datamodels/validation_datamodel.owl.ttl
+-rw-r--r--   0        0        0    33912 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/datamodels/validation_datamodel.py
+-rw-r--r--   0        0        0    10783 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/datamodels/validation_datamodel.schema.json
+-rw-r--r--   0        0        0     9005 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/datamodels/validation_datamodel.yaml
+-rw-r--r--   0        0        0     6640 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/datamodels/value_set_configuration.owl.ttl
+-rw-r--r--   0        0        0     8458 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/datamodels/value_set_configuration.py
+-rw-r--r--   0        0        0     2276 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/datamodels/value_set_configuration.yaml
+-rw-r--r--   0        0        0     6549 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/datamodels/vocabulary.py
+-rw-r--r--   0        0        0     6452 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/aggregator/__init__.py
+-rw-r--r--   0        0        0     6377 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/aggregator/aggregator_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/agrkb/__init__.py
+-rw-r--r--   0        0        0     8848 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/agrkb/agrkb_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/amigo/__init__.py
+-rw-r--r--   0        0        0    16195 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/amigo/amigo_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/cx/__init__.py
+-rw-r--r--   0        0        0     1985 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/cx/cx_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/eutils/__init__.py
+-rw-r--r--   0        0        0     2180 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/eutils/eutils_implementation.py
+-rw-r--r--   0        0        0     1055 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/eutils/pubmed_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/fhir/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/funowl/__init__.py
+-rw-r--r--   0        0        0     8473 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/funowl/funowl_implementation.py
+-rw-r--r--   0        0        0     3565 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/gilda.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/kgx/__init__.py
+-rw-r--r--   0        0        0    30523 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/kgx/kgx_implementation.py
+-rw-r--r--   0        0        0    28777 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/llm_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/monarch/__init__.py
+-rw-r--r--   0        0        0     7034 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/monarch/monarch_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/ncbi/__init__.py
+-rw-r--r--   0        0        0     7034 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/neo4j/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/obograph/__init__.py
+-rw-r--r--   0        0        0    17122 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/obograph/obograph_implementation.py
+-rw-r--r--   0        0        0      267 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/ols/__init__.py
+-rw-r--r--   0        0        0      132 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/ols/constants.py
+-rw-r--r--   0        0        0     8071 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/ols/ols_implementation.py
+-rw-r--r--   0        0        0      686 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/ols/oxo_utils.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/ontobee/__init__.py
+-rw-r--r--   0        0        0     2641 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/ontobee/ontobee_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/ontoportal/__init__.py
+-rw-r--r--   0        0        0      382 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/ontoportal/agroportal_implementation.py
+-rw-r--r--   0        0        0     1250 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/ontoportal/bioportal_implementation.py
+-rw-r--r--   0        0        0      378 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
+-rw-r--r--   0        0        0      378 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/ontoportal/matportal_implementation.py
+-rw-r--r--   0        0        0    13670 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/owlery/__init__.py
+-rw-r--r--   0        0        0      427 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/owlery/owlery_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/pantherdb/__init__.py
+-rw-r--r--   0        0        0    12625 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/pantherdb/pantherdb_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/pronto/__init__.py
+-rw-r--r--   0        0        0    37863 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/pronto/pronto_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/robot/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/scigraph/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/semsimian/__init__.py
+-rw-r--r--   0        0        0      247 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/semsimian/profiler.py
+-rw-r--r--   0        0        0    12242 2024-06-01 00:03:35.204948 oaklib-0.6.7/src/oaklib/implementations/semsimian/semsimian_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/simpleobo/__init__.py
+-rw-r--r--   0        0        0    46328 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
+-rw-r--r--   0        0        0    23081 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/simpleobo/simple_obo_parser.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/skos/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/solor/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/solr/__init__.py
+-rw-r--r--   0        0        0       96 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/sparql/__init__.py
+-rw-r--r--   0        0        0    38067 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
+-rw-r--r--   0        0        0      885 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/sparql/lov_implementation.py
+-rw-r--r--   0        0        0     1721 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
+-rw-r--r--   0        0        0     2658 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/sparql/sparql_implementation.py
+-rw-r--r--   0        0        0     2325 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/sparql/sparql_query.py
+-rw-r--r--   0        0        0       96 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/sqldb/__init__.py
+-rw-r--r--   0        0        0   115796 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/sqldb/sql_implementation.py
+-rw-r--r--   0        0        0     1903 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/sqldb/sqlite_utils.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/tabular/__init__.py
+-rw-r--r--   0        0        0    19432 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/tabular/robot_template_implementation.py
+-rw-r--r--   0        0        0     3279 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/tabular/tabular_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/tccm/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/translator/__init__.py
+-rw-r--r--   0        0        0     5442 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/translator/translator_implementation.py
+-rw-r--r--   0        0        0      108 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/ubergraph/__init__.py
+-rw-r--r--   0        0        0    20090 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/umls/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/uniprot/__init__.py
+-rw-r--r--   0        0        0    14740 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/uniprot/uniprot_implementation.py
+-rw-r--r--   0        0        0       96 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/wikidata/__init__.py
+-rw-r--r--   0        0        0    17267 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/implementations/wikidata/wikidata_implementation.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/indexes/__init__.py
+-rw-r--r--   0        0        0     3089 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/indexes/edge_index.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/inference/__init__.py
+-rw-r--r--   0        0        0      748 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/inference/owl_reasoner.py
+-rw-r--r--   0        0        0      105 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/inference/reasoner.py
+-rw-r--r--   0        0        0     6960 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/inference/relation_graph_reasoner.py
+-rw-r--r--   0        0        0      913 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/__init__.py
+-rw-r--r--   0        0        0    28726 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/association_provider_interface.py
+-rw-r--r--   0        0        0    55465 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/basic_ontology_interface.py
+-rw-r--r--   0        0        0     9302 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/class_enrichment_calculation_interface.py
+-rw-r--r--   0        0        0    21219 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/differ_interface.py
+-rw-r--r--   0        0        0     3222 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/dumper_interface.py
+-rw-r--r--   0        0        0      788 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/embedding_provider_interface.py
+-rw-r--r--   0        0        0    13680 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/mapping_provider_interface.py
+-rw-r--r--   0        0        0     3262 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/merge_interface.py
+-rw-r--r--   0        0        0     3103 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/metadata_interface.py
+-rw-r--r--   0        0        0    24049 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/obograph_interface.py
+-rw-r--r--   0        0        0     1003 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/obolegacy_interface.py
+-rw-r--r--   0        0        0      786 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/ontology_generator_interface.py
+-rw-r--r--   0        0        0      784 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/ontology_interface.py
+-rw-r--r--   0        0        0    13645 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/owl_interface.py
+-rw-r--r--   0        0        0     8606 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/patcher_interface.py
+-rw-r--r--   0        0        0     1955 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/rdf_interface.py
+-rw-r--r--   0        0        0     2287 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/relation_graph_interface.py
+-rw-r--r--   0        0        0     3759 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/search_interface.py
+-rw-r--r--   0        0        0    16678 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/semsim_interface.py
+-rw-r--r--   0        0        0     1063 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/skos_interface.py
+-rw-r--r--   0        0        0     2113 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/subsetter_interface.py
+-rw-r--r--   0        0        0    10140 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/summary_statistics_interface.py
+-rw-r--r--   0        0        0    18295 2024-06-01 00:03:35.208948 oaklib-0.6.7/src/oaklib/interfaces/taxon_constraint_interface.py
+-rw-r--r--   0        0        0    10076 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/interfaces/text_annotator_interface.py
+-rw-r--r--   0        0        0    13080 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/interfaces/validator_interface.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/__init__.py
+-rw-r--r--   0        0        0     2091 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/heatmap_writer.py
+-rw-r--r--   0        0        0     1698 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/html_writer.py
+-rw-r--r--   0        0        0     1565 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/obograph_writer.py
+-rw-r--r--   0        0        0     3444 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/rollup_report_writer.py
+-rw-r--r--   0        0        0      739 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/streaming_axiom_writer.py
+-rw-r--r--   0        0        0     9012 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/streaming_csv_writer.py
+-rw-r--r--   0        0        0     1284 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/streaming_fhir_writer.py
+-rw-r--r--   0        0        0     2524 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/streaming_info_writer.py
+-rw-r--r--   0        0        0      785 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/streaming_json_lines_writer.py
+-rw-r--r--   0        0        0     1806 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/streaming_json_writer.py
+-rw-r--r--   0        0        0      741 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/streaming_kgcl_writer.py
+-rw-r--r--   0        0        0     2672 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/streaming_markdown_writer.py
+-rw-r--r--   0        0        0     1152 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/streaming_nl_writer.py
+-rw-r--r--   0        0        0     1117 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/streaming_obo_json_writer.py
+-rw-r--r--   0        0        0     3485 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/streaming_obo_writer.py
+-rw-r--r--   0        0        0     1270 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/streaming_owl_functional_writer.py
+-rw-r--r--   0        0        0     2244 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/streaming_rdf_writer.py
+-rw-r--r--   0        0        0     5101 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/streaming_writer.py
+-rw-r--r--   0        0        0     1318 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/io/streaming_yaml_writer.py
+-rw-r--r--   0        0        0      113 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/mappers/__init__.py
+-rw-r--r--   0        0        0     3956 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/mappers/base_mapper.py
+-rw-r--r--   0        0        0     1979 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/mappers/ontology_metadata_mapper.py
+-rw-r--r--   0        0        0     2363 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/parsers/__init__.py
+-rw-r--r--   0        0        0     1525 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/parsers/association_parser.py
+-rw-r--r--   0        0        0      522 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/parsers/association_parser_factory.py
+-rw-r--r--   0        0        0     4732 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/parsers/boomer_parser.py
+-rw-r--r--   0        0        0     2148 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/parsers/gaf_association_parser.py
+-rw-r--r--   0        0        0     2101 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/parsers/gencc_association_parser.py
+-rw-r--r--   0        0        0     1131 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/parsers/hpoa_association_parser.py
+-rw-r--r--   0        0        0     1673 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/parsers/hpoa_g2d_association_parser.py
+-rw-r--r--   0        0        0      603 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/parsers/hpoa_g2p_association_parser.py
+-rw-r--r--   0        0        0      654 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/parsers/kgx_association_parser.py
+-rw-r--r--   0        0        0     1672 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/parsers/mim2gene_association_parser.py
+-rw-r--r--   0        0        0      526 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/parsers/pairwise_association_parser.py
+-rw-r--r--   0        0        0     1433 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/parsers/parser_base.py
+-rw-r--r--   0        0        0      708 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/parsers/phaf_association_parser.py
+-rw-r--r--   0        0        0     8681 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/parsers/xaf_association_parser.py
+-rw-r--r--   0        0        0    27210 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/query.py
+-rw-r--r--   0        0        0     2210 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/resource.py
+-rw-r--r--   0        0        0    15958 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/selector.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/transformers/__init__.py
+-rw-r--r--   0        0        0      589 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/transformers/chained_ontology_transformer.py
+-rw-r--r--   0        0        0     2757 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/transformers/edge_filter_transformer.py
+-rw-r--r--   0        0        0     1257 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/transformers/graph_transformer.py
+-rw-r--r--   0        0        0     1804 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/transformers/node_filter_transformer.py
+-rw-r--r--   0        0        0      470 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/transformers/ontology_transformer.py
+-rw-r--r--   0        0        0     6353 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/transformers/sep_transformer.py
+-rw-r--r--   0        0        0     1768 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/transformers/transformers_factory.py
+-rw-r--r--   0        0        0      177 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/types.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/__init__.py
+-rw-r--r--   0        0        0     1613 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/apikey_manager.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/associations/__init__.py
+-rw-r--r--   0        0        0    13441 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/associations/association_differ.py
+-rw-r--r--   0        0        0     3427 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/associations/association_index.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/axioms/__init__.py
+-rw-r--r--   0        0        0     7694 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py
+-rw-r--r--   0        0        0     4093 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/axioms/logical_definition_analyzer.py
+-rw-r--r--   0        0        0     8829 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/axioms/logical_definition_summarizer.py
+-rw-r--r--   0        0        0     3325 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/axioms/logical_definition_utilities.py
+-rw-r--r--   0        0        0     1540 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/basic_utils.py
+-rw-r--r--   0        0        0     1356 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/format_utilities.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/graph/__init__.py
+-rw-r--r--   0        0        0     2491 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/graph/networkx_bridge.py
+-rw-r--r--   0        0        0     2857 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/graph/relationship_walker.py
+-rw-r--r--   0        0        0      993 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/identifier_utils.py
+-rw-r--r--   0        0        0      999 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/iterator_utils.py
+-rw-r--r--   0        0        0     1015 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/keyval_cache.py
+-rw-r--r--   0        0        0     3425 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/kgcl_utilities.py
+-rw-r--r--   0        0        0      850 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/label_utilities.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/lexical/__init__.py
+-rw-r--r--   0        0        0    20732 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/lexical/lexical_indexer.py
+-rw-r--r--   0        0        0    10235 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/lexical/patternizer.py
+-rw-r--r--   0        0        0     6881 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/lexical/synonymizer.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/mapping/__init__.py
+-rw-r--r--   0        0        0    14422 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/mapping/boomer_utils.py
+-rw-r--r--   0        0        0    15527 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/mapping/cross_ontology_diffs.py
+-rw-r--r--   0        0        0      751 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/mapping/mapping_propagator.py
+-rw-r--r--   0        0        0    10929 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/mapping/mapping_validation.py
+-rw-r--r--   0        0        0     2558 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/mapping/sssom_utils.py
+-rw-r--r--   0        0        0      690 2024-06-01 00:03:35.212948 oaklib-0.6.7/src/oaklib/utilities/ner_utilities.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/nlp/__init__.py
+-rw-r--r--   0        0        0     3358 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/nlp/natual_language_generation.py
+-rw-r--r--   0        0        0      136 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/oboformat_utils.py
+-rw-r--r--   0        0        0    30409 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/obograph_utils.py
+-rw-r--r--   0        0        0     2275 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/ontology_builder.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/publication_utils/__init__.py
+-rw-r--r--   0        0        0     5283 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/publication_utils/doi_wrapper.py
+-rw-r--r--   0        0        0      960 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/publication_utils/pubdb_wrapper.py
+-rw-r--r--   0        0        0     6575 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/publication_utils/pubmed_wrapper.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/queries/__init__.py
+-rw-r--r--   0        0        0     3717 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/queries/dissector.py
+-rw-r--r--   0        0        0      380 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/rate_limiter.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/reasoning/__init__.py
+-rw-r--r--   0        0        0      569 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/reasoning/relation_graph.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/semsim/__init__.py
+-rw-r--r--   0        0        0     2545 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/semsim/similarity_utils.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/stats/__init__.py
+-rw-r--r--   0        0        0     1511 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/stats/hypergeometric.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/subsets/__init__.py
+-rw-r--r--   0        0        0     2819 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/subsets/slimmer_utils.py
+-rw-r--r--   0        0        0     4701 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/subsets/subset_analysis.py
+-rw-r--r--   0        0        0    12015 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/subsets/value_set_expander.py
+-rw-r--r--   0        0        0    18045 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/table_filler.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/taxon/__init__.py
+-rw-r--r--   0        0        0     1743 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/taxon/taxon_constraint_utils.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/validation/__init__.py
+-rw-r--r--   0        0        0    11118 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/validation/definition_ontology_rule.py
+-rw-r--r--   0        0        0     7492 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/validation/disjointness_rule.py
+-rw-r--r--   0        0        0     1729 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/validation/lint_utils.py
+-rw-r--r--   0        0        0     1402 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/validation/ontology_rule.py
+-rw-r--r--   0        0        0     1275 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/validation/rule_runner.py
+-rw-r--r--   0        0        0      122 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/writers/__init__.py
+-rw-r--r--   0        0        0    15885 2024-06-01 00:03:35.216948 oaklib-0.6.7/src/oaklib/utilities/writers/change_handler.py
+-rw-r--r--   0        0        0     9214 1970-01-01 00:00:00.000000 oaklib-0.6.7/PKG-INFO
```

### Comparing `oaklib-0.6.6/LICENSE` & `oaklib-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/README.md` & `oaklib-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/pyproject.toml` & `oaklib-0.6.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oaklib"
-version = "v0.6.6"
+version = "v0.6.7"
 description = "Ontology Access Kit: Python library for common ontology operations over a variety of backends"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
@@ -89,15 +89,15 @@
 multi_line_output = 3
 include_trailing_comma = true
 reverse_relative = true
 
 [tool.codespell]
 skip = '.git,*.pdf,*.svg,poetry.lock,*.obo,*.ttl,*.ofn,*.gaf,*.tsv,*.json,input'
 ignore-regex = '(^\s*"image/\S+": ".*|[a-z]*\.\.\.)'
-ignore-words-list = 'ptd,ot,nd,ser,oger,gard,te,fo,fof,bu,ue,ois,processus,infarction,infarctions'
+ignore-words-list = 'ptd,ot,nd,ser,oger,gard,te,fo,fof,bu,ue,ois,processus,infarction,infarctions,assertIn,morpholgy'
 
 [tool.ruff]
 lint.extend-ignore = [
     "D211",  # `no-blank-line-before-class`
     "D212",  # `multi-line-summary-first-line`
     "E731",  # Do not assign a `lambda` expression, use a `def`
     "B005",  # Using `.strip()` with multi-character strings is misleading the reader
```

### Comparing `oaklib-0.6.6/src/oaklib/cli.py` & `oaklib-0.6.7/src/oaklib/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,40 +3,31 @@
 ----------------------
 
 Executed using "runoak" command
 """
 
 # TODO: order commands.
 # See https://stackoverflow.com/questions/47972638/how-can-i-define-the-order-of-click-sub-commands-in-help
-import itertools
 import json
 import logging
 import os
-import re
-import secrets
 import statistics as stats
 import sys
 from collections import defaultdict
 from enum import Enum, unique
 from itertools import chain
 from pathlib import Path
 from time import time
 from types import ModuleType
 from typing import (
-    IO,
     Any,
-    Dict,
-    Iterable,
-    Iterator,
     List,
     Optional,
     TextIO,
-    Tuple,
     Type,
-    Union,
 )
 
 import click
 import kgcl_schema.grammar.parser as kgcl_parser
 import pystow
 import sssom.writers as sssom_writers
 import sssom_schema
@@ -60,41 +51,36 @@
     Edge,
     Graph,
     GraphDocument,
     LogicalDefinitionAxiom,
     Meta,
     PrefixDeclaration,
 )
-from oaklib.datamodels.search import create_search_configuration
 from oaklib.datamodels.settings import Settings
 from oaklib.datamodels.summary_statistics_datamodel import (
     GroupedStatistics,
     UngroupedStatistics,
 )
 from oaklib.datamodels.text_annotator import TextAnnotationConfiguration
 from oaklib.datamodels.validation_datamodel import ValidationConfiguration
 from oaklib.datamodels.vocabulary import (
-    DEVELOPS_FROM,
-    EQUIVALENT_CLASS,
     HAS_OBO_NAMESPACE,
     IS_A,
     IS_DEFINED_BY,
     OBSOLETION_RELATIONSHIP_PREDICATES,
-    OWL_CLASS,
-    OWL_OBJECT_PROPERTY,
     PART_OF,
     PREFIX_PREDICATE,
-    RDF_TYPE,
 )
 from oaklib.implementations.aggregator.aggregator_implementation import (
     AggregatorImplementation,
 )
 from oaklib.implementations.obograph.obograph_implementation import (
     OboGraphImplementation,
 )
+from oaklib.implementations.semsimian.semsimian_implementation import SemSimianImplementation
 from oaklib.implementations.sqldb.sql_implementation import SqlImplementation
 from oaklib.interfaces import (
     BasicOntologyInterface,
     OntologyInterface,
     SubsetterInterface,
     ValidatorInterface,
 )
@@ -138,21 +124,22 @@
 from oaklib.io.streaming_obo_writer import StreamingOboWriter
 from oaklib.io.streaming_owl_functional_writer import StreamingOwlFunctionalWriter
 from oaklib.io.streaming_rdf_writer import StreamingRdfWriter
 from oaklib.io.streaming_writer import StreamingWriter
 from oaklib.io.streaming_yaml_writer import StreamingYamlWriter
 from oaklib.mappers.ontology_metadata_mapper import OntologyMetadataMapper
 from oaklib.parsers.association_parser_factory import get_association_parser
+from oaklib.query import _process_predicates_arg, curies_from_file, query_terms_iterator
 from oaklib.resource import OntologyResource
 from oaklib.selector import get_adapter, get_resource_from_shorthand
 from oaklib.transformers.transformers_factory import (
     apply_ontology_transformation,
     get_ontology_transformer,
 )
-from oaklib.types import CURIE, PRED_CURIE
+from oaklib.types import CURIE
 from oaklib.utilities import table_filler
 from oaklib.utilities.apikey_manager import set_apikey_value
 from oaklib.utilities.associations.association_differ import AssociationDiffer
 from oaklib.utilities.axioms import (
     logical_definition_analyzer,
     logical_definition_summarizer,
 )
@@ -189,15 +176,14 @@
     graph_to_tree_display,
     shortest_paths,
     trim_graph,
 )
 from oaklib.utilities.publication_utils.pubmed_wrapper import PubmedWrapper
 from oaklib.utilities.semsim.similarity_utils import load_information_content_map
 from oaklib.utilities.subsets.slimmer_utils import (
-    filter_redundant,
     roll_up_to_named_subset,
 )
 from oaklib.utilities.table_filler import ColumnDependency, TableFiller, TableMetadata
 from oaklib.utilities.taxon.taxon_constraint_utils import parse_gain_loss_file
 from oaklib.utilities.validation.lint_utils import lint_ontology
 from oaklib.utilities.validation.rule_runner import RuleRunner
 
@@ -465,62 +451,14 @@
     "--group-by-prefix/--no-group-by-prefix",
     default=False,
     show_default=True,
     help="shortcut for --group-by-property sh:prefix. Groups by the prefix of the CURIE",
 )
 
 
-def _process_predicates_arg(
-    predicates_str: str,
-    expected_number: Optional[int] = None,
-    exclude_predicates_str: Optional[str] = None,
-    impl: Optional[OntologyInterface] = None,
-) -> Optional[List[PRED_CURIE]]:
-    if predicates_str is None and exclude_predicates_str is None:
-        return None
-    if predicates_str is None:
-        inputs = []
-    elif "," in predicates_str:
-        inputs = predicates_str.split(",")
-    else:
-        inputs = predicates_str.split("+")
-    preds = [_shorthand_to_pred_curie(p) for p in inputs]
-    if exclude_predicates_str:
-        if "," in exclude_predicates_str:
-            exclude_inputs = exclude_predicates_str.split(",")
-        else:
-            exclude_inputs = exclude_predicates_str.split("+")
-        exclude_preds = [_shorthand_to_pred_curie(p) for p in exclude_inputs]
-        if not preds:
-            if not impl or not isinstance(impl, BasicOntologyInterface):
-                raise ValueError("Must provide an BasicOntologyInterface to exclude predicates")
-            preds = list(impl.entities(owl_type=OWL_OBJECT_PROPERTY))
-        preds = [p for p in preds if p not in exclude_preds]
-        logging.info(f"Excluding predicates: {exclude_preds} yields: {preds}")
-    if expected_number and len(preds) != expected_number:
-        raise ValueError(f"Expected {expected_number} parses of {predicates_str}, got: {preds}")
-    return preds
-
-
-# TODO: move to vocab
-def _shorthand_to_pred_curie(shorthand: str) -> PRED_CURIE:
-    if shorthand == "i":
-        return IS_A
-    elif shorthand == "p":
-        return PART_OF
-    elif shorthand == "d":
-        return DEVELOPS_FROM
-    elif shorthand == "t":
-        return RDF_TYPE
-    elif shorthand == "e":
-        return EQUIVALENT_CLASS
-    else:
-        return shorthand
-
-
 def _skip_if_absent(if_absent: bool, v: Any):
     if if_absent:
         if if_absent == IfAbsent.absent_only.value and v:
             return True
         elif if_absent == IfAbsent.present_only.value and not v:
             return True
     return False
@@ -552,317 +490,14 @@
         if not isinstance(impl, PatcherInterface):
             raise NotImplementedError(f"Cannot apply {len(changes)} changes")
         for change in changes:
             impl.apply_patch(change)
         impl.save()
 
 
-# A list whose members are either strings (search terms, curies, or directives)
-# or nested lists.
-# TODO: Replace this with an explicit query model with boolean operations
-NESTED_LIST = Union[List[str], List["NESTED_LIST"]]
-
-
-def nest_list_of_terms(terms: List[str]) -> NESTED_LIST:
-    """
-    Gives a list of terms (typically passed on command line),
-    replace blocks between '[', ..., ']' with nested lists of the contents
-
-    :param terms:
-    :return:
-    """
-    nested, rest = _nest_list_of_terms(terms)
-    if rest:
-        raise ValueError(f"Unparsed: {rest}")
-    return nested
-
-
-def _nest_list_of_terms(terms: List[str]) -> Tuple[NESTED_LIST, List[str]]:
-    nested = []
-    while len(terms) > 0:
-        term = terms[0]
-        terms = terms[1:]
-        if term == "[":
-            nxt, rest = _nest_list_of_terms(terms)
-            terms = rest
-            nested.append(nxt)
-        elif term == "]":
-            return nested, terms
-        else:
-            nested.append(term)
-    return nested, []
-
-
-def curies_from_file(
-    file: IO, adapter: Optional[BasicOntologyInterface] = None, allow_labels=False, strict=False
-) -> Iterator[CURIE]:
-    """
-    yield an iterator over CURIEs by parsing a file.
-
-    The file can contain any content, so long as each line
-    starts with a CURIE followed by whitespace -- the remainder of the line
-    is ignored
-
-    :param file:
-    :param adapter: if provided, will be used to resolve CURIEs
-    :param allow_labels: if true, will allow inputs to be labels
-    :param strict: if true, will raise an error if a CURIE cannot be resolved
-    :return:
-    """
-    line_no = 0
-    if allow_labels and not adapter:
-        raise ValueError("Must provide an adapter to resolve labels")
-    for line in file.readlines():
-        line_no += 1
-        if ":" in line or not allow_labels:
-            m = re.match(r"^(\S+)", line)
-            curie = m.group(1)
-            if curie == "id" and line_no == 1:
-                continue
-            yield curie
-        elif allow_labels:
-            candidates = adapter.curies_by_label(line.strip())
-            if strict and len(candidates) != 1:
-                raise ValueError(
-                    f"Could not resolve label {line} to a single CURIE, got {candidates}"
-                )
-            yield from candidates
-
-
-def query_terms_iterator(query_terms: NESTED_LIST, impl: BasicOntologyInterface) -> Iterator[CURIE]:
-    """
-    Turn list of tokens that represent a term query into an iterator for curies.
-
-    For examples, see test_cli
-
-    :param query_terms:
-    :param impl:
-    :return:
-    """
-    # TODO: reimplement using an explicit query model
-    results: Iterable[CURIE] = iter([])
-    predicates = None
-    if isinstance(query_terms, tuple):
-        query_terms = list(query_terms)
-
-    def _parse_params(s: str) -> Dict:
-        # some query terms are parameterized using the syntax
-        # .<TOKEN>//<P1>=<V1>//<P2>=<V2>...
-        d = {}
-        m = re.match(r"\.\w+//(.+)", s)
-        if m:
-            for p in m.group(1).split("//"):
-                if "=" not in p:
-                    raise ValueError(f"All arguments must be of param=val form, got {p} in {s}")
-                [k, v] = p.split("=")
-                if k == "p":
-                    k = "predicates"
-                if k == "predicates":
-                    v = _process_predicates_arg(v)
-                if k == "prefixes":
-                    v = v.split(",")
-                d[k] = v
-        return d
-
-    def chain_results(v):
-        if isinstance(v, str):
-            v = iter([v])
-        nonlocal results
-        results = itertools.chain(results, v)
-
-    # queries can be nested using square brackets
-    query_terms = nest_list_of_terms(query_terms)
-
-    while len(query_terms) > 0:
-        # process each query term. A query term is either:
-        # 1. local, in which case is appends to the result iterator
-        # 2. global, where it applies all subsequent terms
-        term = query_terms[0]
-        query_terms = query_terms[1:]
-        if term == "-":
-            # read from stdin
-            chain_results(curies_from_file(sys.stdin))
-        elif isinstance(term, list):
-            chain_results(query_terms_iterator(term, impl))
-        elif term.startswith(".load="):
-            # load a file of IDs
-            fn = term.replace(".load=", "")
-            with open(fn) as file:
-                chain_results(curies_from_file(file))
-        elif term.startswith(".idfile"):
-            # load a file of IDs
-            fn = query_terms.pop(0)
-            logging.info(f"Reading ids from {fn}")
-            file = open(fn)
-            chain_results(curies_from_file(file))
-        elif term.startswith(".termfile"):
-            # load a file of queries
-            fn = query_terms.pop(0)
-            with open(fn) as file:
-                lines = [line.strip() for line in file.readlines()]
-                query_terms = lines + query_terms
-        elif re.match(r"^([\w\-\.]+):(\S+)$", term):
-            # CURIE
-            chain_results(term)
-        elif re.match(r"^http(\S+)$", term):
-            # URI
-            chain_results(term)
-        elif re.match(r"^\.predicates=(\S*)$", term):
-            logging.warning("Deprecated: pass as parameter instead")
-            m = re.match(r"^\.predicates=(\S*)$", term)
-            predicates = _process_predicates_arg(m.group(1))
-        elif term == ".and":
-            # boolean term: consume the result of the query and intersect
-            rest = list(query_terms_iterator(query_terms, impl))
-            for x in results:
-                if x in rest:
-                    yield x
-            query_terms = []
-        elif term == ".xor":
-            # boolean term: consume the result of the query and xor
-            rest = list(query_terms_iterator(query_terms, impl))
-            remaining = []
-            for x in results:
-                if x not in rest:
-                    yield x
-                else:
-                    remaining.append(x)
-            for x in rest:
-                if x not in remaining:
-                    yield x
-            query_terms = []
-        elif term == ".not" or term == ".minus":
-            # boolean term: consume the result of the query and subtract
-            rest = list(query_terms_iterator(query_terms, impl))
-            for x in results:
-                if x not in rest:
-                    yield x
-            query_terms = []
-        elif term == ".or":
-            # or is implicit
-            pass
-        elif term.startswith(".all"):
-            chain_results(impl.entities(filter_obsoletes=False))
-        elif term.startswith(".classes"):
-            chain_results(impl.entities(owl_type=OWL_CLASS))
-        elif term.startswith(".relations"):
-            chain_results(impl.entities(owl_type=OWL_OBJECT_PROPERTY))
-        elif term.startswith(".rand"):
-            params = _parse_params(term)
-            sample_size = params.get("n", "100")
-            entities = list(impl.entities())
-            sample = [
-                entities[secrets.randbelow(len(entities))] for x in range(1, int(sample_size))
-            ]
-            chain_results(sample)
-        elif term.startswith(".in"):
-            # subset query
-            subset = query_terms[0]
-            query_terms = query_terms[1:]
-            chain_results(impl.subset_members(subset))
-        elif term.startswith(".is_obsolete"):
-            chain_results(impl.obsoletes())
-        elif term.startswith(".non_obsolete"):
-            chain_results(impl.entities(filter_obsoletes=True))
-        elif term.startswith(".dangling"):
-            chain_results(impl.dangling())
-        elif term.startswith(".filter"):
-            # arbitrary python expression
-            expr = query_terms[0]
-            query_terms = query_terms[1:]
-            chain_results(eval(expr, {"impl": impl, "terms": results}))  # noqa
-        elif term.startswith(".query"):
-            # arbitrary SPARQL query
-            params = _parse_params(term)
-            prefixes = params.get("prefixes", None)
-            query = query_terms[0]
-            query_terms = query_terms[1:]
-            chain_results([list(v.values())[0] for v in impl.query(query, prefixes=prefixes)])
-        elif term.startswith(".desc"):
-            # graph query: descendants
-            params = _parse_params(term)
-            this_predicates = params.get("predicates", predicates)
-            rest = list(query_terms_iterator([query_terms[0]], impl))
-            query_terms = query_terms[1:]
-            if isinstance(impl, OboGraphInterface):
-                chain_results(impl.descendants(rest, predicates=this_predicates))
-            else:
-                raise NotImplementedError
-        elif term.startswith(".child"):
-            # graph query: children
-            params = _parse_params(term)
-            this_predicates = params.get("predicates", predicates)
-            rest = list(query_terms_iterator([query_terms[0]], impl))
-            query_terms = query_terms[1:]
-            children = [
-                s for s, _p, _o in impl.relationships(objects=rest, predicates=this_predicates)
-            ]
-            chain_results(children)
-        elif term.startswith(".parent"):
-            # graph query: parents
-            params = _parse_params(term)
-            this_predicates = params.get("predicates", predicates)
-            rest = list(query_terms_iterator([query_terms[0]], impl))
-            query_terms = query_terms[1:]
-            parents = [
-                o for _s, _p, o in impl.relationships(subjects=rest, predicates=this_predicates)
-            ]
-            chain_results(parents)
-        elif term.startswith(".sib"):
-            # graph query: siblings
-            params = _parse_params(term)
-            this_predicates = params.get("predicates", predicates)
-            rest = list(query_terms_iterator([query_terms[0]], impl))
-            query_terms = query_terms[1:]
-            parents = [
-                o for _s, _p, o in impl.relationships(subjects=rest, predicates=this_predicates)
-            ]
-            sibs = [
-                s for s, _p, _o in impl.relationships(objects=parents, predicates=this_predicates)
-            ]
-            chain_results(sibs)
-        elif term.startswith(".anc"):
-            # graph query: ancestors
-            params = _parse_params(term)
-            this_predicates = params.get("predicates", predicates)
-            rest = list(query_terms_iterator([query_terms[0]], impl))
-            query_terms = query_terms[1:]
-            if isinstance(impl, OboGraphInterface):
-                chain_results(impl.ancestors(rest, predicates=this_predicates))
-            else:
-                raise NotImplementedError
-        elif term.startswith(".mrca"):
-            # graph query: most recent common ancestors
-            params = _parse_params(term)
-            this_predicates = params.get("predicates", predicates)
-            rest = list(query_terms_iterator([query_terms[0]], impl))
-            query_terms = query_terms[1:]
-            if isinstance(impl, SemanticSimilarityInterface):
-                chain_results(
-                    impl.setwise_most_recent_common_ancestors(rest, predicates=this_predicates)
-                )
-            else:
-                raise NotImplementedError
-        elif term.startswith(".nr"):
-            # graph query: non-redundant
-            params = _parse_params(term)
-            this_predicates = params.get("predicates", predicates)
-            rest = list(query_terms_iterator([query_terms[0]], impl))
-            query_terms = query_terms[1:]
-            chain_results(filter_redundant(impl, rest, this_predicates))
-        else:
-            # term is not query syntax: feed directly to search
-            if not isinstance(impl, SearchInterface):
-                raise NotImplementedError(f"Search not implemented for {type(impl)}")
-            cfg = create_search_configuration(term)
-            logging.info(f"Search config: {term} => {cfg}")
-            chain_results(impl.basic_search(cfg.search_terms[0], config=cfg))
-    yield from results
-
-
 @click.group()
 @click.option("-v", "--verbose", count=True)
 @click.option("-q", "--quiet/--no-quiet")
 @click.option(
     "--stacktrace/--no-stacktrace",
     default=False,
     show_default=True,
@@ -1211,15 +846,15 @@
 
     Example:
 
         runoak -i obolibrary:go.obo obsoletes --show-migration-relationships GO:0000187 GO:0000188
 
     More examples:
 
-       https://github.com/INCATools/ontology-access-kit/blob/main/notebooks/Commands/TaxonConstraints.ipynb
+       https://github.com/INCATools/ontology-access-kit/blob/main/notebooks/Commands/Obsoletes.ipynb
 
     Python API:
 
        https://incatools.github.io/ontology-access-kit/interfaces/basic
 
     """
     impl = settings.impl
@@ -1871,14 +1506,20 @@
     impl = settings.impl
     if not isinstance(impl, OboGraphInterface):
         raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
     impl.precompute_lookups()
     if stylemap is None:
         stylemap = default_stylemap_path()
     actual_predicates = _process_predicates_arg(predicates)
+    curies_highlight = None
+    if "@" in terms:
+        ix = terms.index("@")
+        terms_highlight = terms[0:ix]
+        terms = terms[ix + 1 :]
+        curies_highlight = list(query_terms_iterator(terms_highlight, impl))
     curies = list(query_terms_iterator(terms, impl))
     if add_mrcas:
         if isinstance(impl, SemanticSimilarityInterface):
             curies_to_add = [
                 lca
                 for s, o, lca in impl.multiset_most_recent_common_ancestors(
                     curies, predicates=actual_predicates
@@ -1906,19 +1547,21 @@
         logging.info(f"Trimming graph, max_hops={max_hops}")
         graph = trim_graph(graph, curies, distance=max_hops, include_intermediates=True)
     logging.info(f"Drawing graph seeded from {curies}")
     if meta:
         impl.add_metadata(graph)
     if not graph.nodes:
         raise ValueError(f"No nodes in graph for {curies}")
+    if curies_highlight is None:
+        curies_highlight = curies
     # TODO: abstract this out
     if not output_type or output_type in ["png", "svg", "dot"]:
         graph_to_image(
             graph,
-            seeds=curies,
+            seeds=curies_highlight,
             stylemap=stylemap,
             configure=configure,
             imgfile=output,
             view=view,
             format=output_type,
         )
     else:
@@ -2944,15 +2587,20 @@
     writer.output = output
     logging.info(f"file={writer.file} {type(writer.output)}")
     if main_score_field and isinstance(writer, HeatmapWriter):
         writer.value_field = main_score_field
     if not isinstance(impl, SemanticSimilarityInterface):
         raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
     if information_content_file:
-        impl.cached_information_content_map = load_information_content_map(information_content_file)
+        if isinstance(impl, SemSimianImplementation):
+            impl.custom_ic_map_path = information_content_file
+        else:
+            impl.cached_information_content_map = load_information_content_map(
+                information_content_file
+            )
     set1it = None
     set2it = None
     if not (set1_file or set2_file):
         terms = list(terms)
         ix = terms.index("@")
         logging.info(f"Splitting terms {terms} on {ix}")
         set1it = query_terms_iterator(terms[0:ix], impl)
@@ -3025,16 +2673,26 @@
 
     """
     impl = settings.impl
     writer = _get_writer(output_type, impl, StreamingYamlWriter, datamodels.similarity)
     writer.output = output
     if not isinstance(impl, SemanticSimilarityInterface):
         raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
+
+    # TODO: @cmungall - one possibility in future is to relieve client of the need for
+    # out of band knowledge about impl details. The generic SemSim interface could have
+    # a load_ic_map method, with the generic impl being to directly load, and the semsimian
+    # impl passing the path through.
     if information_content_file:
-        impl.cached_information_content_map = load_information_content_map(information_content_file)
+        if isinstance(impl, SemSimianImplementation):
+            impl.custom_ic_map_path = information_content_file
+        else:
+            impl.cached_information_content_map = load_information_content_map(
+                information_content_file
+            )
     terms = list(terms)
     ix = terms.index("@")
     set1 = list(query_terms_iterator(terms[0:ix], impl))
     set2 = list(query_terms_iterator(terms[ix + 1 :], impl))
     logging.info(f"Set1={set1}")
     logging.info(f"Set2={set2}")
     actual_predicates = _process_predicates_arg(predicates)
@@ -4077,33 +3735,35 @@
     writer.output = output
     writer.autolabel = autolabel
     if not isinstance(impl, MappingProviderInterface):
         raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
     mapper_impl = impl
     if mapper:
         mapper_impl = get_adapter(mapper)
+
+    def _emit(mapping):
+        if autolabel:
+            impl.inject_mapping_labels([mapping])
+        writer.emit(mapping)
+
     if len(terms) == 0:
         logging.info(f"No terms provided: fetching all mappings for {maps_to_source}")
         for mapping in mapper_impl.sssom_mappings_by_source(
             subject_or_object_source=maps_to_source
         ):
-            if autolabel:
-                impl.inject_mapping_labels([mapping])
-            writer.emit(mapping)
+            _emit(mapping)
     else:
         logging.info(f"Fetching mappings for {terms}")
         for curie_it in chunk(query_terms_iterator(terms, impl)):
             for mapping in list(mapper_impl.sssom_mappings(curie_it)):
                 if maps_to_source and not mapping.object_id.lower().startswith(
                     f"{maps_to_source.lower()}:"
                 ):
                     continue
-                if autolabel:
-                    impl.inject_mapping_labels([mapping])
-                writer.emit(mapping)
+                _emit(mapping)
     writer.finish()
 
 
 @main.command()
 @output_option
 @output_type_option
 @autolabel_option
@@ -5012,15 +4672,15 @@
     default=0.05,
     show_default=True,
     help="The cutoff for the p-value; any p-values greater than this are not reported.",
 )
 @click.option(
     "--sample-file",
     "-U",
-    required=True,
+    required=False,
     type=click.File(mode="r"),
     help="file containing input list of entity IDs (e.g. gene IDs)",
 )
 @click.option(
     "--background-file",
     "-B",
     type=click.File(mode="r"),
@@ -5084,15 +4744,26 @@
     reflexive relations between each term and itself. This can be useful for summarizing term lists,
     but note that P-values may not be meaningful.
 
     """
     impl = settings.impl
     actual_predicates = _process_predicates_arg(predicates)
     actual_association_predicates = _process_predicates_arg(association_predicates)
-    subjects = list(curies_from_file(sample_file, adapter=impl, allow_labels=allow_labels))
+    if sample_file:
+        subjects = list(curies_from_file(sample_file, adapter=impl, allow_labels=allow_labels))
+    else:
+        if "@" in terms:
+            ix = terms.index("@")
+            logging.info(f"Splitting terms into two, position = {ix}")
+            subjects = list(query_terms_iterator(terms[0:ix], impl))
+            terms = terms[ix + 1 :]
+        else:
+            subjects = list(query_terms_iterator(terms, impl))
+    if not subjects:
+        raise ValueError("No terms or upload provided")
     background = (
         list(curies_from_file(background_file, adapter=impl, allow_labels=allow_labels))
         if background_file
         else None
     )
     if not isinstance(impl, ClassEnrichmentCalculationInterface):
         raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
@@ -5764,18 +5435,31 @@
 )
 @click.option(
     "--ensure-strict-prefixes/--no-ensure-strict-prefixes",
     default=False,
     show_default=True,
     help="Clean prefix map and mappings before generating an output.",
 )
+@click.option(
+    "--exclude-mapped/--no-exclude-mapped",
+    default=False,
+    show_default=True,
+    help="Return only mappings for subjects that have not been mapped",
+)
 @output_option
 @click.argument("terms", nargs=-1)
 def lexmatch(
-    output, recreate, ensure_strict_prefixes, rules_file, lexical_index_file, add_labels, terms
+    output,
+    recreate,
+    ensure_strict_prefixes,
+    rules_file,
+    lexical_index_file,
+    add_labels,
+    terms,
+    exclude_mapped,
 ):
     """
     Performs lexical matching between pairs of terms in one more more ontologies.
 
     Examples
     -
         runoak -i foo.obo lexmatch -o foo.sssom.tsv
@@ -5855,14 +5539,15 @@
         ix = load_lexical_index(lexical_index_file)
     else:
         logging.info("Creating index")
         if ruleset:
             syn_rules = [x.synonymizer for x in ruleset.rules if x.synonymizer]
         else:
             syn_rules = []
+        logging.info(f"Synonymizer rules: {syn_rules}")
         ix = create_lexical_index(impl, synonym_rules=syn_rules)
     if lexical_index_file:
         if recreate:
             logging.info("Saving index")
             save_lexical_index(ix, lexical_index_file)
     logging.info(f"Generating mappings from {len(ix.groupings)} groupings")
     # TODO: abstract this way from serialization format
@@ -5871,14 +5556,31 @@
         ix,
         ruleset=ruleset,
         subjects=subjects,
         objects=objects,
         prefix_map=prefix_map,
         ensure_strict_prefixes=ensure_strict_prefixes,
     )
+    # TODO: coordinate with sssom-py to have simpler ways of filtering, no reliance on pandas
+    if exclude_mapped and not msdf.df.empty:
+        if not isinstance(impl, MappingProviderInterface):
+            raise ValueError(f"{type(impl)} does not implement MappingProviderInterface")
+        df = msdf.df
+        subjects = set(df["subject_id"])
+        existing_mappings = list(impl.sssom_mappings(subjects))
+        pairs = [(m.subject_id, m.object_source) for m in existing_mappings]
+        pairs += [(m.object_id, m.subject_source) for m in existing_mappings]
+        # filter df by pairs
+        df = df[
+            df.apply(lambda x: (x["subject_id"], x["object_id"].split(":")[0]) not in pairs, axis=1)
+        ]
+        df = df[
+            df.apply(lambda x: (x["object_id"], x["subject_id"].split(":")[0]) not in pairs, axis=1)
+        ]
+        msdf.df = df
     sssom_writers.write_table(msdf, output)
 
 
 @main.command()
 @click.option("--other-ontology", help="other ontology")
 @output_option
 @click.argument("terms", nargs=-1)
```

### Comparing `oaklib-0.6.6/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml` & `oaklib-0.6.7/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/conf/mondo-g2d-input-spec.yaml` & `oaklib-0.6.7/src/oaklib/conf/mondo-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml` & `oaklib-0.6.7/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/conf/obograph-style.json` & `oaklib-0.6.7/src/oaklib/conf/obograph-style.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996309715512614%*

 * *Differences: {"'prefixProperties'": "{'CHEBI': {'fillcolor': 'mediumturquoise'}}",*

 * * "'relationProperties'": "{'BFO:0000051': OrderedDict([('arrowhead', 'box'), ('color', 'teal'), "*

 * *                         "('penwidth', 2), ('label', 'ⓗ')])}"}*

```diff
@@ -35,15 +35,15 @@
     "fillcolor": "white",
     "includeIdInLabel": "true",
     "prefixProperties": {
         "BFO": {
             "fillcolor": "cyan"
         },
         "CHEBI": {
-            "fillcolor": "cyan"
+            "fillcolor": "mediumturquoise"
         },
         "CL": {
             "fillcolor": "azure2"
         },
         "ENM": {
             "fillcolor": "cornsilk"
         },
@@ -110,14 +110,20 @@
     "relationProperties": {
         "BFO:0000050": {
             "arrowhead": "tee",
             "color": "blue",
             "label": "\u24df",
             "penwidth": 3
         },
+        "BFO:0000051": {
+            "arrowhead": "box",
+            "color": "teal",
+            "label": "\u24d7",
+            "penwidth": 2
+        },
         "RO:0001025": {
             "arrowhead": "diamond",
             "color": "green",
             "label": "L",
             "penwidth": 2
         },
         "RO:0002087": {
```

### Comparing `oaklib-0.6.6/src/oaklib/converters/data_model_converter.py` & `oaklib-0.6.7/src/oaklib/converters/data_model_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/converters/logical_definition_flattener.py` & `oaklib-0.6.7/src/oaklib/converters/logical_definition_flattener.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/converters/obo_graph_to_cx_converter.py` & `oaklib-0.6.7/src/oaklib/converters/obo_graph_to_cx_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/converters/obo_graph_to_fhir_converter.py` & `oaklib-0.6.7/src/oaklib/converters/obo_graph_to_fhir_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/converters/obo_graph_to_obo_format_converter.py` & `oaklib-0.6.7/src/oaklib/converters/obo_graph_to_obo_format_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py` & `oaklib-0.6.7/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/association.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/association.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/association.py` & `oaklib-0.6.7/src/oaklib/datamodels/association.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/association.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/association.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/class_enrichment.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/class_enrichment.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/class_enrichment.py` & `oaklib-0.6.7/src/oaklib/datamodels/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/class_enrichment.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/cross_ontology_diff.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/cross_ontology_diff.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/cross_ontology_diff.py` & `oaklib-0.6.7/src/oaklib/datamodels/cross_ontology_diff.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/cross_ontology_diff.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/cross_ontology_diff.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/cx.py` & `oaklib-0.6.7/src/oaklib/datamodels/cx.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/cx.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/cx.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/fhir.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/fhir.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/fhir.py` & `oaklib-0.6.7/src/oaklib/datamodels/fhir.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/fhir.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/fhir.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/input_specification.py` & `oaklib-0.6.7/src/oaklib/datamodels/input_specification.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/input_specification.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/input_specification.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/item_list.py` & `oaklib-0.6.7/src/oaklib/datamodels/item_list.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/item_list.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/item_list.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/lexical_index.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/lexical_index.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/lexical_index.py` & `oaklib-0.6.7/src/oaklib/datamodels/lexical_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/lexical_index.schema.json` & `oaklib-0.6.7/src/oaklib/datamodels/lexical_index.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/lexical_index.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/lexical_index.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/mapping_cluster_datamodel.py` & `oaklib-0.6.7/src/oaklib/datamodels/mapping_cluster_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/mapping_cluster_datamodel.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/mapping_cluster_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.py` & `oaklib-0.6.7/src/oaklib/datamodels/mapping_rules_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.schema.json` & `oaklib-0.6.7/src/oaklib/datamodels/mapping_rules_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/mapping_rules_datamodel.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/mapping_rules_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/obograph.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/obograph.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/obograph.py` & `oaklib-0.6.7/src/oaklib/datamodels/obograph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/obograph.schema.json` & `oaklib-0.6.7/src/oaklib/datamodels/obograph.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/obograph.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/obograph.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/ontology_metadata.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.py` & `oaklib-0.6.7/src/oaklib/datamodels/ontology_metadata.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.schema.json` & `oaklib-0.6.7/src/oaklib/datamodels/ontology_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/ontology_metadata.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/ontology_metadata.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/oxo.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/oxo.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/oxo.py` & `oaklib-0.6.7/src/oaklib/datamodels/oxo.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/oxo.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/oxo.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/search.py` & `oaklib-0.6.7/src/oaklib/datamodels/search.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/search_datamodel.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/search_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/search_datamodel.py` & `oaklib-0.6.7/src/oaklib/datamodels/search_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/search_datamodel.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/search_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/similarity.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/similarity.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/similarity.py` & `oaklib-0.6.7/src/oaklib/datamodels/similarity.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/similarity.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/similarity.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.py` & `oaklib-0.6.7/src/oaklib/datamodels/summary_statistics_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.schema.json` & `oaklib-0.6.7/src/oaklib/datamodels/summary_statistics_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/summary_statistics_datamodel.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/summary_statistics_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/synonymizer_datamodel.py` & `oaklib-0.6.7/src/oaklib/datamodels/synonymizer_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/synonymizer_datamodel.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/synonymizer_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/taxon_constraints.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/taxon_constraints.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/taxon_constraints.py` & `oaklib-0.6.7/src/oaklib/datamodels/taxon_constraints.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/taxon_constraints.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/taxon_constraints.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/text_annotator.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/text_annotator.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/text_annotator.py` & `oaklib-0.6.7/src/oaklib/datamodels/text_annotator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/text_annotator.schema.json` & `oaklib-0.6.7/src/oaklib/datamodels/text_annotator.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/text_annotator.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/text_annotator.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/validation_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.py` & `oaklib-0.6.7/src/oaklib/datamodels/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.schema.json` & `oaklib-0.6.7/src/oaklib/datamodels/validation_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/validation_datamodel.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/value_set_configuration.owl.ttl` & `oaklib-0.6.7/src/oaklib/datamodels/value_set_configuration.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/value_set_configuration.py` & `oaklib-0.6.7/src/oaklib/datamodels/value_set_configuration.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/value_set_configuration.yaml` & `oaklib-0.6.7/src/oaklib/datamodels/value_set_configuration.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/datamodels/vocabulary.py` & `oaklib-0.6.7/src/oaklib/datamodels/vocabulary.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/__init__.py` & `oaklib-0.6.7/src/oaklib/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/aggregator/aggregator_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/aggregator/aggregator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/agrkb/agrkb_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/agrkb/agrkb_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/amigo/amigo_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/amigo/amigo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/cx/cx_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/cx/cx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/eutils/eutils_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/eutils/eutils_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/eutils/pubmed_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/eutils/pubmed_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/funowl/funowl_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/funowl/funowl_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/gilda.py` & `oaklib-0.6.7/src/oaklib/implementations/gilda.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/kgx/kgx_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/kgx/kgx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/llm_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/llm_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/monarch/monarch_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/monarch/monarch_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/obograph/obograph_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/obograph/obograph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/ols/ols_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/ols/ols_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/ols/oxo_utils.py` & `oaklib-0.6.7/src/oaklib/implementations/ols/oxo_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/ontobee/ontobee_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/ontobee/ontobee_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/ontoportal/bioportal_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/ontoportal/bioportal_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py` & `oaklib-0.6.7/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/pantherdb/pantherdb_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/pantherdb/pantherdb_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/pronto/pronto_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/pronto/pronto_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/semsimian/semsimian_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/semsimian/semsimian_implementation.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,29 +10,32 @@
     BestMatch,
     TermInfo,
     TermPairwiseSimilarity,
     TermSetPairwiseSimilarity,
 )
 from oaklib.datamodels.vocabulary import OWL_THING
 from oaklib.implementations.sqldb.sql_implementation import SqlImplementation
+from oaklib.interfaces.association_provider_interface import AssociationProviderInterface
 from oaklib.interfaces.basic_ontology_interface import BasicOntologyInterface
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.interfaces.search_interface import SearchInterface
 from oaklib.interfaces.semsim_interface import SemanticSimilarityInterface
 from oaklib.types import CURIE, PRED_CURIE
 
 wrapped_adapter: BasicOntologyInterface = None
 
 __all__ = [
     "SemSimianImplementation",
 ]
 
 
 @dataclass
-class SemSimianImplementation(SearchInterface, SemanticSimilarityInterface, OboGraphInterface):
+class SemSimianImplementation(
+    SearchInterface, SemanticSimilarityInterface, OboGraphInterface, AssociationProviderInterface
+):
     """Rust implementation of semantic similarity measures."""
 
     delegated_methods: ClassVar[List[str]] = [
         BasicOntologyInterface.label,
         BasicOntologyInterface.labels,
         BasicOntologyInterface.entities,
         BasicOntologyInterface.curie_to_uri,
@@ -43,16 +46,20 @@
         BasicOntologyInterface.definitions,
         SearchInterface.basic_search,
         OboGraphInterface.node,
         OboGraphInterface.ancestors,
         OboGraphInterface.descendants,
         SemanticSimilarityInterface.get_information_content,
         SemanticSimilarityInterface.information_content_scores,
+        AssociationProviderInterface.associations,
+        AssociationProviderInterface.add_associations,
     ]
 
+    custom_ic_map_path: str = None
+
     semsimian_object_cache: Dict[Tuple[PRED_CURIE], Optional["Semsimian"]] = field(default_factory=dict)  # type: ignore # noqa
 
     def __post_init__(self):
         slug = self.resource.slug
         from oaklib.selector import get_adapter
 
         slug = slug.replace("semsimian:", "")
@@ -75,24 +82,29 @@
         ]
 
     def _get_semsimian_object(
         self,
         predicates: List[PRED_CURIE] = None,
         attributes: List[str] = None,
         resource_path: str = None,
+        custom_ic_map_path: str = None,
     ) -> "Semsimian":  # type: ignore # noqa
         """
         Get Semsimian object from "semsimian_object_cache" or add a new one.
 
         :param predicates: collection of predicates, defaults to None
         :return: A Semsimian object.
         """
         from semsimian import Semsimian
 
         predicates = tuple(sorted(predicates))
+
+        if custom_ic_map_path is not None:
+            logging.info(f"Using custom IC map with Semsimian: {custom_ic_map_path}")
+
         if predicates not in self.semsimian_object_cache:
             # spo = [
             #     r
             #     for r in self.wrapped_adapter.relationships(
             #         include_entailed=True, predicates=predicates
             #     )
             # ]
@@ -102,14 +114,15 @@
                 self.resource_path = str(self.wrapped_adapter.engine.url)
 
             self.semsimian_object_cache[predicates] = Semsimian(
                 spo=None,
                 predicates=predicates,
                 pairwise_similarity_attributes=attributes,
                 resource_path=self.resource_path,
+                custom_ic_map_path=self.custom_ic_map_path,
             )
 
         return self.semsimian_object_cache[predicates]
 
     def pairwise_similarity(
         self,
         subject: CURIE,
@@ -130,15 +143,17 @@
         :param object_ancestors: optional pre-generated ancestor list
         :param min_jaccard_similarity: optional minimum jaccard similarity
         :param min_ancestor_information_content: optional minimum ancestor information content
         :return:
         """
         logging.debug(f"Calculating pairwise similarity for {subject} x {object} over {predicates}")
         semsimian = self._get_semsimian_object(
-            predicates=predicates, attributes=self.term_pairwise_similarity_attributes
+            predicates=predicates,
+            attributes=self.term_pairwise_similarity_attributes,
+            custom_ic_map_path=self.custom_ic_map_path,
         )
 
         jaccard_val = semsimian.jaccard_similarity(subject, object)
 
         if math.isnan(jaccard_val):
             return None
 
@@ -185,15 +200,17 @@
         :param objects:
         :param predicates:
         :return:
         """
         objects = list(objects)
         logging.info(f"Calculating all-by-all pairwise similarity for {len(objects)} objects")
         semsimian = self._get_semsimian_object(
-            predicates=predicates, attributes=self.term_pairwise_similarity_attributes
+            predicates=predicates,
+            attributes=self.term_pairwise_similarity_attributes,
+            custom_ic_map_path=self.custom_ic_map_path,
         )
         all_results = semsimian.all_by_all_pairwise_similarity(
             subject_terms=set(subjects),
             object_terms=set(objects),
             minimum_jaccard_threshold=min_jaccard_similarity,
             minimum_resnik_threshold=min_ancestor_information_content,
             # predicates=set(predicates) if predicates else None,
```

### Comparing `oaklib-0.6.6/src/oaklib/implementations/simpleobo/simple_obo_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/simpleobo/simple_obo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/simpleobo/simple_obo_parser.py` & `oaklib-0.6.7/src/oaklib/implementations/simpleobo/simple_obo_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/sparql/abstract_sparql_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/sparql/abstract_sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/sparql/lov_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/sparql/lov_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/sparql/oak_metamodel_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/sparql/oak_metamodel_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/sparql/sparql_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/sparql/sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/sparql/sparql_query.py` & `oaklib-0.6.7/src/oaklib/implementations/sparql/sparql_query.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/sqldb/sql_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/sqldb/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/sqldb/sqlite_utils.py` & `oaklib-0.6.7/src/oaklib/implementations/sqldb/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/tabular/robot_template_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/tabular/robot_template_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/tabular/tabular_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/tabular/tabular_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/translator/translator_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/translator/translator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/ubergraph/ubergraph_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/ubergraph/ubergraph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/uniprot/uniprot_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/uniprot/uniprot_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/implementations/wikidata/wikidata_implementation.py` & `oaklib-0.6.7/src/oaklib/implementations/wikidata/wikidata_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/indexes/edge_index.py` & `oaklib-0.6.7/src/oaklib/indexes/edge_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/inference/owl_reasoner.py` & `oaklib-0.6.7/src/oaklib/inference/owl_reasoner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/inference/relation_graph_reasoner.py` & `oaklib-0.6.7/src/oaklib/inference/relation_graph_reasoner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/__init__.py` & `oaklib-0.6.7/src/oaklib/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/association_provider_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/association_provider_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
                 objects = list(
                     self.descendants(list(objects), predicates=object_closure_predicates)
                 )
             else:
                 raise NotImplementedError
         ix = self._association_index
         if ix is None:
-            logging.warning("No association index")
+            logging.warning(f"No association index for {type(self)}")
             return
         yield from ix.lookup(subjects, predicates, objects)
 
     def _inject_subject_labels(self, association_iterator: Iterable[Association]):
         for assoc_it in chunk(association_iterator):
             associations = list(assoc_it)
             subjects = {a.subject for a in associations}
@@ -460,29 +460,30 @@
             subject_closure_predicates=subject_closure_predicates,
             predicate_closure_predicates=predicate_closure_predicates,
             include_modified=include_modified,
             **kwargs,
         )
         assoc_map = defaultdict(list)
         cached = {}
-        if isinstance(self, OboGraphInterface):
-            for association in association_it:
-                if group_by == "object":
-                    grp = association.object
-                    if grp not in cached:
-                        grps = list(self.ancestors([grp], predicates=object_closure_predicates))
-                        cached[grp] = grps
-                    else:
-                        grps = cached[grp]
-                elif group_by == "subject":
-                    grps = [association.subject]
+        if not isinstance(self, OboGraphInterface):
+            raise ValueError("This method requires an OboGraphInterface")
+        for association in association_it:
+            if group_by == "object":
+                grp = association.object
+                if grp not in cached:
+                    grps = list(self.ancestors([grp], predicates=object_closure_predicates))
+                    cached[grp] = grps
                 else:
-                    raise ValueError(f"Unknown group_by: {group_by}")
-                for grp in grps:
-                    assoc_map[grp].append(association)
+                    grps = cached[grp]
+            elif group_by == "subject":
+                grps = [association.subject]
+            else:
+                raise ValueError(f"Unknown group_by: {group_by}")
+            for grp in grps:
+                assoc_map[grp].append(association)
         for k, v in assoc_map.items():
             yield k, len(v)
 
     def association_subject_counts(
         self,
         subjects: Iterable[CURIE] = None,
         predicates: Iterable[PRED_CURIE] = None,
```

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/basic_ontology_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/basic_ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/class_enrichment_calculation_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/class_enrichment_calculation_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,10 +209,12 @@
         GO:0016020 membrane 0.004
         ...
 
 
         """
         assocs = []
         for e in self.entities(filter_obsoletes=True):
+            if e.startswith("<"):
+                continue
             assoc = Association(subject=e, predicate=EQUIVALENT_CLASS, object=e)
             assocs.append(assoc)
         self.add_associations(assocs)
```

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/differ_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/differ_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/dumper_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/dumper_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/embedding_provider_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/embedding_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/mapping_provider_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/mapping_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/merge_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/merge_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/metadata_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/metadata_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/obograph_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/obograph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/obolegacy_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/obolegacy_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/ontology_generator_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/ontology_generator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/ontology_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/owl_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/owl_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/patcher_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/patcher_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/rdf_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/rdf_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/relation_graph_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/relation_graph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/search_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/semsim_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/semsim_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -217,44 +217,49 @@
         :param object_closure_predicates:
         :param use_associations:
         :param term_to_entities_map:
         :param kwargs:
         :return:
         """
         curies = list(curies)
-        if self.cached_information_content_map is not None:
-            for curie in curies:
-                if curie in self.cached_information_content_map:
-                    yield curie, self.cached_information_content_map[curie]
-            return
-        if use_associations:
+        if self.cached_information_content_map is None and use_associations:
+            logging.info("Calculating and caching IC map from associations")
             from oaklib.interfaces.association_provider_interface import (
                 AssociationProviderInterface,
             )
 
             if not isinstance(self, AssociationProviderInterface):
                 raise ValueError(
                     f"unable to retrieve associations from this interface, type {type(self)}"
                 )
+            self.cached_information_content_map = {}
             all_entities = set()
             for a in self.associations():
                 all_entities.add(a.subject)
             num_entities = len(all_entities)
             logging.info(f"num_entities={num_entities}")
+            for term, count in self.association_subject_counts(
+                predicates=predicates, object_closure_predicates=object_closure_predicates
+            ):
+                if count > num_entities:
+                    raise AssertionError(f"Count {count} > num_entities {num_entities}")
+                self.cached_information_content_map[term] = -math.log(
+                    count / num_entities
+                ) / math.log(2)
+            if curies:
+                for curie in curies:
+                    if curie not in self.cached_information_content_map:
+                        self.cached_information_content_map[curie] = 0.0
+        if self.cached_information_content_map is not None:
+            logging.info("Using cached IC map")
             for curie in curies:
-                entities = list(
-                    self.associations_subjects(
-                        objects=[curie],
-                        predicates=predicates,
-                        object_closure_predicates=object_closure_predicates,
-                    )
-                )
-                if entities:
-                    yield curie, -math.log(len(entities) / num_entities)
+                if curie in self.cached_information_content_map:
+                    yield curie, self.cached_information_content_map[curie]
             return
+        logging.info("Calculating and caching IC map from ontology")
         all_entities = list(self.entities())
         num_entities = len(all_entities)
         if not isinstance(self, OboGraphInterface):
             raise NotImplementedError
         yielded_owl_thing = False
         for curie in curies:
             descendants = list(self.descendants([curie], object_closure_predicates))
```

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/skos_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/skos_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/subsetter_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/subsetter_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/summary_statistics_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/summary_statistics_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/taxon_constraint_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/taxon_constraint_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/text_annotator_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/text_annotator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/interfaces/validator_interface.py` & `oaklib-0.6.7/src/oaklib/interfaces/validator_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from abc import ABC
 from typing import Any, Dict, Iterable, List, Optional, Union
 
 from linkml_runtime.dumpers import json_dumper
 
 from oaklib.datamodels.ontology_metadata import DefinitionConstraintComponent
 from oaklib.datamodels.synonymizer_datamodel import RuleSet
@@ -286,14 +287,17 @@
         Lookup references in external ontologies.
 
         :param references: list of CURIEs to look up
         :param adapters: adapter mapping to look up external entities
         :param kwargs: additional arguments
         :return: mapping between CURIEs and pub objects
         """
+        if None in references:
+            logging.warning(f"Null in references: {references}")
+            references = [r for r in references if r]
         pubmed_wrapper = PubmedWrapper()
         pub_prefixes = ["PMID", "DOI", "PMC", "PMCID"]
         publication_ids = [
             x for x in references if any(x.upper().startswith(y) for y in pub_prefixes)
         ]
         objs = pubmed_wrapper.objects_by_ids(publication_ids)
         # seed with Nones
```

### Comparing `oaklib-0.6.6/src/oaklib/io/heatmap_writer.py` & `oaklib-0.6.7/src/oaklib/io/heatmap_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/html_writer.py` & `oaklib-0.6.7/src/oaklib/io/html_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/obograph_writer.py` & `oaklib-0.6.7/src/oaklib/io/obograph_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/rollup_report_writer.py` & `oaklib-0.6.7/src/oaklib/io/rollup_report_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/streaming_axiom_writer.py` & `oaklib-0.6.7/src/oaklib/io/streaming_axiom_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/streaming_csv_writer.py` & `oaklib-0.6.7/src/oaklib/io/streaming_csv_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/streaming_fhir_writer.py` & `oaklib-0.6.7/src/oaklib/io/streaming_fhir_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/streaming_info_writer.py` & `oaklib-0.6.7/src/oaklib/io/streaming_info_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/streaming_json_lines_writer.py` & `oaklib-0.6.7/src/oaklib/io/streaming_json_lines_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/streaming_json_writer.py` & `oaklib-0.6.7/src/oaklib/io/streaming_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/streaming_kgcl_writer.py` & `oaklib-0.6.7/src/oaklib/io/streaming_kgcl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/streaming_markdown_writer.py` & `oaklib-0.6.7/src/oaklib/io/streaming_markdown_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/streaming_nl_writer.py` & `oaklib-0.6.7/src/oaklib/io/streaming_nl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/streaming_obo_json_writer.py` & `oaklib-0.6.7/src/oaklib/io/streaming_obo_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/streaming_obo_writer.py` & `oaklib-0.6.7/src/oaklib/io/streaming_obo_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/streaming_owl_functional_writer.py` & `oaklib-0.6.7/src/oaklib/io/streaming_owl_functional_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/streaming_rdf_writer.py` & `oaklib-0.6.7/src/oaklib/io/streaming_rdf_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/streaming_writer.py` & `oaklib-0.6.7/src/oaklib/io/streaming_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/io/streaming_yaml_writer.py` & `oaklib-0.6.7/src/oaklib/io/streaming_yaml_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/mappers/base_mapper.py` & `oaklib-0.6.7/src/oaklib/mappers/base_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/mappers/ontology_metadata_mapper.py` & `oaklib-0.6.7/src/oaklib/mappers/ontology_metadata_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/parsers/__init__.py` & `oaklib-0.6.7/src/oaklib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/parsers/association_parser.py` & `oaklib-0.6.7/src/oaklib/parsers/association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/parsers/association_parser_factory.py` & `oaklib-0.6.7/src/oaklib/parsers/association_parser_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/parsers/boomer_parser.py` & `oaklib-0.6.7/src/oaklib/parsers/boomer_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/parsers/gaf_association_parser.py` & `oaklib-0.6.7/src/oaklib/parsers/gaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/parsers/gencc_association_parser.py` & `oaklib-0.6.7/src/oaklib/parsers/gencc_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/parsers/hpoa_association_parser.py` & `oaklib-0.6.7/src/oaklib/parsers/hpoa_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/parsers/hpoa_g2d_association_parser.py` & `oaklib-0.6.7/src/oaklib/parsers/hpoa_g2d_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/parsers/hpoa_g2p_association_parser.py` & `oaklib-0.6.7/src/oaklib/parsers/hpoa_g2p_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/parsers/kgx_association_parser.py` & `oaklib-0.6.7/src/oaklib/parsers/kgx_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/parsers/mim2gene_association_parser.py` & `oaklib-0.6.7/src/oaklib/parsers/mim2gene_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/parsers/pairwise_association_parser.py` & `oaklib-0.6.7/src/oaklib/parsers/pairwise_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/parsers/parser_base.py` & `oaklib-0.6.7/src/oaklib/parsers/parser_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/parsers/phaf_association_parser.py` & `oaklib-0.6.7/src/oaklib/parsers/phaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/parsers/xaf_association_parser.py` & `oaklib-0.6.7/src/oaklib/parsers/xaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/resource.py` & `oaklib-0.6.7/src/oaklib/resource.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/selector.py` & `oaklib-0.6.7/src/oaklib/selector.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/transformers/chained_ontology_transformer.py` & `oaklib-0.6.7/src/oaklib/transformers/chained_ontology_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/transformers/edge_filter_transformer.py` & `oaklib-0.6.7/src/oaklib/transformers/edge_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/transformers/graph_transformer.py` & `oaklib-0.6.7/src/oaklib/transformers/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/transformers/node_filter_transformer.py` & `oaklib-0.6.7/src/oaklib/transformers/node_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/transformers/sep_transformer.py` & `oaklib-0.6.7/src/oaklib/transformers/sep_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/transformers/transformers_factory.py` & `oaklib-0.6.7/src/oaklib/transformers/transformers_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/apikey_manager.py` & `oaklib-0.6.7/src/oaklib/utilities/apikey_manager.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/associations/association_differ.py` & `oaklib-0.6.7/src/oaklib/utilities/associations/association_differ.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/associations/association_index.py` & `oaklib-0.6.7/src/oaklib/utilities/associations/association_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py` & `oaklib-0.6.7/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/axioms/logical_definition_analyzer.py` & `oaklib-0.6.7/src/oaklib/utilities/axioms/logical_definition_analyzer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/axioms/logical_definition_summarizer.py` & `oaklib-0.6.7/src/oaklib/utilities/axioms/logical_definition_summarizer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/axioms/logical_definition_utilities.py` & `oaklib-0.6.7/src/oaklib/utilities/axioms/logical_definition_utilities.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import List, Optional
 
+from oaklib import BasicOntologyInterface
 from oaklib.datamodels.obograph import LogicalDefinitionAxiom
 from oaklib.datamodels.vocabulary import IS_A
+from oaklib.interfaces import OboGraphInterface
 from oaklib.types import CURIE, PRED_CURIE
 
 
 def logical_definition_matches(
     ldef: LogicalDefinitionAxiom,
     subjects: Optional[List[CURIE]] = None,
     predicates: Optional[List[PRED_CURIE]] = None,
@@ -53,7 +55,34 @@
         if objects:
             if not class_signature.intersection(objects):
                 return False
     if subjects:
         if ldef.definedClassId not in subjects:
             return False
     return True
+
+
+def roll_up_to_genus(
+    term: CURIE, adapter: BasicOntologyInterface, predicates: List[PRED_CURIE]
+) -> CURIE:
+    """
+    Walks up the genus hierarchy.
+
+    This can be used to extract the "meaningful" genus of a compositional term
+
+    :param term:
+    :param adapter:
+    :param predicates:
+    :return:
+    """
+    if not isinstance(adapter, OboGraphInterface):
+        raise NotImplementedError
+    replacement = None
+    for ldef in adapter.logical_definitions([term]):
+        if len(ldef.restrictions) == 1 and len(ldef.genusIds) == 1:
+            restr = ldef.restrictions[0]
+            if restr.propertyId in predicates:
+                replacement = ldef.genusIds[0]
+    if replacement:
+        return roll_up_to_genus(replacement, adapter, predicates)
+    else:
+        return term
```

### Comparing `oaklib-0.6.6/src/oaklib/utilities/basic_utils.py` & `oaklib-0.6.7/src/oaklib/utilities/basic_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/format_utilities.py` & `oaklib-0.6.7/src/oaklib/utilities/format_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/graph/networkx_bridge.py` & `oaklib-0.6.7/src/oaklib/utilities/graph/networkx_bridge.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/graph/relationship_walker.py` & `oaklib-0.6.7/src/oaklib/utilities/graph/relationship_walker.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/identifier_utils.py` & `oaklib-0.6.7/src/oaklib/utilities/identifier_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/iterator_utils.py` & `oaklib-0.6.7/src/oaklib/utilities/iterator_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/keyval_cache.py` & `oaklib-0.6.7/src/oaklib/utilities/keyval_cache.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/kgcl_utilities.py` & `oaklib-0.6.7/src/oaklib/utilities/kgcl_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/label_utilities.py` & `oaklib-0.6.7/src/oaklib/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/lexical/lexical_indexer.py` & `oaklib-0.6.7/src/oaklib/utilities/lexical/lexical_indexer.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,14 +107,15 @@
         synonym_rules.extend(
             [x.synonymizer for x in mapping_rule_collection.rules if x.synonymizer]
         )
     if pipelines is None:
         steps = [
             LexicalTransformation(TransformationType.CaseNormalization),
             LexicalTransformation(TransformationType.WhitespaceNormalization),
+            # LexicalTransformation(TransformationType.WordOrderNormalization),
         ]
         if synonym_rules:
             steps.append(
                 LexicalTransformation(TransformationType.Synonymization, params=synonym_rules)
             )
         pipelines = [LexicalTransformationPipeline(name="default", transformations=steps)]
     logging.info(f"Creating lexical index, pipelines={pipelines}")
@@ -147,14 +148,17 @@
 
                 for pipeline in pipelines:
                     synonymized = False  # Flag indicating whether the term was synonymized or not.
                     term2 = term
                     for tr in pipeline.transformations:
                         if tr.type.code == TransformationType.Synonymization:
                             synonymized, term2, qualifier = apply_transformation(term2, tr)
+                            logging.debug(
+                                f"Synonymized: {synonymized} {term} => {term2} ({qualifier}) // {tr}"
+                            )
                             if qualifier != DEFAULT_QUALIFIER and qualifier is not None:
                                 pred = QUALIFIER_DICT[qualifier]
 
                         else:
                             term2 = apply_transformation(term2, tr)
 
                     rel = RelationshipToTerm(
@@ -469,26 +473,51 @@
     return True
 
 
 def apply_transformation(
     term: str, transformation: LexicalTransformation
 ) -> Union[str, Tuple[bool, str, str]]:
     """
-    Apply an individual transformation on a term
+    Apply an individual transformation on a term.
+
+    >>> apply_transformation("FooBar", LexicalTransformation(TransformationType.CaseNormalization))
+    'foobar'
+
+    >>> apply_transformation("foo   bar", LexicalTransformation(TransformationType.WhitespaceNormalization))
+    'foo bar'
+
+    >>> apply_transformation("bar, foo; abc", LexicalTransformation(TransformationType.WordOrderNormalization))
+    'abc bar foo'
+
+    >>> rule = Synonymizer(match=r"iest$", replacement="y")
+    >>> apply_transformation("fuzziest", LexicalTransformation(TransformationType.Synonymization, params=[rule]))
+    (True, 'fuzzy', None)
+
+    >>> rule = Synonymizer(match=r"iest$", replacement="y", qualifier="related")
+    >>> apply_transformation("fuzziest", LexicalTransformation(TransformationType.Synonymization, params=[rule]))
+    (True, 'fuzzy', 'related')
+
+    >>> rule = Synonymizer(match=r"iest$", replacement="y")
+    >>> apply_transformation("foo", LexicalTransformation(TransformationType.Synonymization, params=[rule]))
+    (False, 'foo', 'exact')
 
     :param term: Original label.
     :param transformation: Type of transformation to be performed on the label.
-    :return: Transformed label.
+    :return: Transformed label or tuple of (if the label changed, new label, qualifier)
     """
     typ = str(transformation.type)
     logging.debug(f"Applying: {transformation}")
     if typ == TransformationType.CaseNormalization.text:
         return term.lower()
     elif typ == TransformationType.WhitespaceNormalization.text:
         return re.sub(" {2,}", " ", term.strip())
+    elif typ == TransformationType.WordOrderNormalization.text:
+        toks = term.split()
+        toks = [x.rstrip(",;") for x in toks]
+        return " ".join(sorted(toks))
     elif typ == TransformationType.Synonymization.text:
         synonymized_results = apply_synonymizer(term, transformation.params)
         true_results = [x for x in list(synonymized_results) if x[0] is True]
         if len(true_results) > 0:
             return true_results[-1]
         else:
             return (False, term, DEFAULT_QUALIFIER)
```

### Comparing `oaklib-0.6.6/src/oaklib/utilities/lexical/patternizer.py` & `oaklib-0.6.7/src/oaklib/utilities/lexical/patternizer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/lexical/synonymizer.py` & `oaklib-0.6.7/src/oaklib/utilities/lexical/synonymizer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/mapping/boomer_utils.py` & `oaklib-0.6.7/src/oaklib/utilities/mapping/boomer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/mapping/cross_ontology_diffs.py` & `oaklib-0.6.7/src/oaklib/utilities/mapping/cross_ontology_diffs.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/mapping/mapping_propagator.py` & `oaklib-0.6.7/src/oaklib/utilities/mapping/mapping_propagator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/mapping/mapping_validation.py` & `oaklib-0.6.7/src/oaklib/utilities/mapping/mapping_validation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/mapping/sssom_utils.py` & `oaklib-0.6.7/src/oaklib/utilities/mapping/sssom_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/ner_utilities.py` & `oaklib-0.6.7/src/oaklib/utilities/ner_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/nlp/natual_language_generation.py` & `oaklib-0.6.7/src/oaklib/utilities/nlp/natual_language_generation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/obograph_utils.py` & `oaklib-0.6.7/src/oaklib/utilities/obograph_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/ontology_builder.py` & `oaklib-0.6.7/src/oaklib/utilities/ontology_builder.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/publication_utils/doi_wrapper.py` & `oaklib-0.6.7/src/oaklib/utilities/publication_utils/doi_wrapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/publication_utils/pubdb_wrapper.py` & `oaklib-0.6.7/src/oaklib/utilities/publication_utils/pubdb_wrapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/publication_utils/pubmed_wrapper.py` & `oaklib-0.6.7/src/oaklib/utilities/publication_utils/pubmed_wrapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/reasoning/relation_graph.py` & `oaklib-0.6.7/src/oaklib/utilities/reasoning/relation_graph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/semsim/similarity_utils.py` & `oaklib-0.6.7/src/oaklib/utilities/semsim/similarity_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/stats/hypergeometric.py` & `oaklib-0.6.7/src/oaklib/utilities/stats/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/subsets/slimmer_utils.py` & `oaklib-0.6.7/src/oaklib/utilities/subsets/slimmer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/subsets/subset_analysis.py` & `oaklib-0.6.7/src/oaklib/utilities/subsets/subset_analysis.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/subsets/value_set_expander.py` & `oaklib-0.6.7/src/oaklib/utilities/subsets/value_set_expander.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/table_filler.py` & `oaklib-0.6.7/src/oaklib/utilities/table_filler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/taxon/taxon_constraint_utils.py` & `oaklib-0.6.7/src/oaklib/utilities/taxon/taxon_constraint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/validation/definition_ontology_rule.py` & `oaklib-0.6.7/src/oaklib/utilities/validation/definition_ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/validation/disjointness_rule.py` & `oaklib-0.6.7/src/oaklib/utilities/validation/disjointness_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/validation/lint_utils.py` & `oaklib-0.6.7/src/oaklib/utilities/validation/lint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/validation/ontology_rule.py` & `oaklib-0.6.7/src/oaklib/utilities/validation/ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/validation/rule_runner.py` & `oaklib-0.6.7/src/oaklib/utilities/validation/rule_runner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/src/oaklib/utilities/writers/change_handler.py` & `oaklib-0.6.7/src/oaklib/utilities/writers/change_handler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.6/PKG-INFO` & `oaklib-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaklib
-Version: 0.6.6
+Version: 0.6.7
 Summary: Ontology Access Kit: Python library for common ontology operations over a variety of backends
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

