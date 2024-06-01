# Comparing `tmp/nostr_dvm-0.5.4.tar.gz` & `tmp/nostr_dvm-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostr_dvm-0.5.4.tar", last modified: Sat Jun  1 17:18:13 2024, max compression
+gzip compressed data, was "nostr_dvm-0.5.5.tar", last modified: Sat Jun  1 17:31:28 2024, max compression
```

## Comparing `nostr_dvm-0.5.4.tar` & `nostr_dvm-0.5.5.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.956800 nostr_dvm-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-06-01 17:18:13.956800 nostr_dvm-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.940800 nostr_dvm-0.5.4/nostr_dvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.940800 nostr_dvm-0.5.4/nostr_dvm/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.940800 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.940800 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_interrogator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_upscale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/whisperx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/whisperx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    41554 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/dvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/interfaces/dvmtaskinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.952800 nostr_dvm-0.5.4/nostr_dvm/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/advanced_search_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular.py
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py
--rw-r--r--   0 runner    (1001) docker     (127)    13878 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14061 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/convert_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_bot_farms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_censor_wot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_inactive_follows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_nonfollowers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_openai_dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/imageinterrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/imageupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/search_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/summarization_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/summarization_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/textextraction_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/textextraction_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/textextraction_whisperx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/textgeneration_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/textgeneration_llmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/textgeneration_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/texttospeech.py
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/translation_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/translation_libretranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/videogeneration_replicate_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/videogeneration_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.956800 nostr_dvm-0.5.4/nostr_dvm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/cashu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/dvmconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/external_dvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/mediasource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/nip88_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/nip89_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/nostr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/nwc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/output_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/print.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.956800 nostr_dvm-0.5.4/nostr_dvm/utils/scrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/scrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/scrapper/media_scrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/subscription_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15010 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/zap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.956800 nostr_dvm-0.5.4/nostr_dvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-06-01 17:18:13.000000 nostr_dvm-0.5.4/nostr_dvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-06-01 17:18:13.000000 nostr_dvm-0.5.4/nostr_dvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 17:18:13.000000 nostr_dvm-0.5.4/nostr_dvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-06-01 17:18:13.000000 nostr_dvm-0.5.4/nostr_dvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 17:18:13.000000 nostr_dvm-0.5.4/nostr_dvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 17:18:13.956800 nostr_dvm-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.956800 nostr_dvm-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/tests/test_dvm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.650043 nostr_dvm-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-06-01 17:31:28.650043 nostr_dvm-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.634043 nostr_dvm-0.5.5/nostr_dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.638043 nostr_dvm-0.5.5/nostr_dvm/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.638043 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.638043 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.638043 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.638043 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.638043 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.638043 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_interrogator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.642043 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.642043 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.642043 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/whisperx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/whisperx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41554 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/dvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.642043 nostr_dvm-0.5.5/nostr_dvm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/interfaces/dvmtaskinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.646043 nostr_dvm-0.5.5/nostr_dvm/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/advanced_search_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13986 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14061 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/convert_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_bot_farms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_censor_wot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_inactive_follows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_nonfollowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_openai_dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/imageinterrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/imageupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/search_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/summarization_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/summarization_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/textextraction_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/textextraction_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/textextraction_whisperx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/textgeneration_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/textgeneration_llmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/textgeneration_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/texttospeech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/translation_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/translation_libretranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/videogeneration_replicate_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/tasks/videogeneration_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.650043 nostr_dvm-0.5.5/nostr_dvm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/cashu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/dvmconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/external_dvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/mediasource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/nip88_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/nip89_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/nostr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/nwc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/output_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.650043 nostr_dvm-0.5.5/nostr_dvm/utils/scrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/scrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/scrapper/media_scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/subscription_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15010 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/nostr_dvm/utils/zap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.650043 nostr_dvm-0.5.5/nostr_dvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-06-01 17:31:28.000000 nostr_dvm-0.5.5/nostr_dvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-06-01 17:31:28.000000 nostr_dvm-0.5.5/nostr_dvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 17:31:28.000000 nostr_dvm-0.5.5/nostr_dvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-06-01 17:31:28.000000 nostr_dvm-0.5.5/nostr_dvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 17:31:28.000000 nostr_dvm-0.5.5/nostr_dvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 17:31:28.650043 nostr_dvm-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:31:28.650043 nostr_dvm-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/tests/test_dvm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-01 17:31:24.000000 nostr_dvm-0.5.5/tests/test_events.py
```

### Comparing `nostr_dvm-0.5.4/LICENSE` & `nostr_dvm-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/PKG-INFO` & `nostr_dvm-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.5.4
+Version: 0.5.5
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.5.4/README.md` & `nostr_dvm-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/utils.py` & `nostr_dvm-0.5.5/nostr_dvm/backends/nova_server/utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/bot.py` & `nostr_dvm-0.5.5/nostr_dvm/bot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/dvm.py` & `nostr_dvm-0.5.5/nostr_dvm/dvm.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/interfaces/dvmtaskinterface.py` & `nostr_dvm-0.5.5/nostr_dvm/interfaces/dvmtaskinterface.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/subscription.py` & `nostr_dvm-0.5.5/nostr_dvm/subscription.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/advanced_search.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/advanced_search.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/advanced_search_wine.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/advanced_search_wine.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular_followers.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular_followers.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
             # print(best_entry.as_json())
             followings = []
             for tag in best_entry.tags():
                 if tag.as_vec()[0] == "p":
                     following = PublicKey.parse(tag.as_vec()[1])
                     followings.append(following)
