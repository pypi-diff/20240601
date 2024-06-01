# Comparing `tmp/pyaedt-0.9.2.tar.gz` & `tmp/pyaedt-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyaedt-0.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyaedt-0.9.2.tar` & `pyaedt-0.9.3.tar`

### file list

```diff
@@ -1,217 +1,216 @@
--rw-r--r--   0        0        0     1090 2024-05-29 06:44:51.797667 pyaedt-0.9.2/LICENSE
--rw-r--r--   0        0        0    11391 2024-05-29 06:44:51.797667 pyaedt-0.9.2/README.md
--rw-r--r--   0        0        0     3339 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/__init__.py
--rw-r--r--   0        0        0    32198 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6766 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    90755 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    55394 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    11416 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3136 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    13300 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4487 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4723 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   141518 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/application/Design.py
--rw-r--r--   0        0        0     5985 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    79373 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12942 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    15469 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/application/analysis_hf.py
--rw-r--r--   0        0        0    37712 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    79315 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/circuit.py
--rw-r--r--   0        0        0    10493 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    86016 2024-05-29 06:44:53.829676 pyaedt-0.9.2/pyaedt/desktop.py
--rw-r--r--   0        0        0    25696 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/downloads.py
--rw-r--r--   0        0        0      202 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/edb.py
--rw-r--r--   0        0        0    10953 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/emit.py
--rw-r--r--   0        0        0     5884 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     3685 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0     2574 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/emit_core/emit_constants.py
--rw-r--r--   0        0        0        1 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7262 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    29659 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0     9836 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/Ansys.png
--rw-r--r--   0        0        0      737 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/AnsysTemplate.json
--rw-r--r--   0        0        0    15327 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    16041 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     1345 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/ami.json
--rw-r--r--   0        0        0     3356 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0        0 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/com_parameters.py
--rw-r--r--   0        0        0    36938 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/compliance.py
--rw-r--r--   0        0        0    89198 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    27640 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    72540 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0      184 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/desktop_sessions.py
--rw-r--r--   0        0        0     3914 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    67824 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0    14707 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/grpc_plugin_dll_class.py
--rw-r--r--   0        0        0    43045 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     2642 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/ibis_v7.json
--rw-r--r--   0        0        0     6857 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0    21288 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    65974 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    19739 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3468 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    17193 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/settings.py
--rw-r--r--   0        0        0    25002 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/spisim.py
--rw-r--r--   0        0        0    19961 2024-05-29 06:44:53.833675 pyaedt-0.9.2/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0   249460 2024-05-29 06:44:53.837676 pyaedt-0.9.2/pyaedt/hfss.py
--rw-r--r--   0        0        0    84141 2024-05-29 06:44:53.837676 pyaedt-0.9.2/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   269765 2024-05-29 06:44:53.837676 pyaedt-0.9.2/pyaedt/icepak.py
--rw-r--r--   0        0        0   128452 2024-05-29 06:44:53.837676 pyaedt-0.9.2/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7746 2024-05-29 06:44:53.837676 pyaedt-0.9.2/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24017 2024-05-29 06:44:53.837676 pyaedt-0.9.2/pyaedt/mechanical.py
--rw-r--r--   0        0        0     2154 2024-05-29 06:44:53.837676 pyaedt-0.9.2/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0      198 2024-05-29 06:44:53.837676 pyaedt-0.9.2/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    19281 2024-05-29 06:44:53.837676 pyaedt-0.9.2/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     2536 2024-05-29 06:44:53.837676 pyaedt-0.9.2/pyaedt/misc/ansys_cloud.areg
--rw-r--r--   0        0        0     1951 2024-05-29 06:44:53.837676 pyaedt-0.9.2/pyaedt/misc/config.schema.json
--rw-r--r--   0        0        0       44 2024-05-29 06:44:53.837676 pyaedt-0.9.2/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0     2623 2024-05-29 06:44:53.837676 pyaedt-0.9.2/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   744826 2024-05-29 06:44:53.841676 pyaedt-0.9.2/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2024-05-29 06:44:53.841676 pyaedt-0.9.2/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2024-05-29 06:44:53.841676 pyaedt-0.9.2/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2024-05-29 06:44:53.841676 pyaedt-0.9.2/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      277 2024-05-29 06:44:53.841676 pyaedt-0.9.2/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      960 2024-05-29 06:44:53.841676 pyaedt-0.9.2/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2024-05-29 06:44:53.841676 pyaedt-0.9.2/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0       58 2024-05-29 06:44:53.841676 pyaedt-0.9.2/pyaedt/misc/spisim_com_configuration_files/__init__.py
--rw-r--r--   0        0        0     5001 2024-05-29 06:44:53.841676 pyaedt-0.9.2/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json
--rw-r--r--   0        0        0     4962 2024-05-29 06:44:53.841676 pyaedt-0.9.2/pyaedt/misc/spisim_com_configuration_files/com_93_8.json
--rw-r--r--   0        0        0     4964 2024-05-29 06:44:53.841676 pyaedt-0.9.2/pyaedt/misc/spisim_com_configuration_files/com_94_17.json
--rw-r--r--   0        0        0    11888 2024-05-29 06:44:53.841676 pyaedt-0.9.2/pyaedt/misc/spisim_com_configuration_files/com_parameters.py
--rw-r--r--   0        0        0    15075 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py
--rw-r--r--   0        0        0      577 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/misc/tb_nexxim_mapping.toml
--rw-r--r--   0        0        0      868 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    13650 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    19389 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18045 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16174 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   122675 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0    78334 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   333130 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    14806 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   142563 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    28939 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/cad/component_array.py
--rw-r--r--   0        0        0    40951 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    47933 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    58475 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    51586 2024-05-29 06:44:53.845676 pyaedt-0.9.2/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12204 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    43496 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    38149 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8247 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    66421 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    14701 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    35800 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    66209 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6750 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    71849 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    31625 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    49876 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    63930 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    23403 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    50195 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   166694 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    70334 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    15739 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    55348 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    39012 2024-05-29 06:44:53.849676 pyaedt-0.9.2/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0   103157 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    32810 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53456 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11939 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    54338 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4309 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   215452 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    70341 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   147490 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    32118 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    30459 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   133787 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   138613 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    94112 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/q3d.py
--rw-r--r--   0        0        0    10417 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      398 2024-05-29 06:44:53.853676 pyaedt-0.9.2/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    41447 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9235 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2050 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2546 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       94 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      717 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2795 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1352 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      325 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    35749 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4195 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    30633 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1460 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20283 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14337 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      303 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2528 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7410 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    20988 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     1153 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/circuit/__init__.py
--rw-r--r--   0        0        0    23464 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/customize_automation_tab.py
--rw-r--r--   0        0        0     1153 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/emit/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/hfss/__init__.py
--rw-r--r--   0        0        0     1145 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/hfss/images/large/antenna.png
--rw-r--r--   0        0        0     1987 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/hfss/images/large/push.png
--rw-r--r--   0        0        0     3391 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/hfss/push_excitation_from_file.py
--rw-r--r--   0        0        0      456 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/hfss/toolkits_catalog.toml
--rw-r--r--   0        0        0     1153 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/hfss3dlayout/__init__.py
--rw-r--r--   0        0        0     3509 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/hfss3dlayout/export_to_3D.py
--rw-r--r--   0        0        0     2447 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/hfss3dlayout/images/large/cad3d.png
--rw-r--r--   0        0        0      140 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/hfss3dlayout/toolkits_catalog.toml
--rw-r--r--   0        0        0     1153 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/icepak/__init__.py
--rw-r--r--   0        0        0    35360 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/images/large/logo.png
--rw-r--r--   0        0        0      855 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/images/large/pyansys.png
--rw-r--r--   0        0        0     1153 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/installer/__init__.py
--rw-r--r--   0        0        0     3454 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/installer/console_setup.py
--rw-r--r--   0        0        0     1511 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/installer/create_report.py
--rw-r--r--   0        0        0    15102 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/installer/extension_manager.py
--rw-r--r--   0        0        0      477 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/installer/extensions_catalog.toml
--rw-r--r--   0        0        0     1247 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/installer/images/large/console.png
--rw-r--r--   0        0        0      719 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/installer/images/large/extension_manager.png
--rw-r--r--   0        0        0     1920 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/installer/images/large/jupyter.png
--rw-r--r--   0        0        0     1845 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/installer/images/large/run_script.png
--rw-r--r--   0        0        0     1649 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/installer/jupyter_template.ipynb
--rw-r--r--   0        0        0     3745 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/installer/pyaedt_installer.py
--rw-r--r--   0        0        0     1153 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/maxwell2d/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/maxwell3d/__init__.py
--rw-r--r--   0        0        0     1206 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/maxwell3d/images/large/magnet_segmentation.png
--rw-r--r--   0        0        0      302 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/maxwell3d/toolkits_catalog.toml
--rw-r--r--   0        0        0     1153 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/mechanical/__init__.py
--rw-r--r--   0        0        0     2214 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/misc.py
--rw-r--r--   0        0        0     1153 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/project/__init__.py
--rw-r--r--   0        0        0     1571 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/project/create_report.py
--rw-r--r--   0        0        0     2447 2024-05-29 06:44:53.857676 pyaedt-0.9.2/pyaedt/workflows/project/images/large/cad3d.png
--rw-r--r--   0        0        0      573 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/project/images/large/pdf.png
--rw-r--r--   0        0        0     4293 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/project/import_nastran.py
--rw-r--r--   0        0        0      302 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/project/toolkits_catalog.toml
--rw-r--r--   0        0        0     1153 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/q2d/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/q3d/__init__.py
--rw-r--r--   0        0        0     1153 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/templates/__init__.py
--rw-r--r--   0        0        0     3651 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/templates/jupyter.py_build
--rw-r--r--   0        0        0     3370 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/templates/pyaedt_console.py_build
--rw-r--r--   0        0        0     5555 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/templates/pyaedt_utils.py
--rw-r--r--   0        0        0     3349 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/templates/run_extension_manager.py_build
--rw-r--r--   0        0        0     3633 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/templates/run_pyaedt_script.py_build
--rw-r--r--   0        0        0     3329 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/templates/run_pyaedt_toolkit_script.py_build
--rw-r--r--   0        0        0     1866 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/templates/toolkit_template.py
--rw-r--r--   0        0        0     1153 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/twinbuilder/__init__.py
--rw-r--r--   0        0        0     5031 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/twinbuilder/convert_to_circuit.py
--rw-r--r--   0        0        0      552 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/twinbuilder/images/large/export_to_circuit.png
--rw-r--r--   0        0        0      171 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyaedt/workflows/twinbuilder/toolkits_catalog.toml
--rw-r--r--   0        0        0     6600 2024-05-29 06:44:53.861676 pyaedt-0.9.2/pyproject.toml
--rw-r--r--   0        0        0    17255 1970-01-01 00:00:00.000000 pyaedt-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-06-01 14:51:30.643876 pyaedt-0.9.3/LICENSE
+-rw-r--r--   0        0        0    11391 2024-06-01 14:51:30.643876 pyaedt-0.9.3/README.md
+-rw-r--r--   0        0        0     3339 2024-06-01 14:51:32.687881 pyaedt-0.9.3/pyaedt/__init__.py
+-rw-r--r--   0        0        0    32198 2024-06-01 14:51:32.687881 pyaedt-0.9.3/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6766 2024-06-01 14:51:32.687881 pyaedt-0.9.3/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    90755 2024-06-01 14:51:32.687881 pyaedt-0.9.3/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    55394 2024-06-01 14:51:32.687881 pyaedt-0.9.3/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    11416 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3136 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    13300 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4487 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4723 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   141518 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     5985 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    79373 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12942 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    15469 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/application/analysis_hf.py
+-rw-r--r--   0        0        0    37712 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    79315 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10493 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    87007 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/desktop.py
+-rw-r--r--   0        0        0    25694 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/downloads.py
+-rw-r--r--   0        0        0      202 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/edb.py
+-rw-r--r--   0        0        0    10953 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/emit.py
+-rw-r--r--   0        0        0     5884 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     3685 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0     2574 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/emit_core/emit_constants.py
+-rw-r--r--   0        0        0        1 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7262 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    29699 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0     9836 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/generic/Ansys.png
+-rw-r--r--   0        0        0      737 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/generic/AnsysTemplate.json
+-rw-r--r--   0        0        0    15327 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    16041 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     1345 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/generic/ami.json
+-rw-r--r--   0        0        0     3356 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0        0 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/generic/com_parameters.py
+-rw-r--r--   0        0        0    36938 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/generic/compliance.py
+-rw-r--r--   0        0        0    89198 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    27640 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    72540 2024-06-01 14:51:32.691881 pyaedt-0.9.3/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0      184 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/generic/desktop_sessions.py
+-rw-r--r--   0        0        0     3914 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    67817 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0    14679 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/generic/grpc_plugin_dll_class.py
+-rw-r--r--   0        0        0    43045 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     2642 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/generic/ibis_v7.json
+-rw-r--r--   0        0        0     6857 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0    21288 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    65974 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    19739 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3468 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    17193 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/generic/settings.py
+-rw-r--r--   0        0        0    25002 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/generic/spisim.py
+-rw-r--r--   0        0        0    19961 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0   249460 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/hfss.py
+-rw-r--r--   0        0        0    84141 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   269987 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/icepak.py
+-rw-r--r--   0        0        0   128452 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7746 2024-06-01 14:51:32.695881 pyaedt-0.9.3/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24017 2024-06-01 14:51:32.699881 pyaedt-0.9.3/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     2154 2024-06-01 14:51:32.699881 pyaedt-0.9.3/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0      198 2024-06-01 14:51:32.699881 pyaedt-0.9.3/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    19281 2024-06-01 14:51:32.699881 pyaedt-0.9.3/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     2536 2024-06-01 14:51:32.699881 pyaedt-0.9.3/pyaedt/misc/ansys_cloud.areg
+-rw-r--r--   0        0        0     1951 2024-06-01 14:51:32.699881 pyaedt-0.9.3/pyaedt/misc/config.schema.json
+-rw-r--r--   0        0        0       44 2024-06-01 14:51:32.699881 pyaedt-0.9.3/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0     2623 2024-06-01 14:51:32.699881 pyaedt-0.9.3/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   744826 2024-06-01 14:51:32.699881 pyaedt-0.9.3/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2024-06-01 14:51:32.699881 pyaedt-0.9.3/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      277 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      960 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0       58 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/misc/spisim_com_configuration_files/__init__.py
+-rw-r--r--   0        0        0     5001 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json
+-rw-r--r--   0        0        0     4962 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/misc/spisim_com_configuration_files/com_93_8.json
+-rw-r--r--   0        0        0     4964 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/misc/spisim_com_configuration_files/com_94_17.json
+-rw-r--r--   0        0        0    11888 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/misc/spisim_com_configuration_files/com_parameters.py
+-rw-r--r--   0        0        0    15075 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py
+-rw-r--r--   0        0        0      577 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/misc/tb_nexxim_mapping.toml
+-rw-r--r--   0        0        0      868 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    13650 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    19389 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18045 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16174 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   122675 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0    78334 2024-06-01 14:51:32.703881 pyaedt-0.9.3/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   333130 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    14806 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   142563 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    28939 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/cad/component_array.py
+-rw-r--r--   0        0        0    40951 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    47933 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    58475 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    51586 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12204 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    43496 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    38149 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8247 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    66421 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    14701 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    35800 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    66209 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6750 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    73064 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    31625 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    49876 2024-06-01 14:51:32.707881 pyaedt-0.9.3/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    63930 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    23403 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    50195 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   181021 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    70334 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    15739 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    55348 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    39012 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0   103157 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    32810 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53456 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    11939 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    54338 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4309 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   215452 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    70341 2024-06-01 14:51:32.711881 pyaedt-0.9.3/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   147490 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    32118 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    30459 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   133787 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   138407 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    96177 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10417 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      398 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    41447 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9235 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2050 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2546 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       94 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      717 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2795 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1352 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      325 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    35749 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4195 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    30633 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1460 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20283 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14337 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      303 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2528 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7410 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    20988 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     1153 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/workflows/__init__.py
+-rw-r--r--   0        0        0     1153 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/workflows/circuit/__init__.py
+-rw-r--r--   0        0        0    21991 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/workflows/customize_automation_tab.py
+-rw-r--r--   0        0        0     1153 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/workflows/emit/__init__.py
+-rw-r--r--   0        0        0     1153 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/workflows/hfss/__init__.py
+-rw-r--r--   0        0        0     1145 2024-06-01 14:51:32.715881 pyaedt-0.9.3/pyaedt/workflows/hfss/images/large/antenna.png
+-rw-r--r--   0        0        0     1987 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/hfss/images/large/push.png
+-rw-r--r--   0        0        0     6290 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/hfss/push_excitation_from_file.py
+-rw-r--r--   0        0        0      456 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/hfss/toolkits_catalog.toml
+-rw-r--r--   0        0        0     1153 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/hfss3dlayout/__init__.py
+-rw-r--r--   0        0        0     5735 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/hfss3dlayout/export_to_3d.py
+-rw-r--r--   0        0        0     2447 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/hfss3dlayout/images/large/cad3d.png
+-rw-r--r--   0        0        0      140 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/hfss3dlayout/toolkits_catalog.toml
+-rw-r--r--   0        0        0     1153 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/icepak/__init__.py
+-rw-r--r--   0        0        0    35360 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/images/large/logo.png
+-rw-r--r--   0        0        0      855 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/images/large/pyansys.png
+-rw-r--r--   0        0        0     1153 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/installer/__init__.py
+-rw-r--r--   0        0        0     3454 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/installer/console_setup.py
+-rw-r--r--   0        0        0    15104 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/installer/extension_manager.py
+-rw-r--r--   0        0        0      477 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/installer/extensions_catalog.toml
+-rw-r--r--   0        0        0     1247 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/installer/images/large/console.png
+-rw-r--r--   0        0        0      719 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/installer/images/large/extension_manager.png
+-rw-r--r--   0        0        0     1920 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/installer/images/large/jupyter.png
+-rw-r--r--   0        0        0     1845 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/installer/images/large/run_script.png
+-rw-r--r--   0        0        0     1649 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/installer/jupyter_template.ipynb
+-rw-r--r--   0        0        0     3745 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/installer/pyaedt_installer.py
+-rw-r--r--   0        0        0     1153 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/maxwell2d/__init__.py
+-rw-r--r--   0        0        0     1153 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/maxwell3d/__init__.py
+-rw-r--r--   0        0        0     1206 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/maxwell3d/images/large/magnet_segmentation.png
+-rw-r--r--   0        0        0      302 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/maxwell3d/toolkits_catalog.toml
+-rw-r--r--   0        0        0     1153 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/mechanical/__init__.py
+-rw-r--r--   0        0        0     3313 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/misc.py
+-rw-r--r--   0        0        0     1153 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/project/__init__.py
+-rw-r--r--   0        0        0     3312 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/project/create_report.py
+-rw-r--r--   0        0        0     2447 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/project/images/large/cad3d.png
+-rw-r--r--   0        0        0      573 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/project/images/large/pdf.png
+-rw-r--r--   0        0        0     8415 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/project/import_nastran.py
+-rw-r--r--   0        0        0      302 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/project/toolkits_catalog.toml
+-rw-r--r--   0        0        0     1153 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/q2d/__init__.py
+-rw-r--r--   0        0        0     1153 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/q3d/__init__.py
+-rw-r--r--   0        0        0     1153 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/templates/__init__.py
+-rw-r--r--   0        0        0     2526 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/templates/extension_template.py
+-rw-r--r--   0        0        0     3651 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/templates/jupyter.py_build
+-rw-r--r--   0        0        0     3370 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/templates/pyaedt_console.py_build
+-rw-r--r--   0        0        0     5555 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/templates/pyaedt_utils.py
+-rw-r--r--   0        0        0     3349 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/templates/run_extension_manager.py_build
+-rw-r--r--   0        0        0     3633 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/templates/run_pyaedt_script.py_build
+-rw-r--r--   0        0        0     3329 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/templates/run_pyaedt_toolkit_script.py_build
+-rw-r--r--   0        0        0     1153 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/twinbuilder/__init__.py
+-rw-r--r--   0        0        0     7104 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/twinbuilder/convert_to_circuit.py
+-rw-r--r--   0        0        0      552 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/twinbuilder/images/large/export_to_circuit.png
+-rw-r--r--   0        0        0      171 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyaedt/workflows/twinbuilder/toolkits_catalog.toml
+-rw-r--r--   0        0        0     7019 2024-06-01 14:51:32.719881 pyaedt-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    18015 1970-01-01 00:00:00.000000 pyaedt-0.9.3/PKG-INFO
```

