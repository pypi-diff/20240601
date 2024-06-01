# Comparing `tmp/monstr-0.1.5.tar.gz` & `tmp/monstr-0.1.6.tar.gz`

## Comparing `monstr-0.1.5.tar` & `monstr-0.1.6.tar`

### file list

```diff
@@ -1,86 +1,91 @@
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 monstr-0.1.5/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/backup.py
--rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/create_test_environment.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/entities.py
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/giftwrap_chat.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/keys.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/nip44_post.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/nip4_post.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/note_listen.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/note_listen_auth.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/note_post.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/post_auth.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/post_pow.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/post_signer.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/post_text.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/print_text_notes.py
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/query.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/republish.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/run_relay.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/run_relay_auth.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/run_relay_auth_sub.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/run_relay_mem_store.py
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/simple_bot.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/single_query.py
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 monstr-0.1.5/examples/view_profile.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/__init__.py
--rw-r--r--   0        0        0    19257 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/encrypt.py
--rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/entities.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/exception.py
--rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/giftwrap.py
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/inbox.py
--rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/signing.py
--rw-r--r--   0        0        0     8157 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/channels/__init__.py
--rw-r--r--   0        0        0     7060 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/channels/channel.py
--rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/channels/event_handlers.py
--rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/channels/persist.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/client/__init__.py
--rw-r--r--   0        0        0    47903 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/client/client.py
--rw-r--r--   0        0        0    11076 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/client/event_handlers.py
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/client/messaging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/data/__init__.py
--rw-r--r--   0        0        0    13946 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/data/data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/db/__init__.py
--rw-r--r--   0        0        0    15723 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/db/db.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/event/__init__.py
--rw-r--r--   0        0        0    20402 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/event/event.py
--rw-r--r--   0        0        0    18258 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/event/event_handlers.py
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/event/expire.py
--rw-r--r--   0        0        0    29044 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/event/persist.py
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/event/persist_memory.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/event/persist_postgres.py
--rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/event/persist_sqlite.py
--rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/event/persist_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/ident/__init__.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/ident/alias.py
--rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/ident/event_handlers.py
--rw-r--r--   0        0        0    30307 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/ident/persist.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/ident/persist_test.py
--rw-r--r--   0        0        0    27579 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/ident/profile.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/relay/__init__.py
--rw-r--r--   0        0        0    11408 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/relay/accept_handlers.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/relay/exceptions.py
--rw-r--r--   0        0        0    28631 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/relay/relay.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/settings/__init__.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/settings/handler.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/settings/persist.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/spam_handlers/__init__.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 monstr-0.1.5/src/monstr/spam_handlers/spam_handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 monstr-0.1.5/tests/nip13.py
--rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 monstr-0.1.5/tests/nip19.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 monstr-0.1.5/tests/nip4.py
--rw-r--r--   0        0        0    11387 2020-02-02 00:00:00.000000 monstr-0.1.5/tests/nip44.py
--rw-r--r--   0        0        0    37630 2020-02-02 00:00:00.000000 monstr-0.1.5/tests/nip44.vectors.json
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 monstr-0.1.5/tests/nip59.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 monstr-0.1.5/tests/persist_test.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 monstr-0.1.5/tests/relay_test.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 monstr-0.1.5/tests/scratch.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 monstr-0.1.5/tests/test_texts.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 monstr-0.1.5/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 monstr-0.1.5/LICENSE
--rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 monstr-0.1.5/README.md
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 monstr-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 monstr-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 monstr-0.1.6/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/backup.py
+-rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/create_test_environment.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/entities.py
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/giftwrap_chat.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/keys.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/nip44_post.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/nip4_post.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/note_listen.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/note_listen_auth.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/note_post.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/post_auth.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/post_pow.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/post_signer.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/post_text.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/print_text_notes.py
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/query.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/republish.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/run_relay.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/run_relay_auth.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/run_relay_auth_sub.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/run_relay_mem_store.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/run_relay_tor.py
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/simple_bot.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/single_query.py
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 monstr-0.1.6/examples/view_profile.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.6/src/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/__init__.py
+-rw-r--r--   0        0        0    19257 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/encrypt.py
+-rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/entities.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/exception.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/giftwrap.py
+-rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/inbox.py
+-rw-r--r--   0        0        0     8157 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/channels/__init__.py
+-rw-r--r--   0        0        0     7060 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/channels/channel.py
+-rw-r--r--   0        0        0     8343 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/channels/event_handlers.py
+-rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/channels/persist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/client/__init__.py
+-rw-r--r--   0        0        0    47911 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/client/client.py
+-rw-r--r--   0        0        0    11076 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/client/event_handlers.py
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/client/messaging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/data/__init__.py
+-rw-r--r--   0        0        0    13946 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/data/data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/db/__init__.py
+-rw-r--r--   0        0        0    15723 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/db/db.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/event/__init__.py
+-rw-r--r--   0        0        0    20572 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/event/event.py
+-rw-r--r--   0        0        0    18258 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/event/event_handlers.py
+-rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/event/expire.py
+-rw-r--r--   0        0        0    29044 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/event/persist.py
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/event/persist_memory.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/event/persist_postgres.py
+-rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/event/persist_sqlite.py
+-rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/event/persist_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/ident/__init__.py
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/ident/alias.py
+-rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/ident/event_handlers.py
+-rw-r--r--   0        0        0    30307 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/ident/persist.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/ident/persist_test.py
+-rw-r--r--   0        0        0    27579 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/ident/profile.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/relay/__init__.py
+-rw-r--r--   0        0        0    11408 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/relay/accept_handlers.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/relay/exceptions.py
+-rw-r--r--   0        0        0    28631 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/relay/relay.py
+-rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/relay/tor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/settings/__init__.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/settings/handler.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/settings/persist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/signing/__init__.py
+-rw-r--r--   0        0        0    10019 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/signing/nip46.py
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/signing/signing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/spam_handlers/__init__.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 monstr-0.1.6/src/monstr/spam_handlers/spam_handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monstr-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 monstr-0.1.6/tests/nip13.py
+-rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 monstr-0.1.6/tests/nip19.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 monstr-0.1.6/tests/nip4.py
+-rw-r--r--   0        0        0    11387 2020-02-02 00:00:00.000000 monstr-0.1.6/tests/nip44.py
+-rw-r--r--   0        0        0    37630 2020-02-02 00:00:00.000000 monstr-0.1.6/tests/nip44.vectors.json
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 monstr-0.1.6/tests/nip59.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 monstr-0.1.6/tests/persist_test.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 monstr-0.1.6/tests/relay_test.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 monstr-0.1.6/tests/scratch.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 monstr-0.1.6/tests/test_texts.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 monstr-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 monstr-0.1.6/LICENSE
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 monstr-0.1.6/README.md
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 monstr-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 monstr-0.1.6/PKG-INFO
```

