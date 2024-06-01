# Comparing `tmp/an-website-24.5.tar.gz` & `tmp/an_website-24.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "an-website-24.5.tar", last modified: Thu May 16 06:02:26 2024, max compression
+gzip compressed data, was "an_website-24.6.tar", last modified: Sat Jun  1 18:02:16 2024, max compression
```

## Comparing `an-website-24.5.tar` & `an_website-24.6.tar`

### file list

```diff
@@ -1,468 +1,470 @@
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.543903 an-website-24.5/
--rw-r--r--   0 runner    (1001) docker     (118)     1843 2024-05-16 06:02:16.000000 an-website-24.5/Containerfile
--rw-r--r--   0 runner    (1001) docker     (118)    34351 2024-05-16 06:02:16.000000 an-website-24.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (118)      246 2024-05-16 06:02:16.000000 an-website-24.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (118)     8194 2024-05-16 06:02:26.542904 an-website-24.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (118)     3443 2024-05-16 06:02:16.000000 an-website-24.5/README.md
--rw-r--r--   0 runner    (1001) docker     (118)       40 2024-05-16 06:02:26.000000 an-website-24.5/REVISION.txt
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.473903 an-website-24.5/an_website/
--rw-r--r--   0 runner    (1001) docker     (118)     3742 2024-05-16 06:02:16.000000 an-website-24.5/an_website/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     2004 2024-05-16 06:02:16.000000 an-website-24.5/an_website/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.475903 an-website-24.5/an_website/backdoor/
--rw-r--r--   0 runner    (1001) docker     (118)     1225 2024-05-16 06:02:16.000000 an-website-24.5/an_website/backdoor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)    12974 2024-05-16 06:02:16.000000 an-website-24.5/an_website/backdoor/backdoor.py
--rwxr-xr-x   0 runner    (1001) docker     (118)    23349 2024-05-16 06:02:16.000000 an-website-24.5/an_website/backdoor/client.py
--rw-r--r--   0 runner    (1001) docker     (118)   800629 2024-05-16 06:02:16.000000 an-website-24.5/an_website/ca-bundle.crt
--rw-r--r--   0 runner    (1001) docker     (118)      197 2024-05-16 06:02:16.000000 an-website-24.5/an_website/ca-license.txt
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.475903 an-website-24.5/an_website/commitment/
--rw-r--r--   0 runner    (1001) docker     (118)      829 2024-05-16 06:02:16.000000 an-website-24.5/an_website/commitment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     4699 2024-05-16 06:02:16.000000 an-website-24.5/an_website/commitment/commitment.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.476903 an-website-24.5/an_website/contact/
--rw-r--r--   0 runner    (1001) docker     (118)      861 2024-05-16 06:02:16.000000 an-website-24.5/an_website/contact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     9383 2024-05-16 06:02:16.000000 an-website-24.5/an_website/contact/contact.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.476903 an-website-24.5/an_website/currency_converter/
--rw-r--r--   0 runner    (1001) docker     (118)      843 2024-05-16 06:02:16.000000 an-website-24.5/an_website/currency_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     9496 2024-05-16 06:02:16.000000 an-website-24.5/an_website/currency_converter/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.476903 an-website-24.5/an_website/discord/
--rw-r--r--   0 runner    (1001) docker     (118)      859 2024-05-16 06:02:16.000000 an-website-24.5/an_website/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     6019 2024-05-16 06:02:16.000000 an-website-24.5/an_website/discord/discord.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.463903 an-website-24.5/an_website/elasticsearch/
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.462903 an-website-24.5/an_website/elasticsearch/component_templates/
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.483903 an-website-24.5/an_website/elasticsearch/component_templates/ecs/
--rw-r--r--   0 runner    (1001) docker     (118)    11358 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (118)      581 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (118)     1016 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/agent.json
--rw-r--r--   0 runner    (1001) docker     (118)      481 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/base.json
--rw-r--r--   0 runner    (1001) docker     (118)     5211 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/client.json
--rw-r--r--   0 runner    (1001) docker     (118)     1996 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/cloud.json
--rw-r--r--   0 runner    (1001) docker     (118)     2344 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/container.json
--rw-r--r--   0 runner    (1001) docker     (118)      528 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/data_stream.json
--rw-r--r--   0 runner    (1001) docker     (118)     5221 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/destination.json
--rw-r--r--   0 runner    (1001) docker     (118)     7487 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/dll.json
--rw-r--r--   0 runner    (1001) docker     (118)     2406 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/dns.json
--rw-r--r--   0 runner    (1001) docker     (118)      378 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/ecs.json
--rw-r--r--   0 runner    (1001) docker     (118)     2992 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/email.json
--rw-r--r--   0 runner    (1001) docker     (118)      875 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/error.json
--rw-r--r--   0 runner    (1001) docker     (118)     2761 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/event.json
--rw-r--r--   0 runner    (1001) docker     (118)    17010 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/file.json
--rw-r--r--   0 runner    (1001) docker     (118)      589 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/group.json
--rw-r--r--   0 runner    (1001) docker     (118)     6913 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/host.json
--rw-r--r--   0 runner    (1001) docker     (118)     2327 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/http.json
--rw-r--r--   0 runner    (1001) docker     (118)     2217 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/log.json
--rw-r--r--   0 runner    (1001) docker     (118)     2169 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/network.json
--rw-r--r--   0 runner    (1001) docker     (118)     6135 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/observer.json
--rw-r--r--   0 runner    (1001) docker     (118)     1506 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/orchestrator.json
--rw-r--r--   0 runner    (1001) docker     (118)      627 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/organization.json
--rw-r--r--   0 runner    (1001) docker     (118)     1618 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/package.json
--rw-r--r--   0 runner    (1001) docker     (118)    59330 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/process.json
--rw-r--r--   0 runner    (1001) docker     (118)     1110 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/registry.json
--rw-r--r--   0 runner    (1001) docker     (118)      656 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/related.json
--rw-r--r--   0 runner    (1001) docker     (118)     1347 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/rule.json
--rw-r--r--   0 runner    (1001) docker     (118)     5211 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/server.json
--rw-r--r--   0 runner    (1001) docker     (118)     1341 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/service.json
--rw-r--r--   0 runner    (1001) docker     (118)     5211 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/source.json
--rw-r--r--   0 runner    (1001) docker     (118)    73278 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/threat.json
--rw-r--r--   0 runner    (1001) docker     (118)    11965 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/tls.json
--rw-r--r--   0 runner    (1001) docker     (118)      724 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/tracing.json
--rw-r--r--   0 runner    (1001) docker     (118)     1914 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/url.json
--rw-r--r--   0 runner    (1001) docker     (118)     6976 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/user.json
--rw-r--r--   0 runner    (1001) docker     (118)     2182 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/user_agent.json
--rw-r--r--   0 runner    (1001) docker     (118)     1966 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/vulnerability.json
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.483903 an-website-24.5/an_website/elasticsearch/index_templates/
--rw-r--r--   0 runner    (1001) docker     (118)      824 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/index_templates/reporting.json
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.484903 an-website-24.5/an_website/elasticsearch/index_templates/shortener/
--rw-r--r--   0 runner    (1001) docker     (118)      385 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/index_templates/shortener/shorten.json
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.484903 an-website-24.5/an_website/elasticsearch/ingest_pipelines/
--rw-r--r--   0 runner    (1001) docker     (118)      336 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/ingest_pipelines/reporting.json
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.484903 an-website-24.5/an_website/elasticsearch/ingest_pipelines/shortener/
--rw-r--r--   0 runner    (1001) docker     (118)      285 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/ingest_pipelines/shortener/shorten.json
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.484903 an-website-24.5/an_website/element_web_link/
--rw-r--r--   0 runner    (1001) docker     (118)      836 2024-05-16 06:02:16.000000 an-website-24.5/an_website/element_web_link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     1243 2024-05-16 06:02:16.000000 an-website-24.5/an_website/element_web_link/element_web_link.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.485903 an-website-24.5/an_website/emoji_chat/
--rw-r--r--   0 runner    (1001) docker     (118)      816 2024-05-16 06:02:16.000000 an-website-24.5/an_website/emoji_chat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)    12091 2024-05-16 06:02:16.000000 an-website-24.5/an_website/emoji_chat/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.485903 an-website-24.5/an_website/endpoints/
--rw-r--r--   0 runner    (1001) docker     (118)      837 2024-05-16 06:02:16.000000 an-website-24.5/an_website/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     4254 2024-05-16 06:02:16.000000 an-website-24.5/an_website/endpoints/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.485903 an-website-24.5/an_website/example/
--rw-r--r--   0 runner    (1001) docker     (118)      812 2024-05-16 06:02:16.000000 an-website-24.5/an_website/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     2666 2024-05-16 06:02:16.000000 an-website-24.5/an_website/example/example.py
--rw-r--r--   0 runner    (1001) docker     (118)     4469 2024-05-16 06:02:16.000000 an-website-24.5/an_website/fake_orjson.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.486903 an-website-24.5/an_website/hangman_solver/
--rw-r--r--   0 runner    (1001) docker     (118)      846 2024-05-16 06:02:16.000000 an-website-24.5/an_website/hangman_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     5079 2024-05-16 06:02:16.000000 an-website-24.5/an_website/hangman_solver/hangman_solver.py
--rw-r--r--   0 runner    (1001) docker     (118)     3978 2024-05-16 06:02:16.000000 an-website-24.5/an_website/hangman_solver/wordgame_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.486903 an-website-24.5/an_website/host_info/
--rw-r--r--   0 runner    (1001) docker     (118)      838 2024-05-16 06:02:16.000000 an-website-24.5/an_website/host_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     5245 2024-05-16 06:02:16.000000 an-website-24.5/an_website/host_info/host_info.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.486903 an-website-24.5/an_website/js_licenses/
--rw-r--r--   0 runner    (1001) docker     (118)      860 2024-05-16 06:02:16.000000 an-website-24.5/an_website/js_licenses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     3513 2024-05-16 06:02:16.000000 an-website-24.5/an_website/js_licenses/js_licenses.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.487903 an-website-24.5/an_website/kangaroo_comics/
--rw-r--r--   0 runner    (1001) docker     (118)      851 2024-05-16 06:02:16.000000 an-website-24.5/an_website/kangaroo_comics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     2421 2024-05-16 06:02:16.000000 an-website-24.5/an_website/kangaroo_comics/comics.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.487903 an-website-24.5/an_website/lolwut/
--rw-r--r--   0 runner    (1001) docker     (118)      832 2024-05-16 06:02:16.000000 an-website-24.5/an_website/lolwut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     3186 2024-05-16 06:02:16.000000 an-website-24.5/an_website/lolwut/lolwut.py
--rw-r--r--   0 runner    (1001) docker     (118)    42730 2024-05-16 06:02:16.000000 an-website-24.5/an_website/main.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.487903 an-website-24.5/an_website/main_page/
--rw-r--r--   0 runner    (1001) docker     (118)      833 2024-05-16 06:02:16.000000 an-website-24.5/an_website/main_page/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     1801 2024-05-16 06:02:16.000000 an-website-24.5/an_website/main_page/main_page.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.488903 an-website-24.5/an_website/patches/
--rw-r--r--   0 runner    (1001) docker     (118)    12034 2024-05-16 06:02:16.000000 an-website-24.5/an_website/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     1738 2024-05-16 06:02:16.000000 an-website-24.5/an_website/patches/braille.py
--rw-r--r--   0 runner    (1001) docker     (118)     3944 2024-05-16 06:02:16.000000 an-website-24.5/an_website/patches/json.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.488903 an-website-24.5/an_website/ping/
--rw-r--r--   0 runner    (1001) docker     (118)      832 2024-05-16 06:02:16.000000 an-website-24.5/an_website/ping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     1644 2024-05-16 06:02:16.000000 an-website-24.5/an_website/ping/ping.py
--rw-r--r--   0 runner    (1001) docker     (118)    62500 2024-05-16 06:02:16.000000 an-website-24.5/an_website/primes.bin
--rw-r--r--   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:16.000000 an-website-24.5/an_website/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.490903 an-website-24.5/an_website/quotes/
--rw-r--r--   0 runner    (1001) docker     (118)     6032 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     9977 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/create.py
--rwxr-xr-x   0 runner    (1001) docker     (118)     1437 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/edit.sh
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.490903 an-website-24.5/an_website/quotes/files/
--rw-r--r--   0 runner    (1001) docker     (118)     5101 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/files/StempelNichtWitzig.png
--rw-r--r--   0 runner    (1001) docker     (118)     3058 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/files/StempelWitzig.png
--rw-r--r--   0 runner    (1001) docker     (118)    42308 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/files/bg.png
--rw-r--r--   0 runner    (1001) docker     (118)    50944 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/files/oswald.regular.ttf
--rw-r--r--   0 runner    (1001) docker     (118)     2800 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/generator.py
--rw-r--r--   0 runner    (1001) docker     (118)    12882 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/image.py
--rw-r--r--   0 runner    (1001) docker     (118)     7514 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/info.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.491903 an-website-24.5/an_website/quotes/quote_of_the_day/
--rw-r--r--   0 runner    (1001) docker     (118)     5687 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/quote_of_the_day/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     2509 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/quote_of_the_day/data.py
--rw-r--r--   0 runner    (1001) docker     (118)     5544 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/quote_of_the_day/store.py
--rw-r--r--   0 runner    (1001) docker     (118)    17654 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/quotes.py
--rw-r--r--   0 runner    (1001) docker     (118)     1574 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/share.py
--rw-r--r--   0 runner    (1001) docker     (118)    26353 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.491903 an-website-24.5/an_website/random_text/
--rw-r--r--   0 runner    (1001) docker     (118)      839 2024-05-16 06:02:16.000000 an-website-24.5/an_website/random_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     4126 2024-05-16 06:02:16.000000 an-website-24.5/an_website/random_text/random_text.py
--rw-r--r--   0 runner    (1001) docker     (118)  3039490 2024-05-16 06:02:16.000000 an-website-24.5/an_website/random_text/words.txt
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.494903 an-website-24.5/an_website/redirect/
--rw-r--r--   0 runner    (1001) docker     (118)      837 2024-05-16 06:02:16.000000 an-website-24.5/an_website/redirect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     2514 2024-05-16 06:02:16.000000 an-website-24.5/an_website/redirect/redirect.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.495903 an-website-24.5/an_website/reporting/
--rw-r--r--   0 runner    (1001) docker     (118)      837 2024-05-16 06:02:16.000000 an-website-24.5/an_website/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     8680 2024-05-16 06:02:16.000000 an-website-24.5/an_website/reporting/reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.495903 an-website-24.5/an_website/search/
--rw-r--r--   0 runner    (1001) docker     (118)      847 2024-05-16 06:02:16.000000 an-website-24.5/an_website/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     9733 2024-05-16 06:02:16.000000 an-website-24.5/an_website/search/search.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.495903 an-website-24.5/an_website/services/
--rw-r--r--   0 runner    (1001) docker     (118)      866 2024-05-16 06:02:16.000000 an-website-24.5/an_website/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     3716 2024-05-16 06:02:16.000000 an-website-24.5/an_website/services/services.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.496903 an-website-24.5/an_website/settings/
--rw-r--r--   0 runner    (1001) docker     (118)      846 2024-05-16 06:02:16.000000 an-website-24.5/an_website/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     4739 2024-05-16 06:02:16.000000 an-website-24.5/an_website/settings/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.496903 an-website-24.5/an_website/snow/
--rw-r--r--   0 runner    (1001) docker     (118)     1111 2024-05-16 06:02:16.000000 an-website-24.5/an_website/snow/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.496903 an-website-24.5/an_website/soundboard/
--rw-r--r--   0 runner    (1001) docker     (118)     3334 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     7982 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/data.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.506903 an-website-24.5/an_website/soundboard/files/
--rw-r--r--   0 runner    (1001) docker     (118)    50432 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/dietmar-ich_hab_seine_hausaufgaben_aufgegessen.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    70592 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/fw-ihr_linken_intellektuellen_fuzzies.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    43007 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/gott-das_ist_privat.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    81459 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/gott-so_so_du_hast_also_keine_eier.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    48858 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/jesus-guck_mal_was_ich_kann.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    53986 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-aber_nicht_zu_lidl.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    74486 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-alles_kapitalismus_alles_nestle_alles_haehnchen.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    28211 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-das_ist_freiwillig.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    84635 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-finsterstes_mittelalter_alter.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    46007 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-hallo.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    72923 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-hier_sind_wir_jetzt_unterhalte_uns.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    41997 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-i_love_it.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    49865 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-ich_bin_kommunist.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    59749 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-ich_darf_nich_und_ich_will_nich.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    90810 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-im_so_happy_for_no_reason_but_i_dont_care.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    48353 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-ja_ja.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    56648 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-kein_problem_ich_hab_zeit.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    47101 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-koestlich.mp3
--rw-r--r--   0 runner    (1001) docker     (118)   113893 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-man_darf_nie_aufhoeren_alles_kritisch_zu_hinterfragen.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    48043 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-ohh_hee.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    70477 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-this_kinda_feels_really_really_awesome.mp3
--rw-r--r--   0 runner    (1001) docker     (118)   191215 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-wir_kaempfen_fuer_eine_gerechte_weltordnung_brot_fuer_alle_und_die_aechtung_von_sogennanntem_musikfernsehen.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    57217 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-wir_sind_keine_intellektuellen.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    51169 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-wolln_wir_uns_dutzen.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    38466 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kuh-ahamumumu.mp3
--rw-r--r--   0 runner    (1001) docker     (118)   120162 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-du_bist_also_teil_der_juedisch-bolschewistischen_weltverschwoerung.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    39036 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-fuer_nichts_und_wieder_nichts.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    67629 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-i_am_bored.mp3
--rw-r--r--   0 runner    (1001) docker     (118)   134445 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-i_am_bored_in_the_usa.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    89930 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-im_just_here_for_the_famous_breakfast.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    33069 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-ja_herzlich_willkommen.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    39663 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-sprich_bitte_nur_fuer_dich.mp3
--rw-r--r--   0 runner    (1001) docker     (118)   189292 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-ueber_mich_hat_die_zeit_geschrieben_dass_ich_der_wahrscheinlich_einflussreichste_linke_interlektulelle_deutschlands_sei.mp3
--rw-r--r--   0 runner    (1001) docker     (118)   127434 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-und_da_ist_mir_aufgefallen_dass_ich_keine_eier_hab.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    56423 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-und_mich_dann_auch_noch_beschneiden_lassen.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    48303 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-von_mir_aus.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    44620 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-yeah.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    25452 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/psychiater-aha.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    43250 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/sarah-hey_thats_cool.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    46290 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/sarah-i_love_life.mp3
--rw-r--r--   0 runner    (1001) docker     (118)   155900 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/sarah-thats_amazing_its_like_you_know_i_dont_know_kind_of_like_whatever_and_stuff.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    61219 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/sarah-the_world_is_so_beautiful.mp3
--rw-r--r--   0 runner    (1001) docker     (118)   138254 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/sarah-well_thats_just_like_you_know_amazing.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    68839 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/sarah-yes_its_just_perfect.mp3
--rw-r--r--   0 runner    (1001) docker     (118)    48809 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/icon.svg
--rw-r--r--   0 runner    (1001) docker     (118)     5010 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/info.json
--rw-r--r--   0 runner    (1001) docker     (118)     6481 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/soundboard.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.507903 an-website-24.5/an_website/static/
--rw-r--r--   0 runner    (1001) docker     (118)      199 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/.env
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.511903 an-website-24.5/an_website/static/css/
--rw-r--r--   0 runner    (1001) docker     (118)      144 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/ansi2html.css
--rw-r--r--   0 runner    (1001) docker     (118)      329 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/ansi2html.css.map
--rw-r--r--   0 runner    (1001) docker     (118)     5793 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/base.css
--rw-r--r--   0 runner    (1001) docker     (118)    13928 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/base.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      437 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/comic.css
--rw-r--r--   0 runner    (1001) docker     (118)     1034 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/comic.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      358 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/emoji_chat.css
--rw-r--r--   0 runner    (1001) docker     (118)      771 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/emoji_chat.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      210 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/error.css
--rw-r--r--   0 runner    (1001) docker     (118)      510 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/error.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      750 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/form.css
--rw-r--r--   0 runner    (1001) docker     (118)     1682 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/form.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      599 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/kangaroo_comics.css
--rw-r--r--   0 runner    (1001) docker     (118)     1424 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/kangaroo_comics.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      174 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/main_page.css
--rw-r--r--   0 runner    (1001) docker     (118)      424 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/main_page.css.map
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.513903 an-website-24.5/an_website/static/css/quotes/
--rw-r--r--   0 runner    (1001) docker     (118)      480 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/generator.css
--rw-r--r--   0 runner    (1001) docker     (118)     1043 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/generator.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      549 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/info.css
--rw-r--r--   0 runner    (1001) docker     (118)     1317 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/info.css.map
--rw-r--r--   0 runner    (1001) docker     (118)     2205 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/quotes.css
--rw-r--r--   0 runner    (1001) docker     (118)     4984 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/quotes.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      806 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/share.css
--rw-r--r--   0 runner    (1001) docker     (118)     2038 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/share.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      436 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/redirect.css
--rw-r--r--   0 runner    (1001) docker     (118)     1076 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/redirect.css.map
--rw-r--r--   0 runner    (1001) docker     (118)    52690 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/snow.css
--rw-r--r--   0 runner    (1001) docker     (118)    42520 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/snow.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      479 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/soundboard.css
--rw-r--r--   0 runner    (1001) docker     (118)     1074 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/soundboard.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      492 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/table.css
--rw-r--r--   0 runner    (1001) docker     (118)     1051 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/table.css.map
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.516903 an-website-24.5/an_website/static/css/themes/
--rw-r--r--   0 runner    (1001) docker     (118)      342 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/blue.css
--rw-r--r--   0 runner    (1001) docker     (118)      779 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/blue.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      786 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/christmas.css
--rw-r--r--   0 runner    (1001) docker     (118)     1889 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/christmas.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      345 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/default.css
--rw-r--r--   0 runner    (1001) docker     (118)      782 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/default.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      384 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/fun.css
--rw-r--r--   0 runner    (1001) docker     (118)      810 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/fun.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      347 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/green.css
--rw-r--r--   0 runner    (1001) docker     (118)      784 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/green.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      355 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/light.css
--rw-r--r--   0 runner    (1001) docker     (118)      792 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/light.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      360 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/light_blue.css
--rw-r--r--   0 runner    (1001) docker     (118)      797 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/light_blue.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      342 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/orange.css
--rw-r--r--   0 runner    (1001) docker     (118)      779 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/orange.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      341 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/pink.css
--rw-r--r--   0 runner    (1001) docker     (118)      778 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/pink.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      343 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/purple.css
--rw-r--r--   0 runner    (1001) docker     (118)      780 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/purple.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      341 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/yellow.css
--rw-r--r--   0 runner    (1001) docker     (118)      778 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/yellow.css.map
--rw-r--r--   0 runner    (1001) docker     (118)      250 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/uptime.css
--rw-r--r--   0 runner    (1001) docker     (118)      599 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/uptime.css.map
--rw-r--r--   0 runner    (1001) docker     (118)     9109 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/favicon.jxl
--rw-r--r--   0 runner    (1001) docker     (118)    12948 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.517903 an-website-24.5/an_website/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (118)      538 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/fonts/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (118)    33916 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/fonts/comic.woff2
--rw-r--r--   0 runner    (1001) docker     (118)    12152 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/fonts/comicmono.woff2
--rw-r--r--   0 runner    (1001) docker     (118)     4120 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/fonts/cursedtimerulil-aznm.woff2
--rw-r--r--   0 runner    (1001) docker     (118)      377 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/humans.txt
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.520903 an-website-24.5/an_website/static/img/
--rw-r--r--   0 runner    (1001) docker     (118)  1047428 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/2020-11-03.jpg
--rw-r--r--   0 runner    (1001) docker     (118)      763 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (118)      258 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/arrow.svg
--rw-r--r--   0 runner    (1001) docker     (118)      405 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/close.svg
--rw-r--r--   0 runner    (1001) docker     (118)      467 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/hamburger-menu-icon.svg
--rw-r--r--   0 runner    (1001) docker     (118)    23613 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/kangarooface.svg
--rw-r--r--   0 runner    (1001) docker     (118)    24121 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/logo.svg
--rw-r--r--   0 runner    (1001) docker     (118)     1444 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/netcup-oekostrom2.jxl
--rw-r--r--   0 runner    (1001) docker     (118)     2592 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/netcup-oekostrom2.png
--rw-r--r--   0 runner    (1001) docker     (118)      161 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/plus.svg
--rw-r--r--   0 runner    (1001) docker     (118)      197 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/report.svg
--rw-r--r--   0 runner    (1001) docker     (118)      589 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/rss.svg
--rw-r--r--   0 runner    (1001) docker     (118)      597 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/save.svg
--rw-r--r--   0 runner    (1001) docker     (118)      472 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/share.svg
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.520903 an-website-24.5/an_website/static/img/stamps/
--rw-r--r--   0 runner    (1001) docker     (118)     8849 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/stamps/nichtwitzig.small.svg
--rw-r--r--   0 runner    (1001) docker     (118)     5797 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/stamps/witzig.small.svg
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.468903 an-website-24.5/an_website/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.521903 an-website-24.5/an_website/static/js/currency_converter/
--rw-r--r--   0 runner    (1001) docker     (118)     2021 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/currency_converter/converter.js
--rw-r--r--   0 runner    (1001) docker     (118)     8735 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/currency_converter/converter.js.map
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.521903 an-website-24.5/an_website/static/js/emoji_chat/
--rw-r--r--   0 runner    (1001) docker     (118)     3023 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/emoji_chat/chat.js
--rw-r--r--   0 runner    (1001) docker     (118)    11583 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/emoji_chat/chat.js.map
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.521903 an-website-24.5/an_website/static/js/hangman_solver/
--rw-r--r--   0 runner    (1001) docker     (118)     3978 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/hangman_solver/hangman_solver.js
--rw-r--r--   0 runner    (1001) docker     (118)    17899 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/hangman_solver/hangman_solver.js.map
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.522904 an-website-24.5/an_website/static/js/kangaroo_comics/
--rw-r--r--   0 runner    (1001) docker     (118)     7855 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/kangaroo_comics/comics.js
--rw-r--r--   0 runner    (1001) docker     (118)    22718 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/kangaroo_comics/comics.js.map
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.522904 an-website-24.5/an_website/static/js/quotes/
--rw-r--r--   0 runner    (1001) docker     (118)      485 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/quotes/create.js
--rw-r--r--   0 runner    (1001) docker     (118)     1634 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/quotes/create.js.map
--rw-r--r--   0 runner    (1001) docker     (118)     3144 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/quotes/quotes.js
--rw-r--r--   0 runner    (1001) docker     (118)    12154 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/quotes/quotes.js.map
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.523903 an-website-24.5/an_website/static/js/search/
--rw-r--r--   0 runner    (1001) docker     (118)      790 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/search/search.js
--rw-r--r--   0 runner    (1001) docker     (118)     2600 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/search/search.js.map
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.523903 an-website-24.5/an_website/static/js/settings/
--rw-r--r--   0 runner    (1001) docker     (118)     1440 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/settings/settings.js
--rw-r--r--   0 runner    (1001) docker     (118)     4676 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/settings/settings.js.map
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.523903 an-website-24.5/an_website/static/js/snow/
--rw-r--r--   0 runner    (1001) docker     (118)     1219 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/snow/snow.js
--rw-r--r--   0 runner    (1001) docker     (118)     5306 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/snow/snow.js.map
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.524903 an-website-24.5/an_website/static/js/swapped_words/
--rw-r--r--   0 runner    (1001) docker     (118)     1274 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/swapped_words/swap.js
--rw-r--r--   0 runner    (1001) docker     (118)     4000 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/swapped_words/swap.js.map
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.524903 an-website-24.5/an_website/static/js/uptime/
--rw-r--r--   0 runner    (1001) docker     (118)      585 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/uptime/uptime.js
--rw-r--r--   0 runner    (1001) docker     (118)     2236 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/uptime/uptime.js.map
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.525903 an-website-24.5/an_website/static/js/utils/
--rw-r--r--   0 runner    (1001) docker     (118)     1165 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/utils/better_ui.js
--rw-r--r--   0 runner    (1001) docker     (118)     3610 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/utils/better_ui.js.map
--rw-r--r--   0 runner    (1001) docker     (118)     2923 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/utils/dynload.js
--rw-r--r--   0 runner    (1001) docker     (118)    10506 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/utils/dynload.js.map
--rw-r--r--   0 runner    (1001) docker     (118)     1995 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/utils/utils.js
--rw-r--r--   0 runner    (1001) docker     (118)     6498 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/utils/utils.js.map
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.525903 an-website-24.5/an_website/static/js/vendored/
--rw-r--r--   0 runner    (1001) docker     (118)    95822 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/vendored/vanilla.js
--rw-r--r--   0 runner    (1001) docker     (118)   534836 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/vendored/vanilla.js.map
--rw-r--r--   0 runner    (1001) docker     (118)      354 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/manifest.json
--rw-r--r--   0 runner    (1001) docker     (118)       77 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.526903 an-website-24.5/an_website/swapped_words/
--rw-r--r--   0 runner    (1001) docker     (118)     1794 2024-05-16 06:02:16.000000 an-website-24.5/an_website/swapped_words/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)      926 2024-05-16 06:02:16.000000 an-website-24.5/an_website/swapped_words/config.sw
--rw-r--r--   0 runner    (1001) docker     (118)    12837 2024-05-16 06:02:16.000000 an-website-24.5/an_website/swapped_words/config_file.py
--rw-r--r--   0 runner    (1001) docker     (118)     6238 2024-05-16 06:02:16.000000 an-website-24.5/an_website/swapped_words/swap.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.527903 an-website-24.5/an_website/templates/
--rw-r--r--   0 runner    (1001) docker     (118)      559 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/ansi2html.html
--rw-r--r--   0 runner    (1001) docker     (118)     3650 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (118)      557 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (118)     4964 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (118)     3004 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.530903 an-website-24.5/an_website/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (118)      392 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/EXAMPLE.html
--rw-r--r--   0 runner    (1001) docker     (118)      985 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/contact.html
--rw-r--r--   0 runner    (1001) docker     (118)     1854 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/converter.html
--rw-r--r--   0 runner    (1001) docker     (118)     1130 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/emoji_chat.html
--rw-r--r--   0 runner    (1001) docker     (118)       70 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/empty.html
--rw-r--r--   0 runner    (1001) docker     (118)     1128 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/endpoints.html
--rw-r--r--   0 runner    (1001) docker     (118)     3405 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/hangman_solver.html
--rw-r--r--   0 runner    (1001) docker     (118)      116 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/ip.html
--rw-r--r--   0 runner    (1001) docker     (118)      804 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/js_licenses.html
--rw-r--r--   0 runner    (1001) docker     (118)     1064 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/kangaroo_comics.html
--rw-r--r--   0 runner    (1001) docker     (118)     1973 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/main_page.html
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.532904 an-website-24.5/an_website/templates/pages/quotes/
--rw-r--r--   0 runner    (1001) docker     (118)      343 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/author_info.html
--rw-r--r--   0 runner    (1001) docker     (118)     2210 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/create1.html
--rw-r--r--   0 runner    (1001) docker     (118)     1843 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/create2.html
--rw-r--r--   0 runner    (1001) docker     (118)     1349 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/generator.html
--rw-r--r--   0 runner    (1001) docker     (118)     2284 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/info.html
--rw-r--r--   0 runner    (1001) docker     (118)     2960 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/main_page.html
--rw-r--r--   0 runner    (1001) docker     (118)      196 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/quote_info.html
--rw-r--r--   0 runner    (1001) docker     (118)     7157 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/quotes.html
--rw-r--r--   0 runner    (1001) docker     (118)     6779 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/share.html
--rw-r--r--   0 runner    (1001) docker     (118)     1183 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/redirect.html
--rw-r--r--   0 runner    (1001) docker     (118)      990 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/search.html
--rw-r--r--   0 runner    (1001) docker     (118)      968 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/services.html
--rw-r--r--   0 runner    (1001) docker     (118)     4530 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/settings.html
--rw-r--r--   0 runner    (1001) docker     (118)     1057 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/soundboard.html
--rw-r--r--   0 runner    (1001) docker     (118)     1843 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/swapped_words.html
--rw-r--r--   0 runner    (1001) docker     (118)      841 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/troet.html
--rw-r--r--   0 runner    (1001) docker     (118)      930 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/uptime.html
--rw-r--r--   0 runner    (1001) docker     (118)      847 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/version.html
--rw-r--r--   0 runner    (1001) docker     (118)      964 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/wordgame_solver.html
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.532904 an-website-24.5/an_website/templates/rss/
--rw-r--r--   0 runner    (1001) docker     (118)     1108 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/rss/quote_of_the_day.xml
--rw-r--r--   0 runner    (1001) docker     (118)      495 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/rss/soundboard.xml
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.532904 an-website-24.5/an_website/troet/
--rw-r--r--   0 runner    (1001) docker     (118)      833 2024-05-16 06:02:16.000000 an-website-24.5/an_website/troet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     2761 2024-05-16 06:02:16.000000 an-website-24.5/an_website/troet/troet.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.533903 an-website-24.5/an_website/update/
--rw-r--r--   0 runner    (1001) docker     (118)      837 2024-05-16 06:02:16.000000 an-website-24.5/an_website/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     4490 2024-05-16 06:02:16.000000 an-website-24.5/an_website/update/update.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.533903 an-website-24.5/an_website/uptime/
--rw-r--r--   0 runner    (1001) docker     (118)      863 2024-05-16 06:02:16.000000 an-website-24.5/an_website/uptime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     6967 2024-05-16 06:02:16.000000 an-website-24.5/an_website/uptime/uptime.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.535904 an-website-24.5/an_website/utils/
--rw-r--r--   0 runner    (1001) docker     (118)     1679 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)    40385 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/base_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (118)     9147 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/better_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (118)     6771 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/data_parsing.py
--rw-r--r--   0 runner    (1001) docker     (118)     7845 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (118)     4964 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (118)     8104 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (118)     9034 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (118)     4751 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/search.py
--rw-r--r--   0 runner    (1001) docker     (118)     6982 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/static_file_from_traversable.py
--rw-r--r--   0 runner    (1001) docker     (118)     6753 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/static_file_handling.py
--rw-r--r--   0 runner    (1001) docker     (118)     5326 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/token.py
--rw-r--r--   0 runner    (1001) docker     (118)    25599 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.536903 an-website-24.5/an_website/vendored/
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.537903 an-website-24.5/an_website/vendored/apm-rum/
--rw-r--r--   0 runner    (1001) docker     (118)   579743 2024-05-16 06:02:16.000000 an-website-24.5/an_website/vendored/apm-rum/elastic-apm-rum.umd.js
--rw-r--r--   0 runner    (1001) docker     (118)    61332 2024-05-16 06:02:16.000000 an-website-24.5/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js
--rw-r--r--   0 runner    (1001) docker     (118)   263069 2024-05-16 06:02:16.000000 an-website-24.5/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js.map
--rw-r--r--   0 runner    (1001) docker     (118)    56683 2024-05-16 06:02:16.000000 an-website-24.5/an_website/vendored/media-types.json
--rw-r--r--   0 runner    (1001) docker     (118)   205599 2024-05-16 06:02:16.000000 an-website-24.5/an_website/vendored/mime-db.json
--rwxr-xr-x   0 runner    (1001) docker     (118)   255236 2024-05-16 06:02:16.000000 an-website-24.5/an_website/vendored/screenfetch
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.538904 an-website-24.5/an_website/version/
--rw-r--r--   0 runner    (1001) docker     (118)      836 2024-05-16 06:02:16.000000 an-website-24.5/an_website/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     3862 2024-05-16 06:02:16.000000 an-website-24.5/an_website/version/version.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.538904 an-website-24.5/an_website/whats_my_ip/
--rw-r--r--   0 runner    (1001) docker     (118)      845 2024-05-16 06:02:17.000000 an-website-24.5/an_website/whats_my_ip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     2496 2024-05-16 06:02:17.000000 an-website-24.5/an_website/whats_my_ip/ip.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.538904 an-website-24.5/an_website/wiki/
--rw-r--r--   0 runner    (1001) docker     (118)      848 2024-05-16 06:02:17.000000 an-website-24.5/an_website/wiki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (118)     1883 2024-05-16 06:02:17.000000 an-website-24.5/an_website/wiki/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.542904 an-website-24.5/an_website.egg-info/
--rw-r--r--   0 runner    (1001) docker     (118)     8194 2024-05-16 06:02:26.000000 an-website-24.5/an_website.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (118)    16466 2024-05-16 06:02:26.000000 an-website-24.5/an_website.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (118)        1 2024-05-16 06:02:26.000000 an-website-24.5/an_website.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (118)      109 2024-05-16 06:02:26.000000 an-website-24.5/an_website.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (118)        1 2024-05-16 06:02:23.000000 an-website-24.5/an_website.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (118)     1861 2024-05-16 06:02:26.000000 an-website-24.5/an_website.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (118)       11 2024-05-16 06:02:26.000000 an-website-24.5/an_website.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (118)     1750 2024-05-16 06:02:17.000000 an-website-24.5/build-oci-image.sh
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.539903 an-website-24.5/example-configurations/
--rw-r--r--   0 runner    (1001) docker     (118)     1528 2024-05-16 06:02:17.000000 an-website-24.5/example-configurations/config.ini.default
--rw-r--r--   0 runner    (1001) docker     (118)     2328 2024-05-16 06:02:17.000000 an-website-24.5/example-configurations/config.ini.example
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.539903 an-website-24.5/example-configurations/nginx/
--rw-r--r--   0 runner    (1001) docker     (118)     1874 2024-05-16 06:02:17.000000 an-website-24.5/example-configurations/nginx/an-website.conf
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.539903 an-website-24.5/example-configurations/supervisord/
--rw-r--r--   0 runner    (1001) docker     (118)      200 2024-05-16 06:02:17.000000 an-website-24.5/example-configurations/supervisord/an_website.ini
--rw-r--r--   0 runner    (1001) docker     (118)     3034 2024-05-16 06:02:17.000000 an-website-24.5/pip-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (118)     1032 2024-05-16 06:02:17.000000 an-website-24.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (118)       38 2024-05-16 06:02:26.543903 an-website-24.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (118)     3602 2024-05-16 06:02:17.000000 an-website-24.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.541903 an-website-24.5/tests/
--rw-r--r--   0 runner    (1001) docker     (118)     8267 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_backdoor.py
--rw-r--r--   0 runner    (1001) docker     (118)     1226 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_christmas.py
--rw-r--r--   0 runner    (1001) docker     (118)     4847 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_commitment.py
--rw-r--r--   0 runner    (1001) docker     (118)     3517 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_contact.py
--rw-r--r--   0 runner    (1001) docker     (118)     2402 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_currency_converter.py
--rw-r--r--   0 runner    (1001) docker     (118)     3476 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_hangman_solver.py
--rw-r--r--   0 runner    (1001) docker     (118)     6783 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (118)     5772 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (118)    13039 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_quotes.py
--rw-r--r--   0 runner    (1001) docker     (118)     1666 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_random_text.py
--rw-r--r--   0 runner    (1001) docker     (118)    18637 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_request_handlers.py
--rw-r--r--   0 runner    (1001) docker     (118)     5374 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (118)    11416 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_swapped_words.py
--rw-r--r--   0 runner    (1001) docker     (118)     2557 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_token.py
--rw-r--r--   0 runner    (1001) docker     (118)     3402 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_traversable_static_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (118)     2769 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_troet.py
--rw-r--r--   0 runner    (1001) docker     (118)     1956 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_uptime.py
--rw-r--r--   0 runner    (1001) docker     (118)     5609 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.633020 an_website-24.6/
+-rw-r--r--   0 runner    (1001) docker     (118)     1843 2024-06-01 18:02:11.000000 an_website-24.6/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (118)    34351 2024-06-01 18:02:11.000000 an_website-24.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (118)      246 2024-06-01 18:02:11.000000 an_website-24.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (118)     8142 2024-06-01 18:02:16.632020 an_website-24.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (118)     3443 2024-06-01 18:02:11.000000 an_website-24.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (118)       40 2024-06-01 18:02:16.000000 an_website-24.6/REVISION.txt
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.561020 an_website-24.6/an_website/
+-rw-r--r--   0 runner    (1001) docker     (118)     3742 2024-06-01 18:02:11.000000 an_website-24.6/an_website/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2004 2024-06-01 18:02:11.000000 an_website-24.6/an_website/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.563020 an_website-24.6/an_website/backdoor/
+-rw-r--r--   0 runner    (1001) docker     (118)     1225 2024-06-01 18:02:11.000000 an_website-24.6/an_website/backdoor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)    12974 2024-06-01 18:02:11.000000 an_website-24.6/an_website/backdoor/backdoor.py
+-rwxr-xr-x   0 runner    (1001) docker     (118)    23349 2024-06-01 18:02:11.000000 an_website-24.6/an_website/backdoor/client.py
+-rw-r--r--   0 runner    (1001) docker     (118)   800629 2024-06-01 18:02:11.000000 an_website-24.6/an_website/ca-bundle.crt
+-rw-r--r--   0 runner    (1001) docker     (118)      197 2024-06-01 18:02:11.000000 an_website-24.6/an_website/ca-license.txt
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.563020 an_website-24.6/an_website/commitment/
+-rw-r--r--   0 runner    (1001) docker     (118)      829 2024-06-01 18:02:11.000000 an_website-24.6/an_website/commitment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4699 2024-06-01 18:02:11.000000 an_website-24.6/an_website/commitment/commitment.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.564020 an_website-24.6/an_website/contact/
+-rw-r--r--   0 runner    (1001) docker     (118)      861 2024-06-01 18:02:11.000000 an_website-24.6/an_website/contact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     9573 2024-06-01 18:02:11.000000 an_website-24.6/an_website/contact/contact.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.564020 an_website-24.6/an_website/currency_converter/
+-rw-r--r--   0 runner    (1001) docker     (118)      843 2024-06-01 18:02:11.000000 an_website-24.6/an_website/currency_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     9496 2024-06-01 18:02:11.000000 an_website-24.6/an_website/currency_converter/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.564020 an_website-24.6/an_website/discord/
+-rw-r--r--   0 runner    (1001) docker     (118)      859 2024-06-01 18:02:11.000000 an_website-24.6/an_website/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6019 2024-06-01 18:02:11.000000 an_website-24.6/an_website/discord/discord.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.550020 an_website-24.6/an_website/elasticsearch/
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.550020 an_website-24.6/an_website/elasticsearch/component_templates/
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.571020 an_website-24.6/an_website/elasticsearch/component_templates/ecs/
+-rw-r--r--   0 runner    (1001) docker     (118)    11358 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (118)      581 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (118)     1016 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/agent.json
+-rw-r--r--   0 runner    (1001) docker     (118)      481 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/base.json
+-rw-r--r--   0 runner    (1001) docker     (118)     5211 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/client.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1996 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/cloud.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2344 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/container.json
+-rw-r--r--   0 runner    (1001) docker     (118)      528 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/data_stream.json
+-rw-r--r--   0 runner    (1001) docker     (118)     5221 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/destination.json
+-rw-r--r--   0 runner    (1001) docker     (118)     7487 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/dll.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2406 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/dns.json
+-rw-r--r--   0 runner    (1001) docker     (118)      378 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/ecs.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2992 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/email.json
+-rw-r--r--   0 runner    (1001) docker     (118)      875 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/error.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2761 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/event.json
+-rw-r--r--   0 runner    (1001) docker     (118)    17010 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/file.json
+-rw-r--r--   0 runner    (1001) docker     (118)      589 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/group.json
+-rw-r--r--   0 runner    (1001) docker     (118)     6913 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/host.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2327 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/http.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2217 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/log.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2169 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/network.json
+-rw-r--r--   0 runner    (1001) docker     (118)     6135 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/observer.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1506 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/orchestrator.json
+-rw-r--r--   0 runner    (1001) docker     (118)      627 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/organization.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1618 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/package.json
+-rw-r--r--   0 runner    (1001) docker     (118)    59330 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/process.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1110 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/registry.json
+-rw-r--r--   0 runner    (1001) docker     (118)      656 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/related.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1347 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/rule.json
+-rw-r--r--   0 runner    (1001) docker     (118)     5211 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/server.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1341 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/service.json
+-rw-r--r--   0 runner    (1001) docker     (118)     5211 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/source.json
+-rw-r--r--   0 runner    (1001) docker     (118)    73278 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/threat.json
+-rw-r--r--   0 runner    (1001) docker     (118)    11965 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/tls.json
+-rw-r--r--   0 runner    (1001) docker     (118)      724 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/tracing.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1914 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/url.json
+-rw-r--r--   0 runner    (1001) docker     (118)     6976 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/user.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2182 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/user_agent.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1966 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/component_templates/ecs/vulnerability.json
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.571020 an_website-24.6/an_website/elasticsearch/index_templates/
+-rw-r--r--   0 runner    (1001) docker     (118)      824 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/index_templates/reporting.json
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.572020 an_website-24.6/an_website/elasticsearch/index_templates/shortener/
+-rw-r--r--   0 runner    (1001) docker     (118)      385 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/index_templates/shortener/shorten.json
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.572020 an_website-24.6/an_website/elasticsearch/ingest_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (118)      336 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/ingest_pipelines/reporting.json
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.572020 an_website-24.6/an_website/elasticsearch/ingest_pipelines/shortener/
+-rw-r--r--   0 runner    (1001) docker     (118)      285 2024-06-01 18:02:11.000000 an_website-24.6/an_website/elasticsearch/ingest_pipelines/shortener/shorten.json
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.572020 an_website-24.6/an_website/element_web_link/
+-rw-r--r--   0 runner    (1001) docker     (118)      836 2024-06-01 18:02:11.000000 an_website-24.6/an_website/element_web_link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1243 2024-06-01 18:02:11.000000 an_website-24.6/an_website/element_web_link/element_web_link.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.573020 an_website-24.6/an_website/emoji_chat/
+-rw-r--r--   0 runner    (1001) docker     (118)      816 2024-06-01 18:02:11.000000 an_website-24.6/an_website/emoji_chat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)    12095 2024-06-01 18:02:11.000000 an_website-24.6/an_website/emoji_chat/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.573020 an_website-24.6/an_website/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (118)      837 2024-06-01 18:02:11.000000 an_website-24.6/an_website/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4254 2024-06-01 18:02:11.000000 an_website-24.6/an_website/endpoints/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.573020 an_website-24.6/an_website/example/
+-rw-r--r--   0 runner    (1001) docker     (118)      812 2024-06-01 18:02:11.000000 an_website-24.6/an_website/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2666 2024-06-01 18:02:11.000000 an_website-24.6/an_website/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4469 2024-06-01 18:02:11.000000 an_website-24.6/an_website/fake_orjson.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.574020 an_website-24.6/an_website/hangman_solver/
+-rw-r--r--   0 runner    (1001) docker     (118)      846 2024-06-01 18:02:11.000000 an_website-24.6/an_website/hangman_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5079 2024-06-01 18:02:11.000000 an_website-24.6/an_website/hangman_solver/hangman_solver.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3978 2024-06-01 18:02:11.000000 an_website-24.6/an_website/hangman_solver/wordgame_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.574020 an_website-24.6/an_website/host_info/
+-rw-r--r--   0 runner    (1001) docker     (118)      838 2024-06-01 18:02:11.000000 an_website-24.6/an_website/host_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5245 2024-06-01 18:02:11.000000 an_website-24.6/an_website/host_info/host_info.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.574020 an_website-24.6/an_website/js_licenses/
+-rw-r--r--   0 runner    (1001) docker     (118)      860 2024-06-01 18:02:11.000000 an_website-24.6/an_website/js_licenses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3513 2024-06-01 18:02:11.000000 an_website-24.6/an_website/js_licenses/js_licenses.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.575020 an_website-24.6/an_website/kangaroo_comics/
+-rw-r--r--   0 runner    (1001) docker     (118)      851 2024-06-01 18:02:11.000000 an_website-24.6/an_website/kangaroo_comics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2421 2024-06-01 18:02:11.000000 an_website-24.6/an_website/kangaroo_comics/comics.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.575020 an_website-24.6/an_website/lolwut/
+-rw-r--r--   0 runner    (1001) docker     (118)      832 2024-06-01 18:02:11.000000 an_website-24.6/an_website/lolwut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3186 2024-06-01 18:02:11.000000 an_website-24.6/an_website/lolwut/lolwut.py
+-rw-r--r--   0 runner    (1001) docker     (118)    34967 2024-06-01 18:02:11.000000 an_website-24.6/an_website/main.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.575020 an_website-24.6/an_website/main_page/
+-rw-r--r--   0 runner    (1001) docker     (118)      833 2024-06-01 18:02:11.000000 an_website-24.6/an_website/main_page/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1801 2024-06-01 18:02:11.000000 an_website-24.6/an_website/main_page/main_page.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.576020 an_website-24.6/an_website/patches/
+-rw-r--r--   0 runner    (1001) docker     (118)    12264 2024-06-01 18:02:11.000000 an_website-24.6/an_website/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1738 2024-06-01 18:02:11.000000 an_website-24.6/an_website/patches/braille.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3944 2024-06-01 18:02:11.000000 an_website-24.6/an_website/patches/json.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.576020 an_website-24.6/an_website/ping/
+-rw-r--r--   0 runner    (1001) docker     (118)      832 2024-06-01 18:02:11.000000 an_website-24.6/an_website/ping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1644 2024-06-01 18:02:11.000000 an_website-24.6/an_website/ping/ping.py
+-rw-r--r--   0 runner    (1001) docker     (118)    62500 2024-06-01 18:02:11.000000 an_website-24.6/an_website/primes.bin
+-rw-r--r--   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:11.000000 an_website-24.6/an_website/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.578020 an_website-24.6/an_website/quotes/
+-rw-r--r--   0 runner    (1001) docker     (118)     6151 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     9977 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/create.py
+-rwxr-xr-x   0 runner    (1001) docker     (118)     1437 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/edit.sh
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.579020 an_website-24.6/an_website/quotes/files/
+-rw-r--r--   0 runner    (1001) docker     (118)     5101 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/files/StempelNichtWitzig.png
+-rw-r--r--   0 runner    (1001) docker     (118)     3058 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/files/StempelWitzig.png
+-rw-r--r--   0 runner    (1001) docker     (118)    42308 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/files/bg.png
+-rw-r--r--   0 runner    (1001) docker     (118)    50944 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/files/oswald.regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (118)     2800 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/generator.py
+-rw-r--r--   0 runner    (1001) docker     (118)    12882 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/image.py
+-rw-r--r--   0 runner    (1001) docker     (118)     7514 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/info.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.579020 an_website-24.6/an_website/quotes/quote_of_the_day/
+-rw-r--r--   0 runner    (1001) docker     (118)     5687 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/quote_of_the_day/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2509 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/quote_of_the_day/data.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5544 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/quote_of_the_day/store.py
+-rw-r--r--   0 runner    (1001) docker     (118)    17654 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/quotes.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1574 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/share.py
+-rw-r--r--   0 runner    (1001) docker     (118)    26567 2024-06-01 18:02:11.000000 an_website-24.6/an_website/quotes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.580020 an_website-24.6/an_website/random_text/
+-rw-r--r--   0 runner    (1001) docker     (118)      839 2024-06-01 18:02:11.000000 an_website-24.6/an_website/random_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4126 2024-06-01 18:02:11.000000 an_website-24.6/an_website/random_text/random_text.py
+-rw-r--r--   0 runner    (1001) docker     (118)  3039490 2024-06-01 18:02:11.000000 an_website-24.6/an_website/random_text/words.txt
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.583020 an_website-24.6/an_website/redirect/
+-rw-r--r--   0 runner    (1001) docker     (118)      837 2024-06-01 18:02:11.000000 an_website-24.6/an_website/redirect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2827 2024-06-01 18:02:11.000000 an_website-24.6/an_website/redirect/redirect.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.583020 an_website-24.6/an_website/reporting/
+-rw-r--r--   0 runner    (1001) docker     (118)      837 2024-06-01 18:02:11.000000 an_website-24.6/an_website/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     8680 2024-06-01 18:02:11.000000 an_website-24.6/an_website/reporting/reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.583020 an_website-24.6/an_website/search/
+-rw-r--r--   0 runner    (1001) docker     (118)      847 2024-06-01 18:02:11.000000 an_website-24.6/an_website/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     9733 2024-06-01 18:02:11.000000 an_website-24.6/an_website/search/search.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.583020 an_website-24.6/an_website/services/
+-rw-r--r--   0 runner    (1001) docker     (118)      866 2024-06-01 18:02:11.000000 an_website-24.6/an_website/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3716 2024-06-01 18:02:11.000000 an_website-24.6/an_website/services/services.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.584020 an_website-24.6/an_website/settings/
+-rw-r--r--   0 runner    (1001) docker     (118)      846 2024-06-01 18:02:11.000000 an_website-24.6/an_website/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4739 2024-06-01 18:02:11.000000 an_website-24.6/an_website/settings/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.584020 an_website-24.6/an_website/snow/
+-rw-r--r--   0 runner    (1001) docker     (118)     1111 2024-06-01 18:02:11.000000 an_website-24.6/an_website/snow/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.585020 an_website-24.6/an_website/soundboard/
+-rw-r--r--   0 runner    (1001) docker     (118)     3334 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     7982 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/data.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.594020 an_website-24.6/an_website/soundboard/files/
+-rw-r--r--   0 runner    (1001) docker     (118)    50432 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/dietmar-ich_hab_seine_hausaufgaben_aufgegessen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    70592 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/fw-ihr_linken_intellektuellen_fuzzies.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    43007 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/gott-das_ist_privat.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    81459 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/gott-so_so_du_hast_also_keine_eier.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    48858 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/jesus-guck_mal_was_ich_kann.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    53986 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/kaenguru-aber_nicht_zu_lidl.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    74486 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/kaenguru-alles_kapitalismus_alles_nestle_alles_haehnchen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    28211 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/kaenguru-das_ist_freiwillig.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    84635 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/kaenguru-finsterstes_mittelalter_alter.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    46007 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/kaenguru-hallo.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    72923 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/kaenguru-hier_sind_wir_jetzt_unterhalte_uns.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    41997 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/kaenguru-i_love_it.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    49865 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/kaenguru-ich_bin_kommunist.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    59749 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/kaenguru-ich_darf_nich_und_ich_will_nich.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    90810 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/kaenguru-im_so_happy_for_no_reason_but_i_dont_care.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    48353 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/kaenguru-ja_ja.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    56648 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/kaenguru-kein_problem_ich_hab_zeit.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    47101 2024-06-01 18:02:11.000000 an_website-24.6/an_website/soundboard/files/kaenguru-koestlich.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   113893 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/kaenguru-man_darf_nie_aufhoeren_alles_kritisch_zu_hinterfragen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    48043 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/kaenguru-ohh_hee.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    70477 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/kaenguru-this_kinda_feels_really_really_awesome.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   191215 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/kaenguru-wir_kaempfen_fuer_eine_gerechte_weltordnung_brot_fuer_alle_und_die_aechtung_von_sogennanntem_musikfernsehen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    57217 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/kaenguru-wir_sind_keine_intellektuellen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    51169 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/kaenguru-wolln_wir_uns_dutzen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    38466 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/kuh-ahamumumu.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   120162 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/muk-du_bist_also_teil_der_juedisch-bolschewistischen_weltverschwoerung.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    39036 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/muk-fuer_nichts_und_wieder_nichts.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    67629 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/muk-i_am_bored.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   134445 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/muk-i_am_bored_in_the_usa.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    89930 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/muk-im_just_here_for_the_famous_breakfast.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    33069 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/muk-ja_herzlich_willkommen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    39663 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/muk-sprich_bitte_nur_fuer_dich.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   189292 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/muk-ueber_mich_hat_die_zeit_geschrieben_dass_ich_der_wahrscheinlich_einflussreichste_linke_interlektulelle_deutschlands_sei.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   127434 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/muk-und_da_ist_mir_aufgefallen_dass_ich_keine_eier_hab.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    56423 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/muk-und_mich_dann_auch_noch_beschneiden_lassen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    48303 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/muk-von_mir_aus.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    44620 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/muk-yeah.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    25452 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/psychiater-aha.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    43250 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/sarah-hey_thats_cool.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    46290 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/sarah-i_love_life.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   155900 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/sarah-thats_amazing_its_like_you_know_i_dont_know_kind_of_like_whatever_and_stuff.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    61219 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/sarah-the_world_is_so_beautiful.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   138254 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/sarah-well_thats_just_like_you_know_amazing.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    68839 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/files/sarah-yes_its_just_perfect.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    48809 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (118)     5010 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/info.json
+-rw-r--r--   0 runner    (1001) docker     (118)     6481 2024-06-01 18:02:12.000000 an_website-24.6/an_website/soundboard/soundboard.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.595020 an_website-24.6/an_website/static/
+-rw-r--r--   0 runner    (1001) docker     (118)      199 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/.env
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.599020 an_website-24.6/an_website/static/css/
+-rw-r--r--   0 runner    (1001) docker     (118)      144 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/ansi2html.css
+-rw-r--r--   0 runner    (1001) docker     (118)      329 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/ansi2html.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)     5793 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (118)    13928 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/base.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      437 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/comic.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1034 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/comic.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      358 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/emoji_chat.css
+-rw-r--r--   0 runner    (1001) docker     (118)      771 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/emoji_chat.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      210 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/error.css
+-rw-r--r--   0 runner    (1001) docker     (118)      510 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/error.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      750 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/form.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1682 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/form.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      599 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/kangaroo_comics.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1424 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/kangaroo_comics.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      174 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/main_page.css
+-rw-r--r--   0 runner    (1001) docker     (118)      424 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/main_page.css.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.600020 an_website-24.6/an_website/static/css/quotes/
+-rw-r--r--   0 runner    (1001) docker     (118)      480 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/quotes/generator.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1043 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/quotes/generator.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      549 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/quotes/info.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1317 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/quotes/info.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)     2205 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/quotes/quotes.css
+-rw-r--r--   0 runner    (1001) docker     (118)     4984 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/quotes/quotes.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      806 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/quotes/share.css
+-rw-r--r--   0 runner    (1001) docker     (118)     2038 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/quotes/share.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      436 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/redirect.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1076 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/redirect.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)    52690 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/snow.css
+-rw-r--r--   0 runner    (1001) docker     (118)    42520 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/snow.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      479 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/soundboard.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1074 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/soundboard.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      492 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/table.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1051 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/table.css.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.604020 an_website-24.6/an_website/static/css/themes/
+-rw-r--r--   0 runner    (1001) docker     (118)      342 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/blue.css
+-rw-r--r--   0 runner    (1001) docker     (118)      779 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/blue.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      786 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/christmas.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1889 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/christmas.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      345 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/default.css
+-rw-r--r--   0 runner    (1001) docker     (118)      782 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/default.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      384 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/fun.css
+-rw-r--r--   0 runner    (1001) docker     (118)      810 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/fun.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      347 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/green.css
+-rw-r--r--   0 runner    (1001) docker     (118)      784 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/green.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      355 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/light.css
+-rw-r--r--   0 runner    (1001) docker     (118)      792 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/light.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      360 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/light_blue.css
+-rw-r--r--   0 runner    (1001) docker     (118)      797 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/light_blue.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      342 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/orange.css
+-rw-r--r--   0 runner    (1001) docker     (118)      779 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/orange.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      341 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/pink.css
+-rw-r--r--   0 runner    (1001) docker     (118)      778 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/pink.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      343 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/purple.css
+-rw-r--r--   0 runner    (1001) docker     (118)      780 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/purple.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      341 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (118)      778 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/themes/yellow.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      250 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/uptime.css
+-rw-r--r--   0 runner    (1001) docker     (118)      599 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/css/uptime.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)     9109 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/favicon.jxl
+-rw-r--r--   0 runner    (1001) docker     (118)    12948 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.605020 an_website-24.6/an_website/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (118)      538 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/fonts/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (118)    33916 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/fonts/comic.woff2
+-rw-r--r--   0 runner    (1001) docker     (118)    12152 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/fonts/comicmono.woff2
+-rw-r--r--   0 runner    (1001) docker     (118)     4120 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/fonts/cursedtimerulil-aznm.woff2
+-rw-r--r--   0 runner    (1001) docker     (118)      377 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/humans.txt
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.608020 an_website-24.6/an_website/static/img/
+-rw-r--r--   0 runner    (1001) docker     (118)  1047428 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/2020-11-03.jpg
+-rw-r--r--   0 runner    (1001) docker     (118)      763 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (118)      258 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (118)      405 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/close.svg
+-rw-r--r--   0 runner    (1001) docker     (118)      467 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/hamburger-menu-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (118)    23613 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/kangarooface.svg
+-rw-r--r--   0 runner    (1001) docker     (118)    24121 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (118)     1444 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/netcup-oekostrom2.jxl
+-rw-r--r--   0 runner    (1001) docker     (118)     2592 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/netcup-oekostrom2.png
+-rw-r--r--   0 runner    (1001) docker     (118)      161 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/plus.svg
+-rw-r--r--   0 runner    (1001) docker     (118)      197 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/report.svg
+-rw-r--r--   0 runner    (1001) docker     (118)      589 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/rss.svg
+-rw-r--r--   0 runner    (1001) docker     (118)      597 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/save.svg
+-rw-r--r--   0 runner    (1001) docker     (118)      472 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/share.svg
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.608020 an_website-24.6/an_website/static/img/stamps/
+-rw-r--r--   0 runner    (1001) docker     (118)     8849 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/stamps/nichtwitzig.small.svg
+-rw-r--r--   0 runner    (1001) docker     (118)     5797 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/img/stamps/witzig.small.svg
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.556020 an_website-24.6/an_website/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.609020 an_website-24.6/an_website/static/js/currency_converter/
+-rw-r--r--   0 runner    (1001) docker     (118)     2021 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/currency_converter/converter.js
+-rw-r--r--   0 runner    (1001) docker     (118)     8735 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/currency_converter/converter.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.609020 an_website-24.6/an_website/static/js/emoji_chat/
+-rw-r--r--   0 runner    (1001) docker     (118)     3023 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/emoji_chat/chat.js
+-rw-r--r--   0 runner    (1001) docker     (118)    11583 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/emoji_chat/chat.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.609020 an_website-24.6/an_website/static/js/hangman_solver/
+-rw-r--r--   0 runner    (1001) docker     (118)     3978 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/hangman_solver/hangman_solver.js
+-rw-r--r--   0 runner    (1001) docker     (118)    17899 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/hangman_solver/hangman_solver.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.610020 an_website-24.6/an_website/static/js/kangaroo_comics/
+-rw-r--r--   0 runner    (1001) docker     (118)     7855 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/kangaroo_comics/comics.js
+-rw-r--r--   0 runner    (1001) docker     (118)    22718 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/kangaroo_comics/comics.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.610020 an_website-24.6/an_website/static/js/quotes/
+-rw-r--r--   0 runner    (1001) docker     (118)      485 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/quotes/create.js
+-rw-r--r--   0 runner    (1001) docker     (118)     1634 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/quotes/create.js.map
+-rw-r--r--   0 runner    (1001) docker     (118)     3144 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/quotes/quotes.js
+-rw-r--r--   0 runner    (1001) docker     (118)    12154 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/quotes/quotes.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.611020 an_website-24.6/an_website/static/js/search/
+-rw-r--r--   0 runner    (1001) docker     (118)      790 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/search/search.js
+-rw-r--r--   0 runner    (1001) docker     (118)     2600 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/search/search.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.611020 an_website-24.6/an_website/static/js/settings/
+-rw-r--r--   0 runner    (1001) docker     (118)     1440 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/settings/settings.js
+-rw-r--r--   0 runner    (1001) docker     (118)     4676 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/settings/settings.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.611020 an_website-24.6/an_website/static/js/snow/
+-rw-r--r--   0 runner    (1001) docker     (118)     1219 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/snow/snow.js
+-rw-r--r--   0 runner    (1001) docker     (118)     5306 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/snow/snow.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.612020 an_website-24.6/an_website/static/js/swapped_words/
+-rw-r--r--   0 runner    (1001) docker     (118)     1274 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/swapped_words/swap.js
+-rw-r--r--   0 runner    (1001) docker     (118)     4000 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/swapped_words/swap.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.612020 an_website-24.6/an_website/static/js/uptime/
+-rw-r--r--   0 runner    (1001) docker     (118)      585 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/uptime/uptime.js
+-rw-r--r--   0 runner    (1001) docker     (118)     2236 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/uptime/uptime.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.613020 an_website-24.6/an_website/static/js/utils/
+-rw-r--r--   0 runner    (1001) docker     (118)     1165 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/utils/better_ui.js
+-rw-r--r--   0 runner    (1001) docker     (118)     3610 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/utils/better_ui.js.map
+-rw-r--r--   0 runner    (1001) docker     (118)     2923 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/utils/dynload.js
+-rw-r--r--   0 runner    (1001) docker     (118)    10506 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/utils/dynload.js.map
+-rw-r--r--   0 runner    (1001) docker     (118)     1995 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/utils/utils.js
+-rw-r--r--   0 runner    (1001) docker     (118)     6498 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/utils/utils.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.614020 an_website-24.6/an_website/static/js/vendored/
+-rw-r--r--   0 runner    (1001) docker     (118)    95822 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/vendored/vanilla.js
+-rw-r--r--   0 runner    (1001) docker     (118)   534836 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/js/vendored/vanilla.js.map
+-rw-r--r--   0 runner    (1001) docker     (118)      354 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (118)       77 2024-06-01 18:02:12.000000 an_website-24.6/an_website/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.615020 an_website-24.6/an_website/swapped_words/
+-rw-r--r--   0 runner    (1001) docker     (118)     1794 2024-06-01 18:02:12.000000 an_website-24.6/an_website/swapped_words/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)      926 2024-06-01 18:02:12.000000 an_website-24.6/an_website/swapped_words/config.sw
+-rw-r--r--   0 runner    (1001) docker     (118)    12837 2024-06-01 18:02:12.000000 an_website-24.6/an_website/swapped_words/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6238 2024-06-01 18:02:12.000000 an_website-24.6/an_website/swapped_words/swap.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.616020 an_website-24.6/an_website/templates/
+-rw-r--r--   0 runner    (1001) docker     (118)      559 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/ansi2html.html
+-rw-r--r--   0 runner    (1001) docker     (118)     3650 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (118)      557 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (118)     4964 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (118)     3126 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.619020 an_website-24.6/an_website/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (118)      392 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/EXAMPLE.html
+-rw-r--r--   0 runner    (1001) docker     (118)      985 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/contact.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1854 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/converter.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1130 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/emoji_chat.html
+-rw-r--r--   0 runner    (1001) docker     (118)       70 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/empty.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1128 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/endpoints.html
+-rw-r--r--   0 runner    (1001) docker     (118)     3413 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/hangman_solver.html
+-rw-r--r--   0 runner    (1001) docker     (118)      116 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/ip.html
+-rw-r--r--   0 runner    (1001) docker     (118)      804 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/js_licenses.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1064 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/kangaroo_comics.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1973 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/main_page.html
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.621020 an_website-24.6/an_website/templates/pages/quotes/
+-rw-r--r--   0 runner    (1001) docker     (118)      343 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/quotes/author_info.html
+-rw-r--r--   0 runner    (1001) docker     (118)     2210 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/quotes/create1.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1843 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/quotes/create2.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1349 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/quotes/generator.html
+-rw-r--r--   0 runner    (1001) docker     (118)     2284 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/quotes/info.html
+-rw-r--r--   0 runner    (1001) docker     (118)     2960 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/quotes/main_page.html
+-rw-r--r--   0 runner    (1001) docker     (118)      196 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/quotes/quote_info.html
+-rw-r--r--   0 runner    (1001) docker     (118)     7157 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/quotes/quotes.html
+-rw-r--r--   0 runner    (1001) docker     (118)     6865 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/quotes/share.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1183 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/redirect.html
+-rw-r--r--   0 runner    (1001) docker     (118)      990 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/search.html
+-rw-r--r--   0 runner    (1001) docker     (118)      968 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/services.html
+-rw-r--r--   0 runner    (1001) docker     (118)     4669 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/settings.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1057 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/soundboard.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1843 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/swapped_words.html
+-rw-r--r--   0 runner    (1001) docker     (118)      841 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/troet.html
+-rw-r--r--   0 runner    (1001) docker     (118)      930 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/uptime.html
+-rw-r--r--   0 runner    (1001) docker     (118)      847 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/version.html
+-rw-r--r--   0 runner    (1001) docker     (118)      964 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/pages/wordgame_solver.html
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.621020 an_website-24.6/an_website/templates/rss/
+-rw-r--r--   0 runner    (1001) docker     (118)     1108 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/rss/quote_of_the_day.xml
+-rw-r--r--   0 runner    (1001) docker     (118)      495 2024-06-01 18:02:12.000000 an_website-24.6/an_website/templates/rss/soundboard.xml
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.621020 an_website-24.6/an_website/troet/
+-rw-r--r--   0 runner    (1001) docker     (118)      833 2024-06-01 18:02:12.000000 an_website-24.6/an_website/troet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2761 2024-06-01 18:02:12.000000 an_website-24.6/an_website/troet/troet.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.622020 an_website-24.6/an_website/update/
+-rw-r--r--   0 runner    (1001) docker     (118)      837 2024-06-01 18:02:12.000000 an_website-24.6/an_website/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4490 2024-06-01 18:02:12.000000 an_website-24.6/an_website/update/update.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.622020 an_website-24.6/an_website/uptime/
+-rw-r--r--   0 runner    (1001) docker     (118)      863 2024-06-01 18:02:12.000000 an_website-24.6/an_website/uptime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6967 2024-06-01 18:02:12.000000 an_website-24.6/an_website/uptime/uptime.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.624020 an_website-24.6/an_website/utils/
+-rw-r--r--   0 runner    (1001) docker     (118)     1679 2024-06-01 18:02:12.000000 an_website-24.6/an_website/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5720 2024-06-01 18:02:12.000000 an_website-24.6/an_website/utils/background_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (118)    40484 2024-06-01 18:02:12.000000 an_website-24.6/an_website/utils/base_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (118)     9147 2024-06-01 18:02:12.000000 an_website-24.6/an_website/utils/better_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6771 2024-06-01 18:02:12.000000 an_website-24.6/an_website/utils/data_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (118)     7845 2024-06-01 18:02:12.000000 an_website-24.6/an_website/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6375 2024-06-01 18:02:12.000000 an_website-24.6/an_website/utils/elasticsearch_setup.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4964 2024-06-01 18:02:12.000000 an_website-24.6/an_website/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (118)     8104 2024-06-01 18:02:12.000000 an_website-24.6/an_website/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (118)     9076 2024-06-01 18:02:12.000000 an_website-24.6/an_website/utils/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4751 2024-06-01 18:02:12.000000 an_website-24.6/an_website/utils/search.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6982 2024-06-01 18:02:12.000000 an_website-24.6/an_website/utils/static_file_from_traversable.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6753 2024-06-01 18:02:12.000000 an_website-24.6/an_website/utils/static_file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5326 2024-06-01 18:02:12.000000 an_website-24.6/an_website/utils/token.py
+-rw-r--r--   0 runner    (1001) docker     (118)    25880 2024-06-01 18:02:12.000000 an_website-24.6/an_website/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.625020 an_website-24.6/an_website/vendored/
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.627020 an_website-24.6/an_website/vendored/apm-rum/
+-rw-r--r--   0 runner    (1001) docker     (118)   579743 2024-06-01 18:02:12.000000 an_website-24.6/an_website/vendored/apm-rum/elastic-apm-rum.umd.js
+-rw-r--r--   0 runner    (1001) docker     (118)    61332 2024-06-01 18:02:12.000000 an_website-24.6/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js
+-rw-r--r--   0 runner    (1001) docker     (118)   263069 2024-06-01 18:02:12.000000 an_website-24.6/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (118)    56683 2024-06-01 18:02:12.000000 an_website-24.6/an_website/vendored/media-types.json
+-rw-r--r--   0 runner    (1001) docker     (118)   205599 2024-06-01 18:02:12.000000 an_website-24.6/an_website/vendored/mime-db.json
+-rwxr-xr-x   0 runner    (1001) docker     (118)   255236 2024-06-01 18:02:12.000000 an_website-24.6/an_website/vendored/screenfetch
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.627020 an_website-24.6/an_website/version/
+-rw-r--r--   0 runner    (1001) docker     (118)      836 2024-06-01 18:02:12.000000 an_website-24.6/an_website/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3862 2024-06-01 18:02:12.000000 an_website-24.6/an_website/version/version.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.627020 an_website-24.6/an_website/whats_my_ip/
+-rw-r--r--   0 runner    (1001) docker     (118)      845 2024-06-01 18:02:12.000000 an_website-24.6/an_website/whats_my_ip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2496 2024-06-01 18:02:12.000000 an_website-24.6/an_website/whats_my_ip/ip.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.628020 an_website-24.6/an_website/wiki/
+-rw-r--r--   0 runner    (1001) docker     (118)      848 2024-06-01 18:02:12.000000 an_website-24.6/an_website/wiki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1883 2024-06-01 18:02:12.000000 an_website-24.6/an_website/wiki/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.632020 an_website-24.6/an_website.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (118)     8142 2024-06-01 18:02:16.000000 an_website-24.6/an_website.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (118)    16543 2024-06-01 18:02:16.000000 an_website-24.6/an_website.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (118)        1 2024-06-01 18:02:16.000000 an_website-24.6/an_website.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (118)      109 2024-06-01 18:02:16.000000 an_website-24.6/an_website.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (118)        1 2024-06-01 18:02:14.000000 an_website-24.6/an_website.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (118)     1890 2024-06-01 18:02:16.000000 an_website-24.6/an_website.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (118)       11 2024-06-01 18:02:16.000000 an_website-24.6/an_website.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (118)     1750 2024-06-01 18:02:12.000000 an_website-24.6/build-oci-image.sh
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.628020 an_website-24.6/example-configurations/
+-rw-r--r--   0 runner    (1001) docker     (118)     1526 2024-06-01 18:02:12.000000 an_website-24.6/example-configurations/config.ini.default
+-rw-r--r--   0 runner    (1001) docker     (118)     2328 2024-06-01 18:02:12.000000 an_website-24.6/example-configurations/config.ini.example
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.628020 an_website-24.6/example-configurations/nginx/
+-rw-r--r--   0 runner    (1001) docker     (118)     1874 2024-06-01 18:02:12.000000 an_website-24.6/example-configurations/nginx/an-website.conf
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.628020 an_website-24.6/example-configurations/supervisord/
+-rw-r--r--   0 runner    (1001) docker     (118)      200 2024-06-01 18:02:12.000000 an_website-24.6/example-configurations/supervisord/an_website.ini
+-rw-r--r--   0 runner    (1001) docker     (118)     2982 2024-06-01 18:02:12.000000 an_website-24.6/pip-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (118)     1032 2024-06-01 18:02:12.000000 an_website-24.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (118)       38 2024-06-01 18:02:16.633020 an_website-24.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (118)     3602 2024-06-01 18:02:12.000000 an_website-24.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-06-01 18:02:16.631020 an_website-24.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (118)     8267 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_backdoor.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1226 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_christmas.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4847 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_commitment.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3517 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_contact.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2402 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_currency_converter.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3476 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_hangman_solver.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6783 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5772 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (118)    13039 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1666 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_random_text.py
+-rw-r--r--   0 runner    (1001) docker     (118)    18637 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_request_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5374 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (118)    11416 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_swapped_words.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2557 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3402 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_traversable_static_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2769 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_troet.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1956 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_uptime.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5609 2024-06-01 18:02:12.000000 an_website-24.6/tests/test_utils.py
```

### Comparing `an-website-24.5/Containerfile` & `an_website-24.6/Containerfile`

 * *Files identical despite different names*

### Comparing `an-website-24.5/LICENSE.md` & `an_website-24.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `an-website-24.5/PKG-INFO` & `an_website-24.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: an-website
-Version: 24.5
+Version: 24.6
 Summary: #1 Website in the Worlds
 Home-page: https://github.com/asozialesnetzwerk/an-website
 Author: Das Asoziale Netzwerk
 Author-email: contact@asozial.org
 License: AGPL-3.0-or-later
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,32 +25,32 @@
 Requires-Dist: async-timeout==4.0.3; python_full_version < "3.11.3"
 Requires-Dist: attrs==23.2.0; python_version >= "3.7"
 Requires-Dist: beautifulsoup4==4.12.3; python_full_version >= "3.6.0"
 Requires-Dist: blake3==0.4.1
 Requires-Dist: brotli==1.1.0
 Requires-Dist: certifi==2023.11.17; python_version >= "3.6"
 Requires-Dist: cffi==1.16.0; python_version >= "3.8"
-Requires-Dist: defity==0.3.1; python_version >= "3.7"
+Requires-Dist: defity==0.4.0; python_version >= "3.9"
 Requires-Dist: defusedxml==0.7.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"
 Requires-Dist: dill==0.3.8; python_version >= "3.8"
 Requires-Dist: dunamai==1.21.1; python_version >= "3.5"
 Requires-Dist: ecs-logging==2.1.0; python_version >= "3.6"
-Requires-Dist: elastic-apm==6.22.0; python_version >= "3.6" and python_version < "4"
+Requires-Dist: elastic-apm==6.22.2; python_version >= "3.6" and python_version < "4"
 Requires-Dist: elastic-enterprise-search==8.11.0; python_version >= "3.6"
-Requires-Dist: elastic-transport==8.13.0; python_version >= "3.7"
+Requires-Dist: elastic-transport==8.13.1; python_version >= "3.7"
 Requires-Dist: elasticsearch[async]==8.12.1; python_version >= "3.7"
 Requires-Dist: emoji==2.11.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: frozenlist==1.4.1; python_version >= "3.8"
 Requires-Dist: funcparserlib==1.0.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6" and python_version < "3.13"
 Requires-Dist: get-version==3.5.5; python_version >= "3.9"
-Requires-Dist: hangman-solver-rs==0.2.1; python_version >= "3.10"
+Requires-Dist: hangman-solver-rs==0.3.1; python_version >= "3.12"
 Requires-Dist: hiredis==2.3.2
 Requires-Dist: html2text==2020.1.16; python_version >= "3.5"
-Requires-Dist: hy==0.28.0; python_version < "3.13" and python_version >= "3.8"
-Requires-Dist: hyrule==0.5.0; python_version < "3.13"
+Requires-Dist: hy==0.29.0; python_version < "3.13" and python_version >= "3.8"
+Requires-Dist: hyrule==0.6.0; python_version < "3.13"
 Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: jsonpickle==3.0.4; python_version >= "3.7"
 Requires-Dist: lxml==5.2.2; python_version >= "3.6"
 Requires-Dist: multidict==6.0.5; python_version >= "3.7"
 Requires-Dist: openmoji-dist==15.0.0.1
 Requires-Dist: orjson==3.10.3; python_version >= "3.8"
 Requires-Dist: packaging==23.2; python_version >= "3.7"
@@ -63,27 +63,27 @@
 Requires-Dist: pyjwt==2.8.0; python_version >= "3.7"
 Requires-Dist: pysocks==1.7.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: python-dateutil==2.9.0.post0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: python-geoip-geolite2-yplan==2019.1224
 Requires-Dist: python-geoip-yplan==1.2
 Requires-Dist: pytz==2023.4
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
-Requires-Dist: rapidfuzz==3.9.0; python_version >= "3.8"
+Requires-Dist: rapidfuzz==3.9.3; python_version >= "3.8"
 Requires-Dist: redis[hiredis]==5.0.4; python_version >= "3.7"
 Requires-Dist: regex==2023.12.25; python_version >= "3.7"
 Requires-Dist: setproctitle==1.3.3; python_version >= "3.7"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: soupsieve==2.5; python_version >= "3.8"
 Requires-Dist: tornado==6.4; python_version >= "3.8"
 Requires-Dist: typed-stream==0.131.0; python_version >= "3.10"
 Requires-Dist: tzdata==2023.4; python_version >= "2"
 Requires-Dist: ultradict==0.0.6; python_version >= "3.8"
 Requires-Dist: urllib3==2.2.1; python_version >= "3.8"
 Requires-Dist: uvloop==0.19.0; python_full_version >= "3.8.0"
-Requires-Dist: wrapt==1.14.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"
+Requires-Dist: wrapt==1.16.0; python_version >= "3.6"
 Requires-Dist: yarl==1.9.4; python_version >= "3.7"
 
 # Webseite des AN
 
 ![License](https://img.shields.io/pypi/l/an-website?label=License)
 ![Python](https://img.shields.io/pypi/pyversions/an-website?label=Python)
 ![Implementation](https://img.shields.io/pypi/implementation/an-website?label=Implementation)
```

