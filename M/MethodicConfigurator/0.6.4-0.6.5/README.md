# Comparing `tmp/methodicconfigurator-0.6.4.tar.gz` & `tmp/methodicconfigurator-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodicconfigurator-0.6.4.tar", last modified: Wed May 29 22:20:38 2024, max compression
+gzip compressed data, was "methodicconfigurator-0.6.5.tar", last modified: Sat Jun  1 15:36:26 2024, max compression
```

## Comparing `methodicconfigurator-0.6.4.tar` & `methodicconfigurator-0.6.5.tar`

### file list

```diff
@@ -1,315 +1,322 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.381293 methodicconfigurator-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.317293 methodicconfigurator-0.6.4/MethodicConfigurator/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/ArduPilot_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    26216 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/ArduPilot_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28737 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/annotate_params.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4997 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/ardupilot_methodic_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)    30690 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/backend_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/backend_filesystem_configuration_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/backend_filesystem_vehicle_components.py
--rw-r--r--   0 runner    (1001) docker     (127)    31001 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/backend_flightcontroller.py
--rw-r--r--   0 runner    (1001) docker     (127)    26774 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/backend_mavftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/battery_cell_voltages.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/common_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/extract_param_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18645 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_component_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_component_editor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14736 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_connection_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_directory_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    37652 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_parameter_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    27039 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2468 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/get_release_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/param_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/param_pid_adjustment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    22803 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/tempcal_imu.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/MethodicConfigurator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.381293 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-29 22:20:38.000000 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24202 2024-05-29 22:20:38.000000 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:20:38.000000 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-29 22:20:38.000000 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 22:20:38.000000 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 22:20:38.000000 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:20:31.000000 methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-29 22:20:38.381293 methodicconfigurator-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 22:20:38.381293 methodicconfigurator-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.309292 methodicconfigurator-0.6.4/vehicle_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.309292 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.337293 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/
--rw-r--r--   0 runner    (1001) docker     (127)    17325 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/12_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/13_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/14_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/15_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/16_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/17_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/18_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/19_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/20_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/21_ekf_config.param
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/22_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/23_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/24_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/25_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/26_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/27_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/28_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/29_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/30_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/31_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/32_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/33_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/34_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/35_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/36_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/37_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/38_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/39_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/40_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/41_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/42_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/43_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/44_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/45_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/46_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/47_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/48_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/49_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/50_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1998191 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)    77536 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/tempcal_acc.png
--rw-r--r--   0 runner    (1001) docker     (127)    78746 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/tempcal_gyro.png
--rw-r--r--   0 runner    (1001) docker     (127)  5007981 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/vehicle_components.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.313293 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.349293 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/14_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/16_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/19_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/20_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/21_ekf_config.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/25_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/26_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/27_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/28_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/30_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/32_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/33_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/34_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/35_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/36_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/37_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/38_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/49_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/50_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1476098 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.357293 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/14_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/16_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/17_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/18_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/19_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/20_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/21_ekf_config.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/23_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/25_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/26_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/27_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/28_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/30_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/32_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/33_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/34_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/35_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/36_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/37_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/38_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/49_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/50_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1599965 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.369293 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/14_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/15_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/16_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/17_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/18_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/19_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/20_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/21_ekf_config.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/23_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/24_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/25_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/26_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/27_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/28_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/29_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/30_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/31_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/32_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/33_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/34_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/35_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/36_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/37_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/38_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/40_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/41_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/43_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/44_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/45_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/46_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/49_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/50_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1966610 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:20:38.381293 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/04_board_orientation.param
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/06_telemetry.param
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/07_esc.param
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/08_batt1.param
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/10_gnss.param
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_mp_setup_mandatory_hardware.param
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_general_configuration.param
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/14_logging.param
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_motor.param
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_pid_adjustment.param
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/17_remote_id.param
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/19_notch_filter_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/20_throttle_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/21_ekf_config.param
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/23_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_inflight_magnetometer_fit_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/25_inflight_magnetometer_fit_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/26_quick_tune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/27_quick_tune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/28_evaluate_the_aircraft_tune_ff_disable.param
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_evaluate_the_aircraft_tune_ff_enable.param
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/30_autotune_roll_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_roll_results.param
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/32_autotune_pitch_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/33_autotune_pitch_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/34_autotune_yaw_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/35_autotune_yaw_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/36_autotune_yawd_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/37_autotune_yawd_results.param
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/38_autotune_roll_pitch_retune_setup.param
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_autotune_roll_pitch_retune_results.param
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_windspeed_estimation.param
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_barometer_compensation.param
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_roll.param
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_pitch.param
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_system_id_yaw.param
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_system_id_thrust.param
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_analytical_pid_optimization.param
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_everyday_use.param
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_position_controller.param
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/49_precision_land.param
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/50_guided_operation.param
--rw-r--r--   0 runner    (1001) docker     (127)  1982447 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml
--rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-29 22:20:13.000000 methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:36:26.197481 methodicconfigurator-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:36:26.129480 methodicconfigurator-0.6.5/MethodicConfigurator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/ArduPilot_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26216 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/ArduPilot_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29101 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/annotate_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/ardupilot_methodic_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32247 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/backend_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/backend_filesystem_configuration_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/backend_filesystem_vehicle_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/backend_flightcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11588 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/backend_flightcontroller_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26774 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/backend_mavftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/battery_cell_voltages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/common_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/extract_param_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/frontend_tkinter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22456 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/frontend_tkinter_component_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/frontend_tkinter_component_editor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14736 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/frontend_tkinter_connection_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22207 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/frontend_tkinter_directory_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/frontend_tkinter_flightcontroller_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38178 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/frontend_tkinter_parameter_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26538 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2468 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/get_release_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/param_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/param_pid_adjustment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22803 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/tempcal_imu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/MethodicConfigurator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:36:26.193481 methodicconfigurator-0.6.5/MethodicConfigurator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-06-01 15:36:26.000000 methodicconfigurator-0.6.5/MethodicConfigurator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24710 2024-06-01 15:36:26.000000 methodicconfigurator-0.6.5/MethodicConfigurator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 15:36:26.000000 methodicconfigurator-0.6.5/MethodicConfigurator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-06-01 15:36:26.000000 methodicconfigurator-0.6.5/MethodicConfigurator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-01 15:36:26.000000 methodicconfigurator-0.6.5/MethodicConfigurator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-01 15:36:26.000000 methodicconfigurator-0.6.5/MethodicConfigurator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 15:36:19.000000 methodicconfigurator-0.6.5/MethodicConfigurator.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-06-01 15:36:26.197481 methodicconfigurator-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 15:36:26.197481 methodicconfigurator-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:36:26.125480 methodicconfigurator-0.6.5/vehicle_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:36:26.125480 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:36:26.149480 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/
+-rw-r--r--   0 runner    (1001) docker     (127)    17325 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/11_initial_atc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/12_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/13_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/14_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/15_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/16_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/17_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/18_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/19_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/20_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/21_ekf_config.param
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/22_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/23_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/24_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/24_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/25_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/26_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/27_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/28_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/29_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/30_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/31_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/32_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/33_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/34_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/35_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/36_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/37_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/38_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/39_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/40_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/41_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/42_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/43_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/44_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/45_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/46_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/47_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/49_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/50_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1969521 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    77536 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/tempcal_acc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78746 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/tempcal_gyro.png
+-rw-r--r--   0 runner    (1001) docker     (127)  5007981 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:36:26.125480 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:36:26.157480 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/11_initial_atc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/14_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/16_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/19_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/20_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/21_ekf_config.param
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/25_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/26_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/27_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/28_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/30_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/32_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/33_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/34_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/35_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/36_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/37_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/38_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/49_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/50_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1476098 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:36:26.169480 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/11_initial_atc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/14_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/16_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/17_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/18_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/19_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/20_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/21_ekf_config.param
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/23_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/25_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/26_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/27_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/28_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/30_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/32_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/33_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/34_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/35_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/36_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/37_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/38_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/49_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/50_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1599965 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:36:26.181481 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    23067 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/11_initial_atc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/12_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/13_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/14_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/15_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/16_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/17_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/18_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/19_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/20_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/21_ekf_config.param
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/22_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/23_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/24_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/24_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/25_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/26_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/27_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/28_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/29_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/30_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/31_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/32_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/33_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/34_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/35_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/36_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/37_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/38_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/39_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/40_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/41_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/42_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/43_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/44_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/45_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/46_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/47_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/49_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/50_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1969521 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/vehicle_components.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:36:26.193481 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/04_board_orientation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/06_telemetry.param
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/07_esc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/08_batt1.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/10_gnss.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/11_initial_atc.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_mp_setup_mandatory_hardware.param
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_general_configuration.param
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/14_logging.param
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_motor.param
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_pid_adjustment.param
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/17_remote_id.param
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/19_notch_filter_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/20_throttle_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/21_ekf_config.param
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/23_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_inflight_magnetometer_fit_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_inflight_magnetometer_fit_setup.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/25_inflight_magnetometer_fit_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/26_quick_tune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/27_quick_tune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/28_evaluate_the_aircraft_tune_ff_disable.param
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_evaluate_the_aircraft_tune_ff_enable.param
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/30_autotune_roll_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_roll_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/32_autotune_pitch_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/33_autotune_pitch_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/34_autotune_yaw_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/35_autotune_yaw_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/36_autotune_yawd_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/37_autotune_yawd_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/38_autotune_roll_pitch_retune_setup.param
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_autotune_roll_pitch_retune_results.param
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_windspeed_estimation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_barometer_compensation.param
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_roll.param
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_pitch.param
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_system_id_yaw.param
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_system_id_thrust.param
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_analytical_pid_optimization.param
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_position_controller.param
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_guided_operation.param
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/49_precision_land.param
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/50_everyday_use.param
+-rw-r--r--   0 runner    (1001) docker     (127)  1982447 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   126547 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-06-01 15:36:01.000000 methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json
```

### Comparing `methodicconfigurator-0.6.4/LICENSE.md` & `methodicconfigurator-0.6.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/ArduPilot_icon.png` & `methodicconfigurator-0.6.5/MethodicConfigurator/ArduPilot_icon.png`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/ArduPilot_logo.png` & `methodicconfigurator-0.6.5/MethodicConfigurator/ArduPilot_logo.png`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/annotate_params.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/annotate_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,67 +107,74 @@
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, Par):
             return self.value == other.value and self.comment == other.comment
         return False
 
     @staticmethod
-    def load_param_file_into_dict(param_file: str) -> Dict[str, 'Par']:  # pylint: disable=R0912
+    def load_param_file_into_dict(param_file: str) -> Dict[str, 'Par']:
         """
         Loads an ArduPilot parameter file into a dictionary with name, value pairs.
 
         Parameters:
         parm_file (str): The name of the parameter file to load.
 
         Returns:
         dict: A dictionary containing the parameters from the file.
         """
         parameter_dict = {}
-        with open(param_file, encoding="utf-8") as f_handle:
-            for i, line in enumerate(f_handle, start=1):
-                original_line = line
-                line = line.strip()
-                comment = None
-                if not line:
-                    continue  # skip empty lines
-                if line[0] == "#":
-                    continue  # skip comments
-                if "#" in line:
-                    line, comment = line.split("#", 1)  # strip trailing comments
-                    comment = comment.strip()
-                if "," in line:
-                    # parse mission planner style parameter files
-                    parameter, value = line.split(",", 1)
-                elif " " in line:
-                    # parse mavproxy style parameter files
-                    parameter, value = line.split(" ", 1)
-                elif "\t" in line:
-                    parameter, value = line.split("\t", 1)
-                else:
-                    raise SystemExit(f"Missing parameter-value separator: {line} in {param_file} line {i}")
-                parameter = parameter.strip()
-                if len(parameter) > PARAM_NAME_MAX_LEN:
-                    raise SystemExit(f"Too long parameter name: {parameter} in {param_file} line {i}")
-                if not re.match(PARAM_NAME_REGEX, parameter):
-                    raise SystemExit(f"Invalid characters in parameter name {parameter} in {param_file} line {i}")
-                if parameter in parameter_dict:
-                    raise SystemExit(f"Duplicated parameter {parameter} in {param_file} line {i}")
-                try:
-                    fvalue = float(value.strip())
-                    parameter_dict[parameter] = Par(fvalue, comment)
-                except ValueError as exc:
-                    raise SystemExit(f"Invalid parameter value {value} in {param_file} line {i}") from exc
-                except IOError as exc:
-                    _exc_type, exc_value, exc_traceback = sys_exc_info()
-                    fname = os_path.split(exc_traceback.tb_frame.f_code.co_filename)[1]
-                    logging.critical("in line %s of file %s: %s", exc_traceback.tb_lineno, fname, exc_value)
-                    raise SystemExit(f"Caused by line {i} of file {param_file}: {original_line}") from exc
+        try:
+            with open(param_file, encoding="utf-8") as f_handle:
+                for i, line in enumerate(f_handle, start=1):
+                    original_line = line
+                    line = line.strip()
+                    comment = None
+                    if not line:
+                        continue  # skip empty lines
+                    if line[0] == "#":
+                        continue  # skip comments
+                    if "#" in line:
+                        line, comment = line.split("#", 1)  # strip trailing comments
+                        comment = comment.strip()
+                    if "," in line:
+                        # parse mission planner style parameter files
+                        parameter, value = line.split(",", 1)
+                    elif " " in line:
+                        # parse mavproxy style parameter files
+                        parameter, value = line.split(" ", 1)
+                    elif "\t" in line:
+                        parameter, value = line.split("\t", 1)
+                    else:
+                        raise SystemExit(f"Missing parameter-value separator: {line} in {param_file} line {i}")
+                    parameter = parameter.strip()
+                    Par.validate_parameter(param_file, parameter_dict, i, original_line, comment, parameter, value)
+        except UnicodeDecodeError as exp:
+            raise SystemExit(f"Fatal error reading {param_file}: {exp}") from exp
         return parameter_dict
 
     @staticmethod
