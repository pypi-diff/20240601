# Comparing `tmp/aiogram_broadcaster-0.4.7.tar.gz` & `tmp/aiogram_broadcaster-0.5.0.tar.gz`

## Comparing `aiogram_broadcaster-0.4.7.tar` & `aiogram_broadcaster-0.5.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/.editorconfig
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/Makefile
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/.github/workflows/tests.yml
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/__meta__.py
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/broadcaster.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/py.typed
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/__init__.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/animation.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/audio.py
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/base.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/chat_action.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/contact.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/dice.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/document.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/from_chat.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/game.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/invoice.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/key_based.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/lazy.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/location.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/media_group.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/message.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/photo.py
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/poll.py
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/sticker.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/text.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/venue.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/video.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/video_note.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/voice.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/event/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/event/manager.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/event/observer.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/event/registry.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/__init__.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/chat_engine.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/container.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/group.py
--rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/mailer.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/settings.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/statistic.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/status.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/task_manager.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/placeholder/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/placeholder/item.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/placeholder/manager.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/placeholder/placeholder.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/placeholder/registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/__init__.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/base.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/file.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/mongodb.py
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/redis.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/utils/__init__.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/utils/chain.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/utils/interrupt.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/utils/loggers.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/examples/events.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/examples/key_based_content.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/examples/lazy_content.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/examples/mre.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/examples/multibot.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/examples/placeholders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_contents/__init__.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_contents/test_base.py
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_contents/test_contents.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_contents/test_key_based.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_contents/test_lazy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_event/__init__.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_event/test_manager.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_event/test_observer.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_event/test_registry.py
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_mailer/test_settings.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_mailer/test_task_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_placeholder/__init__.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_placeholder/test_item.py
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_placeholder/test_manager.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_placeholder/test_placeholder.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_placeholder/test_registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_utils/test_chain.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_utils/test_interrupt.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/LICENSE
--rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/README.md
--rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/pyproject.toml
--rw-r--r--   0        0        0    18852 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/.editorconfig
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/Makefile
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/__meta__.py
+-rw-r--r--   0        0        0     9132 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/broadcaster.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/py.typed
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/__init__.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/animation.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/audio.py
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/base.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/chat_action.py
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/contact.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/dice.py
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/document.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/from_chat.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/game.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/invoice.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/key_based.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/lazy.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/location.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/media_group.py
+-rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/message.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/photo.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/poll.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/sticker.py
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/text.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/venue.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/video.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/video_note.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/voice.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/event/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/event/manager.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/event/observer.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/event/registry.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/mailer/__init__.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/mailer/chat_engine.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/mailer/container.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/mailer/group.py
+-rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/mailer/mailer.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/mailer/settings.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/mailer/statistic.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/mailer/status.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/mailer/task_manager.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/placeholder/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/placeholder/item.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/placeholder/manager.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/placeholder/placeholder.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/placeholder/registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/storages/__init__.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/storages/base.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/storages/file.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/storages/mongodb.py
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/storages/redis.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/storages/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/utils/__init__.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/utils/chain.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/utils/interrupt.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/aiogram_broadcaster/utils/loggers.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/examples/events.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/examples/key_based_content.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/examples/lazy_content.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/examples/mre.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/examples/multibot.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/examples/placeholders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_contents/__init__.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_contents/test_base.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_contents/test_contents.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_contents/test_key_based.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_contents/test_lazy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_event/__init__.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_event/test_manager.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_event/test_observer.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_event/test_registry.py
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_mailer/test_settings.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_mailer/test_task_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_placeholder/__init__.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_placeholder/test_item.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_placeholder/test_manager.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_placeholder/test_placeholder.py
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_placeholder/test_registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_utils/test_chain.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/tests/test_utils/test_interrupt.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/LICENSE
+-rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/README.md
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    19092 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.5.0/PKG-INFO
```

### Comparing `aiogram_broadcaster-0.4.7/Makefile` & `aiogram_broadcaster-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/.github/workflows/pypi-publish.yml` & `aiogram_broadcaster-0.5.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/.github/workflows/tests.yml` & `aiogram_broadcaster-0.5.0/.github/workflows/tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "${{ matrix.python-version }}"
           cache: pip
           cache-dependency-path: pyproject.toml
 
       - name: Install dependencies
-        run: python -m pip install --upgrade .[dev,test,redis,mongo,sqlalchemy] build pip
+        run: python -m pip install --upgrade .[dev,test,redis,mongo,sqlalchemy] build pip aiogram
 
       - name: Lint code
         run: make lint
 
       - name: Run tests
         run: make test
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/broadcaster.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/broadcaster.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
         self.event = EventManager(name="root")
         self.placeholder = PlaceholderManager(name="root")
 
     def as_group(self) -> MailerGroup:
         if not self._mailers:
             raise RuntimeError("No mailers for grouping.")
-        return MailerGroup(*self._mailers.values())
+        return MailerGroup(*self)
 
     async def create_mailers(
         self,
         *bots: Bot,
         content: BaseContent,
         chats: Iterable[int],
         interval: Optional[float] = None,
@@ -185,15 +185,15 @@
         if not self.storage:
             raise RuntimeError("Storage not found.")
         mailer_ids = await self.storage.get_mailer_ids()
         if not mailer_ids:
             return
         bots = {bot.id: bot for bot in self.bots}
         for mailer_id in mailer_ids:
-            if mailer_id in self._mailers:
+            if mailer_id in self:
                 continue
             try:
                 record = await self.storage.get(mailer_id=mailer_id)
             except ValidationError:
                 loggers.pool.exception("Failed to restore mailer id=%d.", mailer_id)
                 continue
             if record.bot_id not in bots:
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/__init__.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/animation.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/photo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,75 @@
 from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
-from aiogram.methods import SendAnimation
+from aiogram.methods import SendPhoto
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
     InputFile,
     MessageEntity,
     ReplyKeyboardMarkup,
     ReplyKeyboardRemove,
 )
 
 from .base import BaseContent
 
 
-class AnimationContent(BaseContent):
-    animation: Union[InputFile, str]
+class PhotoContent(BaseContent):
+    photo: Union[InputFile, str]
     business_connection_id: Optional[str] = None
-    duration: Optional[int] = None
-    width: Optional[int] = None
-    height: Optional[int] = None
-    thumbnail: Optional[InputFile] = None
     caption: Optional[str] = None
     parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
     caption_entities: Optional[List[MessageEntity]] = None
+    show_caption_above_media: Optional[Union[bool, Default]] = Default("show_caption_above_media")
     has_spoiler: Optional[bool] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
+    message_effect_id: Optional[str] = None
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
     ] = None
 