### Comparing `pyaedt-0.9.2/LICENSE` & `pyaedt-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/README.md` & `pyaedt-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/__init__.py` & `pyaedt-0.9.3/pyaedt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 deprecation_warning()
 
 #
 
 pyaedt_path = os.path.dirname(__file__)
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 version = __version__
 
 #
 
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
```

### Comparing `pyaedt-0.9.2/pyaedt/aedt_logger.py` & `pyaedt-0.9.3/pyaedt/aedt_logger.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.9.3/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/application/Analysis.py` & `pyaedt-0.9.3/pyaedt/application/Analysis.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/application/Analysis3D.py` & `pyaedt-0.9.3/pyaedt/application/Analysis3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.9.3/pyaedt/application/Analysis3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.9.3/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.9.3/pyaedt/application/AnalysisNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.9.3/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.9.3/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/application/Design.py` & `pyaedt-0.9.3/pyaedt/application/Design.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/application/JobManager.py` & `pyaedt-0.9.3/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/application/Variables.py` & `pyaedt-0.9.3/pyaedt/application/Variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/application/aedt_objects.py` & `pyaedt-0.9.3/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/application/analysis_hf.py` & `pyaedt-0.9.3/pyaedt/application/analysis_hf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/application/design_solutions.py` & `pyaedt-0.9.3/pyaedt/application/design_solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/circuit.py` & `pyaedt-0.9.3/pyaedt/circuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/common_rpc.py` & `pyaedt-0.9.3/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/desktop.py` & `pyaedt-0.9.3/pyaedt/desktop.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from pyaedt.aedt_logger import AedtLogger
 from pyaedt.aedt_logger import pyaedt_logger
 from pyaedt.generic.general_methods import generate_unique_name
 
 if is_linux:
     os.environ["ANS_NODEPCHECK"] = str(1)
 
-if is_linux and is_ironpython:
+if is_linux and is_ironpython:  # pragma: no cover
     import subprocessdotnet as subprocess
 else:
     import subprocess
 
 from pyaedt import __version__
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.desktop_sessions import _desktop_sessions
@@ -243,35 +243,35 @@
     Returns
     -------
     bool
         ``True`` when successful, ``False`` when failed.
 
     """
     if settings.remote_rpc_session or (settings.aedt_version >= "2022.2" and is_grpc_api and not is_ironpython):
-        if close_desktop and desktop_class.parent_desktop_id:
+        if close_desktop and desktop_class.parent_desktop_id:  # pragma: no cover
             pyaedt_logger.error("A child desktop session is linked to this session.")
             pyaedt_logger.error("Multiple desktop sessions must be released in reverse order.")
             return False
         elif close_desktop:
             try:
                 os.kill(pid, 9)
                 if _desktop_sessions:
                     for v in _desktop_sessions.values():
-                        if pid in v.parent_desktop_id:
+                        if pid in v.parent_desktop_id:  # pragma: no cover
                             del v.parent_desktop_id[v.parent_desktop_id.index(pid)]
                 return True
             except Exception:  # pragma: no cover
                 warnings.warn("Something went wrong closing AEDT. Exception in `_main.oDesktop.QuitApplication()`.")
-        else:
+        else:  # pragma: no cover
             for k, d in _desktop_sessions.items():
                 if k == pid:
                     d.grpc_plugin.recreate_application(True)
                     d.grpc_plugin.Release()
                     return True
-    elif not inside_desktop:
+    elif not inside_desktop:  # pragma: no cover
         if close_desktop:
             try:
                 os.kill(pid, 9)
             except Exception:  # pragma: no cover
                 warnings.warn("Something went wrong closing AEDT. Exception in `os.kill(pid, 9)`.")
                 return False
         else:
@@ -280,15 +280,15 @@
                 while scopeID <= 5:
                     desktop_class.COMUtil.ReleaseCOMObjectScope(desktop_class.COMUtil.PInvokeProxyAPI, scopeID)
                     scopeID += 1
             except Exception:
                 pyaedt_logger.warning(
                     "Something went wrong releasing AEDT. Exception in `_main.COMUtil.ReleaseCOMObjectScope`."
                 )
-    if not settings.remote_rpc_session and not is_ironpython and close_desktop:
+    if not settings.remote_rpc_session and not is_ironpython and close_desktop:  # pragma: no cover
         timeout = 10
         while pid in active_sessions():
             time.sleep(1)
             timeout -= 1
             if timeout == 0:
                 try:
                     os.kill(pid, 9)
@@ -308,15 +308,15 @@
     ----------
     command : str
         Command to execute.
     bufsize : int, optional
         Buffer size. The default is ``None``.
 
     """
-    if bufsize:
+    if bufsize:  # pragma no cover
         return subprocess.call(command, bufsize=bufsize)
     else:
         return subprocess.call(command)
 
 
 def get_version_env_variable(version_id):
     """Get the environment variable for the AEDT version.
@@ -338,27 +338,27 @@
     'ANSYSEM_ROOT212'
 
     """
     version_env_var = "ANSYSEM_ROOT"
     values = version_id.split(".")
     version = int(values[0][2:])
     release = int(values[1])
-    if version < 20:
+    if version < 20:  # pragma no cover
         if release < 3:
             version += 1
         else:
             release += 2
     version_env_var += str(version) + str(release)
     return version_env_var
 
 
 def is_student_version(oDesktop):
     edt_root = os.path.normpath(oDesktop.GetExeDir())
     if is_windows and os.path.isdir(edt_root):
-        if any("ansysedtsv" in fn.lower() for fn in os.listdir(edt_root)):
+        if any("ansysedtsv" in fn.lower() for fn in os.listdir(edt_root)):  # pragma no cover
             return True
     return False
 
 
 def _init_desktop_from_design(*args, **kwargs):
     """Distinguishes if the ``Desktop`` class is initialized internally from the ``Design``
     class or directly from the user. For example, ``desktop=Desktop()``)."""