+    def validate_parameter(param_file, parameter_dict, i, original_line, comment, parameter, value):  # pylint: disable=too-many-arguments
+        if len(parameter) > PARAM_NAME_MAX_LEN:
+            raise SystemExit(f"Too long parameter name: {parameter} in {param_file} line {i}")
+        if not re.match(PARAM_NAME_REGEX, parameter):
+            raise SystemExit(f"Invalid characters in parameter name {parameter} in {param_file} line {i}")
+        if parameter in parameter_dict:
+            raise SystemExit(f"Duplicated parameter {parameter} in {param_file} line {i}")
+        try:
+            fvalue = float(value.strip())
+            parameter_dict[parameter] = Par(fvalue, comment)
+        except ValueError as exc:
+            raise SystemExit(f"Invalid parameter value {value} in {param_file} line {i}") from exc
+        except IOError as exc:
+            _exc_type, exc_value, exc_traceback = sys_exc_info()
+            fname = os_path.split(exc_traceback.tb_frame.f_code.co_filename)[1]
+            logging.critical("in line %s of file %s: %s", exc_traceback.tb_lineno, fname, exc_value)
+            raise SystemExit(f"Caused by line {i} of file {param_file}: {original_line}") from exc
+
+    @staticmethod
     def missionplanner_sort(item: str) -> Tuple[str, ...]:
         """
         Sorts a parameter name according to the rules defined in the Mission Planner software.
 
         Args:
             item: The parameter name to sort.
 
@@ -206,15 +213,15 @@
         formatted_params = []
         if file_format == "missionplanner":
             for key, parameter in param_dict.items():
                 if parameter.comment:
                     formatted_params.append(f"{key},{format(parameter.value, '.6f').rstrip('0').rstrip('.')}"
                                             f"  # {parameter.comment}")
                 else:
-                    formatted_params.append(f"{key},{parameter.value}")
+                    formatted_params.append(f"{key},{format(parameter.value, '.6f').rstrip('0').rstrip('.')}")
         elif file_format == "mavproxy":
             for key, parameter in param_dict.items():
                 if parameter.comment:
                     formatted_params.append(f"{key:<16} {parameter.value:<8.6f}  # {parameter.comment}")
                 else:
                     formatted_params.append(f"{key:<16} {parameter.value:<8.6f}")
         return formatted_params
@@ -590,15 +597,15 @@
                 prefix_parts = [
                         f"{data['humanName']}",
                     ]
                 prefix_parts += data["documentation"]
                 for key, value in data["fields"].items():
                     prefix_parts.append(f"{key}: {value}")
                 prefix_parts += format_columns(data["values"])
-                doc_text = "\n# ".join(prefix_parts)  # pylint: disable=C0103
+                doc_text = "\n# ".join(prefix_parts)
                 if param_name in param_default_dict:
                     default_value = format(param_default_dict[param_name].value, '.6f').rstrip('0').rstrip('.')
                     doc_text += f"\n# Default: {default_value}"
                 if not is_first_param_in_file:
                     new_lines.append("\n")
                 new_lines.append(f"# {doc_text}\n{line}\n")
                 documented_params += 1
```

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/ardupilot_methodic_configurator.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/ardupilot_methodic_configurator.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,25 +7,29 @@
 
 SPDX-License-Identifier:    GPL-3
 '''
 
 import argparse
 from logging import basicConfig as logging_basicConfig
 from logging import getLevelName as logging_getLevelName
-# from logging import debug as logging_debug
+from logging import debug as logging_debug
 from logging import info as logging_info
 from logging import warning as logging_warning
 from logging import error as logging_error
 from sys import exit as sys_exit
 
 from MethodicConfigurator.backend_filesystem import LocalFilesystem
 from MethodicConfigurator.backend_flightcontroller import FlightController
 
+from MethodicConfigurator.frontend_tkinter_base import show_error_message
+
 from MethodicConfigurator.frontend_tkinter_connection_selection import ConnectionSelectionWindow
 
+from MethodicConfigurator.frontend_tkinter_flightcontroller_info import FlightControllerInfoWindow
+
 from MethodicConfigurator.frontend_tkinter_directory_selection import VehicleDirectorySelectionWindow
 
 from MethodicConfigurator.frontend_tkinter_component_editor import ComponentEditorWindow
 
 from MethodicConfigurator.frontend_tkinter_parameter_editor import ParameterEditorWindow
 
 from MethodicConfigurator.common_arguments import add_common_arguments_and_parse
@@ -54,15 +58,15 @@
                                      'The process gets repeated for each intermediate parameter file.')
     parser = FlightController.add_argparse_arguments(parser)
     parser = LocalFilesystem.add_argparse_arguments(parser)
     parser = ComponentEditorWindow.add_argparse_arguments(parser)
     return add_common_arguments_and_parse(parser)
 
 
-def main():
+def main():  # pylint: disable=too-many-branches
     args = argument_parser()
 
     logging_basicConfig(level=logging_getLevelName(args.loglevel), format='%(asctime)s - %(levelname)s - %(message)s')
 
     # Connect to the flight controller and read the parameters
     flight_controller = FlightController(args.reboot_time)
 
@@ -71,40 +75,63 @@
         if "No serial ports found" not in error_str:
             logging_error(error_str)
         conn_sel_window = ConnectionSelectionWindow(flight_controller, error_str)
         conn_sel_window.root.mainloop()
 
     vehicle_type = args.vehicle_type
     if vehicle_type == "":  # not explicitly set, to try to guess it
-        if flight_controller.vehicle_type is not None:
-            vehicle_type = flight_controller.vehicle_type
-            logging_info("Vehicle type not set explicitly, auto-detected %s.", vehicle_type)
+        if flight_controller.info.vehicle_type is not None:
+            vehicle_type = flight_controller.info.vehicle_type
+            logging_debug("Vehicle type not set explicitly, auto-detected %s.", vehicle_type)
     else:
         logging_info("Vehicle type explicitly set to %s.", vehicle_type)
 
     if vehicle_type == "": # did not guess it, default to ArduCopter
         vehicle_type = "ArduCopter"
         logging_warning("Could not detect vehicle type. Defaulting to ArduCopter.")
 
-    local_filesystem = LocalFilesystem(args.vehicle_dir, vehicle_type, args.allow_editing_template_files)
+    if flight_controller.master is not None:
+        FlightControllerInfoWindow(flight_controller)
+
+    try:
+        local_filesystem = LocalFilesystem(args.vehicle_dir, vehicle_type, args.allow_editing_template_files)
+    except SystemExit as exp:
+        show_error_message("Fatal error reading parameter files", f"{exp}")
+        raise
 
     # Get the list of intermediate parameter files files that will be processed sequentially
     files = list(local_filesystem.file_parameters.keys())
 
+    vehicle_dir_window = None
     if not files:
-        vehicle_dir_window = VehicleDirectorySelectionWindow(local_filesystem)
+        vehicle_dir_window = VehicleDirectorySelectionWindow(local_filesystem, flight_controller.master is not None)
         vehicle_dir_window.root.mainloop()
 
     start_file = local_filesystem.get_start_file(args.n)
 
+    component_editor_window = ComponentEditorWindow(VERSION, local_filesystem)
+    component_editor_window.set_vehicle_type_and_version(vehicle_type, flight_controller.info.flight_sw_version_and_type)
+    if vehicle_dir_window and \
+       vehicle_dir_window.created_new_vehicle_from_template and \
+       flight_controller.fc_parameters:
+        # copy vehicle parameters to component editor values
+        component_editor_window.set_values_from_fc_parameters(flight_controller.fc_parameters, local_filesystem.doc_dict)
     if not args.skip_component_editor:
-        component_editor_window = ComponentEditorWindow(VERSION, local_filesystem)
-        component_editor_window.set_vehicle_type_and_version(vehicle_type, flight_controller.version)
         component_editor_window.root.mainloop()
 
+    if vehicle_dir_window and \
+       vehicle_dir_window.created_new_vehicle_from_template and \
+       vehicle_dir_window.use_fc_params.get():
+        error_message = local_filesystem.copy_fc_params_values_to_template_created_vehicle_files(
+            flight_controller.fc_parameters)
+        if error_message:
+            logging_error(error_message)
+            show_error_message("Error in derived parameters", error_message)
+            sys_exit(1)
+
     # Call the GUI function with the starting intermediate parameter file
     ParameterEditorWindow(start_file, flight_controller, local_filesystem, VERSION)
 
     # Close the connection to the flight controller
     flight_controller.disconnect()
     sys_exit(0)
```

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/backend_filesystem.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/backend_filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -387,17 +387,22 @@
 
     def vehicle_image_filepath(self):
         return os_path.join(self.vehicle_dir, 'vehicle.jpg')
 
     def vehicle_image_exists(self):
         return os_path.exists(self.vehicle_image_filepath())
 
-    def new_vehicle_dir(self, base_dir: str, new_dir: str):
+    @staticmethod
+    def new_vehicle_dir(base_dir: str, new_dir: str):
         return os_path.join(base_dir, new_dir)
 
+    @staticmethod
+    def directory_exists(directory: str) -> bool:
+        return os_path.exists(directory)
+
     def create_new_vehicle_dir(self, new_vehicle_dir: str):
         # Check if the new vehicle directory already exists
         if os_path.exists(new_vehicle_dir):
             return "Directory already exists, choose a different one"
 
         try:
             # Create the new vehicle directory
@@ -557,15 +562,15 @@
         program_dir = current_dir
 
         if platform_system() == 'Windows':
             site_directory = LocalFilesystem.__site_config_dir()
         else:
             site_directory = program_dir
         template_default_dir = os_path.join(site_directory, "vehicle_templates", "ArduCopter",
-                                            "diatone_taycan_mxc", "4.5.1-params")
+                                            "diatone_taycan_mxc", "4.5.3-params")
         vehicles_default_dir = os_path.join(settings_directory, "vehicles")
         if not os_path.exists(vehicles_default_dir):
             os_makedirs(vehicles_default_dir, exist_ok=True)
 
         template_dir = settings["directory_selection"].get("template_dir", template_default_dir)
         new_base_dir = settings["directory_selection"].get("new_base_dir", vehicles_default_dir)
         vehicle_dir = settings["directory_selection"].get("vehicle_dir", vehicles_default_dir)
@@ -623,14 +628,40 @@
         start_file_index = last_uploaded_index + 1
         if start_file_index >= len(files):
             # Handle the case where last_uploaded_filename is the last file in the list
             logging_warning("Last uploaded file is the last file in the list. Starting from there.")
             start_file_index = len(files) - 1
         return files[start_file_index]
 
+    def get_eval_variables(self):
+        variables = {}
+        if hasattr(self, 'vehicle_components') and self.vehicle_components and \
+                'Components' in self.vehicle_components:
+            variables['vehicle_components'] = self.vehicle_components['Components']
+        if hasattr(self, 'doc_dict') and self.doc_dict:
+            variables['doc_dict'] = self.doc_dict
+        return variables
+
+    def copy_fc_params_values_to_template_created_vehicle_files(self, fc_parameters: Dict[str, 'Par']):
+        eval_variables = self.get_eval_variables()
+        for param_filename, param_dict in self.file_parameters.items():
+            for param_name, param in param_dict.items():
+                if param_name in fc_parameters:
+                    param.value = fc_parameters[param_name]
+            if self.configuration_steps and param_filename in self.configuration_steps:
+                step_dict = self.configuration_steps[param_filename]
+                error_msg = self.compute_parameters(param_filename, step_dict, 'forced', eval_variables)
+                if error_msg:
+                    return error_msg
+                error_msg = self.compute_parameters(param_filename, step_dict, 'derived', eval_variables)
+                if error_msg:
+                    return error_msg
+            Par.export_to_param(Par.format_params(param_dict), os_path.join(self.vehicle_dir, param_filename))
+        return ''
+
     @staticmethod
     def supported_vehicles():
         return ['AP_Periph', 'AntennaTracker', 'ArduCopter', 'ArduPlane',
                                     'ArduSub', 'Blimp', 'Heli', 'Rover', 'SITL']
 
     @staticmethod
     def add_argparse_arguments(parser):
```

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/backend_filesystem_configuration_steps.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/backend_filesystem_configuration_steps.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/backend_filesystem_vehicle_components.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/backend_filesystem_vehicle_components.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/backend_mavftp.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/backend_mavftp.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/battery_cell_voltages.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/battery_cell_voltages.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/common_arguments.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/common_arguments.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/extract_param_defaults.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/extract_param_defaults.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_base.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/frontend_tkinter_base.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_component_editor.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/frontend_tkinter_component_editor.py`

 * *Files 24% similar despite different names*

```diff
@@ -74,28 +74,78 @@
             self.data['Components'] = {}
         if 'Battery' not in self.data['Components']:
             self.data['Components']['Battery'] = {}
         if 'Specifications' not in self.data['Components']['Battery']:
             self.data['Components']['Battery']['Specifications'] = {}
         if 'Chemistry' not in self.data['Components']['Battery']['Specifications']:
             self.data['Components']['Battery']['Specifications']['Chemistry'] = "Lipo"
+        if 'Capacity mAh' not in self.data['Components']['Battery']['Specifications']:
+            self.data['Components']['Battery']['Specifications']['Capacity mAh'] = 0
+        if 'Frame' not in self.data['Components']:
+            self.data['Components']['Frame'] = {}
+        if 'Specifications' not in self.data['Components']['Frame']:
+            self.data['Components']['Frame']['Specifications'] = {}
+        if 'TOW min Kg' not in self.data['Components']['Frame']['Specifications']:
+            self.data['Components']['Frame']['Specifications']['TOW min Kg'] = 1
+        if 'TOW max Kg' not in self.data['Components']['Frame']['Specifications']:
+            self.data['Components']['Frame']['Specifications']['TOW max Kg'] = 1
 
     def set_vehicle_type_and_version(self, vehicle_type: str, version: str):
         self.data['Components']['Flight Controller']['Firmware']['Type'] = vehicle_type
         entry = self.entry_widgets[('Flight Controller', 'Firmware', 'Type')]
         entry.delete(0, tk.END)
         entry.insert(0, vehicle_type)
         entry.config(state="disabled")
         if version:
             self.data['Components']['Flight Controller']['Firmware']['Version'] = version
             entry = self.entry_widgets[('Flight Controller', 'Firmware', 'Version')]
             entry.delete(0, tk.END)
             entry.insert(0, version)
             entry.config(state="disabled")
 
+    @staticmethod
+    def reverse_key_search(doc: dict, param_name: str, values: list) -> list:
+        return [key for key, value in doc[param_name]["values"].items() if value in values]
+
+    def set_values_from_fc_parameters(self, fc_parameters: dict, doc: dict):
+        serial_ports = ["SERIAL1", "SERIAL2", "SERIAL3", "SERIAL4", "SERIAL5", "SERIAL6", "SERIAL7", "SERIAL8"]
+        #can_ports = ["CAN1", "CAN2"]
+        #i2c_ports = ["I2C1", "I2C2", "I2C3", "I2C4"]
+
+        rc_receiver_protocols = self.reverse_key_search(doc, "SERIAL1_PROTOCOL", ["RC Input"])
+        telemetry_protocols = self.reverse_key_search(doc, "SERIAL1_PROTOCOL",
+                                                      ["MAVLink1", "MAVLink2", "MAVLink High Latency"])
+        gnss_protocols = self.reverse_key_search(doc, "SERIAL1_PROTOCOL", ["GPS"])
+        esc_protocols = self.reverse_key_search(doc, "SERIAL1_PROTOCOL", ["ESC Telemetry", "FETtecOneWire", "CoDevESC"])
+        for serial in serial_ports:
+            if serial + "_PROTOCOL" in fc_parameters:
+                if fc_parameters[serial + "_PROTOCOL"] in rc_receiver_protocols:
+                    self.data['Components']['RC Receiver']['FC Connection']['Type'] = serial
+                    #self.data['Components']['RC Receiver']['FC Connection']['Protocol'] = \
+                    # doc['RC_PROTOCOLS']['values'][fc_parameters['RC_PROTOCOLS']]
+                elif fc_parameters[serial + "_PROTOCOL"] in telemetry_protocols:
+                    self.data['Components']['Telemetry']['FC Connection']['Type'] = serial
+                    self.data['Components']['Telemetry']['FC Connection']['Protocol'] = \
+                        doc[serial + "_PROTOCOL"]['values'][str(fc_parameters[serial + "_PROTOCOL"]).rstrip('0').rstrip('.')]
+                elif fc_parameters[serial + "_PROTOCOL"] in gnss_protocols:
+                    self.data['Components']['GNSS Receiver']['FC Connection']['Type'] = serial
+                    self.data['Components']['GNSS Receiver']['FC Connection']['Protocol'] = \
+                        doc['GPS_TYPE']['values'][str(fc_parameters['GPS_TYPE']).rstrip('0').rstrip('.')]
+                elif fc_parameters[serial + "_PROTOCOL"] in esc_protocols:
+                    self.data['Components']['ESC']['FC Connection']['Type'] = serial
+                    self.data['Components']['ESC']['FC Connection']['Protocol'] = \
+                        doc['MOT_PWM_TYPE']['values'][str(fc_parameters['MOT_PWM_TYPE']).rstrip('0').rstrip('.')]
+        if "BATT_MONITOR" in fc_parameters:
+            analog = [key for key, value in doc["BATT_MONITOR"]["values"].items() \
+                      if value in ['Analog Voltage Only', 'Analog Voltage and Current']]
+            if fc_parameters["BATT_MONITOR"] in analog:
+                self.data['Components']['Battery Monitor']['FC Connection']['Type'] = "Analog"
+            self.data['Components']['Battery Monitor']['FC Connection']['Protocol'] = \
+                doc['BATT_MONITOR']['values'][str(fc_parameters["BATT_MONITOR"]).rstrip('0').rstrip('.')]
+
     def add_entry_or_combobox(self, value, entry_frame, path):
         serial_ports = ["SERIAL1", "SERIAL2", "SERIAL3", "SERIAL4", "SERIAL5", "SERIAL6", "SERIAL7", "SERIAL8"]
         can_ports = ["CAN1", "CAN2"]
         i2c_ports = ["I2C1", "I2C2", "I2C3", "I2C4"]
 
         combobox_config = {
             ('Flight Controller', 'Firmware', 'Type'): {
```

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_component_editor_base.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/frontend_tkinter_component_editor_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     contain vehicle component configurations. It inherits from the BaseWindow
     class, which provides basic window functionality.
     """
     def __init__(self, version, local_filesystem: LocalFilesystem=None):
         super().__init__()
         self.local_filesystem = local_filesystem
 
-        self.root.title("Amilcar Lucas's - ArduPilot methodic configurator - " + version + " - Vehicle Component Editor")
+        self.root.title("Amilcar Lucas's - ArduPilot methodic configurator " + version + " - Vehicle Component Editor")
         self.root.geometry("880x600") # Set the window width
 
         self.data = local_filesystem.load_vehicle_components_json_data(local_filesystem.vehicle_dir)
         if len(self.data) < 1:
             # Schedule the window to be destroyed after the mainloop has started
             self.root.after(100, self.root.destroy) # Adjust the delay as needed
             return
```

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_connection_selection.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/frontend_tkinter_connection_selection.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_directory_selection.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/frontend_tkinter_directory_selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,22 +17,25 @@
 
 from logging import basicConfig as logging_basicConfig
 from logging import getLevelName as logging_getLevelName
 from logging import warning as logging_warning
 from logging import debug as logging_error
 
 import tkinter as tk
+from tkinter import messagebox
 from tkinter import ttk
 from tkinter import filedialog
+from tkinter import Checkbutton
+
+from MethodicConfigurator.version import VERSION
 
 from MethodicConfigurator.common_arguments import add_common_arguments_and_parse
 
 from MethodicConfigurator.backend_filesystem import LocalFilesystem
 
-from MethodicConfigurator.frontend_tkinter_base import show_error_message
 from MethodicConfigurator.frontend_tkinter_base import show_no_param_files_error
 from MethodicConfigurator.frontend_tkinter_base import show_tooltip
 from MethodicConfigurator.frontend_tkinter_base import BaseWindow
 
 
 class DirectorySelectionWidgets():
     """
@@ -147,20 +150,26 @@
         self.local_filesystem = local_filesystem
         self.destroy_parent_on_open = destroy_parent_on_open
 
     def on_select_directory(self):
         # Call the base class method to open the directory selection dialog
         if super().on_select_directory():
             if "vehicle_templates" in self.directory and not self.local_filesystem.allow_editing_template_files:
-                show_error_message("Invalid Vehicle Directory Selected",
-                                   "Please do not edit the files provided 'vehicle_templates' directory\n"
-                                   "as those are used as a template for new vehicles")
+                messagebox.showerror("Invalid Vehicle Directory Selected",
+                                     "Please do not edit the files provided 'vehicle_templates' directory\n"
+                                     "as those are used as a template for new vehicles")
                 return
             self.local_filesystem.vehicle_dir = self.directory
-            self.local_filesystem.re_init(self.directory, self.local_filesystem.vehicle_type)
+
+            try:
+                self.local_filesystem.re_init(self.directory, self.local_filesystem.vehicle_type)
+            except SystemExit as exp:
+                messagebox.showerror("Fatal error reading parameter files", f"{exp}")
+                raise
+
             files = list(self.local_filesystem.file_parameters.keys())
             if files:
                 LocalFilesystem.store_recently_used_vehicle_dir(self.directory)
                 if hasattr(self.parent, 'file_selection_combobox'):
                     # Update the file selection combobox with the new files
                     self.parent.file_selection_combobox.set_entries_tupple(files, files[0])
                     # Trigger the combobox change event to update the table
@@ -178,55 +187,70 @@
 
     This class extends the BaseWindow class to provide a graphical user interface
     for selecting a vehicle directory that contains intermediate parameter files
     for ArduPilot. It allows the user to choose between creating a new vehicle
     configuration directory based on an existing template or using an existing
     vehicle configuration directory.
     """
-    def __init__(self, local_filesystem: LocalFilesystem):
+    def __init__(self, local_filesystem: LocalFilesystem, fc_connected: bool = False):
         super().__init__()
         self.local_filesystem = local_filesystem
-        self.root.title("Select Vehicle directory")
-        self.root.geometry("800x535") # Set the window size
+        self.root.title("Amilcar Lucas's - ArduPilot methodic configurator " + VERSION + " - Select Vehicle directory")
+        self.root.geometry("800x575") # Set the window size
+        self.use_fc_params = tk.BooleanVar(value=False)
+        self.created_new_vehicle_from_template = False
 
         # Explain why we are here
         if local_filesystem.vehicle_dir == LocalFilesystem.getcwd():
             introduction_text = "No intermediate parameter files found\nin current working directory."
         else:
             introduction_text = "No intermediate parameter files found\nin the --vehicle-dir specified directory."
         introduction_label = tk.Label(self.root, text=introduction_text + \
                                            "\nChoose one of the following three options:")
         introduction_label.pack(expand=False, fill=tk.X, padx=6, pady=6)
         template_dir, new_base_dir, vehicle_dir = LocalFilesystem.get_recently_used_dirs()
         self.create_option1_widgets(template_dir,
                                     new_base_dir,
-                                    "MyVehicleName")
+                                    "MyVehicleName",
+                                    fc_connected)
         self.create_option2_widgets(vehicle_dir)
         self.create_option3_widgets(vehicle_dir)
 
         # Bind the close_connection_and_quit function to the window close event
         self.root.protocol("WM_DELETE_WINDOW", self.close_and_quit)
 
     def close_and_quit(self):
         sys_exit(0)
 
-    def create_option1_widgets(self, initial_template_dir: str, initial_base_dir: str, initial_new_dir: str):
+    def create_option1_widgets(self, initial_template_dir: str, initial_base_dir: str, initial_new_dir: str,
+                               fc_connected: bool):
         # Option 1 - Create a new vehicle configuration directory based on an existing template
         option1_label_frame = tk.LabelFrame(self.root, text="Create a new vehicle configuration directory")
         option1_label_frame.pack(expand=True, fill=tk.X, padx=6, pady=5)
         template_dir_edit_tooltip = "Existing vehicle template directory containing the\n" \
                                     "intermediate parameter files to be copied to the new vehicle directory"
         template_dir_btn_tooltip = "Select the existing vehicle template directory containing the\n" \
                                    "intermediate parameter files to be copied to the new vehicle directory"
         self.template_dir = DirectorySelectionWidgets(self, option1_label_frame, initial_template_dir,
                                                       "(source) Template directory:",
                                                       False,
                                                       template_dir_edit_tooltip,
                                                       template_dir_btn_tooltip)
         self.template_dir.container_frame.pack(expand=False, fill=tk.X, padx=3, pady=5, anchor=tk.NW)
+
+        use_fc_params_checkbox = Checkbutton(option1_label_frame, variable=self.use_fc_params,
+                                             text="Use parameter values from connected FC, not from template files")
+        use_fc_params_checkbox.pack(anchor=tk.NW)
+        show_tooltip(use_fc_params_checkbox, "Use the parameter values from the connected flight controller instead\n" \
+                     "of the template files when creating a new vehicle directory from a template.\n" \
+                     "This option is only available when a flight controller is connected")
+        if not fc_connected:
+            self.use_fc_params.set(False)
+            use_fc_params_checkbox.config(state=tk.DISABLED)
+
         new_base_dir_edit_tooltip = "Existing directory where the new vehicle directory will be created"
         new_base_dir_btn_tooltip = "Select the existing directory where the new vehicle directory will be created"
         self.new_base_dir = DirectorySelectionWidgets(self, option1_label_frame, initial_base_dir,
                                                       "(destination) base directory:",
                                                       False,
                                                       new_base_dir_edit_tooltip,
                                                       new_base_dir_btn_tooltip)
@@ -274,62 +298,83 @@
                      "Directly open the last used vehicle directory for configuring the vehicle")
 
     def create_new_vehicle_from_template(self):
         # Get the selected template directory and new vehicle directory name
         template_dir = self.template_dir.get_selected_directory()
         new_base_dir = self.new_base_dir.get_selected_directory()
         new_vehicle_name = self.new_dir.get_selected_directory()
+
+        if template_dir == "":
+            messagebox.showerror("Vehicle template directory", "Vehicle template directory cannot be empty")
+            return
+        if not LocalFilesystem.directory_exists(template_dir):
+            messagebox.showerror("Vehicle template directory", "Vehicle template directory does not exist")
+            return
+
         if new_vehicle_name == "":
-            show_error_message("New vehicle directory", "New vehicle name cannot be empty")
+            messagebox.showerror("New vehicle directory", "New vehicle name cannot be empty")
             return
         if not LocalFilesystem.valid_directory_name(new_vehicle_name):
-            show_error_message("New vehicle directory", "New vehicle name must not contain invalid characters")
+            messagebox.showerror("New vehicle directory", "New vehicle name must not contain invalid characters")
             return
-        new_vehicle_dir = self.local_filesystem.new_vehicle_dir(new_base_dir, new_vehicle_name)
+        new_vehicle_dir = LocalFilesystem.new_vehicle_dir(new_base_dir, new_vehicle_name)
 
         error_msg = self.local_filesystem.create_new_vehicle_dir(new_vehicle_dir)
         if error_msg:
-            show_error_message("New vehicle directory", error_msg)
+            messagebox.showerror("New vehicle directory", error_msg)
             return
 
         error_msg = self.local_filesystem.copy_template_files_to_new_vehicle_dir(template_dir, new_vehicle_dir)
         if error_msg:
-            show_error_message("Copying template files", error_msg)
+            messagebox.showerror("Copying template files", error_msg)
             return
 
         # Update the local_filesystem with the new vehicle directory
         self.local_filesystem.vehicle_dir = new_vehicle_dir
-        self.local_filesystem.re_init(new_vehicle_dir, self.local_filesystem.vehicle_type)
+
+        try:
+            self.local_filesystem.re_init(new_vehicle_dir, self.local_filesystem.vehicle_type)
+        except SystemExit as exp:
+            messagebox.showerror("Fatal error reading parameter files", f"{exp}")
+            raise
+
         files = list(self.local_filesystem.file_parameters.keys())
         if files:
             LocalFilesystem.store_recently_used_template_dirs(template_dir, new_base_dir)
             LocalFilesystem.store_recently_used_vehicle_dir(new_vehicle_dir)
             self.root.destroy()
         else:
             # No intermediate parameter files were found in the source template directory
             error_message = f"No intermediate parameter files found in the selected '{template_dir}'" \
                 " template vehicle directory.\n" \
                 "Please select a vehicle directory containing valid ArduPilot intermediate parameter files."
-            show_error_message("No Parameter Files Found", error_message)
+            messagebox.showerror("No Parameter Files Found", error_message)
+        self.created_new_vehicle_from_template = True
 
     def open_last_vehicle_directory(self, last_vehicle_dir: str):
         # Attempt to open the last opened vehicle directory
         if last_vehicle_dir:
             # If a last opened directory is found, proceed as if the user had manually selected it
             self.local_filesystem.vehicle_dir = last_vehicle_dir
-            self.local_filesystem.re_init(last_vehicle_dir, self.local_filesystem.vehicle_type)
+
+            try:
+                self.local_filesystem.re_init(last_vehicle_dir, self.local_filesystem.vehicle_type)
+            except SystemExit as exp:
+                messagebox.showerror("Fatal error reading parameter files", f"{exp}")
+                raise
+
             files = list(self.local_filesystem.file_parameters.keys())
             if files:
                 self.root.destroy()
             else:
                 show_no_param_files_error(last_vehicle_dir)
         else:
             # If no last opened directory is found, display a message to the user
-            show_error_message("No Last Vehicle Directory Found",
-                            "No last opened vehicle directory was found. Please select a directory manually.")
+            messagebox.showerror("No Last Vehicle Directory Found",
+                                 "No last opened vehicle directory was found. Please select a directory manually.")
 
 def argument_parser():
     """
     Parses command-line arguments for the script.
 
     This function sets up an argument parser to handle the command-line arguments for the script.
```

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_parameter_editor.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/frontend_tkinter_parameter_editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,29 +177,29 @@
         self.show_only_differences = None
         self.annotate_params_into_files = None
         self.parameter_editor_table = None
         self.reset_progress_window = None
         self.param_download_progress_window = None
         self.tempcal_imu_progress_window = None
 