### Comparing `an-website-24.5/README.md` & `an_website-24.6/README.md`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/__init__.py` & `an_website-24.6/an_website/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/__main__.py` & `an_website-24.6/an_website/__main__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/backdoor/__init__.py` & `an_website-24.6/an_website/backdoor/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/backdoor/backdoor.py` & `an_website-24.6/an_website/backdoor/backdoor.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/backdoor/client.py` & `an_website-24.6/an_website/backdoor/client.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/ca-bundle.crt` & `an_website-24.6/an_website/ca-bundle.crt`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/commitment/__init__.py` & `an_website-24.6/an_website/commitment/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/commitment/commitment.py` & `an_website-24.6/an_website/commitment/commitment.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/contact/__init__.py` & `an_website-24.6/an_website/contact/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/contact/contact.py` & `an_website-24.6/an_website/contact/contact.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 import time
 from collections.abc import Iterable, Mapping
 from configparser import ConfigParser
 from datetime import datetime, timezone
 from email import utils as email_utils
 from email.message import Message
 from math import pi
-from typing import Any, Final
+from typing import Any, Final, cast
 from urllib.parse import quote, urlencode
 
+import typed_stream
 from tornado.web import Application, HTTPError, MissingArgumentError
 
 from .. import NAME
 from ..utils.request_handler import HTMLRequestHandler
 from ..utils.utils import ModuleInfo
 
 LOGGER: Final = logging.getLogger(__name__)