@@ -425,28 +425,31 @@
     """
 
     # _sessions = {}
     _invoked_from_design = False
 
     def __new__(cls, *args, **kwargs):
         # The following commented lines will be useful when we will need to search among multiple saved desktop.
-        # specified_version = kwargs.get("specified_version") or None if not args else args[0]
+        specified_version = kwargs.get("specified_version") or None if (not args or len(args) < 1) else args[0]
         new_desktop_session = kwargs.get("new_desktop_session") or False if (not args or len(args) < 3) else args[2]
         # student_version = kwargs.get("student_version") or False if (not args or len(args)<5) else args[4]
         # machine = kwargs.get("machine") or "" if (not args or len(args)<6) else args[5]
+        specified_version = get_string_version(specified_version)
         port = kwargs.get("port") or 0 if (not args or len(args) < 7) else args[6]
         aedt_process_id = kwargs.get("aedt_process_id") or None if (not args or len(args) < 8) else args[7]
         if settings.use_multi_desktop and not inside_desktop and new_desktop_session:
             pyaedt_logger.info("Initializing new Desktop session.")
             return object.__new__(cls)
         elif len(_desktop_sessions.keys()) > 0:
-            if settings.use_multi_desktop and (port or aedt_process_id):
+            if settings.use_multi_desktop and (port or aedt_process_id or specified_version):
                 for el in list(_desktop_sessions.values()):
-                    if (el.port != 0 and el.port == port) or (
-                        el.aedt_process_id and el.aedt_process_id == aedt_process_id
+                    if (
+                        (port != 0 and el.port == port)
+                        or (aedt_process_id and el.aedt_process_id == aedt_process_id)
+                        or (not port and not aedt_process_id and el.aedt_version_id == specified_version)
                     ):
                         return el
                 return object.__new__(cls)
             sessions = list(_desktop_sessions.keys())
             try:
                 process_id = _desktop_sessions[sessions[0]].odesktop.GetProcessID()
                 pyaedt_logger.info("Returning found Desktop session with PID {}!".format(process_id))
@@ -475,15 +478,15 @@
         if _desktop_sessions and specified_version is None:
             specified_version = list(_desktop_sessions.values())[-1].aedt_version_id
         if aedt_process_id:  # pragma no cover
             aedt_process_id = int(aedt_process_id)
         if getattr(self, "_initialized", None) is not None and self._initialized:
             try:
                 self.grpc_plugin.recreate_application(True)
-            except Exception:
+            except Exception:  # nosec
                 pass
             return
         else:
             self._initialized = True
         self._initialized_from_design = True if Desktop._invoked_from_design else False
         Desktop._invoked_from_design = False
         self.parent_desktop_id = []
@@ -491,26 +494,26 @@
         self._connected_app_instances = 0
 
         """Initialize desktop."""
         self.launched_by_pyaedt = False
 
         # Used in unit tests. The ``PYAEDT_NON_GRAPHICAL`` environment variable overrides
         # the ``non_graphical`` argument.
-        if os.getenv("PYAEDT_NON_GRAPHICAL", None) is not None:
+        if os.getenv("PYAEDT_NON_GRAPHICAL", None) is not None:  # pragma no cover
             non_graphical = os.getenv("PYAEDT_NON_GRAPHICAL", "false").lower() in ("true", "1", "t")
         # Used in Examples generation to force the desktop opening
-        if os.getenv("PYAEDT_DOC_GENERATION", "False").lower() in ("true", "1", "t"):
+        if os.getenv("PYAEDT_DOC_GENERATION", "False").lower() in ("true", "1", "t"):  # pragma no cover
             new_desktop_session = True
         # Used in toolkit scripts. The ``PYAEDT_SCRIPT_PROCESS_ID`` environment variable overrides
         # the ``aedt_process_id`` argument.
-        if os.getenv("PYAEDT_SCRIPT_PROCESS_ID", None):
+        if os.getenv("PYAEDT_SCRIPT_PROCESS_ID", None):  # pragma no cover
             aedt_process_id = int(os.getenv("PYAEDT_SCRIPT_PROCESS_ID"))
         # Used in toolkit scripts. The ``PYAEDT_SCRIPT_VERSION`` environment variable overrides
         # the ``specified_version`` argument.
-        if os.getenv("PYAEDT_SCRIPT_VERSION", None):
+        if os.getenv("PYAEDT_SCRIPT_VERSION", None):  # pragma no cover
             specified_version = str(os.getenv("PYAEDT_SCRIPT_VERSION"))
 
         self.close_on_exit = close_on_exit
         self.machine = machine
         self.port = port
         self.non_graphical = non_graphical
         self.is_grpc_api = None
@@ -565,52 +568,52 @@
                     starting_mode = "com"
             else:
                 raise ValueError(
                     "The version specified ({}) doesn't correspond to the pid specified ({})".format(
                         specified_version, aedt_process_id
                     )
                 )
-        elif float(version_key[0:6]) < 2022.2:
+        elif float(version_key[0:6]) < 2022.2:  # pragma no cover
             starting_mode = "com"
             if non_graphical:
                 self._logger.disable_desktop_log()
-        elif float(version_key[0:6]) == 2022.2:
+        elif float(version_key[0:6]) == 2022.2:  # pragma no cover
             if non_graphical:
                 self._logger.disable_desktop_log()
             if self.machine and self.port:
                 starting_mode = "grpc"  # if the machine and port is specified, user wants to use gRPC
             elif settings.use_grpc_api is None:
                 starting_mode = "com"  # default if user doesn't specify use_grpc_api
             else:
                 starting_mode = "grpc" if settings.use_grpc_api else "com"
         elif float(version_key[0:6]) > 2022.2:
-            if settings.use_grpc_api is None:
+            if settings.use_grpc_api is None:  # pragma no cover
                 starting_mode = "grpc"  # default if user doesn't specify use_grpc_api
             else:
                 starting_mode = "grpc" if settings.use_grpc_api else "com"
         else:  # pragma: no cover
             # it should not arrive here, it means that there is a starting case not covered by the decision tree
             raise Exception("Unsupported AEDT starting mode")
         # Starting AEDT
-        if "console" in starting_mode:
+        if "console" in starting_mode:  # pragma no cover
             # technically not a startup mode, we have just to load oDesktop
             self.odesktop = sys.modules["__main__"].oDesktop
             self.close_on_exit = False
             try:
                 self.non_graphical = self.odesktop.GetIsNonGraphical()
             except Exception:  # pragma: no cover
                 self.non_graphical = non_graphical
             self.is_grpc_api = False
 
         else:
             settings.aedt_version = version_key
-            if starting_mode == "ironpython":
+            if starting_mode == "ironpython":  # pragma no cover
                 self._logger.info("Launching PyAEDT outside AEDT with IronPython.")
                 self._init_ironpython(non_graphical, new_desktop_session, version)
-            elif starting_mode == "com":
+            elif starting_mode == "com":  # pragma no cover
                 self._logger.info("Launching PyAEDT outside AEDT with CPython and PythonNET.")
                 self._init_dotnet(
                     non_graphical,
                     new_desktop_session,
                     version,
                     student_version_flag,
                     version_key,
@@ -624,15 +627,15 @@
         settings.enable_desktop_logs = not self.non_graphical
         self._init_desktop()
         self._logger.info("pyaedt v%s", pyaedt_version)
         if not settings.remote_api:
             self._logger.info("Python version %s", sys.version)
 
         current_pid = int(self.odesktop.GetProcessID())
-        if aedt_process_id and not new_desktop_session and aedt_process_id != current_pid:
+        if aedt_process_id and not new_desktop_session and aedt_process_id != current_pid:  # pragma no cover
             raise Exception(
                 "AEDT started a new session instead of connecting to the session with pid: {}".format(aedt_process_id)
             )
         self.aedt_process_id = current_pid
 
         current_is_student = is_student_version(self.odesktop)
         if student_version ^ current_is_student:
@@ -643,25 +646,25 @@
             )
         self.student_version = current_is_student
 
         self.aedt_version_id = self.odesktop.GetVersion()[0:6]
 
         self._logger.info("AEDT %s Build Date %s", self.odesktop.GetVersion(), self.odesktop.GetBuildDateTimeString())
 
-        if is_ironpython:
+        if is_ironpython:  # pragma no cover
             sys.path.append(os.path.join(settings.aedt_install_dir, "common", "commonfiles", "IronPython", "DLLs"))
         if "GetGrpcServerPort" in dir(self.odesktop):
             self.port = self.odesktop.GetGrpcServerPort()
         # save the current desktop session in the database
         _desktop_sessions[self.aedt_process_id] = self
 
     def __enter__(self):
         return self
 
-    def __exit__(self, ex_type, ex_value, ex_traceback):
+    def __exit__(self, ex_type, ex_value, ex_traceback):  # pragma no cover
         # Write the trace stack to the log file if an exception occurred in the main script.
         if ex_type:
             err = self._exception(ex_value, ex_traceback)
         if self.close_on_exit or not is_ironpython:
             self.release_desktop(close_projects=self.close_on_exit, close_on_exit=self.close_on_exit)
 
     @pyaedt_function_handler()
@@ -687,15 +690,15 @@
             projectname = self.project_list()[project_design_name[0]]
         elif isinstance(project_design_name[0], str) and project_design_name[0] in self.project_list():
             projectname = project_design_name[0]
         else:
             return None
 
         initial_oproject = self.active_project()
-        if initial_oproject.GetName() != projectname:
+        if initial_oproject.GetName() != projectname:  # pragma no cover
             self.active_project(projectname)
 
         if isinstance(project_design_name[1], int) and project_design_name[1] < len(self.design_list()):
             designname = self.design_list()[project_design_name[1]]
         elif isinstance(project_design_name[1], str) and project_design_name[1] in self.design_list():
             designname = project_design_name[1]
         else:
@@ -841,15 +844,15 @@
                 version = "Ansoft.ElectronicsDesktop." + settings.remote_rpc_session.aedt_version[0:6]
                 return settings.remote_rpc_session.student_version, settings.remote_rpc_session.aedt_version, version
             except Exception:
                 return False, "", ""
 
         return student_version, specified_version, version
 
-    def _init_ironpython(self, non_graphical, new_aedt_session, version):
+    def _init_ironpython(self, non_graphical, new_aedt_session, version):  # pragma no cover
         from pyaedt.generic.clr_module import _clr
 
         base_path = settings.aedt_install_dir
         sys.path.append(base_path)
         sys.path.append(os.path.join(base_path, "PythonFiles", "DesktopPlugin"))
         _clr.AddReference("Ansys.Ansoft.CoreCOMScripting")
         AnsoftCOMUtil = __import__("Ansys.Ansoft.CoreCOMScripting")
@@ -863,22 +866,23 @@
         self.odesktop = oAnsoftApp.GetAppDesktop()
         self.isoutsideDesktop = True
         sys.path.append(os.path.join(base_path, "common", "commonfiles", "IronPython", "DLLs"))
         self.is_grpc_api = False
 
         return True
 
-    def _run_student(self):
+    @staticmethod
+    def _run_student():  # pragma: no cover
         DETACHED_PROCESS = 0x00000008
         pid = subprocess.Popen(
             [os.path.join(settings.aedt_install_dir, "ansysedtsv.exe")], creationflags=DETACHED_PROCESS
         ).pid
         time.sleep(5)
 
-    def _dispatch_win32(self, version):
+    def _dispatch_win32(self, version):  # pragma: no cover
         from pyaedt.generic.clr_module import win32_client
 
         o_ansoft_app = win32_client.Dispatch(version)
         self.odesktop = o_ansoft_app.GetAppDesktop()
         self.isoutsideDesktop = True
 
     def _init_dotnet(
@@ -957,15 +961,15 @@
         machine="",
         port=0,
         non_graphical=False,
         new_session=False,
         version=None,
         is_grpc=True,
     ):
-        if not is_grpc:
+        if not is_grpc:  # pragma: no cover
             from pyaedt.generic.clr_module import _clr
 
             _clr.AddReference("Ansys.Ansoft.CoreCOMScripting")
             AnsoftCOMUtil = __import__("Ansys.Ansoft.CoreCOMScripting")
             self.COMUtil = AnsoftCOMUtil.Ansoft.CoreCOMScripting.Util.COMUtil
             StandalonePyScriptWrapper = AnsoftCOMUtil.Ansoft.CoreCOMScripting.COM.StandalonePyScriptWrapper
             if non_graphical or new_session:
@@ -1012,15 +1016,15 @@
         """
         try:
             return self.grpc_plugin.odesktop
         except Exception:
             return self._odesktop
 
     @odesktop.setter
-    def odesktop(self, val):
+    def odesktop(self, val):  # pragma: no cover
         self._odesktop = val
 
     def _init_grpc(self, non_graphical, new_aedt_session, version, student_version, version_key):
         if settings.remote_rpc_session:  # pragma: no cover
             settings.remote_api = True
             if not self.machine:
                 try:
@@ -1035,18 +1039,18 @@
         if not self.machine or self.machine in [
             "localhost",
             "127.0.0.1",
             socket.getfqdn(),
             socket.getfqdn().split(".")[0],
         ]:
             self.machine = "127.0.0.1"
-        else:
+        else:  # pragma: no cover
             settings.remote_api = True
         if not self.port:
-            if self.machine and self.machine != "127.0.0.1":
+            if self.machine and self.machine != "127.0.0.1":  # pragma: no cover
                 self.logger.error("New session of AEDT cannot be started on remote machine from Desktop Class.")
                 self.logger.error("Either use port argument or start an rpc session to start AEDT on remote machine.")
                 self.logger.error("Use client = pyaedt.common_rpc.client(machinename) to start a remote session.")
                 self.logger.error("Use client.aedt(port) to start aedt on remote machine before connecting.")
             elif new_aedt_session:
                 self.port = _find_free_port()
                 self.logger.info("New AEDT session is starting on gRPC port %s", self.port)
@@ -1285,15 +1289,16 @@
                     return True
                 else:
                     oproject_target = self.active_project(target_project)
                     if not oproject_target:
                         oproject_target = self.odesktop.NewProject(target_project)
                         oproject_target.Paste()
                         return True
-        return False
+        else:  # pragma: no cover
+            return False
 
     @pyaedt_function_handler()
     def project_path(self, project_name=None):
         """Get the path to the project.
 
         Parameters
         ----------
@@ -1361,23 +1366,24 @@
         str
             Design type.
         """
         if not project_name:
             oproject = self.active_project()
         else:
             oproject = self.active_project(project_name)
-        if not oproject:
+        if not oproject:  # pragma: no cover
             return ""
         if not design_name:
             odesign = self.active_design(oproject)
         else:
             odesign = self.active_design(oproject, design_name)
         if odesign:
             return odesign.GetDesignType()
-        return ""
+        else:  # pragma: no cover
+            return ""
 
     @property
     def personallib(self):
         """PersonalLib directory.
 
         Returns
         -------
@@ -1431,15 +1437,15 @@
         -------
         str
            Full absolute path for the ``pyaedt`` directory.
 
         """
         return os.path.realpath(os.path.join(self.src_dir, ".."))
 
-    def _exception(self, ex_value, tb_data):
+    def _exception(self, ex_value, tb_data):  # pragma: no cover
         """Write the trace stack to AEDT when a Python error occurs.
 
         Parameters
         ----------
         ex_value : str
             Type of the exception.
         tb_data : str
@@ -1662,15 +1668,15 @@
             except Exception:
                 self.logger.warning("Error setting up Key %s.", key_full_name)
                 return False
         else:
             self.logger.warning("Key value must be an integer or string.")
             return False
 
-    def change_active_dso_config_name(self, product_name="HFSS", config_name="Local"):
+    def change_active_dso_config_name(self, product_name="HFSS", config_name="Local"):  # pragma: no cover
         """Change a specific registry key to a new value.
 
         Parameters
         ----------
         product_name : str, optional
             Name of the tool to apply the active configuration to. The default is
             ``"HFSS"``.
@@ -1687,15 +1693,15 @@
             self.change_registry_key("Desktop/ActiveDSOConfigurations/{}".format(product_name), config_name)
             self.logger.info("Configuration Changed correctly to %s for %s.", config_name, product_name)
             return True
         except Exception:
             self.logger.warning("Error Setting Up Configuration %s for %s.", config_name, product_name)
             return False
 
-    def change_registry_from_file(self, registry_file, make_active=True):
+    def change_registry_from_file(self, registry_file, make_active=True):  # pragma: no cover
         """Apply desktop registry settings from an ACF file.
 
         One way to get an ACF file is to export a configuration from the AEDT UI and then edit and reuse it.
 
         Parameters
         ----------
         registry_file : str
```

### Comparing `pyaedt-0.9.2/pyaedt/downloads.py` & `pyaedt-0.9.3/pyaedt/downloads.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Download example datasets from https://github.com/pyansys/example-data"""
+"""Download example datasets from https://github.com/ansys/example-data"""
 
 import os
 import shutil
 import tempfile
 import zipfile
 
 from pyaedt.generic.general_methods import is_ironpython