-        self.root.title("Amilcar Lucas's - ArduPilot methodic configurator - " + version + \
+        self.root.title("Amilcar Lucas's - ArduPilot methodic configurator " + version + \
                         " - Parameter file editor and uploader")
         self.root.geometry("900x500") # Set the window width
 
         # Bind the close_connection_and_quit function to the window close event
         self.root.protocol("WM_DELETE_WINDOW", self.close_connection_and_quit)
 
         self.__create_conf_widgets(version)
 
         # Create a DocumentationFrame object for the Documentation Content
         self.documentation_frame = DocumentationFrame(self.root, self.local_filesystem, self.current_file)
 
         self.__create_parameter_area_widgets()
 
-        self.root.after(50, self.download_flight_controller_parameters(redownload=False)) # 50 milliseconds
+        #self.root.after(50, self.on_param_file_combobox_change(None, True)) # trigger a table update
         self.root.after(50, self.__please_read_the_docs())
         self.root.mainloop()
 
     def __create_conf_widgets(self, version: str):
         config_frame = tk.Frame(self.root)
         config_frame.pack(side=tk.TOP, fill="x", expand=False, pady=(4, 0)) # Pack the frame at the top of the window
 
@@ -312,15 +312,19 @@
                                            "the GUI will be unresponsive until it finishes.")
                     self.tempcal_imu_progress_window = ProgressWindow(self.root, "Reading IMU calibration messages",
                                                                       "Please wait, this can take a long time")
                     # Pass the selected filename to the IMUfit class
                     IMUfit(filename, tempcal_imu_result_param_fullpath, False, False, False, False,
                             self.local_filesystem.vehicle_dir, self.tempcal_imu_progress_window.update_progress_bar_300_pct)
                     self.tempcal_imu_progress_window.destroy()