@@ -50,14 +51,19 @@
         aliases=("/contact",),
         hidden=True,
     )
 
 
 def apply_contact_stuff_to_app(app: Application, config: ConfigParser) -> None:
     """Apply contact stuff to the app."""
+    if "/kontakt" not in typed_stream.Stream(
+        cast(Iterable[ModuleInfo], app.settings.get("MODULE_INFOS", ()))
+    ).map(lambda m: m.path):
+        return
+
     contact_address = config.get(
         "CONTACT",
         "CONTACT_ADDRESS",
         fallback=(
             f"{NAME.removesuffix('-dev')}@restmail.net"
             if app.settings.get("debug")
             else ""
```

### Comparing `an-website-24.5/an_website/currency_converter/__init__.py` & `an_website-24.6/an_website/currency_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/currency_converter/converter.py` & `an_website-24.6/an_website/currency_converter/converter.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/discord/__init__.py` & `an_website-24.6/an_website/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/discord/discord.py` & `an_website-24.6/an_website/discord/discord.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/LICENSE.txt` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/NOTICE.txt` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/agent.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/agent.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/client.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/client.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/cloud.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/cloud.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/container.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/container.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/data_stream.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/data_stream.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/destination.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/destination.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/dll.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/dll.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/dns.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/dns.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/email.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/email.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/error.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/error.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/event.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/event.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/file.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/file.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/group.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/group.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/host.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/host.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/http.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/http.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/log.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/log.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/network.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/network.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/observer.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/observer.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/orchestrator.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/orchestrator.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/organization.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/organization.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/package.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/package.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/process.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/process.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/registry.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/registry.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/related.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/related.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/rule.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/rule.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/server.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/server.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/service.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/service.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/source.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/source.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/threat.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/threat.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/tls.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/tls.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/tracing.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/tracing.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/url.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/url.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/user.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/user.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/user_agent.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/user_agent.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/component_templates/ecs/vulnerability.json` & `an_website-24.6/an_website/elasticsearch/component_templates/ecs/vulnerability.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/elasticsearch/index_templates/reporting.json` & `an_website-24.6/an_website/elasticsearch/index_templates/reporting.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/element_web_link/__init__.py` & `an_website-24.6/an_website/element_web_link/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/element_web_link/element_web_link.py` & `an_website-24.6/an_website/element_web_link/element_web_link.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/emoji_chat/__init__.py` & `an_website-24.6/an_website/emoji_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/emoji_chat/chat.py` & `an_website-24.6/an_website/emoji_chat/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,15 @@
 import random
 import sys
 import time
 from collections.abc import Awaitable, Iterable, Mapping
 from typing import Any, Final, Literal
 
 import orjson as json
-from emoji import (
-    EMOJI_DATA,
-    demojize,
-    emoji_list,
-    emojize,
-    purely_emoji,
-)
+from emoji import EMOJI_DATA, demojize, emoji_list, emojize, purely_emoji
 from redis.asyncio import Redis
 from tornado.web import HTTPError
 from tornado.websocket import WebSocketHandler
 
 from .. import EPOCH_MS, EVENT_REDIS, ORJSON_OPTIONS
 from ..utils.base_request_handler import BaseRequestHandler
 from ..utils.request_handler import APIRequestHandler, HTMLRequestHandler
@@ -59,16 +53,16 @@
         name="Emoji-Chat",
         description="Ein 🆒er Chat",
         path="/emoji-chat",
         keywords=("Emoji Chat",),
     )
 
 
-MAX_MESSAGE_SAVE_COUNT: Final[Literal[100]] = 100
-MAX_MESSAGE_LENGTH: Final[Literal[20]] = 20
+MAX_MESSAGE_SAVE_COUNT: Final = 100
+MAX_MESSAGE_LENGTH: Final = 20
 
 
 def get_ms_timestamp() -> int:
     """Get the current time in ms."""
     return time.time_ns() // 1_000_000 - EPOCH_MS
 
 
@@ -103,18 +97,19 @@
         ]
     )
 
 
 async def get_messages(
     redis: Redis[str],
     redis_prefix: str,
-    start: int = -MAX_MESSAGE_SAVE_COUNT,
+    start: None | int = None,
     stop: int = -1,
 ) -> list[dict[str, Any]]:
     """Get the messages."""
