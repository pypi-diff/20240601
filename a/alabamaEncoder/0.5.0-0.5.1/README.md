# Comparing `tmp/alabamaencoder-0.5.0.tar.gz` & `tmp/alabamaencoder-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alabamaencoder-0.5.0.tar", last modified: Thu May 30 16:09:21 2024, max compression
+gzip compressed data, was "alabamaencoder-0.5.1.tar", last modified: Sat Jun  1 17:03:53 2024, max compression
```

## Comparing `alabamaencoder-0.5.0.tar` & `alabamaencoder-0.5.1.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.202224 alabamaencoder-0.5.0/
--rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      377 2024-05-30 16:09:21.202224 alabamaencoder-0.5.0/PKG-INFO
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.182223 alabamaencoder-0.5.0/alabamaEncode/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2021-04-17 09:55:33.000000 alabamaencoder-0.5.0/alabamaEncode/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.182223 alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 08:49:47.000000 alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1564 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/aom_firstpass.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1026 2023-12-18 07:05:43.000000 alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/perdict.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.182223 alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/train/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 10:35:40.000000 alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/train/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12402 2023-12-14 22:03:21.000000 alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/train/train.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.182223 alabamaencoder-0.5.0/alabamaEncode/cli/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:52:09.000000 alabamaencoder-0.5.0/alabamaEncode/cli/__init__.py
--rwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)     4898 2024-05-30 02:35:51.000000 alabamaencoder-0.5.0/alabamaEncode/cli/__main__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.182223 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 18:44:18.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4150 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/autopaths.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    19457 2024-05-30 13:15:45.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/cli_args.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1162 2024-03-05 20:46:37.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/paths.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      795 2024-05-30 02:02:54.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/ratecontrol.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1130 2023-12-10 18:44:44.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/res_preset.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1992 2024-05-30 02:17:46.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/validate_files.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1182 2024-05-30 02:17:46.000000 alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/video_filters.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.182223 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:25:35.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.186223 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:35.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.186223 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-17 00:34:57.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1064 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3401 2024-03-05 22:28:46.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4061 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10641 2024-05-30 02:25:07.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      597 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      606 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5578 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      448 2023-12-10 19:05:23.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/chunk_analyse_step.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      623 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_step.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.186223 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-05 14:55:01.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11063 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6476 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2292 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      850 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2487 2024-05-29 18:57:24.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/opinionated_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4887 2024-05-30 02:10:49.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/pipelines.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      133 2024-01-15 01:49:31.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/refine_step.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.186223 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/refine_steps/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-14 19:17:26.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/refine_steps/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4965 2024-05-30 02:18:47.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/refine_steps/multires_package.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7817 2024-01-20 18:40:41.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.186223 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:49.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1563 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/args_tune.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4702 2024-05-30 02:23:07.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/autocrop.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      552 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/denoise_filtering.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2409 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/encoding_tiles.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7516 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6001 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/sequence_autograin.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3092 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3103 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/x264_tune.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.190224 alabamaencoder-0.5.0/alabamaEncode/core/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-19 23:19:38.000000 alabamaencoder-0.5.0/alabamaEncode/core/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3885 2024-05-30 02:29:55.000000 alabamaencoder-0.5.0/alabamaEncode/core/chunk_job.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10534 2024-05-30 02:18:05.000000 alabamaencoder-0.5.0/alabamaEncode/core/context.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.190224 alabamaencoder-0.5.0/alabamaEncode/core/extras/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-24 18:44:15.000000 alabamaencoder-0.5.0/alabamaEncode/core/extras/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12749 2024-05-30 02:32:33.000000 alabamaencoder-0.5.0/alabamaEncode/core/extras/auto_thumbnailer.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1776 2023-12-24 03:53:49.000000 alabamaencoder-0.5.0/alabamaEncode/core/extras/ws_update.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13723 2024-05-30 02:32:32.000000 alabamaencoder-0.5.0/alabamaEncode/core/ffmpeg.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5676 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/core/final_touches.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    19233 2024-05-30 02:36:52.000000 alabamaencoder-0.5.0/alabamaEncode/core/job.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.190224 alabamaencoder-0.5.0/alabamaEncode/core/util/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 02:17:11.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      125 2024-05-30 02:20:37.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/abort_controler.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2895 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/bin_utils.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4947 2024-01-31 09:31:42.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/cli_executor.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      773 2024-05-30 02:32:32.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/get_yuv_stream.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1877 2024-04-22 19:11:27.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/kv.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      813 2023-11-25 00:35:54.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/path.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      556 2023-11-12 21:29:16.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/timer.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3758 2024-05-25 22:57:08.000000 alabamaencoder-0.5.0/alabamaEncode/core/util/yuv.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.190224 alabamaencoder-0.5.0/alabamaEncode/demon/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:38:55.000000 alabamaencoder-0.5.0/alabamaEncode/demon/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2289 2024-03-05 20:43:08.000000 alabamaencoder-0.5.0/alabamaEncode/demon/demon.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.190224 alabamaencoder-0.5.0/alabamaEncode/encoder/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-09-27 12:09:43.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      748 2024-01-17 00:16:49.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/codec.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11448 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/encoder.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1628 2024-05-29 16:04:18.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/encoder_factory.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.194224 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4379 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/Aomenc.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2092 2024-05-30 02:18:47.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/Nvenc.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1596 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/SvtAvif.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7672 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/Svtenc.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2177 2024-05-30 02:18:47.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/VaapiH264.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2119 2024-05-30 02:18:47.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/VaapiH265.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2315 2024-05-30 02:18:47.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/VideoToolbox.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7253 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/X264.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4107 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/X265.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2022-12-05 03:43:14.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2043 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/rav1e.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3567 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/impl/vp9.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      269 2024-01-17 00:14:46.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/rate_dist.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2494 2024-02-04 12:07:28.000000 alabamaencoder-0.5.0/alabamaEncode/encoder/stats.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.194224 alabamaencoder-0.5.0/alabamaEncode/experiments/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3713 2023-12-11 23:14:15.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/Aq.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4337 2023-12-11 23:14:15.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/Overlays.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2950 2024-02-02 15:19:02.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/Svtav1Speed.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5719 2023-12-11 23:14:15.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/Svtav1Tunes.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3749 2023-12-11 23:14:15.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/TemporalFiltering.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-06 18:23:30.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2501 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/ai_feature_extract.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      319 2023-12-10 22:37:13.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/aom_extract.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5797 2024-05-30 02:25:08.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/convexhull.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    16870 2024-05-30 02:25:07.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/crf_vmaf_relation.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4926 2024-05-30 02:25:07.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/denoise.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2195 2024-05-30 02:25:08.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/sequence_convex.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      254 2024-05-30 02:23:03.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/serialise_context.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      798 2024-05-30 02:18:47.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/streaming_output.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6592 2023-12-11 23:14:15.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/superres.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4106 2023-11-15 20:26:48.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/target_vmaf.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.198224 alabamaencoder-0.5.0/alabamaEncode/experiments/util/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11478 2024-02-04 12:09:55.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/util/ExperimentUtil.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-10-17 18:48:28.000000 alabamaencoder-0.5.0/alabamaEncode/experiments/util/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.198224 alabamaencoder-0.5.0/alabamaEncode/metrics/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-17 22:15:46.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5252 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/calculate.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      911 2023-11-22 22:07:47.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/comparison_display.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      384 2024-01-26 03:01:39.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/exception.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3043 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/image.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.198224 alabamaencoder-0.5.0/alabamaEncode/metrics/impl/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-02-04 12:02:29.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/impl/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      934 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/impl/psnr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1442 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/impl/ssim.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3108 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/impl/ssimu2.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9098 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/impl/vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      117 2024-02-04 12:09:55.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/metric.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      373 2024-02-04 12:36:30.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/options.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      308 2024-02-02 14:53:33.000000 alabamaencoder-0.5.0/alabamaEncode/metrics/result.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.198224 alabamaencoder-0.5.0/alabamaEncode/parallel_execution/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-16 16:38:33.000000 alabamaencoder-0.5.0/alabamaEncode/parallel_execution/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      865 2024-05-30 02:29:55.000000 alabamaencoder-0.5.0/alabamaEncode/parallel_execution/celery_app.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3853 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/parallel_execution/celery_autoscaler.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      148 2023-11-05 09:04:10.000000 alabamaencoder-0.5.0/alabamaEncode/parallel_execution/command.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12824 2024-05-30 02:29:55.000000 alabamaencoder-0.5.0/alabamaEncode/parallel_execution/execute_commands.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      415 2024-05-30 02:29:55.000000 alabamaencoder-0.5.0/alabamaEncode/parallel_execution/worker.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.202224 alabamaencoder-0.5.0/alabamaEncode/scene/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-15 20:18:27.000000 alabamaencoder-0.5.0/alabamaEncode/scene/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1810 2024-03-29 15:35:11.000000 alabamaencoder-0.5.0/alabamaEncode/scene/annel.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9700 2024-05-30 02:18:05.000000 alabamaencoder-0.5.0/alabamaEncode/scene/chunk.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13591 2024-05-30 02:19:21.000000 alabamaencoder-0.5.0/alabamaEncode/scene/concat.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11209 2024-05-30 02:25:07.000000 alabamaencoder-0.5.0/alabamaEncode/scene/scene_detection.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4456 2024-05-30 02:18:05.000000 alabamaencoder-0.5.0/alabamaEncode/scene/sequence.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 16:09:21.202224 alabamaencoder-0.5.0/alabamaEncoder.egg-info/
--rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      377 2024-05-30 16:09:21.000000 alabamaencoder-0.5.0/alabamaEncoder.egg-info/PKG-INFO
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5807 2024-05-30 16:09:21.000000 alabamaencoder-0.5.0/alabamaEncoder.egg-info/SOURCES.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        1 2024-05-30 16:09:21.000000 alabamaencoder-0.5.0/alabamaEncoder.egg-info/dependency_links.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       67 2024-05-30 16:09:21.000000 alabamaencoder-0.5.0/alabamaEncoder.egg-info/entry_points.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      124 2024-05-30 16:09:21.000000 alabamaencoder-0.5.0/alabamaEncoder.egg-info/requires.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       14 2024-05-30 16:09:21.000000 alabamaencoder-0.5.0/alabamaEncoder.egg-info/top_level.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-05-30 16:09:21.202224 alabamaencoder-0.5.0/setup.cfg
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      538 2024-05-30 16:08:35.000000 alabamaencoder-0.5.0/setup.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.920935 alabamaencoder-0.5.1/
+-rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      377 2024-06-01 17:03:53.920935 alabamaencoder-0.5.1/PKG-INFO
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.892934 alabamaencoder-0.5.1/alabamaEncode/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2021-04-17 09:55:33.000000 alabamaencoder-0.5.1/alabamaEncode/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.892934 alabamaencoder-0.5.1/alabamaEncode/ai_vmaf/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 08:49:47.000000 alabamaencoder-0.5.1/alabamaEncode/ai_vmaf/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1564 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/ai_vmaf/aom_firstpass.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1026 2023-12-18 07:05:43.000000 alabamaencoder-0.5.1/alabamaEncode/ai_vmaf/perdict.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.892934 alabamaencoder-0.5.1/alabamaEncode/ai_vmaf/train/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 10:35:40.000000 alabamaencoder-0.5.1/alabamaEncode/ai_vmaf/train/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12402 2023-12-14 22:03:21.000000 alabamaencoder-0.5.1/alabamaEncode/ai_vmaf/train/train.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.892934 alabamaencoder-0.5.1/alabamaEncode/cli/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:52:09.000000 alabamaencoder-0.5.1/alabamaEncode/cli/__init__.py
+-rwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)     4898 2024-05-30 02:35:51.000000 alabamaencoder-0.5.1/alabamaEncode/cli/__main__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.892934 alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 18:44:18.000000 alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4150 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/autopaths.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    19843 2024-05-31 14:08:46.000000 alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/cli_args.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1162 2024-03-05 20:46:37.000000 alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/paths.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      795 2024-05-30 02:02:54.000000 alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/ratecontrol.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1130 2023-12-10 18:44:44.000000 alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/res_preset.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1992 2024-06-01 01:04:42.000000 alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/validate_files.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1182 2024-05-30 02:17:46.000000 alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/video_filters.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.896934 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:25:35.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.896934 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:35.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.896934 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-17 00:34:57.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1064 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3401 2024-03-05 22:28:46.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4061 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10641 2024-05-30 02:25:07.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      597 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      606 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5598 2024-05-31 00:45:18.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      448 2023-12-10 19:05:23.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/chunk_analyse_step.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      623 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/final_encode_step.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.896934 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-05 14:55:01.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11068 2024-05-31 00:43:48.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6476 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2292 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      850 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2495 2024-05-31 15:11:22.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/opinionated_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4887 2024-05-30 02:10:49.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/pipelines.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      133 2024-01-15 01:49:31.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/refine_step.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.900935 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/refine_steps/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-14 19:17:26.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/refine_steps/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4965 2024-05-30 02:18:47.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/refine_steps/multires_package.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7817 2024-01-20 18:40:41.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.900935 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:49.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1563 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/args_tune.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4702 2024-05-30 02:23:07.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/autocrop.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      552 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/denoise_filtering.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2409 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/encoding_tiles.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7516 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6001 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/sequence_autograin.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3092 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3103 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/x264_tune.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.900935 alabamaencoder-0.5.1/alabamaEncode/core/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-19 23:19:38.000000 alabamaencoder-0.5.1/alabamaEncode/core/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3885 2024-05-30 02:29:55.000000 alabamaencoder-0.5.1/alabamaEncode/core/chunk_job.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10683 2024-05-31 00:46:26.000000 alabamaencoder-0.5.1/alabamaEncode/core/context.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.904935 alabamaencoder-0.5.1/alabamaEncode/core/extras/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-24 18:44:15.000000 alabamaencoder-0.5.1/alabamaEncode/core/extras/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12749 2024-05-30 02:32:33.000000 alabamaencoder-0.5.1/alabamaEncode/core/extras/auto_thumbnailer.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1776 2023-12-24 03:53:49.000000 alabamaencoder-0.5.1/alabamaEncode/core/extras/ws_update.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    14459 2024-05-31 15:14:10.000000 alabamaencoder-0.5.1/alabamaEncode/core/ffmpeg.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7604 2024-05-31 15:27:03.000000 alabamaencoder-0.5.1/alabamaEncode/core/final_touches.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    19286 2024-05-31 15:12:12.000000 alabamaencoder-0.5.1/alabamaEncode/core/job.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.904935 alabamaencoder-0.5.1/alabamaEncode/core/util/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-30 02:17:11.000000 alabamaencoder-0.5.1/alabamaEncode/core/util/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      125 2024-05-30 02:20:37.000000 alabamaencoder-0.5.1/alabamaEncode/core/util/abort_controler.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2895 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/core/util/bin_utils.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4947 2024-01-31 09:31:42.000000 alabamaencoder-0.5.1/alabamaEncode/core/util/cli_executor.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      773 2024-05-30 02:32:32.000000 alabamaencoder-0.5.1/alabamaEncode/core/util/get_yuv_stream.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1877 2024-04-22 19:11:27.000000 alabamaencoder-0.5.1/alabamaEncode/core/util/kv.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      813 2023-11-25 00:35:54.000000 alabamaencoder-0.5.1/alabamaEncode/core/util/path.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      556 2023-11-12 21:29:16.000000 alabamaencoder-0.5.1/alabamaEncode/core/util/timer.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3758 2024-05-25 22:57:08.000000 alabamaencoder-0.5.1/alabamaEncode/core/util/yuv.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.904935 alabamaencoder-0.5.1/alabamaEncode/demon/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:38:55.000000 alabamaencoder-0.5.1/alabamaEncode/demon/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2289 2024-03-05 20:43:08.000000 alabamaencoder-0.5.1/alabamaEncode/demon/demon.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.904935 alabamaencoder-0.5.1/alabamaEncode/encoder/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-09-27 12:09:43.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      748 2024-01-17 00:16:49.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/codec.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11448 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/encoder.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1628 2024-05-29 16:04:18.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/encoder_factory.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.908935 alabamaencoder-0.5.1/alabamaEncode/encoder/impl/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4379 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/impl/Aomenc.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2092 2024-05-30 02:18:47.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/impl/Nvenc.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1596 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/impl/SvtAvif.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7672 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/impl/Svtenc.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2177 2024-05-30 02:18:47.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/impl/VaapiH264.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2119 2024-05-30 02:18:47.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/impl/VaapiH265.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2315 2024-05-30 02:18:47.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/impl/VideoToolbox.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7253 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/impl/X264.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3626 2024-05-31 20:04:23.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/impl/X265.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2022-12-05 03:43:14.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/impl/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2043 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/impl/rav1e.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3567 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/impl/vp9.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      269 2024-01-17 00:14:46.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/rate_dist.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2494 2024-02-04 12:07:28.000000 alabamaencoder-0.5.1/alabamaEncode/encoder/stats.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.912935 alabamaencoder-0.5.1/alabamaEncode/experiments/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3713 2023-12-11 23:14:15.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/Aq.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4337 2023-12-11 23:14:15.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/Overlays.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2950 2024-02-02 15:19:02.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/Svtav1Speed.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5719 2023-12-11 23:14:15.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/Svtav1Tunes.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3749 2023-12-11 23:14:15.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/TemporalFiltering.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-06 18:23:30.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2501 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/ai_feature_extract.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      319 2023-12-10 22:37:13.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/aom_extract.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5797 2024-05-30 02:25:08.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/convexhull.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    16870 2024-05-30 02:25:07.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/crf_vmaf_relation.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4926 2024-05-30 02:25:07.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/denoise.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2195 2024-05-30 02:25:08.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/sequence_convex.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      254 2024-05-30 02:23:03.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/serialise_context.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      798 2024-05-30 02:18:47.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/streaming_output.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6592 2023-12-11 23:14:15.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/superres.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4106 2023-11-15 20:26:48.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/target_vmaf.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.912935 alabamaencoder-0.5.1/alabamaEncode/experiments/util/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11478 2024-02-04 12:09:55.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/util/ExperimentUtil.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-10-17 18:48:28.000000 alabamaencoder-0.5.1/alabamaEncode/experiments/util/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.916935 alabamaencoder-0.5.1/alabamaEncode/metrics/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-17 22:15:46.000000 alabamaencoder-0.5.1/alabamaEncode/metrics/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5252 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/metrics/calculate.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      911 2023-11-22 22:07:47.000000 alabamaencoder-0.5.1/alabamaEncode/metrics/comparison_display.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      384 2024-01-26 03:01:39.000000 alabamaencoder-0.5.1/alabamaEncode/metrics/exception.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3043 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/metrics/image.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.916935 alabamaencoder-0.5.1/alabamaEncode/metrics/impl/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-02-04 12:02:29.000000 alabamaencoder-0.5.1/alabamaEncode/metrics/impl/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      934 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/metrics/impl/psnr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1442 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/metrics/impl/ssim.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3108 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/metrics/impl/ssimu2.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9258 2024-05-31 00:22:51.000000 alabamaencoder-0.5.1/alabamaEncode/metrics/impl/vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      117 2024-02-04 12:09:55.000000 alabamaencoder-0.5.1/alabamaEncode/metrics/metric.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      373 2024-02-04 12:36:30.000000 alabamaencoder-0.5.1/alabamaEncode/metrics/options.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      308 2024-02-02 14:53:33.000000 alabamaencoder-0.5.1/alabamaEncode/metrics/result.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.916935 alabamaencoder-0.5.1/alabamaEncode/parallel_execution/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-16 16:38:33.000000 alabamaencoder-0.5.1/alabamaEncode/parallel_execution/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      865 2024-05-30 02:29:55.000000 alabamaencoder-0.5.1/alabamaEncode/parallel_execution/celery_app.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3853 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/parallel_execution/celery_autoscaler.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      148 2023-11-05 09:04:10.000000 alabamaencoder-0.5.1/alabamaEncode/parallel_execution/command.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12824 2024-05-30 02:29:55.000000 alabamaencoder-0.5.1/alabamaEncode/parallel_execution/execute_commands.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      415 2024-05-30 02:29:55.000000 alabamaencoder-0.5.1/alabamaEncode/parallel_execution/worker.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.920935 alabamaencoder-0.5.1/alabamaEncode/scene/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-15 20:18:27.000000 alabamaencoder-0.5.1/alabamaEncode/scene/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1810 2024-03-29 15:35:11.000000 alabamaencoder-0.5.1/alabamaEncode/scene/annel.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9700 2024-05-30 02:18:05.000000 alabamaencoder-0.5.1/alabamaEncode/scene/chunk.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13591 2024-05-30 02:19:21.000000 alabamaencoder-0.5.1/alabamaEncode/scene/concat.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11209 2024-05-30 02:25:07.000000 alabamaencoder-0.5.1/alabamaEncode/scene/scene_detection.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4456 2024-05-30 02:18:05.000000 alabamaencoder-0.5.1/alabamaEncode/scene/sequence.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-06-01 17:03:53.920935 alabamaencoder-0.5.1/alabamaEncoder.egg-info/
+-rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      377 2024-06-01 17:03:53.000000 alabamaencoder-0.5.1/alabamaEncoder.egg-info/PKG-INFO
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5807 2024-06-01 17:03:53.000000 alabamaencoder-0.5.1/alabamaEncoder.egg-info/SOURCES.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        1 2024-06-01 17:03:53.000000 alabamaencoder-0.5.1/alabamaEncoder.egg-info/dependency_links.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       67 2024-06-01 17:03:53.000000 alabamaencoder-0.5.1/alabamaEncoder.egg-info/entry_points.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      124 2024-06-01 17:03:53.000000 alabamaencoder-0.5.1/alabamaEncoder.egg-info/requires.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       14 2024-06-01 17:03:53.000000 alabamaencoder-0.5.1/alabamaEncoder.egg-info/top_level.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-06-01 17:03:53.920935 alabamaencoder-0.5.1/setup.cfg
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      538 2024-06-01 17:03:39.000000 alabamaencoder-0.5.1/setup.py
```

### Comparing `alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/aom_firstpass.py` & `alabamaencoder-0.5.1/alabamaEncode/ai_vmaf/aom_firstpass.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/perdict.py` & `alabamaencoder-0.5.1/alabamaEncode/ai_vmaf/perdict.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/ai_vmaf/train/train.py` & `alabamaencoder-0.5.1/alabamaEncode/ai_vmaf/train/train.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/cli/__main__.py` & `alabamaencoder-0.5.1/alabamaEncode/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/autopaths.py` & `alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/autopaths.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/cli_args.py` & `alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/cli_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,15 @@
         default=ctx.chunk_order,
         choices=[
             "random",
             "sequential",
             "length_desc",
             "length_asc",
             "sequential_reverse",
+            "even"
         ],
         dest="chunk_order",
     )
 
     parser.add_argument(
         "--start_offset",
         help="Offset from the beginning of the video (in seconds), useful for cutting intros etc",
@@ -359,28 +360,42 @@
         type=str,
         default=ctx.sub_file,
         help="Subtitles file, eg .srt or .vvt",
         dest="sub_file",
     )
 
     parser.add_argument(
+        "--crf_limits",
+        type=str,
+        help="limits for crf when targeting vmaf, comma separated eg 20,35",
+        dest="crf_limits",
+    )
+
+    parser.add_argument(
         "--vmaf_phone_model",
         action="store_true",
         help="use vmaf phone model for auto crf tuning",
         default=ctx.vmaf_phone_model,
     )
 
     parser.add_argument(
         "--vmaf_4k_model",
         action="store_true",
         help="use vmaf 4k model for auto crf tuning",
         dest="vmaf_4k_model",
     )
 
     parser.add_argument(
+        '--vmaf_subsample',
+        type=int,
+        help="compute scores only every N frames",
+        dest="vmaf_subsample"
+    )
+
+    parser.add_argument(
         "--vmaf_no_motion",
         action="store_true",
         help="use vmaf no motion model for auto crf tuning",
         dest="vmaf_no_motion",
     )
 
     parser.add_argument(
@@ -404,18 +419,17 @@
         default=ctx.probe_count,
         help="Max number of probes for metric targeting, higher is more accurate but slower",
         action=range_action(1, 10),
         dest="probe_count",
     )
 
     parser.add_argument(
-        "--probe_speed",
-        dest="probe_speed_override",
+        "--vmaf_probe_speed",
+        dest="vmaf_probe_speed",
         type=int,
-        default=ctx.prototype_encoder.speed,
         help="Override the speed for target vmaf probes",
         action=range_action(0, 10),
     )
 
     parser.add_argument(
         "--vmaf_reference_display",
         type=str,
@@ -597,22 +611,24 @@
     ctx.prototype_encoder.matrix_coefficients = args.matrix_coefficients
     ctx.prototype_encoder.maximum_content_light_level = args.maximum_content_light_level
     ctx.prototype_encoder.maximum_frame_average_light_level = args.frame_average_light
     ctx.prototype_encoder.chroma_sample_position = args.chroma_sample_position
     ctx.prototype_encoder.video_filters = args.video_filters
     ctx.auto_crop = args.auto_crop
     ctx.bitrate_string = args.bitrate
+    ctx.crf_limits = args.crf_limits
     ctx.vmaf_phone_model = args.vmaf_phone_model
     ctx.vmaf_4k_model = args.vmaf_4k_model
+    ctx.vmaf_subsample = args.vmaf_subsample
     ctx.vmaf_no_motion = args.vmaf_no_motion
     ctx.auto_accept_autocrop = args.auto_accept_autocrop
     ctx.resolution_preset = args.resolution_preset
     ctx.probe_count = args.probe_count
     ctx.vmaf_reference_display = args.vmaf_reference_display
-    ctx.probe_speed_override = args.probe_speed_override
+    ctx.vmaf_probe_speed = args.vmaf_probe_speed
     ctx.crf_map = args.crf_map
     ctx.pin_to_cores = args.dont_pin_to_cores
     ctx.prototype_encoder.niceness = args.niceness
     ctx.vmaf_target_representation = args.vmaf_target_repesentation
     ctx.print_analysis_logs = args.print_analysis_logs
     ctx.poster_url = args.poster_url
     ctx.offload_server = args.offload_server
```

### Comparing `alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/paths.py` & `alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/paths.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/ratecontrol.py` & `alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/ratecontrol.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/res_preset.py` & `alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/res_preset.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/validate_files.py` & `alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/validate_files.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/cli/cli_setup/video_filters.py` & `alabamaencoder-0.5.1/alabamaEncode/cli/cli_setup/video_filters.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                 return float(result_from_kv)
 
             enc_copy.crf = _crf
             enc_copy.output_path = os.path.join(
                 probe_file_base,
                 f"probe.{_crf}{enc_copy.get_chunk_file_extension()}",
             )
-            enc_copy.speed = max(get_vmaf_probe_speed(enc_copy), enc.speed)
+            enc_copy.speed = max(get_vmaf_probe_speed(enc_copy, ctx), enc.speed)
             enc_copy.override_flags = None
             # TODO: calculate metrics outside enc.run to add the flexibility to calc other ones
             stats: EncodeStats = enc_copy.run(
                 metric_to_calculate=metric,
                 metric_params=ctx.get_vmaf_options(),
                 override_if_exists=False,
             )
@@ -71,22 +71,22 @@
         if probes > 3:
             ctx.log(
                 f"probe count in TargetVmaf is set to {probes}, this is too high, <=3",
                 level=1,
             )
 
         trys = []
-        low_crf, high_crf = get_crf_limits(enc_copy)
+        low_crf, high_crf = get_crf_limits(enc_copy, ctx)
         depth = 0
         mid_crf = 0
         while low_crf <= high_crf and depth < probes:
             mid_crf = (low_crf + high_crf) // 2
 
             if (depth == 2 and ctx.probe_count == 3) or (depth == 1 and ctx.probe_count == 2):
-                ll, lh = get_crf_limits(enc_copy)
+                ll, lh = get_crf_limits(enc_copy, ctx)
                 m = (ll + lh) // 2
                 # if closer to edge then the middle, use that edge
                 if abs(mid_crf - ll) < abs(mid_crf - m):
                     mid_crf = ll
                 else:
                     mid_crf = lh
 
@@ -134,15 +134,15 @@
                 crf = crf_low + (crf_high - crf_low) * (
                     (target_metric - metric_low) / (metric_high - metric_low)
                 )
 
                 if not enc_copy.supports_float_crfs():
                     crf = int(crf)
 
-                crf_min, crf_max = get_crf_limits(enc_copy)
+                crf_min, crf_max = get_crf_limits(enc_copy, ctx)
 
                 crf = max(min(crf, crf_max), crf_min)
         else:
             crf = mid_crf
 
         ctx.log(f"{chunk.log_prefix()}Decided on crf: {crf}", category="probe")
```

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_step.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/final_encode_step.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         enc.rate_distribution = EncoderRateDistribution.CQ
 
         best_crf_from_kv = ctx.get_kv().get("best_crfs", chunk.chunk_index)
         if best_crf_from_kv is not None:
             _, stats, _, _, _ = run_probe(best_crf_from_kv)
             return finish(stats, best_crf_from_kv)
 
-        low_crf, high_crf = get_crf_limits(enc)
+        low_crf, high_crf = get_crf_limits(enc, ctx)
         max_score_error = 0.7
 
         tol = 0.10 if enc.supports_float_crfs() else 1
         gr = (1 + 5**0.5) / 2
 
         a = high_crf - (high_crf - low_crf) / gr
         b = low_crf + (high_crf - low_crf) / gr
```

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/opinionated_vmaf.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/opinionated_vmaf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-
 from alabamaEncode.encoder.codec import Codec
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.impl.Aomenc import EncoderAom
 from alabamaEncode.encoder.impl.Svtenc import EncoderSvt
 from alabamaEncode.encoder.impl.VideoToolbox import EncoderAppleHEVC
 
 
@@ -20,18 +18,18 @@
             return 0, 63
         case Codec.vp9:
             return 0, 63
         case _:
             raise ValueError(f"FATAL: Unknown codec: {codec}")
 
 
-def get_vmaf_probe_speed(encoder: Encoder) -> int:
-    env_name = "VMAF_PROBE_SPEED"
-    if env_name in os.environ:
-        return int(os.environ[env_name])
+def get_vmaf_probe_speed(encoder: Encoder, ctx=None) -> int:
+    if ctx is not None:
+        if ctx.vmaf_probe_speed != -1:
+            return ctx.vmaf_probe_speed
     match encoder:
         case EncoderSvt():
             return 13
         case _:
             # TODO: pick other values
             return 5
 
@@ -49,18 +47,18 @@
     match codec:
         case Codec.av1:
             return ["1920:-2", "1280:-2", "960:-2", "854:-2"]
         case _:
             return ["1920:-2", "1280:-2", "960:-2", "854:-2", "768:-2", "480:-2"]
 
 
-def get_crf_limits(encoder: Encoder) -> tuple[int, int]:
-    env_name = "CRF_LIMITS"
-    if env_name in os.environ:
-        return tuple(map(int, os.environ[env_name].split(",")))
+def get_crf_limits(encoder: Encoder, ctx=None) -> tuple[int, int]:
+    if ctx is not None:
+        if ctx.crf_limits is not None:
+            return tuple(map(int, ctx.crf_limits.split(",")))
     match encoder.get_codec():
         case Codec.av1:
             match encoder:
                 case EncoderSvt():
                     return 20, 35
                 case _:
                     return 18, 40
```

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/pipelines.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/pipelines.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/refine_steps/multires_package.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/refine_steps/multires_package.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/args_tune.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/args_tune.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/autocrop.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/autocrop.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/denoise_filtering.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/denoise_filtering.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/encoding_tiles.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/encoding_tiles.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/sequence_autograin.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/sequence_autograin.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/conent_analysis/sequence/x264_tune.py` & `alabamaencoder-0.5.1/alabamaEncode/conent_analysis/sequence/x264_tune.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/core/chunk_job.py` & `alabamaencoder-0.5.1/alabamaEncode/core/chunk_job.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/core/context.py` & `alabamaencoder-0.5.1/alabamaEncode/core/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,20 @@
             "cutoff_bitrate": self.cutoff_bitrate,
             "max_bitrate": self.max_bitrate,
             "simple_denoise": self.simple_denoise,
             "vmaf": self.vmaf,
             "probe_count": self.probe_count,
             "vmaf_reference_display": self.vmaf_reference_display,
             "crf_based_vmaf_targeting": self.crf_based_vmaf_targeting,
+            "crf_limits": self.crf_limits,
             "vmaf_4k_model": self.vmaf_4k_model,
             "vmaf_phone_model": self.vmaf_phone_model,
             "vmaf_no_motion": self.vmaf_no_motion,
-            "probe_speed_override": self.probe_speed_override,
+            "vmaf_subsample": self.vmaf_subsample,
+            "vmaf_probe_speed": self.vmaf_probe_speed,
             "vmaf_target_representation": self.vmaf_target_representation,
             "crf_map": self.crf_map,
             "max_scene_length": self.max_scene_length,
             "start_offset": self.start_offset,
             "end_offset": self.end_offset,
             "override_scenecache_path_check": self.override_scenecache_path_check,
             "title": self.title,
@@ -142,24 +144,26 @@
     bitrate_adjust_mode: str = ""
     cutoff_bitrate: int = -1
     max_bitrate: int = 0
     simple_denoise = False
     args_tune = "appeal"
     calc_final_vmaf = False
 
+    crf_limits = None
     metric_to_target = "vmaf"
     vmaf: int = 96
+    vmaf_subsample = -1
     denoise_vmaf_ref = False
     probe_count = 2
     vmaf_reference_display = ""
     crf_based_vmaf_targeting = True
     vmaf_4k_model = False
     vmaf_phone_model = False
     vmaf_no_motion = False
-    probe_speed_override = prototype_encoder.speed
+    vmaf_probe_speed = -1
     vmaf_target_representation = "mean"
     dynamic_vmaf_target = False
     dynamic_vmaf_target_vbr = False
     best_crfs = []
 
     crf_map = ""
 
@@ -216,14 +220,15 @@
             ref=(
                 ComparisonDisplayResolution.from_string(self.vmaf_reference_display)
                 if self.vmaf_reference_display
                 else None
             ),
             no_motion=self.vmaf_no_motion,
             denoise_refrence=self.denoise_vmaf_ref,
+            subsample=self.vmaf_subsample
         )
 
     def get_metric_target(self) -> Tuple[Metric, float]:
         """
         Return what metric and to what degree to target based on config
         TO BE FILLED
         """
```

### Comparing `alabamaencoder-0.5.0/alabamaEncode/core/extras/auto_thumbnailer.py` & `alabamaencoder-0.5.1/alabamaEncode/core/extras/auto_thumbnailer.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/core/extras/ws_update.py` & `alabamaencoder-0.5.1/alabamaEncode/core/extras/ws_update.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/core/ffmpeg.py` & `alabamaencoder-0.5.1/alabamaEncode/core/ffmpeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,37 @@
             )
             .verify()
             .strip_mp4_warning()
             .get_as_int()
         )
 
     @staticmethod