-                    self.local_filesystem.file_parameters = self.local_filesystem.read_params_from_files()
+                    try:
+                        self.local_filesystem.file_parameters = self.local_filesystem.read_params_from_files()
+                    except SystemExit as exp:
+                        messagebox.showerror("Fatal error reading parameter files", f"{exp}")
+                        raise
                     self.parameter_editor_table.set_at_least_one_param_edited(True)  # force writing doc annotations to file
 
     def __should_copy_fc_values_to_file(self, selected_file: str):
         auto_changed_by = self.local_filesystem.auto_changed_by(selected_file)
         if auto_changed_by and self.flight_controller.fc_parameters:
             if messagebox.askyesno("Update file with values from FC?",
                                    "This configuration step should be performed outside this tool by\n"
@@ -415,38 +419,44 @@
                         if param_name in self.flight_controller.fc_parameters:
                             logging_info("Parameter %s changed from %f to %f, reset required", param_name,
                                          self.flight_controller.fc_parameters[param_name], param.value)
                         else:
                             logging_info("Parameter %s changed to %f, reset required", param_name, param.value)
                         fc_reset_required = True
                     # Check if any of the selected parameters have a _TYPE, _EN, or _ENABLE suffix
-                    elif param_name.endswith(('_TYPE', '_EN', '_ENABLE')):
+                    elif param_name.endswith(('_TYPE', '_EN', '_ENABLE', 'SID_AXIS')):
                         self.flight_controller.set_param(param_name, float(param.value))
                         self.at_least_one_changed_parameter_written = True
                         if param_name in self.flight_controller.fc_parameters:
                             logging_info("Parameter %s changed from %f to %f, possible reset required", param_name,
                                          self.flight_controller.fc_parameters[param_name], param.value)
                         else:
                             logging_info("Parameter %s changed to %f, possible reset required", param_name, param.value)
                         fc_reset_unsure.append(param_name)
             except ValueError as e:
                 logging_error("Failed to set parameter %s: %s", param_name, e)
                 messagebox.showerror("ArduPilot methodic configurator", f"Failed to set parameter {param_name}: {e}")
 
+        self.__reset_and_reconnect(fc_reset_required, fc_reset_unsure)
+
+    def __reset_and_reconnect(self, fc_reset_required, fc_reset_unsure):
         if not fc_reset_required:
             if fc_reset_unsure:
                 # Ask the user if they want to reset the ArduPilot
                 fc_reset_required = messagebox.askyesno("Possible reset required", f"{(', ').join(fc_reset_unsure)} parameter"
                                                         "(s) potentially require a reset\nDo you want to reset the ArduPilot?")
 
         if fc_reset_required:
             self.reset_progress_window = ProgressWindow(self.root, "Resetting Flight Controller",
                                                         "Waiting for {} of {} seconds")
             # Call reset_and_reconnect with a callback to update the reset progress bar and the progress message
-            self.flight_controller.reset_and_reconnect(self.reset_progress_window.update_progress_bar)
+            error_message = self.flight_controller.reset_and_reconnect(self.reset_progress_window.update_progress_bar)
+            if error_message:
+                logging_error(error_message)
+                messagebox.showerror("ArduPilot methodic configurator", error_message)
             self.reset_progress_window.destroy()  # for the case that we are doing a test and there is no real FC connected
 
     def on_upload_selected_click(self):
         self.parameter_editor_table.generate_edit_widgets_focus_out()
 
         self.write_changes_to_intermediate_parameter_file()
         selected_params = self.parameter_editor_table.get_upload_selected_params(self.current_file)
```

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/frontend_tkinter_parameter_editor_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,39 +29,33 @@
 from MethodicConfigurator.frontend_tkinter_base import show_tooltip
 #from MethodicConfigurator.frontend_tkinter_base import AutoResizeCombobox
 from MethodicConfigurator.frontend_tkinter_base import ScrollFrame
 
 from MethodicConfigurator.annotate_params import Par
 
 
-class ParameterEditorTable(ScrollFrame):  # pylint: disable=too-many-ancestors, too-many-instance-attributes
+class ParameterEditorTable(ScrollFrame):  # pylint: disable=too-many-ancestors
     """
     A class to manage and display the parameter editor table within the GUI.
 
     This class inherits from ScrollFrame and is responsible for creating,
     managing, and updating the table that displays parameters for editing.
     """
     def __init__(self, root, local_filesystem, parameter_editor):
         super().__init__(root)
         self.root = root
         self.local_filesystem = local_filesystem
         self.parameter_editor = parameter_editor
-        self.background_color = root.cget("background")
         self.current_file = None
         self.upload_checkbutton_var = {}
         self.at_least_one_param_edited = False
 
         # Prepare a dictionary that maps variable names to their values
         # These variables are used by the forced_parameters and derived_parameters in *_configuration_steps.json files
-        self.variables = {}
-        if hasattr(self.local_filesystem, 'vehicle_components') and self.local_filesystem.vehicle_components and \
-                'Components' in self.local_filesystem.vehicle_components:
-            self.variables['vehicle_components'] = self.local_filesystem.vehicle_components['Components']
-        if hasattr(self.local_filesystem, 'doc_dict') and self.local_filesystem.doc_dict:
-            self.variables['doc_dict'] = self.local_filesystem.doc_dict
+        self.variables = local_filesystem.get_eval_variables()
 
         self.compute_forced_and_derived_parameters()
 
     def compute_forced_and_derived_parameters(self):
         if self.local_filesystem.configuration_steps:
             for filename, file_info in self.local_filesystem.configuration_steps.items():
                 error_msg = self.local_filesystem.compute_parameters(filename, file_info, 'forced', self.variables)
@@ -181,15 +175,15 @@
         return delete_button
 
     def __create_parameter_name(self, param_name, param_metadata, doc_tooltip):
         is_calibration = param_metadata.get('Calibration', False) if param_metadata else False
         is_readonly = param_metadata.get('ReadOnly', False) if param_metadata else False
         parameter_label = tk.Label(self.view_port, text=param_name + (" " * (16 - len(param_name))),
                                            background="red" if is_readonly else "yellow" if is_calibration else
-                                           self.background_color)
+                                           self.root.cget("background"))
         if doc_tooltip:
             show_tooltip(parameter_label, doc_tooltip)
         return parameter_label
 
     def __create_flightcontroller_value(self, fc_parameters, param_name, param_default, doc_tooltip):
         if param_name in fc_parameters:
             value_str = format(fc_parameters[param_name], '.6f').rstrip('0').rstrip('.')
```

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/get_release_stats.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/get_release_stats.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/param_ftp.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/param_ftp.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/param_pid_adjustment_update.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/param_pid_adjustment_update.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator/tempcal_imu.py` & `methodicconfigurator-0.6.5/MethodicConfigurator/tempcal_imu.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/PKG-INFO` & `methodicconfigurator-0.6.5/MethodicConfigurator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MethodicConfigurator
-Version: 0.6.4
+Version: 0.6.5
 Summary: A clear configuration sequence for ArduPilot vehicles
 Home-page: https://github.com/ArduPilot/MethodicConfigurator
 Author: Amilcar do Carmo Lucas
 Author-email: amilcar.lucas@iav.de
 License: GPLv3
 Keywords: ArduPilot,Configuration,SCM,Methodic,ArduCopter,ArduPlane,ArduRover,ArduSub
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `methodicconfigurator-0.6.4/MethodicConfigurator.egg-info/SOURCES.txt` & `methodicconfigurator-0.6.5/MethodicConfigurator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 MethodicConfigurator/__init__.py
 MethodicConfigurator/annotate_params.py
 MethodicConfigurator/ardupilot_methodic_configurator.py
 MethodicConfigurator/backend_filesystem.py
 MethodicConfigurator/backend_filesystem_configuration_steps.py
 MethodicConfigurator/backend_filesystem_vehicle_components.py
 MethodicConfigurator/backend_flightcontroller.py
+MethodicConfigurator/backend_flightcontroller_info.py
 MethodicConfigurator/backend_mavftp.py
 MethodicConfigurator/battery_cell_voltages.py
 MethodicConfigurator/common_arguments.py
 MethodicConfigurator/extract_param_defaults.py
 MethodicConfigurator/frontend_tkinter_base.py
 MethodicConfigurator/frontend_tkinter_component_editor.py
 MethodicConfigurator/frontend_tkinter_component_editor_base.py
 MethodicConfigurator/frontend_tkinter_connection_selection.py
 MethodicConfigurator/frontend_tkinter_directory_selection.py
+MethodicConfigurator/frontend_tkinter_flightcontroller_info.py
 MethodicConfigurator/frontend_tkinter_parameter_editor.py
 MethodicConfigurator/frontend_tkinter_parameter_editor_table.py
 MethodicConfigurator/get_release_stats.py
 MethodicConfigurator/param_ftp.py
 MethodicConfigurator/param_pid_adjustment_update.py
 MethodicConfigurator/tempcal_imu.py
 MethodicConfigurator/version.py
@@ -39,28 +41,29 @@
 vehicle_templates/ArduCopter/X11_plus/03_imu_temperature_calibration_results.param
 vehicle_templates/ArduCopter/X11_plus/04_board_orientation.param
 vehicle_templates/ArduCopter/X11_plus/05_remote_controller.param
 vehicle_templates/ArduCopter/X11_plus/06_telemetry.param
 vehicle_templates/ArduCopter/X11_plus/07_esc.param
 vehicle_templates/ArduCopter/X11_plus/08_batt1.param
 vehicle_templates/ArduCopter/X11_plus/10_gnss.param
+vehicle_templates/ArduCopter/X11_plus/11_initial_atc.param
 vehicle_templates/ArduCopter/X11_plus/12_mp_setup_mandatory_hardware.param
 vehicle_templates/ArduCopter/X11_plus/13_general_configuration.param
 vehicle_templates/ArduCopter/X11_plus/14_logging.param
 vehicle_templates/ArduCopter/X11_plus/15_motor.param
 vehicle_templates/ArduCopter/X11_plus/16_pid_adjustment.param
 vehicle_templates/ArduCopter/X11_plus/17_remote_id.param
 vehicle_templates/ArduCopter/X11_plus/18_notch_filter_setup.param
 vehicle_templates/ArduCopter/X11_plus/19_notch_filter_results.param
 vehicle_templates/ArduCopter/X11_plus/20_throttle_controller.param
 vehicle_templates/ArduCopter/X11_plus/21_ekf_config.param
-vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.pdef.xml
 vehicle_templates/ArduCopter/X11_plus/22_quick_tune_setup.param
 vehicle_templates/ArduCopter/X11_plus/23_quick_tune_results.param
 vehicle_templates/ArduCopter/X11_plus/24_inflight_magnetometer_fit_setup.param
+vehicle_templates/ArduCopter/X11_plus/24_inflight_magnetometer_fit_setup.pdef.xml
 vehicle_templates/ArduCopter/X11_plus/25_inflight_magnetometer_fit_results.param
 vehicle_templates/ArduCopter/X11_plus/26_quick_tune_setup.param
 vehicle_templates/ArduCopter/X11_plus/27_quick_tune_results.param
 vehicle_templates/ArduCopter/X11_plus/28_evaluate_the_aircraft_tune_ff_disable.param
 vehicle_templates/ArduCopter/X11_plus/29_evaluate_the_aircraft_tune_ff_enable.param
 vehicle_templates/ArduCopter/X11_plus/30_autotune_roll_setup.param
 vehicle_templates/ArduCopter/X11_plus/31_autotune_roll_results.param
@@ -75,18 +78,18 @@
 vehicle_templates/ArduCopter/X11_plus/40_windspeed_estimation.param
 vehicle_templates/ArduCopter/X11_plus/41_barometer_compensation.param
 vehicle_templates/ArduCopter/X11_plus/42_system_id_roll.param
 vehicle_templates/ArduCopter/X11_plus/43_system_id_pitch.param
 vehicle_templates/ArduCopter/X11_plus/44_system_id_yaw.param
 vehicle_templates/ArduCopter/X11_plus/45_system_id_thrust.param
 vehicle_templates/ArduCopter/X11_plus/46_analytical_pid_optimization.param
-vehicle_templates/ArduCopter/X11_plus/47_everyday_use.param
-vehicle_templates/ArduCopter/X11_plus/48_position_controller.param
+vehicle_templates/ArduCopter/X11_plus/47_position_controller.param
+vehicle_templates/ArduCopter/X11_plus/48_guided_operation.param
 vehicle_templates/ArduCopter/X11_plus/49_precision_land.param
-vehicle_templates/ArduCopter/X11_plus/50_guided_operation.param
+vehicle_templates/ArduCopter/X11_plus/50_everyday_use.param
 vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml
 vehicle_templates/ArduCopter/X11_plus/tempcal_acc.png
 vehicle_templates/ArduCopter/X11_plus/tempcal_gyro.png
 vehicle_templates/ArduCopter/X11_plus/vehicle.jpg
 vehicle_templates/ArduCopter/X11_plus/vehicle_components.json
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param
@@ -94,28 +97,29 @@
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/04_board_orientation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/06_telemetry.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/08_batt1.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/11_initial_atc.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_mp_setup_mandatory_hardware.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_general_configuration.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/14_logging.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/15_motor.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/16_pid_adjustment.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/17_remote_id.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/19_notch_filter_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/20_throttle_controller.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/21_ekf_config.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_quick_tune_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/23_quick_tune_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_inflight_magnetometer_fit_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_inflight_magnetometer_fit_setup.pdef.xml
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/25_inflight_magnetometer_fit_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/26_quick_tune_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/27_quick_tune_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/28_evaluate_the_aircraft_tune_ff_disable.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/29_evaluate_the_aircraft_tune_ff_enable.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/30_autotune_roll_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/31_autotune_roll_results.param
@@ -130,45 +134,46 @@
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/40_windspeed_estimation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/41_barometer_compensation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_roll.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/43_system_id_pitch.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/44_system_id_yaw.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/45_system_id_thrust.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/46_analytical_pid_optimization.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_everyday_use.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_position_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_position_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_guided_operation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/49_precision_land.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/50_guided_operation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/50_everyday_use.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/04_board_orientation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/06_telemetry.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/08_batt1.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/11_initial_atc.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_mp_setup_mandatory_hardware.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_general_configuration.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/14_logging.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/15_motor.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/16_pid_adjustment.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/17_remote_id.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/18_notch_filter_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/19_notch_filter_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/20_throttle_controller.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/21_ekf_config.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_quick_tune_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/23_quick_tune_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_inflight_magnetometer_fit_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_inflight_magnetometer_fit_setup.pdef.xml
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/25_inflight_magnetometer_fit_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/26_quick_tune_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/27_quick_tune_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/28_evaluate_the_aircraft_tune_ff_disable.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/29_evaluate_the_aircraft_tune_ff_enable.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/30_autotune_roll_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/31_autotune_roll_results.param
@@ -183,98 +188,100 @@
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/40_windspeed_estimation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/41_barometer_compensation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_roll.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/43_system_id_pitch.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/44_system_id_yaw.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/45_system_id_thrust.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/46_analytical_pid_optimization.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_everyday_use.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_position_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_position_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_guided_operation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/49_precision_land.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/50_guided_operation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/50_everyday_use.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/04_board_orientation.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/06_telemetry.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/08_batt1.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/09_batt2.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/10_gnss.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_mp_setup_mandatory_hardware.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_general_configuration.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/14_logging.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/15_motor.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/16_pid_adjustment.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/17_remote_id.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/18_notch_filter_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/19_notch_filter_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/20_throttle_controller.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/21_ekf_config.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_quick_tune_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/23_quick_tune_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/24_inflight_magnetometer_fit_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/25_inflight_magnetometer_fit_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/26_quick_tune_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/27_quick_tune_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/28_evaluate_the_aircraft_tune_ff_disable.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/29_evaluate_the_aircraft_tune_ff_enable.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/30_autotune_roll_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/31_autotune_roll_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/32_autotune_pitch_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/33_autotune_pitch_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/34_autotune_yaw_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/35_autotune_yaw_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/36_autotune_yawd_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/37_autotune_yawd_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/38_autotune_roll_pitch_retune_setup.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_autotune_roll_pitch_retune_results.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/40_windspeed_estimation.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/41_barometer_compensation.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_roll.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/43_system_id_pitch.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/44_system_id_yaw.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/45_system_id_thrust.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/46_analytical_pid_optimization.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_everyday_use.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_position_controller.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/49_precision_land.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/50_guided_operation.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/00_default.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/02_imu_temperature_calibration_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/03_imu_temperature_calibration_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/04_board_orientation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/05_remote_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/06_telemetry.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/07_esc.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/08_batt1.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/09_batt2.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/10_gnss.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/11_initial_atc.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/12_mp_setup_mandatory_hardware.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/13_general_configuration.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/14_logging.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/15_motor.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/16_pid_adjustment.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/17_remote_id.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/18_notch_filter_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/19_notch_filter_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/20_throttle_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/21_ekf_config.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/22_quick_tune_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/23_quick_tune_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/24_inflight_magnetometer_fit_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/24_inflight_magnetometer_fit_setup.pdef.xml
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/25_inflight_magnetometer_fit_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/26_quick_tune_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/27_quick_tune_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/28_evaluate_the_aircraft_tune_ff_disable.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/29_evaluate_the_aircraft_tune_ff_enable.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/30_autotune_roll_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/31_autotune_roll_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/32_autotune_pitch_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/33_autotune_pitch_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/34_autotune_yaw_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/35_autotune_yaw_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/36_autotune_yawd_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/37_autotune_yawd_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/38_autotune_roll_pitch_retune_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/39_autotune_roll_pitch_retune_results.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/40_windspeed_estimation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/41_barometer_compensation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/42_system_id_roll.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/43_system_id_pitch.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/44_system_id_yaw.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/45_system_id_thrust.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/46_analytical_pid_optimization.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/47_position_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/48_guided_operation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/49_precision_land.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/50_everyday_use.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/apm.pdef.xml
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/vehicle.jpg
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/vehicle_components.json
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/04_board_orientation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/06_telemetry.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/07_esc.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/08_batt1.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/10_gnss.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/11_initial_atc.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_mp_setup_mandatory_hardware.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/13_general_configuration.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/14_logging.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/15_motor.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_pid_adjustment.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/17_remote_id.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/19_notch_filter_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/20_throttle_controller.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/21_ekf_config.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_quick_tune_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/23_quick_tune_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_inflight_magnetometer_fit_setup.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_inflight_magnetometer_fit_setup.pdef.xml
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/25_inflight_magnetometer_fit_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/26_quick_tune_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/27_quick_tune_results.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/28_evaluate_the_aircraft_tune_ff_disable.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/29_evaluate_the_aircraft_tune_ff_enable.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/30_autotune_roll_setup.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/31_autotune_roll_results.param
@@ -289,14 +296,14 @@
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/40_windspeed_estimation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/41_barometer_compensation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_roll.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/43_system_id_pitch.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/44_system_id_yaw.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/45_system_id_thrust.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/46_analytical_pid_optimization.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_everyday_use.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_position_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_position_controller.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_guided_operation.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/49_precision_land.param
-vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/50_guided_operation.param
+vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/50_everyday_use.param
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg
 vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json
```

### Comparing `methodicconfigurator-0.6.4/PKG-INFO` & `methodicconfigurator-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MethodicConfigurator
-Version: 0.6.4
+Version: 0.6.5
 Summary: A clear configuration sequence for ArduPilot vehicles
 Home-page: https://github.com/ArduPilot/MethodicConfigurator
 Author: Amilcar do Carmo Lucas
 Author-email: amilcar.lucas@iav.de
 License: GPLv3
 Keywords: ArduPilot,Configuration,SCM,Methodic,ArduCopter,ArduPlane,ArduRover,ArduSub
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `methodicconfigurator-0.6.4/README.md` & `methodicconfigurator-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/setup.py` & `methodicconfigurator-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/00_default.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/02_imu_temperature_calibration_setup.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/02_imu_temperature_calibration_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/03_imu_temperature_calibration_results.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/03_imu_temperature_calibration_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/07_esc.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/07_esc.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/10_gnss.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/10_gnss.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/12_mp_setup_mandatory_hardware.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/12_mp_setup_mandatory_hardware.param`

 * *Files 2% similar despite different names*

```diff
@@ -69,11 +69,14 @@
 RC7_TRIM,1395.0
 RC8_MAX,1900.0
 RC8_MIN,1100.0
 RC8_TRIM,1500.0
 RC9_MAX,1933.0
 RC9_MIN,1066.0
 RC9_TRIM,1066.0
+RC10_MAX,1932
+RC10_MIN,1057
+RC10_TRIM,1057
 SERVO1_FUNCTION,33.0
 SERVO2_FUNCTION,34.0
 SERVO3_FUNCTION,35.0
 SERVO4_FUNCTION,36.0
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/13_general_configuration.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/13_general_configuration.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/16_pid_adjustment.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/16_pid_adjustment.param`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 # If you have a very small, or a very large vehicle that requires non-default PID values for a safe flight, change them here
 #
 # Usually, smaller vehicles require lower than default PID rate values.
 # Larger vehicles usually require higher than default PID rate values.
 
-ATC_ANG_PIT_P,6.0
-ATC_ANG_RLL_P,5.2
-ATC_ANG_YAW_P,3.0
-ATC_INPUT_TC,0.17
-ATC_RAT_PIT_D,0.002781  #  (0.0036 default)
-ATC_RAT_PIT_I,0.085568  #  = 1.283176 * (0.135 default)
-ATC_RAT_PIT_P,0.085568  #  = 1.283176 * (0.135 default)
-ATC_RAT_RLL_D,0.00309  #  = 0.690593 * (0.0036 default)
-ATC_RAT_RLL_I,0.095506  #  = 1.061015 * (0.135 default)
-ATC_RAT_RLL_P,0.095506  #  = 1.061015 * (0.135 default)
+ATC_INPUT_TC,0.15
+ATC_RAT_PIT_D,0.003334  #  = 0.925972 * (0.0036 default)
+ATC_RAT_PIT_I,0.173229  #  = 1.283176 * (0.135 default)
+ATC_RAT_PIT_P,0.173229  #  = 1.283176 * (0.135 default)
+ATC_RAT_RLL_D,0.002486  #  = 0.690593 * (0.0036 default)
+ATC_RAT_RLL_I,0.143237  #  = 1.061015 * (0.135 default)
+ATC_RAT_RLL_P,0.143237  #  = 1.061015 * (0.135 default)
 ATC_RAT_YAW_D,0  #  = 1 * (0 default)
-ATC_RAT_YAW_I,0.025  #  = 2.514026 * (0.018 default)
-ATC_RAT_YAW_P,0.25  #  = 2.514026 * (0.18 default)
+ATC_RAT_YAW_I,0.045252  #  = 2.514026 * (0.018 default)
+ATC_RAT_YAW_P,0.452525  #  = 2.514026 * (0.18 default)
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/18_notch_filter_setup.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/18_notch_filter_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/19_notch_filter_results.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/19_notch_filter_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/24_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/24_inflight_magnetometer_fit_setup.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/24_inflight_magnetometer_fit_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/25_inflight_magnetometer_fit_results.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/25_inflight_magnetometer_fit_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/42_system_id_roll.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/42_system_id_roll.param`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-ANGLE_MAX,1500  # limit the angle to limit the speed at SID-chirp low-frequencies
+ANGLE_MAX,2000  # limit the angle to limit the speed at SID-chirp low-frequencies
 ARMING_CHECK,540126  # disable Parameter check because we need to set ATC_RAT_RLL_I out-of-range (was 30175)
-ATC_RAT_RLL_I,0 # prevent the rate controllers from compensating too much of the frequency-sweep signal
-ATC_RATE_FF_ENAB,0 # prevent the rate controllers from compensating too much of the frequency-sweep signal
-LOG_DISARMED,0 # was only needed for wind speed estimation
-LOG_REPLAY,0 # was only needed for wind speed estimation
-SID_AXIS,10
+ATC_ANG_PIT_P,4.5  # reset to default to not interfere with sysID
+ATC_ANG_RLL_P,4.5  # reset to default to not interfere with sysID
+ATC_ANG_YAW_P,4.5  # reset to default to not interfere with sysID
+ATC_RAT_RLL_I,0  # prevent the rate controllers from compensating too much of the frequency-sweep signal
+ATC_RATE_FF_ENAB,0  # prevent the rate controllers from compensating too much of the frequency-sweep signal
+FLTMODE5,25  # Activate sysid instead of autotune
+LOG_BITMASK,176127  # attitude sample rate at loop rate
+LOG_DISARMED,0  # was only needed for wind speed estimation
+LOG_REPLAY,0  # was only needed for wind speed estimation
+SID_AXIS,10  # Inject chip on the mixer roll signal
 SID_F_START_HZ,0.05
 SID_F_STOP_HZ,5
 SID_MAGNITUDE,0.15
 SID_T_FADE_IN,5.0
 SID_T_FADE_OUT,5.0
 SID_T_REC,130.0
-TUNE,58  # System identification magnitude
-TUNE_MAX,0.40  # System identification max magnitude
+TUNE,0  # System identification magnitude
+TUNE_MAX,0.4  # System identification max magnitude
 TUNE_MIN,0.02  # System identification min magnitude
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/47_everyday_use.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/50_everyday_use.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/48_position_controller.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/47_position_controller.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/49_precision_land.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/49_precision_land.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml`

 * *Files 20% similar despite different names*

#### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/apm.pdef.xml`

```diff
@@ -1,9 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- Dynamically generated list of documented parameters (generated by param_parse.py) -->
+<!-- Generated from git tag Copter-4.5.3 on 2024-05-30 14:47:49 -->
 <paramfile>
   <vehicles>
     <parameters name="ArduCopter">
       <param humanName="Eeprom format version number" name="ArduCopter:FORMAT_VERSION" documentation="This value is incremented when changes are made to the eeprom format" user="Advanced">
         <field name="ReadOnly">True</field>
       </param>
       <param humanName="MAVLink system ID of this vehicle" name="ArduCopter:SYSID_THISMAV" documentation="Allows setting an individual MAVLink system id for this vehicle to distinguish it from others on the same network" user="Advanced">
@@ -1934,14 +1935,20 @@
         </values>
       </param>
       <param humanName="Compass magnetic field strength error threshold vs earth magnetic model" name="ARMING_MAGTHRESH" documentation="Compass magnetic field strength error threshold vs earth magnetic model.  X and y axis are compared using this threhold, Z axis uses 2x this threshold.  0 to disable check" user="Advanced">
         <field name="Units">mGauss</field>
         <field name="UnitText">milligauss</field>
         <field name="Range">0 500</field>
       </param>
+      <param humanName="Disable CrashDump Arming check" name="ARMING_CRSDP_IGN" documentation="Must have value &quot;1&quot; if crashdump data is present on the system, or a prearm failure will be raised.  Do not set this parameter unless the risks of doing so are fully understood.  The presence of a crash dump means that the firmware currently installed has suffered a critical software failure which resulted in the autopilot immediately rebooting.  The crashdump file gives diagnostic information which can help in finding the issue, please contact the ArduPIlot support team.  If this crashdump data is present, the vehicle is likely unsafe to fly.  Check the ArduPilot documentation for more details." user="Advanced">
+        <values>
+          <value code="0">Crash Dump arming check active</value>
+          <value code="1">Crash Dump arming check deactivated</value>
+        </values>
+      </param>
     </parameters>
     <parameters name="AROT_">
       <param humanName="Enable settings for RSC Setpoint" name="AROT_ENABLE" documentation="Allows you to enable (1) or disable (0) the autonomous autorotation capability." user="Advanced">
         <values>
           <value code="0">Disabled</value>
           <value code="1">Enabled</value>
         </values>
@@ -2763,15 +2770,15 @@
       </param>
       <param humanName="Avoidance behaviour" name="AVOID_BEHAVE" documentation="Avoidance behaviour (slide or stop)" user="Standard">
         <values>
           <value code="0">Slide</value>
           <value code="1">Stop</value>
         </values>
       </param>
-      <param humanName="Avoidance maximum backup speed" name="AVOID_BACKUP_SPD" documentation="Maximum speed that will be used to back away from obstacles in GPS modes (m/s). Set zero to disable" user="Standard">
+      <param humanName="Avoidance maximum horizontal backup speed" name="AVOID_BACKUP_SPD" documentation="Maximum speed that will be used to back away from obstacles horizontally in position control modes (m/s). Set zero to disable horizontal backup." user="Standard">
         <field name="Units">m/s</field>
         <field name="UnitText">meters per second</field>
         <field name="Range">0 2</field>
       </param>
       <param humanName="Avoidance minimum altitude" name="AVOID_ALT_MIN" documentation="Minimum altitude above which proximity based avoidance will start working. This requires a valid downward facing rangefinder reading to work. Set zero to disable" user="Standard">
         <field name="Units">m</field>
         <field name="UnitText">meters</field>
@@ -2783,14 +2790,19 @@
         <field name="Range">0 9</field>
       </param>
       <param humanName="Avoidance deadzone between stopping and backing away from obstacle" name="AVOID_BACKUP_DZ" documentation="Distance beyond AVOID_MARGIN parameter, after which vehicle will backaway from obstacles. Increase this parameter if you see vehicle going back and forth in front of obstacle." user="Standard">
         <field name="Units">m</field>
         <field name="UnitText">meters</field>
         <field name="Range">0 2</field>
       </param>
+      <param humanName="Avoidance maximum vertical backup speed" name="AVOID_BACKZ_SPD" documentation="Maximum speed that will be used to back away from obstacles vertically in height control modes (m/s). Set zero to disable vertical backup." user="Standard">
+        <field name="Units">m/s</field>
+        <field name="UnitText">meters per second</field>
+        <field name="Range">0 2</field>
+      </param>
     </parameters>
     <parameters name="BARO">
       <param humanName="Ground Pressure" name="BARO1_GND_PRESS" documentation="calibrated ground pressure in Pascals" user="Advanced">
         <field name="Units">Pa</field>
         <field name="UnitText">pascal</field>
         <field name="Increment">1</field>
         <field name="ReadOnly">True</field>
@@ -6916,14 +6928,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -7034,14 +7047,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -7152,14 +7166,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -7270,14 +7285,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -12994,14 +13010,17 @@
         <field name="Range">0.0 0.2</field>
         <field name="Increment">.005</field>
       </param>
       <param humanName="Mount Target sysID" name="MNT1_SYSID_DFLT" documentation="Default Target sysID for the mount to point to" user="Standard">
         <field name="RebootRequired">True</field>
       </param>
       <param humanName="Mount Device ID" name="MNT1_DEVID" documentation="Mount device ID, taking into account its type, bus and instance" user="Advanced"/>
+      <param humanName="Mount options" name="MNT1_OPTIONS" documentation="Mount options bitmask" user="Standard">
+        <field name="Bitmask">0:RC lock state from previous mode</field>
+      </param>
     </parameters>
     <parameters name="MNT2">
       <param humanName="Mount Type" name="MNT2_TYPE" documentation="Mount Type" user="Standard">
         <values>
           <value code="0">None</value>
           <value code="1">Servo</value>
           <value code="2">3DR Solo</value>
@@ -13118,14 +13137,17 @@
         <field name="Range">0.0 0.2</field>
         <field name="Increment">.005</field>
       </param>
       <param humanName="Mount Target sysID" name="MNT2_SYSID_DFLT" documentation="Default Target sysID for the mount to point to" user="Standard">
         <field name="RebootRequired">True</field>
       </param>
       <param humanName="Mount Device ID" name="MNT2_DEVID" documentation="Mount device ID, taking into account its type, bus and instance" user="Advanced"/>
+      <param humanName="Mount options" name="MNT2_OPTIONS" documentation="Mount options bitmask" user="Standard">
+        <field name="Bitmask">0:RC lock state from previous mode</field>
+      </param>
     </parameters>
     <parameters name="MOT_">
       <param humanName="Matrix Yaw Min" name="MOT_YAW_HEADROOM" documentation="Yaw control is given at least this pwm in microseconds range" user="Advanced">
         <field name="Range">0 500</field>
         <field name="Units">PWM</field>
         <field name="UnitText">PWM in microseconds</field>
       </param>
@@ -18184,14 +18206,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -18333,14 +18356,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -18482,14 +18506,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -18631,14 +18656,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -18780,14 +18806,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -18929,14 +18956,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -19078,14 +19106,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -19227,14 +19256,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -19376,14 +19406,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -19525,14 +19556,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -19674,14 +19706,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -19823,14 +19856,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -19972,14 +20006,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -20121,14 +20156,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -20270,14 +20306,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -20419,14 +20456,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/tempcal_acc.png` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/tempcal_acc.png`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/tempcal_gyro.png` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/tempcal_gyro.png`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/vehicle.jpg` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/X11_plus/vehicle_components.json` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/vehicle_components.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9888599537037037%*

 * *Differences: {"'Components'": "{'Flight Controller': {'Firmware': {'Version': '4.5.3'}}, 'Frame': {'Product': "*

 * *                 "{'Model': 'Custom Aluminum'}, 'Notes': 'Frame is custom, X type frame, the "*

 * *                 "middle is welded. Arm length is 1950mm.', 'Specifications': OrderedDict([('TOW "*

 * *                 "min Kg', 20), ('TOW max Kg', 50)])}, 'RC Controller': {'Notes': 'It has 10 "*

 * *                 "channels and an integrated RC transmitter'}, 'Telemetry': {'Notes': 'High range "*

 * *                 "and st […]*

```diff
@@ -1,18 +1,19 @@
 {
     "Components": {
         "Battery": {
             "Notes": "Normal battery 3.5 kg.",
             "Product": {
                 "Manufacturer": "gensTattu",
-                "Model": "6C 30000mah",
+                "Model": "6C 30000mAh",
                 "URL": "https://genstattu.com/tattu-g-tech-30000mah-6s-22-2v-25c-lipo-battery-pack-with-as150u-f-plug/",
                 "Version": "AS150U-F"
             },
             "Specifications": {
+                "Capacity mAh": 30000,
                 "Chemistry": "LipoHV",
                 "Number of cells": 6,
                 "Volt per cell crit": 3.55,
                 "Volt per cell low": 3.6,
                 "Volt per cell max": 4.2
             }
         },
@@ -49,31 +50,35 @@
                 "URL": "https://vi.aliexpress.com/i/1005005384267348.html?gatewayAdapt=glo2vnm",
                 "Version": "1"
             }
         },
         "Flight Controller": {
             "Firmware": {
                 "Type": "ArduCopter",
-                "Version": "4.5.1"
+                "Version": "4.5.3"
             },
             "Notes": "This is CubeOrange with 94.5mm x 44.3mm x 17.3mm",
             "Product": {
                 "Manufacturer": "CubePilot",
                 "Model": "CubeOrange",
                 "URL": "https://www.robotshop.com/products/cubepilot-the-cube-orange-standard-set-ads-b-carrier-board",
                 "Version": "1.0"
             }
         },
         "Frame": {
-            "Notes": "Frame is custom, X type frame, the middle is welded. Arm lenght is 1950mm.",
+            "Notes": "Frame is custom, X type frame, the middle is welded. Arm length is 1950mm.",
             "Product": {
                 "Manufacturer": "Papa Seleckis",
-                "Model": "Custom Aluminiumm",
+                "Model": "Custom Aluminum",
                 "URL": "",
                 "Version": "30 Kg payload"
+            },
+            "Specifications": {
+                "TOW max Kg": 50,
+                "TOW min Kg": 20
             }
         },
         "GNSS receiver": {
             "FC Connection": {
                 "Protocol": "DroneCAN",
                 "Type": "CAN1"
             },
@@ -98,15 +103,15 @@
                 "Version": ""
             },
             "Specifications": {
                 "Poles": 14
             }
         },
         "Propellers": {
-            "Notes": "Hobbywing high quality propellers",
+            "Notes": "Hobbywing high-quality propellers",
             "Product": {
                 "Manufacturer": "HOBBYWING",
                 "Model": "43\"",
                 "URL": "https://www.amazon.com/HAWEWE-Hobbywing-Plastics-Propeller-Agricultural/dp/B0CH7WLPCG",
                 "Version": ""
             },
             "Specifications": {
@@ -114,15 +119,15 @@
             }
         },
         "RC Controller": {
             "Firmware": {
                 "Type": "AT9S",
                 "Version": "V1.2.9"
             },
-            "Notes": "It has 10 channels and integrated RC transmitter",
+            "Notes": "It has 10 channels and an integrated RC transmitter",
             "Product": {
                 "Manufacturer": "Radiolink",
                 "Model": "AT9S Pro",
                 "URL": "https://www.amazon.com/Radiolink-Remote-Controller-Receiver-Helicopter/dp/B07VC3VJGM?th=1",
                 "Version": ""
             }
         },
