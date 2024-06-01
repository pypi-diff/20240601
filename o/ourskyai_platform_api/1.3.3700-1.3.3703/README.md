# Comparing `tmp/ourskyai_platform_api-1.3.3700.tar.gz` & `tmp/ourskyai_platform_api-1.3.3703.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_platform_api-1.3.3700.tar", max compression
+gzip compressed data, was "ourskyai_platform_api-1.3.3703.tar", max compression
```

## Comparing `ourskyai_platform_api-1.3.3700.tar` & `ourskyai_platform_api-1.3.3703.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     9968 2024-05-31 18:11:15.679962 ourskyai_platform_api-1.3.3700/README.md
--rw-r--r--   0        0        0     6552 2024-05-31 18:11:19.239848 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/__init__.py
--rw-r--r--   0        0        0      109 2024-05-31 18:11:19.271847 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/api/__init__.py
--rw-r--r--   0        0        0   206365 2024-05-31 18:11:19.363844 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/api/default_api.py
--rw-r--r--   0        0        0    30373 2024-05-31 18:11:19.423842 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-31 18:11:19.471840 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/api_response.py
--rw-r--r--   0        0        0    14693 2024-05-31 18:11:19.519839 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/configuration.py
--rw-r--r--   0        0        0     5436 2024-05-31 18:11:19.555838 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/exceptions.py
--rw-r--r--   0        0        0     5881 2024-05-31 18:11:19.599836 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/__init__.py
--rw-r--r--   0        0        0      745 2024-05-31 18:11:19.643835 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/camera_mode.py
--rw-r--r--   0        0        0     1907 2024-05-31 18:11:19.703833 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/empty_success.py
--rw-r--r--   0        0        0     1189 2024-05-31 18:11:19.751831 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/filter_type.py
--rw-r--r--   0        0        0     1933 2024-05-31 18:11:19.795830 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/fits_header.py
--rw-r--r--   0        0        0     2158 2024-05-31 18:11:19.883827 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/location.py
--rw-r--r--   0        0        0      777 2024-05-31 18:11:19.919826 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/metric_type.py
--rw-r--r--   0        0        0      750 2024-05-31 18:11:19.983824 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/mount_type.py
--rw-r--r--   0        0        0      890 2024-05-31 18:11:20.047822 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/node_state.py
--rw-r--r--   0        0        0      830 2024-05-31 18:11:20.099820 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/optical_tube_type.py
--rw-r--r--   0        0        0     2407 2024-05-31 18:11:20.143819 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/plate_solve_parameters.py
--rw-r--r--   0        0        0      754 2024-05-31 18:11:20.195817 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/shutter_type.py
--rw-r--r--   0        0        0     1895 2024-05-31 18:11:20.259815 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/successful_create.py
--rw-r--r--   0        0        0      771 2024-05-31 18:11:20.307814 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/tracking_type.py
--rw-r--r--   0        0        0     2622 2024-05-31 18:11:20.359812 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_auto_focus_instruction.py
--rw-r--r--   0        0        0     2366 2024-05-31 18:11:20.403811 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py
--rw-r--r--   0        0        0     4920 2024-05-31 18:11:20.451809 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_camera.py
--rw-r--r--   0        0        0     2115 2024-05-31 18:11:20.483808 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_client_token.py
--rw-r--r--   0        0        0     2047 2024-05-31 18:11:20.515807 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_complete_observation_request.py
--rw-r--r--   0        0        0     2047 2024-05-31 18:11:20.611804 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2118 2024-05-31 18:11:20.643803 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2692 2024-05-31 18:11:20.695801 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2302 2024-05-31 18:11:20.739800 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     2071 2024-05-31 18:11:20.783799 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py
--rw-r--r--   0        0        0     2710 2024-05-31 18:11:20.839797 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_node_diagnostic.py
--rw-r--r--   0        0        0     2715 2024-05-31 18:11:20.887795 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
--rw-r--r--   0        0        0     3152 2024-05-31 18:11:20.935794 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2453 2024-05-31 18:11:20.963793 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2124 2024-05-31 18:11:21.007791 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_diagnostic_instruction.py
--rw-r--r--   0        0        0     2444 2024-05-31 18:11:21.055790 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0      719 2024-05-31 18:11:21.099788 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_file_type.py
--rw-r--r--   0        0        0     3298 2024-05-31 18:11:21.171786 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2054 2024-05-31 18:11:21.211785 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2570 2024-05-31 18:11:21.263783 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_get_instruction_request.py
--rw-r--r--   0        0        0     2370 2024-05-31 18:11:21.431778 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7081 2024-05-31 18:11:21.471777 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2330 2024-05-31 18:11:21.523775 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2519 2024-05-31 18:11:21.595773 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     2675 2024-05-31 18:11:21.663770 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
--rw-r--r--   0        0        0     3985 2024-05-31 18:11:21.711769 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_ground_station_participant.py
--rw-r--r--   0        0        0     3445 2024-05-31 18:11:21.747768 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5803 2024-05-31 18:11:21.791766 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0     3763 2024-05-31 18:11:21.915762 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_instruction.py
--rw-r--r--   0        0        0     2400 2024-05-31 18:11:21.959761 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_metric.py
--rw-r--r--   0        0        0     1917 2024-05-31 18:11:22.051758 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_mount.py
--rw-r--r--   0        0        0     4470 2024-05-31 18:11:22.127755 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_node.py
--rw-r--r--   0        0        0      850 2024-05-31 18:11:22.187754 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_node_component_type.py
--rw-r--r--   0        0        0     1963 2024-05-31 18:11:22.247752 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_node_controller_artifact.py
--rw-r--r--   0        0        0     1669 2024-05-31 18:11:22.307750 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_node_diagnostic_type.py
--rw-r--r--   0        0        0     2573 2024-05-31 18:11:22.339749 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     5537 2024-05-31 18:11:22.407747 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_observation_instruction.py
--rw-r--r--   0        0        0     2242 2024-05-31 18:11:22.455745 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     2135 2024-05-31 18:11:22.487744 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
--rw-r--r--   0        0        0     2648 2024-05-31 18:11:22.543742 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
--rw-r--r--   0        0        0     2054 2024-05-31 18:11:22.599740 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2401 2024-05-31 18:11:22.651739 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_release.py
--rw-r--r--   0        0        0     2053 2024-05-31 18:11:22.695737 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2946 2024-05-31 18:11:22.735736 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2243 2024-05-31 18:11:22.811734 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     3601 2024-05-31 18:11:22.859732 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_update_node_components_request.py
--rw-r--r--   0        0        0     6269 2024-05-31 18:11:22.915730 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
--rw-r--r--   0        0        0     2402 2024-05-31 18:11:22.959729 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
--rw-r--r--   0        0        0     2591 2024-05-31 18:11:23.003728 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
--rw-r--r--   0        0        0     4620 2024-05-31 18:11:23.043726 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2525 2024-05-31 18:11:23.079725 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0     2224 2024-05-31 18:11:23.127724 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v2_complete_observation_request.py
--rw-r--r--   0        0        0        0 2024-05-31 18:11:23.159722 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/py.typed
--rw-r--r--   0        0        0    12941 2024-05-31 18:11:23.211721 ourskyai_platform_api-1.3.3700/ourskyai_platform_api/rest.py
--rw-r--r--   0        0        0      751 2024-05-31 18:11:23.243720 ourskyai_platform_api-1.3.3700/pyproject.toml
--rw-r--r--   0        0        0    10945 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3700/PKG-INFO
+-rw-r--r--   0        0        0     9968 2024-05-31 22:57:59.086838 ourskyai_platform_api-1.3.3703/README.md
+-rw-r--r--   0        0        0     6552 2024-05-31 22:58:02.642843 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/__init__.py
+-rw-r--r--   0        0        0      109 2024-05-31 22:58:02.674843 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/api/__init__.py
+-rw-r--r--   0        0        0   206365 2024-05-31 22:58:02.790843 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/api/default_api.py
+-rw-r--r--   0        0        0    30373 2024-05-31 22:58:02.834843 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-31 22:58:02.890843 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/api_response.py
+-rw-r--r--   0        0        0    14693 2024-05-31 22:58:02.946843 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/configuration.py
+-rw-r--r--   0        0        0     5436 2024-05-31 22:58:03.018844 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/exceptions.py
+-rw-r--r--   0        0        0     5881 2024-05-31 22:58:03.078844 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-31 22:58:03.138844 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/camera_mode.py
+-rw-r--r--   0        0        0     1907 2024-05-31 22:58:03.186844 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/empty_success.py
+-rw-r--r--   0        0        0     1189 2024-05-31 22:58:03.226844 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/filter_type.py
+-rw-r--r--   0        0        0     1933 2024-05-31 22:58:03.262844 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/fits_header.py
+-rw-r--r--   0        0        0     2158 2024-05-31 22:58:03.310844 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/location.py
+-rw-r--r--   0        0        0      777 2024-05-31 22:58:03.362844 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/metric_type.py
+-rw-r--r--   0        0        0      750 2024-05-31 22:58:03.414844 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/mount_type.py
+-rw-r--r--   0        0        0      890 2024-05-31 22:58:03.482844 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/node_state.py
+-rw-r--r--   0        0        0      830 2024-05-31 22:58:03.550844 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0     2407 2024-05-31 22:58:03.598844 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/plate_solve_parameters.py
+-rw-r--r--   0        0        0      754 2024-05-31 22:58:03.646844 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1895 2024-05-31 22:58:03.786845 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/successful_create.py
+-rw-r--r--   0        0        0      771 2024-05-31 22:58:03.878845 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/tracking_type.py
+-rw-r--r--   0        0        0     2710 2024-05-31 22:58:03.942845 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_auto_focus_instruction.py
+-rw-r--r--   0        0        0     2366 2024-05-31 22:58:04.026845 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py
+-rw-r--r--   0        0        0     4920 2024-05-31 22:58:04.090845 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2115 2024-05-31 22:58:04.142845 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_client_token.py
+-rw-r--r--   0        0        0     2047 2024-05-31 22:58:04.202845 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_complete_observation_request.py
+-rw-r--r--   0        0        0     2047 2024-05-31 22:58:04.286846 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2118 2024-05-31 22:58:04.346845 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2692 2024-05-31 22:58:04.398846 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2302 2024-05-31 22:58:04.458846 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     2071 2024-05-31 22:58:04.506846 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py
+-rw-r--r--   0        0        0     2710 2024-05-31 22:58:04.542846 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_node_diagnostic.py
+-rw-r--r--   0        0        0     2715 2024-05-31 22:58:04.590846 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py
+-rw-r--r--   0        0        0     3152 2024-05-31 22:58:04.650846 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2453 2024-05-31 22:58:04.706846 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2124 2024-05-31 22:58:04.778846 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_diagnostic_instruction.py
+-rw-r--r--   0        0        0     2444 2024-05-31 22:58:04.850846 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0      719 2024-05-31 22:58:04.902846 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_file_type.py
+-rw-r--r--   0        0        0     3298 2024-05-31 22:58:04.962846 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2054 2024-05-31 22:58:05.010846 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2570 2024-05-31 22:58:05.090847 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_get_instruction_request.py
+-rw-r--r--   0        0        0     2370 2024-05-31 22:58:05.134847 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7081 2024-05-31 22:58:05.242847 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2330 2024-05-31 22:58:05.294847 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2519 2024-05-31 22:58:05.386847 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2675 2024-05-31 22:58:05.426847 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py
+-rw-r--r--   0        0        0     3985 2024-05-31 22:58:05.470847 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_ground_station_participant.py
+-rw-r--r--   0        0        0     3445 2024-05-31 22:58:05.534847 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5803 2024-05-31 22:58:05.586847 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0     3763 2024-05-31 22:58:05.626848 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_instruction.py
+-rw-r--r--   0        0        0     2400 2024-05-31 22:58:05.674847 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_metric.py
+-rw-r--r--   0        0        0     1917 2024-05-31 22:58:05.718848 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4470 2024-05-31 22:58:05.770848 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_node.py
+-rw-r--r--   0        0        0      850 2024-05-31 22:58:05.818848 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_node_component_type.py
+-rw-r--r--   0        0        0     1963 2024-05-31 22:58:05.874848 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_node_controller_artifact.py
+-rw-r--r--   0        0        0     1669 2024-05-31 22:58:05.938848 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_node_diagnostic_type.py
+-rw-r--r--   0        0        0     2573 2024-05-31 22:58:05.990848 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     5537 2024-05-31 22:58:06.038848 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_observation_instruction.py
+-rw-r--r--   0        0        0     2242 2024-05-31 22:58:06.098848 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     2135 2024-05-31 22:58:06.138848 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py
+-rw-r--r--   0        0        0     2648 2024-05-31 22:58:06.186848 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py
+-rw-r--r--   0        0        0     2054 2024-05-31 22:58:06.230848 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2401 2024-05-31 22:58:06.286848 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_release.py
+-rw-r--r--   0        0        0     2053 2024-05-31 22:58:06.338849 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2946 2024-05-31 22:58:06.390849 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2243 2024-05-31 22:58:06.434849 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     3601 2024-05-31 22:58:06.494849 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_update_node_components_request.py
+-rw-r--r--   0        0        0     6269 2024-05-31 22:58:06.538849 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_update_node_components_request_camera.py
+-rw-r--r--   0        0        0     2402 2024-05-31 22:58:06.598849 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_update_node_components_request_mount.py
+-rw-r--r--   0        0        0     2591 2024-05-31 22:58:06.646849 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py
+-rw-r--r--   0        0        0     4620 2024-05-31 22:58:06.686849 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2525 2024-05-31 22:58:06.730849 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0     2224 2024-05-31 22:58:06.810849 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v2_complete_observation_request.py
+-rw-r--r--   0        0        0        0 2024-05-31 22:58:06.842849 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/py.typed
+-rw-r--r--   0        0        0    12941 2024-05-31 22:58:06.890849 ourskyai_platform_api-1.3.3703/ourskyai_platform_api/rest.py
+-rw-r--r--   0        0        0      751 2024-05-31 22:58:06.946849 ourskyai_platform_api-1.3.3703/pyproject.toml
+-rw-r--r--   0        0        0    10945 1970-01-01 00:00:00.000000 ourskyai_platform_api-1.3.3703/PKG-INFO
```

### Comparing `ourskyai_platform_api-1.3.3700/README.md` & `ourskyai_platform_api-1.3.3703/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-platform-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3700
-- Package version: 1.3.3700
+- API version: 1.3.3703
+- Package version: 1.3.3703
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/__init__.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3700"
+__version__ = "1.3.3703"
 
 # import apis into sdk package
 from ourskyai_platform_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_platform_api.api_response import ApiResponse
 from ourskyai_platform_api.api_client import ApiClient
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/api/default_api.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/api_client.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import atexit
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.3.3700/python'
+        self.user_agent = 'OpenAPI-Generator/1.3.3703/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/api_response.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/configuration.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -371,16 +371,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.3.3700\n"\
-               "SDK Package Version: 1.3.3700".\
+               "Version of the API: 1.3.3703\n"\
+               "SDK Package Version: 1.3.3703".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/exceptions.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/__init__.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/camera_mode.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/camera_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/empty_success.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/empty_success.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/filter_type.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/filter_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/fits_header.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/fits_header.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/location.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/location.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/metric_type.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/metric_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/mount_type.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/mount_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/node_state.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/node_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/optical_tube_type.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/optical_tube_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/plate_solve_parameters.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/plate_solve_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/shutter_type.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/shutter_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/successful_create.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/successful_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/tracking_type.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_file_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,24 +17,23 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class TrackingType(str, Enum):
+class V1FileType(str, Enum):
     """
-    TrackingType
+    V1FileType
     """
 
     """
     allowed enum values
     """