### Comparing `monstr-0.1.5/.github/workflows/python-package.yml` & `monstr-0.1.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/backup.py` & `monstr-0.1.6/examples/backup.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/create_test_environment.py` & `monstr-0.1.6/examples/create_test_environment.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/giftwrap_chat.py` & `monstr-0.1.6/examples/giftwrap_chat.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/keys.py` & `monstr-0.1.6/examples/keys.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/nip44_post.py` & `monstr-0.1.6/examples/nip44_post.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/nip4_post.py` & `monstr-0.1.6/examples/nip4_post.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/note_listen.py` & `monstr-0.1.6/examples/note_listen.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/note_listen_auth.py` & `monstr-0.1.6/examples/note_listen_auth.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/note_post.py` & `monstr-0.1.6/examples/note_post.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/post_auth.py` & `monstr-0.1.6/examples/post_auth.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/post_pow.py` & `monstr-0.1.6/examples/post_pow.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/post_signer.py` & `monstr-0.1.6/examples/post_signer.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/post_text.py` & `monstr-0.1.6/examples/post_text.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/print_text_notes.py` & `monstr-0.1.6/examples/print_text_notes.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/query.py` & `monstr-0.1.6/examples/query.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/republish.py` & `monstr-0.1.6/examples/republish.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/run_relay_auth.py` & `monstr-0.1.6/examples/run_relay_auth.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/run_relay_auth_sub.py` & `monstr-0.1.6/examples/run_relay_auth_sub.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/simple_bot.py` & `monstr-0.1.6/examples/simple_bot.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/single_query.py` & `monstr-0.1.6/examples/single_query.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/examples/view_profile.py` & `monstr-0.1.6/examples/view_profile.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/encrypt.py` & `monstr-0.1.6/src/monstr/encrypt.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/entities.py` & `monstr-0.1.6/src/monstr/entities.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/giftwrap.py` & `monstr-0.1.6/src/monstr/giftwrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import random
 from datetime import datetime
-from monstr.signing import SignerInterface, BasicKeySigner
+from monstr.signing.signing import SignerInterface, BasicKeySigner
 from monstr.encrypt import Keys
 from monstr.event.event import Event
 from monstr.util import util_funcs
 
 
 class GiftWrapException(Exception):
     pass
```

### Comparing `monstr-0.1.5/src/monstr/inbox.py` & `monstr-0.1.6/src/monstr/inbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import hashlib
 import json
 from monstr.encrypt import Keys