@@ -161,15 +166,15 @@
                 "Protocol": "MAVLink2",
                 "Type": "SERIAL1"
             },
             "Firmware": {
                 "Type": "",
                 "Version": ""
             },
-            "Notes": "High range and strenght telemetry.",
+            "Notes": "High range and strength telemetry.",
             "Product": {
                 "Manufacturer": "HOLYBRO",
                 "Model": "Microhard Telemetry Radio P840",
                 "URL": "https://holybro.com/products/microhard-radio?variant=41473588265149",
                 "Version": ""
             }
         }
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/02_imu_temperature_calibration_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/03_imu_temperature_calibration_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/05_remote_controller.param`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ARMING_RUDDER,0  # We find it safer to use only a switch to arm instead of through rudder inputs
-BRD_ALT_CONFIG,1 # Matek H743-specific: Hardware-Pin Rx6 is Rx from UART 7
-RC_OPTIONS,288 # Enables Crossfire Telemetry
-RC_PROTOCOLS,512 # Deactivates all protocols except TBS Crossfire
-RC6_OPTION,153 # "Arm/Disarm", to use an arming switch (here Channel 6)
+BRD_ALT_CONFIG,1  # Matek H743-specific: Hardware-Pin Rx6 is Rx from UART 7
+RC_OPTIONS,288  # Enables Crossfire Telemetry
+RC_PROTOCOLS,512  # Selected in the component editor
+RC6_OPTION,153  # "Arm/Disarm", to use an arming switch (here Channel 6)
 RC7_OPTION,31  # "Motor Emergency Stop", stops all motors immediately at a high signal
 RC8_OPTION,30  # "Lost Copter Sound", generates a loud tone from the buzzer at a high signal to locate a lost multicopter
-RC9_OPTION,300 # Used to jump to the next waypoint
-RSSI_TYPE,3 # TBS Crossfire protocol provides RSSI
-SERIAL7_PROTOCOL,23 # Specifies the serial port 7 as RC-Input
+RC9_OPTION,300  # Used to jump to the next waypoint
+RSSI_TYPE,3  # TBS Crossfire protocol provides RSSI
+SERIAL7_PROTOCOL,23  # Specifies the serial port 7 as RC-Input
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/07_esc.param`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 ATC_RAT_PIT_SMAX,25  # limit the slew rate to prevent possible ESC desync - https://ardupilot.org/copter/docs/common-servo-limit-cycle-detection.html
 ATC_RAT_RLL_SMAX,25  # limit the slew rate to prevent possible ESC desync - https://ardupilot.org/copter/docs/common-servo-limit-cycle-detection.html
 ATC_RAT_YAW_SMAX,25  # limit the slew rate to prevent possible ESC desync - https://ardupilot.org/copter/docs/common-servo-limit-cycle-detection.html
-MOT_PWM_TYPE,6  # the most recomended speed for ArduCopter
+MOT_HOVER_LEARN,2  # So that it can tune the throttle controller on the 20_throttle_controller.param file
+MOT_PWM_MAX,2000
+MOT_PWM_MIN,1000
+MOT_PWM_TYPE,6  # Specified in component editor window
+MOT_SPOOL_TIME,0.5  # left at default because copter is small
 NTF_BUZZ_TYPES,3  # the 4-in-1 ESC uses this
 NTF_LED_TYPES,2369  # Built-in LED, NCP5623 External (Holybro F9P), Neopixel (Matek H743 slim v3), and DShot (4-in-1 ESC)
 PSC_ACCZ_SMAX,25  # limit the slew rate to prevent possible ESC desync - https://ardupilot.org/copter/docs/common-servo-limit-cycle-detection.html
 SERIAL5_BAUD,115  # bi-directional DShot telemetry data rate from T-Motor F45 4in1 ESC V2
 SERIAL5_PROTOCOL,16  # bi-directional DShot telemetry pin is connected to SERIAL5
 SERVO_BLH_AUTO,1  # Enables BLHeli pass-thru
 SERVO_BLH_BDMASK,15  # All four of our ESC support bi-directional DShot
@@ -23,7 +27,8 @@
 SERVO3_MAX,2000  # Use the full available 1000-2000 DShot range
 SERVO3_MIN,1000  # Use the full available 1000-2000 DShot range
 SERVO3_TRIM,1000  # Use the full available 1000-2000 DShot range
 SERVO4_MAX,2000  # Use the full available 1000-2000 DShot range
 SERVO4_MIN,1000  # Use the full available 1000-2000 DShot range
 SERVO4_TRIM,1000  # Use the full available 1000-2000 DShot range
 TKOFF_RPM_MIN,1400  # Our motors should idle at around 1400 RPM, see https://ardupilot.org/copter/docs/tkoff-rpm-min.html
+TKOFF_SLEW_TIME,2  # left at default because copter is small
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/09_batt2.param`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-BATT2_AMP_PERVLT,17.5
-BATT2_ARM_VOLT,15 # In our build this is a redundant monitor for batt1 so == BATT_ARM_VOLT
-BATT2_CAPACITY,1800 # In our build this is a redundant monitor for batt1 so == BATT_CAPACITY
-BATT2_CRT_MAH,450 # In our build this is a redundant monitor for batt1 so == BATT_CRT_MAH
-BATT2_CRT_VOLT,14 # In our build this is a redundant monitor for batt1 so == BATT_CRT_VOLT
+BATT2_AMP_PERVLT,17.73  # calibrated using batt charger
+BATT2_ARM_VOLT,15  # In our build this is a redundant monitor for batt1 so == BATT_ARM_VOLT
+BATT2_CAPACITY,1800  # In our build this is a redundant monitor for batt1 so == BATT_CAPACITY
+BATT2_CRT_MAH,450  # In our build this is a redundant monitor for batt1 so == BATT_CRT_MAH
+BATT2_CRT_VOLT,14  # In our build this is a redundant monitor for batt1 so == BATT_CRT_VOLT
 BATT2_CURR_PIN,7
-BATT2_FS_CRT_ACT,1  # flying indoors, just land ASAP, no need to hit the celing while doing RTL
-BATT2_FS_LOW_ACT,1  # flying indoors, just land ASAP, no need to hit the celing while doing RTL
+BATT2_FS_CRT_ACT,1  # flying indoors, just land ASAP, no need to hit the ceiling while doing RTL
+BATT2_FS_LOW_ACT,1  # flying indoors, just land ASAP, no need to hit the ceiling while doing RTL
 BATT2_FS_VOLTSRC,1  # In our build this is a redundant monitor for batt1 so == BATT_FS_VOLTSRC
 BATT2_LOW_MAH,600  # In our build this is a redundant monitor for batt1 so == BATT_LOW_MAH
 BATT2_LOW_VOLT,14.4  # In our build this is a redundant monitor for batt1 so == BATT_LOW_VOLT
 BATT2_MONITOR,4
-BATT2_VOLT_MULT,228.342 # Use a power source with a voltage close to BATT2_LOW_VOLT measure with a calibrated voltimeter and adapt this parameter so that the telemetry voltage reading matches it
+BATT2_VOLT_MULT,228.342  # Use a power source with a voltage close to BATT2_LOW_VOLT measure with a calibrated voltimeter and adapt this parameter so that the telemetry voltage reading matches it
 BATT2_VOLT_PIN,18
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/10_gnss.param`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 BRD_SAFETY_DEFLT,0  # Matek H743 Slim has no safety switch
 GPS_GNSS_MODE,7  # limit the constalations to ensure an update rate higher than 5Hz
 GPS_POS1_X,0.056  # HX-CH7604A GNSS antenna pahse center location relative to CG
 GPS_POS1_Y,0  # HX-CH7604A GNSS antenna pahse center location relative to CG
 GPS_POS1_Z,-0.07  # HX-CH7604A GNSS antenna pahse center location relative to CG
-GPS_TYPE,2  # set it explicit to uBlox, instead of guessing which GNSS receiver we have
+GPS_TYPE,2  # Defined in component editor
 SERIAL3_PROTOCOL,5  # GNSS receiver is connected to serial3
 WPNAV_RADIUS,100  # we have a good GNSS receiver so we can afford to fly precisely
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_mp_setup_mandatory_hardware.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/12_mp_setup_mandatory_hardware.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_general_configuration.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/13_general_configuration.param`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-ARMING_CHECK,1  # perform all arming checks. If you have a problem fix it's source. Do NOT change this
+ARMING_CHECK,1  # Perform all arming checks. If you have a problem fix its source. Do NOT change this
 BRD_RTC_TZ_MIN,60  # Berlin time zone
 FENCE_TYPE,7  # cylinder and max altitude, to obey local regulations and safety measures
 INS_ACCEL_FILTER,10  # the default is 20 and that lets too much noise in
 INS_POS1_X,0  # was -0.005
 INS_POS1_Y,0  # was -0.011
 INS_POS2_X,0  # was -0.011
 INS_POS2_Y,0  # was -0.01
 LAND_ALT_LOW,200  # come down fast and only slow down close to the ground. We have a good GNSS receiver, so thrust it
 RTL_ALT,300  # The default is too high for the kind of flights we do. This reduces the altitude for indoors
 RTL_LOIT_TIME,1000  # The default is too long. This reduces the time
 SCHED_LOOP_RATE,800  # On our vehicle the propellers rotate at speeds higher than 400Hz and we have a powerful STM32 H7 family processor. So we increase this for added performance.
-SCR_ENABLE,1  # For VTOL-Quicktune, MagFit automation and Windspeed Estimation automation
+SCR_ENABLE,1  # Use lua scripting for VTOL-Quicktune, MagFit automation and Windspeed Estimation automation
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/16_pid_adjustment.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/16_pid_adjustment.param`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # If you have a very small, or a very large vehicle that requires non-default PID values for a safe flight, change them here
 #
 # Usually, smaller vehicles require lower than default PID rate values.
 # Larger vehicles usually require higher than default PID rate values.
 
+ATC_INPUT_TC,0.15
 ATC_RAT_PIT_D,0.003334  #  = 0.925972 * (0.0036 default)
 ATC_RAT_PIT_I,0.173229  #  = 1.283176 * (0.135 default)
 ATC_RAT_PIT_P,0.173229  #  = 1.283176 * (0.135 default)
 ATC_RAT_RLL_D,0.002486  #  = 0.690593 * (0.0036 default)
 ATC_RAT_RLL_I,0.143237  #  = 1.061015 * (0.135 default)
 ATC_RAT_RLL_P,0.143237  #  = 1.061015 * (0.135 default)
 ATC_RAT_YAW_D,0  #  = 1 * (0 default)
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_setup.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/18_notch_filter_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_inflight_magnetometer_fit_setup.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/24_inflight_magnetometer_fit_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_autotune_roll_pitch_retune_results.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/39_autotune_roll_pitch_retune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_roll.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/42_system_id_roll.param`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-ANGLE_MAX,1500  # limit the angle to limit the speed at SID-chirp low-frequencies
+ANGLE_MAX,2000  # limit the angle to limit the speed at SID-chirp low-frequencies
 ARMING_CHECK,540126  # disable Parameter check because we need to set ATC_RAT_RLL_I out-of-range (was 30175)
+ATC_ANG_PIT_P,4.5  # reset to default to not interfere with sysID
+ATC_ANG_RLL_P,4.5  # reset to default to not interfere with sysID
+ATC_ANG_YAW_P,4.5  # reset to default to not interfere with sysID
 ATC_RAT_RLL_I,0  # prevent the rate controllers from compensating too much of the frequency-sweep signal
 ATC_RATE_FF_ENAB,0  # prevent the rate controllers from compensating too much of the frequency-sweep signal
-FLTMODE5,25
+FLTMODE5,25  # Activate sysid instead of autotune
+LOG_BITMASK,176127  # attitude sample rate at loop rate
 LOG_DISARMED,0  # was only needed for wind speed estimation
 LOG_REPLAY,0  # was only needed for wind speed estimation
 SID_AXIS,10  # Inject chip on the mixer roll signal
 SID_F_START_HZ,0.05
 SID_F_STOP_HZ,5
 SID_MAGNITUDE,0.15
 SID_T_FADE_IN,5.0
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_everyday_use.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/50_everyday_use.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/48_position_controller.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/47_position_controller.param`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ANGLE_MAX,6500
+LOIT_ACC_MAX,500
 LOIT_BRK_ACCEL,500
 LOIT_BRK_DELAY,0.05
 LOIT_BRK_JERK,4000
 PSC_VELXY_FF,0.85  # PSCN.AE/PSCN.VE if you have flown North-South or PSCE.AE/PSCE.VE if you have flown East-West
 WPNAV_ACCEL,400  # high speed missions in auto
 WPNAV_ACCEL_C,800  # 2 * WPNAV_ACCEL so that the cornering behaviour is mostly controlled by WPNAV_RADIUS https://github.com/ArduPilot/ardupilot/pull/25928
 WPNAV_ACCEL_Z,200  # high speed missions in auto
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/49_precision_land.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/49_precision_land.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.3.8-params/vehicle_components.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954788773148148%*

 * *Differences: {"'Components'": "{'Flight Controller': {'Firmware': {'Version': '4.3.8'}}, 'Frame': "*

 * *                 "{'Specifications': OrderedDict([('TOW min Kg', 0.6), ('TOW max Kg', 0.6)])}, "*

 * *                 "'Battery Monitor': {'Firmware': {'Version': '4.3.8'}}, 'Battery': "*

 * *                 "{'Specifications': {'Capacity mAh': 1800}}}"}*

```diff
@@ -5,29 +5,30 @@
             "Product": {
                 "Manufacturer": "SLS",
                 "Model": "X-Cube 1800mAh 4S1P 14,8V 40C/80C",
                 "URL": "https://www.stefansliposhop.de/akkus/sls-x-cube/sls-x-cube-40c/sls-x-cube-1800mah-4s1p-14-8v-40c-80c::1568.html",
                 "Version": ""
             },
             "Specifications": {
+                "Capacity mAh": 1800,
                 "Chemistry": "Lipo",
                 "Number of cells": 4,
                 "Volt per cell crit": 3.55,
                 "Volt per cell low": 3.6,
                 "Volt per cell max": 4.2
             }
         },
         "Battery Monitor": {
             "FC Connection": {
                 "Protocol": "Analog Voltage and Current",
                 "Type": "Analog"
             },
             "Firmware": {
                 "Type": "ArduCopter",
-                "Version": "4.5.1"
+                "Version": "4.3.8"
             },
             "Notes": "Voltage is done via the flight controller. Current is done via the ESC.",
             "Product": {
                 "Manufacturer": "Matek",
                 "Model": "H743 SLIM",
                 "URL": "https://www.mateksys.com/?portfolio=h743-slim",
                 "Version": "3"
@@ -49,15 +50,15 @@
                 "URL": "https://www.diatone.us/products/mb-f45_128k-bl32-esc",
                 "Version": "1"
             }
         },
         "Flight Controller": {
             "Firmware": {
                 "Type": "ArduCopter",
-                "Version": "4.5.1"
+                "Version": "4.3.8"
             },
             "Notes": "This is a custom build with a Matek H743 SLIM flight controller. The board is a 20x20mm stackable board with a 400Mhz processor, 1Mb flash, 512kb RAM, and a 32-bit STM32H743 processor. The board has a built-in barometer, 6 UARTs, 8 PWM outputs, and 8 ADC inputs.",
             "Product": {
                 "Manufacturer": "Matek",
                 "Model": "H743 SLIM",
                 "URL": "https://www.mateksys.com/?portfolio=h743-slim",
                 "Version": "V3"
@@ -66,14 +67,18 @@
         "Frame": {
             "Notes": "A small 3'' ducted frame",
             "Product": {
                 "Manufacturer": "Diatone",
                 "Model": "Taycan MX-C",
                 "URL": "https://www.diatone.us/products/diatone-mxc-taycan-duct-3-inch-cinewhoop-fpv-drone",
                 "Version": "2022"
+            },
+            "Specifications": {
+                "TOW max Kg": 0.6,
+                "TOW min Kg": 0.6
             }
         },
         "GNSS receiver": {
             "FC Connection": {
                 "Protocol": "uBlox",
                 "Type": "SERIAL3"
             },
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/02_imu_temperature_calibration_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/03_imu_temperature_calibration_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/05_remote_controller.param`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ARMING_RUDDER,0  # We find it safer to use only a switch to arm instead of through rudder inputs
-BRD_ALT_CONFIG,1 # Matek H743-specific: Hardware-Pin Rx6 is Rx from UART 7
-RC_OPTIONS,288 # Enables Crossfire Telemetry
-RC_PROTOCOLS,512 # Deactivates all protocols except TBS Crossfire
-RC6_OPTION,153 # "Arm/Disarm", to use an arming switch (here Channel 6)
+BRD_ALT_CONFIG,1  # Matek H743-specific: Hardware-Pin Rx6 is Rx from UART 7
+RC_OPTIONS,288  # Enables Crossfire Telemetry
+RC_PROTOCOLS,512  # Selected in the component editor
+RC6_OPTION,153  # "Arm/Disarm", to use an arming switch (here Channel 6)
 RC7_OPTION,31  # "Motor Emergency Stop", stops all motors immediately at a high signal
 RC8_OPTION,30  # "Lost Copter Sound", generates a loud tone from the buzzer at a high signal to locate a lost multicopter
-RC9_OPTION,300 # Used to jump to the next waypoint
-RSSI_TYPE,3 # TBS Crossfire protocol provides RSSI
-SERIAL7_PROTOCOL,23 # Specifies the serial port 7 as RC-Input
+RC9_OPTION,300  # Used to jump to the next waypoint
+RSSI_TYPE,3  # TBS Crossfire protocol provides RSSI
+SERIAL7_PROTOCOL,23  # Specifies the serial port 7 as RC-Input
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/07_esc.param`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 ATC_RAT_PIT_SMAX,25  # limit the slew rate to prevent possible ESC desync - https://ardupilot.org/copter/docs/common-servo-limit-cycle-detection.html
 ATC_RAT_RLL_SMAX,25  # limit the slew rate to prevent possible ESC desync - https://ardupilot.org/copter/docs/common-servo-limit-cycle-detection.html
 ATC_RAT_YAW_SMAX,25  # limit the slew rate to prevent possible ESC desync - https://ardupilot.org/copter/docs/common-servo-limit-cycle-detection.html
-MOT_PWM_TYPE,6  # the most recomended speed for ArduCopter
+MOT_HOVER_LEARN,2  # So that it can tune the throttle controller on the 20_throttle_controller.param file
+MOT_PWM_MAX,2000
+MOT_PWM_MIN,1000
+MOT_PWM_TYPE,6  # Specified in component editor window
+MOT_SPOOL_TIME,0.5  # left at default because copter is small
 NTF_BUZZ_TYPES,3  # the 4-in-1 ESC uses this
 NTF_LED_TYPES,2369  # Built-in LED, NCP5623 External (Holybro F9P), Neopixel (Matek H743 slim v3), and DShot (4-in-1 ESC)
 PSC_ACCZ_SMAX,25  # limit the slew rate to prevent possible ESC desync - https://ardupilot.org/copter/docs/common-servo-limit-cycle-detection.html
 SERIAL5_BAUD,115  # bi-directional DShot telemetry data rate from T-Motor F45 4in1 ESC V2
 SERIAL5_PROTOCOL,16  # bi-directional DShot telemetry pin is connected to SERIAL5
 SERVO_BLH_AUTO,1  # Enables BLHeli pass-thru
 SERVO_BLH_BDMASK,15  # All four of our ESC support bi-directional DShot
@@ -23,7 +27,8 @@
 SERVO3_MAX,2000  # Use the full available 1000-2000 DShot range
 SERVO3_MIN,1000  # Use the full available 1000-2000 DShot range
 SERVO3_TRIM,1000  # Use the full available 1000-2000 DShot range
 SERVO4_MAX,2000  # Use the full available 1000-2000 DShot range
 SERVO4_MIN,1000  # Use the full available 1000-2000 DShot range
 SERVO4_TRIM,1000  # Use the full available 1000-2000 DShot range
 TKOFF_RPM_MIN,1400  # Our motors should idle at around 1400 RPM, see https://ardupilot.org/copter/docs/tkoff-rpm-min.html
+TKOFF_SLEW_TIME,2  # left at default because copter is small
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/09_batt2.param`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-BATT2_AMP_PERVLT,17.5
-BATT2_ARM_VOLT,15 # In our build this is a redundant monitor for batt1 so == BATT_ARM_VOLT
-BATT2_CAPACITY,1800 # In our build this is a redundant monitor for batt1 so == BATT_CAPACITY
-BATT2_CRT_MAH,450 # In our build this is a redundant monitor for batt1 so == BATT_CRT_MAH
-BATT2_CRT_VOLT,14 # In our build this is a redundant monitor for batt1 so == BATT_CRT_VOLT
+BATT2_AMP_PERVLT,17.73  # calibrated using batt charger
+BATT2_ARM_VOLT,15  # In our build this is a redundant monitor for batt1 so == BATT_ARM_VOLT
+BATT2_CAPACITY,1800  # In our build this is a redundant monitor for batt1 so == BATT_CAPACITY
+BATT2_CRT_MAH,450  # In our build this is a redundant monitor for batt1 so == BATT_CRT_MAH
+BATT2_CRT_VOLT,14  # In our build this is a redundant monitor for batt1 so == BATT_CRT_VOLT
 BATT2_CURR_PIN,7