+    def get_pix_fmt(path: PathAlabama) -> str:
+        path.check_video()
+        return (
+            run_cli(
+                f"ffprobe -v error -select_streams v:0 -show_entries stream=pix_fmt "
+                f"-of default=noprint_wrappers=1:nokey=1 {path.get_safe()}"
+            )
+            .verify()
+            .strip_mp4_warning()
+            .get_output()
+        )
+
+    @staticmethod
+    def get_bit_depth(path: PathAlabama) -> int:
+        pix_fmt = Ffmpeg.get_pix_fmt(path)
+        if pix_fmt == "yuv420p":
+            return 8
+        elif pix_fmt == "yuv420p10le":
+            return 10
+        else:
+            raise NotImplemented(f"could not parse bitdepth out of: {pix_fmt}; please report it")
+
+    @staticmethod
     def is_hdr(path: PathAlabama) -> bool:
         """Check if a video is HDR"""
         path.check_video()
         out = (
             run_cli(
                 (
                     f"ffprobe -v quiet -show_entries stream=color_transfer "
```

### Comparing `alabamaencoder-0.5.0/alabamaEncode/core/job.py` & `alabamaencoder-0.5.1/alabamaEncode/core/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,19 @@
 from alabamaEncode.conent_analysis.pipelines import (
     run_sequence_pipeline,
     get_refine_steps,
 )
 from alabamaEncode.core.chunk_job import ChunkEncoder
 from alabamaEncode.core.context import AlabamaContext
 from alabamaEncode.core.extras.ws_update import WebsocketServer
-from alabamaEncode.core.ffmpeg import Ffmpeg
 from alabamaEncode.core.final_touches import (
     print_stats,
     generate_previews,
     create_torrent_file,
 )
-from alabamaEncode.core.util.path import PathAlabama
 from alabamaEncode.parallel_execution.celery_app import app
 from alabamaEncode.parallel_execution.execute_commands import execute_commands
 from alabamaEncode.scene.annel import annealing
 from alabamaEncode.scene.concat import VideoConcatenator
 from alabamaEncode.scene.scene_detection import scene_detect
 from alabamaEncode.scene.sequence import ChunkSequence
 
@@ -341,14 +339,16 @@
                         command_objects.sort(
                             key=lambda x: x.job.chunk.length, reverse=True
                         )
                     elif ctx.chunk_order == "sequential":
                         pass
                     elif ctx.chunk_order == "sequential_reverse":
                         command_objects.reverse()
+                    elif ctx.chunk_order == "even":
+                        command_objects = annealing(command_objects, 1000)
                     else:
                         raise ValueError(f"Invalid chunk order: {ctx.chunk_order}")
 
                     if ctx.throughput_scaling:
                         # make the chunk length distribution homogenous
                         command_objects = annealing(command_objects, 1000)
 
@@ -427,27 +427,27 @@
         self.update_proc_done(99)
         self.update_current_step_name("Final touches")
 
         if self.ctx.generate_stats:
             print_stats(
                 output_folder=self.ctx.output_folder,
                 output=self.ctx.output_file,
-                input_file=self.ctx.raw_input_file,
-                grain_synth=self.ctx.prototype_encoder.grain_synth,
+                # input_file=self.ctx.raw_input_file,
+                # grain_synth=self.ctx.prototype_encoder.grain_synth,
                 title=self.ctx.get_title(),
-                cut_intro=(True if self.ctx.start_offset > 0 else False),
-                cut_credits=(True if self.ctx.end_offset > 0 else False),
-                croped=(True if self.ctx.crop_string != "" else False),
-                scaled=(True if self.ctx.scale_string != "" else False),
-                tonemaped=(
-                    True
-                    if not self.ctx.prototype_encoder.hdr
-                    and Ffmpeg.is_hdr(PathAlabama(self.ctx.input_file))
-                    else False
-                ),
+                # cut_intro=(True if self.ctx.start_offset > 0 else False),
+                # cut_credits=(True if self.ctx.end_offset > 0 else False),
+                # croped=(True if self.ctx.crop_string != "" else False),
+                # scaled=(True if self.ctx.scale_string != "" else False),
+                # tonemaped=(
+                #     True
+                #     if not self.ctx.prototype_encoder.hdr
+                #     and Ffmpeg.is_hdr(PathAlabama(self.ctx.input_file))
+                #     else False
+                # ),
             )
         if self.ctx.generate_previews:
             generate_previews(
                 input_file=self.ctx.output_file, output_folder=self.ctx.output_folder
             )
             create_torrent_file(
                 video=self.ctx.output_file,
```

### Comparing `alabamaencoder-0.5.0/alabamaEncode/core/util/bin_utils.py` & `alabamaencoder-0.5.1/alabamaEncode/core/util/bin_utils.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/core/util/cli_executor.py` & `alabamaencoder-0.5.1/alabamaEncode/core/util/cli_executor.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/core/util/get_yuv_stream.py` & `alabamaencoder-0.5.1/alabamaEncode/core/util/get_yuv_stream.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/core/util/kv.py` & `alabamaencoder-0.5.1/alabamaEncode/core/util/kv.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/core/util/path.py` & `alabamaencoder-0.5.1/alabamaEncode/core/util/path.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/core/util/timer.py` & `alabamaencoder-0.5.1/alabamaEncode/core/util/timer.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/core/util/yuv.py` & `alabamaencoder-0.5.1/alabamaEncode/core/util/yuv.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/demon/demon.py` & `alabamaencoder-0.5.1/alabamaEncode/demon/demon.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/encoder/codec.py` & `alabamaencoder-0.5.1/alabamaEncode/encoder/codec.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/encoder/encoder.py` & `alabamaencoder-0.5.1/alabamaEncode/encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/encoder/encoder_factory.py` & `alabamaencoder-0.5.1/alabamaEncode/encoder/encoder_factory.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/Aomenc.py` & `alabamaencoder-0.5.1/alabamaEncode/encoder/impl/Aomenc.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/Nvenc.py` & `alabamaencoder-0.5.1/alabamaEncode/encoder/impl/Nvenc.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/SvtAvif.py` & `alabamaencoder-0.5.1/alabamaEncode/encoder/impl/SvtAvif.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/Svtenc.py` & `alabamaencoder-0.5.1/alabamaEncode/encoder/impl/Svtenc.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/VaapiH264.py` & `alabamaencoder-0.5.1/alabamaEncode/encoder/impl/VaapiH264.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/VaapiH265.py` & `alabamaencoder-0.5.1/alabamaEncode/encoder/impl/VaapiH265.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/VideoToolbox.py` & `alabamaencoder-0.5.1/alabamaEncode/encoder/impl/VideoToolbox.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/X264.py` & `alabamaencoder-0.5.1/alabamaEncode/encoder/impl/X264.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/X265.py` & `alabamaencoder-0.5.1/alabamaEncode/encoder/impl/X265.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,18 @@
         return "X265"
 
     def get_codec(self) -> Codec:
         return Codec.h265
 
     def get_version(self) -> str:
         return (
-            run_cli(f"{get_binary('x264')} --help")
+            run_cli(f"{get_binary('x265')} --help")
             .get_output()
             .split("\n")[0]
-            .replace("x265", "")
+            .replace("x265 [info]: HEVC encoder version ", "")
             .strip()
         )
 
     def get_encode_commands(self) -> List[str]:
         if self.speed == 0:
             self.speed = 1
 
@@ -45,24 +45,17 @@
                 f"--colormatrix={colormatrix} --chromaloc={chromeloc} "
                 f"--max-cll {self.maximum_content_light_level},{self.maximum_frame_average_light_level}"
             )
             kommand += f" --hdr10 "
             # if self.svt_master_display:
             #     kommand += f' --mastering-display "{self.svt_master_display}" '
 
-        kommand += (
-            " --wpp --ctu=64 --tu-intra-depth=2 --me=3 --subme=3 --merange=57 --rect --amp --max-merge=3 -"
-            "-temporal-mvp --no-early-skip --rdpenalty=0 --no-tskip --no-tskip-fast --strong-intra-smoothing "
-            "--no-lossless --no-cu-lossless --no-constrained-intra --no-fast-intra --open-gop --interlace=0 "
-            "--min-keyint=24 --scenecut=40 --rc-lookahead=30 --bframes=8 "
-            "--bframe-bias=0 --b-adapt=2 --ref=3 --weightp --weightb --aq-mode=2 --aq-strength=1.00 "
-            "--cbqpoffs=0 --crqpoffs=0 --rd=6 --psy-rd=0.00 --psy-rdoq=0.00 --signhide --lft --sao "
-            "--no-sao-non-deblock --b-pyramid --cutree --qcomp=0.60 --qpmin=0 --qpstep=4 --ipratio=1.40"
-            " --pbratio=1.30 "
-        )
+        kommand += " --no-scenecut "
+
+        kommand += f" --keyint={self.keyint} "
 
         match self.rate_distribution:
             case EncoderRateDistribution.CQ:
                 kommand += f" --crf={self.crf}"
             case _:
                 raise Exception(
                     f"FATAL: rate distribution {self.rate_distribution} not supported"
@@ -86,16 +79,14 @@
             case 2:
                 kommand += " --preset=slower"
             case 1:
                 kommand += " --preset=veryslow"
             case 0:
                 kommand += " --preset=placebo"
 
-        kommand += f" --keyint={self.keyint} "
-
         if self.passes == 2:
             raise Exception("FATAL: 2 pass encoding not supported")
         elif self.passes == 1:
             hevc_file = self.output_path.replace(".mkv", ".hevc")
             remux_command = (
                 f'{get_binary("mkvmerge")} -o "{self.output_path}" "{hevc_file}"'
             )
@@ -103,7 +94,16 @@
             return [f'{kommand} -o "{hevc_file}"', remux_command, del_commnad]
 
     def get_chunk_file_extension(self) -> str:
         return ".mkv"
 
     def supports_float_crfs(self) -> bool:
         return True
+
+
+if __name__ == '__main__':
+    x265 = EncoderX265()
+    print(x265.get_pretty_name())
+    print(x265.get_codec())
+    print(x265.get_version())
+    print(x265.get_chunk_file_extension())
+    print(x265.supports_float_crfs())
```

### Comparing `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/rav1e.py` & `alabamaencoder-0.5.1/alabamaEncode/encoder/impl/rav1e.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/encoder/impl/vp9.py` & `alabamaencoder-0.5.1/alabamaEncode/encoder/impl/vp9.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/encoder/stats.py` & `alabamaencoder-0.5.1/alabamaEncode/encoder/stats.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/experiments/Aq.py` & `alabamaencoder-0.5.1/alabamaEncode/experiments/Aq.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/experiments/Overlays.py` & `alabamaencoder-0.5.1/alabamaEncode/experiments/Overlays.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/experiments/Svtav1Speed.py` & `alabamaencoder-0.5.1/alabamaEncode/experiments/Svtav1Speed.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/experiments/Svtav1Tunes.py` & `alabamaencoder-0.5.1/alabamaEncode/experiments/Svtav1Tunes.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/experiments/TemporalFiltering.py` & `alabamaencoder-0.5.1/alabamaEncode/experiments/TemporalFiltering.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/experiments/ai_feature_extract.py` & `alabamaencoder-0.5.1/alabamaEncode/experiments/ai_feature_extract.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/experiments/convexhull.py` & `alabamaencoder-0.5.1/alabamaEncode/experiments/convexhull.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/experiments/crf_vmaf_relation.py` & `alabamaencoder-0.5.1/alabamaEncode/experiments/crf_vmaf_relation.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/experiments/denoise.py` & `alabamaencoder-0.5.1/alabamaEncode/experiments/denoise.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/experiments/sequence_convex.py` & `alabamaencoder-0.5.1/alabamaEncode/experiments/sequence_convex.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/experiments/streaming_output.py` & `alabamaencoder-0.5.1/alabamaEncode/experiments/streaming_output.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/experiments/superres.py` & `alabamaencoder-0.5.1/alabamaEncode/experiments/superres.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/experiments/target_vmaf.py` & `alabamaencoder-0.5.1/alabamaEncode/experiments/target_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/experiments/util/ExperimentUtil.py` & `alabamaencoder-0.5.1/alabamaEncode/experiments/util/ExperimentUtil.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/metrics/calculate.py` & `alabamaencoder-0.5.1/alabamaEncode/metrics/calculate.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/metrics/comparison_display.py` & `alabamaencoder-0.5.1/alabamaEncode/metrics/comparison_display.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/metrics/image.py` & `alabamaencoder-0.5.1/alabamaEncode/metrics/image.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/metrics/impl/psnr.py` & `alabamaencoder-0.5.1/alabamaEncode/metrics/impl/psnr.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/metrics/impl/ssim.py` & `alabamaencoder-0.5.1/alabamaEncode/metrics/impl/ssim.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/metrics/impl/ssimu2.py` & `alabamaencoder-0.5.1/alabamaEncode/metrics/impl/ssimu2.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/metrics/impl/vmaf.py` & `alabamaencoder-0.5.1/alabamaEncode/metrics/impl/vmaf.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 class VmafOptions(MetricOptions):
     def __init__(
         self,
         phone=False,
         uhd=False,
         neg=False,
         no_motion=False,
+        subsample=-1,
         **kwargs,
     ):
         self.phone = phone
         self.uhd = uhd
         self.neg = neg
         self.no_motion = no_motion
+        self.subsample = subsample
         super().__init__(**kwargs)
 
     def get_model(self) -> str:
         models = get_models()
         if self.no_motion:
             return f'path={models["normal_neg_nomotion"]}'
         if self.neg:
@@ -78,14 +80,17 @@
     vmaf_command = (
         f'{get_binary("vmaf")} -q --json --output "{log_path}" --model {vmaf_options.get_model()} '
         f"--reference {ref_pipe} "
         f"--distorted {dist_pipe}"
         f" --threads {vmaf_options.threads}"
     )
 
+    if vmaf_options.subsample != -1:
+        vmaf_command += f" --subsample {vmaf_options.subsample}"
+
     cli_results = run_cli_parallel(
         [
             ref_command,
             dist_command,
             vmaf_command,
         ]
     )
```

### Comparing `alabamaencoder-0.5.0/alabamaEncode/parallel_execution/celery_app.py` & `alabamaencoder-0.5.1/alabamaEncode/parallel_execution/celery_app.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/parallel_execution/celery_autoscaler.py` & `alabamaencoder-0.5.1/alabamaEncode/parallel_execution/celery_autoscaler.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/parallel_execution/execute_commands.py` & `alabamaencoder-0.5.1/alabamaEncode/parallel_execution/execute_commands.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/scene/annel.py` & `alabamaencoder-0.5.1/alabamaEncode/scene/annel.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/scene/chunk.py` & `alabamaencoder-0.5.1/alabamaEncode/scene/chunk.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/scene/concat.py` & `alabamaencoder-0.5.1/alabamaEncode/scene/concat.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/scene/scene_detection.py` & `alabamaencoder-0.5.1/alabamaEncode/scene/scene_detection.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncode/scene/sequence.py` & `alabamaencoder-0.5.1/alabamaEncode/scene/sequence.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/alabamaEncoder.egg-info/SOURCES.txt` & `alabamaencoder-0.5.1/alabamaEncoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.5.0/setup.py` & `alabamaencoder-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="alabamaEncoder",
-    version="0.5.0",
+    version="0.5.1",
     packages=find_packages(),
     install_requires=[
         "scenedetect",
         "tqdm",
         "celery",
         "redis",
         "psutil",
```

