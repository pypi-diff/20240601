# Comparing `tmp/nostr_dvm-0.5.3.tar.gz` & `tmp/nostr_dvm-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostr_dvm-0.5.3.tar", last modified: Fri May 31 14:29:10 2024, max compression
+gzip compressed data, was "nostr_dvm-0.5.4.tar", last modified: Sat Jun  1 17:18:13 2024, max compression
```

## Comparing `nostr_dvm-0.5.3.tar` & `nostr_dvm-0.5.4.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.057166 nostr_dvm-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-31 14:29:10.057166 nostr_dvm-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.041166 nostr_dvm-0.5.3/nostr_dvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.041166 nostr_dvm-0.5.3/nostr_dvm/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.041166 nostr_dvm-0.5.3/nostr_dvm/backends/mlx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.041166 nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.045166 nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.045166 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.045166 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.045166 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/image_interrogator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.045166 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/image_upscale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.045166 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.049166 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/whisperx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/whisperx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    40530 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/dvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.049166 nostr_dvm-0.5.3/nostr_dvm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/interfaces/dvmtaskinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.053166 nostr_dvm-0.5.3/nostr_dvm/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/advanced_search_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/content_discovery_currently_popular.py
--rw-r--r--   0 runner    (1001) docker     (127)    14146 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py
--rw-r--r--   0 runner    (1001) docker     (127)    13777 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13735 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/convert_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/discovery_bot_farms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/discovery_censor_wot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/discovery_inactive_follows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/discovery_nonfollowers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/imagegeneration_openai_dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/imagegeneration_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/imageinterrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/imageupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/search_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/summarization_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/summarization_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/textextraction_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/textextraction_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/textextraction_whisperx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/textgeneration_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/textgeneration_llmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/textgeneration_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/texttospeech.py
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/translation_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/translation_libretranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/videogeneration_replicate_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/tasks/videogeneration_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.057166 nostr_dvm-0.5.3/nostr_dvm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/cashu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/dvmconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/external_dvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/mediasource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/nip88_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/nip89_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/nostr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/nwc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/output_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/print.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.057166 nostr_dvm-0.5.3/nostr_dvm/utils/scrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/scrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/scrapper/media_scrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/subscription_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15010 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/nostr_dvm/utils/zap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.057166 nostr_dvm-0.5.3/nostr_dvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-31 14:29:10.000000 nostr_dvm-0.5.3/nostr_dvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-31 14:29:10.000000 nostr_dvm-0.5.3/nostr_dvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:29:10.000000 nostr_dvm-0.5.3/nostr_dvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-31 14:29:10.000000 nostr_dvm-0.5.3/nostr_dvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 14:29:10.000000 nostr_dvm-0.5.3/nostr_dvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:29:10.057166 nostr_dvm-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:29:10.057166 nostr_dvm-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/tests/test_dvm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-31 14:29:06.000000 nostr_dvm-0.5.3/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.956800 nostr_dvm-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-06-01 17:18:13.956800 nostr_dvm-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.940800 nostr_dvm-0.5.4/nostr_dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.940800 nostr_dvm-0.5.4/nostr_dvm/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.940800 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.940800 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_interrogator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/whisperx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/whisperx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41554 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/dvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.944800 nostr_dvm-0.5.4/nostr_dvm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/interfaces/dvmtaskinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.952800 nostr_dvm-0.5.4/nostr_dvm/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/advanced_search_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13878 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14061 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/convert_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_bot_farms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_censor_wot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_inactive_follows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_nonfollowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_openai_dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/imageinterrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/imageupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/search_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/summarization_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/summarization_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/textextraction_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/textextraction_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/textextraction_whisperx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/textgeneration_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/textgeneration_llmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/textgeneration_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/texttospeech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/translation_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/translation_libretranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/videogeneration_replicate_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/tasks/videogeneration_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.956800 nostr_dvm-0.5.4/nostr_dvm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/cashu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/dvmconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/external_dvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13406 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/mediasource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/nip88_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/nip89_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/nostr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/nwc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/output_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.956800 nostr_dvm-0.5.4/nostr_dvm/utils/scrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/scrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/scrapper/media_scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/subscription_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15010 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/nostr_dvm/utils/zap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.956800 nostr_dvm-0.5.4/nostr_dvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-06-01 17:18:13.000000 nostr_dvm-0.5.4/nostr_dvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-06-01 17:18:13.000000 nostr_dvm-0.5.4/nostr_dvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 17:18:13.000000 nostr_dvm-0.5.4/nostr_dvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-06-01 17:18:13.000000 nostr_dvm-0.5.4/nostr_dvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 17:18:13.000000 nostr_dvm-0.5.4/nostr_dvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 17:18:13.956800 nostr_dvm-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:18:13.956800 nostr_dvm-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/tests/test_dvm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-06-01 17:18:10.000000 nostr_dvm-0.5.4/tests/test_events.py
```

### Comparing `nostr_dvm-0.5.3/LICENSE` & `nostr_dvm-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/PKG-INFO` & `nostr_dvm-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.5.3
+Version: 0.5.4
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.5.3/README.md` & `nostr_dvm-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/backends/nova_server/utils.py` & `nostr_dvm-0.5.4/nostr_dvm/backends/nova_server/utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/bot.py` & `nostr_dvm-0.5.4/nostr_dvm/bot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/dvm.py` & `nostr_dvm-0.5.4/nostr_dvm/dvm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 import subprocess
 from datetime import timedelta
 from sys import platform
 
 from nostr_sdk import PublicKey, Keys, Client, Tag, Event, EventBuilder, Filter, HandleNotification, Timestamp, \