-BATT2_FS_CRT_ACT,1  # flying indoors, just land ASAP, no need to hit the celing while doing RTL
-BATT2_FS_LOW_ACT,1  # flying indoors, just land ASAP, no need to hit the celing while doing RTL
+BATT2_FS_CRT_ACT,1  # flying indoors, just land ASAP, no need to hit the ceiling while doing RTL
+BATT2_FS_LOW_ACT,1  # flying indoors, just land ASAP, no need to hit the ceiling while doing RTL
 BATT2_FS_VOLTSRC,1  # In our build this is a redundant monitor for batt1 so == BATT_FS_VOLTSRC
 BATT2_LOW_MAH,600  # In our build this is a redundant monitor for batt1 so == BATT_LOW_MAH
 BATT2_LOW_VOLT,14.4  # In our build this is a redundant monitor for batt1 so == BATT_LOW_VOLT
 BATT2_MONITOR,4
-BATT2_VOLT_MULT,228.342 # Use a power source with a voltage close to BATT2_LOW_VOLT measure with a calibrated voltimeter and adapt this parameter so that the telemetry voltage reading matches it
+BATT2_VOLT_MULT,228.342  # Use a power source with a voltage close to BATT2_LOW_VOLT measure with a calibrated voltimeter and adapt this parameter so that the telemetry voltage reading matches it
 BATT2_VOLT_PIN,18
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/10_gnss.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_mp_setup_mandatory_hardware.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/12_mp_setup_mandatory_hardware.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_general_configuration.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/13_general_configuration.param`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-ARMING_CHECK,1  # perform all arming checks. If you have a problem fix it's source. Do NOT change this
+ARMING_CHECK,1  # Perform all arming checks. If you have a problem fix its source. Do NOT change this
 BRD_RTC_TZ_MIN,60  # Berlin time zone
 FENCE_TYPE,7  # cylinder and max altitude, to obey local regulations and safety measures
 INS_ACCEL_FILTER,10  # the default is 20 and that lets too much noise in
 INS_POS1_X,0  # was -0.005
 INS_POS1_Y,0  # was -0.011
 INS_POS2_X,0  # was -0.011
 INS_POS2_Y,0  # was -0.01
 LAND_ALT_LOW,200  # come down fast and only slow down close to the ground. We have a good GNSS receiver, so thrust it
 RTL_ALT,300  # The default is too high for the kind of flights we do. This reduces the altitude for indoors
 RTL_LOIT_TIME,1000  # The default is too long. This reduces the time
 SCHED_LOOP_RATE,800  # On our vehicle the propellers rotate at speeds higher than 400Hz and we have a powerful STM32 H7 family processor. So we increase this for added performance.
-SCR_ENABLE,1  # For VTOL-Quicktune, MagFit automation and Windspeed Estimation automation
+SCR_ENABLE,1  # Use lua scripting for VTOL-Quicktune, MagFit automation and Windspeed Estimation automation
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/16_pid_adjustment.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_pid_adjustment.param`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # If you have a very small, or a very large vehicle that requires non-default PID values for a safe flight, change them here
 #
 # Usually, smaller vehicles require lower than default PID rate values.
 # Larger vehicles usually require higher than default PID rate values.
 
+ATC_INPUT_TC,0.15
 ATC_RAT_PIT_D,0.003334  #  = 0.925972 * (0.0036 default)
 ATC_RAT_PIT_I,0.173229  #  = 1.283176 * (0.135 default)
 ATC_RAT_PIT_P,0.173229  #  = 1.283176 * (0.135 default)
 ATC_RAT_RLL_D,0.002486  #  = 0.690593 * (0.0036 default)
 ATC_RAT_RLL_I,0.143237  #  = 1.061015 * (0.135 default)
 ATC_RAT_RLL_P,0.143237  #  = 1.061015 * (0.135 default)
 ATC_RAT_YAW_D,0  #  = 1 * (0 default)
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/18_notch_filter_setup.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/18_notch_filter_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_inflight_magnetometer_fit_setup.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/24_inflight_magnetometer_fit_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_autotune_roll_pitch_retune_results.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/39_autotune_roll_pitch_retune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_roll.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/42_system_id_roll.param`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-ANGLE_MAX,1500  # limit the angle to limit the speed at SID-chirp low-frequencies
+ANGLE_MAX,2000  # limit the angle to limit the speed at SID-chirp low-frequencies
 ARMING_CHECK,540126  # disable Parameter check because we need to set ATC_RAT_RLL_I out-of-range (was 30175)
+ATC_ANG_PIT_P,4.5  # reset to default to not interfere with sysID
+ATC_ANG_RLL_P,4.5  # reset to default to not interfere with sysID
+ATC_ANG_YAW_P,4.5  # reset to default to not interfere with sysID
 ATC_RAT_RLL_I,0  # prevent the rate controllers from compensating too much of the frequency-sweep signal
 ATC_RATE_FF_ENAB,0  # prevent the rate controllers from compensating too much of the frequency-sweep signal
-FLTMODE5,25
+FLTMODE5,25  # Activate sysid instead of autotune
+LOG_BITMASK,176127  # attitude sample rate at loop rate
 LOG_DISARMED,0  # was only needed for wind speed estimation
 LOG_REPLAY,0  # was only needed for wind speed estimation
 SID_AXIS,10  # Inject chip on the mixer roll signal
 SID_F_START_HZ,0.05
 SID_F_STOP_HZ,5
 SID_MAGNITUDE,0.15
 SID_T_FADE_IN,5.0
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_everyday_use.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/50_everyday_use.param`

 * *Files 12% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 ATC_THR_MIX_MAX,0.7  # according to autotune documentation this should be raised up-to 0.9 after the tune
 BATT_FS_LOW_ACT,2  # outdoors we want the drone to come back
 BATT2_FS_LOW_ACT,2  # outdoors we want the drone to come back