-from monstr.signing import SignerInterface
+from monstr.signing.signing import SignerInterface
 from monstr.event.event import Event
 from monstr.util import util_funcs
 
 
 class Inbox:
 
     """
```

### Comparing `monstr-0.1.5/src/monstr/signing.py` & `monstr-0.1.6/src/monstr/signing/signing.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/util.py` & `monstr-0.1.6/src/monstr/util.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/channels/channel.py` & `monstr-0.1.6/src/monstr/channels/channel.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/channels/event_handlers.py` & `monstr-0.1.6/src/monstr/channels/event_handlers.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/channels/persist.py` & `monstr-0.1.6/src/monstr/channels/persist.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/client/client.py` & `monstr-0.1.6/src/monstr/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import asyncio
 import json
 from typing import Callable
 from json import JSONDecodeError
 from datetime import datetime
 from monstr.util import util_funcs
 from monstr.event.event import Event
-from monstr.signing import SignerInterface, BasicKeySigner
+from monstr.signing.signing import SignerInterface, BasicKeySigner
 from monstr.encrypt import Keys
 
 
 class QueryTimeoutException(Exception):
     pass
```

### Comparing `monstr-0.1.5/src/monstr/client/event_handlers.py` & `monstr-0.1.6/src/monstr/client/event_handlers.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/client/messaging.py` & `monstr-0.1.6/src/monstr/client/messaging.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/data/data.py` & `monstr-0.1.6/src/monstr/data/data.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/db/db.py` & `monstr-0.1.6/src/monstr/db/db.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/event/event.py` & `monstr-0.1.6/src/monstr/event/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,18 @@
     # https://github.com/nostr-protocol/nips/blob/af6893145f9a4a63be3d90beffbcfd4d90e872ae/28.md
     KIND_CHANNEL_CREATE = 40
     KIND_CHANNEL_META = 41
     KIND_CHANNEL_MESSAGE = 42
     KIND_CHANNEL_HIDE = 43
     KIND_CHANNEL_MUTE = 44
 
+    # used for messaging in in remote signing as nip46, should be encryped as nip4
+    # https://github.com/nostr-protocol/nips/blob/master/46.md
+    KIND_NIP46 = 24133
+
     # nip 98 http auth header event https://github.com/nostr-protocol/nips/blob/master/98.md
     KIND_HTTP_AUTH = 27235
 
     # nip42 auth event https://github.com/nostr-protocol/nips/blob/master/42.md
     KIND_AUTH = 22242
 
     # a wrapped event to be republished see https://github.com/motorina0/nips/blob/republish_events/705.md
```

### Comparing `monstr-0.1.5/src/monstr/event/event_handlers.py` & `monstr-0.1.6/src/monstr/event/event_handlers.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/event/expire.py` & `monstr-0.1.6/src/monstr/event/expire.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/event/persist.py` & `monstr-0.1.6/src/monstr/event/persist.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/event/persist_memory.py` & `monstr-0.1.6/src/monstr/event/persist_memory.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/event/persist_postgres.py` & `monstr-0.1.6/src/monstr/event/persist_postgres.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/event/persist_sqlite.py` & `monstr-0.1.6/src/monstr/event/persist_sqlite.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/event/persist_test.py` & `monstr-0.1.6/src/monstr/event/persist_test.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/ident/alias.py` & `monstr-0.1.6/src/monstr/ident/alias.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/ident/event_handlers.py` & `monstr-0.1.6/src/monstr/ident/event_handlers.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/ident/persist.py` & `monstr-0.1.6/src/monstr/ident/persist.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/ident/persist_test.py` & `monstr-0.1.6/src/monstr/ident/persist_test.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/ident/profile.py` & `monstr-0.1.6/src/monstr/ident/profile.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/relay/accept_handlers.py` & `monstr-0.1.6/src/monstr/relay/accept_handlers.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/relay/exceptions.py` & `monstr-0.1.6/src/monstr/relay/exceptions.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/relay/relay.py` & `monstr-0.1.6/src/monstr/relay/relay.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/settings/handler.py` & `monstr-0.1.6/src/monstr/settings/handler.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/settings/persist.py` & `monstr-0.1.6/src/monstr/settings/persist.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/src/monstr/spam_handlers/spam_handlers.py` & `monstr-0.1.6/src/monstr/spam_handlers/spam_handlers.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/tests/nip13.py` & `monstr-0.1.6/tests/nip13.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/tests/nip19.py` & `monstr-0.1.6/tests/nip19.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/tests/nip4.py` & `monstr-0.1.6/tests/nip4.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/tests/nip44.py` & `monstr-0.1.6/tests/nip44.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/tests/nip44.vectors.json` & `monstr-0.1.6/tests/nip44.vectors.json`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/tests/nip59.py` & `monstr-0.1.6/tests/nip59.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/tests/persist_test.py` & `monstr-0.1.6/tests/persist_test.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/tests/relay_test.py` & `monstr-0.1.6/tests/relay_test.py`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/tests/test_texts.json` & `monstr-0.1.6/tests/test_texts.json`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/LICENSE` & `monstr-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/README.md` & `monstr-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/pyproject.toml` & `monstr-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monstr-0.1.5/PKG-INFO` & `monstr-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: monstr
-Version: 0.1.5
+Version: 0.1.6
 Summary: Monstr: Python Nostr module. Python code for working with nostr.
 Project-URL: Documentation, https://github.com/monty888/monstr/blob/master/README.md
 Project-URL: Issues, https://github.com/monty888/monstr/issues
 Project-URL: Source, https://github.com/monty888/monstr
 Author-email: Monty888 <Monty888@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