-    SIDEREAL = 'SIDEREAL'
-    TARGET_RATE = 'TARGET_RATE'
+    ZIP = 'ZIP'
 
     @classmethod
-    def from_json(cls, json_str: str) -> TrackingType:
-        """Create an instance of TrackingType from a JSON string"""
-        return TrackingType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1FileType:
+        """Create an instance of V1FileType from a JSON string"""
+        return V1FileType(json.loads(json_str))
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_auto_focus_instruction.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_auto_focus_instruction.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, conlist
+from pydantic import BaseModel, Field, StrictStr, conlist
 from ourskyai_platform_api.models.v1_auto_focus_instruction_coordinates_inner import V1AutoFocusInstructionCoordinatesInner
 
 class V1AutoFocusInstruction(BaseModel):
     """
     Autofocus Instruction  # noqa: E501
     """
+    id: StrictStr = Field(...)
     coordinates: Optional[conlist(V1AutoFocusInstructionCoordinatesInner)] = None
-    __properties = ["coordinates"]
+    __properties = ["id", "coordinates"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -68,12 +69,13 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return V1AutoFocusInstruction.parse_obj(obj)
 
         _obj = V1AutoFocusInstruction.parse_obj({
+            "id": obj.get("id"),
             "coordinates": [V1AutoFocusInstructionCoordinatesInner.from_dict(_item) for _item in obj.get("coordinates")] if obj.get("coordinates") is not None else None
         })
         return _obj
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_auto_focus_instruction_coordinates_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_camera.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_client_token.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_client_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_complete_observation_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_complete_observation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_image_set_image_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_image_set_image_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_image_set_image_response.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_image_set_image_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_image_set_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_image_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_mount_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_mount_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_node_controller_artifact_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_node_diagnostic.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_node_diagnostic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_node_diagnostics_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_node_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_create_optical_tube_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_diagnostic_instruction.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_diagnostic_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_elevation_mask_point.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_elevation_mask_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_file_type.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/tracking_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,23 +17,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1FileType(str, Enum):
+class TrackingType(str, Enum):
     """
-    V1FileType
+    TrackingType
     """
 
     """
     allowed enum values
     """
-    ZIP = 'ZIP'
+    SIDEREAL = 'SIDEREAL'
+    TARGET_RATE = 'TARGET_RATE'
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1FileType:
-        """Create an instance of V1FileType from a JSON string"""
-        return V1FileType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> TrackingType:
+        """Create an instance of TrackingType from a JSON string"""
+        return TrackingType(json.loads(json_str))
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_gain_curve.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_gain_curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_gain_curve_point.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_gain_curve_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_get_instruction_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_get_instruction_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_get_nodes.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_get_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_get_or_create_camera_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_get_or_create_camera_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_get_or_create_mount_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_get_or_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_get_plate_solve_catalog_diff_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_ground_station_participant.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_ground_station_participant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_image_set.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_image_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_image_set_image.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_image_set_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_instruction.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_instruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_metric.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_mount.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_mount.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_node.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_node_component_type.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_node_component_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_node_controller_artifact.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_node_controller_artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_node_diagnostic_type.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_node_diagnostic_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_node_with_location.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_node_with_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_observation_instruction.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_observation_instruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_optical_tube.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_optical_tube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_plate_solve_catalog_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_plate_solve_catalog_file_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_read_noise_point.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_read_noise_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_release.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_release.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_setup_action.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_setup_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_slew_timing.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_slew_timing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_slew_timing_interval.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_slew_timing_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_update_node_components_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_update_node_components_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_update_node_components_request_camera.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_update_node_components_request_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_update_node_components_request_mount.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_update_node_components_request_mount.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_update_node_components_request_optical_tube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_update_node_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_update_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v1_video_mode_framerate_property.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v1_video_mode_framerate_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/models/v2_complete_observation_request.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/models/v2_complete_observation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_platform_api-1.3.3700/ourskyai_platform_api/rest.py` & `ourskyai_platform_api-1.3.3703/ourskyai_platform_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Platform
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_platform_api-1.3.3700/pyproject.toml` & `ourskyai_platform_api-1.3.3703/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_platform_api"
-version = "1.3.3700"
+version = "1.3.3703"
 description = "OurSky Platform"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Platform"]
 include = ["ourskyai_platform_api/py.typed"]
```

### Comparing `ourskyai_platform_api-1.3.3700/PKG-INFO` & `ourskyai_platform_api-1.3.3703/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_platform_api
-Version: 1.3.3700
+Version: 1.3.3703
 Summary: OurSky Platform
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Platform
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-platform-api
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.3.3700
-- Package version: 1.3.3700
+- API version: 1.3.3703
+- Package version: 1.3.3703
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