```

### Comparing `pyaedt-0.9.2/pyaedt/emit.py` & `pyaedt-0.9.3/pyaedt/emit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/emit_core/Couplings.py` & `pyaedt-0.9.3/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/emit_core/__init__.py` & `pyaedt-0.9.3/pyaedt/emit_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/emit_core/emit_constants.py` & `pyaedt-0.9.3/pyaedt/emit_core/emit_constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/emit_core/results/results.py` & `pyaedt-0.9.3/pyaedt/emit_core/results/results.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/emit_core/results/revision.py` & `pyaedt-0.9.3/pyaedt/emit_core/results/revision.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,15 @@
         if self.emit_project._aedt_version < "2024.1":  # pragma: no cover
             raise RuntimeError("This function only supported in AEDT version 2024.1 and later.")
         if self.revision_loaded:
             engine = self.emit_project._emit_api.get_engine()
             engine.n_to_1_limit = max_instances
 
     @pyaedt_function_handler()
-    def interference_type_classification(self, domain, use_filter=False, filter_list=None):
+    def interference_type_classification(self, domain, use_filter=False, filter_list=None):  # pragma: no cover
         """
         Classify interference type as according to inband/inband,
         out of band/in band, inband/out of band, and out of band/out of band.
 
         Parameters
         ----------
             domain :
@@ -546,15 +546,15 @@
         self,
         domain,
         global_protection_level=True,
         global_levels=None,
         protection_levels=None,
         use_filter=False,
         filter_list=None,
-    ):
+    ):  # pragma: no cover
         """
         Classify worst-case power at each Rx radio according to interference type.
 
         Options for interference type are `inband/inband, out of band/in band,
         inband/out of band, and out of band/out of band.
 
         Parameters
```

### Comparing `pyaedt-0.9.2/pyaedt/generic/Ansys.png` & `pyaedt-0.9.3/pyaedt/generic/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/AnsysTemplate.json` & `pyaedt-0.9.3/pyaedt/generic/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/DataHandlers.py` & `pyaedt-0.9.3/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.9.3/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/ami.json` & `pyaedt-0.9.3/pyaedt/generic/ami.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/clr_module.py` & `pyaedt-0.9.3/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/compliance.py` & `pyaedt-0.9.3/pyaedt/generic/compliance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/configurations.py` & `pyaedt-0.9.3/pyaedt/generic/configurations.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/constants.py` & `pyaedt-0.9.3/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/design_types.py` & `pyaedt-0.9.3/pyaedt/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/filesystem.py` & `pyaedt-0.9.3/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/general_methods.py` & `pyaedt-0.9.3/pyaedt/generic/general_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1506,15 +1506,15 @@
         elif window == "blackman":
             win = np.blackman(num_points)
     if win is not None:
         valueFFT = np.fft.fft(value * win, num_points)
     else:
         valueFFT = np.fft.fft(value, num_points)
     Npoints = int(len(valueFFT) / 2)
-    valueFFT = valueFFT[1 : Npoints + 1]
+    valueFFT = valueFFT[:Npoints]
     valueFFT = 2 * valueFFT / len(valueFFT)
     n = np.arange(num_points)
     freq = n / deltaT
     return freq, valueFFT
 
 
 @pyaedt_function_handler()
```

### Comparing `pyaedt-0.9.2/pyaedt/generic/grpc_plugin_dll_class.py` & `pyaedt-0.9.3/pyaedt/generic/grpc_plugin_dll_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         return "Instance of an Aedt object:" + str(self.objectID)
 
     def __Invoke__(self, funcName, argv):
         if settings.enable_debug_grpc_api_logger:
             settings.logger.debug("{} {}".format(funcName, argv))
         try:
             if settings.use_multi_desktop and funcName not in exclude_list:
-                self.dllapi.recreate_application(True if self.is_linux else False)
+                self.dllapi.recreate_application(True)
             ret = _retry_ntimes(
                 settings.number_of_grpc_api_retries,
                 self.dllapi.AedtAPI.InvokeAedtObjMethod,
                 self.objectID,
                 funcName,
                 argv,
             )  # Call C function
```

### Comparing `pyaedt-0.9.2/pyaedt/generic/ibis_reader.py` & `pyaedt-0.9.3/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/ibis_v7.json` & `pyaedt-0.9.3/pyaedt/generic/ibis_v7.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/near_field_import.py` & `pyaedt-0.9.3/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/pdf.py` & `pyaedt-0.9.3/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/plot.py` & `pyaedt-0.9.3/pyaedt/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/python_optimizers.py` & `pyaedt-0.9.3/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/report_file_parser.py` & `pyaedt-0.9.3/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/settings.py` & `pyaedt-0.9.3/pyaedt/generic/settings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/spisim.py` & `pyaedt-0.9.3/pyaedt/generic/spisim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.9.3/pyaedt/generic/touchstone_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/hfss.py` & `pyaedt-0.9.3/pyaedt/hfss.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/hfss3dlayout.py` & `pyaedt-0.9.3/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/icepak.py` & `pyaedt-0.9.3/pyaedt/icepak.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,54 +1,47 @@
 """This module contains the ``Icepak`` class."""
 
 from __future__ import absolute_import  # noreorder
 
 from collections import OrderedDict
 import csv
 import os
+import re
 import warnings
 
-from pyaedt import is_ironpython
+import pyaedt
 from pyaedt import is_linux
-from pyaedt.application.Design import DesignSettingsManipulation
-from pyaedt.generic.general_methods import GrpcApiError
-from pyaedt.modeler.cad.elements3d import FacePrimitive
-from pyaedt.modeler.geometry_operators import GeometryOperators as go
-from pyaedt.modules.SetupTemplates import SetupKeys
-
-if is_linux and is_ironpython:
-    import subprocessdotnet as subprocess
-else:
-    import subprocess
-
-import re
-
 from pyaedt.application.Analysis3D import FieldAnalysis3D
+from pyaedt.application.Design import DesignSettingsManipulation
 from pyaedt.generic.DataHandlers import _arg2dict
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.DataHandlers import random_string
 from pyaedt.generic.configurations import ConfigurationsIcepak
+from pyaedt.generic.general_methods import GrpcApiError
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.settings import settings
 from pyaedt.modeler.cad.components_3d import UserDefinedComponent
+from pyaedt.modeler.cad.elements3d import FacePrimitive
 from pyaedt.modeler.geometry_operators import GeometryOperators
+from pyaedt.modeler.geometry_operators import GeometryOperators as go
 from pyaedt.modules.Boundary import BoundaryDictionary
 from pyaedt.modules.Boundary import BoundaryObject
 from pyaedt.modules.Boundary import ExponentialDictionary
 from pyaedt.modules.Boundary import LinearDictionary
 from pyaedt.modules.Boundary import NativeComponentObject
 from pyaedt.modules.Boundary import NativeComponentPCB
 from pyaedt.modules.Boundary import NetworkObject
 from pyaedt.modules.Boundary import PieceWiseLinearDictionary
 from pyaedt.modules.Boundary import PowerLawDictionary
 from pyaedt.modules.Boundary import SinusoidalDictionary
 from pyaedt.modules.Boundary import SquareWaveDictionary
 from pyaedt.modules.Boundary import _create_boundary
+from pyaedt.modules.SetupTemplates import SetupKeys
 from pyaedt.modules.monitor_icepak import Monitor
 
 
 class Icepak(FieldAnalysis3D):
     """Provides the Icepak application interface.
 
     This class allows you to connect to an existing Icepak design or create a
@@ -2373,15 +2366,16 @@
             Coordinate system for the PCB. The default is ``"Global"``.
         rad : str, optional
             Radiating faces. The default is ``"Nothing"``.
         extent_type : str, optional
             Type of the extent. Options are ``"Bounding Box"`` and ``"Polygon"``.
             The default is ``"Bounding Box"``.
         outline_polygon : str, optional
-            Name of the polygon if ``extentype="Polygon"``. The default is ``""``.
+            Name of the polygon if ``extentype="Polygon"``. The default is ``""``,
+            in which case the outline polygon is automatically identified.
         powerin : str, optional
             Power to dissipate if cosimulation is disabled. The default is ``"0W"``.
         custom_x_resolution
             The default is ``None``.
         custom_y_resolution
             The default is ``None``.
 
@@ -2487,14 +2481,18 @@
             user_defined_component = UserDefinedComponent(
                 self.modeler, native.name, native_props["NativeComponentDefinitionProvider"], "PCB"
             )
             self.modeler.user_defined_components[native.name] = user_defined_component
             self.modeler.refresh_all_ids()
             self.materials._load_from_project()
             self._native_components.append(native)
+            if extent_type == "Polygon" and not outline_polygon:
+                outline_polygon = native.identify_extent_poly()
+                if outline_polygon:
+                    native.set_board_settings("Polygon", outline_polygon)
             return native
         return False
 
     @pyaedt_function_handler()
     def create_pcb_from_3dlayout(
         self,
             component_name,
@@ -2914,15 +2912,15 @@
         object_lists=None,
         meshtype="tetrahedral",
         min_size=None,
         max_size=None,
         inflation_layer_number=3,
         inflation_growth_rate=1.2,
         mesh_growth_rate=1.2,
-    ):
+    ):  # pragma: no cover
         """Generate a Fluent mesh for a list of selected objects and assign the mesh automatically to the objects.
 
         Parameters
         ----------
         object_lists : list, optional
             List of objects to compute the Fluent mesh on. The default is ``None``, in which case
             all fluids objects are used to compute the mesh.
@@ -3062,15 +3060,15 @@
         ]
         self.logger.info("Fluent is starting in Background with command line")
         if is_linux:
             fl_ucommand = ["bash"] + fl_ucommand + [fl_uscript_file_pointer]
         else:
             fl_ucommand = ["bash"] + fl_ucommand + ['"' + fl_uscript_file_pointer + '"']
         self.logger.info(" ".join(fl_ucommand))
-        subprocess.call(fl_ucommand)
+        pyaedt.desktop.run_process(fl_ucommand)
         if os.path.exists(mesh_file_pointer):
             self.logger.info("'" + mesh_file_pointer + "' has been created.")
             return self.mesh.assign_mesh_from_file(object_lists, mesh_file_pointer)
         self.logger.error("Failed to create msh file")
 
         return False
```

### Comparing `pyaedt-0.9.2/pyaedt/maxwell.py` & `pyaedt-0.9.3/pyaedt/maxwell.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/maxwellcircuit.py` & `pyaedt-0.9.3/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/mechanical.py` & `pyaedt-0.9.3/pyaedt/mechanical.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.9.3/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/amat.xml` & `pyaedt-0.9.3/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/ansys_cloud.areg` & `pyaedt-0.9.3/pyaedt/misc/ansys_cloud.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/config.schema.json` & `pyaedt-0.9.3/pyaedt/misc/config.schema.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/misc.py` & `pyaedt-0.9.3/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.9.3/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.9.3/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.9.3/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.9.3/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.9.3/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.9.3/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json` & `pyaedt-0.9.3/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/spisim_com_configuration_files/com_93_8.json` & `pyaedt-0.9.3/pyaedt/misc/spisim_com_configuration_files/com_93_8.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/spisim_com_configuration_files/com_94_17.json` & `pyaedt-0.9.3/pyaedt/misc/spisim_com_configuration_files/com_94_17.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/spisim_com_configuration_files/com_parameters.py` & `pyaedt-0.9.3/pyaedt/misc/spisim_com_configuration_files/com_parameters.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py` & `pyaedt-0.9.3/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/tb_nexxim_mapping.toml` & `pyaedt-0.9.3/pyaedt/misc/tb_nexxim_mapping.toml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/misc/template.acf` & `pyaedt-0.9.3/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.9.3/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.9.3/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.9.3/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.9.3/pyaedt/modeler/advanced_cad/parts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.9.3/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.9.3/pyaedt/modeler/cad/Modeler.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.9.3/pyaedt/modeler/cad/Primitives.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.9.3/pyaedt/modeler/cad/Primitives2D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.9.3/pyaedt/modeler/cad/Primitives3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/cad/component_array.py` & `pyaedt-0.9.3/pyaedt/modeler/cad/component_array.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.9.3/pyaedt/modeler/cad/components_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.9.3/pyaedt/modeler/cad/elements3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.9.3/pyaedt/modeler/cad/object3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.9.3/pyaedt/modeler/cad/polylines.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/calculators.py` & `pyaedt-0.9.3/pyaedt/modeler/calculators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.9.3/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.9.3/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.9.3/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.9.3/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.9.3/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.9.3/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.9.3/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/modeler2d.py` & `pyaedt-0.9.3/pyaedt/modeler/modeler2d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/modeler3d.py` & `pyaedt-0.9.3/pyaedt/modeler/modeler3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -873,86 +873,15 @@
                     and bounding_box[2] <= bound[5] <= bounding_box[5]
                 ):
                     objects.append(obj)
 
         return objects
 
     @pyaedt_function_handler()
-    def import_nastran(
-        self,
-        file_path,
-        import_lines=True,
-        lines_thickness=0,
-        import_as_light_weight=False,
-        decimation=0,
-        group_parts=True,
-        enable_planar_merge="True",
-    ):
-        """Import Nastran file into 3D Modeler by converting the faces to stl and reading it. The solids are
-        translated directly to AEDT format.
-
-        Parameters
-        ----------
-        file_path : str
-            Path to .nas file.
-        import_lines : bool, optional
-            Whether to import the lines or only triangles. Default is ``True``.
-        lines_thickness : float, optional
-            Whether to thicken lines after creation and it's default value.
-            Every line will be parametrized with a design variable called ``xsection_linename``.
-        import_as_light_weight : bool, optional
-            Import the stl generatated as light weight. It works only on SBR+ and HFSS Regions. Default is ``False``.
-        decimation : float, optional
-            Fraction of the original mesh to remove before creating the stl file.  If set to ``0.9``,
-            this function tries to reduce the data set to 10% of its
-            original size and removes 90% of the input triangles.
-        group_parts : bool, optional
-            Whether to group imported parts by object ID. The default is ``True``.
-        enable_planar_merge : str, optional
-            Whether to enable or not planar merge. It can be ``"True"``, ``"False"`` or ``"Auto"``.
-            ``"Auto"`` will disable the planar merge if stl contains more than 50000 triangles.
-
-        Returns
-        -------
-        List of :class:`pyaedt.modeler.Object3d.Object3d`
-        """
-        autosave = (
-            True if self._app.odesktop.GetRegistryInt("Desktop/Settings/ProjectOptions/DoAutoSave") == 1 else False
-        )
-        self._app.odesktop.EnableAutoSave(False)
-
-        def _write_solid_stl(triangle, pp):
-            try:
-                # points = [nas_to_dict["Points"][id] for id in triangle]
-                points = [pp[i] for i in triangle]
-            except KeyError:
-                return
-            fc = GeometryOperators.get_polygon_centroid(points)
-            v1 = points[0]
-            v2 = points[1]
-            cv1 = GeometryOperators.v_points(fc, v1)
-            cv2 = GeometryOperators.v_points(fc, v2)
-            if cv2[0] == cv1[0] == 0.0 and cv2[1] == cv1[1] == 0.0:
-                n = [0, 0, 1]
-            elif cv2[0] == cv1[0] == 0.0 and cv2[2] == cv1[2] == 0.0:
-                n = [0, 1, 0]
-            elif cv2[1] == cv1[1] == 0.0 and cv2[2] == cv1[2] == 0.0:
-                n = [1, 0, 0]
-            else:
-                n = GeometryOperators.v_cross(cv1, cv2)
-
-            normal = GeometryOperators.normalize_vector(n)
-            if normal:
-                f.write(" facet normal {} {} {}\n".format(normal[0], normal[1], normal[2]))
-                f.write("  outer loop\n")
-                f.write("   vertex {} {} {}\n".format(points[0][0], points[0][1], points[0][2]))
-                f.write("   vertex {} {} {}\n".format(points[1][0], points[1][1], points[1][2]))
-                f.write("   vertex {} {} {}\n".format(points[2][0], points[2][1], points[2][2]))
-                f.write("  endloop\n")
-                f.write(" endfacet\n")
+    def _parse_nastran(self, file_path):
 
         nas_to_dict = {"Points": [], "PointsId": {}, "Triangles": {}, "Lines": {}, "Solids": {}}
 
         self.logger.reset_timer()
         self.logger.info("Loading file")
         pid = 0
         with open_file(file_path, "r") as f:
@@ -1151,111 +1080,217 @@
                         )
                     else:
                         nas_to_dict["Lines"][obj_id] = [
                             [nas_to_dict["PointsId"][int(n1)], nas_to_dict["PointsId"][int(n2)]]
                         ]
 
         self.logger.info("File loaded")
-        objs_before = [i for i in self.object_names]
+        return nas_to_dict
 
-        if nas_to_dict["Triangles"] or nas_to_dict["Solids"] or nas_to_dict["Lines"]:
-            self.logger.info("Creating STL file with detected faces")
-            output_stl = ""
-            enable_stl_merge = False if enable_planar_merge == "False" or enable_planar_merge is False else True
-            if nas_to_dict["Triangles"]:
-                output_stl = os.path.join(self._app.working_directory, self._app.design_name + "_tria.stl")
-                f = open(output_stl, "w")
-
-            def decimate(points_in, faces_in, points_out, faces_out):
-                if 0 < decimation < 1:
-                    aggressivity = 3
-                    if 0.7 > decimation > 0.3:
-                        aggressivity = 5
-                    elif decimation >= 0.7:
-                        aggressivity = 7
-                    points_out, faces_out = fast_simplification.simplify(
-                        points_in, faces_in, decimation, agg=aggressivity
-                    )
+    @pyaedt_function_handler()
+    def _write_stl(self, nas_to_dict, decimation, enable_planar_merge):
+        def _write_solid_stl(triangle, pp):
+            try:
+                # points = [nas_to_dict["Points"][id] for id in triangle]
+                points = [pp[i] for i in triangle]
+            except KeyError:  # pragma: no cover
+                return
+            fc = GeometryOperators.get_polygon_centroid(points)
+            v1 = points[0]
+            v2 = points[1]
+            cv1 = GeometryOperators.v_points(fc, v1)
+            cv2 = GeometryOperators.v_points(fc, v2)
+            if cv2[0] == cv1[0] == 0.0 and cv2[1] == cv1[1] == 0.0:
+                n = [0, 0, 1]  # pragma: no cover
+            elif cv2[0] == cv1[0] == 0.0 and cv2[2] == cv1[2] == 0.0:
+                n = [0, 1, 0]  # pragma: no cover
+            elif cv2[1] == cv1[1] == 0.0 and cv2[2] == cv1[2] == 0.0:
+                n = [1, 0, 0]  # pragma: no cover
+            else:
+                n = GeometryOperators.v_cross(cv1, cv2)
 
-                return points_out, faces_out
+            normal = GeometryOperators.normalize_vector(n)
+            if normal:
+                f.write(" facet normal {} {} {}\n".format(normal[0], normal[1], normal[2]))
+                f.write("  outer loop\n")
+                f.write("   vertex {} {} {}\n".format(points[0][0], points[0][1], points[0][2]))
+                f.write("   vertex {} {} {}\n".format(points[1][0], points[1][1], points[1][2]))
+                f.write("   vertex {} {} {}\n".format(points[2][0], points[2][1], points[2][2]))
+                f.write("  endloop\n")
+                f.write(" endfacet\n")
+
+        self.logger.info("Creating STL file with detected faces")
+        enable_stl_merge = False if enable_planar_merge == "False" or enable_planar_merge is False else True
+        output_stl = os.path.join(self._app.working_directory, self._app.design_name + "_tria.stl")
+        f = open(output_stl, "w")
+
+        def decimate(points_in, faces_in, stl_id):
+            fin = [[3] + list(i) for i in faces_in]
+            mesh = pv.PolyData(points_in, faces=fin)
+            new_mesh = mesh.decimate_pro(decimation, preserve_topology=True, boundary_vertex_deletion=False)
+            points_out = list(new_mesh.points)
+            faces_out = [i[1:] for i in new_mesh.faces.reshape(-1, 4) if i[0] == 3]
+            self.logger.info(
+                "Final decimation on object {}: {}%".format(
+                    stl_id, 100 * (len(faces_in) - len(faces_out)) / len(faces_in)
+                )
+            )
+            return points_out, faces_out
+
+        for tri_id, triangles in nas_to_dict["Triangles"].items():
+            tri_out = triangles
+            p_out = nas_to_dict["Points"][::]
+            if decimation > 0 and len(triangles) > 20:
+                try:
+                    import pyvista as pv
+
+                    p_out, tri_out = decimate(nas_to_dict["Points"], tri_out, tri_id)
+                except Exception:
+                    self.logger.error("Package pyvista is needed to perform model simplification.")
+                    self.logger.error("Please install it using pip.")
+            f.write("solid Sheet_{}\n".format(tri_id))
+            if enable_planar_merge == "Auto" and len(tri_out) > 50000:
+                enable_stl_merge = False
+            for triangle in tri_out:
+                _write_solid_stl(triangle, p_out)
+            f.write("endsolid\n")
+
+        for solidid, solid_triangles in nas_to_dict["Solids"].items():
+            f.write("solid Solid_{}\n".format(solidid))
+            import pandas as pd
+
+            df = pd.Series(solid_triangles)
+            tri_out = df.drop_duplicates(keep=False).to_list()
+            p_out = nas_to_dict["Points"][::]
+            if decimation > 0 and len(solid_triangles) > 20:
+                try:
+
+                    import pyvista as pv
+
+                    p_out, tri_out = decimate(nas_to_dict["Points"], tri_out, solidid)
+                except Exception:
+                    self.logger.error("Package pyvista is needed to perform model simplification.")
+                    self.logger.error("Please install it using pip.")
+            if enable_planar_merge == "Auto" and len(tri_out) > 50000:
+                enable_stl_merge = False
+            for triangle in tri_out:
+                _write_solid_stl(triangle, p_out)
+            f.write("endsolid\n")
+        f.close()
+        self.logger.info("STL file created")
+        return output_stl, enable_stl_merge
+
+    @pyaedt_function_handler()
+    def import_nastran(
+        self,
+        file_path,
+        import_lines=True,
+        lines_thickness=0,
+        import_as_light_weight=False,
+        decimation=0,
+        group_parts=True,
+        enable_planar_merge="True",
+        save_only_stl=False,
+        preview=False,
+    ):
+        """Import Nastran file into 3D Modeler by converting the faces to stl and reading it. The solids are
+        translated directly to AEDT format.
 
-            for tri_id, triangles in nas_to_dict["Triangles"].items():
+        Parameters
+        ----------
+        file_path : str
+            Path to .nas file.
+        import_lines : bool, optional
+            Whether to import the lines or only triangles. Default is ``True``.
+        lines_thickness : float, optional
+            Whether to thicken lines after creation and it's default value.
+            Every line will be parametrized with a design variable called ``xsection_linename``.
+        import_as_light_weight : bool, optional
+            Import the stl generatated as light weight. It works only on SBR+ and HFSS Regions. Default is ``False``.
+        decimation : float, optional
+            Fraction of the original mesh to remove before creating the stl file.  If set to ``0.9``,
+            this function tries to reduce the data set to 10% of its
+            original size and removes 90% of the input triangles.
+        group_parts : bool, optional
+            Whether to group imported parts by object ID. The default is ``True``.
+        enable_planar_merge : str, optional
+            Whether to enable or not planar merge. It can be ``"True"``, ``"False"`` or ``"Auto"``.
+            ``"Auto"`` will disable the planar merge if stl contains more than 50000 triangles.
+        save_only_stl : bool, optional
+            Whether to import the model in HFSS or only generate the stl file.
+        preview : bool, optional
+            Whether to preview the model in pyvista or skip it.
+
+        Returns
+        -------
+        List of :class:`pyaedt.modeler.Object3d.Object3d`
+        """
+        autosave = (
+            True if self._app.odesktop.GetRegistryInt("Desktop/Settings/ProjectOptions/DoAutoSave") == 1 else False
+        )
+        self._app.odesktop.EnableAutoSave(False)
+
+        nas_to_dict = self._parse_nastran(file_path)
+
+        objs_before = [i for i in self.object_names]
+        if not (nas_to_dict["Triangles"] or nas_to_dict["Solids"] or nas_to_dict["Lines"]):
+            self.logger.error("Failed to import file. Check the model and retry")
+            return False
+        output_stl, enable_stl_merge = self._write_stl(nas_to_dict, decimation, enable_planar_merge)
+        if preview:
+            import pyvista as pv
+
+            pl = pv.Plotter(shape=(1, 2))
+            dargs = dict(show_edges=True, color=True)
+            p_out = nas_to_dict["Points"][::]
+            for triangles in nas_to_dict["Triangles"].values():
                 tri_out = triangles
-                p_out = nas_to_dict["Points"][::]
-                if decimation > 0 and len(triangles) > 20:
-                    try:
-                        import fast_simplification
-
-                        p_out, tri_out = decimate(nas_to_dict["Points"], tri_out, p_out, tri_out)
-                    except Exception:
-                        self.logger.error("Package fast-decimation is needed to perform model simplification.")
-                        self.logger.error("Please install it using pip.")
-                f.write("solid Sheet_{}\n".format(tri_id))
-                if enable_planar_merge == "Auto" and len(tri_out) > 50000:
-                    enable_stl_merge = False
-                for triangle in tri_out:
-                    _write_solid_stl(triangle, p_out)
-                f.write("endsolid\n")
-            if nas_to_dict["Triangles"]:
-                f.close()
-            output_solid = ""
-            enable_solid_merge = False if enable_planar_merge == "False" or enable_planar_merge is False else True
-            if nas_to_dict["Solids"]:
-                output_solid = os.path.join(self._app.working_directory, self._app.design_name + "_solids.stl")
-                f = open(output_solid, "w")
-            for solidid, solid_triangles in nas_to_dict["Solids"].items():
-                f.write("solid Solid_{}\n".format(solidid))
+                fin = [[3] + list(i) for i in tri_out]
+                pl.add_mesh(pv.PolyData(p_out, faces=fin), **dargs)
+            for triangles in nas_to_dict["Solids"].values():
                 import pandas as pd
 
-                df = pd.Series(solid_triangles)
+                df = pd.Series(triangles)
                 tri_out = df.drop_duplicates(keep=False).to_list()
                 p_out = nas_to_dict["Points"][::]
-                if decimation > 0 and len(solid_triangles) > 20:
-                    try:
-                        import fast_simplification
-
-                        p_out, tri_out = decimate(nas_to_dict["Points"], tri_out, p_out, tri_out)
-                    except Exception:
-                        self.logger.error("Package fast-decimation is needed to perform model simplification.")
-                        self.logger.error("Please install it using pip.")
-                if enable_planar_merge == "Auto" and len(tri_out) > 50000:
-                    enable_solid_merge = False
-                for triangle in tri_out:
-                    _write_solid_stl(triangle, p_out)
-                f.write("endsolid\n")
-            if output_solid:
-                f.close()
-            self.logger.info("STL file created")
-            self._app.odesktop.CloseAllWindows()
-            self.logger.info("Importing STL in 3D Modeler")
+                fin = [[3] + list(i) for i in tri_out]
+                pl.add_mesh(pv.PolyData(p_out, faces=fin), **dargs)
+            pl.add_text("Input mesh", font_size=24)
+            pl.reset_camera()
+            pl.subplot(0, 1)
             if output_stl:
-                self.import_3d_cad(
-                    output_stl,
-                    create_lightweigth_part=import_as_light_weight,
-                    healing=False,
-                    merge_planar_faces=enable_stl_merge,
-                )
-            if output_solid:
-                self.import_3d_cad(
-                    output_solid,
-                    create_lightweigth_part=import_as_light_weight,
-                    healing=False,
-                    merge_planar_faces=enable_solid_merge,
-                )
-            self.logger.info("Model imported")
-
-            if group_parts:
-                for el in nas_to_dict["Solids"].keys():
-                    obj_names = [i for i in self.object_names if i.startswith("Solid_{}".format(el))]
-                    self.create_group(obj_names, group_name=str(el))
-                objs = self.object_names[::]
-                for el in nas_to_dict["Triangles"].keys():
-                    obj_names = [i for i in objs if i == "Sheet_{}".format(el) or i.startswith("Sheet_{}_".format(el))]
-                    self.create_group(obj_names, group_name=str(el))
-                self.logger.info("Parts grouped")
+                pl.add_mesh(pv.read(output_stl), **dargs)
+            pl.add_text("Decimated mesh", font_size=24)
+            pl.reset_camera()
+            pl.link_views()
+            if "PYTEST_CURRENT_TEST" not in os.environ:
+                pl.show()
+        self.logger.info("STL files created in {}".format(output_stl))
+        if save_only_stl:
+            return output_stl
+
+        self._app.odesktop.CloseAllWindows()
+        self.logger.info("Importing STL in 3D Modeler")
+        if output_stl:
+            self.import_3d_cad(
+                output_stl,
+                create_lightweigth_part=import_as_light_weight,
+                healing=False,
+                merge_planar_faces=enable_stl_merge,
+            )
+        self.logger.info("Model imported")
+        if group_parts:
+            for el in nas_to_dict["Solids"].keys():
+                obj_names = [i for i in self.object_names if i.startswith("Solid_{}".format(el))]
+                self.create_group(obj_names, group_name=str(el))
+            objs = self.object_names[::]
+            for el in nas_to_dict["Triangles"].keys():
+                obj_names = [i for i in objs if i == "Sheet_{}".format(el) or i.startswith("Sheet_{}_".format(el))]
+                self.create_group(obj_names, group_name=str(el))
+            self.logger.info("Parts grouped")
 
         if import_lines and nas_to_dict["Lines"]:
             for line_name, lines in nas_to_dict["Lines"].items():
                 if lines_thickness:
                     self._app["x_section_{}".format(line_name)] = lines_thickness
                 polys = []
                 id = 0