-LOG_BITMASK,2241500 # 2:GPS,3:System Performance,4:Control Tuning,6:RC input,7:IMU,8:Mission Commands,9:Battery Monitor,12:PID,13:Compass,17:Motors,21:Fast harmonic notch logging
+LOG_BITMASK,144348  # 2:GPS,3:System Performance,4:Control Tuning,6:RC input,7:IMU,8:Mission Commands,9:Battery Monitor,12:PID,13:Compass,17:Motors
 RTL_ALT,500  # The default is too high for the kind of flights we do. This reduces the altitude for outdoors
 RTL_CLIMB_MIN,100  # always rise at least 1 meter as a visual indicator
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/48_position_controller.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/47_position_controller.param`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ANGLE_MAX,6500
+LOIT_ACC_MAX,500
 LOIT_BRK_ACCEL,500
 LOIT_BRK_DELAY,0.05
 LOIT_BRK_JERK,4000
 PSC_VELXY_FF,0.85  # PSCN.AE/PSCN.VE if you have flown North-South or PSCE.AE/PSCE.VE if you have flown East-West
 WPNAV_ACCEL,400  # high speed missions in auto
 WPNAV_ACCEL_C,800  # 2 * WPNAV_ACCEL so that the cornering behaviour is mostly controlled by WPNAV_RADIUS https://github.com/ArduPilot/ardupilot/pull/25928
 WPNAV_ACCEL_Z,200  # high speed missions in auto
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/49_precision_land.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/49_precision_land.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954788773148148%*

 * *Differences: {"'Components'": "{'Flight Controller': {'Firmware': {'Version': '4.6.0-DEV'}}, 'Frame': "*

 * *                 "{'Specifications': OrderedDict([('TOW min Kg', 0.6), ('TOW max Kg', 0.6)])}, "*

 * *                 "'Battery Monitor': {'Firmware': {'Version': '4.6.0-DEV'}}, 'Battery': "*

 * *                 "{'Specifications': {'Capacity mAh': 1800}}}"}*

```diff
@@ -5,29 +5,30 @@
             "Product": {
                 "Manufacturer": "SLS",
                 "Model": "X-Cube 1800mAh 4S1P 14,8V 40C/80C",
                 "URL": "https://www.stefansliposhop.de/akkus/sls-x-cube/sls-x-cube-40c/sls-x-cube-1800mah-4s1p-14-8v-40c-80c::1568.html",
                 "Version": ""
             },
             "Specifications": {
+                "Capacity mAh": 1800,
                 "Chemistry": "Lipo",
                 "Number of cells": 4,
                 "Volt per cell crit": 3.55,
                 "Volt per cell low": 3.6,
                 "Volt per cell max": 4.2
             }
         },
         "Battery Monitor": {
             "FC Connection": {
                 "Protocol": "Analog Voltage and Current",
                 "Type": "Analog"
             },
             "Firmware": {
                 "Type": "ArduCopter",
-                "Version": "4.5.1"
+                "Version": "4.6.0-DEV"
             },
             "Notes": "Voltage is done via the flight controller. Current is done via the ESC.",
             "Product": {
                 "Manufacturer": "Matek",
                 "Model": "H743 SLIM",
                 "URL": "https://www.mateksys.com/?portfolio=h743-slim",
                 "Version": "3"
@@ -49,15 +50,15 @@
                 "URL": "https://www.diatone.us/products/mb-f45_128k-bl32-esc",
                 "Version": "1"
             }
         },
         "Flight Controller": {
             "Firmware": {
                 "Type": "ArduCopter",
-                "Version": "4.5.1"
+                "Version": "4.6.0-DEV"
             },
             "Notes": "This is a custom build with a Matek H743 SLIM flight controller. The board is a 20x20mm stackable board with a 400Mhz processor, 1Mb flash, 512kb RAM, and a 32-bit STM32H743 processor. The board has a built-in barometer, 6 UARTs, 8 PWM outputs, and 8 ADC inputs.",
             "Product": {
                 "Manufacturer": "Matek",
                 "Model": "H743 SLIM",
                 "URL": "https://www.mateksys.com/?portfolio=h743-slim",
                 "Version": "V3"
@@ -66,14 +67,18 @@
         "Frame": {
             "Notes": "A small 3'' ducted frame",
             "Product": {
                 "Manufacturer": "Diatone",
                 "Model": "Taycan MX-C",
                 "URL": "https://www.diatone.us/products/diatone-mxc-taycan-duct-3-inch-cinewhoop-fpv-drone",
                 "Version": "2022"
+            },
+            "Specifications": {
+                "TOW max Kg": 0.6,
+                "TOW min Kg": 0.6
             }
         },
         "GNSS receiver": {
             "FC Connection": {
                 "Protocol": "uBlox",
                 "Type": "SERIAL3"
             },
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/00_default.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/00_default.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/02_imu_temperature_calibration_setup.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/03_imu_temperature_calibration_results.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/05_remote_controller.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/05_remote_controller.param`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ARMING_RUDDER,0  # We find it safer to use only a switch to arm instead of through rudder inputs
-BRD_ALT_CONFIG,1 # Matek H743-specific: Hardware-Pin Rx6 is Rx from UART 7
-RC_OPTIONS,288 # Enables Crossfire Telemetry
-RC_PROTOCOLS,512 # Deactivates all protocols except TBS Crossfire
-RC6_OPTION,153 # "Arm/Disarm", to use an arming switch (here Channel 6)
+BRD_ALT_CONFIG,1  # Matek H743-specific: Hardware-Pin Rx6 is Rx from UART 7
+RC_OPTIONS,288  # Enables Crossfire Telemetry
+RC_PROTOCOLS,512  # Selected in the component editor
+RC6_OPTION,153  # "Arm/Disarm", to use an arming switch (here Channel 6)
 RC7_OPTION,31  # "Motor Emergency Stop", stops all motors immediately at a high signal
 RC8_OPTION,30  # "Lost Copter Sound", generates a loud tone from the buzzer at a high signal to locate a lost multicopter
-RC9_OPTION,300 # Used to jump to the next waypoint
-RSSI_TYPE,3 # TBS Crossfire protocol provides RSSI
-SERIAL7_PROTOCOL,23 # Specifies the serial port 7 as RC-Input
+RC9_OPTION,300  # Used to jump to the next waypoint
+RSSI_TYPE,3  # TBS Crossfire protocol provides RSSI
+SERIAL7_PROTOCOL,23  # Specifies the serial port 7 as RC-Input
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/07_esc.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/07_esc.param`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 ATC_RAT_PIT_SMAX,25  # limit the slew rate to prevent possible ESC desync - https://ardupilot.org/copter/docs/common-servo-limit-cycle-detection.html
 ATC_RAT_RLL_SMAX,25  # limit the slew rate to prevent possible ESC desync - https://ardupilot.org/copter/docs/common-servo-limit-cycle-detection.html
 ATC_RAT_YAW_SMAX,25  # limit the slew rate to prevent possible ESC desync - https://ardupilot.org/copter/docs/common-servo-limit-cycle-detection.html
-MOT_PWM_TYPE,6  # the most recomended speed for ArduCopter
+MOT_HOVER_LEARN,2  # So that it can tune the throttle controller on the 20_throttle_controller.param file
+MOT_PWM_MAX,2000
+MOT_PWM_MIN,1000
+MOT_PWM_TYPE,6  # Specified in component editor window
+MOT_SPOOL_TIME,0.5  # left at default because copter is small
 NTF_BUZZ_TYPES,3  # the 4-in-1 ESC uses this
 NTF_LED_TYPES,2369  # Built-in LED, NCP5623 External (Holybro F9P), Neopixel (Matek H743 slim v3), and DShot (4-in-1 ESC)
 PSC_ACCZ_SMAX,25  # limit the slew rate to prevent possible ESC desync - https://ardupilot.org/copter/docs/common-servo-limit-cycle-detection.html
 SERIAL5_BAUD,115  # bi-directional DShot telemetry data rate from T-Motor F45 4in1 ESC V2
 SERIAL5_PROTOCOL,16  # bi-directional DShot telemetry pin is connected to SERIAL5
 SERVO_BLH_AUTO,1  # Enables BLHeli pass-thru
 SERVO_BLH_BDMASK,15  # All four of our ESC support bi-directional DShot
@@ -23,8 +27,8 @@
 SERVO3_MAX,2000  # Use the full available 1000-2000 DShot range
 SERVO3_MIN,1000  # Use the full available 1000-2000 DShot range
 SERVO3_TRIM,1000  # Use the full available 1000-2000 DShot range
 SERVO4_MAX,2000  # Use the full available 1000-2000 DShot range
 SERVO4_MIN,1000  # Use the full available 1000-2000 DShot range
 SERVO4_TRIM,1000  # Use the full available 1000-2000 DShot range
 TKOFF_RPM_MIN,1400  # Our motors should idle at around 1400 RPM, see https://ardupilot.org/copter/docs/tkoff-rpm-min.html
-MOT_HOVER_LEARN,2
+TKOFF_SLEW_TIME,2  # left at default because copter is small
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/09_batt2.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/09_batt2.param`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-BATT2_AMP_PERVLT,17.5
-BATT2_ARM_VOLT,15 # In our build this is a redundant monitor for batt1 so == BATT_ARM_VOLT
-BATT2_CAPACITY,1800 # In our build this is a redundant monitor for batt1 so == BATT_CAPACITY
-BATT2_CRT_MAH,450 # In our build this is a redundant monitor for batt1 so == BATT_CRT_MAH
-BATT2_CRT_VOLT,14 # In our build this is a redundant monitor for batt1 so == BATT_CRT_VOLT
+BATT2_AMP_PERVLT,17.73  # calibrated using batt charger
+BATT2_ARM_VOLT,15  # In our build this is a redundant monitor for batt1 so == BATT_ARM_VOLT
+BATT2_CAPACITY,1800  # In our build this is a redundant monitor for batt1 so == BATT_CAPACITY
+BATT2_CRT_MAH,450  # In our build this is a redundant monitor for batt1 so == BATT_CRT_MAH
+BATT2_CRT_VOLT,14  # In our build this is a redundant monitor for batt1 so == BATT_CRT_VOLT
 BATT2_CURR_PIN,7
-BATT2_FS_CRT_ACT,1  # flying indoors, just land ASAP, no need to hit the celing while doing RTL
-BATT2_FS_LOW_ACT,1  # flying indoors, just land ASAP, no need to hit the celing while doing RTL
+BATT2_FS_CRT_ACT,1  # flying indoors, just land ASAP, no need to hit the ceiling while doing RTL
+BATT2_FS_LOW_ACT,1  # flying indoors, just land ASAP, no need to hit the ceiling while doing RTL
 BATT2_FS_VOLTSRC,1  # In our build this is a redundant monitor for batt1 so == BATT_FS_VOLTSRC
 BATT2_LOW_MAH,600  # In our build this is a redundant monitor for batt1 so == BATT_LOW_MAH
 BATT2_LOW_VOLT,14.4  # In our build this is a redundant monitor for batt1 so == BATT_LOW_VOLT
 BATT2_MONITOR,4
-BATT2_VOLT_MULT,228.342 # Use a power source with a voltage close to BATT2_LOW_VOLT measure with a calibrated voltimeter and adapt this parameter so that the telemetry voltage reading matches it
+BATT2_VOLT_MULT,228.342  # Use a power source with a voltage close to BATT2_LOW_VOLT measure with a calibrated voltimeter and adapt this parameter so that the telemetry voltage reading matches it
 BATT2_VOLT_PIN,18
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/10_gnss.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/10_gnss.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/12_mp_setup_mandatory_hardware.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/12_mp_setup_mandatory_hardware.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/13_general_configuration.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/13_general_configuration.param`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-ARMING_CHECK,1  # perform all arming checks. If you have a problem fix it's source. Do NOT change this
+ARMING_CHECK,1  # Perform all arming checks. If you have a problem fix its source. Do NOT change this
 BRD_RTC_TZ_MIN,60  # Berlin time zone
 FENCE_TYPE,7  # cylinder and max altitude, to obey local regulations and safety measures
 INS_ACCEL_FILTER,10  # the default is 20 and that lets too much noise in
 INS_POS1_X,0  # was -0.005
 INS_POS1_Y,0  # was -0.011
 INS_POS2_X,0  # was -0.011
 INS_POS2_Y,0  # was -0.01
 LAND_ALT_LOW,200  # come down fast and only slow down close to the ground. We have a good GNSS receiver, so thrust it
 RTL_ALT,300  # The default is too high for the kind of flights we do. This reduces the altitude for indoors
 RTL_LOIT_TIME,1000  # The default is too long. This reduces the time
 SCHED_LOOP_RATE,800  # On our vehicle the propellers rotate at speeds higher than 400Hz and we have a powerful STM32 H7 family processor. So we increase this for added performance.
-SCR_ENABLE,1  # For VTOL-Quicktune, MagFit automation and Windspeed Estimation automation
+SCR_ENABLE,1  # Use lua scripting for VTOL-Quicktune, MagFit automation and Windspeed Estimation automation
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/16_pid_adjustment.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/16_pid_adjustment.param`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# If you have a very small, or a very large vehicle that requires non-default PID values for a safe flight, change them here
-#
-# Usually, smaller vehicles require lower than default PID rate values.
-# Larger vehicles usually require higher than default PID rate values.
-
-ATC_RAT_PIT_D,0.003334  #  = 0.925972 * (0.0036 default)
-ATC_RAT_PIT_I,0.173229  #  = 1.283176 * (0.135 default)
-ATC_RAT_PIT_P,0.173229  #  = 1.283176 * (0.135 default)
-ATC_RAT_RLL_D,0.002486  #  = 0.690593 * (0.0036 default)
-ATC_RAT_RLL_I,0.143237  #  = 1.061015 * (0.135 default)
-ATC_RAT_RLL_P,0.143237  #  = 1.061015 * (0.135 default)
-ATC_RAT_YAW_D,0  #  = 1 * (0 default)
-ATC_RAT_YAW_I,0.045252  #  = 2.514026 * (0.018 default)
-ATC_RAT_YAW_P,0.452525  #  = 2.514026 * (0.18 default)
+# If you have a very small, or a very large vehicle that requires non-default PID values for a safe flight, change them here
+#
+# Usually, smaller vehicles require lower than default PID rate values.
+# Larger vehicles usually require higher than default PID rate values.
+
+ATC_INPUT_TC,0.15
+ATC_RAT_PIT_D,0.003334  #  = 0.925972 * (0.0036 default)
+ATC_RAT_PIT_I,0.173229  #  = 1.283176 * (0.135 default)
+ATC_RAT_PIT_P,0.173229  #  = 1.283176 * (0.135 default)
+ATC_RAT_RLL_D,0.002486  #  = 0.690593 * (0.0036 default)
+ATC_RAT_RLL_I,0.143237  #  = 1.061015 * (0.135 default)
+ATC_RAT_RLL_P,0.143237  #  = 1.061015 * (0.135 default)
+ATC_RAT_YAW_D,0  #  = 1 * (0 default)
+ATC_RAT_YAW_I,0.045252  #  = 2.514026 * (0.018 default)
+ATC_RAT_YAW_P,0.452525  #  = 2.514026 * (0.18 default)
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/18_notch_filter_setup.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/24_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/24_inflight_magnetometer_fit_setup.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_inflight_magnetometer_fit_setup.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/39_autotune_roll_pitch_retune_results.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/39_autotune_roll_pitch_retune_results.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/42_system_id_roll.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/42_system_id_roll.param`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-ANGLE_MAX,1500  # limit the angle to limit the speed at SID-chirp low-frequencies
+ANGLE_MAX,2000  # limit the angle to limit the speed at SID-chirp low-frequencies
 ARMING_CHECK,540126  # disable Parameter check because we need to set ATC_RAT_RLL_I out-of-range (was 30175)
+ATC_ANG_PIT_P,4.5  # reset to default to not interfere with sysID
+ATC_ANG_RLL_P,4.5  # reset to default to not interfere with sysID
+ATC_ANG_YAW_P,4.5  # reset to default to not interfere with sysID
 ATC_RAT_RLL_I,0  # prevent the rate controllers from compensating too much of the frequency-sweep signal
 ATC_RATE_FF_ENAB,0  # prevent the rate controllers from compensating too much of the frequency-sweep signal
-FLTMODE5,25
+FLTMODE5,25  # Activate sysid instead of autotune
+LOG_BITMASK,176127  # attitude sample rate at loop rate
 LOG_DISARMED,0  # was only needed for wind speed estimation
 LOG_REPLAY,0  # was only needed for wind speed estimation
 SID_AXIS,10  # Inject chip on the mixer roll signal
 SID_F_START_HZ,0.05
 SID_F_STOP_HZ,5
 SID_MAGNITUDE,0.15
 SID_T_FADE_IN,5.0
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/47_everyday_use.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/50_everyday_use.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/48_position_controller.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_position_controller.param`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ANGLE_MAX,6500
+LOIT_ACC_MAX,500
 LOIT_BRK_ACCEL,500
 LOIT_BRK_DELAY,0.05
 LOIT_BRK_JERK,4000
 PSC_VELXY_FF,0.85  # PSCN.AE/PSCN.VE if you have flown North-South or PSCE.AE/PSCE.VE if you have flown East-West
 WPNAV_ACCEL,400  # high speed missions in auto
 WPNAV_ACCEL_C,800  # 2 * WPNAV_ACCEL so that the cornering behaviour is mostly controlled by WPNAV_RADIUS https://github.com/ArduPilot/ardupilot/pull/25928
 WPNAV_ACCEL_Z,200  # high speed missions in auto
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/49_precision_land.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/49_precision_land.param`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/apm.pdef.xml`

 * *Files 0% similar despite different names*

#### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/apm.pdef.xml` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/apm.pdef.xml`

```diff
@@ -1,9 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- Dynamically generated list of documented parameters (generated by param_parse.py) -->
+<!-- Generated from git tag Copter-4.5.3 on 2024-05-30 14:47:49 -->
 <paramfile>
   <vehicles>
     <parameters name="ArduCopter">
       <param humanName="Eeprom format version number" name="ArduCopter:FORMAT_VERSION" documentation="This value is incremented when changes are made to the eeprom format" user="Advanced">
         <field name="ReadOnly">True</field>
       </param>
       <param humanName="MAVLink system ID of this vehicle" name="ArduCopter:SYSID_THISMAV" documentation="Allows setting an individual MAVLink system id for this vehicle to distinguish it from others on the same network" user="Advanced">
@@ -1934,14 +1935,20 @@
         </values>
       </param>
       <param humanName="Compass magnetic field strength error threshold vs earth magnetic model" name="ARMING_MAGTHRESH" documentation="Compass magnetic field strength error threshold vs earth magnetic model.  X and y axis are compared using this threhold, Z axis uses 2x this threshold.  0 to disable check" user="Advanced">
         <field name="Units">mGauss</field>
         <field name="UnitText">milligauss</field>
         <field name="Range">0 500</field>
       </param>
+      <param humanName="Disable CrashDump Arming check" name="ARMING_CRSDP_IGN" documentation="Must have value &quot;1&quot; if crashdump data is present on the system, or a prearm failure will be raised.  Do not set this parameter unless the risks of doing so are fully understood.  The presence of a crash dump means that the firmware currently installed has suffered a critical software failure which resulted in the autopilot immediately rebooting.  The crashdump file gives diagnostic information which can help in finding the issue, please contact the ArduPIlot support team.  If this crashdump data is present, the vehicle is likely unsafe to fly.  Check the ArduPilot documentation for more details." user="Advanced">
+        <values>
+          <value code="0">Crash Dump arming check active</value>
+          <value code="1">Crash Dump arming check deactivated</value>
+        </values>
+      </param>
     </parameters>
     <parameters name="AROT_">
       <param humanName="Enable settings for RSC Setpoint" name="AROT_ENABLE" documentation="Allows you to enable (1) or disable (0) the autonomous autorotation capability." user="Advanced">
         <values>
           <value code="0">Disabled</value>
           <value code="1">Enabled</value>
         </values>
@@ -2763,15 +2770,15 @@
       </param>
       <param humanName="Avoidance behaviour" name="AVOID_BEHAVE" documentation="Avoidance behaviour (slide or stop)" user="Standard">
         <values>
           <value code="0">Slide</value>
           <value code="1">Stop</value>
         </values>
       </param>
-      <param humanName="Avoidance maximum backup speed" name="AVOID_BACKUP_SPD" documentation="Maximum speed that will be used to back away from obstacles in GPS modes (m/s). Set zero to disable" user="Standard">
+      <param humanName="Avoidance maximum horizontal backup speed" name="AVOID_BACKUP_SPD" documentation="Maximum speed that will be used to back away from obstacles horizontally in position control modes (m/s). Set zero to disable horizontal backup." user="Standard">
         <field name="Units">m/s</field>
         <field name="UnitText">meters per second</field>
         <field name="Range">0 2</field>
       </param>
       <param humanName="Avoidance minimum altitude" name="AVOID_ALT_MIN" documentation="Minimum altitude above which proximity based avoidance will start working. This requires a valid downward facing rangefinder reading to work. Set zero to disable" user="Standard">
         <field name="Units">m</field>
         <field name="UnitText">meters</field>
@@ -2783,14 +2790,19 @@
         <field name="Range">0 9</field>
       </param>
       <param humanName="Avoidance deadzone between stopping and backing away from obstacle" name="AVOID_BACKUP_DZ" documentation="Distance beyond AVOID_MARGIN parameter, after which vehicle will backaway from obstacles. Increase this parameter if you see vehicle going back and forth in front of obstacle." user="Standard">
         <field name="Units">m</field>
         <field name="UnitText">meters</field>
         <field name="Range">0 2</field>
       </param>
+      <param humanName="Avoidance maximum vertical backup speed" name="AVOID_BACKZ_SPD" documentation="Maximum speed that will be used to back away from obstacles vertically in height control modes (m/s). Set zero to disable vertical backup." user="Standard">
+        <field name="Units">m/s</field>
+        <field name="UnitText">meters per second</field>
+        <field name="Range">0 2</field>
+      </param>
     </parameters>
     <parameters name="BARO">
       <param humanName="Ground Pressure" name="BARO1_GND_PRESS" documentation="calibrated ground pressure in Pascals" user="Advanced">
         <field name="Units">Pa</field>
         <field name="UnitText">pascal</field>
         <field name="Increment">1</field>
         <field name="ReadOnly">True</field>
@@ -6916,14 +6928,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -7034,14 +7047,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -7152,14 +7166,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -7270,14 +7285,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -12994,14 +13010,17 @@
         <field name="Range">0.0 0.2</field>
         <field name="Increment">.005</field>
       </param>
       <param humanName="Mount Target sysID" name="MNT1_SYSID_DFLT" documentation="Default Target sysID for the mount to point to" user="Standard">
         <field name="RebootRequired">True</field>
       </param>
       <param humanName="Mount Device ID" name="MNT1_DEVID" documentation="Mount device ID, taking into account its type, bus and instance" user="Advanced"/>
+      <param humanName="Mount options" name="MNT1_OPTIONS" documentation="Mount options bitmask" user="Standard">
+        <field name="Bitmask">0:RC lock state from previous mode</field>
+      </param>
     </parameters>
     <parameters name="MNT2">
       <param humanName="Mount Type" name="MNT2_TYPE" documentation="Mount Type" user="Standard">
         <values>
           <value code="0">None</value>
           <value code="1">Servo</value>
           <value code="2">3DR Solo</value>
@@ -13118,14 +13137,17 @@
         <field name="Range">0.0 0.2</field>
         <field name="Increment">.005</field>
       </param>
       <param humanName="Mount Target sysID" name="MNT2_SYSID_DFLT" documentation="Default Target sysID for the mount to point to" user="Standard">
         <field name="RebootRequired">True</field>
       </param>
       <param humanName="Mount Device ID" name="MNT2_DEVID" documentation="Mount device ID, taking into account its type, bus and instance" user="Advanced"/>
+      <param humanName="Mount options" name="MNT2_OPTIONS" documentation="Mount options bitmask" user="Standard">
+        <field name="Bitmask">0:RC lock state from previous mode</field>
+      </param>
     </parameters>
     <parameters name="MOT_">
       <param humanName="Matrix Yaw Min" name="MOT_YAW_HEADROOM" documentation="Yaw control is given at least this pwm in microseconds range" user="Advanced">
         <field name="Range">0 500</field>
         <field name="Units">PWM</field>
         <field name="UnitText">PWM in microseconds</field>
       </param>
@@ -18184,14 +18206,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -18333,14 +18356,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -18482,14 +18506,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -18631,14 +18656,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -18780,14 +18806,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -18929,14 +18956,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -19078,14 +19106,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -19227,14 +19256,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -19376,14 +19406,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -19525,14 +19556,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -19674,14 +19706,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -19823,14 +19856,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -19972,14 +20006,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -20121,14 +20156,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -20270,14 +20306,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
@@ -20419,14 +20456,15 @@
           <value code="110">KillIMU3</value>
           <value code="18">LAND Mode</value>
           <value code="56">LOITER Mode</value>
           <value code="29">Landing Gear</value>
           <value code="30">Lost Copter Sound</value>
           <value code="31">Motor Emergency Stop</value>
           <value code="32">Motor Interlock</value>
+          <value code="177">Mount LRF enable</value>
           <value code="163">Mount Lock</value>
           <value code="213">Mount1 Pitch</value>
           <value code="212">Mount1 Roll</value>
           <value code="214">Mount1 Yaw</value>
           <value code="216">Mount2 Pitch</value>
           <value code="215">Mount2 Roll</value>
           <value code="217">Mount2 Yaw</value>
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle.jpg` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.1-params/vehicle_components.json` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.4.4-params/vehicle_components.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954788773148148%*

 * *Differences: {"'Components'": "{'Flight Controller': {'Firmware': {'Version': '4.4.4'}}, 'Frame': "*

 * *                 "{'Specifications': OrderedDict([('TOW min Kg', 0.6), ('TOW max Kg', 0.6)])}, "*

 * *                 "'Battery Monitor': {'Firmware': {'Version': '4.4.4'}}, 'Battery': "*

 * *                 "{'Specifications': {'Capacity mAh': 1800}}}"}*

```diff
@@ -5,29 +5,30 @@
             "Product": {
                 "Manufacturer": "SLS",
                 "Model": "X-Cube 1800mAh 4S1P 14,8V 40C/80C",
                 "URL": "https://www.stefansliposhop.de/akkus/sls-x-cube/sls-x-cube-40c/sls-x-cube-1800mah-4s1p-14-8v-40c-80c::1568.html",
                 "Version": ""
             },
             "Specifications": {
+                "Capacity mAh": 1800,
                 "Chemistry": "Lipo",
                 "Number of cells": 4,
                 "Volt per cell crit": 3.55,
                 "Volt per cell low": 3.6,
                 "Volt per cell max": 4.2
             }
         },
         "Battery Monitor": {
             "FC Connection": {
                 "Protocol": "Analog Voltage and Current",
                 "Type": "Analog"
             },
             "Firmware": {
                 "Type": "ArduCopter",
-                "Version": "4.5.1"
+                "Version": "4.4.4"
             },
             "Notes": "Voltage is done via the flight controller. Current is done via the ESC.",
             "Product": {
                 "Manufacturer": "Matek",
                 "Model": "H743 SLIM",
                 "URL": "https://www.mateksys.com/?portfolio=h743-slim",
                 "Version": "3"
@@ -49,15 +50,15 @@
                 "URL": "https://www.diatone.us/products/mb-f45_128k-bl32-esc",
                 "Version": "1"
             }
         },
         "Flight Controller": {
             "Firmware": {
                 "Type": "ArduCopter",
-                "Version": "4.5.1"
+                "Version": "4.4.4"
             },
             "Notes": "This is a custom build with a Matek H743 SLIM flight controller. The board is a 20x20mm stackable board with a 400Mhz processor, 1Mb flash, 512kb RAM, and a 32-bit STM32H743 processor. The board has a built-in barometer, 6 UARTs, 8 PWM outputs, and 8 ADC inputs.",
             "Product": {
                 "Manufacturer": "Matek",
                 "Model": "H743 SLIM",
                 "URL": "https://www.mateksys.com/?portfolio=h743-slim",
                 "Version": "V3"
@@ -66,14 +67,18 @@
         "Frame": {
             "Notes": "A small 3'' ducted frame",
             "Product": {
                 "Manufacturer": "Diatone",
                 "Model": "Taycan MX-C",
                 "URL": "https://www.diatone.us/products/diatone-mxc-taycan-duct-3-inch-cinewhoop-fpv-drone",
                 "Version": "2022"
+            },
+            "Specifications": {
+                "TOW max Kg": 0.6,
+                "TOW min Kg": 0.6
             }
         },
         "GNSS receiver": {
             "FC Connection": {
                 "Protocol": "uBlox",
                 "Type": "SERIAL3"
             },
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/02_imu_temperature_calibration_setup.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/02_imu_temperature_calibration_setup.param`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-INS_LOG_BAT_MASK,3 # the Matek H743 fligth controller only has two IMUs
-INS_TCAL1_ENABLE,2 # Activates the temperature calibration for IMU 1 at the next start
-INS_TCAL1_TMAX,60 # our H7 processor acts as a heater and heats up the board to almost 60 deg
-INS_TCAL2_ENABLE,2 # Activates the temperature calibration for IMU 2 at the next start
-INS_TCAL2_TMAX,60 # our H7 processor acts as a heater and heats up the board to almost 60 deg
-LOG_BITMASK,524416 # Only for IMU and Raw-IMU
-LOG_DISARMED,1 # to gather data for the offline IMU temperature compensation while the FC is disarmed
+INS_LOG_BAT_MASK,3  # the Matek H743 fligth controller only has two IMUs
+INS_TCAL1_ENABLE,2  # Activates the temperature calibration for IMU 1 at the next start
+INS_TCAL1_TMAX,60  # our H7 processor acts as a heater and heats up the board to almost 60 deg
+INS_TCAL2_ENABLE,2  # Activates the temperature calibration for IMU 2 at the next start
+INS_TCAL2_TMAX,60  # our H7 processor acts as a heater and heats up the board to almost 60 deg
+LOG_BITMASK,524416  # Only for IMU and Raw-IMU
+LOG_DISARMED,1  # Gather data for the offline IMU temperature compensation while the FC is disarmed
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/03_imu_temperature_calibration_results.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/03_imu_temperature_calibration_results.param`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-INS_TCAL1_ACC1_X 115.946591342
-INS_TCAL1_ACC1_Y 498.256973344
-INS_TCAL1_ACC1_Z -381.446151984
-INS_TCAL1_ACC2_X -22.931568706
-INS_TCAL1_ACC2_Y 13.578689275
-INS_TCAL1_ACC2_Z 19.361290207
-INS_TCAL1_ACC3_X -0.601406268
-INS_TCAL1_ACC3_Y 0.213798686
-INS_TCAL1_ACC3_Z 0.011621521
-INS_TCAL1_ENABLE 1
-INS_TCAL1_GYR1_X -32.634220542
-INS_TCAL1_GYR1_Y 79.655005221
-INS_TCAL1_GYR1_Z -151.124203469
-INS_TCAL1_GYR2_X -0.611429461
-INS_TCAL1_GYR2_Y -2.040988991
-INS_TCAL1_GYR2_Z 1.238329627
-INS_TCAL1_GYR3_X -0.009728067
-INS_TCAL1_GYR3_Y 0.019491833
-INS_TCAL1_GYR3_Z 0.001409968
-INS_TCAL1_TMAX 56.0
-INS_TCAL1_TMIN -14.6
-INS_TCAL2_ACC1_X -1088.415600440
-INS_TCAL2_ACC1_Y 806.840522393
-INS_TCAL2_ACC1_Z 327.521202466
-INS_TCAL2_ACC2_X -13.630366124
-INS_TCAL2_ACC2_Y 6.347960639
-INS_TCAL2_ACC2_Z 9.967253125
-INS_TCAL2_ACC3_X -0.376738491
-INS_TCAL2_ACC3_Y 0.002642167
-INS_TCAL2_ACC3_Z -0.065860983
-INS_TCAL2_ENABLE 1
-INS_TCAL2_GYR1_X -44.455145632
-INS_TCAL2_GYR1_Y -8.833005619
-INS_TCAL2_GYR1_Z 88.004538868
-INS_TCAL2_GYR2_X 1.435061412
-INS_TCAL2_GYR2_Y -0.204452936
-INS_TCAL2_GYR2_Z -2.086231519
-INS_TCAL2_GYR3_X -0.048140576
-INS_TCAL2_GYR3_Y -0.002372842
-INS_TCAL2_GYR3_Z -0.028350688
-INS_TCAL2_TMAX 56.5
-INS_TCAL2_TMIN -13.3
+INS_TCAL1_ACC1_X 115.946591342
+INS_TCAL1_ACC1_Y 498.256973344
+INS_TCAL1_ACC1_Z -381.446151984
+INS_TCAL1_ACC2_X -22.931568706
+INS_TCAL1_ACC2_Y 13.578689275
+INS_TCAL1_ACC2_Z 19.361290207
+INS_TCAL1_ACC3_X -0.601406268
+INS_TCAL1_ACC3_Y 0.213798686
+INS_TCAL1_ACC3_Z 0.011621521
+INS_TCAL1_ENABLE 1
+INS_TCAL1_GYR1_X -32.634220542
+INS_TCAL1_GYR1_Y 79.655005221
+INS_TCAL1_GYR1_Z -151.124203469
+INS_TCAL1_GYR2_X -0.611429461
+INS_TCAL1_GYR2_Y -2.040988991
+INS_TCAL1_GYR2_Z 1.238329627
+INS_TCAL1_GYR3_X -0.009728067
+INS_TCAL1_GYR3_Y 0.019491833
+INS_TCAL1_GYR3_Z 0.001409968
+INS_TCAL1_TMAX 56.0
+INS_TCAL1_TMIN -14.6
+INS_TCAL2_ACC1_X -1088.415600440
+INS_TCAL2_ACC1_Y 806.840522393
+INS_TCAL2_ACC1_Z 327.521202466
+INS_TCAL2_ACC2_X -13.630366124
+INS_TCAL2_ACC2_Y 6.347960639
+INS_TCAL2_ACC2_Z 9.967253125
+INS_TCAL2_ACC3_X -0.376738491
+INS_TCAL2_ACC3_Y 0.002642167
+INS_TCAL2_ACC3_Z -0.065860983
+INS_TCAL2_ENABLE 1
+INS_TCAL2_GYR1_X -44.455145632
+INS_TCAL2_GYR1_Y -8.833005619
+INS_TCAL2_GYR1_Z 88.004538868
+INS_TCAL2_GYR2_X 1.435061412
+INS_TCAL2_GYR2_Y -0.204452936
+INS_TCAL2_GYR2_Z -2.086231519
+INS_TCAL2_GYR3_X -0.048140576
+INS_TCAL2_GYR3_Y -0.002372842
+INS_TCAL2_GYR3_Z -0.028350688
+INS_TCAL2_TMAX 56.5
+INS_TCAL2_TMIN -13.3
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/05_remote_controller.param`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 ARMING_RUDDER,0  # We find it safer to use only a switch to arm instead of through rudder inputs
-BRD_ALT_CONFIG,1 # Matek H743-specific: Hardware-Pin Rx6 is Rx from UART 7
-RC_OPTIONS,288 # Enables Crossfire Telemetry
-RC_PROTOCOLS,512 # Deactivates all protocols except TBS Crossfire
-RC6_OPTION,153 # "Arm/Disarm", to use an arming switch (here Channel 6)
+BRD_ALT_CONFIG,1  # Matek H743-specific: Hardware-Pin Rx6 is Rx from UART 7
+RC_OPTIONS,288  # Enables Crossfire Telemetry
+RC_PROTOCOLS,512  # Selected in the component editor
+RC6_OPTION,153  # "Arm/Disarm", to use an arming switch (here Channel 6)
 RC7_OPTION,31  # "Motor Emergency Stop", stops all motors immediately at a high signal
 RC8_OPTION,30  # "Lost Copter Sound", generates a loud tone from the buzzer at a high signal to locate a lost multicopter
-RC9_OPTION,300 # Used to jump to the next waypoint
-RSSI_TYPE,3 # TBS Crossfire protocol provides RSSI
-SERIAL2_BAUD,115 # For Mavlink over crossfire
-SERIAL7_PROTOCOL,23 # Specifies the serial port 7 as RC-Input
+RC9_OPTION,300  # Used to jump to the next waypoint
+RSSI_TYPE,3  # TBS Crossfire protocol provides RSSI
+SERIAL7_PROTOCOL,23  # Specifies the serial port 7 as RC-Input
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/09_batt2.param`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-BATT2_AMP_PERVLT,17.5
-BATT2_ARM_VOLT,15 # In our build this is a redundant monitor for batt1 so == BATT_ARM_VOLT
-BATT2_CAPACITY,1800 # In our build this is a redundant monitor for batt1 so == BATT_CAPACITY
-BATT2_CRT_MAH,450 # In our build this is a redundant monitor for batt1 so == BATT_CRT_MAH
-BATT2_CRT_VOLT,14 # In our build this is a redundant monitor for batt1 so == BATT_CRT_VOLT
+BATT2_AMP_PERVLT,17.73  # calibrated using batt charger
+BATT2_ARM_VOLT,15  # In our build this is a redundant monitor for batt1 so == BATT_ARM_VOLT
+BATT2_CAPACITY,1800  # In our build this is a redundant monitor for batt1 so == BATT_CAPACITY
+BATT2_CRT_MAH,450  # In our build this is a redundant monitor for batt1 so == BATT_CRT_MAH
+BATT2_CRT_VOLT,14  # In our build this is a redundant monitor for batt1 so == BATT_CRT_VOLT
 BATT2_CURR_PIN,7
-BATT2_FS_CRT_ACT,1  # flying indoors, just land ASAP, no need to hit the celing while doing RTL
-BATT2_FS_LOW_ACT,1  # flying indoors, just land ASAP, no need to hit the celing while doing RTL
+BATT2_FS_CRT_ACT,1  # flying indoors, just land ASAP, no need to hit the ceiling while doing RTL
+BATT2_FS_LOW_ACT,1  # flying indoors, just land ASAP, no need to hit the ceiling while doing RTL
 BATT2_FS_VOLTSRC,1  # In our build this is a redundant monitor for batt1 so == BATT_FS_VOLTSRC
 BATT2_LOW_MAH,600  # In our build this is a redundant monitor for batt1 so == BATT_LOW_MAH
 BATT2_LOW_VOLT,14.4  # In our build this is a redundant monitor for batt1 so == BATT_LOW_VOLT
 BATT2_MONITOR,4
-BATT2_VOLT_MULT,228.342 # Use a power source with a voltage close to BATT2_LOW_VOLT measure with a calibrated voltimeter and adapt this parameter so that the telemetry voltage reading matches it
+BATT2_VOLT_MULT,228.342  # Use a power source with a voltage close to BATT2_LOW_VOLT measure with a calibrated voltimeter and adapt this parameter so that the telemetry voltage reading matches it
 BATT2_VOLT_PIN,18
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/16_pid_adjustment.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/X11_plus/16_pid_adjustment.param`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # If you have a very small, or a very large vehicle that requires non-default PID values for a safe flight, change them here
 #
 # Usually, smaller vehicles require lower than default PID rate values.
 # Larger vehicles usually require higher than default PID rate values.
 
-ATC_RAT_PIT_D,0.003334  #  = 0.925972 * (0.0036 default)
-ATC_RAT_PIT_I,0.173229  #  = 1.283176 * (0.135 default)
-ATC_RAT_PIT_P,0.173229  #  = 1.283176 * (0.135 default)
-ATC_RAT_RLL_D,0.002486  #  = 0.690593 * (0.0036 default)
-ATC_RAT_RLL_I,0.143237  #  = 1.061015 * (0.135 default)
-ATC_RAT_RLL_P,0.143237  #  = 1.061015 * (0.135 default)
+ATC_ANG_PIT_P,6.0
+ATC_ANG_RLL_P,5.2
+ATC_ANG_YAW_P,3.0
+ATC_INPUT_TC,0.17  # Make the RC feel a bit slower than default
+ATC_RAT_PIT_D,0.002781  #  (0.0036 default)
+ATC_RAT_PIT_I,0.085568  #  = 1.283176 * (0.135 default)
+ATC_RAT_PIT_P,0.085568  #  = 1.283176 * (0.135 default)
+ATC_RAT_RLL_D,0.00309  #  = 0.690593 * (0.0036 default)
+ATC_RAT_RLL_I,0.095506  #  = 1.061015 * (0.135 default)
+ATC_RAT_RLL_P,0.095506  #  = 1.061015 * (0.135 default)
 ATC_RAT_YAW_D,0  #  = 1 * (0 default)
-ATC_RAT_YAW_I,0.045252  #  = 2.514026 * (0.018 default)
-ATC_RAT_YAW_P,0.452525  #  = 2.514026 * (0.18 default)
+ATC_RAT_YAW_I,0.025  #  = 2.514026 * (0.018 default)
+ATC_RAT_YAW_P,0.25  #  = 2.514026 * (0.18 default)
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/18_notch_filter_setup.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/18_notch_filter_setup.param`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-INS_FAST_SAMPLE,3  # Both IMUs can run fast on the Matek H743 Slim flight controller
-INS_GYRO_RATE,2  # The Matek H743 Slim can do 4KHz here
-INS_HNTCH_ATT,20  # this is just a hunch, it must be improved after the first flight (by the next file)
-INS_HNTCH_BW,20  # this is just a hunch, it must be improved after the first flight (by the next file)
-INS_HNTCH_ENABLE,1  # the first notch filter will be used to filter the noise created by the motors/propellers
-INS_HNTCH_FREQ,160  # Start with 1.4 • INS_GYRO_FILTER
-INS_HNTCH_HMNCS,1  # start with a single frequency
-INS_HNTCH_MODE,3  # Use the BDshot600 RPM telemetry to dynamicaly track noise created by the motors/propellers
-INS_HNTCH_OPTS,6  # One Notch per motor, update at loop rate
-INS_HNTCH_REF,1  # Use the BDshot600 RPM telemetry to dynamicaly track noise created by the motors/propellers
+INS_FAST_SAMPLE,3  # Both IMUs can run fast on the Matek H743 Slim flight controller
+INS_GYRO_RATE,2  # The Matek H743 Slim can do 4KHz here
+INS_HNTCH_ATT,20  # this is just a hunch, it must be improved after the first flight (by the next file)
+INS_HNTCH_BW,20  # this is just a hunch, it must be improved after the first flight (by the next file)
+INS_HNTCH_ENABLE,1  # the first notch filter will be used to filter the noise created by the motors/propellers
+INS_HNTCH_FREQ,161  # Use 1.4 * INS_GYRO_FILTER as a first guess
+INS_HNTCH_HMNCS,1  # start with a single frequency
+INS_HNTCH_MODE,3  # Use the BDshot600 RPM telemetry to dynamicaly track noise created by the motors/propellers
+INS_HNTCH_OPTS,6  # One Notch per motor, update at loop rate
+INS_HNTCH_REF,1  # Use the BDshot600 RPM telemetry to dynamicaly track noise created by the motors/propellers
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/22_inflight_magnetometer_fit_setup.pdef.xml` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_inflight_magnetometer_fit_setup.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/24_inflight_magnetometer_fit_setup.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/24_inflight_magnetometer_fit_setup.param`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MAGH_ALT_DELTA,10 # Height difference between the highest and lowest point of the eight
-MAGH_B,1.2 # Geometric factor for the width of the eight
-MAGH_CMD,117 # Script_Time command value for identification of the script
-MAGH_COUNT,6 # Number of times the drone repeats the eight
-MAGH_LOG_ENABLE,1 # Activates the logging of the MAGH.Active message
-MAGH_MIN_SPEED,5 # Starting speed for the mission; slowly adjusts to the general speed in auto-missions
-MAGH_NUM_WP,18 # Number of waypoints from which the eight is built
-MAGH_USE_LOITER,0 # Sets a Loiter_unlimited command at the beginning of the mission to check the generated waypoints
+MAGH_ALT_DELTA,10 # Height difference between the highest and lowest point of the eight
+MAGH_B,1.2 # Geometric factor for the width of the eight
+MAGH_CMD,117 # Script_Time command value for identification of the script
+MAGH_COUNT,6 # Number of times the drone repeats the eight
+MAGH_LOG_ENABLE,1 # Activates the logging of the MAGH.Active message
+MAGH_MIN_SPEED,5 # Starting speed for the mission; slowly adjusts to the general speed in auto-missions
+MAGH_NUM_WP,18 # Number of waypoints from which the eight is built
+MAGH_USE_LOITER,0 # Sets a Loiter_unlimited command at the beginning of the mission to check the generated waypoints
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_roll.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/42_system_id_roll.param`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-ANGLE_MAX,1500  # limit the angle to limit the speed at SID-chirp low-frequencies
+ANGLE_MAX,2000  # limit the angle to limit the speed at SID-chirp low-frequencies
 ARMING_CHECK,540126  # disable Parameter check because we need to set ATC_RAT_RLL_I out-of-range (was 30175)
-ATC_RAT_RLL_I,0 # prevent the rate controllers from compensating too much of the frequency-sweep signal
-ATC_RATE_FF_ENAB,0 # prevent the rate controllers from compensating too much of the frequency-sweep signal
-LOG_DISARMED,0 # was only needed for wind speed estimation
-LOG_REPLAY,0 # was only needed for wind speed estimation
-SID_AXIS,10
+ATC_ANG_PIT_P,4.5  # reset to default to not interfere with sysID
+ATC_ANG_RLL_P,4.5  # reset to default to not interfere with sysID
+ATC_ANG_YAW_P,4.5  # reset to default to not interfere with sysID
+ATC_RAT_RLL_I,0  # prevent the rate controllers from compensating too much of the frequency-sweep signal
+ATC_RATE_FF_ENAB,0  # prevent the rate controllers from compensating too much of the frequency-sweep signal
+FLTMODE5,25  # Activate sysid instead of autotune
+LOG_BITMASK,176127  # attitude sample rate at loop rate
+LOG_DISARMED,0  # was only needed for wind speed estimation
+LOG_REPLAY,0  # was only needed for wind speed estimation
+SID_AXIS,10  # Inject chip on the mixer roll signal
 SID_F_START_HZ,0.05
 SID_F_STOP_HZ,5
 SID_MAGNITUDE,0.15
 SID_T_FADE_IN,5.0
 SID_T_FADE_OUT,5.0
 SID_T_REC,130.0
-TUNE,58  # System identification magnitude
-TUNE_MAX,0.40  # System identification max magnitude
+TUNE,0  # System identification magnitude
+TUNE_MAX,0.4  # System identification max magnitude
 TUNE_MIN,0.02  # System identification min magnitude
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/47_everyday_use.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/50_everyday_use.param`

 * *Files 12% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-ATC_THR_MIX_MAX,0.7  # according to autotune documentation this should be raised up-to 0.9 after the tune
-BATT_FS_LOW_ACT,2  # outdoors we want the drone to come back
-BATT2_FS_LOW_ACT,2  # outdoors we want the drone to come back
-LOG_BITMASK,2241500 # 2:GPS,3:System Performance,4:Control Tuning,6:RC input,7:IMU,8:Mission Commands,9:Battery Monitor,12:PID,13:Compass,17:Motors,21:Fast harmonic notch logging
-RTL_ALT,500  # The default is too high for the kind of flights we do. This reduces the altitude for outdoors
-RTL_CLIMB_MIN,100  # always rise at least 1 meter as a visual indicator
+ATC_THR_MIX_MAX,0.7  # according to autotune documentation this should be raised up-to 0.9 after the tune
+BATT_FS_LOW_ACT,2  # outdoors we want the drone to come back
+BATT2_FS_LOW_ACT,2  # outdoors we want the drone to come back
+LOG_BITMASK,144348  # 2:GPS,3:System Performance,4:Control Tuning,6:RC input,7:IMU,8:Mission Commands,9:Battery Monitor,12:PID,13:Compass,17:Motors
+RTL_ALT,500  # The default is too high for the kind of flights we do. This reduces the altitude for outdoors
+RTL_CLIMB_MIN,100  # always rise at least 1 meter as a visual indicator
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/48_position_controller.param` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/47_position_controller.param`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-ANGLE_MAX,6500
-LOIT_BRK_ACCEL,500
-LOIT_BRK_DELAY,0.05
-LOIT_BRK_JERK,4000
-PSC_VELXY_FF,0.85  # PSCN.AE/PSCN.VE if you have flown North-South or PSCE.AE/PSCE.VE if you have flown East-West
-WPNAV_ACCEL,400  # high speed missions in auto
-WPNAV_ACCEL_C,800  # 2 * WPNAV_ACCEL so that the cornering behaviour is mostly controlled by WPNAV_RADIUS https://github.com/ArduPilot/ardupilot/pull/25928
-WPNAV_ACCEL_Z,200  # high speed missions in auto
-WPNAV_JERK,5  # high speed missions in auto
-WPNAV_SPEED,2000  # high speed missions in auto
-WPNAV_SPEED_DN,250  # high speed missions in auto
+ANGLE_MAX,6500
+LOIT_ACC_MAX,500
+LOIT_BRK_ACCEL,500
+LOIT_BRK_DELAY,0.05
+LOIT_BRK_JERK,4000
+PSC_VELXY_FF,0.85  # PSCN.AE/PSCN.VE if you have flown North-South or PSCE.AE/PSCE.VE if you have flown East-West
+WPNAV_ACCEL,400  # high speed missions in auto
+WPNAV_ACCEL_C,800  # 2 * WPNAV_ACCEL so that the cornering behaviour is mostly controlled by WPNAV_RADIUS https://github.com/ArduPilot/ardupilot/pull/25928
+WPNAV_ACCEL_Z,200  # high speed missions in auto
+WPNAV_JERK,5  # high speed missions in auto
+WPNAV_SPEED,2000  # high speed missions in auto
+WPNAV_SPEED_DN,250  # high speed missions in auto
```

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/apm.pdef.xml`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle.jpg`

 * *Files identical despite different names*

### Comparing `methodicconfigurator-0.6.4/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.6.0-DEV-params/vehicle_components.json` & `methodicconfigurator-0.6.5/vehicle_templates/ArduCopter/diatone_taycan_mxc/4.5.3-params/vehicle_components.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954788773148148%*

 * *Differences: {"'Components'": "{'Flight Controller': {'Firmware': {'Version': '4.5.3'}}, 'Frame': "*

 * *                 "{'Specifications': OrderedDict([('TOW min Kg', 0.6), ('TOW max Kg', 0.6)])}, "*

 * *                 "'Battery Monitor': {'Firmware': {'Version': '4.5.3'}}, 'Battery': "*

 * *                 "{'Specifications': {'Capacity mAh': 1800}}}"}*

```diff
@@ -5,29 +5,30 @@
             "Product": {
                 "Manufacturer": "SLS",
                 "Model": "X-Cube 1800mAh 4S1P 14,8V 40C/80C",
                 "URL": "https://www.stefansliposhop.de/akkus/sls-x-cube/sls-x-cube-40c/sls-x-cube-1800mah-4s1p-14-8v-40c-80c::1568.html",
                 "Version": ""
             },
             "Specifications": {
+                "Capacity mAh": 1800,
                 "Chemistry": "Lipo",
                 "Number of cells": 4,
                 "Volt per cell crit": 3.55,
                 "Volt per cell low": 3.6,
                 "Volt per cell max": 4.2
             }
         },
         "Battery Monitor": {
             "FC Connection": {
                 "Protocol": "Analog Voltage and Current",
                 "Type": "Analog"
             },
             "Firmware": {
                 "Type": "ArduCopter",
-                "Version": "4.5.1"
+                "Version": "4.5.3"
             },
             "Notes": "Voltage is done via the flight controller. Current is done via the ESC.",
             "Product": {
                 "Manufacturer": "Matek",
                 "Model": "H743 SLIM",
                 "URL": "https://www.mateksys.com/?portfolio=h743-slim",
                 "Version": "3"
@@ -49,15 +50,15 @@
                 "URL": "https://www.diatone.us/products/mb-f45_128k-bl32-esc",
                 "Version": "1"
             }
         },
         "Flight Controller": {
             "Firmware": {
                 "Type": "ArduCopter",
-                "Version": "4.5.1"
+                "Version": "4.5.3"
             },
             "Notes": "This is a custom build with a Matek H743 SLIM flight controller. The board is a 20x20mm stackable board with a 400Mhz processor, 1Mb flash, 512kb RAM, and a 32-bit STM32H743 processor. The board has a built-in barometer, 6 UARTs, 8 PWM outputs, and 8 ADC inputs.",
             "Product": {
                 "Manufacturer": "Matek",
                 "Model": "H743 SLIM",
                 "URL": "https://www.mateksys.com/?portfolio=h743-slim",
                 "Version": "V3"
@@ -66,14 +67,18 @@
         "Frame": {
             "Notes": "A small 3'' ducted frame",
             "Product": {
                 "Manufacturer": "Diatone",
                 "Model": "Taycan MX-C",
                 "URL": "https://www.diatone.us/products/diatone-mxc-taycan-duct-3-inch-cinewhoop-fpv-drone",
                 "Version": "2022"
+            },
+            "Specifications": {
+                "TOW max Kg": 0.6,
+                "TOW min Kg": 0.6
             }
         },
         "GNSS receiver": {
             "FC Connection": {
                 "Protocol": "uBlox",
                 "Type": "SERIAL3"
             },
```