+    start = start if start is not None else -MAX_MESSAGE_SAVE_COUNT
     messages = await redis.lrange(
         f"{redis_prefix}:emoji-chat:message-list", start, stop
     )
     return [json.loads(message) for message in messages]
 
 
 def check_message_invalid(message: str) -> Literal[False] | str:
```

### Comparing `an-website-24.5/an_website/endpoints/__init__.py` & `an_website-24.6/an_website/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/endpoints/endpoints.py` & `an_website-24.6/an_website/endpoints/endpoints.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/example/__init__.py` & `an_website-24.6/an_website/example/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/example/example.py` & `an_website-24.6/an_website/example/example.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/fake_orjson.py` & `an_website-24.6/an_website/fake_orjson.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/hangman_solver/__init__.py` & `an_website-24.6/an_website/hangman_solver/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/hangman_solver/hangman_solver.py` & `an_website-24.6/an_website/hangman_solver/hangman_solver.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/hangman_solver/wordgame_solver.py` & `an_website-24.6/an_website/hangman_solver/wordgame_solver.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/host_info/__init__.py` & `an_website-24.6/an_website/host_info/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/host_info/host_info.py` & `an_website-24.6/an_website/host_info/host_info.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/js_licenses/__init__.py` & `an_website-24.6/an_website/js_licenses/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/js_licenses/js_licenses.py` & `an_website-24.6/an_website/js_licenses/js_licenses.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/kangaroo_comics/__init__.py` & `an_website-24.6/an_website/kangaroo_comics/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/kangaroo_comics/comics.py` & `an_website-24.6/an_website/kangaroo_comics/comics.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/lolwut/__init__.py` & `an_website-24.6/an_website/lolwut/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/lolwut/lolwut.py` & `an_website-24.6/an_website/lolwut/lolwut.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/main.py` & `an_website-24.6/an_website/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,125 +29,93 @@
 import signal
 import ssl
 import sys
 import threading
 import time
 import types
 import uuid