```

### Comparing `pyaedt-0.9.2/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.9.3/pyaedt/modeler/modelerpcb.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.9.3/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.9.3/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modeler/schematic.py` & `pyaedt-0.9.3/pyaedt/modeler/schematic.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.9.3/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/Boundary.py` & `pyaedt-0.9.3/pyaedt/modules/Boundary.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from abc import abstractmethod
 from collections import OrderedDict
 import copy
 import re
 
+from pyaedt import Hfss3dLayout
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.DataHandlers import random_string
 from pyaedt.generic.constants import CATEGORIESQ3D
 from pyaedt.generic.general_methods import PropsManager
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.generic.general_methods import filter_tuple
@@ -326,14 +327,26 @@
             if el.component_name == self.component_name:
                 self._app._native_components.remove(el)
                 del self._app.modeler.user_defined_components[self.name]
                 self._app.modeler.cleanup_objects()
         return True
 
 
+def disable_auto_update(func):
+    def wrapper(self, *args, **kwargs):
+        auto_update = self.auto_update
+        self.auto_update = False
+        out = func(self, *args, **kwargs)
+        self.update()
+        self.auto_update = auto_update
+        return out
+
+    return wrapper
+
+
 class NativeComponentPCB(NativeComponentObject, object):
     """Manages Native Component PCB data and execution.
 
     Parameters
     ----------
     app : object
         AEDT application from the ``pyaedt.application`` class.
@@ -350,14 +363,341 @@
     >>> from pyaedt import Icepak
     >>> ipk = Icepak(solution_type="SBR+")
     >>> par_beam = ipk.create_ipk_3dcomponent_pcb()
     """
 
     def __init__(self, app, component_type, component_name, props):
         NativeComponentObject.__init__(self, app, component_type, component_name, props)
+        self._filter_map2name = {"Cap": "Capacitors", "Ind": "Inductors", "Res": "Resistors"}
+
+    @property
+    @pyaedt_function_handler()
+    def footprint_filter(self):
+        """Minimum component footprint for filtering."""
+        if self._app.settings.aedt_version < "2024.2":
+            return None
+        return self.filters.get("FootPrint", {}).get("Value", None)
+
+    @footprint_filter.setter
+    @pyaedt_function_handler()
+    @disable_auto_update
+    def footprint_filter(self, minimum_footprint):
+        """Set minimum component footprint for filtering.
+
+        Parameters
+        ----------
+        minimum_footprint : str
+            Value with unit of the minimum component footprint for filtering.
+        """
+        if self._app.settings.aedt_version < "2024.2":
+            return False
+        new_filters = self.props["NativeComponentDefinitionProvider"].get("Filters", [])
+        if "FootPrint" in new_filters:
+            new_filters.remove("FootPrint")
+        if minimum_footprint is not None:
+            new_filters.append("FootPrint")
+            self.props["NativeComponentDefinitionProvider"]["FootPrint"] = minimum_footprint
+        self.props["NativeComponentDefinitionProvider"]["Filters"] = new_filters
+
+    @property
+    @pyaedt_function_handler()
+    def power_filter(self):
+        """Minimum component power for filtering."""
+        return self.filters.get("Power", {}).get("Value")
+
+    @power_filter.setter
+    @pyaedt_function_handler()
+    @disable_auto_update
+    def power_filter(self, minimum_power):
+        """Set minimum component power for filtering.
+
+        Parameters
+        ----------
+        minimum_power : str
+            Value with unit of the minimum component power for filtering.
+        """
+        new_filters = self.props["NativeComponentDefinitionProvider"].get("Filters", [])
+        if "Power" in new_filters:
+            new_filters.remove("Power")
+        if minimum_power is not None:
+            new_filters.append("Power")
+            self.props["NativeComponentDefinitionProvider"]["PowerVal"] = minimum_power
+        self.props["NativeComponentDefinitionProvider"]["Filters"] = new_filters
+
+    @property
+    @pyaedt_function_handler()
+    def type_filters(self):
+        """Types of component that are filtered."""
+        return self.filters.get("Types")
+
+    @type_filters.setter
+    @pyaedt_function_handler()
+    @disable_auto_update
+    def type_filters(self, object_type):
+        """Set types of component to filter.
+
+        Parameters
+        ----------
+        object_type : str or list
+            Types of object to filter. Accepted types are ``"Capacitors"``, ``"Inductors"``, ``"Resistors"``.
+        """
+        if not isinstance(object_type, list):
+            object_type = [object_type]
+        if not all(o in self._filter_map2name.values() for o in object_type):
+            self._app.logger.error(
+                "Accepted elements of the list are: {}".format(", ".join(list(self._filter_map2name.values())))
+            )
+        else:
+            new_filters = self.props["NativeComponentDefinitionProvider"].get("Filters", [])
+            map2arg = {v: k for k, v in self._filter_map2name.items()}
+            for f in self._filter_map2name.keys():
+                if f in new_filters:
+                    new_filters.remove(f)
+            new_filters += [map2arg[o] for o in object_type]
+            self.props["NativeComponentDefinitionProvider"]["Filters"] = new_filters
+
+    @property
+    @pyaedt_function_handler()
+    def height_filter(self):
+        """Minimum component height for filtering."""
+        return self.filters.get("Height", {}).get("Value", None)
+
+    @height_filter.setter
+    @pyaedt_function_handler()
+    @disable_auto_update
+    def height_filter(self, minimum_height):
+        """Set minimum component height for filtering and whether to filter 2D objects.
+
+        Parameters
+        ----------
+        minimum_height : str
+            Value with unit of the minimum component power for filtering.
+        """
+        new_filters = self.props["NativeComponentDefinitionProvider"].get("Filters", [])
+        if "Height" in new_filters:
+            new_filters.remove("Height")
+        if minimum_height is not None:
+            new_filters.append("Height")
+            self.props["NativeComponentDefinitionProvider"]["HeightVal"] = minimum_height
+        self.props["NativeComponentDefinitionProvider"]["Filters"] = new_filters
+
+    @property
+    @pyaedt_function_handler()
+    def objects_2d_filter(self):
+        """Whether 2d objects are filtered."""
+        return self.filters.get("Exclude2DObjects", False)
+
+    @objects_2d_filter.setter
+    @pyaedt_function_handler()
+    @disable_auto_update
+    def objects_2d_filter(self, filter):
+        """Set whether 2d objects are filtered.
+
+        Parameters
+        ----------
+        filter : bool
+            Whether 2d objects are filtered
+        """
+        new_filters = self.props["NativeComponentDefinitionProvider"].get("Filters", [])
+        if "HeightExclude2D" in new_filters:
+            new_filters.remove("HeightExclude2D")
+        if filter:
+            new_filters.append("HeightExclude2D")
+        self.props["NativeComponentDefinitionProvider"]["Filters"] = new_filters
+
+    @property
+    @pyaedt_function_handler()
+    def filters(self):
+        """All active filters."""
+        out_filters = {"Type": {"Capacitors": False, "Inductors": False, "Resistors": False}}
+        filters = self.props["NativeComponentDefinitionProvider"].get("Filters", [])
+        filter_map2type = {
+            "Cap": "Type",
+            "FootPrint": "FootPrint",
+            "Height": "Height",
+            "HeightExclude2D": None,
+            "Ind": "Type",
+            "Power": "Power",
+            "Res": "Type",
+        }
+        filter_map2val = {"FootPrint": "FootPrint", "Height": "HeightVal", "Power": "PowerVal"}
+        for f in filters:
+            if filter_map2type[f] == "Type":
+                out_filters["Type"][self._filter_map2name[f]] = True
+            elif filter_map2type[f] is not None:
+                out_filters[f] = {"Value": filter_map2val[f]}
+        if "HeightExclude2D" in filters:
+            out_filters["Exclude2DObjects"] = True
+        return out_filters
+
+    @property
+    @pyaedt_function_handler()
+    def overridden_components(self):
+        """All overridden components."""
+        override_component = (
+            self.props["NativeComponentDefinitionProvider"].get("instanceOverridesMap", {}).get("oneOverrideBlk", [])
+        )
+        return {o["overrideName"]: o["overrideProps"] for o in override_component}
+
+    @pyaedt_function_handler()
+    @disable_auto_update
+    def override_component(
+        self, reference_designator, filter_component=False, power=None, r_jb=None, r_jc=None, height=None
+    ):
+        """Set component override.
+
+        Parameters
+        ----------
+        reference_designator : str
+            Reference designator of the part to override.
+        filter_component : bool, optional
+            Whether to filter out the component. Default is ``False``.
+        power : str, optional
+            Override component power. Default is ``None``, in which case the power is not overridden.
+        r_jb : str, optional
+            Override component r_jb value. Default is ``None``, in which case the resistance is not overridden.
+        r_jc : str, optional
+            Override component r_jc value. Default is ``None``, in which case the resistance is not overridden.
+        height : str, optional
+            Override component height value. Default is ``None``, in which case the height is not overridden.
+
+        Returns
+        -------
+        bool
+            ``True`` if successful. ``False`` otherwise.
+        """
+        override_component = (
+            self.props["NativeComponentDefinitionProvider"].get("instanceOverridesMap", {}).get("oneOverrideBlk", [])
+        )
+        for o in override_component:
+            if o["overrideName"] == reference_designator:
+                override_component.remove(o)
+        if filter_component or any(override_val is not None for override_val in [power, r_jb, r_jc, height]):
+            override_component.append(
+                OrderedDict(
+                    {
+                        "overrideName": reference_designator,
+                        "overrideProps": OrderedDict(
+                            {
+                                "isFiltered": filter_component,
+                                "isOverridePower": power is not None,
+                                "isOverrideThetaJb": r_jb is not None,
+                                "isOverrideThetaJc": r_jc is not None,
+                                "isOverrideHeight": height is not None,
+                                "powerOverride": power if power is not None else "nan",
+                                "thetaJbOverride": r_jb if r_jb is not None else "nan",
+                                "thetaJcOverride": r_jc if r_jc is not None else "nan",
+                            }
+                        ),
+                    }
+                )
+            )
+        self.props["NativeComponentDefinitionProvider"]["instanceOverridesMap"] = {"oneOverrideBlk": override_component}
+        return True
+
+    @pyaedt_function_handler()
+    @disable_auto_update
+    def set_parts(self, parts_choice, simplify_parts=False, surface_material="Steel-oxidised-surface"):
+        """Set how to include PCB parts.
+
+        Parameters
+        ----------
+        parts_choice : str
+            Parts to include: ``"None"``, ``"Device Parts"`` or ``"Package Parts"``.
+        simplify_parts : bool, optional
+            Whether to simplify parts as cuboid. Default is ``False``.
+        surface_material : str, optional
+            Surface material to apply to parts. Default is ``"Steel-oxidised-surface"``.
+
+        Returns
+        -------
+        bool
+            ``True`` if successful. ``False`` otherwise.
+        """
+        allowed_inputs = ["None", "Device Parts", "Package Parts"]
+        try:
+            parts_choice = allowed_inputs.index(parts_choice)
+        except ValueError:
+            self._app.logger.error(
+                "{} is not a valid argument, only allowed input are {}.".format(parts_choice, ", ".join(allowed_inputs))
+            )
+            return False
+        self.props["NativeComponentDefinitionProvider"]["PartsChoice"] = parts_choice
+        self.props["NativeComponentDefinitionProvider"]["ModelDeviceAsRect"] = simplify_parts
+        self.props["NativeComponentDefinitionProvider"]["DeviceSurfaceMaterial"] = surface_material
+        return True
+
+    @pyaedt_function_handler()
+    def identify_extent_poly(self):
+        prj = self.props["NativeComponentDefinitionProvider"]["DefnLink"]["Project"]
+        if prj == "This Project*":
+            prj = self._app.project_name
+        layout = Hfss3dLayout(
+            projectname=prj, designname=self.props["NativeComponentDefinitionProvider"]["DefnLink"]["Design"]
+        )
+        layer = [o for o in layout.modeler.stackup.drawing_layers if o.type == "outline"][0]
+        outlines = [p for p in layout.modeler.polygons.values() if p.placement_layer == layer.name]
+        if len(outlines) > 1:
+            self._app.logger.info(
+                "{} automatically selected as ``extent_polygon``, pass ``extent_polygon`` argument explixitly to select"
+                " a different one. Available choices are: {}".format(
+                    outlines[0].name, ", ".join([o.name for o in outlines])
+                )
+            )
+        elif len(outlines) == 0:
+            self._app.logger.error("No polygon found in the Outline layer.")
+            return False
+        return outlines[0].name
+
+    @pyaedt_function_handler()
+    @disable_auto_update
+    def set_board_settings(
+        self, extent_type=None, extent_polygon=None, board_cutouts_material="air", via_holes_material="air"
+    ):
+        """Set board extent and material settings.
+
+        Parameters
+        ----------
+        extent_type : str, optional
+            Extent definition of the PCB. Default is ``None`` in which case the 3D Layout extent
+            will be used. Other possible options are: ``"Bounding Box"`` or ``"Polygon"``.
+        extent_polygon : str, optional
+            Polygon name to use in the extent definition of the PCB. Default is ``None``. This
+            argument is mandatory if ``extent_type`` is ``"Polygon"``.
+        board_cutouts_material : str, optional
+            Material to apply to cutouts regions. Default is ``"air"``.
+        via_holes_material : str, optional
+            Material to apply to via holes regions. Default is ``"air"``.
+
+        Returns
+        -------
+        bool
+            ``True`` if successful. ``False`` otherwise.
+        """
+        if extent_type is None:
+            self.props["NativeComponentDefinitionProvider"]["Use3DLayoutExtents"] = True
+        else:
+            allowed_extent_types = ["Bounding Box", "Polygon"]
+            if extent_type not in allowed_extent_types:
+                self._app.logger.error(
+                    "Accepted argument for ``extent_type`` are: {}. {} provided".format(
+                        ", ".join(allowed_extent_types), extent_type
+                    )
+                )
+                return False
+            self.props["NativeComponentDefinitionProvider"]["ExtentsType"] = extent_type
+            if extent_type == "Polygon":
+                if extent_polygon is None:
+                    extent_polygon = self.identify_extent_poly()
+                    if not extent_polygon:
+                        return False
+                self.props["NativeComponentDefinitionProvider"]["OutlinePolygon"] = extent_polygon
+        self.props["NativeComponentDefinitionProvider"]["BoardCutoutMaterial"] = board_cutouts_material
+        self.props["NativeComponentDefinitionProvider"]["ViaHoleMaterial"] = via_holes_material
+        return True
 
 
 class BoundaryObject(BoundaryCommon, object):
     """Manages boundary data and execution.
 
     Parameters
     ----------
```

### Comparing `pyaedt-0.9.2/pyaedt/modules/CableModeling.py` & `pyaedt-0.9.3/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.9.3/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.9.3/pyaedt/modules/DesignXPloration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/LayerStackup.py` & `pyaedt-0.9.3/pyaedt/modules/LayerStackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/Material.py` & `pyaedt-0.9.3/pyaedt/modules/Material.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/MaterialLib.py` & `pyaedt-0.9.3/pyaedt/modules/MaterialLib.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/Mesh.py` & `pyaedt-0.9.3/pyaedt/modules/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.9.3/pyaedt/modules/Mesh3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.9.3/pyaedt/modules/MeshIcepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.9.3/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/PostProcessor.py` & `pyaedt-0.9.3/pyaedt/modules/PostProcessor.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.9.3/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/SolveSetup.py` & `pyaedt-0.9.3/pyaedt/modules/SolveSetup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.9.3/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.9.3/pyaedt/modules/monitor_icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/report_templates.py` & `pyaedt-0.9.3/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/modules/solutions.py` & `pyaedt-0.9.3/pyaedt/modules/solutions.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import json
 import logging
 import math
 import os
 import shutil
 import sys
 import time
-import warnings
 
 from pyaedt import is_ironpython
 from pyaedt import pyaedt_function_handler
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.constants import db10
 from pyaedt.generic.constants import db20
@@ -47,51 +46,51 @@
         pv = None
     try:
         import matplotlib.pyplot as plt
     except ImportError:
         plt = None
 
 
-def simplify_stl(input_file, output_file=None, decimation=0.5, aggressiveness=7):
+def simplify_stl(input_file, output_file=None, decimation=0.5, preview=False):
     """Import and simplify a stl file using pyvista and fast-simplification.
 
     Parameters
     ----------
     input_file : str
         Input stl file.
     output_file : str, optional
         Output stl file.
     decimation : float, optional
         Fraction of the original mesh to remove before creating the stl file.  If set to ``0.9``,
         this function will try to reduce the data set to 10% of its
         original size and will remove 90% of the input triangles.