-    init_logger, LogLevel, Options, nip04_encrypt, NostrSigner, Kind
+    init_logger, LogLevel, Options, nip04_encrypt, NostrSigner, Kind, RelayLimits
 
 import time
 
 from nostr_dvm.utils.definitions import EventDefinitions, RequiredJobToWatch, JobToWatch
 from nostr_dvm.utils.dvmconfig import DVMConfig
 from nostr_dvm.utils.admin_utils import admin_make_database_updates, AdminConfig
 from nostr_dvm.utils.backend_utils import get_amount_per_task, check_task_is_supported, get_task
@@ -35,16 +35,17 @@
 
     def __init__(self, dvm_config, admin_config=None):
         self.dvm_config = dvm_config
         self.admin_config = admin_config
         self.keys = Keys.parse(dvm_config.PRIVATE_KEY)
         wait_for_send = False
         skip_disconnected_relays = True
-        opts = (Options().wait_for_send(wait_for_send).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
-                .skip_disconnected_relays(skip_disconnected_relays))
+        relaylimits = RelayLimits.disable()
+        opts = (Options().wait_for_send(wait_for_send). send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
+                .skip_disconnected_relays(skip_disconnected_relays).relay_limits(relaylimits))
 
         signer = NostrSigner.keys(self.keys)
         self.client = Client.with_opts(signer, opts)
 
         self.job_list = []
         self.jobs_on_hold_list = []
         pk = self.keys.public_key()
@@ -686,9 +687,26 @@
                     try:
                         self.jobs_on_hold_list.remove(job)
                     except:
                         print("[" + self.dvm_config.NIP89.NAME + "] Error removing Job on Hold from List after expiry")
 
                 if Timestamp.now().as_secs() > job.timestamp + 60 * 20:  # remove jobs to look for after 20 minutes..
                     self.jobs_on_hold_list.remove(job)
+            advanced_log = False
+            if advanced_log:
+                for url, relay in self.client.relays().items():
+                    stats = relay.stats()
+                    print(f"Relay: {url}")
+                    print(f"Connected: {relay.is_connected()}")
+                    print(f"Status: {relay.status()}")
+                    print("Stats:")
+                    print(f"    Attempts: {stats.attempts()}")
+                    print(f"    Success: {stats.success()}")
+                    print(f"    Bytes sent: {stats.bytes_sent()}")
+                    print(f"    Bytes received: {stats.bytes_received()}")
+                    print(f"    Connected at: {stats.connected_at().to_human_datetime()}")
+                    if stats.latency() is not None:
+                        print(f"    Latency: {stats.latency().total_seconds() * 1000} ms")
+
+                    print("###########################################")
 
             time.sleep(1.0)