-from asyncio import AbstractEventLoop
 from asyncio.runners import _cancel_all_tasks  # type: ignore[attr-defined]
 from base64 import b64encode
-from collections.abc import (
-    Callable,
-    Coroutine,
-    Iterable,
-    Mapping,
-    MutableSequence,
-)
+from collections.abc import Callable, Iterable, Mapping, MutableSequence
 from configparser import ConfigParser
 from functools import partial
 from hashlib import sha256
 from multiprocessing.process import _children  # type: ignore[attr-defined]
-from pathlib import Path
 from socket import socket
-from typing import Any, Final, Literal, TypeAlias, TypedDict, TypeGuard, cast
+from typing import Any, Final, TypedDict, TypeGuard, cast
 from warnings import catch_warnings, simplefilter
 from zoneinfo import ZoneInfo
 
-import orjson
 import regex
 from Crypto.Hash import RIPEMD160
 from ecs_logging import StdlibFormatter
 from elastic_enterprise_search import AppSearch  # type: ignore[import-untyped]
-from elastic_transport import ObjectApiResponse
 from elasticapm.contrib.tornado import ElasticAPM
-from elasticsearch import AsyncElasticsearch, NotFoundError
 from redis.asyncio import (
     BlockingConnectionPool,
     Redis,
     SSLConnection,
     UnixDomainSocketConnection,
 )
 from setproctitle import setproctitle
 from tornado.httpserver import HTTPServer
 from tornado.log import LogFormatter
 from tornado.netutil import bind_sockets, bind_unix_socket
 from tornado.process import fork_processes, task_id
 from tornado.web import Application, RedirectHandler
 from typed_stream import Stream
 
-from . import (
-    DIR,
-    EVENT_ELASTICSEARCH,
-    EVENT_REDIS,
-    EVENT_SHUTDOWN,
-    NAME,
-    TEMPLATES_DIR,
-    UPTIME,
-    VERSION,
-)
+from . import DIR, EVENT_SHUTDOWN, NAME, TEMPLATES_DIR, UPTIME, VERSION
 from .contact.contact import apply_contact_stuff_to_app
-from .quotes.utils import (
-    AUTHORS_CACHE,
-    QUOTES_CACHE,
-    WRONG_QUOTES_CACHE,
-    update_cache_periodically,
-)
-from .utils import static_file_handling
+from .utils import background_tasks, static_file_handling
 from .utils.base_request_handler import BaseRequestHandler
 from .utils.better_config_parser import BetterConfigParser
+from .utils.elasticsearch_setup import setup_elasticsearch
 from .utils.logging import WebhookFormatter, WebhookHandler
 from .utils.request_handler import NotFoundHandler
 from .utils.static_file_handling import StaticFileHandler
 from .utils.utils import (
     ArgparseNamespace,
     Handler,
     ModuleInfo,
     Permission,
     Timer,
     create_argument_parser,
     geoip,
     get_arguments_without_help,
-    none_to_default,
     time_function,
 )
 
 try:
     import perf8  # type: ignore[import, unused-ignore]
 except ModuleNotFoundError:
     perf8 = None  # pylint: disable=invalid-name
 
-ES_WHAT_LITERAL: TypeAlias = Literal[  # pylint: disable=invalid-name
-    "component_templates", "index_templates", "ingest_pipelines"
-]
-
 IGNORED_MODULES: Final[set[str]] = {
-    "patches.*",
-    "static.*",
-    "templates.*",
-} | (set() if sys.flags.dev_mode else {"example.*"})
+    "patches",
+    "static",
+    "templates",
+} | (set() if sys.flags.dev_mode else {"example"})
 
 LOGGER: Final = logging.getLogger(__name__)
 
-HEARTBEAT: float = 0
-
 
 # add all the information from the packages to a list
 # this calls the get_module_info function in every file
 # files and dirs starting with '_' get ignored
 def get_module_infos() -> str | tuple[ModuleInfo, ...]:
     """Import the modules and return the loaded module infos in a tuple."""
     module_infos: list[ModuleInfo] = []
     loaded_modules: list[str] = []
     errors: list[str] = []
 
     for potential_module in os.listdir(DIR):
         if (
             potential_module.startswith("_")
-            or f"{potential_module}.*" in IGNORED_MODULES
+            or potential_module in IGNORED_MODULES
             or not os.path.isdir(os.path.join(DIR, potential_module))
         ):
             continue
 
         _module_infos = get_module_infos_from_module(
             potential_module, errors, ignore_not_found=True
         )
@@ -159,14 +127,17 @@
                     "Found module_infos in %s.__init__.py, "
                     "not searching in other modules in the package."
                 ),
                 potential_module,
             )
             continue
 
+        if f"{potential_module}.*" in IGNORED_MODULES:
+            continue
+
         for potential_file in os.listdir(os.path.join(DIR, potential_module)):
             module_name = f"{potential_module}.{potential_file[:-3]}"
             if (
                 not potential_file.endswith(".py")
                 or module_name in IGNORED_MODULES
                 or potential_file.startswith("_")
             ):
@@ -330,15 +301,15 @@
     return handlers
 
 
 def ignore_modules(config: BetterConfigParser) -> None:
     """Read ignored modules from the config."""
     IGNORED_MODULES.update(
         config.getset(
-            "GENERAL", "IGNORED_MODULES", fallback={"element_web_link.*"}
+            "GENERAL", "IGNORED_MODULES", fallback={"element_web_link"}
         )
     )
 
 
 def get_normed_paths_from_module_infos(
     module_infos: Iterable[ModuleInfo],
 ) -> dict[str, str]:
@@ -386,14 +357,18 @@
             "Getting the module infos took %ss. That's probably too long.",
             duration,
         )
     handlers = get_all_handlers(module_infos)
     return Application(
         handlers,  # type: ignore[arg-type]
         MODULE_INFOS=module_infos,
+        SHOW_HAMBURGER_MENU=not Stream(module_infos)
+        .exclude(lambda info: info.hidden)
+        .filter(lambda info: info.path)
+        .empty(),
         NORMED_PATHS=get_normed_paths_from_module_infos(module_infos),
         HANDLERS=handlers,
         # General settings
         autoreload=False,
         debug=sys.flags.dev_mode,
         default_handler_class=NotFoundHandler,
         compress_response=config.getboolean(
@@ -606,15 +581,15 @@
             "WEBHOOK_ESCAPE_MESSAGE",
             fallback=True,
         )
 
 
 def setup_webhook_logging(  # pragma: no cover
     options: WebhookLoggingOptions,
-    loop: AbstractEventLoop,
+    loop: asyncio.AbstractEventLoop,
 ) -> None:
     """Setup Webhook logging."""  # noqa: D401
     if not options.url:
         return
 
     root_logger = logging.getLogger()
 
@@ -741,192 +716,14 @@
     app.settings["APP_SEARCH_HOST"] = host
     app.settings["APP_SEARCH_KEY"] = key
     app.settings["APP_SEARCH_ENGINE"] = config.get(
         "APP_SEARCH", "ENGINE_NAME", fallback=NAME.removesuffix("-dev")
     )
 
 
-def setup_elasticsearch(app: Application) -> None | AsyncElasticsearch:
-    """Setup Elasticsearch."""  # noqa: D401
-    # pylint: disable-next=import-outside-toplevel
-    from elastic_transport.client_utils import DEFAULT, DefaultType
-
-    config: BetterConfigParser = app.settings["CONFIG"]
-    basic_auth: tuple[str | None, str | None] = (
-        config.get("ELASTICSEARCH", "USERNAME", fallback=None),
-        config.get("ELASTICSEARCH", "PASSWORD", fallback=None),
-    )
-
-    class Kwargs(TypedDict):
-        """Kwargs of AsyncElasticsearch constructor."""
-
-        hosts: tuple[str, ...] | None
-        cloud_id: None | str
-        verify_certs: bool
-        api_key: None | str
-        bearer_auth: None | str
-        client_cert: str | DefaultType
-        client_key: str | DefaultType
-        retry_on_timeout: bool | DefaultType
-
-    kwargs: Kwargs = {
-        "hosts": (
-            tuple(config.getset("ELASTICSEARCH", "HOSTS"))
-            if config.has_option("ELASTICSEARCH", "HOSTS")
-            else None
-        ),
-        "cloud_id": config.get("ELASTICSEARCH", "CLOUD_ID", fallback=None),
-        "verify_certs": config.getboolean(
-            "ELASTICSEARCH", "VERIFY_CERTS", fallback=True
-        ),
-        "api_key": config.get("ELASTICSEARCH", "API_KEY", fallback=None),
-        "bearer_auth": config.get(
-            "ELASTICSEARCH", "BEARER_AUTH", fallback=None
-        ),
-        "client_cert": none_to_default(
-            config.get("ELASTICSEARCH", "CLIENT_CERT", fallback=None), DEFAULT
-        ),
-        "client_key": none_to_default(
-            config.get("ELASTICSEARCH", "CLIENT_KEY", fallback=None), DEFAULT
-        ),
-        "retry_on_timeout": none_to_default(
-            config.getboolean(
-                "ELASTICSEARCH", "RETRY_ON_TIMEOUT", fallback=None
-            ),
-            DEFAULT,
-        ),
-    }
-    if not config.getboolean("ELASTICSEARCH", "ENABLED", fallback=False):
-        app.settings["ELASTICSEARCH"] = None
-        return None
-    elasticsearch = AsyncElasticsearch(
-        basic_auth=(
-            None if None in basic_auth else cast(tuple[str, str], basic_auth)
-        ),
-        ca_certs=os.path.join(DIR, "ca-bundle.crt"),
-        **kwargs,
-    )
-    app.settings["ELASTICSEARCH"] = elasticsearch
-    return elasticsearch
-
-
-async def check_elasticsearch(app: Application) -> None:  # pragma: no cover
-    """Check Elasticsearch."""
-    while not EVENT_SHUTDOWN.is_set():  # pylint: disable=while-used
-        es: AsyncElasticsearch = cast(
-            AsyncElasticsearch, app.settings.get("ELASTICSEARCH")
-        )
-        try:
-            await es.transport.perform_request("HEAD", "/")
-        except Exception:  # pylint: disable=broad-except
-            EVENT_ELASTICSEARCH.clear()
-            LOGGER.exception("Connecting to Elasticsearch failed")
-        else:
-            if not EVENT_ELASTICSEARCH.is_set():
-                try:
-                    await setup_elasticsearch_configs(
-                        es, app.settings["ELASTICSEARCH_PREFIX"]
-                    )
-                except Exception:  # pylint: disable=broad-except
-                    LOGGER.exception(
-                        "An exception occured while configuring Elasticsearch"
-                    )
-                else:
-                    EVENT_ELASTICSEARCH.set()
-        await asyncio.sleep(20)
-
-
-async def setup_elasticsearch_configs(
-    elasticsearch: AsyncElasticsearch,
-    prefix: str,
-) -> None:
-    """Setup Elasticsearch configs."""  # noqa: D401
-    spam: list[Coroutine[None, None, None | ObjectApiResponse[Any]]]
-
-    for i in range(3):
-        spam = []
-
-        what = cast(
-            ES_WHAT_LITERAL,
-            ["ingest_pipelines", "component_templates", "index_templates"][i],
-        )
-
-        base_path = Path(os.path.join(DIR, "elasticsearch", what))
-
-        for path in base_path.rglob("*.json"):
-            if not path.is_file():
-                LOGGER.warning("%s is not a file", path)
-                continue
-
-            body = orjson.loads(
-                path.read_bytes().replace(b"{prefix}", prefix.encode("ASCII"))
-            )
-
-            name = f"{prefix}-{str(path.relative_to(base_path))[:-5].replace('/', '-')}"
-
-            spam.append(
-                setup_elasticsearch_config(
-                    elasticsearch, what, body, name, path
-                )
-            )
-
-        await asyncio.gather(*spam)
-
-
-async def setup_elasticsearch_config(
-    es: AsyncElasticsearch,
-    what: ES_WHAT_LITERAL,
-    body: dict[str, Any],
-    name: str,
-    path: str | Path = "<unknown>",
-) -> None | ObjectApiResponse[Any]:
-    """Setup Elasticsearch config."""  # noqa: D401
-    get: Callable[..., Coroutine[None, None, ObjectApiResponse[Any]]]
-    put: Callable[..., Coroutine[None, None, ObjectApiResponse[Any]]]
-
-    if what == "component_templates":
-        get = es.cluster.get_component_template
-        put = es.cluster.put_component_template
-    elif what == "index_templates":
-        get = es.indices.get_index_template
-        put = es.indices.put_index_template
-    elif what == "ingest_pipelines":
-        get = es.ingest.get_pipeline
-        put = es.ingest.put_pipeline
-    else:
-        raise AssertionError()
-
-    try:
-        if what == "ingest_pipelines":
-            current = await get(id=name)
-            current_version = current[name].get("version", 1)
-        else:
-            current = await get(
-                name=name, filter_path=f"{what}.name,{what}.version"
-            )
-            current_version = current[what][0].get("version", 1)
-    except NotFoundError:
-        current_version = 0
-
-    if current_version < body.get("version", 1):
-        if what == "ingest_pipelines":
-            return await put(id=name, body=body)
-        return await put(name=name, body=body)
-
-    if current_version > body.get("version", 1):
-        LOGGER.warning(
-            "%s has version %s. The version in Elasticsearch is %s!",
-            path,
-            body.get("version", 1),
-            current_version,
-        )
-
-    return None
-
-
 def setup_redis(app: Application) -> None | Redis[str]:
     """Setup Redis."""  # noqa: D401
     config: BetterConfigParser = app.settings["CONFIG"]
 
     class Kwargs(TypedDict, total=False):
         """Kwargs of BlockingConnectionPool constructor."""
 
@@ -1006,46 +803,14 @@
         **kwargs,
     )
     redis = cast("Redis[str]", Redis(connection_pool=connection_pool))
     app.settings["REDIS"] = redis
     return redis
 
 
-async def check_redis(app: Application) -> None:  # pragma: no cover
-    """Check Redis."""
-    while not EVENT_SHUTDOWN.is_set():  # pylint: disable=while-used
-        redis: Redis[str] = cast("Redis[str]", app.settings.get("REDIS"))
-        try:
-            await redis.ping()
-        except Exception:  # pylint: disable=broad-except
-            EVENT_REDIS.clear()
-            LOGGER.exception("Connecting to Redis failed")
-        else:
-            EVENT_REDIS.set()
-        await asyncio.sleep(20)
-
-
-async def check_if_ppid_changed(ppid: int) -> bool:
-    """Check whether Technoblade hates us."""
-    while not EVENT_SHUTDOWN.is_set():  # pylint: disable=while-used
-        if os.getppid() != ppid:
-            EVENT_SHUTDOWN.set()
-            return True
-        await asyncio.sleep(1)
-    return False
-
-
-async def wait_for_shutdown() -> None:  # pragma: no cover
-    """Wait for the shutdown event."""
-    loop = asyncio.get_running_loop()
-    while not EVENT_SHUTDOWN.is_set():  # pylint: disable=while-used
-        await asyncio.sleep(0.05)
-    loop.stop()
-
-
 def signal_handler(  # noqa: D103  # pragma: no cover
     signalnum: int, frame: None | types.FrameType
 ) -> None:
     # pylint: disable=unused-argument, missing-function-docstring
     if signalnum in {signal.SIGINT, signal.SIGTERM}:
         EVENT_SHUTDOWN.set()
     if signalnum == getattr(signal, "SIGHUP", None):
@@ -1056,25 +821,17 @@
     """Install the signal handler."""
     signal.signal(signal.SIGINT, signal_handler)
     signal.signal(signal.SIGTERM, signal_handler)
     if hasattr(signal, "SIGHUP"):
         signal.signal(signal.SIGHUP, signal_handler)
 
 
-async def heartbeat() -> None:
-    """Heartbeat."""
-    global HEARTBEAT  # pylint: disable=global-statement
-    while HEARTBEAT:  # pylint: disable=while-used
-        HEARTBEAT = time.monotonic()
-        await asyncio.sleep(0.05)
-
-
 def supervise() -> None:
     """Supervise."""
-    while foobarbaz := HEARTBEAT:  # pylint: disable=while-used
+    while foobarbaz := background_tasks.HEARTBEAT:  # pylint: disable=while-used
         if time.monotonic() - foobarbaz >= 10:
             worker = task_id()
             pid = os.getpid()
             LOGGER.fatal(
                 "Heartbeat timed out for worker %d (pid %d)", worker, pid
             )
             atexit._run_exitfuncs()  # pylint: disable=protected-access
@@ -1088,16 +845,14 @@
     """
     Start everything.
 
     This is the main function that is called when running this programm.
     """
     # pylint: disable=too-complex, too-many-branches
     # pylint: disable=too-many-locals, too-many-statements