-    aggressiveness : int, optional
-        Controls how aggressively to decimate the mesh.  A value of 10
-        will result in a fast decimation at the expense of mesh
-        quality and shape.  A value of 0 will attempt to preserve the
-        original mesh geometry at the expense of time.  Setting a low
-        value may result in being unable to reach the
-        ``decimation``.
 
     Returns
     -------
     str
         Full path to output stl.
     """
-    try:
-        import fast_simplification
-    except Exception:
-        warnings.warn("Package fast-decimation is needed to perform model simplification.")
-        warnings.warn("Please install it using pip.")
-        return False
     mesh = pv.read(input_file)
     if not output_file:
         output_file = os.path.splitext(input_file)[0] + "_output.stl"
-    simple = fast_simplification.simplify_mesh(mesh, target_reduction=decimation, agg=aggressiveness, verbose=True)
+    simple = mesh.decimate_pro(decimation, preserve_topology=True, boundary_vertex_deletion=False)
     simple.save(output_file)
+    if preview:
+        pl = pv.Plotter(shape=(1, 2))
+        dargs = dict(show_edges=True, color=True)
+        pl.add_mesh(mesh, **dargs)
+        pl.add_text("Input mesh", font_size=24)
+        pl.reset_camera()
+        pl.subplot(0, 1)
+        pl.add_mesh(simple, **dargs)
+        pl.add_text("Decimated mesh", font_size=24)
+        pl.reset_camera()
+        pl.link_views()
+        if "PYTEST_CURRENT_TEST" not in os.environ:
+            pl.show()
     return output_file
 
 
 class SolutionData(object):
     """Contains information from the :func:`GetSolutionDataPerVariation` method."""
 
     def __init__(self, aedtdata):
```

### Comparing `pyaedt-0.9.2/pyaedt/q3d.py` & `pyaedt-0.9.3/pyaedt/q3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1973,14 +1973,61 @@
         for arg_name, arg_value in kwargs.items():
             if setup[arg_name] is not None:
                 setup[arg_name] = arg_value
         setup.auto_update = True
         setup.update()
         return setup
 
+    @pyaedt_function_handler()
+    def assign_thin_conductor(self, assignment, material="copper", thickness=1, name=""):
+        """Assign a thin conductor to a sheet. The method accepts both a sheet name or a face id.
+        If a face it is provided, then a sheet will be created and the boundary assigned to it.
+
+        Parameters
+        ----------
+        assignment : str or int or :class:`pyaedt.modeler.cad.object3d.Object3d` or list
+            Object assignment.
+        material : str, optional
+            Material. Default is ``"copper"``.
+        thickness : float, str, optional
+            Conductor thickness. It can be as number of a string with units. Default is ``1``.
+        name : str, optional
+            Name of the boundary. Default is ``""``.
+
+        Returns
+        -------
+        :class:`pyaedt.modules.Boundary.BoundaryObject`
+            Source object.
+        """
+        assignment = self.modeler.convert_to_selections(assignment, True)
+        new_ass = []
+        for ass in assignment:
+            if isinstance(ass, int):
+                try:
+                    new_ass.append(self.modeler.create_object_from_face(ass)._m_name)
+                except Exception:  # pragma: no cover
+                    self.logger.error("Thin conductor can be applied only to sheet objects or faces.")
+            elif ass in self.modeler.sheet_names:
+                new_ass.append(ass)
+            else:
+                self.logger.error("Thin conductor can be applied only to sheet objects.")
+        if not new_ass:
+            return False
+        if not name:
+            name = generate_unique_name("Thin_Cond")
+        if isinstance(thickness, (float, int)):
+            thickness = str(thickness) + self.modeler.model_units
+        props = OrderedDict({"Objects": new_ass, "Material": material, "Thickness": thickness})
+
+        bound = BoundaryObject(self, name, props, "ThinConductor")
+        if bound.create():
+            self._boundaries[bound.name] = bound
+            return bound
+        return False  # pragma: no cover
+
 
 class Q2d(QExtractor, object):
     """Provides the Q2D app interface.
 
     This class allows you to create an instance of Q2D and link to an
     existing project or create a new one.
```

### Comparing `pyaedt-0.9.2/pyaedt/rmxprt.py` & `pyaedt-0.9.3/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.9.3/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.9.3/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.9.3/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.9.3/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.9.3/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.9.3/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.9.3/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.9.3/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.9.3/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.9.3/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.9.3/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.9.3/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.9.3/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.9.3/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/sbrplus/plot.py` & `pyaedt-0.9.3/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/twinbuilder.py` & `pyaedt-0.9.3/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/__init__.py` & `pyaedt-0.9.3/pyaedt/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/circuit/__init__.py` & `pyaedt-0.9.3/pyaedt/workflows/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/customize_automation_tab.py` & `pyaedt-0.9.3/pyaedt/workflows/customize_automation_tab.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     tab_config_file_path = os.path.join(lib_dir, product, "TabConfig.xml")
     if not os.path.isfile(tab_config_file_path) or overwrite:
         root = ET.Element("TabConfig")
     else:
         try:
             tree = ET.parse(tab_config_file_path)  # nosec
-        except ParseError as e:
+        except ParseError as e:  # pragma: no cover
             warnings.warn("Unable to parse %s\nError received = %s" % (tab_config_file_path, str(e)))
             return
         root = tree.getroot()
 
     panels = root.findall("./panel")
     if panels:
         panel_names = [panel_element.attrib["label"] for panel_element in panels]
@@ -103,15 +103,15 @@
             panel_element = [panel_element for panel_element in panels if panel_element.attrib["label"] == panel][0]
         else:
             panel_element = ET.SubElement(root, "panel", label=panel)
     else:
         panel_element = ET.SubElement(root, "panel", label=panel)
 
     buttons = panel_element.findall("./button")
-    if buttons:
+    if buttons:  # pragma: no cover
         button_names = [button.attrib["label"] for button in buttons]
         if name in button_names:
             # Remove previously existing PyAEDT panel and update with newer one.
             b = [button for button in buttons if button.attrib["label"] == name][0]
             panel_element.remove(b)
 
     if not icon_file:
@@ -141,65 +141,14 @@
     if os.path.isfile(tab_config_file_path):
         shutil.copy(tab_config_file_path, tab_config_file_path + ".orig")
 
     create_xml_tab(root, tab_config_file_path)
     return tab_config_file_path
 
 
-def remove_automation_tab(name, lib_dir, panel="Panel_PyAEDT_Extensions"):
-    """Remove automation tab in AEDT.
-
-    Parameters
-    ----------
-    name : str
-        Toolkit name.
-    lib_dir : str
-        Path to the library directory.
-    panel : str, optional
-        Panel name. The default is ``"Panel_PyAEDT_Extensions"``.
-
-    Returns
-    -------
-    float
-        Result of the dot product.
-
-    """
-
-    tab_config_file_path = os.path.join(lib_dir, "TabConfig.xml")
-    if not os.path.isfile(tab_config_file_path):
-        return True
-    try:
-        tree = ET.parse(tab_config_file_path)  # nosec
-    except ParseError as e:
-        warnings.warn("Unable to parse %s\nError received = %s" % (tab_config_file_path, str(e)))
-        return
-    root = tree.getroot()
-
-    panels = root.findall("./panel")
-    if panels:
-        panel_names = [panel_element.attrib["label"] for panel_element in panels]
-        if panel in panel_names:
-            # Remove previously existing PyAEDT panel and update with newer one.
-            panel_element = [panel_element for panel_element in panels if panel.attrib["label"] == panel][0]
-        else:
-            panel_element = ET.SubElement(root, "panel", label=panel)
-    else:
-        panel_element = ET.SubElement(root, "panel", label=panel)
-
-    buttons = panel_element.findall("./button")
-    if buttons:
-        button_names = [button.attrib["label"] for button in buttons]
-        if name in button_names:
-            # Remove previously existing PyAEDT panel and update with newer one.
-            b = [button for button in buttons if button.attrib["label"] == name][0]
-            panel_element.remove(b)
-
-    create_xml_tab(root, tab_config_file_path)
-
-
 def create_xml_tab(root, output_file):
     """Write the XML file to create the automation tab.
 
     Parameters
     ----------
     root : :class:xml.etree.ElementTree
         Root element of the main panel.
@@ -212,32 +161,32 @@
     with open(output_file, "w") as f:
         f.write(xml_str)
 
 
 def remove_xml_tab(toolkit_dir, name, panel="Panel_PyAEDT_Extensions"):
     """Remove a toolkit configuration file."""
     tab_config_file_path = os.path.join(toolkit_dir, "TabConfig.xml")
-    if not os.path.isfile(tab_config_file_path):
+    if not os.path.isfile(tab_config_file_path):  # pragma: no cover
         return True
     try:
         tree = ET.parse(tab_config_file_path)  # nosec
-    except ParseError as e:
+    except ParseError as e:  # pragma: no cover
         warnings.warn("Unable to parse %s\nError received = %s" % (tab_config_file_path, str(e)))
         return
     root = tree.getroot()
 
     panels = root.findall("./panel")
     if panels:
         panel_names = [panel_element.attrib["label"] for panel_element in panels]
         if panel in panel_names:
             # Remove previously existing PyAEDT panel and update with newer one.
             panel_element = [panel_element for panel_element in panels if panel_element.attrib["label"] == panel][0]
-        else:
+        else:  # pragma: no cover
             panel_element = ET.SubElement(root, "panel", label=panel)
-    else:
+    else:  # pragma: no cover
         panel_element = ET.SubElement(root, "panel", label=panel)
 
     buttons = panel_element.findall("./button")
     if buttons:
         button_names = [button.attrib["label"] for button in buttons]
         if name in button_names:
             # Remove previously existing PyAEDT panel and update with newer one.
@@ -319,50 +268,50 @@
     bool
 
     """
     logger = logging.getLogger("Global")
     if not personal_lib or not aedt_version:
         from pyaedt.generic.desktop_sessions import _desktop_sessions
 
-        if not _desktop_sessions:
+        if not _desktop_sessions:  # pragma: no cover
             logger.error("Personallib or AEDT version is not provided and there is no available desktop session.")
             return False
         d = list(_desktop_sessions.values())[0]
         personal_lib = d.personallib
         aedt_version = d.aedt_version_id
-    if script_file and not os.path.exists(script_file):
+    if script_file and not os.path.exists(script_file):  # pragma: no cover
         logger.error("Script does not exists.")
         return False
     toolkit_dir = os.path.join(personal_lib, "Toolkits")
     tool_map = __tab_map(product)
     file_name = name
-    if "/" in file_name:
+    if "/" in file_name:  # pragma: no cover
         file_name = file_name.replace("/", "_")
     tool_dir = os.path.join(toolkit_dir, tool_map, file_name)
     lib_dir = os.path.join(tool_dir, "Lib")
     toolkit_rel_lib_dir = os.path.relpath(lib_dir, tool_dir)
-    if is_linux and aedt_version <= "2023.1":
+    if is_linux and aedt_version <= "2023.1":  # pragma: no cover
         toolkit_rel_lib_dir = os.path.join("Lib", file_name)
         lib_dir = os.path.join(toolkit_dir, toolkit_rel_lib_dir)
         toolkit_rel_lib_dir = "../../" + toolkit_rel_lib_dir
     os.makedirs(lib_dir, exist_ok=True)
     os.makedirs(tool_dir, exist_ok=True)
     dest_script_path = None
     if script_file and copy_to_personal_lib:
         dest_script_path = os.path.join(lib_dir, os.path.split(script_file)[-1])
         shutil.copy2(script_file, dest_script_path)
 
     version_agnostic = True
-    if aedt_version[2:6].replace(".", "") in sys.executable:
+    if aedt_version[2:6].replace(".", "") in sys.executable:  # pragma: no cover
         executable_version_agnostic = sys.executable.replace(aedt_version[2:6].replace(".", ""), "%s")
         version_agnostic = False
     else:
         executable_version_agnostic = sys.executable
 
-    if executable_interpreter:
+    if executable_interpreter:  # pragma: no cover
         version_agnostic = True
         executable_version_agnostic = executable_interpreter
 
     templates_dir = os.path.dirname(pyaedt.workflows.templates.__file__)
 
     ipython_executable = executable_version_agnostic.replace("python" + __exe(), "ipython" + __exe())
     jupyter_executable = executable_version_agnostic.replace("python" + __exe(), "jupyter" + __exe())