-    async def __call__(self, chat_id: int) -> SendAnimation:
-        return SendAnimation(
+    async def __call__(self, chat_id: int) -> SendPhoto:
+        return SendPhoto(
             chat_id=chat_id,
-            animation=self.animation,
+            photo=self.photo,
             business_connection_id=self.business_connection_id,
-            duration=self.duration,
-            width=self.width,
-            height=self.height,
-            thumbnail=self.thumbnail,
             caption=self.caption,
             parse_mode=self.parse_mode,
             caption_entities=self.caption_entities,
+            show_caption_above_media=self.show_caption_above_media,
             has_spoiler=self.has_spoiler,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
-            animation: Union[InputFile, str],
+            photo: Union[InputFile, str],
             business_connection_id: Optional[str] = ...,
-            duration: Optional[int] = ...,
-            width: Optional[int] = ...,
-            height: Optional[int] = ...,
-            thumbnail: Optional[InputFile] = ...,
             caption: Optional[str] = ...,
             parse_mode: Optional[Union[str, Default]] = ...,
             caption_entities: Optional[List[MessageEntity]] = ...,
+            show_caption_above_media: Optional[Union[bool, Default]] = ...,
             has_spoiler: Optional[bool] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            message_effect_id: Optional[str] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/audio.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     caption_entities: Optional[List[MessageEntity]] = None
     duration: Optional[int] = None
     performer: Optional[str] = None
     title: Optional[str] = None
     thumbnail: Optional[InputFile] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
+    message_effect_id: Optional[str] = None
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
@@ -45,14 +46,15 @@
             caption_entities=self.caption_entities,
             duration=self.duration,
             performer=self.performer,
             title=self.title,
             thumbnail=self.thumbnail,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
@@ -65,14 +67,15 @@
             caption_entities: Optional[List[MessageEntity]] = ...,
             duration: Optional[int] = ...,
             performer: Optional[str] = ...,
             title: Optional[str] = ...,
             thumbnail: Optional[InputFile] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            message_effect_id: Optional[str] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/base.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/base.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/chat_action.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/chat_action.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/contact.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/contact.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     phone_number: str
     first_name: str
     business_connection_id: Optional[str] = None
     last_name: Optional[str] = None
     vcard: Optional[str] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
+    message_effect_id: Optional[str] = None
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
@@ -35,14 +36,15 @@
             phone_number=self.phone_number,
             first_name=self.first_name,
             business_connection_id=self.business_connection_id,
             last_name=self.last_name,
             vcard=self.vcard,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
@@ -51,14 +53,15 @@
             phone_number: str,
             first_name: str,
             business_connection_id: Optional[str] = ...,
             last_name: Optional[str] = ...,
             vcard: Optional[str] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            message_effect_id: Optional[str] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/dice.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/dice.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 class DiceContent(BaseContent):
     business_connection_id: Optional[str] = None
     emoji: Optional[str] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
+    message_effect_id: Optional[str] = None
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
@@ -29,27 +30,29 @@
     async def __call__(self, chat_id: int) -> SendDice:
         return SendDice(
             chat_id=chat_id,
             business_connection_id=self.business_connection_id,
             emoji=self.emoji,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
             business_connection_id: Optional[str] = ...,
             emoji: Optional[str] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            message_effect_id: Optional[str] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/document.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/document.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     thumbnail: Optional[InputFile] = None
     caption: Optional[str] = None
     parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
     caption_entities: Optional[List[MessageEntity]] = None
     disable_content_type_detection: Optional[bool] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
+    message_effect_id: Optional[str] = None
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
@@ -41,14 +42,15 @@
             thumbnail=self.thumbnail,
             caption=self.caption,
             parse_mode=self.parse_mode,
             caption_entities=self.caption_entities,
             disable_content_type_detection=self.disable_content_type_detection,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
@@ -59,14 +61,15 @@
             thumbnail: Optional[InputFile] = ...,
             caption: Optional[str] = ...,
             parse_mode: Optional[Union[str, Default]] = ...,
             caption_entities: Optional[List[MessageEntity]] = ...,
             disable_content_type_detection: Optional[bool] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            message_effect_id: Optional[str] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/from_chat.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/from_chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 class FromChatCopyContent(BaseContent):
     from_chat_id: Union[int, str]
     message_id: int
     caption: Optional[str] = None
     parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
     caption_entities: Optional[List[MessageEntity]] = None
+    show_caption_above_media: Optional[Union[bool, Default]] = Default("show_caption_above_media")
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
@@ -34,14 +35,15 @@
         return CopyMessage(
             chat_id=chat_id,
             from_chat_id=self.from_chat_id,
             message_id=self.message_id,
             caption=self.caption,
             parse_mode=self.parse_mode,
             caption_entities=self.caption_entities,
+            show_caption_above_media=self.show_caption_above_media,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
@@ -50,14 +52,15 @@
             self,
             *,
             from_chat_id: Union[int, str],
             message_id: int,
             caption: Optional[str] = ...,
             parse_mode: Optional[Union[str, Default]] = ...,
             caption_entities: Optional[List[MessageEntity]] = ...,
+            show_caption_above_media: Optional[Union[bool, Default]] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/game.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/game.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,32 +8,35 @@
 
 
 class GameContent(BaseContent):
     game_short_name: str
     business_connection_id: Optional[str] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
+    message_effect_id: Optional[str] = None
     reply_markup: Optional[InlineKeyboardMarkup] = None
 
     async def __call__(self, chat_id: int) -> SendGame:
         return SendGame(
             chat_id=chat_id,
             game_short_name=self.game_short_name,
             business_connection_id=self.business_connection_id,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
             game_short_name: str,
             business_connection_id: Optional[str] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            message_effect_id: Optional[str] = ...,
             reply_markup: Optional[InlineKeyboardMarkup] = ...,
             **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/invoice.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/poll.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,96 +1,103 @@
+from datetime import datetime, timedelta
 from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
-from aiogram.methods import SendInvoice
-from aiogram.types import InlineKeyboardMarkup, LabeledPrice
+from aiogram.methods import SendPoll
+from aiogram.types import (
+    ForceReply,
+    InlineKeyboardMarkup,
+    InputPollOption,
+    MessageEntity,
+    ReplyKeyboardMarkup,
+    ReplyKeyboardRemove,
+)
 
 from .base import BaseContent
 
 
-class InvoiceContent(BaseContent):
-    title: str
-    description: str
-    payload: str
-    provider_token: str
-    currency: str
-    prices: List[LabeledPrice]
-    max_tip_amount: Optional[int] = None
-    suggested_tip_amounts: Optional[List[int]] = None
-    start_parameter: Optional[str] = None
-    provider_data: Optional[str] = None
-    photo_url: Optional[str] = None
-    photo_size: Optional[int] = None
-    photo_width: Optional[int] = None
-    photo_height: Optional[int] = None
-    need_name: Optional[bool] = None
-    need_phone_number: Optional[bool] = None
-    need_email: Optional[bool] = None
-    need_shipping_address: Optional[bool] = None
-    send_phone_number_to_provider: Optional[bool] = None
-    send_email_to_provider: Optional[bool] = None
-    is_flexible: Optional[bool] = None
+class PollContent(BaseContent):
+    question: str
+    options: List[Union[InputPollOption, str]]
+    business_connection_id: Optional[str] = None
+    question_parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
+    question_entities: Optional[List[MessageEntity]] = None
+    is_anonymous: Optional[bool] = None
+    type: Optional[str] = None
+    allows_multiple_answers: Optional[bool] = None
+    correct_option_id: Optional[int] = None
+    explanation: Optional[str] = None
+    explanation_parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
+    explanation_entities: Optional[List[MessageEntity]] = None
+    open_period: Optional[int] = None
+    close_date: Optional[Union[datetime, timedelta, int]] = None
+    is_closed: Optional[bool] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
-    reply_markup: Optional[InlineKeyboardMarkup] = None
+    message_effect_id: Optional[str] = None
+    reply_markup: Optional[
+        Union[
+            InlineKeyboardMarkup,
+            ReplyKeyboardMarkup,
+            ReplyKeyboardRemove,
+            ForceReply,
+        ]
+    ] = None
 
-    async def __call__(self, chat_id: int) -> SendInvoice:
-        return SendInvoice(
+    async def __call__(self, chat_id: int) -> SendPoll:
+        return SendPoll(
             chat_id=chat_id,
-            title=self.title,
-            description=self.description,
-            payload=self.payload,
-            provider_token=self.provider_token,
-            currency=self.currency,
-            prices=self.prices,
-            max_tip_amount=self.max_tip_amount,
-            suggested_tip_amounts=self.suggested_tip_amounts,
-            start_parameter=self.start_parameter,
-            provider_data=self.provider_data,
-            photo_url=self.photo_url,
-            photo_size=self.photo_size,
-            photo_width=self.photo_width,
-            photo_height=self.photo_height,
-            need_name=self.need_name,
-            need_phone_number=self.need_phone_number,
-            need_email=self.need_email,
-            need_shipping_address=self.need_shipping_address,
-            send_phone_number_to_provider=self.send_phone_number_to_provider,
-            send_email_to_provider=self.send_email_to_provider,
-            is_flexible=self.is_flexible,
+            question=self.question,
+            options=self.options,
+            business_connection_id=self.business_connection_id,
+            question_parse_mode=self.question_parse_mode,
+            question_entities=self.question_entities,
+            is_anonymous=self.is_anonymous,
+            type=self.type,
+            allows_multiple_answers=self.allows_multiple_answers,
+            correct_option_id=self.correct_option_id,
+            explanation=self.explanation,
+            explanation_parse_mode=self.explanation_parse_mode,
+            explanation_entities=self.explanation_entities,
+            open_period=self.open_period,
+            close_date=self.close_date,
+            is_closed=self.is_closed,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
-            title: str,
-            description: str,
-            payload: str,
-            provider_token: str,
-            currency: str,
-            prices: List[LabeledPrice],
-            max_tip_amount: Optional[int] = ...,
-            suggested_tip_amounts: Optional[List[int]] = ...,
-            start_parameter: Optional[str] = ...,
-            provider_data: Optional[str] = ...,
-            photo_url: Optional[str] = ...,
-            photo_size: Optional[int] = ...,
-            photo_width: Optional[int] = ...,
-            photo_height: Optional[int] = ...,
-            need_name: Optional[bool] = ...,
-            need_phone_number: Optional[bool] = ...,
-            need_email: Optional[bool] = ...,
-            need_shipping_address: Optional[bool] = ...,
-            send_phone_number_to_provider: Optional[bool] = ...,
-            send_email_to_provider: Optional[bool] = ...,
-            is_flexible: Optional[bool] = ...,
+            question: str,
+            options: List[Union[InputPollOption, str]],
+            business_connection_id: Optional[str] = ...,
+            question_parse_mode: Optional[Union[str, Default]] = ...,
+            question_entities: Optional[List[MessageEntity]] = ...,
+            is_anonymous: Optional[bool] = ...,
+            type: Optional[str] = ...,  # noqa: A002
+            allows_multiple_answers: Optional[bool] = ...,
+            correct_option_id: Optional[int] = ...,
+            explanation: Optional[str] = ...,
+            explanation_parse_mode: Optional[Union[str, Default]] = ...,
+            explanation_entities: Optional[List[MessageEntity]] = ...,
+            open_period: Optional[int] = ...,
+            close_date: Optional[Union[datetime, timedelta, int]] = ...,
+            is_closed: Optional[bool] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
-            reply_markup: Optional[InlineKeyboardMarkup] = ...,
+            message_effect_id: Optional[str] = ...,
+            reply_markup: Optional[
+                Union[
+                    InlineKeyboardMarkup,
+                    ReplyKeyboardMarkup,
+                    ReplyKeyboardRemove,
+                    ForceReply,
+                ]
+            ] = ...,
             **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/key_based.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/key_based.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from typing import TYPE_CHECKING, Any, Dict, Optional
 
 from aiogram.methods import TelegramMethod
-from pydantic import ConfigDict, SerializeAsAny
+from pydantic import SerializeAsAny
 
 from .base import BaseContent
 
 
 class KeyBasedContent(BaseContent, register=False):
-    model_config = ConfigDict(extra="allow")
-
     default: Optional[SerializeAsAny[BaseContent]] = None
     __pydantic_extra__: Dict[str, SerializeAsAny[BaseContent]]
 
     def __getitem__(self, item: str) -> BaseContent:
         if self.default:
             return self.__pydantic_extra__.get(item, self.default)
         return self.__pydantic_extra__[item]
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/lazy.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/lazy.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/location.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/location.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     business_connection_id: Optional[str] = None
     horizontal_accuracy: Optional[float] = None
     live_period: Optional[int] = None
     heading: Optional[int] = None
     proximity_alert_radius: Optional[int] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
+    message_effect_id: Optional[str] = None
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
@@ -39,14 +40,15 @@
             business_connection_id=self.business_connection_id,
             horizontal_accuracy=self.horizontal_accuracy,
             live_period=self.live_period,
             heading=self.heading,
             proximity_alert_radius=self.proximity_alert_radius,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
@@ -57,14 +59,15 @@
             business_connection_id: Optional[str] = ...,
             horizontal_accuracy: Optional[float] = ...,
             live_period: Optional[int] = ...,
             heading: Optional[int] = ...,
             proximity_alert_radius: Optional[int] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            message_effect_id: Optional[str] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/media_group.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/media_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,22 +15,24 @@
             InputMediaPhoto,
             InputMediaVideo,
         ]
     ]
     business_connection_id: Optional[str] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
+    message_effect_id: Optional[str] = None
 
     async def __call__(self, chat_id: int) -> SendMediaGroup:
         return SendMediaGroup(
             chat_id=chat_id,
             media=self.media,
             business_connection_id=self.business_connection_id,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
@@ -42,9 +44,10 @@
                     InputMediaPhoto,
                     InputMediaVideo,
                 ]
             ],
             business_connection_id: Optional[str] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            message_effect_id: Optional[str] = ...,
             **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/message.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 
 class MessageCopyContent(BaseContent):
     message: Message
     caption: Optional[str] = None
     parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
     caption_entities: Optional[List[MessageEntity]] = None
+    show_caption_above_media: Optional[Union[bool, Default]] = Default("show_caption_above_media")
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
@@ -49,14 +50,15 @@
 
     async def __call__(self, chat_id: int) -> CopyMessage:
         return self.message.copy_to(
             chat_id=chat_id,
             caption=self.caption,
             parse_mode=self.parse_mode,
             caption_entities=self.caption_entities,
+            show_caption_above_media=self.show_caption_above_media,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
@@ -64,14 +66,15 @@
         def __init__(
             self,
             *,
             message: Message,
             caption: Optional[str] = ...,
             parse_mode: Optional[Union[str, Default]] = ...,
             caption_entities: Optional[List[MessageEntity]] = ...,
+            show_caption_above_media: Optional[Union[bool, Default]] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
@@ -109,14 +112,15 @@
 
 class MessageSendContent(BaseContent):
     message: Message
     disable_notification: Optional[bool] = None
     reply_markup: Optional[Union[InlineKeyboardMarkup, ReplyKeyboardMarkup]] = None
     business_connection_id: Optional[str] = None
     parse_mode: Optional[str] = None
+    message_effect_id: Optional[str] = None
 
     async def __call__(
         self,
         chat_id: int,
     ) -> Union[
         ForwardMessage,
         SendAnimation,
@@ -136,21 +140,23 @@
     ]:
         return self.message.send_copy(
             chat_id=chat_id,
             disable_notification=self.disable_notification,
             reply_markup=self.reply_markup,
             business_connection_id=self.business_connection_id,
             parse_mode=self.parse_mode,
+            message_effect_id=self.message_effect_id,
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
             message: Message,
             disable_notification: Optional[bool] = ...,
             reply_markup: Optional[Union[InlineKeyboardMarkup, ReplyKeyboardMarkup]] = ...,
             business_connection_id: Optional[str] = ...,
             parse_mode: Optional[str] = ...,
+            message_effect_id: Optional[str] = ...,
             **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/photo.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/voice.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,69 +1,72 @@
 from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
-from aiogram.methods import SendPhoto
+from aiogram.methods import SendVoice
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
     InputFile,
     MessageEntity,
     ReplyKeyboardMarkup,
     ReplyKeyboardRemove,
 )
 
 from .base import BaseContent
 
 
-class PhotoContent(BaseContent):
-    photo: Union[InputFile, str]
+class VoiceContent(BaseContent):
+    voice: Union[InputFile, str]
     business_connection_id: Optional[str] = None
     caption: Optional[str] = None
     parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
     caption_entities: Optional[List[MessageEntity]] = None
-    has_spoiler: Optional[bool] = None
+    duration: Optional[int] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
+    message_effect_id: Optional[str] = None
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
     ] = None
 
-    async def __call__(self, chat_id: int) -> SendPhoto:
-        return SendPhoto(
+    async def __call__(self, chat_id: int) -> SendVoice:
+        return SendVoice(
             chat_id=chat_id,
-            photo=self.photo,
+            voice=self.voice,
             business_connection_id=self.business_connection_id,
             caption=self.caption,
             parse_mode=self.parse_mode,
             caption_entities=self.caption_entities,
-            has_spoiler=self.has_spoiler,
+            duration=self.duration,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
-            photo: Union[InputFile, str],
+            voice: Union[InputFile, str],
             business_connection_id: Optional[str] = ...,
             caption: Optional[str] = ...,
             parse_mode: Optional[Union[str, Default]] = ...,
             caption_entities: Optional[List[MessageEntity]] = ...,
-            has_spoiler: Optional[bool] = ...,
+            duration: Optional[int] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            message_effect_id: Optional[str] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/poll.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/invoice.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,100 +1,99 @@
-from datetime import datetime, timedelta
 from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
-from aiogram.methods import SendPoll
-from aiogram.types import (
-    ForceReply,
-    InlineKeyboardMarkup,
-    InputPollOption,
-    MessageEntity,
-    ReplyKeyboardMarkup,
-    ReplyKeyboardRemove,
-)
+from aiogram.methods import SendInvoice
+from aiogram.types import InlineKeyboardMarkup, LabeledPrice
 
 from .base import BaseContent
 
 
-class PollContent(BaseContent):
-    question: str
-    options: List[Union[InputPollOption, str]]
-    business_connection_id: Optional[str] = None
-    question_parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
-    question_entities: Optional[List[MessageEntity]] = None
-    is_anonymous: Optional[bool] = None
-    type: Optional[str] = None
-    allows_multiple_answers: Optional[bool] = None
-    correct_option_id: Optional[int] = None
-    explanation: Optional[str] = None
-    explanation_parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
-    explanation_entities: Optional[List[MessageEntity]] = None
-    open_period: Optional[int] = None
-    close_date: Optional[Union[datetime, timedelta, int]] = None
-    is_closed: Optional[bool] = None
+class InvoiceContent(BaseContent):
+    title: str
+    description: str
+    payload: str
+    currency: str
+    prices: List[LabeledPrice]
+    provider_token: Optional[str] = None
+    max_tip_amount: Optional[int] = None
+    suggested_tip_amounts: Optional[List[int]] = None
+    start_parameter: Optional[str] = None
+    provider_data: Optional[str] = None
+    photo_url: Optional[str] = None
+    photo_size: Optional[int] = None
+    photo_width: Optional[int] = None
+    photo_height: Optional[int] = None
+    need_name: Optional[bool] = None
+    need_phone_number: Optional[bool] = None
+    need_email: Optional[bool] = None
+    need_shipping_address: Optional[bool] = None
+    send_phone_number_to_provider: Optional[bool] = None
+    send_email_to_provider: Optional[bool] = None
+    is_flexible: Optional[bool] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
-    reply_markup: Optional[
-        Union[
-            InlineKeyboardMarkup,
-            ReplyKeyboardMarkup,
-            ReplyKeyboardRemove,
-            ForceReply,
-        ]
-    ] = None
+    message_effect_id: Optional[str] = None
+    reply_markup: Optional[InlineKeyboardMarkup] = None
 
-    async def __call__(self, chat_id: int) -> SendPoll:
-        return SendPoll(
+    async def __call__(self, chat_id: int) -> SendInvoice:
+        return SendInvoice(
             chat_id=chat_id,
-            question=self.question,
-            options=self.options,
-            business_connection_id=self.business_connection_id,
-            question_parse_mode=self.question_parse_mode,
-            question_entities=self.question_entities,
-            is_anonymous=self.is_anonymous,
-            type=self.type,
-            allows_multiple_answers=self.allows_multiple_answers,
-            correct_option_id=self.correct_option_id,
-            explanation=self.explanation,
-            explanation_parse_mode=self.explanation_parse_mode,
-            explanation_entities=self.explanation_entities,
-            open_period=self.open_period,
-            close_date=self.close_date,
-            is_closed=self.is_closed,
+            title=self.title,
+            description=self.description,
+            payload=self.payload,
+            currency=self.currency,
+            prices=self.prices,
+            provider_token=self.provider_token,
+            max_tip_amount=self.max_tip_amount,
+            suggested_tip_amounts=self.suggested_tip_amounts,
+            start_parameter=self.start_parameter,
+            provider_data=self.provider_data,
+            photo_url=self.photo_url,
+            photo_size=self.photo_size,
+            photo_width=self.photo_width,
+            photo_height=self.photo_height,
+            need_name=self.need_name,
+            need_phone_number=self.need_phone_number,
+            need_email=self.need_email,
+            need_shipping_address=self.need_shipping_address,
+            send_phone_number_to_provider=self.send_phone_number_to_provider,
+            send_email_to_provider=self.send_email_to_provider,
+            is_flexible=self.is_flexible,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
-            question: str,
-            options: List[Union[InputPollOption, str]],
-            business_connection_id: Optional[str] = ...,
-            question_parse_mode: Optional[Union[str, Default]] = ...,
-            question_entities: Optional[List[MessageEntity]] = ...,
-            is_anonymous: Optional[bool] = ...,
-            type: Optional[str] = ...,  # noqa: A002
-            allows_multiple_answers: Optional[bool] = ...,
-            correct_option_id: Optional[int] = ...,
-            explanation: Optional[str] = ...,
-            explanation_parse_mode: Optional[Union[str, Default]] = ...,
-            explanation_entities: Optional[List[MessageEntity]] = ...,
-            open_period: Optional[int] = ...,
-            close_date: Optional[Union[datetime, timedelta, int]] = ...,
-            is_closed: Optional[bool] = ...,
+            title: str,
+            description: str,
+            payload: str,
+            currency: str,
+            prices: List[LabeledPrice],
+            provider_token: Optional[str] = ...,
+            max_tip_amount: Optional[int] = ...,
+            suggested_tip_amounts: Optional[List[int]] = ...,
+            start_parameter: Optional[str] = ...,
+            provider_data: Optional[str] = ...,
+            photo_url: Optional[str] = ...,
+            photo_size: Optional[int] = ...,
+            photo_width: Optional[int] = ...,
+            photo_height: Optional[int] = ...,
+            need_name: Optional[bool] = ...,
+            need_phone_number: Optional[bool] = ...,
+            need_email: Optional[bool] = ...,
+            need_shipping_address: Optional[bool] = ...,
+            send_phone_number_to_provider: Optional[bool] = ...,
+            send_email_to_provider: Optional[bool] = ...,
+            is_flexible: Optional[bool] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
-            reply_markup: Optional[
-                Union[
-                    InlineKeyboardMarkup,
-                    ReplyKeyboardMarkup,
-                    ReplyKeyboardRemove,
-                    ForceReply,
-                ]
-            ] = ...,
+            message_effect_id: Optional[str] = ...,
+            reply_markup: Optional[InlineKeyboardMarkup] = ...,
             **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/sticker.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/animation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,87 @@
-from typing import TYPE_CHECKING, Any, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
-from aiogram.methods import SendSticker
+from aiogram.methods import SendAnimation
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
     InputFile,
+    MessageEntity,
     ReplyKeyboardMarkup,
     ReplyKeyboardRemove,
 )
 
 from .base import BaseContent
 
 
-class StickerContent(BaseContent):
-    sticker: Union[InputFile, str]
+class AnimationContent(BaseContent):
+    animation: Union[InputFile, str]
     business_connection_id: Optional[str] = None
-    emoji: Optional[str] = None
+    duration: Optional[int] = None
+    width: Optional[int] = None
+    height: Optional[int] = None
+    thumbnail: Optional[InputFile] = None
+    caption: Optional[str] = None
+    parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
+    caption_entities: Optional[List[MessageEntity]] = None
+    show_caption_above_media: Optional[Union[bool, Default]] = Default("show_caption_above_media")
+    has_spoiler: Optional[bool] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
+    message_effect_id: Optional[str] = None
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
     ] = None
 
-    async def __call__(self, chat_id: int) -> SendSticker:
-        return SendSticker(
+    async def __call__(self, chat_id: int) -> SendAnimation:
+        return SendAnimation(
             chat_id=chat_id,
-            sticker=self.sticker,
+            animation=self.animation,
             business_connection_id=self.business_connection_id,
-            emoji=self.emoji,
+            duration=self.duration,
+            width=self.width,
+            height=self.height,
+            thumbnail=self.thumbnail,
+            caption=self.caption,
+            parse_mode=self.parse_mode,
+            caption_entities=self.caption_entities,
+            show_caption_above_media=self.show_caption_above_media,
+            has_spoiler=self.has_spoiler,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
-            sticker: Union[InputFile, str],
+            animation: Union[InputFile, str],
             business_connection_id: Optional[str] = ...,
-            emoji: Optional[str] = ...,
+            duration: Optional[int] = ...,
+            width: Optional[int] = ...,
+            height: Optional[int] = ...,
+            thumbnail: Optional[InputFile] = ...,
+            caption: Optional[str] = ...,
+            parse_mode: Optional[Union[str, Default]] = ...,
+            caption_entities: Optional[List[MessageEntity]] = ...,
+            show_caption_above_media: Optional[Union[bool, Default]] = ...,
+            has_spoiler: Optional[bool] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            message_effect_id: Optional[str] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/text.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/text.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     text: str
     business_connection_id: Optional[str] = None
     parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
     entities: Optional[List[MessageEntity]] = None
     link_preview_options: Optional[Union[LinkPreviewOptions, Default]] = Default("link_preview")
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
+    message_effect_id: Optional[str] = None
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
@@ -37,14 +38,15 @@
             text=self.text,
             business_connection_id=self.business_connection_id,
             parse_mode=self.parse_mode,
             entities=self.entities,
             link_preview_options=self.link_preview_options,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
@@ -53,14 +55,15 @@
             text: str,
             business_connection_id: Optional[str] = ...,
             parse_mode: Optional[Union[str, Default]] = ...,
             entities: Optional[List[MessageEntity]] = ...,
             link_preview_options: Optional[Union[LinkPreviewOptions, Default]] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            message_effect_id: Optional[str] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/venue.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/venue.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     business_connection_id: Optional[str] = None
     foursquare_id: Optional[str] = None
     foursquare_type: Optional[str] = None
     google_place_id: Optional[str] = None
     google_place_type: Optional[str] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
+    message_effect_id: Optional[str] = None
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
@@ -43,14 +44,15 @@
             business_connection_id=self.business_connection_id,
             foursquare_id=self.foursquare_id,
             foursquare_type=self.foursquare_type,
             google_place_id=self.google_place_id,
             google_place_type=self.google_place_type,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
@@ -63,14 +65,15 @@
             business_connection_id: Optional[str] = ...,
             foursquare_id: Optional[str] = ...,
             foursquare_type: Optional[str] = ...,
             google_place_id: Optional[str] = ...,
             google_place_type: Optional[str] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            message_effect_id: Optional[str] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/video.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/video.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,20 @@
     duration: Optional[int] = None
     width: Optional[int] = None
     height: Optional[int] = None
     thumbnail: Optional[InputFile] = None
     caption: Optional[str] = None
     parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
     caption_entities: Optional[List[MessageEntity]] = None
+    show_caption_above_media: Optional[Union[bool, Default]] = Default("show_caption_above_media")
     has_spoiler: Optional[bool] = None
     supports_streaming: Optional[bool] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
+    message_effect_id: Optional[str] = None
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
@@ -45,18 +47,20 @@
             duration=self.duration,
             width=self.width,
             height=self.height,
             thumbnail=self.thumbnail,
             caption=self.caption,
             parse_mode=self.parse_mode,
             caption_entities=self.caption_entities,
+            show_caption_above_media=self.show_caption_above_media,
             has_spoiler=self.has_spoiler,
             supports_streaming=self.supports_streaming,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
@@ -67,18 +71,20 @@
             duration: Optional[int] = ...,
             width: Optional[int] = ...,
             height: Optional[int] = ...,
             thumbnail: Optional[InputFile] = ...,
             caption: Optional[str] = ...,
             parse_mode: Optional[Union[str, Default]] = ...,
             caption_entities: Optional[List[MessageEntity]] = ...,
+            show_caption_above_media: Optional[Union[bool, Default]] = ...,
             has_spoiler: Optional[bool] = ...,
             supports_streaming: Optional[bool] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            message_effect_id: Optional[str] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/video_note.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/video_note.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     video_note: Union[InputFile, str]
     business_connection_id: Optional[str] = None
     duration: Optional[int] = None
     length: Optional[int] = None
     thumbnail: Optional[InputFile] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
+    message_effect_id: Optional[str] = None
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
@@ -36,14 +37,15 @@
             video_note=self.video_note,
             business_connection_id=self.business_connection_id,
             duration=self.duration,
             length=self.length,
             thumbnail=self.thumbnail,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
@@ -52,14 +54,15 @@
             video_note: Union[InputFile, str],
             business_connection_id: Optional[str] = ...,
             duration: Optional[int] = ...,
             length: Optional[int] = ...,
             thumbnail: Optional[InputFile] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            message_effect_id: Optional[str] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/voice.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/contents/sticker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,62 @@
-from typing import TYPE_CHECKING, Any, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 from aiogram.client.default import Default
-from aiogram.methods import SendVoice
+from aiogram.methods import SendSticker
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
     InputFile,
-    MessageEntity,
     ReplyKeyboardMarkup,
     ReplyKeyboardRemove,
 )
 
 from .base import BaseContent
 
 
-class VoiceContent(BaseContent):
-    voice: Union[InputFile, str]
+class StickerContent(BaseContent):
+    sticker: Union[InputFile, str]
     business_connection_id: Optional[str] = None
-    caption: Optional[str] = None
-    parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
-    caption_entities: Optional[List[MessageEntity]] = None
-    duration: Optional[int] = None
+    emoji: Optional[str] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
+    message_effect_id: Optional[str] = None
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
     ] = None
 
-    async def __call__(self, chat_id: int) -> SendVoice:
-        return SendVoice(
+    async def __call__(self, chat_id: int) -> SendSticker:
+        return SendSticker(
             chat_id=chat_id,
-            voice=self.voice,
+            sticker=self.sticker,
             business_connection_id=self.business_connection_id,
-            caption=self.caption,
-            parse_mode=self.parse_mode,
-            caption_entities=self.caption_entities,
-            duration=self.duration,
+            emoji=self.emoji,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            message_effect_id=self.message_effect_id,
             reply_markup=self.reply_markup,
             **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
-            voice: Union[InputFile, str],
+            sticker: Union[InputFile, str],
             business_connection_id: Optional[str] = ...,
-            caption: Optional[str] = ...,
-            parse_mode: Optional[Union[str, Default]] = ...,
-            caption_entities: Optional[List[MessageEntity]] = ...,
-            duration: Optional[int] = ...,
+            emoji: Optional[str] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            message_effect_id: Optional[str] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/event/manager.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/event/manager.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/event/observer.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/event/observer.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,12 +22,9 @@
             return callback
 
         return wrapper
 
     def register(self, *callbacks: CallbackType) -> Self:
         if not callbacks:
             raise ValueError("At least one callback must be provided to register.")
-        for callback in callbacks:
-            if not callable(callback):
-                raise TypeError("The callback must be callable.")
-            self.callbacks.append(CallableObject(callback=callback))
+        self.callbacks.extend(CallableObject(callback=callback) for callback in callbacks)
         return self
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/event/registry.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/event/registry.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/chat_engine.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/mailer/chat_engine.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/container.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/mailer/container.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,36 +8,36 @@
 class MailerContainer:
     _mailers: Dict[int, Mailer]
 
     def __init__(self, *mailers: Mailer) -> None:
         self._mailers = {mailer.id: mailer for mailer in mailers}
 
     def __repr__(self) -> str:
-        return f"{type(self).__name__}(total_mailers={len(self._mailers)})"
+        return f"{type(self).__name__}(total_mailers={len(self)})"
 
     def __str__(self) -> str:
-        mailers_string = ", ".join(map(repr, self._mailers.values()))
+        mailers_string = ", ".join(map(repr, self))
         return f"{type(self).__name__}[{mailers_string}]"
 
     def __contains__(self, item: int) -> bool:
         return item in self._mailers
 
     def __getitem__(self, item: int) -> Mailer:
         return self._mailers[item]
 
     def __iter__(self) -> Iterator[Mailer]:
-        return iter(self.mailers.values())
+        return iter(self._mailers.values())
 
     def __len__(self) -> int:
         return len(self._mailers)
 
     def __bool__(self) -> bool:
         if not self._mailers:
             return False
-        return all(self._mailers.values())
+        return all(self)
 
     def __hash__(self) -> int:
         return hash(frozenset(self._mailers))
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, MailerContainer):
             return False
@@ -48,9 +48,9 @@
         return MappingProxyType(mapping=self._mailers)
 
     def get_mailer(self, mailer_id: int) -> Optional[Mailer]:
         return self._mailers.get(mailer_id)
 
     def get_mailers(self, *statuses: MailerStatus) -> List[Mailer]:
         if not statuses:
-            return list(self._mailers.values())
-        return [mailer for mailer in self._mailers.values() if mailer.status in statuses]
+            return list(self)
+        return [mailer for mailer in self if mailer.status in statuses]
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/mailer.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/mailer/mailer.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/settings.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/mailer/settings.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/statistic.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/mailer/statistic.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/task_manager.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/mailer/task_manager.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/placeholder/item.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/placeholder/item.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/placeholder/manager.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/placeholder/manager.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/placeholder/placeholder.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/placeholder/placeholder.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/placeholder/registry.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/placeholder/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,30 +58,25 @@
     def chain_keys(self) -> Generator[str, None, None]:
         for registry in self.chain_tail:
             yield from registry.keys
 
     def register(self, *items: PlaceholderItem) -> Self:
         if not items:
             raise ValueError("At least one placeholder item must be provided to register.")
-        for item in items:
-            if not isinstance(item, PlaceholderItem):
-                raise TypeError(
-                    f"The placeholder item must be an instance of "
-                    f"PlaceholderItem, not a {type(item).__name__}.",
-                )
-            self.placeholders.add(item.as_placeholder())
+        self.placeholders.update(item.as_placeholder() for item in items)
         return self
 
     def add(self, __mapping: Optional[Mapping[str, Any]] = None, /, **kwargs: Any) -> Self:
         if __mapping:
             kwargs.update(__mapping)
         if not kwargs:
             raise ValueError("At least one argument must be provided.")
-        for key, value in kwargs.items():
-            self[key] = value
+        self.placeholders.update(
+            Placeholder(key=key, value=value) for key, value in kwargs.items()
+        )
         return self
 
     def _chain_bind(self, entity: "PlaceholderRegistry") -> None:
         for self_registry in self.chain_tail:
             for entity_registry in entity.chain_tail:
                 if collision_keys := self_registry.keys & entity_registry.keys:
                     raise RuntimeError(
```

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/base.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/storages/base.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/file.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/storages/file.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/mongodb.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/storages/mongodb.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/redis.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/storages/redis.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/sqlalchemy.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/storages/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/aiogram_broadcaster/utils/chain.py` & `aiogram_broadcaster-0.5.0/aiogram_broadcaster/utils/chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Any, ClassVar, Generator, Generic, List, Optional, TypeVar
+from typing import Any, ClassVar, Generator, Generic, List, Optional, Type, TypeVar
 
 
 EntityType = TypeVar("EntityType", bound="Chain[Any]")
 
 
 class Chain(Generic[EntityType]):
-    __chain_entity__: EntityType
+    __chain_entity__: Type[EntityType]
     __chain_sub_name__: ClassVar[str]
     __chain_root__: ClassVar[bool]
     name: str
     head: Optional[EntityType]
     tail: List[EntityType]
 
     def __init_subclass__(cls, sub_name: Optional[str] = None, **kwargs: Any) -> None:
```

### Comparing `aiogram_broadcaster-0.4.7/examples/events.py` & `aiogram_broadcaster-0.5.0/examples/events.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/examples/key_based_content.py` & `aiogram_broadcaster-0.5.0/examples/key_based_content.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/examples/lazy_content.py` & `aiogram_broadcaster-0.5.0/examples/lazy_content.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/examples/mre.py` & `aiogram_broadcaster-0.5.0/examples/mre.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/examples/multibot.py` & `aiogram_broadcaster-0.5.0/examples/multibot.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/examples/placeholders.py` & `aiogram_broadcaster-0.5.0/examples/placeholders.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/tests/test_contents/test_base.py` & `aiogram_broadcaster-0.5.0/tests/test_contents/test_base.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/tests/test_contents/test_contents.py` & `aiogram_broadcaster-0.5.0/tests/test_contents/test_contents.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/tests/test_contents/test_key_based.py` & `aiogram_broadcaster-0.5.0/tests/test_contents/test_key_based.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/tests/test_contents/test_lazy.py` & `aiogram_broadcaster-0.5.0/tests/test_contents/test_lazy.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/tests/test_event/test_manager.py` & `aiogram_broadcaster-0.5.0/tests/test_event/test_manager.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/tests/test_event/test_observer.py` & `aiogram_broadcaster-0.5.0/tests/test_event/test_observer.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,23 +34,14 @@
 
         with pytest.raises(
             ValueError,
             match="At least one callback must be provided to register.",
         ):
             observer.register()
 
-    def test_register_non_callable(self):
-        observer = EventObserver()
-
-        with pytest.raises(
-            TypeError,
-            match="The callback must be callable.",
-        ):
-            observer.register("not a callable")
-
     def test_callable_registration(self):
         observer = EventObserver()
 
         @observer()
         def callback():
             pass
```

### Comparing `aiogram_broadcaster-0.4.7/tests/test_event/test_registry.py` & `aiogram_broadcaster-0.5.0/tests/test_event/test_registry.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/tests/test_mailer/test_settings.py` & `aiogram_broadcaster-0.5.0/tests/test_mailer/test_settings.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/tests/test_mailer/test_task_manager.py` & `aiogram_broadcaster-0.5.0/tests/test_mailer/test_task_manager.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/tests/test_placeholder/test_item.py` & `aiogram_broadcaster-0.5.0/tests/test_placeholder/test_item.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/tests/test_placeholder/test_manager.py` & `aiogram_broadcaster-0.5.0/tests/test_placeholder/test_manager.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/tests/test_placeholder/test_placeholder.py` & `aiogram_broadcaster-0.5.0/tests/test_placeholder/test_placeholder.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/tests/test_placeholder/test_registry.py` & `aiogram_broadcaster-0.5.0/tests/test_placeholder/test_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,14 @@
     def test_register_placeholder_items(self):
         registry = PlaceholderRegistry()
         item1 = DummyPlaceholderItem()
         item2 = DummyPlaceholderItem()
         registry.register(item1, item2)
         assert registry.placeholders == {item1.as_placeholder(), item2.as_placeholder()}
         registry = PlaceholderRegistry()
-        with pytest.raises(TypeError):
-            registry.register("invalid_type")
         assert registry.register(item2) == registry
         with pytest.raises(
             ValueError,
             match="At least one placeholder item must be provided to register.",
         ):
             registry.register()
```

### Comparing `aiogram_broadcaster-0.4.7/tests/test_utils/test_chain.py` & `aiogram_broadcaster-0.5.0/tests/test_utils/test_chain.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/tests/test_utils/test_interrupt.py` & `aiogram_broadcaster-0.5.0/tests/test_utils/test_interrupt.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/LICENSE` & `aiogram_broadcaster-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.7/README.md` & `aiogram_broadcaster-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 * #### Supports [multibot](https://github.com/loRes228/aiogram_broadcaster?tab=readme-ov-file#multibot)
 
 ## Installation
 
 * #### From PyPI
 
 ```commandline
-pip install -U aiogram-broadcaster
+pip install --upgrade aiogram-broadcaster
 ```
 
 * #### From GitHub (_Development build_)
 
 ```commandline
-pip install https://github.com/loRes228/aiogram_broadcaster/archive/refs/heads/dev.zip
+pip install https://github.com/loRes228/aiogram_broadcaster/archive/refs/heads/dev.zip --fore-reinstall
 ```
 
 ## Creating a mailer and running broadcasting
 
 #### How to create a mailer and initiate broadcasting.
 
 #### Usage:
@@ -406,17 +406,17 @@
 
 ## Storages
 
 #### Storage allow you to save mailer states to external storage.
 
 * #### [BaseMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/base.py) Abstract class of storage.
 * #### [FileMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/file.py) Saves the mailers to a file.
-* #### [MongoDBMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/mongodb.py) Saves the mailers to a MongoDB.
-* #### [RedisMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/redis.py) Saves the mailers to a Redis.
-* #### [SQLAlchemyMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/sqlalchemy.py) Saves the mailers using SQLAlchemy.
+* #### [MongoDBMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/mongodb.py) Saves the mailers to a MongoDB. (Extra: mongo)
+* #### [RedisMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/redis.py) Saves the mailers to a Redis. (Extra: redis)
+* #### [SQLAlchemyMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/sqlalchemy.py) Saves the mailers using SQLAlchemy. (Extra: sqlalchemy)
 
 #### Usage:
 
 ```python
 from aiogram_broadcaster import Broadcaster
 from aiogram_broadcaster.storages.redis import RedisMailerStorage
```

### Comparing `aiogram_broadcaster-0.4.7/pyproject.toml` & `aiogram_broadcaster-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     "framework",
     "mailing",
     "mailing-system",
     "telegram",
     "wrapper"
 ]
 dependencies = [
-    "aiogram>=3.6.0"
+    "aiogram>=3.7.0"
 ]
 
 [project.optional-dependencies]
 dev = [
     "mypy>=1.10.0",
     "ruff>=0.4.0",
     "types-aiofiles>=23.2.0"
@@ -72,16 +72,18 @@
     "motor>=3.0.0"
 ]
 sqlalchemy = [
     "SQLAlchemy>=2.0.0"
 ]
 
 [project.urls]
-Repository = "https://github.com/loRes228/aiogram_broadcaster.git"
-Issues = "https://github.com/loRes228/aiogram_broadcaster/issues"
+Homepage = "https://github.com/loRes228/aiogram_broadcaster.git"
+Documentation = "https://github.com/loRes228/aiogram_broadcaster#readme"
+"Source code" = "https://github.com/loRes228/aiogram_broadcaster.git"
+"Issue Tracker" = "https://github.com/loRes228/aiogram_broadcaster/issues"
 
 
 [tool.hatch.version]
 path = "aiogram_broadcaster/__meta__.py"
 
 
 [tool.ruff]
```

### Comparing `aiogram_broadcaster-0.4.7/PKG-INFO` & `aiogram_broadcaster-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.3
 Name: aiogram_broadcaster
-Version: 0.4.7
+Version: 0.5.0
 Summary: A lightweight aiogram-based library for broadcasting Telegram messages.
-Project-URL: Repository, https://github.com/loRes228/aiogram_broadcaster.git
-Project-URL: Issues, https://github.com/loRes228/aiogram_broadcaster/issues
+Project-URL: Homepage, https://github.com/loRes228/aiogram_broadcaster.git
+Project-URL: Documentation, https://github.com/loRes228/aiogram_broadcaster#readme
+Project-URL: Source code, https://github.com/loRes228/aiogram_broadcaster.git
+Project-URL: Issue Tracker, https://github.com/loRes228/aiogram_broadcaster/issues
 Author: LORES
 Maintainer: LORES
 License: MIT License
         
         Copyright (c) 2024 LORES
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,15 +43,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: aiogram>=3.6.0
+Requires-Dist: aiogram>=3.7.0
 Provides-Extra: dev
 Requires-Dist: mypy>=1.10.0; extra == 'dev'
 Requires-Dist: ruff>=0.4.0; extra == 'dev'
 Requires-Dist: types-aiofiles>=23.2.0; extra == 'dev'
 Provides-Extra: mongo
 Requires-Dist: motor>=3.0.0; extra == 'mongo'
 Provides-Extra: redis
@@ -88,21 +90,21 @@
 * #### Supports [multibot](https://github.com/loRes228/aiogram_broadcaster?tab=readme-ov-file#multibot)
 
 ## Installation
 
 * #### From PyPI
 
 ```commandline
-pip install -U aiogram-broadcaster
+pip install --upgrade aiogram-broadcaster
 ```
 
 * #### From GitHub (_Development build_)
 
 ```commandline
-pip install https://github.com/loRes228/aiogram_broadcaster/archive/refs/heads/dev.zip
+pip install https://github.com/loRes228/aiogram_broadcaster/archive/refs/heads/dev.zip --fore-reinstall
 ```
 
 ## Creating a mailer and running broadcasting
 
 #### How to create a mailer and initiate broadcasting.
 
 #### Usage:
@@ -472,17 +474,17 @@
 
 ## Storages
 
 #### Storage allow you to save mailer states to external storage.
 
 * #### [BaseMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/base.py) Abstract class of storage.
 * #### [FileMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/file.py) Saves the mailers to a file.
-* #### [MongoDBMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/mongodb.py) Saves the mailers to a MongoDB.
-* #### [RedisMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/redis.py) Saves the mailers to a Redis.
-* #### [SQLAlchemyMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/sqlalchemy.py) Saves the mailers using SQLAlchemy.
+* #### [MongoDBMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/mongodb.py) Saves the mailers to a MongoDB. (Extra: mongo)
+* #### [RedisMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/redis.py) Saves the mailers to a Redis. (Extra: redis)
+* #### [SQLAlchemyMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/sqlalchemy.py) Saves the mailers using SQLAlchemy. (Extra: sqlalchemy)
 
 #### Usage:
 
 ```python
 from aiogram_broadcaster import Broadcaster
 from aiogram_broadcaster.storages.redis import RedisMailerStorage
```

