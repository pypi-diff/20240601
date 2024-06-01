# Comparing `tmp/ourskyai_astro_api-1.3.3700.tar.gz` & `tmp/ourskyai_astro_api-1.3.3703.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourskyai_astro_api-1.3.3700.tar", max compression
+gzip compressed data, was "ourskyai_astro_api-1.3.3703.tar", max compression
```

## Comparing `ourskyai_astro_api-1.3.3700.tar` & `ourskyai_astro_api-1.3.3703.tar`

### file list

```diff
@@ -1,78 +1,79 @@
--rw-r--r--   0        0        0    11541 2024-05-31 18:11:15.703961 ourskyai_astro_api-1.3.3700/README.md
--rw-r--r--   0        0        0     6292 2024-05-31 18:11:19.291846 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/__init__.py
--rw-r--r--   0        0        0      106 2024-05-31 18:11:19.323845 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/api/__init__.py
--rw-r--r--   0        0        0   260295 2024-05-31 18:11:19.423842 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/api/default_api.py
--rw-r--r--   0        0        0    30352 2024-05-31 18:11:19.499840 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/api_client.py
--rw-r--r--   0        0        0      852 2024-05-31 18:11:19.551838 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/api_response.py
--rw-r--r--   0        0        0    14687 2024-05-31 18:11:19.595836 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/configuration.py
--rw-r--r--   0        0        0     5433 2024-05-31 18:11:19.655835 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/exceptions.py
--rw-r--r--   0        0        0     5651 2024-05-31 18:11:19.711833 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/__init__.py
--rw-r--r--   0        0        0      819 2024-05-31 18:11:19.763831 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/asset_file_type.py
--rw-r--r--   0        0        0      931 2024-05-31 18:11:19.823829 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/asset_type.py
--rw-r--r--   0        0        0      809 2024-05-31 18:11:19.899827 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/calibration_master_type.py
--rw-r--r--   0        0        0     2092 2024-05-31 18:11:19.935826 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/daily_weather_city.py
--rw-r--r--   0        0        0     4308 2024-05-31 18:11:19.967825 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/daily_weather_forecast_item.py
--rw-r--r--   0        0        0     2527 2024-05-31 18:11:20.007823 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py
--rw-r--r--   0        0        0     2551 2024-05-31 18:11:20.055822 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py
--rw-r--r--   0        0        0     2947 2024-05-31 18:11:20.119820 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/daily_weather_forecast_list_response.py
--rw-r--r--   0        0        0     1904 2024-05-31 18:11:20.167818 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/empty_success.py
--rw-r--r--   0        0        0     1186 2024-05-31 18:11:20.203817 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/filter_type.py
--rw-r--r--   0        0        0     1930 2024-05-31 18:11:20.255815 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/fits_header.py
--rw-r--r--   0        0        0     2155 2024-05-31 18:11:20.319813 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/location.py
--rw-r--r--   0        0        0      747 2024-05-31 18:11:20.363812 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/mount_type.py
--rw-r--r--   0        0        0      887 2024-05-31 18:11:20.423810 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/node_state.py
--rw-r--r--   0        0        0      827 2024-05-31 18:11:20.455809 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/optical_tube_type.py
--rw-r--r--   0        0        0      751 2024-05-31 18:11:20.499807 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/shutter_type.py
--rw-r--r--   0        0        0     1892 2024-05-31 18:11:20.583805 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/successful_create.py
--rw-r--r--   0        0        0      768 2024-05-31 18:11:20.647803 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/tracking_type.py
--rw-r--r--   0        0        0     3258 2024-05-31 18:11:20.687801 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_astro_project.py
--rw-r--r--   0        0        0     3969 2024-05-31 18:11:20.735800 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_astro_project_asset.py
--rw-r--r--   0        0        0     2569 2024-05-31 18:11:20.791798 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
--rw-r--r--   0        0        0     2399 2024-05-31 18:11:20.859796 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
--rw-r--r--   0        0        0     2381 2024-05-31 18:11:20.911794 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_astro_target.py
--rw-r--r--   0        0        0     3640 2024-05-31 18:11:20.983792 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_calibration_master.py
--rw-r--r--   0        0        0     4908 2024-05-31 18:11:21.015791 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_camera.py
--rw-r--r--   0        0        0     2421 2024-05-31 18:11:21.047790 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
--rw-r--r--   0        0        0     2668 2024-05-31 18:11:21.111788 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_astro_project_request.py
--rw-r--r--   0        0        0     2121 2024-05-31 18:11:21.143787 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_astro_project_response.py
--rw-r--r--   0        0        0     3777 2024-05-31 18:11:21.175786 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_calibration_master_request.py
--rw-r--r--   0        0        0     2147 2024-05-31 18:11:21.279783 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_calibration_master_response.py
--rw-r--r--   0        0        0     7059 2024-05-31 18:11:21.355780 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_camera_request.py
--rw-r--r--   0        0        0     2044 2024-05-31 18:11:21.407779 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_image_set_image_request.py
--rw-r--r--   0        0        0     2115 2024-05-31 18:11:21.439777 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_image_set_image_response.py
--rw-r--r--   0        0        0     2683 2024-05-31 18:11:21.495776 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_image_set_request.py
--rw-r--r--   0        0        0     2296 2024-05-31 18:11:21.559774 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_mount_request.py
--rw-r--r--   0        0        0     3146 2024-05-31 18:11:21.591773 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_node_request.py
--rw-r--r--   0        0        0     2447 2024-05-31 18:11:21.631771 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_optical_tube_request.py
--rw-r--r--   0        0        0     2441 2024-05-31 18:11:21.675770 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_elevation_mask_point.py
--rw-r--r--   0        0        0     3289 2024-05-31 18:11:21.791766 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_gain_curve.py
--rw-r--r--   0        0        0     2051 2024-05-31 18:11:21.839765 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_gain_curve_point.py
--rw-r--r--   0        0        0     2096 2024-05-31 18:11:21.895763 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
--rw-r--r--   0        0        0     2364 2024-05-31 18:11:21.963761 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_get_nodes.py
--rw-r--r--   0        0        0     7066 2024-05-31 18:11:21.999760 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
--rw-r--r--   0        0        0     2324 2024-05-31 18:11:22.059758 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
--rw-r--r--   0        0        0     2513 2024-05-31 18:11:22.107756 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
--rw-r--r--   0        0        0     3436 2024-05-31 18:11:22.151755 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_image_set.py
--rw-r--r--   0        0        0     5797 2024-05-31 18:11:22.211753 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_image_set_image.py
--rw-r--r--   0        0        0      795 2024-05-31 18:11:22.251752 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_job_kind.py
--rw-r--r--   0        0        0     2632 2024-05-31 18:11:22.287750 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_job_log.py
--rw-r--r--   0        0        0      803 2024-05-31 18:11:22.343749 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_job_status.py
--rw-r--r--   0        0        0     1914 2024-05-31 18:11:22.387747 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_mount.py
--rw-r--r--   0        0        0     4458 2024-05-31 18:11:22.443745 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_node.py
--rw-r--r--   0        0        0     2564 2024-05-31 18:11:22.487744 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_node_with_location.py
--rw-r--r--   0        0        0     2239 2024-05-31 18:11:22.527743 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_optical_tube.py
--rw-r--r--   0        0        0     3057 2024-05-31 18:11:22.571741 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_platform_credit.py
--rw-r--r--   0        0        0      870 2024-05-31 18:11:22.627740 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_platform_credit_source.py
--rw-r--r--   0        0        0      800 2024-05-31 18:11:22.679738 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_platform_credit_type.py
--rw-r--r--   0        0        0      776 2024-05-31 18:11:22.735736 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_platform_credit_unit.py
--rw-r--r--   0        0        0     2045 2024-05-31 18:11:22.771735 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
--rw-r--r--   0        0        0     2051 2024-05-31 18:11:22.819733 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_read_noise_point.py
--rw-r--r--   0        0        0     2050 2024-05-31 18:11:22.867732 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_setup_action.py
--rw-r--r--   0        0        0     2940 2024-05-31 18:11:22.927730 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_slew_timing.py
--rw-r--r--   0        0        0     2240 2024-05-31 18:11:22.963729 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_slew_timing_interval.py
--rw-r--r--   0        0        0     4605 2024-05-31 18:11:23.015727 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_update_node_request.py
--rw-r--r--   0        0        0     2522 2024-05-31 18:11:23.079725 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
--rw-r--r--   0        0        0        0 2024-05-31 18:11:23.111724 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/py.typed
--rw-r--r--   0        0        0    12935 2024-05-31 18:11:23.155723 ourskyai_astro_api-1.3.3700/ourskyai_astro_api/rest.py
--rw-r--r--   0        0        0      739 2024-05-31 18:11:23.191722 ourskyai_astro_api-1.3.3700/pyproject.toml
--rw-r--r--   0        0        0    12509 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3700/PKG-INFO
+-rw-r--r--   0        0        0    11740 2024-05-31 22:57:59.070838 ourskyai_astro_api-1.3.3703/README.md
+-rw-r--r--   0        0        0     6396 2024-05-31 22:58:02.782843 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-31 22:58:02.806843 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/api/__init__.py
+-rw-r--r--   0        0        0   267033 2024-05-31 22:58:02.890843 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/api/default_api.py
+-rw-r--r--   0        0        0    30352 2024-05-31 22:58:02.954843 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-31 22:58:03.010844 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/api_response.py
+-rw-r--r--   0        0        0    14687 2024-05-31 22:58:03.054844 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/configuration.py
+-rw-r--r--   0        0        0     5433 2024-05-31 22:58:03.110844 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/exceptions.py
+-rw-r--r--   0        0        0     5755 2024-05-31 22:58:03.154844 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/__init__.py
+-rw-r--r--   0        0        0      819 2024-05-31 22:58:03.206844 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/asset_file_type.py
+-rw-r--r--   0        0        0      931 2024-05-31 22:58:03.266844 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/asset_type.py
+-rw-r--r--   0        0        0      809 2024-05-31 22:58:03.314844 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/calibration_master_type.py
+-rw-r--r--   0        0        0     2092 2024-05-31 22:58:03.394844 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/daily_weather_city.py
+-rw-r--r--   0        0        0     4308 2024-05-31 22:58:03.446844 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/daily_weather_forecast_item.py
+-rw-r--r--   0        0        0     2527 2024-05-31 22:58:03.494844 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py
+-rw-r--r--   0        0        0     2551 2024-05-31 22:58:03.538844 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py
+-rw-r--r--   0        0        0     2947 2024-05-31 22:58:03.582844 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/daily_weather_forecast_list_response.py
+-rw-r--r--   0        0        0     1904 2024-05-31 22:58:03.634844 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/empty_success.py
+-rw-r--r--   0        0        0     1186 2024-05-31 22:58:03.674845 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/filter_type.py
+-rw-r--r--   0        0        0     1930 2024-05-31 22:58:03.734845 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/fits_header.py
+-rw-r--r--   0        0        0     2155 2024-05-31 22:58:03.766845 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/location.py
+-rw-r--r--   0        0        0      747 2024-05-31 22:58:03.838845 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/mount_type.py
+-rw-r--r--   0        0        0      887 2024-05-31 22:58:03.878845 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/node_state.py
+-rw-r--r--   0        0        0      827 2024-05-31 22:58:03.938845 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/optical_tube_type.py
+-rw-r--r--   0        0        0      751 2024-05-31 22:58:03.978845 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/shutter_type.py
+-rw-r--r--   0        0        0     1892 2024-05-31 22:58:04.046845 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/successful_create.py
+-rw-r--r--   0        0        0      768 2024-05-31 22:58:04.122845 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/tracking_type.py
+-rw-r--r--   0        0        0     3258 2024-05-31 22:58:04.222845 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_astro_project.py
+-rw-r--r--   0        0        0     3969 2024-05-31 22:58:04.282845 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_astro_project_asset.py
+-rw-r--r--   0        0        0     2569 2024-05-31 22:58:04.322846 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py
+-rw-r--r--   0        0        0     2399 2024-05-31 22:58:04.394846 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py
+-rw-r--r--   0        0        0     2381 2024-05-31 22:58:04.474846 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_astro_target.py
+-rw-r--r--   0        0        0     3640 2024-05-31 22:58:04.522846 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_calibration_master.py
+-rw-r--r--   0        0        0     4908 2024-05-31 22:58:04.574846 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_camera.py
+-rw-r--r--   0        0        0     2421 2024-05-31 22:58:04.622846 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py
+-rw-r--r--   0        0        0     2668 2024-05-31 22:58:04.678846 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_astro_project_request.py
+-rw-r--r--   0        0        0     2121 2024-05-31 22:58:04.722846 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_astro_project_response.py
+-rw-r--r--   0        0        0     2822 2024-05-31 22:58:04.766846 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_autofocus_result_request.py
+-rw-r--r--   0        0        0     3777 2024-05-31 22:58:04.818846 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_calibration_master_request.py
+-rw-r--r--   0        0        0     2147 2024-05-31 22:58:04.882846 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_calibration_master_response.py
+-rw-r--r--   0        0        0     7059 2024-05-31 22:58:04.930847 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_camera_request.py
+-rw-r--r--   0        0        0     2044 2024-05-31 22:58:04.986847 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_image_set_image_request.py
+-rw-r--r--   0        0        0     2115 2024-05-31 22:58:05.030847 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_image_set_image_response.py
+-rw-r--r--   0        0        0     2683 2024-05-31 22:58:05.106847 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_image_set_request.py
+-rw-r--r--   0        0        0     2296 2024-05-31 22:58:05.182847 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_mount_request.py
+-rw-r--r--   0        0        0     3146 2024-05-31 22:58:05.242847 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_node_request.py
+-rw-r--r--   0        0        0     2447 2024-05-31 22:58:05.298847 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_optical_tube_request.py
+-rw-r--r--   0        0        0     2441 2024-05-31 22:58:05.358847 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_elevation_mask_point.py
+-rw-r--r--   0        0        0     3289 2024-05-31 22:58:05.402847 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_gain_curve.py
+-rw-r--r--   0        0        0     2051 2024-05-31 22:58:05.458847 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_gain_curve_point.py
+-rw-r--r--   0        0        0     2096 2024-05-31 22:58:05.514847 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py
+-rw-r--r--   0        0        0     2364 2024-05-31 22:58:05.566847 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_get_nodes.py
+-rw-r--r--   0        0        0     7066 2024-05-31 22:58:05.622847 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_get_or_create_camera_request.py
+-rw-r--r--   0        0        0     2324 2024-05-31 22:58:05.662848 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_get_or_create_mount_request.py
+-rw-r--r--   0        0        0     2513 2024-05-31 22:58:05.694848 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py
+-rw-r--r--   0        0        0     3436 2024-05-31 22:58:05.722848 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_image_set.py
+-rw-r--r--   0        0        0     5797 2024-05-31 22:58:05.778848 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_image_set_image.py
+-rw-r--r--   0        0        0      795 2024-05-31 22:58:05.826848 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_job_kind.py
+-rw-r--r--   0        0        0     2632 2024-05-31 22:58:05.890848 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_job_log.py
+-rw-r--r--   0        0        0      803 2024-05-31 22:58:06.002848 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_job_status.py
+-rw-r--r--   0        0        0     1914 2024-05-31 22:58:06.050848 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_mount.py
+-rw-r--r--   0        0        0     4458 2024-05-31 22:58:06.106848 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_node.py
+-rw-r--r--   0        0        0     2564 2024-05-31 22:58:06.158848 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_node_with_location.py
+-rw-r--r--   0        0        0     2239 2024-05-31 22:58:06.198848 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_optical_tube.py
+-rw-r--r--   0        0        0     3057 2024-05-31 22:58:06.266848 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_platform_credit.py
+-rw-r--r--   0        0        0      870 2024-05-31 22:58:06.322849 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_platform_credit_source.py
+-rw-r--r--   0        0        0      800 2024-05-31 22:58:06.378849 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_platform_credit_type.py
+-rw-r--r--   0        0        0      776 2024-05-31 22:58:06.494849 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_platform_credit_unit.py
+-rw-r--r--   0        0        0     2045 2024-05-31 22:58:06.550849 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py
+-rw-r--r--   0        0        0     2051 2024-05-31 22:58:06.594849 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_read_noise_point.py
+-rw-r--r--   0        0        0     2050 2024-05-31 22:58:06.638849 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_setup_action.py
+-rw-r--r--   0        0        0     2940 2024-05-31 22:58:06.698849 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_slew_timing.py
+-rw-r--r--   0        0        0     2240 2024-05-31 22:58:06.758849 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_slew_timing_interval.py
+-rw-r--r--   0        0        0     4605 2024-05-31 22:58:06.806849 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_update_node_request.py
+-rw-r--r--   0        0        0     2522 2024-05-31 22:58:06.854849 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_video_mode_framerate_property.py
+-rw-r--r--   0        0        0        0 2024-05-31 22:58:06.882849 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/py.typed
+-rw-r--r--   0        0        0    12935 2024-05-31 22:58:06.942849 ourskyai_astro_api-1.3.3703/ourskyai_astro_api/rest.py
+-rw-r--r--   0        0        0      739 2024-05-31 22:58:06.986850 ourskyai_astro_api-1.3.3703/pyproject.toml
+-rw-r--r--   0        0        0    12708 1970-01-01 00:00:00.000000 ourskyai_astro_api-1.3.3703/PKG-INFO
```

### Comparing `ourskyai_astro_api-1.3.3700/README.md` & `ourskyai_astro_api-1.3.3703/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ourskyai-astro-api
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
@@ -91,14 +91,15 @@
 ------------ | ------------- | ------------- | -------------
 *DefaultApi* | [**v1_camera_match**](docs/DefaultApi.md#v1_camera_match) | **GET** /v1/camera-match | 
 *DefaultApi* | [**v1_create_astro_camera**](docs/DefaultApi.md#v1_create_astro_camera) | **POST** /v1/astro-camera | 
 *DefaultApi* | [**v1_create_astro_mount**](docs/DefaultApi.md#v1_create_astro_mount) | **POST** /v1/astro-mount | 
 *DefaultApi* | [**v1_create_astro_optical_tube**](docs/DefaultApi.md#v1_create_astro_optical_tube) | **POST** /v1/astro-optical-tube | 
 *DefaultApi* | [**v1_create_astro_project**](docs/DefaultApi.md#v1_create_astro_project) | **POST** /v1/astro-project | 
 *DefaultApi* | [**v1_create_astro_project_image_set**](docs/DefaultApi.md#v1_create_astro_project_image_set) | **POST** /v1/astro-project-image-set | 
+*DefaultApi* | [**v1_create_autofocus_result**](docs/DefaultApi.md#v1_create_autofocus_result) | **POST** /v1/autofocus | 
 *DefaultApi* | [**v1_create_calibration_master**](docs/DefaultApi.md#v1_create_calibration_master) | **POST** /v1/calibration-master | 
 *DefaultApi* | [**v1_create_image_set**](docs/DefaultApi.md#v1_create_image_set) | **POST** /v1/image-set | 
 *DefaultApi* | [**v1_create_image_set_image**](docs/DefaultApi.md#v1_create_image_set_image) | **POST** /v1/image-set-image | 
 *DefaultApi* | [**v1_create_node**](docs/DefaultApi.md#v1_create_node) | **POST** /v1/node | 
 *DefaultApi* | [**v1_delete_astro_project**](docs/DefaultApi.md#v1_delete_astro_project) | **DELETE** /v1/astro-project | 
 *DefaultApi* | [**v1_delete_calibration_master**](docs/DefaultApi.md#v1_delete_calibration_master) | **DELETE** /v1/calibration-master | 
 *DefaultApi* | [**v1_delete_image_set**](docs/DefaultApi.md#v1_delete_image_set) | **DELETE** /v1/image-set | 
@@ -158,14 +159,15 @@
  - [V1AstroProjectAssetMetadataColorCombination](docs/V1AstroProjectAssetMetadataColorCombination.md)
  - [V1AstroTarget](docs/V1AstroTarget.md)
  - [V1CalibrationMaster](docs/V1CalibrationMaster.md)
  - [V1Camera](docs/V1Camera.md)
  - [V1CreateAstroProjectImageSetRequest](docs/V1CreateAstroProjectImageSetRequest.md)
  - [V1CreateAstroProjectRequest](docs/V1CreateAstroProjectRequest.md)
  - [V1CreateAstroProjectResponse](docs/V1CreateAstroProjectResponse.md)
+ - [V1CreateAutofocusResultRequest](docs/V1CreateAutofocusResultRequest.md)
  - [V1CreateCalibrationMasterRequest](docs/V1CreateCalibrationMasterRequest.md)
  - [V1CreateCalibrationMasterResponse](docs/V1CreateCalibrationMasterResponse.md)
  - [V1CreateCameraRequest](docs/V1CreateCameraRequest.md)
  - [V1CreateImageSetImageRequest](docs/V1CreateImageSetImageRequest.md)
  - [V1CreateImageSetImageResponse](docs/V1CreateImageSetImageResponse.md)
  - [V1CreateImageSetRequest](docs/V1CreateImageSetRequest.md)
  - [V1CreateMountRequest](docs/V1CreateMountRequest.md)
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/__init__.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.3.3700"
+__version__ = "1.3.3703"
 
 # import apis into sdk package
 from ourskyai_astro_api.api.default_api import DefaultApi
 
 # import ApiClient
 from ourskyai_astro_api.api_response import ApiResponse
 from ourskyai_astro_api.api_client import ApiClient
@@ -55,14 +55,15 @@
 from ourskyai_astro_api.models.v1_astro_project_asset_metadata_color_combination import V1AstroProjectAssetMetadataColorCombination
 from ourskyai_astro_api.models.v1_astro_target import V1AstroTarget
 from ourskyai_astro_api.models.v1_calibration_master import V1CalibrationMaster
 from ourskyai_astro_api.models.v1_camera import V1Camera
 from ourskyai_astro_api.models.v1_create_astro_project_image_set_request import V1CreateAstroProjectImageSetRequest
 from ourskyai_astro_api.models.v1_create_astro_project_request import V1CreateAstroProjectRequest
 from ourskyai_astro_api.models.v1_create_astro_project_response import V1CreateAstroProjectResponse
+from ourskyai_astro_api.models.v1_create_autofocus_result_request import V1CreateAutofocusResultRequest
 from ourskyai_astro_api.models.v1_create_calibration_master_request import V1CreateCalibrationMasterRequest
 from ourskyai_astro_api.models.v1_create_calibration_master_response import V1CreateCalibrationMasterResponse
 from ourskyai_astro_api.models.v1_create_camera_request import V1CreateCameraRequest
 from ourskyai_astro_api.models.v1_create_image_set_image_request import V1CreateImageSetImageRequest
 from ourskyai_astro_api.models.v1_create_image_set_image_response import V1CreateImageSetImageResponse
 from ourskyai_astro_api.models.v1_create_image_set_request import V1CreateImageSetRequest
 from ourskyai_astro_api.models.v1_create_mount_request import V1CreateMountRequest
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/api/default_api.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/api/default_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import re  # noqa: F401
@@ -29,14 +29,15 @@
 from ourskyai_astro_api.models.v1_astro_project_asset import V1AstroProjectAsset
 from ourskyai_astro_api.models.v1_astro_target import V1AstroTarget
 from ourskyai_astro_api.models.v1_calibration_master import V1CalibrationMaster
 from ourskyai_astro_api.models.v1_camera import V1Camera
 from ourskyai_astro_api.models.v1_create_astro_project_image_set_request import V1CreateAstroProjectImageSetRequest
 from ourskyai_astro_api.models.v1_create_astro_project_request import V1CreateAstroProjectRequest
 from ourskyai_astro_api.models.v1_create_astro_project_response import V1CreateAstroProjectResponse
+from ourskyai_astro_api.models.v1_create_autofocus_result_request import V1CreateAutofocusResultRequest
 from ourskyai_astro_api.models.v1_create_calibration_master_request import V1CreateCalibrationMasterRequest
 from ourskyai_astro_api.models.v1_create_calibration_master_response import V1CreateCalibrationMasterResponse
 from ourskyai_astro_api.models.v1_create_camera_request import V1CreateCameraRequest
 from ourskyai_astro_api.models.v1_create_image_set_image_request import V1CreateImageSetImageRequest
 from ourskyai_astro_api.models.v1_create_image_set_image_response import V1CreateImageSetImageResponse
 from ourskyai_astro_api.models.v1_create_image_set_request import V1CreateImageSetRequest
 from ourskyai_astro_api.models.v1_create_mount_request import V1CreateMountRequest
@@ -995,14 +996,161 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def v1_create_autofocus_result(self, v1_create_autofocus_result_request : V1CreateAutofocusResultRequest, **kwargs) -> SuccessfulCreate:  # noqa: E501
+        """v1_create_autofocus_result  # noqa: E501
+
+        Create an autofocus result.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_create_autofocus_result(v1_create_autofocus_result_request, async_req=True)
+        >>> result = thread.get()
+
+        :param v1_create_autofocus_result_request: (required)
+        :type v1_create_autofocus_result_request: V1CreateAutofocusResultRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: SuccessfulCreate
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the v1_create_autofocus_result_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        return self.v1_create_autofocus_result_with_http_info(v1_create_autofocus_result_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def v1_create_autofocus_result_with_http_info(self, v1_create_autofocus_result_request : V1CreateAutofocusResultRequest, **kwargs) -> ApiResponse:  # noqa: E501
+        """v1_create_autofocus_result  # noqa: E501
+
+        Create an autofocus result.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.v1_create_autofocus_result_with_http_info(v1_create_autofocus_result_request, async_req=True)
+        >>> result = thread.get()
+
+        :param v1_create_autofocus_result_request: (required)
+        :type v1_create_autofocus_result_request: V1CreateAutofocusResultRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(SuccessfulCreate, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'v1_create_autofocus_result_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method v1_create_autofocus_result" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        if _params['v1_create_autofocus_result_request'] is not None:
+            _body_params = _params['v1_create_autofocus_result_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['Roles', 'BearerToken']  # noqa: E501
+
+        _response_types_map = {
+            '200': "SuccessfulCreate",
+        }
+
+        return self.api_client.call_api(
+            '/v1/autofocus', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/api_client.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
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

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/api_response.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/api_response.py`

 * *Files identical despite different names*

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/configuration.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
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

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/exceptions.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 class OpenApiException(Exception):
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/__init__.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
@@ -38,14 +38,15 @@
 from ourskyai_astro_api.models.v1_astro_project_asset_metadata_color_combination import V1AstroProjectAssetMetadataColorCombination
 from ourskyai_astro_api.models.v1_astro_target import V1AstroTarget
 from ourskyai_astro_api.models.v1_calibration_master import V1CalibrationMaster
 from ourskyai_astro_api.models.v1_camera import V1Camera
 from ourskyai_astro_api.models.v1_create_astro_project_image_set_request import V1CreateAstroProjectImageSetRequest
 from ourskyai_astro_api.models.v1_create_astro_project_request import V1CreateAstroProjectRequest
 from ourskyai_astro_api.models.v1_create_astro_project_response import V1CreateAstroProjectResponse
+from ourskyai_astro_api.models.v1_create_autofocus_result_request import V1CreateAutofocusResultRequest
 from ourskyai_astro_api.models.v1_create_calibration_master_request import V1CreateCalibrationMasterRequest
 from ourskyai_astro_api.models.v1_create_calibration_master_response import V1CreateCalibrationMasterResponse
 from ourskyai_astro_api.models.v1_create_camera_request import V1CreateCameraRequest
 from ourskyai_astro_api.models.v1_create_image_set_image_request import V1CreateImageSetImageRequest
 from ourskyai_astro_api.models.v1_create_image_set_image_response import V1CreateImageSetImageResponse
 from ourskyai_astro_api.models.v1_create_image_set_request import V1CreateImageSetRequest
 from ourskyai_astro_api.models.v1_create_mount_request import V1CreateMountRequest
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/asset_file_type.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/asset_file_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/asset_type.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/asset_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/calibration_master_type.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/calibration_master_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/daily_weather_city.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/daily_weather_city.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/daily_weather_forecast_item.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/daily_weather_forecast_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/daily_weather_forecast_item_temp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/daily_weather_forecast_item_weather_inner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/daily_weather_forecast_list_response.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/daily_weather_forecast_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/empty_success.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/empty_success.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/filter_type.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/filter_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/fits_header.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/fits_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/location.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/location.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/mount_type.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/mount_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/node_state.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/node_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/optical_tube_type.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/optical_tube_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/shutter_type.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/shutter_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/successful_create.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/successful_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/tracking_type.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_job_kind.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,24 +17,25 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class TrackingType(str, Enum):
+class V1JobKind(str, Enum):
     """
-    TrackingType
+    V1JobKind
     """
 
     """
     allowed enum values
     """
-    SIDEREAL = 'SIDEREAL'
-    TARGET_RATE = 'TARGET_RATE'
+    STACK = 'STACK'
+    REPROCESS = 'REPROCESS'
+    OBSERVATION_POTENTIAL = 'OBSERVATION_POTENTIAL'
 
     @classmethod
-    def from_json(cls, json_str: str) -> TrackingType:
-        """Create an instance of TrackingType from a JSON string"""
-        return TrackingType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1JobKind:
+        """Create an instance of V1JobKind from a JSON string"""
+        return V1JobKind(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_astro_project.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_astro_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_astro_project_asset.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_astro_project_asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_astro_project_asset_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_astro_project_asset_metadata_color_combination.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_astro_target.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_astro_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_calibration_master.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_calibration_master.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_camera.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_astro_project_image_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_astro_project_request.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_astro_project_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_astro_project_response.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_astro_project_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_calibration_master_request.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_calibration_master_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_calibration_master_response.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_calibration_master_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_camera_request.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_camera_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_image_set_image_request.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_image_set_image_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_image_set_image_response.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_image_set_image_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_image_set_request.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_image_set_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_mount_request.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_mount_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_node_request.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_create_optical_tube_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_elevation_mask_point.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_elevation_mask_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_gain_curve.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_gain_curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_gain_curve_point.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_gain_curve_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_get_astro_platform_credit_balance_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_get_nodes.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_get_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_get_or_create_camera_request.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_get_or_create_camera_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_get_or_create_mount_request.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_get_or_create_mount_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_get_or_create_optical_tube_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_image_set.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_image_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_image_set_image.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_image_set_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_job_kind.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_platform_credit_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,25 +17,23 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1JobKind(str, Enum):
+class V1PlatformCreditType(str, Enum):
     """
-    V1JobKind
+    V1PlatformCreditType
     """
 
     """
     allowed enum values
     """
-    STACK = 'STACK'
-    REPROCESS = 'REPROCESS'
-    OBSERVATION_POTENTIAL = 'OBSERVATION_POTENTIAL'
+    ASTRO_PLATFORM_USAGE = 'ASTRO_PLATFORM_USAGE'
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1JobKind:
-        """Create an instance of V1JobKind from a JSON string"""
-        return V1JobKind(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1PlatformCreditType:
+        """Create an instance of V1PlatformCreditType from a JSON string"""
+        return V1PlatformCreditType(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_job_log.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_job_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_job_status.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_job_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_mount.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_mount.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_node.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_node_with_location.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_node_with_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_optical_tube.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_optical_tube.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_platform_credit.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_platform_credit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_platform_credit_source.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_platform_credit_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_platform_credit_type.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_platform_credit_unit.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import json
@@ -17,23 +17,23 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class V1PlatformCreditType(str, Enum):
+class V1PlatformCreditUnit(str, Enum):
     """
-    V1PlatformCreditType
+    V1PlatformCreditUnit
     """
 
     """
     allowed enum values
     """
-    ASTRO_PLATFORM_USAGE = 'ASTRO_PLATFORM_USAGE'
+    MEGABYTE = 'MEGABYTE'
 
     @classmethod
-    def from_json(cls, json_str: str) -> V1PlatformCreditType:
-        """Create an instance of V1PlatformCreditType from a JSON string"""
-        return V1PlatformCreditType(json.loads(json_str))
+    def from_json(cls, json_str: str) -> V1PlatformCreditUnit:
+        """Create an instance of V1PlatformCreditUnit from a JSON string"""
+        return V1PlatformCreditUnit(json.loads(json_str))
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_put_stack_astro_project_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_read_noise_point.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_read_noise_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_setup_action.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_setup_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_slew_timing.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_slew_timing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_slew_timing_interval.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_slew_timing_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_update_node_request.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_update_node_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/models/v1_video_mode_framerate_property.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/models/v1_video_mode_framerate_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `ourskyai_astro_api-1.3.3700/ourskyai_astro_api/rest.py` & `ourskyai_astro_api-1.3.3703/ourskyai_astro_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     OurSky Astro
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-    The version of the OpenAPI document: 1.3.3700
+    The version of the OpenAPI document: 1.3.3703
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `ourskyai_astro_api-1.3.3700/pyproject.toml` & `ourskyai_astro_api-1.3.3703/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ourskyai_astro_api"
-version = "1.3.3700"
+version = "1.3.3703"
 description = "OurSky Astro"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OurSky Astro"]
 include = ["ourskyai_astro_api/py.typed"]
```

### Comparing `ourskyai_astro_api-1.3.3700/PKG-INFO` & `ourskyai_astro_api-1.3.3703/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ourskyai_astro_api
-Version: 1.3.3700
+Version: 1.3.3703
 Summary: OurSky Astro
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,OurSky Astro
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # ourskyai-astro-api
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
@@ -116,14 +116,15 @@
 ------------ | ------------- | ------------- | -------------
 *DefaultApi* | [**v1_camera_match**](docs/DefaultApi.md#v1_camera_match) | **GET** /v1/camera-match | 
 *DefaultApi* | [**v1_create_astro_camera**](docs/DefaultApi.md#v1_create_astro_camera) | **POST** /v1/astro-camera | 
 *DefaultApi* | [**v1_create_astro_mount**](docs/DefaultApi.md#v1_create_astro_mount) | **POST** /v1/astro-mount | 
 *DefaultApi* | [**v1_create_astro_optical_tube**](docs/DefaultApi.md#v1_create_astro_optical_tube) | **POST** /v1/astro-optical-tube | 
 *DefaultApi* | [**v1_create_astro_project**](docs/DefaultApi.md#v1_create_astro_project) | **POST** /v1/astro-project | 
 *DefaultApi* | [**v1_create_astro_project_image_set**](docs/DefaultApi.md#v1_create_astro_project_image_set) | **POST** /v1/astro-project-image-set | 
+*DefaultApi* | [**v1_create_autofocus_result**](docs/DefaultApi.md#v1_create_autofocus_result) | **POST** /v1/autofocus | 
 *DefaultApi* | [**v1_create_calibration_master**](docs/DefaultApi.md#v1_create_calibration_master) | **POST** /v1/calibration-master | 
 *DefaultApi* | [**v1_create_image_set**](docs/DefaultApi.md#v1_create_image_set) | **POST** /v1/image-set | 
 *DefaultApi* | [**v1_create_image_set_image**](docs/DefaultApi.md#v1_create_image_set_image) | **POST** /v1/image-set-image | 
 *DefaultApi* | [**v1_create_node**](docs/DefaultApi.md#v1_create_node) | **POST** /v1/node | 
 *DefaultApi* | [**v1_delete_astro_project**](docs/DefaultApi.md#v1_delete_astro_project) | **DELETE** /v1/astro-project | 
 *DefaultApi* | [**v1_delete_calibration_master**](docs/DefaultApi.md#v1_delete_calibration_master) | **DELETE** /v1/calibration-master | 
 *DefaultApi* | [**v1_delete_image_set**](docs/DefaultApi.md#v1_delete_image_set) | **DELETE** /v1/image-set | 
@@ -183,14 +184,15 @@
  - [V1AstroProjectAssetMetadataColorCombination](docs/V1AstroProjectAssetMetadataColorCombination.md)
  - [V1AstroTarget](docs/V1AstroTarget.md)
  - [V1CalibrationMaster](docs/V1CalibrationMaster.md)
  - [V1Camera](docs/V1Camera.md)
  - [V1CreateAstroProjectImageSetRequest](docs/V1CreateAstroProjectImageSetRequest.md)
  - [V1CreateAstroProjectRequest](docs/V1CreateAstroProjectRequest.md)
  - [V1CreateAstroProjectResponse](docs/V1CreateAstroProjectResponse.md)
+ - [V1CreateAutofocusResultRequest](docs/V1CreateAutofocusResultRequest.md)
  - [V1CreateCalibrationMasterRequest](docs/V1CreateCalibrationMasterRequest.md)
  - [V1CreateCalibrationMasterResponse](docs/V1CreateCalibrationMasterResponse.md)
  - [V1CreateCameraRequest](docs/V1CreateCameraRequest.md)
  - [V1CreateImageSetImageRequest](docs/V1CreateImageSetImageRequest.md)
  - [V1CreateImageSetImageResponse](docs/V1CreateImageSetImageResponse.md)
  - [V1CreateImageSetRequest](docs/V1CreateImageSetRequest.md)
  - [V1CreateMountRequest](docs/V1CreateMountRequest.md)
```