```

### Comparing `pyaedt-0.9.2/pyaedt/workflows/emit/__init__.py` & `pyaedt-0.9.3/pyaedt/workflows/emit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/hfss/__init__.py` & `pyaedt-0.9.3/pyaedt/workflows/hfss/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/hfss/images/large/antenna.png` & `pyaedt-0.9.3/pyaedt/workflows/hfss/images/large/antenna.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/hfss/images/large/push.png` & `pyaedt-0.9.3/pyaedt/workflows/hfss/images/large/push.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/hfss3dlayout/__init__.py` & `pyaedt-0.9.3/pyaedt/workflows/hfss3dlayout/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/hfss3dlayout/images/large/cad3d.png` & `pyaedt-0.9.3/pyaedt/workflows/hfss3dlayout/images/large/cad3d.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/icepak/__init__.py` & `pyaedt-0.9.3/pyaedt/workflows/icepak/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/images/large/logo.png` & `pyaedt-0.9.3/pyaedt/workflows/images/large/logo.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/images/large/pyansys.png` & `pyaedt-0.9.3/pyaedt/workflows/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/installer/__init__.py` & `pyaedt-0.9.3/pyaedt/workflows/installer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/installer/console_setup.py` & `pyaedt-0.9.3/pyaedt/workflows/installer/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/installer/extension_manager.py` & `pyaedt-0.9.3/pyaedt/workflows/installer/extension_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         if install_action:
             desktop.logger.info("Install {}".format(name))
             if is_windows:
                 executable_interpreter = os.path.join(pyaedt_venv_dir, "Scripts", "python.exe")
             else:
                 executable_interpreter = os.path.join(pyaedt_venv_dir, "bin", "python")
             if not file:
-                file = os.path.join(os.path.dirname(pyaedt.workflows.templates.__file__), "toolkit_template.py")
+                file = os.path.join(os.path.dirname(pyaedt.workflows.templates.__file__), "extension_template.py")
             if os.path.isfile(executable_interpreter):
                 add_script_to_menu(
                     name=name,
                     script_file=file,
                     product=toolkit_level,
                     icon_file=icon,
                     executable_interpreter=executable_interpreter,
```

### Comparing `pyaedt-0.9.2/pyaedt/workflows/installer/images/large/console.png` & `pyaedt-0.9.3/pyaedt/workflows/installer/images/large/console.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/installer/images/large/extension_manager.png` & `pyaedt-0.9.3/pyaedt/workflows/installer/images/large/extension_manager.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/installer/images/large/jupyter.png` & `pyaedt-0.9.3/pyaedt/workflows/installer/images/large/jupyter.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/installer/images/large/run_script.png` & `pyaedt-0.9.3/pyaedt/workflows/installer/images/large/run_script.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/installer/jupyter_template.ipynb` & `pyaedt-0.9.3/pyaedt/workflows/installer/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/installer/pyaedt_installer.py` & `pyaedt-0.9.3/pyaedt/workflows/installer/pyaedt_installer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/maxwell2d/__init__.py` & `pyaedt-0.9.3/pyaedt/workflows/maxwell2d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/maxwell3d/__init__.py` & `pyaedt-0.9.3/pyaedt/workflows/maxwell3d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/maxwell3d/images/large/magnet_segmentation.png` & `pyaedt-0.9.3/pyaedt/workflows/maxwell3d/images/large/magnet_segmentation.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/mechanical/__init__.py` & `pyaedt-0.9.3/pyaedt/workflows/mechanical/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/project/__init__.py` & `pyaedt-0.9.3/pyaedt/workflows/project/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/project/images/large/cad3d.png` & `pyaedt-0.9.3/pyaedt/workflows/project/images/large/cad3d.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/project/images/large/pdf.png` & `pyaedt-0.9.3/pyaedt/workflows/project/images/large/pdf.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/q2d/__init__.py` & `pyaedt-0.9.3/pyaedt/workflows/q2d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/q3d/__init__.py` & `pyaedt-0.9.3/pyaedt/workflows/q3d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/templates/__init__.py` & `pyaedt-0.9.3/pyaedt/workflows/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/templates/jupyter.py_build` & `pyaedt-0.9.3/pyaedt/workflows/templates/jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/templates/pyaedt_console.py_build` & `pyaedt-0.9.3/pyaedt/workflows/templates/pyaedt_console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/templates/pyaedt_utils.py` & `pyaedt-0.9.3/pyaedt/workflows/templates/pyaedt_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/templates/run_extension_manager.py_build` & `pyaedt-0.9.3/pyaedt/workflows/templates/run_extension_manager.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/templates/run_pyaedt_script.py_build` & `pyaedt-0.9.3/pyaedt/workflows/templates/run_pyaedt_script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/templates/run_pyaedt_toolkit_script.py_build` & `pyaedt-0.9.3/pyaedt/workflows/templates/run_pyaedt_toolkit_script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyaedt/workflows/templates/toolkit_template.py` & `pyaedt-0.9.3/pyaedt/workflows/twinbuilder/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,30 +15,7 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
-# Toolkit template if the user does not pass any valid script in the toolkit manager
-
-import pyaedt
-from pyaedt import get_pyaedt_app
-from pyaedt.workflows.misc import get_aedt_version
-from pyaedt.workflows.misc import get_port
-from pyaedt.workflows.misc import get_process_id
-
-port = get_port()
-version = get_aedt_version()
-aedt_process_id = get_process_id()
-
-app = pyaedt.Desktop(new_desktop_session=False, specified_version=version, port=port, aedt_process_id=aedt_process_id)
-
-active_project = app.odesktop.GetActiveProject()
-active_design = active_project.GetActiveDesign()
-
-aedtapp = get_pyaedt_app(design_name=active_design.GetName(), desktop=app)
-
-# Your PyAEDT script
-
-app.release_desktop(False, False)
```

### Comparing `pyaedt-0.9.2/pyaedt/workflows/twinbuilder/images/large/export_to_circuit.png` & `pyaedt-0.9.3/pyaedt/workflows/twinbuilder/images/large/export_to_circuit.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.9.2/pyproject.toml` & `pyaedt-0.9.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     "openpyxl>=3.1.0,<3.3",
     "osmnx>=1.1.0,<1.10",
     "pandas>=1.1.0,<2.3",
     "pytest>=7.4.0,<8.3",
     "pytest-cov>=4.0.0,<5.1",
     "pytest-xdist>=3.5.0,<3.7",
     "pyvista>=0.38.0,<0.44",
-    "fast-simplification>=0.1.7",
     # Never directly imported but required when loading ML related file see #4713
     "scikit-learn>=1.0.0,<1.6",
     "scikit-rf>=0.30.0,<1.1",
     "SRTM.py",
     "utm",
     "vtk==9.2.6",
 ]
@@ -77,15 +76,14 @@
     "nbsphinx>=0.9.0,<0.10",
     "numpydoc>=1.5.0,<1.8",
     "openpyxl>=3.0.0,<3.2",
     "osmnx>=1.1.0,<1.10",
     "pypandoc>=1.10.0,<1.14",
     #"pytest-sphinx",
     "pyvista>=0.38.0,<0.44",
-    "fast-simplification>=0.1.7",
     "recommonmark",
     "scikit-rf>=0.30.0,<1.1",
     "Sphinx==5.3.0; python_version == '3.7'",
     "Sphinx>=7.1.0,<7.4; python_version > '3.7'",
     "sphinx-autobuild==2021.3.14; python_version == '3.7'",
     "sphinx-autobuild==2021.3.14; python_version == '3.8'",
     "sphinx-autobuild==2024.4.16; python_version > '3.8'",
@@ -129,14 +127,32 @@
     # Never directly imported but required when loading ML related file see #4713
     "scikit-learn>=1.0.0,<1.6",
     "scikit-rf>=0.30.0,<1.1",
     "SRTM.py",
     "utm",
     "vtk==9.2.6",
 ]
+installer = [
+    "imageio>=2.30.0,<2.35",
+    "matplotlib>=3.5.0,<3.9",
+    "numpy>=1.20.0,<2",
+    "openpyxl>=3.1.0,<3.3",
+    "osmnx>=1.1.0,<1.10",
+    "pandas>=1.1.0,<2.3",
+    "pyvista>=0.38.0,<0.44",
+    # Never directly imported but required when loading ML related file see #4713
+    "scikit-learn>=1.0.0,<1.6",
+    "scikit-rf>=0.30.0,<1.1",
+    "SRTM.py",
+    "utm",
+    "vtk==9.2.6",
+    "jupyterlab>=3.6.0,<4.3",
+    "ipython>=7.30.0,<8.25",
+    "ipyvtklink>=0.2.0,<0.2.4",
+]
 
 [tool.flit.module]
 name = "pyaedt"
 
 [project.urls]
 Bugs = "https://github.com/ansys/pyaedt/issues"
 Documentation = "https://aedt.docs.pyansys.com"
```

### Comparing `pyaedt-0.9.2/PKG-INFO` & `pyaedt-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.9.2
+Version: 0.9.3
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -44,15 +44,14 @@
 Requires-Dist: matplotlib>=3.5.0,<3.9 ; extra == "doc"
 Requires-Dist: nbsphinx>=0.9.0,<0.10 ; extra == "doc"
 Requires-Dist: numpydoc>=1.5.0,<1.8 ; extra == "doc"
 Requires-Dist: openpyxl>=3.0.0,<3.2 ; extra == "doc"
 Requires-Dist: osmnx>=1.1.0,<1.10 ; extra == "doc"
 Requires-Dist: pypandoc>=1.10.0,<1.14 ; extra == "doc"
 Requires-Dist: pyvista>=0.38.0,<0.44 ; extra == "doc"
-Requires-Dist: fast-simplification>=0.1.7 ; extra == "doc"
 Requires-Dist: recommonmark ; extra == "doc"
 Requires-Dist: scikit-rf>=0.30.0,<1.1 ; extra == "doc"
 Requires-Dist: Sphinx==5.3.0 ; extra == "doc" and ( python_version == '3.7')
 Requires-Dist: Sphinx>=7.1.0,<7.4 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc" and ( python_version == '3.7')
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc" and ( python_version == '3.8')
 Requires-Dist: sphinx-autobuild==2024.4.16 ; extra == "doc" and ( python_version > '3.8')
@@ -75,42 +74,57 @@
 Requires-Dist: sphinx-gallery>=0.14.0,<0.17 ; extra == "doc-no-examples"
 Requires-Dist: sphinx_design>=0.4.0,<0.7 ; extra == "doc-no-examples"
 Requires-Dist: ansys-pythonnet>=3.1.0rc3 ; extra == "dotnet"
 Requires-Dist: cffi==1.15.1 ; extra == "dotnet" and ( platform_system=='Linux' and python_version == '3.7')
 Requires-Dist: cffi>=1.16.0,<1.17 ; extra == "dotnet" and ( platform_system=='Linux' and python_version > '3.7')
 Requires-Dist: dotnetcore2==3.1.23 ; extra == "dotnet" and ( platform_system=='Linux')
 Requires-Dist: pywin32>=303 ; extra == "dotnet" and ( platform_system=='Windows')
+Requires-Dist: imageio>=2.30.0,<2.35 ; extra == "installer"
+Requires-Dist: matplotlib>=3.5.0,<3.9 ; extra == "installer"
+Requires-Dist: numpy>=1.20.0,<2 ; extra == "installer"
+Requires-Dist: openpyxl>=3.1.0,<3.3 ; extra == "installer"
+Requires-Dist: osmnx>=1.1.0,<1.10 ; extra == "installer"
+Requires-Dist: pandas>=1.1.0,<2.3 ; extra == "installer"
+Requires-Dist: pyvista>=0.38.0,<0.44 ; extra == "installer"
+Requires-Dist: scikit-learn>=1.0.0,<1.6 ; extra == "installer"
+Requires-Dist: scikit-rf>=0.30.0,<1.1 ; extra == "installer"
+Requires-Dist: SRTM.py ; extra == "installer"
+Requires-Dist: utm ; extra == "installer"
+Requires-Dist: vtk==9.2.6 ; extra == "installer"
+Requires-Dist: jupyterlab>=3.6.0,<4.3 ; extra == "installer"
+Requires-Dist: ipython>=7.30.0,<8.25 ; extra == "installer"
+Requires-Dist: ipyvtklink>=0.2.0,<0.2.4 ; extra == "installer"
 Requires-Dist: imageio>=2.30.0,<2.35 ; extra == "tests"
 Requires-Dist: ipython>=7.30.0,<8.25 ; extra == "tests"
 Requires-Dist: joblib>=1.0.0,<1.5 ; extra == "tests"
 Requires-Dist: matplotlib>=3.5.0,<3.9 ; extra == "tests"
 Requires-Dist: mock>=5.1.0,<5.2 ; extra == "tests"
 Requires-Dist: numpy>=1.20.0,<2 ; extra == "tests"
 Requires-Dist: openpyxl>=3.1.0,<3.3 ; extra == "tests"
 Requires-Dist: osmnx>=1.1.0,<1.10 ; extra == "tests"
 Requires-Dist: pandas>=1.1.0,<2.3 ; extra == "tests"
 Requires-Dist: pytest>=7.4.0,<8.3 ; extra == "tests"
 Requires-Dist: pytest-cov>=4.0.0,<5.1 ; extra == "tests"
 Requires-Dist: pytest-xdist>=3.5.0,<3.7 ; extra == "tests"
 Requires-Dist: pyvista>=0.38.0,<0.44 ; extra == "tests"
-Requires-Dist: fast-simplification>=0.1.7 ; extra == "tests"
 Requires-Dist: scikit-learn>=1.0.0,<1.6 ; extra == "tests"
 Requires-Dist: scikit-rf>=0.30.0,<1.1 ; extra == "tests"
 Requires-Dist: SRTM.py ; extra == "tests"
 Requires-Dist: utm ; extra == "tests"
 Requires-Dist: vtk==9.2.6 ; extra == "tests"
 Project-URL: Bugs, https://github.com/ansys/pyaedt/issues
 Project-URL: Discussions, https://github.com/ansys/pyaedt/discussions
 Project-URL: Documentation, https://aedt.docs.pyansys.com
 Project-URL: Releases, https://github.com/ansys/pyaedt/releases
 Project-URL: Source, https://github.com/ansys/pyaedt
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: doc-no-examples
 Provides-Extra: dotnet
+Provides-Extra: installer
 Provides-Extra: tests
 
 <!-- -->
 <a name="readme-top"></a>
 <!--
 *** PyAEDT README
 -->
```