-    global HEARTBEAT  # pylint: disable=global-statement
-
     setproctitle(NAME)
 
     install_signal_handler()
 
     parser = create_argument_parser()
     args, _ = parser.parse_known_args(
         get_arguments_without_help(), ArgparseNamespace()
@@ -1219,30 +974,37 @@
         worker = fork_processes(processes)
 
         setproctitle(f"{NAME} - Worker {worker}")
 
         # yeet all children (there should be none, but do it regardless, just in case)
         _children.clear()
 
-        del AUTHORS_CACHE.control.created_by_ultra  # type: ignore[attr-defined]
-        del QUOTES_CACHE.control.created_by_ultra  # type: ignore[attr-defined]
-        del WRONG_QUOTES_CACHE.control.created_by_ultra  # type: ignore[attr-defined]
+        if "an_website.quotes" in sys.modules:
+            from .quotes.utils import (  # pylint: disable=import-outside-toplevel
+                AUTHORS_CACHE,
+                QUOTES_CACHE,
+                WRONG_QUOTES_CACHE,
+            )
+
+            del AUTHORS_CACHE.control.created_by_ultra  # type: ignore[attr-defined]
+            del QUOTES_CACHE.control.created_by_ultra  # type: ignore[attr-defined]
+            del WRONG_QUOTES_CACHE.control.created_by_ultra  # type: ignore[attr-defined]
         del geoip.__kwdefaults__["caches"].control.created_by_ultra
 
         if unix_socket_path:
             sockets.append(
                 bind_unix_socket(
                     os.path.join(unix_socket_path, f"{NAME}.{worker}.sock"),
                     mode=0o666,
                 )
             )
 
     # get loop after forking
     # if not forking allow loop to be set in advance by external code
-    loop: None | AbstractEventLoop
+    loop: None | asyncio.AbstractEventLoop
     try:
         with catch_warnings():  # TODO: remove after dropping support for 3.13
             simplefilter("ignore", DeprecationWarning)
             loop = asyncio.get_event_loop()
         if loop.is_closed():
             loop = None
     except RuntimeError:
@@ -1258,40 +1020,28 @@
     if perf8 and "PERF8" in os.environ:
         loop.run_until_complete(perf8.enable())
 
     setup_webhook_logging(webhook_logging_options, loop)
 
     server.add_sockets(sockets)
 
-    # pylint: disable=unused-variable
-
-    task_heartbeat = loop.create_task(heartbeat())  # noqa: F841
-
-    task_shutdown = loop.create_task(wait_for_shutdown())  # noqa: F841
-
-    if elasticsearch_is_enabled:
-        task_es = loop.create_task(check_elasticsearch(app))  # noqa: F841
-
-    if redis_is_enabled:
-        task_redis = loop.create_task(check_redis(app))  # noqa: F841
-
-    if not worker:  # update from one process only
-        task_quotes = loop.create_task(  # noqa: F841
-            update_cache_periodically(app)
-        )
-
-    if processes:
-        task_check_parent = loop.create_task(  # noqa: F841
-            check_if_ppid_changed(main_pid)
-        )
-
-    # pylint: enable=unused-variable
+    # pylint: disable-next=unused-variable
+    tasks = background_tasks.start_background_tasks(  # noqa: F841
+        module_infos=app.settings["MODULE_INFOS"],
+        loop=loop,
+        main_pid=main_pid,
+        app=app,
+        processes=processes,
+        elasticsearch_is_enabled=elasticsearch_is_enabled,
+        redis_is_enabled=redis_is_enabled,
+        worker=worker,
+    )
 
     if run_supervisor_thread:
-        HEARTBEAT = time.monotonic()
+        background_tasks.HEARTBEAT = time.monotonic()
         threading.Thread(
             target=supervise, name="supervisor", daemon=True
         ).start()
 
     try:
         loop.run_forever()
         EVENT_SHUTDOWN.set()
@@ -1309,10 +1059,10 @@
         finally:
             try:
                 _cancel_all_tasks(loop)
                 loop.run_until_complete(loop.shutdown_asyncgens())
                 loop.run_until_complete(loop.shutdown_default_executor())
             finally:
                 loop.close()
-                HEARTBEAT = 0
+                background_tasks.HEARTBEAT = 0
 
     return 0
```

### Comparing `an-website-24.5/an_website/main_page/__init__.py` & `an_website-24.6/an_website/main_page/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/main_page/main_page.py` & `an_website-24.6/an_website/main_page/main_page.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/patches/__init__.py` & `an_website-24.6/an_website/patches/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 """Patches that improve everything."""
 
 from __future__ import annotations
 
 import http.client
 import json as stdlib_json  # pylint: disable=preferred-module
+import logging
 import os
 import sys
 from collections.abc import Callable
 from configparser import RawConfigParser
 from contextlib import suppress
 from importlib import import_module
 from os.path import abspath, dirname
@@ -327,14 +328,18 @@
 
     def redirect(
         self: RequestHandler,
         url: str,
         permanent: bool = False,
         status: None | int = None,
     ) -> None:
+        if url == self.request.full_url():
+            logging.getLogger(
+                f"{self.__class__.__module__}.{self.__class__.__qualname__}"
+            ).critical("Infinite redirect to %r detected", url)
         if self._headers_written:
             # pylint: disable=broad-exception-raised
             raise Exception("Cannot redirect after headers have been written")
         if status is None:
             status = 308 if permanent else 307
         else:
             assert isinstance(status, int) and 300 <= status <= 399  # type: ignore[redundant-expr]  # noqa: B950
```

### Comparing `an-website-24.5/an_website/patches/braille.py` & `an_website-24.6/an_website/patches/braille.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/patches/json.py` & `an_website-24.6/an_website/patches/json.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/ping/__init__.py` & `an_website-24.6/an_website/ping/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/ping/ping.py` & `an_website-24.6/an_website/ping/ping.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/primes.bin` & `an_website-24.6/an_website/primes.bin`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/quotes/__init__.py` & `an_website-24.6/an_website/quotes/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from .quote_of_the_day import (
     QuoteOfTheDayAPI,
     QuoteOfTheDayRedirect,
     QuoteOfTheDayRSS,
 )
 from .quotes import QuoteAPIHandler, QuoteById, QuoteMainPage, QuoteRedirectAPI
 from .share import ShareQuote
+from .utils import update_cache_periodically
 
 DIR: Final = abspath(dirname(__file__))
 
 
 def get_module_info() -> ModuleInfo:
     """Create and return the ModuleInfo for this module."""
     return ModuleInfo(
@@ -160,8 +161,9 @@
             "Zitate",
             "Witzig",
             "Känguru",
             "Marc-Uwe Kling",
             "falsche Zitate",
             "falsch zugeordnete Zitate",
         ),
+        required_background_tasks=frozenset({update_cache_periodically}),
     )
```

### Comparing `an-website-24.5/an_website/quotes/create.py` & `an_website-24.6/an_website/quotes/create.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/quotes/edit.sh` & `an_website-24.6/an_website/quotes/edit.sh`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/quotes/files/StempelNichtWitzig.png` & `an_website-24.6/an_website/quotes/files/StempelNichtWitzig.png`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/quotes/files/StempelWitzig.png` & `an_website-24.6/an_website/quotes/files/StempelWitzig.png`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/quotes/files/bg.png` & `an_website-24.6/an_website/quotes/files/bg.png`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/quotes/files/oswald.regular.ttf` & `an_website-24.6/an_website/quotes/files/oswald.regular.ttf`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/quotes/generator.py` & `an_website-24.6/an_website/quotes/generator.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/quotes/image.py` & `an_website-24.6/an_website/quotes/image.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/quotes/info.py` & `an_website-24.6/an_website/quotes/info.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/quotes/quote_of_the_day/__init__.py` & `an_website-24.6/an_website/quotes/quote_of_the_day/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/quotes/quote_of_the_day/data.py` & `an_website-24.6/an_website/quotes/quote_of_the_day/data.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/quotes/quote_of_the_day/store.py` & `an_website-24.6/an_website/quotes/quote_of_the_day/store.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/quotes/quotes.py` & `an_website-24.6/an_website/quotes/quotes.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/quotes/share.py` & `an_website-24.6/an_website/quotes/share.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/quotes/utils.py` & `an_website-24.6/an_website/quotes/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,29 +28,30 @@
 from datetime import date, datetime, timezone
 from multiprocessing import Value
 from typing import Any, Final, Literal, cast
 from urllib.parse import urlencode
 
 import elasticapm
 import orjson as json
+import typed_stream
 from redis.asyncio import Redis
 from tornado.httpclient import AsyncHTTPClient
 from tornado.web import Application, HTTPError
 from UltraDict import UltraDict  # type: ignore[import-untyped]
 
 from .. import DIR as ROOT_DIR
 from .. import (
     EVENT_REDIS,
     EVENT_SHUTDOWN,
     NAME,
     ORJSON_OPTIONS,
     pytest_is_running,
 )
 from ..utils.request_handler import HTMLRequestHandler
-from ..utils.utils import Permission, emojify, ratelimit
+from ..utils.utils import ModuleInfo, Permission, emojify, ratelimit
 
 DIR: Final = os.path.dirname(__file__)
 
 LOGGER: Final = logging.getLogger(__name__)
 
 API_URL: Final[str] = "https://zitate.prapsschnalinen.de/api"
 
@@ -400,17 +401,15 @@
     if not name:
         name = "None"
 
     author = AUTHORS_CACHE.get(author_id)
     if author is None:  # author not in cache, create new one
         # pylint: disable=too-many-function-args
         author = Author(author_id, name, None)
-        MAX_AUTHORS_ID.value = max(
-            MAX_AUTHORS_ID.value, author_id
-        )
+        MAX_AUTHORS_ID.value = max(MAX_AUTHORS_ID.value, author_id)
     else:  # update to make sure cache is correct
         author.update_name(name)
 
     AUTHORS_CACHE[author.id] = author
 
     return author
 
@@ -442,17 +441,15 @@
     quote_str = fix_quote_str(json_data["quote"])
 
     if quote is None:  # no quote supplied, try getting it from cache
         quote = QUOTES_CACHE.get(quote_id)
     if quote is None:  # new quote
         # pylint: disable=too-many-function-args
         quote = Quote(quote_id, quote_str, author)
-        MAX_QUOTES_ID.value = max(
-            MAX_QUOTES_ID.value, quote.id
-        )
+        MAX_QUOTES_ID.value = max(MAX_QUOTES_ID.value, quote.id)
     else:  # quote was already saved
         quote.update_quote(quote_str, author.id, author.name)
 
     QUOTES_CACHE[quote.id] = quote
 
     return quote
 
@@ -509,17 +506,25 @@
     for json_data in json_list:
         _ = parse_fun(json_data)
         await asyncio.sleep(0)
         return_list.append(_)
     return tuple(return_list)
 
 
-async def update_cache_periodically(app: Application) -> None:
+async def update_cache_periodically(
+    app: Application, worker: int | None
+) -> None:
     """Start updating the cache every hour."""
     # pylint: disable=too-complex
+    if "/troet" in typed_stream.Stream(
+        cast(Iterable[ModuleInfo], app.settings.get("MODULE_INFOS", ()))
+    ).map(lambda m: m.path):
+        app.settings["SHOW_SHARING_ON_MASTODON"] = True
+    if worker:
+        return
     with contextlib.suppress(asyncio.TimeoutError):
         await asyncio.wait_for(EVENT_REDIS.wait(), 5)
     redis: Redis[str] = cast("Redis[str]", app.settings.get("REDIS"))
     prefix: str = app.settings.get("REDIS_PREFIX", NAME).removesuffix("-dev")
     apm: None | elasticapm.Client
     if EVENT_REDIS.is_set():  # pylint: disable=too-many-nested-blocks
         await parse_list_of_quote_data(
@@ -710,24 +715,20 @@
 async def get_rating_by_id(quote_id: int, author_id: int) -> int:
     """Get the rating of a wrong quote."""
     return (await get_wrong_quote(quote_id, author_id)).rating
 
 
 def get_random_quote_id() -> int:
     """Get random quote id."""
-    return random.randint(  # nosec: B311
-        1, MAX_QUOTES_ID.value
-    )
+    return random.randint(1, MAX_QUOTES_ID.value)  # nosec: B311
 
 
 def get_random_author_id() -> int:
     """Get random author id."""
-    return random.randint(  # nosec: B311
-        1, MAX_AUTHORS_ID.value
-    )
+    return random.randint(1, MAX_AUTHORS_ID.value)  # nosec: B311
 
 
 def get_random_id() -> tuple[int, int]:
     """Get random wrong quote id."""
     return (
         get_random_quote_id(),
         get_random_author_id(),
```

### Comparing `an-website-24.5/an_website/random_text/__init__.py` & `an_website-24.6/an_website/random_text/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/random_text/random_text.py` & `an_website-24.6/an_website/random_text/random_text.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/random_text/words.txt` & `an_website-24.6/an_website/random_text/words.txt`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/redirect/__init__.py` & `an_website-24.6/an_website/redirect/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/redirect/redirect.py` & `an_website-24.6/an_website/redirect/redirect.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 This page will ask users if they want to leave this website.
 """
 
 from __future__ import annotations
 
 from urllib.parse import urlsplit
 
+from tornado.web import Application
+
 from .. import pytest_is_running
 from ..utils.request_handler import HTMLRequestHandler
 from ..utils.utils import ModuleInfo
 
 
 def get_module_info() -> ModuleInfo:
     """Create and return the ModuleInfo for this module."""
@@ -35,17 +37,23 @@
         description=(
             "Seite, die User davon abhält versehentlich eine fremde "
             "Webseite zu besuchen"
         ),
         path="/redirect",
         short_name="Weiterleitung",
         hidden=True,
+        required_background_tasks=(_confirm_loading,),
     )
 
 
+async def _confirm_loading(app: Application, worker: int | None) -> None:
+    """Save in settings that the redirect module has been loaded."""
+    app.settings["REDIRECT_MODULE_LOADED"] = worker or True  # noqa: SIM222
+
+
 class RedirectPage(HTMLRequestHandler):
     """The redirect page that redirects you to another page."""
 
     async def get(self, *, head: bool = False) -> None:
         """Handle GET requests to the redirect page."""
         # pylint: disable=unused-argument
```

### Comparing `an-website-24.5/an_website/reporting/__init__.py` & `an_website-24.6/an_website/reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/reporting/reporting.py` & `an_website-24.6/an_website/reporting/reporting.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/search/__init__.py` & `an_website-24.6/an_website/search/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/search/search.py` & `an_website-24.6/an_website/search/search.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/services/__init__.py` & `an_website-24.6/an_website/services/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/services/services.py` & `an_website-24.6/an_website/services/services.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/settings/__init__.py` & `an_website-24.6/an_website/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/settings/settings.py` & `an_website-24.6/an_website/settings/settings.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/snow/LICENSE` & `an_website-24.6/an_website/snow/LICENSE`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/__init__.py` & `an_website-24.6/an_website/soundboard/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/data.py` & `an_website-24.6/an_website/soundboard/data.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/dietmar-ich_hab_seine_hausaufgaben_aufgegessen.mp3` & `an_website-24.6/an_website/soundboard/files/dietmar-ich_hab_seine_hausaufgaben_aufgegessen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/fw-ihr_linken_intellektuellen_fuzzies.mp3` & `an_website-24.6/an_website/soundboard/files/fw-ihr_linken_intellektuellen_fuzzies.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/gott-das_ist_privat.mp3` & `an_website-24.6/an_website/soundboard/files/gott-das_ist_privat.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/gott-so_so_du_hast_also_keine_eier.mp3` & `an_website-24.6/an_website/soundboard/files/gott-so_so_du_hast_also_keine_eier.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/jesus-guck_mal_was_ich_kann.mp3` & `an_website-24.6/an_website/soundboard/files/jesus-guck_mal_was_ich_kann.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-aber_nicht_zu_lidl.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-aber_nicht_zu_lidl.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-alles_kapitalismus_alles_nestle_alles_haehnchen.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-alles_kapitalismus_alles_nestle_alles_haehnchen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-das_ist_freiwillig.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-das_ist_freiwillig.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-finsterstes_mittelalter_alter.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-finsterstes_mittelalter_alter.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-hallo.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-hallo.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-hier_sind_wir_jetzt_unterhalte_uns.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-hier_sind_wir_jetzt_unterhalte_uns.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-i_love_it.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-i_love_it.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-ich_bin_kommunist.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-ich_bin_kommunist.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-ich_darf_nich_und_ich_will_nich.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-ich_darf_nich_und_ich_will_nich.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-im_so_happy_for_no_reason_but_i_dont_care.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-im_so_happy_for_no_reason_but_i_dont_care.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-ja_ja.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-ja_ja.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-kein_problem_ich_hab_zeit.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-kein_problem_ich_hab_zeit.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-koestlich.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-koestlich.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-man_darf_nie_aufhoeren_alles_kritisch_zu_hinterfragen.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-man_darf_nie_aufhoeren_alles_kritisch_zu_hinterfragen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-ohh_hee.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-ohh_hee.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-this_kinda_feels_really_really_awesome.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-this_kinda_feels_really_really_awesome.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-wir_kaempfen_fuer_eine_gerechte_weltordnung_brot_fuer_alle_und_die_aechtung_von_sogennanntem_musikfernsehen.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-wir_kaempfen_fuer_eine_gerechte_weltordnung_brot_fuer_alle_und_die_aechtung_von_sogennanntem_musikfernsehen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-wir_sind_keine_intellektuellen.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-wir_sind_keine_intellektuellen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kaenguru-wolln_wir_uns_dutzen.mp3` & `an_website-24.6/an_website/soundboard/files/kaenguru-wolln_wir_uns_dutzen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/kuh-ahamumumu.mp3` & `an_website-24.6/an_website/soundboard/files/kuh-ahamumumu.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/muk-du_bist_also_teil_der_juedisch-bolschewistischen_weltverschwoerung.mp3` & `an_website-24.6/an_website/soundboard/files/muk-du_bist_also_teil_der_juedisch-bolschewistischen_weltverschwoerung.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/muk-fuer_nichts_und_wieder_nichts.mp3` & `an_website-24.6/an_website/soundboard/files/muk-fuer_nichts_und_wieder_nichts.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/muk-i_am_bored.mp3` & `an_website-24.6/an_website/soundboard/files/muk-i_am_bored.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/muk-i_am_bored_in_the_usa.mp3` & `an_website-24.6/an_website/soundboard/files/muk-i_am_bored_in_the_usa.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/muk-im_just_here_for_the_famous_breakfast.mp3` & `an_website-24.6/an_website/soundboard/files/muk-im_just_here_for_the_famous_breakfast.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/muk-ja_herzlich_willkommen.mp3` & `an_website-24.6/an_website/soundboard/files/muk-ja_herzlich_willkommen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/muk-sprich_bitte_nur_fuer_dich.mp3` & `an_website-24.6/an_website/soundboard/files/muk-sprich_bitte_nur_fuer_dich.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/muk-ueber_mich_hat_die_zeit_geschrieben_dass_ich_der_wahrscheinlich_einflussreichste_linke_interlektulelle_deutschlands_sei.mp3` & `an_website-24.6/an_website/soundboard/files/muk-ueber_mich_hat_die_zeit_geschrieben_dass_ich_der_wahrscheinlich_einflussreichste_linke_interlektulelle_deutschlands_sei.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/muk-und_da_ist_mir_aufgefallen_dass_ich_keine_eier_hab.mp3` & `an_website-24.6/an_website/soundboard/files/muk-und_da_ist_mir_aufgefallen_dass_ich_keine_eier_hab.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/muk-und_mich_dann_auch_noch_beschneiden_lassen.mp3` & `an_website-24.6/an_website/soundboard/files/muk-und_mich_dann_auch_noch_beschneiden_lassen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/muk-von_mir_aus.mp3` & `an_website-24.6/an_website/soundboard/files/muk-von_mir_aus.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/muk-yeah.mp3` & `an_website-24.6/an_website/soundboard/files/muk-yeah.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/psychiater-aha.mp3` & `an_website-24.6/an_website/soundboard/files/psychiater-aha.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/sarah-hey_thats_cool.mp3` & `an_website-24.6/an_website/soundboard/files/sarah-hey_thats_cool.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/sarah-i_love_life.mp3` & `an_website-24.6/an_website/soundboard/files/sarah-i_love_life.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/sarah-thats_amazing_its_like_you_know_i_dont_know_kind_of_like_whatever_and_stuff.mp3` & `an_website-24.6/an_website/soundboard/files/sarah-thats_amazing_its_like_you_know_i_dont_know_kind_of_like_whatever_and_stuff.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/sarah-the_world_is_so_beautiful.mp3` & `an_website-24.6/an_website/soundboard/files/sarah-the_world_is_so_beautiful.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/sarah-well_thats_just_like_you_know_amazing.mp3` & `an_website-24.6/an_website/soundboard/files/sarah-well_thats_just_like_you_know_amazing.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/files/sarah-yes_its_just_perfect.mp3` & `an_website-24.6/an_website/soundboard/files/sarah-yes_its_just_perfect.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/icon.svg` & `an_website-24.6/an_website/soundboard/icon.svg`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/info.json` & `an_website-24.6/an_website/soundboard/info.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/soundboard/soundboard.py` & `an_website-24.6/an_website/soundboard/soundboard.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/base.css` & `an_website-24.6/an_website/static/css/base.css`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/base.css.map` & `an_website-24.6/an_website/static/css/base.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/comic.css.map` & `an_website-24.6/an_website/static/css/comic.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/emoji_chat.css.map` & `an_website-24.6/an_website/static/css/emoji_chat.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/form.css` & `an_website-24.6/an_website/static/css/form.css`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/form.css.map` & `an_website-24.6/an_website/static/css/form.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/kangaroo_comics.css` & `an_website-24.6/an_website/static/css/kangaroo_comics.css`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/kangaroo_comics.css.map` & `an_website-24.6/an_website/static/css/kangaroo_comics.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/quotes/generator.css.map` & `an_website-24.6/an_website/static/css/quotes/generator.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/quotes/info.css` & `an_website-24.6/an_website/static/css/quotes/info.css`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/quotes/info.css.map` & `an_website-24.6/an_website/static/css/quotes/info.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/quotes/quotes.css` & `an_website-24.6/an_website/static/css/quotes/quotes.css`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/quotes/quotes.css.map` & `an_website-24.6/an_website/static/css/quotes/quotes.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/quotes/share.css` & `an_website-24.6/an_website/static/css/quotes/share.css`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/quotes/share.css.map` & `an_website-24.6/an_website/static/css/quotes/share.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/redirect.css.map` & `an_website-24.6/an_website/static/css/redirect.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/snow.css` & `an_website-24.6/an_website/static/css/snow.css`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/snow.css.map` & `an_website-24.6/an_website/static/css/snow.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/soundboard.css.map` & `an_website-24.6/an_website/static/css/soundboard.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/table.css.map` & `an_website-24.6/an_website/static/css/table.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/themes/blue.css.map` & `an_website-24.6/an_website/static/css/themes/blue.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/themes/christmas.css` & `an_website-24.6/an_website/static/css/themes/christmas.css`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/themes/christmas.css.map` & `an_website-24.6/an_website/static/css/themes/christmas.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/themes/default.css.map` & `an_website-24.6/an_website/static/css/themes/default.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/themes/fun.css.map` & `an_website-24.6/an_website/static/css/themes/fun.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/themes/green.css.map` & `an_website-24.6/an_website/static/css/themes/green.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/themes/light.css.map` & `an_website-24.6/an_website/static/css/themes/light.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/themes/light_blue.css.map` & `an_website-24.6/an_website/static/css/themes/light_blue.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/themes/orange.css.map` & `an_website-24.6/an_website/static/css/themes/orange.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/themes/pink.css.map` & `an_website-24.6/an_website/static/css/themes/pink.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/themes/purple.css.map` & `an_website-24.6/an_website/static/css/themes/purple.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/themes/yellow.css.map` & `an_website-24.6/an_website/static/css/themes/yellow.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/css/uptime.css.map` & `an_website-24.6/an_website/static/css/uptime.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/favicon.jxl` & `an_website-24.6/an_website/static/favicon.jxl`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/favicon.png` & `an_website-24.6/an_website/static/favicon.png`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/fonts/NOTICE.txt` & `an_website-24.6/an_website/static/fonts/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/fonts/comic.woff2` & `an_website-24.6/an_website/static/fonts/comic.woff2`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/fonts/comicmono.woff2` & `an_website-24.6/an_website/static/fonts/comicmono.woff2`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/fonts/cursedtimerulil-aznm.woff2` & `an_website-24.6/an_website/static/fonts/cursedtimerulil-aznm.woff2`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/img/2020-11-03.jpg` & `an_website-24.6/an_website/static/img/2020-11-03.jpg`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/img/NOTICE.txt` & `an_website-24.6/an_website/static/img/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/img/kangarooface.svg` & `an_website-24.6/an_website/static/img/kangarooface.svg`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/img/logo.svg` & `an_website-24.6/an_website/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/img/netcup-oekostrom2.jxl` & `an_website-24.6/an_website/static/img/netcup-oekostrom2.jxl`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/img/netcup-oekostrom2.png` & `an_website-24.6/an_website/static/img/netcup-oekostrom2.png`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/img/rss.svg` & `an_website-24.6/an_website/static/img/rss.svg`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/img/save.svg` & `an_website-24.6/an_website/static/img/save.svg`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/img/stamps/nichtwitzig.small.svg` & `an_website-24.6/an_website/static/img/stamps/nichtwitzig.small.svg`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/img/stamps/witzig.small.svg` & `an_website-24.6/an_website/static/img/stamps/witzig.small.svg`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/currency_converter/converter.js` & `an_website-24.6/an_website/static/js/currency_converter/converter.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/currency_converter/converter.js.map` & `an_website-24.6/an_website/static/js/currency_converter/converter.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/emoji_chat/chat.js` & `an_website-24.6/an_website/static/js/emoji_chat/chat.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/emoji_chat/chat.js.map` & `an_website-24.6/an_website/static/js/emoji_chat/chat.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/hangman_solver/hangman_solver.js` & `an_website-24.6/an_website/static/js/hangman_solver/hangman_solver.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/hangman_solver/hangman_solver.js.map` & `an_website-24.6/an_website/static/js/hangman_solver/hangman_solver.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/kangaroo_comics/comics.js` & `an_website-24.6/an_website/static/js/kangaroo_comics/comics.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/kangaroo_comics/comics.js.map` & `an_website-24.6/an_website/static/js/kangaroo_comics/comics.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/quotes/create.js.map` & `an_website-24.6/an_website/static/js/quotes/create.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/quotes/quotes.js` & `an_website-24.6/an_website/static/js/quotes/quotes.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/quotes/quotes.js.map` & `an_website-24.6/an_website/static/js/quotes/quotes.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/search/search.js` & `an_website-24.6/an_website/static/js/search/search.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/search/search.js.map` & `an_website-24.6/an_website/static/js/search/search.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/settings/settings.js` & `an_website-24.6/an_website/static/js/settings/settings.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/settings/settings.js.map` & `an_website-24.6/an_website/static/js/settings/settings.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/snow/snow.js` & `an_website-24.6/an_website/static/js/snow/snow.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/snow/snow.js.map` & `an_website-24.6/an_website/static/js/snow/snow.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/swapped_words/swap.js` & `an_website-24.6/an_website/static/js/swapped_words/swap.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/swapped_words/swap.js.map` & `an_website-24.6/an_website/static/js/swapped_words/swap.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/uptime/uptime.js` & `an_website-24.6/an_website/static/js/uptime/uptime.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/uptime/uptime.js.map` & `an_website-24.6/an_website/static/js/uptime/uptime.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/utils/better_ui.js` & `an_website-24.6/an_website/static/js/utils/better_ui.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/utils/better_ui.js.map` & `an_website-24.6/an_website/static/js/utils/better_ui.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/utils/dynload.js` & `an_website-24.6/an_website/static/js/utils/dynload.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/utils/dynload.js.map` & `an_website-24.6/an_website/static/js/utils/dynload.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/utils/utils.js` & `an_website-24.6/an_website/static/js/utils/utils.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/utils/utils.js.map` & `an_website-24.6/an_website/static/js/utils/utils.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/vendored/vanilla.js` & `an_website-24.6/an_website/static/js/vendored/vanilla.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/static/js/vendored/vanilla.js.map` & `an_website-24.6/an_website/static/js/vendored/vanilla.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/swapped_words/__init__.py` & `an_website-24.6/an_website/swapped_words/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/swapped_words/config.sw` & `an_website-24.6/an_website/swapped_words/config.sw`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/swapped_words/config_file.py` & `an_website-24.6/an_website/swapped_words/config_file.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/swapped_words/swap.py` & `an_website-24.6/an_website/swapped_words/swap.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/ansi2html.html` & `an_website-24.6/an_website/templates/ansi2html.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/base.html` & `an_website-24.6/an_website/templates/base.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/error.html` & `an_website-24.6/an_website/templates/error.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/footer.html` & `an_website-24.6/an_website/templates/footer.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/header.html` & `an_website-24.6/an_website/templates/header.html`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,16 @@
            href="{{fix_url('/')}}"
            class="no-style-a-emoji"
            id="back-to-home">
             <img src="{{fix_static('img/logo.svg')}}" alt="Zurück zur Startseite">
         </a>
         <h1 id="title" short_title="{{short_title}}">{{title}}</h1>
     </section>
-    {% if settings %}
+    {# NETCUP won't be shown if SHOW_HAMBURGER_MENU is False (that looks ugly) #}
+    {% if settings and settings.get("SHOW_HAMBURGER_MENU") %}
         <img id="open-pane"
              src="{{fix_static('img/hamburger-menu-icon.svg')}}"
              alt="Menü">
         <nav id="site-pane" tabindex="-1">
             <h2 data-elastic-exclude>Unterseiten:</h2>
             <ul class="list">
                 {% for i, info in enumerate(settings.get("MODULE_INFOS")) %}
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 _[_Z_u_r_Ã_¼_c_k_ _z_u_r_ _S_t_a_r_t_s_e_i_t_e_]
 ************ {{{{ttiittllee}}}} ************
-{% if settings %}[MenÃ¼]
+{# NETCUP won't be shown if SHOW_HAMBURGER_MENU is False (that looks ugly) #}
+{% if settings and settings.get("SHOW_HAMBURGER_MENU") %}[MenÃ¼]
 ********** UUnntteerrsseeiitteenn:: **********
     * {% for i, info in enumerate(settings.get("MODULE_INFOS")) %} {% if not
       info.hidden and info.path %}
     * % if i < 6 %} tooltip-position="bottom" {% end %} {% if info.path == "/
       js-lizenzen/" %} data-jslicense="1" {% end %} >{{info.name}}
  {% if info.sub_pages %}
     * {% for page_info in info.sub_pages %} {% if not page_info.hidden and
```

### Comparing `an-website-24.5/an_website/templates/pages/contact.html` & `an_website-24.6/an_website/templates/pages/contact.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/converter.html` & `an_website-24.6/an_website/templates/pages/converter.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/emoji_chat.html` & `an_website-24.6/an_website/templates/pages/emoji_chat.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/endpoints.html` & `an_website-24.6/an_website/templates/pages/endpoints.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/hangman_solver.html` & `an_website-24.6/an_website/templates/pages/hangman_solver.html`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         <input type="submit"
                id="submit"
                value="Eingabe">
     </form>
 
     <div id="letter-frequency-information">
-        {% if hangman_result.letter_frequency %}
+        {% if hangman_result.matching_words_count > 0 %}
             Mögliche Buchstaben:
             {{ ", ".join([f"{char}: {count}" for char, count in hangman_result.letter_frequency]) }}
         {% else %}Nichts gefunden.{% end %}
     </div>
 
     <div id="matching-words">
         {% if hangman_result.matching_words_count > 0 %}
```

#### html2text {}

```diff
@@ -12,17 +12,17 @@
 % if hangman_result.language.value == "de_basic" %} selected {% end %}
 value="de_basic">Deutsch (Grundformen) ohne Umlaute
 % if hangman_result.language.value == "de_basic" %} selected {% end %}
 value="de_basic_umlauts">Deutsch (Grundformen)
 % if hangman_result.language.value == "en" %} selected {% end %}
 value="en">Englisch
 {% raw form_appendix %}[Eingabe]
-{% if hangman_result.letter_frequency %} MÃ¶gliche Buchstaben: {{ ", ".join([f"
-{char}: {count}" for char, count in hangman_result.letter_frequency]) }} {%
-else %}Nichts gefunden.{% end %}
+{% if hangman_result.matching_words_count > 0 %} MÃ¶gliche Buchstaben: {{ ",
+".join([f"{char}: {count}" for char, count in hangman_result.letter_frequency])
+}} {% else %}Nichts gefunden.{% end %}
 {% if hangman_result.matching_words_count > 0 %} {{min
 (hangman_result.matching_words_count, data.get_max_words())}}/{
 {hangman_result.matching_words_count}} passenden WÃ¶rter:
     * {% for word in hangman_result.words %}
     * {{word}}
     * {% end %}
 {% end %}
```

### Comparing `an-website-24.5/an_website/templates/pages/js_licenses.html` & `an_website-24.6/an_website/templates/pages/js_licenses.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/kangaroo_comics.html` & `an_website-24.6/an_website/templates/pages/kangaroo_comics.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/main_page.html` & `an_website-24.6/an_website/templates/pages/main_page.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/quotes/create1.html` & `an_website-24.6/an_website/templates/pages/quotes/create1.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/quotes/create2.html` & `an_website-24.6/an_website/templates/pages/quotes/create2.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/quotes/generator.html` & `an_website-24.6/an_website/templates/pages/quotes/generator.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/quotes/info.html` & `an_website-24.6/an_website/templates/pages/quotes/info.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/quotes/main_page.html` & `an_website-24.6/an_website/templates/pages/quotes/main_page.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/quotes/quotes.html` & `an_website-24.6/an_website/templates/pages/quotes/quotes.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/quotes/share.html` & `an_website-24.6/an_website/templates/pages/quotes/share.html`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,25 @@
           href="{{fix_static('css/quotes/share.css')}}">
 {% end %}
 
 {% block body %}
   {{wrong_quote}}<br>
   {% comment Initially generated using https://sharingbuttons.io since then improved. %}
   <div>
-    <a id="mastodon"
-       href="{{fix_url('/troet', save='sure', text=f'{u_text}\n\n{u_url}\n\n#falscheZitate')}}"
-       aria-label="Tröte auf Mastodon"
-       tooltip="Tröt!"
-       tooltip-position="bottom">
-      <svg xmlns="http://www.w3.org/2000/svg" width="61.076954mm" height="65.47831mm" viewBox="0 0 216.4144 232.00976" aria-hidden="true">
-        <path fill="#fff" d="M211.80734 139.0875c-3.18125 16.36625-28.4925 34.2775-57.5625 37.74875-15.15875 1.80875-30.08375 3.47125-45.99875 2.74125-26.0275-1.1925-46.565-6.2125-46.565-6.2125 0 2.53375.15625 4.94625.46875 7.2025 3.38375 25.68625 25.47 27.225 46.39125 27.9425 21.11625.7225 39.91875-5.20625 39.91875-5.20625l.8675 19.09s-14.77 7.93125-41.08125 9.39c-14.50875.7975-32.52375-.365-53.50625-5.91875C9.23234 213.82 1.40609 165.31125.20859 116.09125c-.365-14.61375-.14-28.39375-.14-39.91875 0-50.33 32.97625-65.0825 32.97625-65.0825C49.67234 3.45375 78.20359.2425 107.86484 0h.72875c29.66125.2425 58.21125 3.45375 74.8375 11.09 0 0 32.975 14.7525 32.975 65.0825 0 0 .41375 37.13375-4.59875 62.915"/>
-        <path fill="#2b90d9" d="M177.50984 80.077v60.94125h-24.14375v-59.15c0-12.46875-5.24625-18.7975-15.74-18.7975-11.6025 0-17.4175 7.5075-17.4175 22.3525v32.37625H96.20734V85.42325c0-14.845-5.81625-22.3525-17.41875-22.3525-10.49375 0-15.74 6.32875-15.74 18.7975v59.15H38.90484V80.077c0-12.455 3.17125-22.3525 9.54125-29.675 6.56875-7.3225 15.17125-11.07625 25.85-11.07625 12.355 0 21.71125 4.74875 27.8975 14.2475l6.01375 10.08125 6.015-10.08125c6.185-9.49875 15.54125-14.2475 27.8975-14.2475 10.6775 0 19.28 3.75375 25.85 11.07625 6.36875 7.3225 9.54 17.22 9.54 29.675"/>
-      </svg>Teile auf Mastodon</a>
+    {% if settings.get("SHOW_SHARING_ON_MASTODON") %}
+      <a id="mastodon"
+         href="{{fix_url('/troet', save='sure', text=f'{u_text}\n\n{u_url}\n\n#falscheZitate')}}"
+         aria-label="Tröte auf Mastodon"
+         tooltip="Tröt!"
+         tooltip-position="bottom">
+        <svg xmlns="http://www.w3.org/2000/svg" width="61.076954mm" height="65.47831mm" viewBox="0 0 216.4144 232.00976" aria-hidden="true">
+          <path fill="#fff" d="M211.80734 139.0875c-3.18125 16.36625-28.4925 34.2775-57.5625 37.74875-15.15875 1.80875-30.08375 3.47125-45.99875 2.74125-26.0275-1.1925-46.565-6.2125-46.565-6.2125 0 2.53375.15625 4.94625.46875 7.2025 3.38375 25.68625 25.47 27.225 46.39125 27.9425 21.11625.7225 39.91875-5.20625 39.91875-5.20625l.8675 19.09s-14.77 7.93125-41.08125 9.39c-14.50875.7975-32.52375-.365-53.50625-5.91875C9.23234 213.82 1.40609 165.31125.20859 116.09125c-.365-14.61375-.14-28.39375-.14-39.91875 0-50.33 32.97625-65.0825 32.97625-65.0825C49.67234 3.45375 78.20359.2425 107.86484 0h.72875c29.66125.2425 58.21125 3.45375 74.8375 11.09 0 0 32.975 14.7525 32.975 65.0825 0 0 .41375 37.13375-4.59875 62.915"/>
+          <path fill="#2b90d9" d="M177.50984 80.077v60.94125h-24.14375v-59.15c0-12.46875-5.24625-18.7975-15.74-18.7975-11.6025 0-17.4175 7.5075-17.4175 22.3525v32.37625H96.20734V85.42325c0-14.845-5.81625-22.3525-17.41875-22.3525-10.49375 0-15.74 6.32875-15.74 18.7975v59.15H38.90484V80.077c0-12.455 3.17125-22.3525 9.54125-29.675 6.56875-7.3225 15.17125-11.07625 25.85-11.07625 12.355 0 21.71125 4.74875 27.8975 14.2475l6.01375 10.08125 6.015-10.08125c6.185-9.49875 15.54125-14.2475 27.8975-14.2475 10.6775 0 19.28 3.75375 25.85 11.07625 6.36875 7.3225 9.54 17.22 9.54 29.675"/>
+        </svg>Teile auf Mastodon</a>
+    {% end %}
 
     <a no-dynload id="email"
        href="mailto:?subject={{text}}&amp;body={{quote_url}}"
        aria-label="Teile über E-Mail">
       <svg class="stroke-2x" xmlns="http://www.w3.org/2000/svg" viewBox="-1 -1 26 26" aria-hidden="true">
         <path d="M23.5 18c0 .8-.7 1.5-1.5 1.5H2c-.8 0-1.5-.7-1.5-1.5V6c0-.8.7-1.5 1.5-1.5h20c.8 0 1.5.7 1.5 1.5v12zm-3-9.5L12 14 3.5 8.5m0 7.5L7 14m13.5 2L17 14"/>
       </svg>Teile über E-Mail</a>
```

### Comparing `an-website-24.5/an_website/templates/pages/redirect.html` & `an_website-24.6/an_website/templates/pages/redirect.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/search.html` & `an_website-24.6/an_website/templates/pages/search.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/services.html` & `an_website-24.6/an_website/templates/pages/services.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/settings.html` & `an_website-24.6/an_website/templates/pages/settings.html`

 * *Files 3% similar despite different names*

```diff
@@ -22,30 +22,32 @@
                 <input type="checkbox"
                        name="no_3rd_party"
                        {% if no_3rd_party %} checked {% end %}
                        value="sure">
             </label>
         {% end %}
 
-        {% if ask_before_leaving_default %}
-            <label class="form-element">
-                Seite ohne zu fragen verlassen
-                <input type="checkbox"
-                       name="ask_before_leaving"
-                       {% if not ask_before_leaving %} checked {% end %}
-                       value="nope">
-            </label>
-        {% else %}
-            <label class="form-element">
-                Frage bevor dem Verlassen der Seite
-                <input type="checkbox"
-                       name="ask_before_leaving"
-                       {% if ask_before_leaving %} checked {% end %}
-                       value="sure">
-            </label>
+        {% if settings.get("REDIRECT_API_LOADED") %}
+            {% if ask_before_leaving_default %}
+                <label class="form-element">
+                    Seite ohne zu fragen verlassen
+                    <input type="checkbox"
+                           name="ask_before_leaving"
+                           {% if not ask_before_leaving %} checked {% end %}
+                           value="nope">
+                </label>
+            {% else %}
+                <label class="form-element">
+                    Frage bevor dem Verlassen der Seite
+                    <input type="checkbox"
+                           name="ask_before_leaving"
+                           {% if ask_before_leaving %} checked {% end %}
+                           value="sure">
+                </label>
+            {% end %}
         {% end %}
 
         <label class="form-element">
             Nutze coole Emojis von OpenMoji
             <select name="openmoji">
                 <option {% if not openmoji %} selected {% end %}
                         value="nope">Deaktiviert</option>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 {% extends "../base.html" %} {% block head %}
 {% end %} {% block body %}
 {% if no_3rd_party_default %} Erlaube Inhalte von Drittanbietern
 % if not no_3rd_party %} checked {% end %} value="nope"> {% else %} Deaktiviere
 Inhalte von Drittanbietern
 % if no_3rd_party %} checked {% end %} value="sure"> {% end %} {% if
-ask_before_leaving_default %} Seite ohne zu fragen verlassen
+settings.get("REDIRECT_API_LOADED") %} {% if ask_before_leaving_default %}
+Seite ohne zu fragen verlassen
 % if not ask_before_leaving %} checked {% end %} value="nope"> {% else %} Frage
 bevor dem Verlassen der Seite
 % if not openmoji %} selected {% end %} value="nope">Deaktiviert
 % if openmoji == "glyf_colr0" %} selected {% end %} value="glyf_colr0">Font
 (COLRv0)
 % if openmoji == "glyf_colr1" %} selected {% end %} value="glyf_colr1">Font
 (COLRv1)