-
+            print("[" + self.dvm_config.NIP89.NAME + "] Considering " + str(len(followings)) + " Followers")
             filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).authors(followings).since(since)
             events = self.client.database().query([filter1])
             print("[" + self.dvm_config.NIP89.NAME + "] Considering " + str(len(events)) + " Events")
 
             ns.finallist = {}
             for event in events:
                 # if event.created_at().as_secs() > timestamp_since:
```

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular_topic.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/content_discovery_currently_popular_topic.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/convert_media.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/convert_media.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_bot_farms.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_bot_farms.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_censor_wot.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_censor_wot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_inactive_follows.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_inactive_follows.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_nonfollowers.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_nonfollowers.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_trending_notes_nostrband.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/discovery_trending_notes_nostrband.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_openai_dalle.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_openai_dalle.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_sd21_mlx.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_sd21_mlx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_sdxl.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/imageinterrogator.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/imageinterrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/imageupscale.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/imageupscale.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/search_users.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/search_users.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/summarization_huggingchat.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/summarization_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/summarization_unleashed_chat.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/summarization_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/textextraction_google.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/textextraction_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/textextraction_pdf.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/textextraction_pdf.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/textextraction_whisperx.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/textextraction_whisperx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/textgeneration_huggingchat.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/textgeneration_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/textgeneration_llmlite.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/textgeneration_llmlite.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/textgeneration_unleashed_chat.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/textgeneration_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/texttospeech.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/texttospeech.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/translation_google.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/translation_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/translation_libretranslate.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/translation_libretranslate.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/videogeneration_replicate_svd.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/videogeneration_replicate_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/tasks/videogeneration_svd.py` & `nostr_dvm-0.5.5/nostr_dvm/tasks/videogeneration_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/admin_utils.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/admin_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/backend_utils.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/cashu_utils.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/cashu_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/database_utils.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/definitions.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/dvmconfig.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/dvmconfig.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/external_dvm_utils.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/external_dvm_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/mediasource_utils.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/mediasource_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/nip88_utils.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/nip88_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/nip89_utils.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/nip89_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/nostr_utils.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/nostr_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/nwc_tools.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/nwc_tools.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/output_utils.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/scrapper/media_scrapper.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/scrapper/media_scrapper.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/subscription_utils.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/subscription_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm/utils/zap_utils.py` & `nostr_dvm-0.5.5/nostr_dvm/utils/zap_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/nostr_dvm.egg-info/PKG-INFO` & `nostr_dvm-0.5.5/nostr_dvm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.5.4
+Version: 0.5.5
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.5.4/nostr_dvm.egg-info/SOURCES.txt` & `nostr_dvm-0.5.5/nostr_dvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/setup.py` & `nostr_dvm-0.5.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.5.4'
+VERSION = '0.5.5'
 DESCRIPTION = 'A framework to build and run Nostr NIP90 Data Vending Machines'
 LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. See the github repository for more information')
 
 # Setting up
 setup(
     name="nostr-dvm",
     version=VERSION,
```

### Comparing `nostr_dvm-0.5.4/tests/test_dvm_client.py` & `nostr_dvm-0.5.5/tests/test_dvm_client.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.4/tests/test_events.py` & `nostr_dvm-0.5.5/tests/test_events.py`

 * *Files identical despite different names*