```

### Comparing `nostr_dvm-0.5.3/nostr_dvm/interfaces/dvmtaskinterface.py` & `nostr_dvm-0.5.4/nostr_dvm/interfaces/dvmtaskinterface.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/subscription.py` & `nostr_dvm-0.5.4/nostr_dvm/subscription.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/advanced_search.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/advanced_search.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/advanced_search_wine.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/advanced_search_wine.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/content_discovery_currently_popular.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 from datetime import timedelta
 from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, NostrDatabase, \
-    ClientBuilder, Filter, NegentropyOptions, NegentropyDirection, init_logger, LogLevel, Event, EventId, Kind
+    ClientBuilder, Filter, NegentropyOptions, NegentropyDirection, init_logger, LogLevel, Event, EventId, Kind, \
+    RelayOptions
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils import definitions
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.nip88_utils import NIP88Config, check_and_set_d_tag_nip88, check_and_set_tiereventid_nip88
@@ -54,28 +55,30 @@
                 self.db_since = int(self.options.get("db_since"))
             if self.options.get("logger"):
                 self.logger = bool(self.options.get("logger"))
 
             if self.logger:
                 init_logger(LogLevel.DEBUG)
 
-        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
+        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_LONG_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
         database = NostrDatabase.sqlite(self.db_name)
         self.client = ClientBuilder().signer(signer).database(database).opts(opts).build()
 
-        self.client.add_relay("wss://relay.damus.io")
-        self.client.add_relay("wss://nostr.oxtr.dev")
-        self.client.add_relay("wss://nostr21.com")
+        ropts = RelayOptions().ping(False)
+        self.client.add_relay_with_opts("wss://relay.damus.io", ropts)
+        self.client.add_relay_with_opts("wss://nostr.oxtr.dev", ropts)
+        self.client.add_relay_with_opts("wss://nostr21.com", ropts)
 
         self.client.connect()
 
 
+
         if self.dvm_config.UPDATE_DATABASE:
             self.sync_db()
 
         if not self.personalized:
             self.result = self.calculate_result(self.request_form)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