```

### Comparing `an-website-24.5/an_website/templates/pages/soundboard.html` & `an_website-24.6/an_website/templates/pages/soundboard.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/swapped_words.html` & `an_website-24.6/an_website/templates/pages/swapped_words.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/troet.html` & `an_website-24.6/an_website/templates/pages/troet.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/uptime.html` & `an_website-24.6/an_website/templates/pages/uptime.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/version.html` & `an_website-24.6/an_website/templates/pages/version.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/pages/wordgame_solver.html` & `an_website-24.6/an_website/templates/pages/wordgame_solver.html`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/templates/rss/quote_of_the_day.xml` & `an_website-24.6/an_website/templates/rss/quote_of_the_day.xml`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/troet/__init__.py` & `an_website-24.6/an_website/troet/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/troet/troet.py` & `an_website-24.6/an_website/troet/troet.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/update/__init__.py` & `an_website-24.6/an_website/update/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/update/update.py` & `an_website-24.6/an_website/update/update.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/uptime/__init__.py` & `an_website-24.6/an_website/uptime/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/uptime/uptime.py` & `an_website-24.6/an_website/uptime/uptime.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/utils/__init__.py` & `an_website-24.6/an_website/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/utils/base_request_handler.py` & `an_website-24.6/an_website/utils/base_request_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,15 +310,18 @@
         otherwise just return the URL with no_3rd_party appended.
         """
         if url is None:
             url = self.request.full_url()
         if isinstance(url, str):
             url = urlsplit(url)
         if url.netloc and url.netloc.lower() != self.request.host.lower():
-            if not self.user_settings.ask_before_leaving:
+            if (
+                not self.user_settings.ask_before_leaving
+                or not self.settings.get("REDIRECT_MODULE_LOADED")
+            ):
                 return url.geturl()
             path = "/redirect"
             query_args["to"] = url.geturl()
             url = urlsplit(self.request.full_url())
         else:
             path = url.path if new_path is None else new_path
         path = f"/{path.strip('/')}".lower()
@@ -1042,15 +1045,15 @@
                 if permission.name:
                     self.set_header(
                         f"X-Permission-{permission.name}",
                         bool_to_str(bool(self.is_authorized(permission))),
                     )
         self.set_header("Vary", "Accept,Accept-Encoding,Authorization,Cookie")
         self.origin_trial(
-            "Ajkk8O9wTRnbG/A5GvQUW2G8n/y6carJa8GuV9PFXfsqBZq08anjBkvSJLxzrV8dRobSyXCV/wkpyl2Zco2SLgQAAABmeyJvcmlnaW4iOiJodHRwczovL2Fzb3ppYWwub3JnOjQ0MyIsImZlYXR1cmUiOiJXZWJBcHBUYWJTdHJpcCIsImV4cGlyeSI6MTcxNjk0MDc5OSwiaXNTdWJkb21haW4iOnRydWV9"  # noqa: B950  # pylint: disable=line-too-long, useless-suppression
+            "AqP0dXp3uiIft5WtVI2f2KoR13gQy0w2lrhRj7E8zo0J0XlmWGPDSulJZvPqj+GtF+WQtqQJdht4bQgi852+2QAAAABmeyJvcmlnaW4iOiJodHRwczovL2Fzb3ppYWwub3JnOjQ0MyIsImZlYXR1cmUiOiJXZWJBcHBUYWJTdHJpcCIsImV4cGlyeSI6MTcyMjk4ODc5OSwiaXNTdWJkb21haW4iOnRydWV9"  # noqa: B950  # pylint: disable=line-too-long, useless-suppression
         )
 
     @classmethod
     def supports_head(cls) -> bool:
         """Check whether this request handler supports HEAD requests."""
         signature = inspect.signature(cls.get)
         return (
```

### Comparing `an-website-24.5/an_website/utils/better_config_parser.py` & `an_website-24.6/an_website/utils/better_config_parser.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/utils/data_parsing.py` & `an_website-24.6/an_website/utils/data_parsing.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/utils/decorators.py` & `an_website-24.6/an_website/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/utils/logging.py` & `an_website-24.6/an_website/utils/logging.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/utils/options.py` & `an_website-24.6/an_website/utils/options.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/utils/request_handler.py` & `an_website-24.6/an_website/utils/request_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,25 +92,25 @@
 
         new_path = replace_umlauts(new_path)
 
         if new_path.lower() in SUS_PATHS:
             self.set_status(469, reason="Nice Try")
             return self.write_error(469)
 
-        if new_path != self.request.path:
+        if new_path and new_path != self.request.path:
             return self.redirect(self.fix_url(new_path=new_path), True)
 
         this_path_normalized = unquote(new_path).strip("/").lower()
 
         paths: Mapping[str, str] = self.settings.get("NORMED_PATHS") or {}
 
         if p := paths.get(this_path_normalized):
             return self.redirect(self.fix_url(new_path=p), False)
 
-        if len(this_path_normalized) <= 1:
+        if len(this_path_normalized) <= 1 and self.request.path != "/":
             return self.redirect(self.fix_url(new_path="/"))
 
         prefixes = tuple(
             (p, repl)
             for p, repl in paths.items()
             if this_path_normalized.startswith(f"{p}/")
             if f"/{p}" != repl.lower()
```

### Comparing `an-website-24.5/an_website/utils/search.py` & `an_website-24.6/an_website/utils/search.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/utils/static_file_from_traversable.py` & `an_website-24.6/an_website/utils/static_file_from_traversable.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/utils/static_file_handling.py` & `an_website-24.6/an_website/utils/static_file_handling.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/utils/token.py` & `an_website-24.6/an_website/utils/token.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/utils/utils.py` & `an_website-24.6/an_website/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,31 +25,34 @@
 import random
 import sys
 import time
 from base64 import b85encode
 from collections.abc import (
     Awaitable,
     Callable,
+    Collection,
     Generator,
     Iterable,
     Mapping,
     Set,
 )
 from dataclasses import dataclass, field
 from datetime import datetime, timezone
 from enum import IntFlag
 from functools import cache, partial
 from hashlib import sha1
 from ipaddress import IPv4Address, IPv6Address, ip_address, ip_network
 from pathlib import Path
 from typing import (
     IO,
+    TYPE_CHECKING,
     Any,
     Final,
     Literal,
+    ParamSpec,
     TypeAlias,
     TypeVar,
     Union,
     cast,
     get_args,
 )
 from urllib.parse import SplitResult, parse_qsl, urlencode, urlsplit, urlunsplit
@@ -65,17 +68,21 @@
 from redis.asyncio import Redis
 from tornado.web import HTTPError, RequestHandler
 from UltraDict import UltraDict  # type: ignore[import-untyped]
 
 from .. import DIR as ROOT_DIR
 from .. import STATIC_DIR
 
+if TYPE_CHECKING:
+    from .background_tasks import BackgroundTask
+
 LOGGER: Final = logging.getLogger(__name__)
 
 T = TypeVar("T")
+P = ParamSpec("P")
 
 T_Val = TypeVar("T_Val")  # pylint: disable=invalid-name
 
 TOptionalStr = TypeVar(  # pylint: disable=invalid-name
     "TOptionalStr", None, str
 )
 
@@ -788,18 +795,20 @@
 
 def strangle(string: str) -> float:
     """Convert a string to an angle."""
     hasher = sha1(string.encode("UTF-8"), usedforsecurity=False)
     return int.from_bytes(hasher.digest()[:2], "little") / (1 << 16) * 360
 
 
-def time_function(function: Callable[..., T], *args: Any) -> tuple[T, float]:
+def time_function(
+    function: Callable[P, T], *args: P.args, **kwargs: P.kwargs
+) -> tuple[T, float]:
     """Run the function and return the result and the time it took in seconds."""
     timer = Timer()
-    return function(*args), timer.stop()
+    return function(*args, **kwargs), timer.stop()
 
 
 def time_to_str(spam: float) -> str:
     """Convert the time into a string with second precision."""
     int_time = int(spam)
     div_60 = int(int_time / 60)
     div_60_60 = int(div_60 / 60)
@@ -832,14 +841,17 @@
 
     This gets created by every module to add the handlers.
     """
 
     handlers: tuple[Handler, ...] = field(default_factory=tuple[Handler, ...])
     sub_pages: tuple[PageInfo, ...] = field(default_factory=tuple)
     aliases: tuple[str, ...] | Mapping[str, str] = field(default_factory=tuple)
+    required_background_tasks: Collection[BackgroundTask] = field(
+        default_factory=frozenset
+    )
 
     def get_keywords_as_str(self, path: str) -> str:
         """Get the keywords as comma-seperated string."""
         page_info = self.get_page_info(path)
         if self != page_info:
             return ", ".join((*self.keywords, *page_info.keywords))
```

### Comparing `an-website-24.5/an_website/vendored/apm-rum/elastic-apm-rum.umd.js` & `an_website-24.6/an_website/vendored/apm-rum/elastic-apm-rum.umd.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js` & `an_website-24.6/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js.map` & `an_website-24.6/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/vendored/media-types.json` & `an_website-24.6/an_website/vendored/media-types.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/vendored/mime-db.json` & `an_website-24.6/an_website/vendored/mime-db.json`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/vendored/screenfetch` & `an_website-24.6/an_website/vendored/screenfetch`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/version/__init__.py` & `an_website-24.6/an_website/version/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/version/version.py` & `an_website-24.6/an_website/version/version.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/whats_my_ip/__init__.py` & `an_website-24.6/an_website/whats_my_ip/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/whats_my_ip/ip.py` & `an_website-24.6/an_website/whats_my_ip/ip.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/wiki/__init__.py` & `an_website-24.6/an_website/wiki/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website/wiki/wiki.py` & `an_website-24.6/an_website/wiki/wiki.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/an_website.egg-info/PKG-INFO` & `an_website-24.6/an_website.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: an-website
-Version: 24.5
+Version: 24.6
 Summary: #1 Website in the Worlds
 Home-page: https://github.com/asozialesnetzwerk/an-website
 Author: Das Asoziale Netzwerk
 Author-email: contact@asozial.org
 License: AGPL-3.0-or-later
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,32 +25,32 @@
 Requires-Dist: async-timeout==4.0.3; python_full_version < "3.11.3"
 Requires-Dist: attrs==23.2.0; python_version >= "3.7"
 Requires-Dist: beautifulsoup4==4.12.3; python_full_version >= "3.6.0"
 Requires-Dist: blake3==0.4.1
 Requires-Dist: brotli==1.1.0
 Requires-Dist: certifi==2023.11.17; python_version >= "3.6"
 Requires-Dist: cffi==1.16.0; python_version >= "3.8"
-Requires-Dist: defity==0.3.1; python_version >= "3.7"
+Requires-Dist: defity==0.4.0; python_version >= "3.9"
 Requires-Dist: defusedxml==0.7.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"
 Requires-Dist: dill==0.3.8; python_version >= "3.8"
 Requires-Dist: dunamai==1.21.1; python_version >= "3.5"
 Requires-Dist: ecs-logging==2.1.0; python_version >= "3.6"
-Requires-Dist: elastic-apm==6.22.0; python_version >= "3.6" and python_version < "4"
+Requires-Dist: elastic-apm==6.22.2; python_version >= "3.6" and python_version < "4"
 Requires-Dist: elastic-enterprise-search==8.11.0; python_version >= "3.6"
-Requires-Dist: elastic-transport==8.13.0; python_version >= "3.7"
+Requires-Dist: elastic-transport==8.13.1; python_version >= "3.7"
 Requires-Dist: elasticsearch[async]==8.12.1; python_version >= "3.7"
 Requires-Dist: emoji==2.11.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: frozenlist==1.4.1; python_version >= "3.8"
 Requires-Dist: funcparserlib==1.0.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6" and python_version < "3.13"
 Requires-Dist: get-version==3.5.5; python_version >= "3.9"
-Requires-Dist: hangman-solver-rs==0.2.1; python_version >= "3.10"
+Requires-Dist: hangman-solver-rs==0.3.1; python_version >= "3.12"
 Requires-Dist: hiredis==2.3.2
 Requires-Dist: html2text==2020.1.16; python_version >= "3.5"
-Requires-Dist: hy==0.28.0; python_version < "3.13" and python_version >= "3.8"
-Requires-Dist: hyrule==0.5.0; python_version < "3.13"
+Requires-Dist: hy==0.29.0; python_version < "3.13" and python_version >= "3.8"
+Requires-Dist: hyrule==0.6.0; python_version < "3.13"
 Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: jsonpickle==3.0.4; python_version >= "3.7"
 Requires-Dist: lxml==5.2.2; python_version >= "3.6"
 Requires-Dist: multidict==6.0.5; python_version >= "3.7"
 Requires-Dist: openmoji-dist==15.0.0.1
 Requires-Dist: orjson==3.10.3; python_version >= "3.8"
 Requires-Dist: packaging==23.2; python_version >= "3.7"
@@ -63,27 +63,27 @@
 Requires-Dist: pyjwt==2.8.0; python_version >= "3.7"
 Requires-Dist: pysocks==1.7.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: python-dateutil==2.9.0.post0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: python-geoip-geolite2-yplan==2019.1224
 Requires-Dist: python-geoip-yplan==1.2
 Requires-Dist: pytz==2023.4
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
-Requires-Dist: rapidfuzz==3.9.0; python_version >= "3.8"
+Requires-Dist: rapidfuzz==3.9.3; python_version >= "3.8"
 Requires-Dist: redis[hiredis]==5.0.4; python_version >= "3.7"
 Requires-Dist: regex==2023.12.25; python_version >= "3.7"
 Requires-Dist: setproctitle==1.3.3; python_version >= "3.7"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: soupsieve==2.5; python_version >= "3.8"
 Requires-Dist: tornado==6.4; python_version >= "3.8"
 Requires-Dist: typed-stream==0.131.0; python_version >= "3.10"
 Requires-Dist: tzdata==2023.4; python_version >= "2"
 Requires-Dist: ultradict==0.0.6; python_version >= "3.8"
 Requires-Dist: urllib3==2.2.1; python_version >= "3.8"
 Requires-Dist: uvloop==0.19.0; python_full_version >= "3.8.0"
-Requires-Dist: wrapt==1.14.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"
+Requires-Dist: wrapt==1.16.0; python_version >= "3.6"
 Requires-Dist: yarl==1.9.4; python_version >= "3.7"
 
 # Webseite des AN
 
 ![License](https://img.shields.io/pypi/l/an-website?label=License)
 ![Python](https://img.shields.io/pypi/pyversions/an-website?label=Python)
 ![Implementation](https://img.shields.io/pypi/implementation/an-website?label=Implementation)
```

### Comparing `an-website-24.5/an_website.egg-info/SOURCES.txt` & `an_website-24.6/an_website.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -337,18 +337,20 @@
 an_website/troet/__init__.py
 an_website/troet/troet.py
 an_website/update/__init__.py
 an_website/update/update.py
 an_website/uptime/__init__.py
 an_website/uptime/uptime.py
 an_website/utils/__init__.py
+an_website/utils/background_tasks.py
 an_website/utils/base_request_handler.py
 an_website/utils/better_config_parser.py
 an_website/utils/data_parsing.py
 an_website/utils/decorators.py
+an_website/utils/elasticsearch_setup.py
 an_website/utils/logging.py
 an_website/utils/options.py
 an_website/utils/request_handler.py
 an_website/utils/search.py
 an_website/utils/static_file_from_traversable.py
 an_website/utils/static_file_handling.py
 an_website/utils/token.py
```

### Comparing `an-website-24.5/an_website.egg-info/requires.txt` & `an_website-24.6/an_website.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,62 +14,63 @@
 [:python_full_version >= "3.6.0"]
 beautifulsoup4==4.12.3
 
 [:python_full_version >= "3.8.0"]
 uvloop==0.19.0
 
 [:python_version < "3.13"]
-hyrule==0.5.0
+hyrule==0.6.0
 
 [:python_version < "3.13" and python_version >= "3.8"]
-hy==0.28.0
+hy==0.29.0
 
 [:python_version >= "2"]
 tzdata==2023.4
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"]
 emoji==2.11.1
 pysocks==1.7.1
 python-dateutil==2.9.0.post0
 six==1.16.0
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"]
 defusedxml==0.7.1
 pycryptodome==3.20.0
-wrapt==1.14.1
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6" and python_version < "3.13"]
 funcparserlib==1.0.1
 
 [:python_version >= "3.10"]
-hangman-solver-rs==0.2.1
 typed-stream==0.131.0
 
+[:python_version >= "3.12"]
+hangman-solver-rs==0.3.1
+
 [:python_version >= "3.5"]
 dunamai==1.21.1
 html2text==2020.1.16
 idna==3.7
 pycurl==7.45.2
 
 [:python_version >= "3.6"]
 certifi==2023.11.17
 ecs-logging==2.1.0
 elastic-enterprise-search==8.11.0
 lxml==5.2.2
 pyyaml==6.0.1
+wrapt==1.16.0
 
 [:python_version >= "3.6" and python_version < "4"]
-elastic-apm==6.22.0
+elastic-apm==6.22.2
 
 [:python_version >= "3.7"]
 aiosignal==1.3.1
 ansi2html==1.9.1
 attrs==23.2.0
-defity==0.3.1
-elastic-transport==8.13.0
+elastic-transport==8.13.1
 elasticsearch[async]==8.12.1
 jsonpickle==3.0.4
 multidict==6.0.5
 packaging==23.2
 pyjwt==2.8.0
 redis[hiredis]==5.0.4
 regex==2023.12.25
@@ -82,15 +83,16 @@
 dill==0.3.8
 frozenlist==1.4.1
 orjson==3.10.3
 pillow==10.3.0
 pillow-jxl-plugin==1.2.4
 pycares==4.4.0
 pycparser==2.22
-rapidfuzz==3.9.0
+rapidfuzz==3.9.3
 soupsieve==2.5
 tornado==6.4
 ultradict==0.0.6
 urllib3==2.2.1
 
 [:python_version >= "3.9"]
+defity==0.4.0
 get-version==3.5.5
```

### Comparing `an-website-24.5/build-oci-image.sh` & `an_website-24.6/build-oci-image.sh`

 * *Files identical despite different names*

### Comparing `an-website-24.5/example-configurations/config.ini.default` & `an_website-24.6/example-configurations/config.ini.default`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 webhook_content_type = application/json
 webhook_body_format = {"text":"[%(levelname)1.1s %(asctime)s %(module)s:%(lineno)d] %(message)s"}
 #webhook_timestamp_format = 
 #webhook_timestamp_timezone = 
 webhook_escape_message = sure
 
 [GENERAL]
-ignored_modules = element_web_link.*
+ignored_modules = element_web_link
 compress_response = nope
 cookie_secret = xyzzy
 #domain = 
 netcup = nope
 commitment_uri = https://github.asozial.org/an-website/commitment.txt
 #onion_address = 
 ratelimits = nope
```

### Comparing `an-website-24.5/example-configurations/config.ini.example` & `an_website-24.6/example-configurations/config.ini.example`

 * *Files identical despite different names*

### Comparing `an-website-24.5/example-configurations/nginx/an-website.conf` & `an_website-24.6/example-configurations/nginx/an-website.conf`

 * *Files identical despite different names*

### Comparing `an-website-24.5/pip-requirements.txt` & `an_website-24.6/pip-requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 async-timeout==4.0.3; python_full_version < '3.11.3'
 attrs==23.2.0; python_version >= '3.7'
 beautifulsoup4==4.12.3; python_full_version >= '3.6.0'
 blake3==0.4.1
 brotli==1.1.0
 certifi==2023.11.17; python_version >= '3.6'
 cffi==1.16.0; python_version >= '3.8'
-defity==0.3.1; python_version >= '3.7'
+defity==0.4.0; python_version >= '3.9'
 defusedxml==0.7.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
 dill==0.3.8; python_version >= '3.8'
 dunamai==1.21.1; python_version >= '3.5'
 ecs-logging==2.1.0; python_version >= '3.6'
-elastic-apm==6.22.0; python_version >= '3.6' and python_version < '4'
+elastic-apm==6.22.2; python_version >= '3.6' and python_version < '4'
 elastic-enterprise-search==8.11.0; python_version >= '3.6'
-elastic-transport==8.13.0; python_version >= '3.7'
+elastic-transport==8.13.1; python_version >= '3.7'
 elasticsearch[async]==8.12.1; python_version >= '3.7'
 emoji==2.11.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 frozenlist==1.4.1; python_version >= '3.8'
 funcparserlib==1.0.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6' and python_version < '3.13'
 get-version==3.5.5; python_version >= '3.9'
-hangman-solver-rs==0.2.1; python_version >= '3.10'
+hangman-solver-rs==0.3.1; python_version >= '3.12'
 hiredis==2.3.2
 html2text==2020.1.16; python_version >= '3.5'
-hy==0.28.0; python_version < '3.13' and python_version >= '3.8'
-hyrule==0.5.0; python_version < '3.13'
+hy==0.29.0; python_version < '3.13' and python_version >= '3.8'
+hyrule==0.6.0; python_version < '3.13'
 idna==3.7; python_version >= '3.5'
 jsonpickle==3.0.4; python_version >= '3.7'
 lxml==5.2.2; python_version >= '3.6'
 multidict==6.0.5; python_version >= '3.7'
 openmoji-dist==15.0.0.1
 orjson==3.10.3; python_version >= '3.8'
 packaging==23.2; python_version >= '3.7'
@@ -44,21 +44,21 @@
 pyjwt==2.8.0; python_version >= '3.7'
 pysocks==1.7.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 python-dateutil==2.9.0.post0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 python-geoip-geolite2-yplan==2019.1224
 python-geoip-yplan==1.2
 pytz==2023.4
 pyyaml==6.0.1; python_version >= '3.6'
-rapidfuzz==3.9.0; python_version >= '3.8'
+rapidfuzz==3.9.3; python_version >= '3.8'
 redis[hiredis]==5.0.4; python_version >= '3.7'
 regex==2023.12.25; python_version >= '3.7'
 setproctitle==1.3.3; python_version >= '3.7'
 six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 soupsieve==2.5; python_version >= '3.8'
 tornado==6.4; python_version >= '3.8'
 typed-stream==0.131.0; python_version >= '3.10'
 tzdata==2023.4; python_version >= '2'
 ultradict==0.0.6; python_version >= '3.8'
 urllib3==2.2.1; python_version >= '3.8'
 uvloop==0.19.0; python_full_version >= '3.8.0'
-wrapt==1.14.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
+wrapt==1.16.0; python_version >= '3.6'
 yarl==1.9.4; python_version >= '3.7'
```

### Comparing `an-website-24.5/pyproject.toml` & `an_website-24.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools==69.2.0", "wheel==0.42.0"]
+requires = ["setuptools==69.5.1", "wheel==0.42.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.bandit]
 skips = ["B101", "B311", "B413"]
 
 [tool.black]
 target-version = ["py312"]
```

### Comparing `an-website-24.5/setup.py` & `an_website-24.6/setup.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_backdoor.py` & `an_website-24.6/tests/test_backdoor.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_christmas.py` & `an_website-24.6/tests/test_christmas.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_commitment.py` & `an_website-24.6/tests/test_commitment.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_contact.py` & `an_website-24.6/tests/test_contact.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_currency_converter.py` & `an_website-24.6/tests/test_currency_converter.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_hangman_solver.py` & `an_website-24.6/tests/test_hangman_solver.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_main.py` & `an_website-24.6/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_permissions.py` & `an_website-24.6/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_quotes.py` & `an_website-24.6/tests/test_quotes.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_random_text.py` & `an_website-24.6/tests/test_random_text.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_request_handlers.py` & `an_website-24.6/tests/test_request_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         "/vertauschte-woerter",
         {307},
         httpclient=SimpleAsyncHTTPClient(),
     )
 
     await assert_valid_redirect(fetch, "/a?x=y", "/?x=y", {307})
 
-    await assert_valid_redirect(fetch, "/index.php", "/", {308})
+    await assert_valid_redirect(fetch, "/index.php", "/", {307})
     assert_valid_html_response(
         await fetch(
             "/index.php", method="POST", allow_nonstandard_methods=True
         ),
         {404},
     )
```

### Comparing `an-website-24.5/tests/test_settings.py` & `an_website-24.6/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_swapped_words.py` & `an_website-24.6/tests/test_swapped_words.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_token.py` & `an_website-24.6/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_traversable_static_file_handler.py` & `an_website-24.6/tests/test_traversable_static_file_handler.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_troet.py` & `an_website-24.6/tests/test_troet.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_uptime.py` & `an_website-24.6/tests/test_uptime.py`

 * *Files identical despite different names*

### Comparing `an-website-24.5/tests/test_utils.py` & `an_website-24.6/tests/test_utils.py`

 * *Files identical despite different names*