@@ -138,14 +141,17 @@
                 filt = Filter().kinds([definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REPOST,
                                        definitions.EventDefinitions.KIND_REACTION,
                                        definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(since)
                 reactions = self.client.database().query([filt])
                 if len(reactions) >= self.min_reactions:
                     ns.finallist[event.id().to_hex()] = len(reactions)
 
+        if len(ns.finallist) == 0:
+            return self.result
+
         result_list = []
         finallist_sorted = sorted(ns.finallist.items(), key=lambda x: x[1], reverse=True)[:int(options["max_results"])]
         for entry in finallist_sorted:
             e_tag = Tag.parse(["e", entry[0]])
             result_list.append(e_tag.as_vec())
 
         return json.dumps(result_list)
```

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular_by_top_zaps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 from datetime import timedelta
 from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, NostrDatabase, \
-    ClientBuilder, Filter, NegentropyOptions, NegentropyDirection, init_logger, LogLevel, Event, EventId, Kind
+    ClientBuilder, Filter, NegentropyOptions, NegentropyDirection, init_logger, LogLevel, Event, EventId, Kind, \
+    RelayOptions
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils import definitions
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.nip88_utils import NIP88Config, check_and_set_d_tag_nip88, check_and_set_tiereventid_nip88
@@ -55,24 +56,25 @@
                 self.db_since = int(self.options.get("db_since"))
             if self.options.get("logger"):
                 self.logger = bool(self.options.get("logger"))
 
             if self.logger:
                 init_logger(LogLevel.DEBUG)
 
-        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
+        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_LONG_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
         database = NostrDatabase.sqlite(self.db_name)
         self.client = ClientBuilder().signer(signer).database(database).opts(opts).build()
 
-        self.client.add_relay("wss://relay.damus.io")
-        self.client.add_relay("wss://nostr.oxtr.dev")
-        self.client.add_relay("wss://nostr21.com")
+        ropts = RelayOptions().ping(False)
+        self.client.add_relay_with_opts("wss://relay.damus.io", ropts)
+        self.client.add_relay_with_opts("wss://nostr.oxtr.dev", ropts)
+        self.client.add_relay_with_opts("wss://nostr21.com", ropts)
 
         self.client.connect()
 
         if self.dvm_config.UPDATE_DATABASE:
             self.sync_db()
 
         if not self.personalized:
```

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/content_discovery_currently_popular_followers.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular_followers.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,20 +54,21 @@
         opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
         database = NostrDatabase.sqlite(self.db_name)
         self.client = ClientBuilder().signer(signer).database(database).opts(opts).build()
 
-        self.client.add_relay("wss://relay.damus.io")
-        self.client.add_relay("wss://nostr.oxtr.dev")
-        self.client.add_relay("wss://nostr21.com")
-
         ropts = RelayOptions().ping(False)
-        self.client.add_relay_with_opts("wss://nostr.band", ropts)
+        self.client.add_relay_with_opts("wss://relay.damus.io", ropts)
+        self.client.add_relay_with_opts("wss://nostr.oxtr.dev", ropts)
+        self.client.add_relay_with_opts("wss://nostr21.com", ropts)
+
+        #ropts = RelayOptions().ping(False)
+        #self.client.add_relay_with_opts("wss://nostr.band", ropts)
 
         self.client.connect()
 
         if self.dvm_config.UPDATE_DATABASE:
             self.sync_db()
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
@@ -110,15 +111,15 @@
         from types import SimpleNamespace
         ns = SimpleNamespace()
 
         options = self.set_options(request_form)
 
         relaylimits = RelayLimits.disable()
         opts = (
-            Options().wait_for_send(True).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)).relay_limits(
+            Options().wait_for_send(True).send_timeout(timedelta(seconds=self.dvm_config.RELAY_LONG_TIMEOUT)).relay_limits(
                 relaylimits))
 
         user = PublicKey.parse(options["user"])
         followers_filter = Filter().author(user).kinds([Kind(3)])
         followers = self.client.get_events_of([followers_filter], timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
 
         # Negentropy reconciliation
```

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/content_discovery_currently_popular_topic.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/content_discovery_currently_popular_topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 from datetime import timedelta
 from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, NostrDatabase, \
-    ClientBuilder, Filter, NegentropyOptions, NegentropyDirection, init_logger, LogLevel, Event, EventId, Kind
+    ClientBuilder, Filter, NegentropyOptions, NegentropyDirection, init_logger, LogLevel, Event, EventId, Kind, \
+    RelayLimits, RelayOptions
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils import definitions
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.nip88_utils import NIP88Config, check_and_set_d_tag_nip88, check_and_set_tiereventid_nip88
@@ -69,24 +70,31 @@
                 self.db_since = int(self.options.get("db_since"))
             if self.options.get("logger"):
                 self.logger = bool(self.options.get("logger"))
 
             if self.logger:
                 init_logger(LogLevel.DEBUG)
 
-        opts = (Options().wait_for_send(True).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
+        relaylimits = RelayLimits.disable()
+        opts = (Options().wait_for_send(True).send_timeout(timedelta(seconds=dvm_config.RELAY_LONG_TIMEOUT))
+                .relay_limits(relaylimits))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
         database = NostrDatabase.sqlite(self.db_name)
         self.client = ClientBuilder().signer(signer).database(database).opts(opts).build()
 
-        self.client.add_relay("wss://relay.damus.io")
-        self.client.add_relay("wss://nostr.oxtr.dev")
-        self.client.add_relay("wss://nostr21.com")
+        #self.client.add_relay("wss://relay.damus.io")
+        #self.client.add_relay("wss://nostr.oxtr.dev")
+
+        ropts = RelayOptions().ping(False)
+        self.client.add_relay_with_opts("wss://relay.damus.io", ropts)
+        self.client.add_relay_with_opts("wss://nostr.oxtr.dev", ropts)
+        self.client.add_relay_with_opts("wss://nostr21.com", ropts)
+
         self.client.connect()
 
         if self.dvm_config.UPDATE_DATABASE:
             self.sync_db()
         if not self.personalized:
             self.result = self.calculate_result(self.request_form)
```

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/convert_media.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/convert_media.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/discovery_bot_farms.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_bot_farms.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/discovery_censor_wot.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_censor_wot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/discovery_inactive_follows.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_inactive_follows.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/discovery_nonfollowers.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_nonfollowers.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/discovery_trending_notes_nostrband.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/discovery_trending_notes_nostrband.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/imagegeneration_openai_dalle.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_openai_dalle.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/imagegeneration_sd21_mlx.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_sd21_mlx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/imagegeneration_sdxl.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/imageinterrogator.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/imageinterrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/imageupscale.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/imageupscale.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/search_users.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/search_users.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/summarization_huggingchat.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/summarization_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/summarization_unleashed_chat.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/summarization_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/textextraction_google.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/textextraction_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/textextraction_pdf.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/textextraction_pdf.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/textextraction_whisperx.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/textextraction_whisperx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/textgeneration_huggingchat.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/textgeneration_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/textgeneration_llmlite.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/textgeneration_llmlite.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/textgeneration_unleashed_chat.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/textgeneration_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/texttospeech.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/texttospeech.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/translation_google.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/translation_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/translation_libretranslate.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/translation_libretranslate.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/videogeneration_replicate_svd.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/videogeneration_replicate_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/tasks/videogeneration_svd.py` & `nostr_dvm-0.5.4/nostr_dvm/tasks/videogeneration_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/admin_utils.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/admin_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/backend_utils.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/cashu_utils.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/cashu_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/database_utils.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/definitions.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/dvmconfig.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/dvmconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,23 @@
 class DVMConfig:
     SUPPORTED_DVMS = []
     PRIVATE_KEY: str = ""
     PUBLIC_KEY: str = ""
     FIX_COST: float = None
     PER_UNIT_COST: float = None
 
-    RELAY_LIST = ["wss://dvms.f7z.io", "wss://relay.damus.io", "wss://nostr.wine",
+    RELAY_LIST = ["wss://dvms.f7z.io",
                   "wss://nostr.mom", "wss://nostr.oxtr.dev", "wss://relay.nostr.bg",
                   "wss://relay.nostr.net"
                   ]
 
+    #"wss://relay.damus.io"
+
     RELAY_TIMEOUT = 5
+    RELAY_LONG_TIMEOUT = 30
     EXTERNAL_POST_PROCESS_TYPE = PostProcessFunctionType.NONE  # Leave this on None, except the DVM is external
     LNBITS_INVOICE_KEY = ''  # Will all automatically generated by default, or read from .env
     LNBITS_ADMIN_KEY = ''  # In order to pay invoices, e.g. from the bot to DVMs, or reimburse users.
     LNBITS_URL = 'https://lnbits.com'
     LN_ADDRESS = ''
     SCRIPT = ''
     IDENTIFIER = ''
```

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/external_dvm_utils.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/external_dvm_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/mediasource_utils.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/mediasource_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/nip88_utils.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/nip88_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/nip89_utils.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/nip89_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/nostr_utils.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/nostr_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/nwc_tools.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/nwc_tools.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/output_utils.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/scrapper/media_scrapper.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/scrapper/media_scrapper.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/subscription_utils.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/subscription_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm/utils/zap_utils.py` & `nostr_dvm-0.5.4/nostr_dvm/utils/zap_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/nostr_dvm.egg-info/PKG-INFO` & `nostr_dvm-0.5.4/nostr_dvm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.5.3
+Version: 0.5.4
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.5.3/nostr_dvm.egg-info/SOURCES.txt` & `nostr_dvm-0.5.4/nostr_dvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/setup.py` & `nostr_dvm-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.5.3'
+VERSION = '0.5.4'
 DESCRIPTION = 'A framework to build and run Nostr NIP90 Data Vending Machines'
 LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. See the github repository for more information')
 
 # Setting up
 setup(
     name="nostr-dvm",
     version=VERSION,
```

### Comparing `nostr_dvm-0.5.3/tests/test_dvm_client.py` & `nostr_dvm-0.5.4/tests/test_dvm_client.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.5.3/tests/test_events.py` & `nostr_dvm-0.5.4/tests/test_events.py`

 * *Files identical despite different names*

