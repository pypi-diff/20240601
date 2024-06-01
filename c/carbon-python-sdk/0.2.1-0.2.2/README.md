# Comparing `tmp/carbon_python_sdk-0.2.1.tar.gz` & `tmp/carbon_python_sdk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbon_python_sdk-0.2.1.tar", max compression
+gzip compressed data, was "carbon_python_sdk-0.2.2.tar", max compression
```

## Comparing `carbon_python_sdk-0.2.1.tar` & `carbon_python_sdk-0.2.2.tar`

### file list

```diff
@@ -1,981 +1,985 @@
--rw-r--r--   0        0        0     1081 2024-05-30 19:55:10.782600 carbon_python_sdk-0.2.1/LICENSE
--rw-r--r--   0        0        0   112828 2024-05-30 19:57:32.272363 carbon_python_sdk-0.2.1/README.md
--rw-r--r--   0        0        0      675 2024-05-30 19:57:32.272988 carbon_python_sdk-0.2.1/carbon/__init__.py
--rw-r--r--   0        0        0    76940 2024-05-30 19:57:32.274703 carbon_python_sdk-0.2.1/carbon/api_client.py
--rw-r--r--   0        0        0      663 2024-05-30 19:55:10.639307 carbon_python_sdk-0.2.1/carbon/api_response.py
--rw-r--r--   0        0        0      214 2024-05-30 19:55:10.639416 carbon_python_sdk-0.2.1/carbon/apis/__init__.py
--rw-r--r--   0        0        0    11104 2024-05-30 19:55:10.639511 carbon_python_sdk-0.2.1/carbon/apis/path_to_api.py
--rw-r--r--   0        0        0      233 2024-05-30 19:55:10.639705 carbon_python_sdk-0.2.1/carbon/apis/paths/__init__.py
--rw-r--r--   0        0        0      101 2024-05-30 19:55:10.639790 carbon_python_sdk-0.2.1/carbon/apis/paths/add_webhook.py
--rw-r--r--   0        0        0      114 2024-05-30 19:55:10.639877 carbon_python_sdk-0.2.1/carbon/apis/paths/auth_v1_access_token.py
--rw-r--r--   0        0        0      118 2024-05-30 19:55:10.639963 carbon_python_sdk-0.2.1/carbon/apis/paths/auth_v1_white_labeling.py
--rw-r--r--   0        0        0      119 2024-05-30 19:55:10.640210 carbon_python_sdk-0.2.1/carbon/apis/paths/create_user_file_tags.py
--rw-r--r--   0        0        0      103 2024-05-30 19:55:10.640347 carbon_python_sdk-0.2.1/carbon/apis/paths/delete_files.py
--rw-r--r--   0        0        0      108 2024-05-30 19:55:10.640448 carbon_python_sdk-0.2.1/carbon/apis/paths/delete_files_v2.py
--rw-r--r--   0        0        0      119 2024-05-30 19:55:10.640540 carbon_python_sdk-0.2.1/carbon/apis/paths/delete_user_file_tags.py
--rw-r--r--   0        0        0      103 2024-05-30 19:55:10.640627 carbon_python_sdk-0.2.1/carbon/apis/paths/delete_users.py
--rw-r--r--   0        0        0      133 2024-05-30 19:55:10.640715 carbon_python_sdk-0.2.1/carbon/apis/paths/delete_webhook_webhook_id.py
--rw-r--r--   0        0        0      120 2024-05-30 19:55:10.640803 carbon_python_sdk-0.2.1/carbon/apis/paths/deletefile_file_id.py
--rw-r--r--   0        0        0      100 2024-05-30 19:55:10.640891 carbon_python_sdk-0.2.1/carbon/apis/paths/embeddings.py
--rw-r--r--   0        0        0       96 2024-05-30 19:55:10.640978 carbon_python_sdk-0.2.1/carbon/apis/paths/fetch_urls.py
--rw-r--r--   0        0        0      123 2024-05-30 19:55:10.641072 carbon_python_sdk-0.2.1/carbon/apis/paths/fetch_youtube_transcript.py
--rw-r--r--   0        0        0       89 2024-05-30 19:55:10.641154 carbon_python_sdk-0.2.1/carbon/apis/paths/health.py
--rw-r--r--   0        0        0      134 2024-05-30 19:55:10.641235 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_confluence_list.py
--rw-r--r--   0        0        0      134 2024-05-30 19:55:10.641317 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_confluence_sync.py
--rw-r--r--   0        0        0      119 2024-05-30 19:55:10.641399 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_connect.py
--rw-r--r--   0        0        0      124 2024-05-30 19:55:10.641482 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_files_sync.py
--rw-r--r--   0        0        0      123 2024-05-30 19:55:10.641564 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_freshdesk.py
--rw-r--r--   0        0        0      119 2024-05-30 19:55:10.641644 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_gitbook.py
--rw-r--r--   0        0        0      129 2024-05-30 19:55:10.641725 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_gitbook_spaces.py
--rw-r--r--   0        0        0      128 2024-05-30 19:55:10.641811 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_gitbook_sync.py
--rw-r--r--   0        0        0      117 2024-05-30 19:55:10.641897 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_github.py
--rw-r--r--   0        0        0      125 2024-05-30 19:55:10.641993 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_github_repos.py
--rw-r--r--   0        0        0      137 2024-05-30 19:55:10.642079 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_github_sync_repos.py
--rw-r--r--   0        0        0      124 2024-05-30 19:55:10.642164 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_gmail_sync.py
--rw-r--r--   0        0        0      134 2024-05-30 19:55:10.642252 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_gmail_user_labels.py
--rw-r--r--   0        0        0      124 2024-05-30 19:55:10.642339 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_items_list.py
--rw-r--r--   0        0        0      124 2024-05-30 19:55:10.642419 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_items_sync.py
--rw-r--r--   0        0        0      122 2024-05-30 19:55:10.642499 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_oauth_url.py
--rw-r--r--   0        0        0      128 2024-05-30 19:55:10.642586 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_outlook_sync.py
--rw-r--r--   0        0        0      146 2024-05-30 19:55:10.642674 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_outlook_user_categories.py
--rw-r--r--   0        0        0      140 2024-05-30 19:55:10.642757 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_outlook_user_folders.py
--rw-r--r--   0        0        0      120 2024-05-30 19:55:10.642840 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_rss_feed.py
--rw-r--r--   0        0        0      109 2024-05-30 19:55:10.642921 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_s3.py
--rw-r--r--   0        0        0      120 2024-05-30 19:55:10.643007 carbon_python_sdk-0.2.1/carbon/apis/paths/integrations_s3_files.py
--rw-r--r--   0        0        0      128 2024-05-30 19:55:10.643095 carbon_python_sdk-0.2.1/carbon/apis/paths/modify_user_configuration.py
--rw-r--r--   0        0        0      101 2024-05-30 19:55:10.643332 carbon_python_sdk-0.2.1/carbon/apis/paths/organization.py
--rw-r--r--   0        0        0      125 2024-05-30 19:55:10.643422 carbon_python_sdk-0.2.1/carbon/apis/paths/organization_statistics.py
--rw-r--r--   0        0        0      117 2024-05-30 19:55:10.643518 carbon_python_sdk-0.2.1/carbon/apis/paths/organization_update.py
--rw-r--r--   0        0        0      112 2024-05-30 19:55:10.643604 carbon_python_sdk-0.2.1/carbon/apis/paths/parsed_file_file_id.py
--rw-r--r--   0        0        0      106 2024-05-30 19:55:10.643687 carbon_python_sdk-0.2.1/carbon/apis/paths/process_sitemap.py
--rw-r--r--   0        0        0      106 2024-05-30 19:55:10.643766 carbon_python_sdk-0.2.1/carbon/apis/paths/raw_file_file_id.py
--rw-r--r--   0        0        0      101 2024-05-30 19:55:10.643852 carbon_python_sdk-0.2.1/carbon/apis/paths/resync_file.py
--rw-r--r--   0        0        0      116 2024-05-30 19:55:10.643941 carbon_python_sdk-0.2.1/carbon/apis/paths/revoke_access_token.py
--rw-r--r--   0        0        0      107 2024-05-30 19:55:10.644023 carbon_python_sdk-0.2.1/carbon/apis/paths/scrape_sitemap.py
--rw-r--r--   0        0        0       98 2024-05-30 19:55:10.644104 carbon_python_sdk-0.2.1/carbon/apis/paths/search_urls.py
--rw-r--r--   0        0        0      101 2024-05-30 19:55:10.644183 carbon_python_sdk-0.2.1/carbon/apis/paths/text_chunks.py
--rw-r--r--   0        0        0      103 2024-05-30 19:55:10.644262 carbon_python_sdk-0.2.1/carbon/apis/paths/update_users.py
--rw-r--r--   0        0        0      133 2024-05-30 19:55:10.644340 carbon_python_sdk-0.2.1/carbon/apis/paths/upload_chunks_and_embeddings.py
--rw-r--r--   0        0        0      117 2024-05-30 19:55:10.644424 carbon_python_sdk-0.2.1/carbon/apis/paths/upload_file_from_url.py
--rw-r--r--   0        0        0      101 2024-05-30 19:55:10.644500 carbon_python_sdk-0.2.1/carbon/apis/paths/upload_text.py
--rw-r--r--   0        0        0      100 2024-05-30 19:55:10.644579 carbon_python_sdk-0.2.1/carbon/apis/paths/uploadfile.py
--rw-r--r--   0        0        0       88 2024-05-30 19:55:10.644658 carbon_python_sdk-0.2.1/carbon/apis/paths/user.py
--rw-r--r--   0        0        0      112 2024-05-30 19:55:10.644745 carbon_python_sdk-0.2.1/carbon/apis/paths/user_data_sources.py
--rw-r--r--   0        0        0       99 2024-05-30 19:55:10.644831 carbon_python_sdk-0.2.1/carbon/apis/paths/user_files.py
--rw-r--r--   0        0        0      104 2024-05-30 19:55:10.644916 carbon_python_sdk-0.2.1/carbon/apis/paths/user_files_v2.py
--rw-r--r--   0        0        0       99 2024-05-30 19:55:10.644999 carbon_python_sdk-0.2.1/carbon/apis/paths/web_scrape.py
--rw-r--r--   0        0        0       96 2024-05-30 19:55:10.645082 carbon_python_sdk-0.2.1/carbon/apis/paths/webhooks.py
--rw-r--r--   0        0        0     2044 2024-05-30 19:55:10.645166 carbon_python_sdk-0.2.1/carbon/apis/tag_to_api.py
--rw-r--r--   0        0        0      655 2024-05-30 19:55:10.645270 carbon_python_sdk-0.2.1/carbon/apis/tags/__init__.py
--rw-r--r--   0        0        0      125 2024-05-30 19:55:10.645348 carbon_python_sdk-0.2.1/carbon/apis/tags/auth_api.py
--rw-r--r--   0        0        0      671 2024-05-30 19:55:10.645433 carbon_python_sdk-0.2.1/carbon/apis/tags/auth_api_generated.py
--rw-r--r--   0        0        0      493 2024-05-30 19:55:10.645515 carbon_python_sdk-0.2.1/carbon/apis/tags/auth_api_raw.py
--rw-r--r--   0        0        0      154 2024-05-30 19:55:10.645597 carbon_python_sdk-0.2.1/carbon/apis/tags/data_sources_api.py
--rw-r--r--   0        0        0      717 2024-05-30 19:55:10.645682 carbon_python_sdk-0.2.1/carbon/apis/tags/data_sources_api_generated.py
--rw-r--r--   0        0        0      510 2024-05-30 19:55:10.645763 carbon_python_sdk-0.2.1/carbon/apis/tags/data_sources_api_raw.py
--rw-r--r--   0        0        0      149 2024-05-30 19:55:10.645848 carbon_python_sdk-0.2.1/carbon/apis/tags/embeddings_api.py
--rw-r--r--   0        0        0      806 2024-05-30 19:55:10.645933 carbon_python_sdk-0.2.1/carbon/apis/tags/embeddings_api_generated.py
--rw-r--r--   0        0        0      610 2024-05-30 19:55:10.646012 carbon_python_sdk-0.2.1/carbon/apis/tags/embeddings_api_raw.py
--rw-r--r--   0        0        0      129 2024-05-30 19:55:10.646090 carbon_python_sdk-0.2.1/carbon/apis/tags/files_api.py
--rw-r--r--   0        0        0     1495 2024-05-30 19:55:10.646295 carbon_python_sdk-0.2.1/carbon/apis/tags/files_api_generated.py
--rw-r--r--   0        0        0     1379 2024-05-30 19:55:10.646406 carbon_python_sdk-0.2.1/carbon/apis/tags/files_api_raw.py
--rw-r--r--   0        0        0      133 2024-05-30 19:55:10.646492 carbon_python_sdk-0.2.1/carbon/apis/tags/health_api.py
--rw-r--r--   0        0        0      558 2024-05-30 19:55:10.646578 carbon_python_sdk-0.2.1/carbon/apis/tags/health_api_generated.py
--rw-r--r--   0        0        0      366 2024-05-30 19:55:10.646666 carbon_python_sdk-0.2.1/carbon/apis/tags/health_api_raw.py
--rw-r--r--   0        0        0      157 2024-05-30 19:55:10.646744 carbon_python_sdk-0.2.1/carbon/apis/tags/integrations_api.py
--rw-r--r--   0        0        0     2493 2024-05-30 19:55:10.646827 carbon_python_sdk-0.2.1/carbon/apis/tags/integrations_api_generated.py
--rw-r--r--   0        0        0     2403 2024-05-30 19:55:10.646903 carbon_python_sdk-0.2.1/carbon/apis/tags/integrations_api_raw.py
--rw-r--r--   0        0        0      161 2024-05-30 19:55:10.646982 carbon_python_sdk-0.2.1/carbon/apis/tags/organizations_api.py
--rw-r--r--   0        0        0      747 2024-05-30 19:55:10.647061 carbon_python_sdk-0.2.1/carbon/apis/tags/organizations_api_generated.py
--rw-r--r--   0        0        0      539 2024-05-30 19:55:10.647142 carbon_python_sdk-0.2.1/carbon/apis/tags/organizations_api_raw.py
--rw-r--r--   0        0        0      129 2024-05-30 19:55:10.647225 carbon_python_sdk-0.2.1/carbon/apis/tags/users_api.py
--rw-r--r--   0        0        0      781 2024-05-30 19:55:10.647306 carbon_python_sdk-0.2.1/carbon/apis/tags/users_api_generated.py
--rw-r--r--   0        0        0      611 2024-05-30 19:55:10.647383 carbon_python_sdk-0.2.1/carbon/apis/tags/users_api_raw.py
--rw-r--r--   0        0        0      145 2024-05-30 19:55:10.647462 carbon_python_sdk-0.2.1/carbon/apis/tags/utilities_api.py
--rw-r--r--   0        0        0      984 2024-05-30 19:55:10.647544 carbon_python_sdk-0.2.1/carbon/apis/tags/utilities_api_generated.py
--rw-r--r--   0        0        0      810 2024-05-30 19:55:10.647622 carbon_python_sdk-0.2.1/carbon/apis/tags/utilities_api_raw.py
--rw-r--r--   0        0        0      141 2024-05-30 19:55:10.647698 carbon_python_sdk-0.2.1/carbon/apis/tags/webhooks_api.py
--rw-r--r--   0        0        0      713 2024-05-30 19:55:10.647778 carbon_python_sdk-0.2.1/carbon/apis/tags/webhooks_api_generated.py
--rw-r--r--   0        0        0      525 2024-05-30 19:55:10.647859 carbon_python_sdk-0.2.1/carbon/apis/tags/webhooks_api_raw.py
--rw-r--r--   0        0        0     1986 2024-05-30 19:55:10.647939 carbon_python_sdk-0.2.1/carbon/client.py
--rw-r--r--   0        0        0     1986 2024-05-30 19:55:10.648012 carbon_python_sdk-0.2.1/carbon/client.pyi
--rw-r--r--   0        0        0      676 2024-05-30 19:55:10.648089 carbon_python_sdk-0.2.1/carbon/client_custom.py
--rw-r--r--   0        0        0    17804 2024-05-30 19:57:32.275865 carbon_python_sdk-0.2.1/carbon/configuration.py
--rw-r--r--   0        0        0     7679 2024-05-30 19:55:10.648289 carbon_python_sdk-0.2.1/carbon/exceptions.py
--rw-r--r--   0        0        0     2274 2024-05-30 19:55:10.648364 carbon_python_sdk-0.2.1/carbon/exceptions_base.py
--rw-r--r--   0        0        0      340 2024-05-30 19:55:10.648568 carbon_python_sdk-0.2.1/carbon/model/__init__.py
--rw-r--r--   0        0        0     2282 2024-05-30 19:55:10.648646 carbon_python_sdk-0.2.1/carbon/model/add_webhook_props.py
--rw-r--r--   0        0        0     2282 2024-05-30 19:55:10.648722 carbon_python_sdk-0.2.1/carbon/model/add_webhook_props.pyi
--rw-r--r--   0        0        0     2371 2024-05-30 19:55:10.648802 carbon_python_sdk-0.2.1/carbon/model/body_create_upload_file_uploadfile_post.py
--rw-r--r--   0        0        0     2371 2024-05-30 19:55:10.648879 carbon_python_sdk-0.2.1/carbon/model/body_create_upload_file_uploadfile_post.pyi
--rw-r--r--   0        0        0     4752 2024-05-30 19:55:10.648965 carbon_python_sdk-0.2.1/carbon/model/chunk_properties.py
--rw-r--r--   0        0        0     4752 2024-05-30 19:55:10.649050 carbon_python_sdk-0.2.1/carbon/model/chunk_properties.pyi
--rw-r--r--   0        0        0     4359 2024-05-30 19:55:10.649256 carbon_python_sdk-0.2.1/carbon/model/chunk_properties_nullable.py
--rw-r--r--   0        0        0     4359 2024-05-30 19:55:10.649342 carbon_python_sdk-0.2.1/carbon/model/chunk_properties_nullable.pyi
--rw-r--r--   0        0        0     4319 2024-05-30 19:55:10.649430 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings.py
--rw-r--r--   0        0        0     4319 2024-05-30 19:55:10.649513 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings.pyi
--rw-r--r--   0        0        0     1100 2024-05-30 19:55:10.649588 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_embedding.py
--rw-r--r--   0        0        0     1100 2024-05-30 19:55:10.649667 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_embedding.pyi
--rw-r--r--   0        0        0     6672 2024-05-30 19:55:10.649750 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0     6672 2024-05-30 19:55:10.649834 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input.pyi
--rw-r--r--   0        0        0     1521 2024-05-30 19:55:10.649914 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.py
--rw-r--r--   0        0        0     1521 2024-05-30 19:55:10.649997 carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.pyi
--rw-r--r--   0        0        0      548 2024-05-30 19:55:10.650072 carbon_python_sdk-0.2.1/carbon/model/configuration_keys.py
--rw-r--r--   0        0        0      548 2024-05-30 19:55:10.650148 carbon_python_sdk-0.2.1/carbon/model/configuration_keys.pyi
--rw-r--r--   0        0        0     4861 2024-05-30 19:55:10.650237 carbon_python_sdk-0.2.1/carbon/model/confluence_authentication.py
--rw-r--r--   0        0        0     4861 2024-05-30 19:55:10.650322 carbon_python_sdk-0.2.1/carbon/model/confluence_authentication.pyi
--rw-r--r--   0        0        0     6269 2024-05-30 19:55:10.650409 carbon_python_sdk-0.2.1/carbon/model/connect_data_source_input.py
--rw-r--r--   0        0        0     6269 2024-05-30 19:55:10.650494 carbon_python_sdk-0.2.1/carbon/model/connect_data_source_input.pyi
--rw-r--r--   0        0        0     3763 2024-05-30 19:55:10.650570 carbon_python_sdk-0.2.1/carbon/model/connect_data_source_response.py
--rw-r--r--   0        0        0     3763 2024-05-30 19:55:10.650647 carbon_python_sdk-0.2.1/carbon/model/connect_data_source_response.pyi
--rw-r--r--   0        0        0     1369 2024-05-30 19:55:10.650722 carbon_python_sdk-0.2.1/carbon/model/custom_credentials_type.py
--rw-r--r--   0        0        0     1114 2024-05-30 19:55:10.650799 carbon_python_sdk-0.2.1/carbon/model/custom_credentials_type.pyi
--rw-r--r--   0        0        0      554 2024-05-30 19:55:10.650872 carbon_python_sdk-0.2.1/carbon/model/data_source_extended_input.py
--rw-r--r--   0        0        0      554 2024-05-30 19:55:10.650947 carbon_python_sdk-0.2.1/carbon/model/data_source_extended_input.pyi
--rw-r--r--   0        0        0     1183 2024-05-30 19:55:10.651021 carbon_python_sdk-0.2.1/carbon/model/data_source_last_sync_actions.py
--rw-r--r--   0        0        0      998 2024-05-30 19:55:10.651099 carbon_python_sdk-0.2.1/carbon/model/data_source_last_sync_actions.pyi
--rw-r--r--   0        0        0     1256 2024-05-30 19:55:10.651174 carbon_python_sdk-0.2.1/carbon/model/data_source_sync_statuses.py
--rw-r--r--   0        0        0     1033 2024-05-30 19:55:10.651247 carbon_python_sdk-0.2.1/carbon/model/data_source_sync_statuses.pyi
--rw-r--r--   0        0        0     6578 2024-05-30 19:55:10.651329 carbon_python_sdk-0.2.1/carbon/model/data_source_type.py
--rw-r--r--   0        0        0     4915 2024-05-30 19:55:10.651414 carbon_python_sdk-0.2.1/carbon/model/data_source_type.pyi
--rw-r--r--   0        0        0     6953 2024-05-30 19:55:10.651500 carbon_python_sdk-0.2.1/carbon/model/data_source_type_nullable.py
--rw-r--r--   0        0        0     6953 2024-05-30 19:55:10.651584 carbon_python_sdk-0.2.1/carbon/model/data_source_type_nullable.pyi
--rw-r--r--   0        0        0     6047 2024-05-30 19:55:10.651668 carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input.py
--rw-r--r--   0        0        0     6047 2024-05-30 19:55:10.651756 carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input.pyi
--rw-r--r--   0        0        0     1097 2024-05-30 19:55:10.651835 carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input_file_ids.py
--rw-r--r--   0        0        0     1097 2024-05-30 19:55:10.651911 carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input_file_ids.pyi
--rw-r--r--   0        0        0     3161 2024-05-30 19:55:10.651985 carbon_python_sdk-0.2.1/carbon/model/delete_files_v2_query_input.py
--rw-r--r--   0        0        0     3161 2024-05-30 19:55:10.652059 carbon_python_sdk-0.2.1/carbon/model/delete_files_v2_query_input.pyi
--rw-r--r--   0        0        0     2600 2024-05-30 19:55:10.652134 carbon_python_sdk-0.2.1/carbon/model/delete_users_input.py
--rw-r--r--   0        0        0     2600 2024-05-30 19:55:10.652211 carbon_python_sdk-0.2.1/carbon/model/delete_users_input.pyi
--rw-r--r--   0        0        0     1199 2024-05-30 19:55:10.652286 carbon_python_sdk-0.2.1/carbon/model/delete_users_input_customer_ids.py
--rw-r--r--   0        0        0     1199 2024-05-30 19:55:10.652361 carbon_python_sdk-0.2.1/carbon/model/delete_users_input_customer_ids.pyi
--rw-r--r--   0        0        0     3902 2024-05-30 19:55:10.652435 carbon_python_sdk-0.2.1/carbon/model/directory_item.py
--rw-r--r--   0        0        0     3902 2024-05-30 19:55:10.652512 carbon_python_sdk-0.2.1/carbon/model/directory_item.pyi
--rw-r--r--   0        0        0    16065 2024-05-30 19:55:10.652593 carbon_python_sdk-0.2.1/carbon/model/document_response.py
--rw-r--r--   0        0        0    16065 2024-05-30 19:55:10.652824 carbon_python_sdk-0.2.1/carbon/model/document_response.pyi
--rw-r--r--   0        0        0     3350 2024-05-30 19:55:10.653034 carbon_python_sdk-0.2.1/carbon/model/document_response_list.py
--rw-r--r--   0        0        0     3350 2024-05-30 19:55:10.653118 carbon_python_sdk-0.2.1/carbon/model/document_response_list.pyi
--rw-r--r--   0        0        0     7489 2024-05-30 19:55:10.653217 carbon_python_sdk-0.2.1/carbon/model/document_response_tags.py
--rw-r--r--   0        0        0     7489 2024-05-30 19:55:10.653532 carbon_python_sdk-0.2.1/carbon/model/document_response_tags.pyi
--rw-r--r--   0        0        0     1088 2024-05-30 19:55:10.653728 carbon_python_sdk-0.2.1/carbon/model/document_response_vector.py
--rw-r--r--   0        0        0     1088 2024-05-30 19:55:10.653835 carbon_python_sdk-0.2.1/carbon/model/document_response_vector.pyi
--rw-r--r--   0        0        0     6594 2024-05-30 19:55:10.653948 carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk.py
--rw-r--r--   0        0        0     6594 2024-05-30 19:55:10.654057 carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk.pyi
--rw-r--r--   0        0        0     1096 2024-05-30 19:55:10.654159 carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk_embedding.py
--rw-r--r--   0        0        0     1096 2024-05-30 19:55:10.654257 carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk_embedding.pyi
--rw-r--r--   0        0        0     3163 2024-05-30 19:55:10.654362 carbon_python_sdk-0.2.1/carbon/model/embedding_generators.py
--rw-r--r--   0        0        0     2260 2024-05-30 19:55:10.654460 carbon_python_sdk-0.2.1/carbon/model/embedding_generators.pyi
--rw-r--r--   0        0        0     3543 2024-05-30 19:55:10.654564 carbon_python_sdk-0.2.1/carbon/model/embedding_generators_nullable.py
--rw-r--r--   0        0        0     3543 2024-05-30 19:55:10.654659 carbon_python_sdk-0.2.1/carbon/model/embedding_generators_nullable.pyi
--rw-r--r--   0        0        0     4307 2024-05-30 19:55:10.654765 carbon_python_sdk-0.2.1/carbon/model/embedding_properties.py
--rw-r--r--   0        0        0     4307 2024-05-30 19:55:10.654878 carbon_python_sdk-0.2.1/carbon/model/embedding_properties.pyi
--rw-r--r--   0        0        0     3267 2024-05-30 19:55:10.654977 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_filters.py
--rw-r--r--   0        0        0     3267 2024-05-30 19:55:10.655079 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_filters.pyi
--rw-r--r--   0        0        0     1141 2024-05-30 19:55:10.655176 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_order_by_columns.py
--rw-r--r--   0        0        0      956 2024-05-30 19:55:10.655294 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_order_by_columns.pyi
--rw-r--r--   0        0        0     5194 2024-05-30 19:55:10.655400 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_query_input.py
--rw-r--r--   0        0        0     5194 2024-05-30 19:55:10.655496 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_query_input.pyi
--rw-r--r--   0        0        0     3847 2024-05-30 19:55:10.655592 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_response.py
--rw-r--r--   0        0        0     3847 2024-05-30 19:55:10.655697 carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_response.pyi
--rw-r--r--   0        0        0     1944 2024-05-30 19:55:10.655789 carbon_python_sdk-0.2.1/carbon/model/external_file_sync_statuses.py
--rw-r--r--   0        0        0     1503 2024-05-30 19:55:10.655883 carbon_python_sdk-0.2.1/carbon/model/external_file_sync_statuses.pyi
--rw-r--r--   0        0        0    17950 2024-05-30 19:55:10.655984 carbon_python_sdk-0.2.1/carbon/model/external_source_item.py
--rw-r--r--   0        0        0    17950 2024-05-30 19:55:10.656098 carbon_python_sdk-0.2.1/carbon/model/external_source_item.pyi
--rw-r--r--   0        0        0     1102 2024-05-30 19:55:10.656204 carbon_python_sdk-0.2.1/carbon/model/external_source_items_order_by.py
--rw-r--r--   0        0        0      933 2024-05-30 19:55:10.656297 carbon_python_sdk-0.2.1/carbon/model/external_source_items_order_by.pyi
--rw-r--r--   0        0        0     4287 2024-05-30 19:55:10.656396 carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response.py
--rw-r--r--   0        0        0     4287 2024-05-30 19:55:10.656485 carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response.pyi
--rw-r--r--   0        0        0     1187 2024-05-30 19:55:10.656569 carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response_urls.py
--rw-r--r--   0        0        0     1187 2024-05-30 19:55:10.656654 carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response_urls.pyi
--rw-r--r--   0        0        0     1166 2024-05-30 19:55:10.656733 carbon_python_sdk-0.2.1/carbon/model/file_content_types.py
--rw-r--r--   0        0        0      985 2024-05-30 19:55:10.656808 carbon_python_sdk-0.2.1/carbon/model/file_content_types.pyi
--rw-r--r--   0        0        0     1926 2024-05-30 19:55:10.656885 carbon_python_sdk-0.2.1/carbon/model/file_content_types_nullable.py
--rw-r--r--   0        0        0     1926 2024-05-30 19:55:10.656973 carbon_python_sdk-0.2.1/carbon/model/file_content_types_nullable.pyi
--rw-r--r--   0        0        0     5789 2024-05-30 19:55:10.657063 carbon_python_sdk-0.2.1/carbon/model/file_formats.py
--rw-r--r--   0        0        0     4344 2024-05-30 19:55:10.657150 carbon_python_sdk-0.2.1/carbon/model/file_formats.pyi
--rw-r--r--   0        0        0     6161 2024-05-30 19:55:10.657240 carbon_python_sdk-0.2.1/carbon/model/file_formats_nullable.py
--rw-r--r--   0        0        0     6161 2024-05-30 19:55:10.657328 carbon_python_sdk-0.2.1/carbon/model/file_formats_nullable.pyi
--rw-r--r--   0        0        0     8647 2024-05-30 19:55:10.657413 carbon_python_sdk-0.2.1/carbon/model/file_statistics.py
--rw-r--r--   0        0        0     8647 2024-05-30 19:55:10.657559 carbon_python_sdk-0.2.1/carbon/model/file_statistics.pyi
--rw-r--r--   0        0        0     8000 2024-05-30 19:55:10.657704 carbon_python_sdk-0.2.1/carbon/model/file_statistics_nullable.py
--rw-r--r--   0        0        0     8000 2024-05-30 19:55:10.657794 carbon_python_sdk-0.2.1/carbon/model/file_statistics_nullable.pyi
--rw-r--r--   0        0        0     4847 2024-05-30 19:55:10.657887 carbon_python_sdk-0.2.1/carbon/model/file_sync_config.py
--rw-r--r--   0        0        0     4847 2024-05-30 19:55:10.657977 carbon_python_sdk-0.2.1/carbon/model/file_sync_config.pyi
--rw-r--r--   0        0        0     5047 2024-05-30 19:55:10.658070 carbon_python_sdk-0.2.1/carbon/model/file_sync_config_nullable.py
--rw-r--r--   0        0        0     5047 2024-05-30 19:55:10.658162 carbon_python_sdk-0.2.1/carbon/model/file_sync_config_nullable.pyi
--rw-r--r--   0        0        0     1283 2024-05-30 19:55:10.658246 carbon_python_sdk-0.2.1/carbon/model/files_query_user_files_deprecated_response.py
--rw-r--r--   0        0        0     1283 2024-05-30 19:55:10.658337 carbon_python_sdk-0.2.1/carbon/model/files_query_user_files_deprecated_response.pyi
--rw-r--r--   0        0        0    15514 2024-05-30 19:55:10.658422 carbon_python_sdk-0.2.1/carbon/model/fresh_desk_connect_request.py
--rw-r--r--   0        0        0    15514 2024-05-30 19:55:10.658648 carbon_python_sdk-0.2.1/carbon/model/fresh_desk_connect_request.pyi
--rw-r--r--   0        0        0     3529 2024-05-30 19:55:10.658860 carbon_python_sdk-0.2.1/carbon/model/freskdesk_authentication.py
--rw-r--r--   0        0        0     3529 2024-05-30 19:55:10.658949 carbon_python_sdk-0.2.1/carbon/model/freskdesk_authentication.pyi
--rw-r--r--   0        0        0     2362 2024-05-30 19:55:10.659032 carbon_python_sdk-0.2.1/carbon/model/generic_success_response.py
--rw-r--r--   0        0        0     2362 2024-05-30 19:55:10.659109 carbon_python_sdk-0.2.1/carbon/model/generic_success_response.pyi
--rw-r--r--   0        0        0    15782 2024-05-30 19:55:10.659195 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body.py
--rw-r--r--   0        0        0    15631 2024-05-30 19:55:10.659611 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body.pyi
--rw-r--r--   0        0        0     1159 2024-05-30 19:55:10.660004 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_file_ids.py
--rw-r--r--   0        0        0     1159 2024-05-30 19:55:10.660104 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_file_ids.pyi
--rw-r--r--   0        0        0     1264 2024-05-30 19:55:10.660210 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_parent_file_ids.py
--rw-r--r--   0        0        0     1264 2024-05-30 19:55:10.660304 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_parent_file_ids.pyi
--rw-r--r--   0        0        0     1377 2024-05-30 19:55:10.660400 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_query_vector.py
--rw-r--r--   0        0        0     1377 2024-05-30 19:55:10.660498 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_query_vector.pyi
--rw-r--r--   0        0        0     6490 2024-05-30 19:55:10.660598 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_tags.py
--rw-r--r--   0        0        0     6490 2024-05-30 19:55:10.660702 carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_tags.pyi
--rw-r--r--   0        0        0     3779 2024-05-30 19:55:10.660795 carbon_python_sdk-0.2.1/carbon/model/gitbook_authetication.py
--rw-r--r--   0        0        0     3779 2024-05-30 19:55:10.660885 carbon_python_sdk-0.2.1/carbon/model/gitbook_authetication.pyi
--rw-r--r--   0        0        0    14852 2024-05-30 19:55:10.660977 carbon_python_sdk-0.2.1/carbon/model/gitbook_connect_request.py
--rw-r--r--   0        0        0    14852 2024-05-30 19:55:10.661208 carbon_python_sdk-0.2.1/carbon/model/gitbook_connect_request.pyi
--rw-r--r--   0        0        0    13012 2024-05-30 19:55:10.661449 carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request.py
--rw-r--r--   0        0        0    13012 2024-05-30 19:55:10.661830 carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request.pyi
--rw-r--r--   0        0        0     1220 2024-05-30 19:55:10.662054 carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request_space_ids.py
--rw-r--r--   0        0        0     1197 2024-05-30 19:55:10.662150 carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request_space_ids.pyi
--rw-r--r--   0        0        0     3635 2024-05-30 19:55:10.662253 carbon_python_sdk-0.2.1/carbon/model/github_authentication.py
--rw-r--r--   0        0        0     3635 2024-05-30 19:55:10.662355 carbon_python_sdk-0.2.1/carbon/model/github_authentication.pyi
--rw-r--r--   0        0        0     3626 2024-05-30 19:55:10.662451 carbon_python_sdk-0.2.1/carbon/model/github_connect_request.py
--rw-r--r--   0        0        0     3626 2024-05-30 19:55:10.662549 carbon_python_sdk-0.2.1/carbon/model/github_connect_request.pyi
--rw-r--r--   0        0        0     3792 2024-05-30 19:55:10.662653 carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request.py
--rw-r--r--   0        0        0     3792 2024-05-30 19:55:10.662756 carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request.pyi
--rw-r--r--   0        0        0     1246 2024-05-30 19:55:10.662987 carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request_repos.py
--rw-r--r--   0        0        0     1201 2024-05-30 19:55:10.663108 carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request_repos.pyi
--rw-r--r--   0        0        0    16085 2024-05-30 19:55:10.663216 carbon_python_sdk-0.2.1/carbon/model/gmail_sync_input.py
--rw-r--r--   0        0        0    16085 2024-05-30 19:55:10.663455 carbon_python_sdk-0.2.1/carbon/model/gmail_sync_input.pyi
--rw-r--r--   0        0        0      963 2024-05-30 19:55:10.663691 carbon_python_sdk-0.2.1/carbon/model/helpdesk_file_types.py
--rw-r--r--   0        0        0      834 2024-05-30 19:55:10.663787 carbon_python_sdk-0.2.1/carbon/model/helpdesk_file_types.pyi
--rw-r--r--   0        0        0     3251 2024-05-30 19:55:10.663886 carbon_python_sdk-0.2.1/carbon/model/http_validation_error.py
--rw-r--r--   0        0        0     3251 2024-05-30 19:55:10.663982 carbon_python_sdk-0.2.1/carbon/model/http_validation_error.pyi
--rw-r--r--   0        0        0     2974 2024-05-30 19:55:10.664086 carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params.py
--rw-r--r--   0        0        0     2974 2024-05-30 19:55:10.664184 carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params.pyi
--rw-r--r--   0        0        0     2907 2024-05-30 19:55:10.664286 carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params_nullable.py
--rw-r--r--   0        0        0     2907 2024-05-30 19:55:10.664385 carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params_nullable.pyi
--rw-r--r--   0        0        0     6323 2024-05-30 19:55:10.664491 carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_request.py
--rw-r--r--   0        0        0     6323 2024-05-30 19:55:10.664600 carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_request.pyi
--rw-r--r--   0        0        0     3820 2024-05-30 19:55:10.664697 carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_response.py
--rw-r--r--   0        0        0     3820 2024-05-30 19:55:10.664793 carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_response.pyi
--rw-r--r--   0        0        0     5498 2024-05-30 19:55:10.664900 carbon_python_sdk-0.2.1/carbon/model/list_items_filters.py
--rw-r--r--   0        0        0     5498 2024-05-30 19:55:10.665003 carbon_python_sdk-0.2.1/carbon/model/list_items_filters.pyi
--rw-r--r--   0        0        0     1095 2024-05-30 19:55:10.665102 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_external_ids.py
--rw-r--r--   0        0        0     1095 2024-05-30 19:55:10.665198 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_external_ids.pyi
--rw-r--r--   0        0        0     1079 2024-05-30 19:55:10.665291 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_ids.py
--rw-r--r--   0        0        0     1079 2024-05-30 19:55:10.665392 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_ids.pyi
--rw-r--r--   0        0        0     5708 2024-05-30 19:55:10.665498 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable.py
--rw-r--r--   0        0        0     5708 2024-05-30 19:55:10.665603 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable.pyi
--rw-r--r--   0        0        0     1111 2024-05-30 19:55:10.665690 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_external_ids.py
--rw-r--r--   0        0        0     1111 2024-05-30 19:55:10.665785 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_external_ids.pyi
--rw-r--r--   0        0        0     1095 2024-05-30 19:55:10.665876 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_ids.py
--rw-r--r--   0        0        0     1095 2024-05-30 19:55:10.665957 carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_ids.pyi
--rw-r--r--   0        0        0     3613 2024-05-30 19:55:10.666037 carbon_python_sdk-0.2.1/carbon/model/list_request.py
--rw-r--r--   0        0        0     3613 2024-05-30 19:55:10.666117 carbon_python_sdk-0.2.1/carbon/model/list_request.pyi
--rw-r--r--   0        0        0     3228 2024-05-30 19:55:10.666200 carbon_python_sdk-0.2.1/carbon/model/list_response.py
--rw-r--r--   0        0        0     3228 2024-05-30 19:55:10.666284 carbon_python_sdk-0.2.1/carbon/model/list_response.pyi
--rw-r--r--   0        0        0     3129 2024-05-30 19:55:10.666466 carbon_python_sdk-0.2.1/carbon/model/modify_user_configuration_input.py
--rw-r--r--   0        0        0     3129 2024-05-30 19:55:10.666580 carbon_python_sdk-0.2.1/carbon/model/modify_user_configuration_input.pyi
--rw-r--r--   0        0        0      560 2024-05-30 19:57:32.276931 carbon_python_sdk-0.2.1/carbon/model/multi_modal_embedding_generators.py
--rw-r--r--   0        0        0      560 2024-05-30 19:57:32.277033 carbon_python_sdk-0.2.1/carbon/model/multi_modal_embedding_generators.pyi
--rw-r--r--   0        0        0     3699 2024-05-30 19:55:10.666853 carbon_python_sdk-0.2.1/carbon/model/notion_authentication.py
--rw-r--r--   0        0        0     3699 2024-05-30 19:55:10.666933 carbon_python_sdk-0.2.1/carbon/model/notion_authentication.pyi
--rw-r--r--   0        0        0     4300 2024-05-30 19:55:10.667026 carbon_python_sdk-0.2.1/carbon/model/o_auth_authentication.py
--rw-r--r--   0        0        0     4300 2024-05-30 19:55:10.667119 carbon_python_sdk-0.2.1/carbon/model/o_auth_authentication.pyi
--rw-r--r--   0        0        0    29598 2024-05-30 19:55:10.667218 carbon_python_sdk-0.2.1/carbon/model/o_auth_url_request.py
--rw-r--r--   0        0        0    29598 2024-05-30 19:55:10.667346 carbon_python_sdk-0.2.1/carbon/model/o_auth_url_request.pyi
--rw-r--r--   0        0        0      930 2024-05-30 19:55:10.667437 carbon_python_sdk-0.2.1/carbon/model/order_dir.py
--rw-r--r--   0        0        0      813 2024-05-30 19:55:10.667515 carbon_python_sdk-0.2.1/carbon/model/order_dir.pyi
--rw-r--r--   0        0        0      932 2024-05-30 19:55:10.667596 carbon_python_sdk-0.2.1/carbon/model/order_dir_v2.py
--rw-r--r--   0        0        0      815 2024-05-30 19:55:10.667673 carbon_python_sdk-0.2.1/carbon/model/order_dir_v2.pyi
--rw-r--r--   0        0        0    18921 2024-05-30 19:55:10.667758 carbon_python_sdk-0.2.1/carbon/model/organization_response.py
--rw-r--r--   0        0        0    18921 2024-05-30 19:55:10.667858 carbon_python_sdk-0.2.1/carbon/model/organization_response.pyi
--rw-r--r--   0        0        0    17065 2024-05-30 19:55:10.667967 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_api.py
--rw-r--r--   0        0        0    17065 2024-05-30 19:55:10.668074 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_api.pyi
--rw-r--r--   0        0        0     4467 2024-05-30 19:55:10.668181 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters.py
--rw-r--r--   0        0        0     4467 2024-05-30 19:55:10.668283 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters.pyi
--rw-r--r--   0        0        0     1113 2024-05-30 19:55:10.668373 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters_ids.py
--rw-r--r--   0        0        0     1113 2024-05-30 19:55:10.668461 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters_ids.pyi
--rw-r--r--   0        0        0     1014 2024-05-30 19:55:10.668550 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_order_by_columns.py
--rw-r--r--   0        0        0      871 2024-05-30 19:55:10.668632 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_order_by_columns.pyi
--rw-r--r--   0        0        0     4657 2024-05-30 19:55:10.668724 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_query_input.py
--rw-r--r--   0        0        0     4657 2024-05-30 19:55:10.668816 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_query_input.pyi
--rw-r--r--   0        0        0     3947 2024-05-30 19:55:10.668899 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_response.py
--rw-r--r--   0        0        0     3947 2024-05-30 19:55:10.668980 carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_response.pyi
--rw-r--r--   0        0        0     3408 2024-05-30 19:55:10.669059 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create.py
--rw-r--r--   0        0        0     3408 2024-05-30 19:55:10.669138 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create.pyi
--rw-r--r--   0        0        0     6330 2024-05-30 19:55:10.669244 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create_tags.py
--rw-r--r--   0        0        0     6330 2024-05-30 19:55:10.669340 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create_tags.pyi
--rw-r--r--   0        0        0     3418 2024-05-30 19:55:10.669421 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove.py
--rw-r--r--   0        0        0     3418 2024-05-30 19:55:10.669505 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove.pyi
--rw-r--r--   0        0        0     1213 2024-05-30 19:55:10.669589 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove_tags.py
--rw-r--r--   0        0        0     1213 2024-05-30 19:55:10.669673 carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove_tags.pyi
--rw-r--r--   0        0        0    21692 2024-05-30 19:55:10.669764 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters.py
--rw-r--r--   0        0        0    21692 2024-05-30 19:55:10.669866 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters.pyi
--rw-r--r--   0        0        0     1238 2024-05-30 19:55:10.669961 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_external_file_ids.py
--rw-r--r--   0        0        0     1238 2024-05-30 19:55:10.670057 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_external_file_ids.pyi
--rw-r--r--   0        0        0     1186 2024-05-30 19:55:10.670149 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_ids.py
--rw-r--r--   0        0        0     1186 2024-05-30 19:55:10.670244 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_ids.pyi
--rw-r--r--   0        0        0     1296 2024-05-30 19:55:10.670497 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.py
--rw-r--r--   0        0        0     1296 2024-05-30 19:55:10.670608 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.pyi
--rw-r--r--   0        0        0     1135 2024-05-30 19:55:10.670705 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.py
--rw-r--r--   0        0        0     1135 2024-05-30 19:55:10.670798 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.pyi
--rw-r--r--   0        0        0     1216 2024-05-30 19:55:10.670893 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_request_ids.py
--rw-r--r--   0        0        0     1192 2024-05-30 19:55:10.670982 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_request_ids.pyi
--rw-r--r--   0        0        0     6420 2024-05-30 19:55:10.671075 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_tags.py
--rw-r--r--   0        0        0     6420 2024-05-30 19:55:10.671174 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_tags.pyi
--rw-r--r--   0        0        0     1469 2024-05-30 19:55:10.671390 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_order_by_types.py
--rw-r--r--   0        0        0     1198 2024-05-30 19:55:10.671492 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_order_by_types.pyi
--rw-r--r--   0        0        0     8629 2024-05-30 19:55:10.671586 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_query_input.py
--rw-r--r--   0        0        0     8629 2024-05-30 19:55:10.671738 carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_query_input.pyi
--rw-r--r--   0        0        0     2378 2024-05-30 19:55:10.671879 carbon_python_sdk-0.2.1/carbon/model/outh_url_response.py
--rw-r--r--   0        0        0     2378 2024-05-30 19:55:10.671973 carbon_python_sdk-0.2.1/carbon/model/outh_url_response.pyi
--rw-r--r--   0        0        0    17193 2024-05-30 19:55:10.672075 carbon_python_sdk-0.2.1/carbon/model/outlook_sync_input.py
--rw-r--r--   0        0        0    17193 2024-05-30 19:55:10.672467 carbon_python_sdk-0.2.1/carbon/model/outlook_sync_input.pyi
--rw-r--r--   0        0        0     2807 2024-05-30 19:55:10.672569 carbon_python_sdk-0.2.1/carbon/model/pagination.py
--rw-r--r--   0        0        0     2807 2024-05-30 19:55:10.672767 carbon_python_sdk-0.2.1/carbon/model/pagination.pyi
--rw-r--r--   0        0        0     2452 2024-05-30 19:55:10.672853 carbon_python_sdk-0.2.1/carbon/model/presigned_url_response.py
--rw-r--r--   0        0        0     2452 2024-05-30 19:55:10.672932 carbon_python_sdk-0.2.1/carbon/model/presigned_url_response.pyi
--rw-r--r--   0        0        0    10223 2024-05-30 19:55:10.673010 carbon_python_sdk-0.2.1/carbon/model/raw_text_input.py
--rw-r--r--   0        0        0    10151 2024-05-30 19:55:10.673141 carbon_python_sdk-0.2.1/carbon/model/raw_text_input.pyi
--rw-r--r--   0        0        0     5578 2024-05-30 19:55:10.673283 carbon_python_sdk-0.2.1/carbon/model/resync_file_query_input.py
--rw-r--r--   0        0        0     5578 2024-05-30 19:55:10.673376 carbon_python_sdk-0.2.1/carbon/model/resync_file_query_input.pyi
--rw-r--r--   0        0        0     2489 2024-05-30 19:55:10.673455 carbon_python_sdk-0.2.1/carbon/model/revoke_access_token_input.py
--rw-r--r--   0        0        0     2489 2024-05-30 19:55:10.673537 carbon_python_sdk-0.2.1/carbon/model/revoke_access_token_input.pyi
--rw-r--r--   0        0        0    12076 2024-05-30 19:55:10.673614 carbon_python_sdk-0.2.1/carbon/model/rss_feed_input.py
--rw-r--r--   0        0        0    12076 2024-05-30 19:55:10.673746 carbon_python_sdk-0.2.1/carbon/model/rss_feed_input.pyi
--rw-r--r--   0        0        0     3724 2024-05-30 19:55:10.673876 carbon_python_sdk-0.2.1/carbon/model/s3_auth_request.py
--rw-r--r--   0        0        0     3724 2024-05-30 19:55:10.674059 carbon_python_sdk-0.2.1/carbon/model/s3_auth_request.pyi
--rw-r--r--   0        0        0     3739 2024-05-30 19:55:10.674136 carbon_python_sdk-0.2.1/carbon/model/s3_authentication.py
--rw-r--r--   0        0        0     3739 2024-05-30 19:55:10.674222 carbon_python_sdk-0.2.1/carbon/model/s3_authentication.pyi
--rw-r--r--   0        0        0    19565 2024-05-30 19:55:10.674310 carbon_python_sdk-0.2.1/carbon/model/s3_file_sync_input.py
--rw-r--r--   0        0        0    19565 2024-05-30 19:55:10.674406 carbon_python_sdk-0.2.1/carbon/model/s3_file_sync_input.pyi
--rw-r--r--   0        0        0     3936 2024-05-30 19:55:10.674492 carbon_python_sdk-0.2.1/carbon/model/s3_get_file_input.py
--rw-r--r--   0        0        0     3936 2024-05-30 19:55:10.674568 carbon_python_sdk-0.2.1/carbon/model/s3_get_file_input.pyi
--rw-r--r--   0        0        0     4813 2024-05-30 19:55:10.674656 carbon_python_sdk-0.2.1/carbon/model/salesforce_authentication.py
--rw-r--r--   0        0        0     4813 2024-05-30 19:55:10.674744 carbon_python_sdk-0.2.1/carbon/model/salesforce_authentication.pyi
--rw-r--r--   0        0        0     5449 2024-05-30 19:55:10.674829 carbon_python_sdk-0.2.1/carbon/model/sharepoint_authentication.py
--rw-r--r--   0        0        0     5449 2024-05-30 19:55:10.674916 carbon_python_sdk-0.2.1/carbon/model/sharepoint_authentication.pyi
--rw-r--r--   0        0        0     1566 2024-05-30 19:55:10.675002 carbon_python_sdk-0.2.1/carbon/model/simple_o_auth_data_sources.py
--rw-r--r--   0        0        0     1263 2024-05-30 19:55:10.675082 carbon_python_sdk-0.2.1/carbon/model/simple_o_auth_data_sources.pyi
--rw-r--r--   0        0        0     6587 2024-05-30 19:55:10.675172 carbon_python_sdk-0.2.1/carbon/model/single_chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0     6587 2024-05-30 19:55:10.675269 carbon_python_sdk-0.2.1/carbon/model/single_chunks_and_embeddings_upload_input.pyi
--rw-r--r--   0        0        0    15650 2024-05-30 19:55:10.675348 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request.py
--rw-r--r--   0        0        0    15608 2024-05-30 19:55:10.675568 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request.pyi
--rw-r--r--   0        0        0     1113 2024-05-30 19:55:10.676392 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0     1113 2024-05-30 19:55:10.676479 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_classes_to_skip.pyi
--rw-r--r--   0        0        0     1117 2024-05-30 19:55:10.676562 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0     1117 2024-05-30 19:55:10.676647 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_selectors_to_skip.pyi
--rw-r--r--   0        0        0     1109 2024-05-30 19:55:10.676727 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0     1109 2024-05-30 19:55:10.676807 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_html_tags_to_skip.pyi
--rw-r--r--   0        0        0     6392 2024-05-30 19:55:10.676896 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_tags.py
--rw-r--r--   0        0        0     6392 2024-05-30 19:55:10.676989 carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_tags.pyi
--rw-r--r--   0        0        0     2485 2024-05-30 19:55:10.677069 carbon_python_sdk-0.2.1/carbon/model/sync_directory_request.py
--rw-r--r--   0        0        0     2485 2024-05-30 19:55:10.677155 carbon_python_sdk-0.2.1/carbon/model/sync_directory_request.pyi
--rw-r--r--   0        0        0     2784 2024-05-30 19:55:10.677232 carbon_python_sdk-0.2.1/carbon/model/sync_files_ids.py
--rw-r--r--   0        0        0     2784 2024-05-30 19:55:10.677309 carbon_python_sdk-0.2.1/carbon/model/sync_files_ids.pyi
--rw-r--r--   0        0        0    22189 2024-05-30 19:55:10.677396 carbon_python_sdk-0.2.1/carbon/model/sync_files_request.py
--rw-r--r--   0        0        0    22189 2024-05-30 19:55:10.677492 carbon_python_sdk-0.2.1/carbon/model/sync_files_request.pyi
--rw-r--r--   0        0        0    16413 2024-05-30 19:55:10.677586 carbon_python_sdk-0.2.1/carbon/model/sync_options.py
--rw-r--r--   0        0        0    16413 2024-05-30 19:55:10.677679 carbon_python_sdk-0.2.1/carbon/model/sync_options.pyi
--rw-r--r--   0        0        0     3009 2024-05-30 19:55:10.677765 carbon_python_sdk-0.2.1/carbon/model/text_embedding_generators.py
--rw-r--r--   0        0        0     2160 2024-05-30 19:55:10.677846 carbon_python_sdk-0.2.1/carbon/model/text_embedding_generators.pyi
--rw-r--r--   0        0        0     3042 2024-05-30 19:55:10.677926 carbon_python_sdk-0.2.1/carbon/model/token_response.py
--rw-r--r--   0        0        0     3042 2024-05-30 19:55:10.678008 carbon_python_sdk-0.2.1/carbon/model/token_response.pyi
--rw-r--r--   0        0        0     2620 2024-05-30 19:55:10.678085 carbon_python_sdk-0.2.1/carbon/model/update_organization_input.py
--rw-r--r--   0        0        0     2620 2024-05-30 19:55:10.678165 carbon_python_sdk-0.2.1/carbon/model/update_organization_input.pyi
--rw-r--r--   0        0        0     9214 2024-05-30 19:55:10.678249 carbon_python_sdk-0.2.1/carbon/model/update_users_input.py
--rw-r--r--   0        0        0     9128 2024-05-30 19:55:10.678384 carbon_python_sdk-0.2.1/carbon/model/update_users_input.pyi
--rw-r--r--   0        0        0     1267 2024-05-30 19:55:10.678526 carbon_python_sdk-0.2.1/carbon/model/update_users_input_customer_ids.py
--rw-r--r--   0        0        0     1243 2024-05-30 19:55:10.678815 carbon_python_sdk-0.2.1/carbon/model/update_users_input_customer_ids.pyi
--rw-r--r--   0        0        0    12928 2024-05-30 19:55:10.678905 carbon_python_sdk-0.2.1/carbon/model/upload_file_from_url_input.py
--rw-r--r--   0        0        0    12928 2024-05-30 19:55:10.679123 carbon_python_sdk-0.2.1/carbon/model/upload_file_from_url_input.pyi
--rw-r--r--   0        0        0     8405 2024-05-30 19:55:10.679342 carbon_python_sdk-0.2.1/carbon/model/user_configuration.py
--rw-r--r--   0        0        0     8319 2024-05-30 19:55:10.679633 carbon_python_sdk-0.2.1/carbon/model/user_configuration.pyi
--rw-r--r--   0        0        0     8665 2024-05-30 19:55:10.679916 carbon_python_sdk-0.2.1/carbon/model/user_configuration_nullable.py
--rw-r--r--   0        0        0     8579 2024-05-30 19:55:10.680045 carbon_python_sdk-0.2.1/carbon/model/user_configuration_nullable.pyi
--rw-r--r--   0        0        0    35549 2024-05-30 19:55:10.680194 carbon_python_sdk-0.2.1/carbon/model/user_file.py
--rw-r--r--   0        0        0    35549 2024-05-30 19:55:10.680300 carbon_python_sdk-0.2.1/carbon/model/user_file.pyi
--rw-r--r--   0        0        0     1650 2024-05-30 19:55:10.680390 carbon_python_sdk-0.2.1/carbon/model/user_file_embedding_properties.py
--rw-r--r--   0        0        0     1650 2024-05-30 19:55:10.680469 carbon_python_sdk-0.2.1/carbon/model/user_file_embedding_properties.pyi
--rw-r--r--   0        0        0     3751 2024-05-30 19:55:10.680549 carbon_python_sdk-0.2.1/carbon/model/user_files_v2.py
--rw-r--r--   0        0        0     3751 2024-05-30 19:55:10.680625 carbon_python_sdk-0.2.1/carbon/model/user_files_v2.pyi
--rw-r--r--   0        0        0     2416 2024-05-30 19:55:10.680704 carbon_python_sdk-0.2.1/carbon/model/user_request_content.py
--rw-r--r--   0        0        0     2416 2024-05-30 19:55:10.680934 carbon_python_sdk-0.2.1/carbon/model/user_request_content.pyi
--rw-r--r--   0        0        0    17500 2024-05-30 19:55:10.681021 carbon_python_sdk-0.2.1/carbon/model/user_response.py
--rw-r--r--   0        0        0    17500 2024-05-30 19:55:10.681140 carbon_python_sdk-0.2.1/carbon/model/user_response.pyi
--rw-r--r--   0        0        0     1511 2024-05-30 19:55:10.681232 carbon_python_sdk-0.2.1/carbon/model/user_response_auto_sync_enabled_sources.py
--rw-r--r--   0        0        0     1511 2024-05-30 19:55:10.681311 carbon_python_sdk-0.2.1/carbon/model/user_response_auto_sync_enabled_sources.pyi
--rw-r--r--   0        0        0     1246 2024-05-30 19:55:10.681392 carbon_python_sdk-0.2.1/carbon/model/user_response_unique_file_tags.py
--rw-r--r--   0        0        0     1246 2024-05-30 19:55:10.681475 carbon_python_sdk-0.2.1/carbon/model/user_response_unique_file_tags.pyi
--rw-r--r--   0        0        0     1315 2024-05-30 19:55:10.681559 carbon_python_sdk-0.2.1/carbon/model/utilities_scrape_web_request.py
--rw-r--r--   0        0        0     1315 2024-05-30 19:55:10.681642 carbon_python_sdk-0.2.1/carbon/model/utilities_scrape_web_request.pyi
--rw-r--r--   0        0        0     3352 2024-05-30 19:55:10.681722 carbon_python_sdk-0.2.1/carbon/model/validation_error.py
--rw-r--r--   0        0        0     3352 2024-05-30 19:55:10.681802 carbon_python_sdk-0.2.1/carbon/model/validation_error.pyi
--rw-r--r--   0        0        0     3149 2024-05-30 19:55:10.681883 carbon_python_sdk-0.2.1/carbon/model/validation_error_loc.py
--rw-r--r--   0        0        0     3149 2024-05-30 19:55:10.681963 carbon_python_sdk-0.2.1/carbon/model/validation_error_loc.pyi
--rw-r--r--   0        0        0     6973 2024-05-30 19:55:10.682051 carbon_python_sdk-0.2.1/carbon/model/webhook.py
--rw-r--r--   0        0        0     6973 2024-05-30 19:55:10.682143 carbon_python_sdk-0.2.1/carbon/model/webhook.pyi
--rw-r--r--   0        0        0     2396 2024-05-30 19:55:10.682229 carbon_python_sdk-0.2.1/carbon/model/webhook_filters.py
--rw-r--r--   0        0        0     2396 2024-05-30 19:55:10.682460 carbon_python_sdk-0.2.1/carbon/model/webhook_filters.pyi
--rw-r--r--   0        0        0     1075 2024-05-30 19:55:10.682542 carbon_python_sdk-0.2.1/carbon/model/webhook_filters_ids.py
--rw-r--r--   0        0        0     1075 2024-05-30 19:55:10.682619 carbon_python_sdk-0.2.1/carbon/model/webhook_filters_ids.pyi
--rw-r--r--   0        0        0     6395 2024-05-30 19:55:10.682704 carbon_python_sdk-0.2.1/carbon/model/webhook_no_key.py
--rw-r--r--   0        0        0     6395 2024-05-30 19:55:10.682788 carbon_python_sdk-0.2.1/carbon/model/webhook_no_key.pyi
--rw-r--r--   0        0        0      995 2024-05-30 19:55:10.682868 carbon_python_sdk-0.2.1/carbon/model/webhook_order_by_columns.py
--rw-r--r--   0        0        0      852 2024-05-30 19:55:10.682943 carbon_python_sdk-0.2.1/carbon/model/webhook_order_by_columns.pyi
--rw-r--r--   0        0        0     4347 2024-05-30 19:55:10.683030 carbon_python_sdk-0.2.1/carbon/model/webhook_query_input.py
--rw-r--r--   0        0        0     4347 2024-05-30 19:55:10.683121 carbon_python_sdk-0.2.1/carbon/model/webhook_query_input.pyi
--rw-r--r--   0        0        0     3798 2024-05-30 19:55:10.683207 carbon_python_sdk-0.2.1/carbon/model/webhook_query_response.py
--rw-r--r--   0        0        0     3798 2024-05-30 19:55:10.683287 carbon_python_sdk-0.2.1/carbon/model/webhook_query_response.pyi
--rw-r--r--   0        0        0      959 2024-05-30 19:55:10.683367 carbon_python_sdk-0.2.1/carbon/model/webhook_status.py
--rw-r--r--   0        0        0      830 2024-05-30 19:55:10.683445 carbon_python_sdk-0.2.1/carbon/model/webhook_status.pyi
--rw-r--r--   0        0        0    16894 2024-05-30 19:55:10.683532 carbon_python_sdk-0.2.1/carbon/model/webscrape_request.py
--rw-r--r--   0        0        0    16810 2024-05-30 19:55:10.683644 carbon_python_sdk-0.2.1/carbon/model/webscrape_request.pyi
--rw-r--r--   0        0        0     1105 2024-05-30 19:55:10.683738 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0     1105 2024-05-30 19:55:10.683820 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_classes_to_skip.pyi
--rw-r--r--   0        0        0     1109 2024-05-30 19:55:10.683902 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0     1109 2024-05-30 19:55:10.683983 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_selectors_to_skip.pyi
--rw-r--r--   0        0        0     1101 2024-05-30 19:55:10.684184 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0     1101 2024-05-30 19:55:10.684380 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_html_tags_to_skip.pyi
--rw-r--r--   0        0        0     6384 2024-05-30 19:55:10.684576 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_tags.py
--rw-r--r--   0        0        0     6384 2024-05-30 19:55:10.684677 carbon_python_sdk-0.2.1/carbon/model/webscrape_request_tags.pyi
--rw-r--r--   0        0        0     3117 2024-05-30 19:55:10.684770 carbon_python_sdk-0.2.1/carbon/model/white_labeling_response.py
--rw-r--r--   0        0        0     3117 2024-05-30 19:55:10.684866 carbon_python_sdk-0.2.1/carbon/model/white_labeling_response.pyi
--rw-r--r--   0        0        0     5401 2024-05-30 19:55:10.684969 carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response.py
--rw-r--r--   0        0        0     5401 2024-05-30 19:55:10.685075 carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response.pyi
--rw-r--r--   0        0        0     1375 2024-05-30 19:55:10.685172 carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript.py
--rw-r--r--   0        0        0     1375 2024-05-30 19:55:10.685274 carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript.pyi
--rw-r--r--   0        0        0     3326 2024-05-30 19:55:10.685374 carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript_item.py
--rw-r--r--   0        0        0     3326 2024-05-30 19:55:10.685594 carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript_item.pyi
--rw-r--r--   0        0        0     3653 2024-05-30 19:55:10.685809 carbon_python_sdk-0.2.1/carbon/model/zendesk_authentication.py
--rw-r--r--   0        0        0     3653 2024-05-30 19:55:10.685905 carbon_python_sdk-0.2.1/carbon/model/zendesk_authentication.pyi
--rw-r--r--   0        0        0     4907 2024-05-30 19:55:10.685999 carbon_python_sdk-0.2.1/carbon/model/zotero_authentication.py
--rw-r--r--   0        0        0     4907 2024-05-30 19:55:10.686097 carbon_python_sdk-0.2.1/carbon/model/zotero_authentication.pyi
--rw-r--r--   0        0        0    13560 2024-05-30 19:57:32.277856 carbon_python_sdk-0.2.1/carbon/models/__init__.py
--rw-r--r--   0        0        0    25498 2024-05-30 19:55:10.686466 carbon_python_sdk-0.2.1/carbon/operation_parameter_map.py
--rw-r--r--   0        0        0     3147 2024-05-30 19:55:10.686693 carbon_python_sdk-0.2.1/carbon/paths/__init__.py
--rw-r--r--   0        0        0      293 2024-05-30 19:55:10.686787 carbon_python_sdk-0.2.1/carbon/paths/add_webhook/__init__.py
--rw-r--r--   0        0        0    13948 2024-05-30 19:55:10.686875 carbon_python_sdk-0.2.1/carbon/paths/add_webhook/post.py
--rw-r--r--   0        0        0    13811 2024-05-30 19:55:10.687094 carbon_python_sdk-0.2.1/carbon/paths/add_webhook/post.pyi
--rw-r--r--   0        0        0      311 2024-05-30 19:55:10.687312 carbon_python_sdk-0.2.1/carbon/paths/auth_v1_access_token/__init__.py
--rw-r--r--   0        0        0    11830 2024-05-30 19:55:10.687394 carbon_python_sdk-0.2.1/carbon/paths/auth_v1_access_token/get.py
--rw-r--r--   0        0        0    11656 2024-05-30 19:55:10.687528 carbon_python_sdk-0.2.1/carbon/paths/auth_v1_access_token/get.pyi
--rw-r--r--   0        0        0      315 2024-05-30 19:55:10.687669 carbon_python_sdk-0.2.1/carbon/paths/auth_v1_white_labeling/__init__.py
--rw-r--r--   0        0        0    11193 2024-05-30 19:55:10.687752 carbon_python_sdk-0.2.1/carbon/paths/auth_v1_white_labeling/get.py
--rw-r--r--   0        0        0    11049 2024-05-30 19:55:10.687884 carbon_python_sdk-0.2.1/carbon/paths/auth_v1_white_labeling/get.pyi
--rw-r--r--   0        0        0      313 2024-05-30 19:55:10.688134 carbon_python_sdk-0.2.1/carbon/paths/create_user_file_tags/__init__.py
--rw-r--r--   0        0        0    15880 2024-05-30 19:55:10.688212 carbon_python_sdk-0.2.1/carbon/paths/create_user_file_tags/post.py
--rw-r--r--   0        0        0    15706 2024-05-30 19:55:10.688423 carbon_python_sdk-0.2.1/carbon/paths/create_user_file_tags/post.pyi
--rw-r--r--   0        0        0      295 2024-05-30 19:55:10.688634 carbon_python_sdk-0.2.1/carbon/paths/delete_files/__init__.py
--rw-r--r--   0        0        0    19307 2024-05-30 19:55:10.688719 carbon_python_sdk-0.2.1/carbon/paths/delete_files/post.py
--rw-r--r--   0        0        0    19133 2024-05-30 19:55:10.688810 carbon_python_sdk-0.2.1/carbon/paths/delete_files/post.pyi
--rw-r--r--   0        0        0      301 2024-05-30 19:55:10.688902 carbon_python_sdk-0.2.1/carbon/paths/delete_files_v2/__init__.py
--rw-r--r--   0        0        0    15967 2024-05-30 19:55:10.688995 carbon_python_sdk-0.2.1/carbon/paths/delete_files_v2/post.py
--rw-r--r--   0        0        0    15793 2024-05-30 19:55:10.689212 carbon_python_sdk-0.2.1/carbon/paths/delete_files_v2/post.pyi
--rw-r--r--   0        0        0      313 2024-05-30 19:55:10.689786 carbon_python_sdk-0.2.1/carbon/paths/delete_user_file_tags/__init__.py
--rw-r--r--   0        0        0    15814 2024-05-30 19:55:10.689864 carbon_python_sdk-0.2.1/carbon/paths/delete_user_file_tags/post.py
--rw-r--r--   0        0        0    15640 2024-05-30 19:55:10.690460 carbon_python_sdk-0.2.1/carbon/paths/delete_user_file_tags/post.pyi
--rw-r--r--   0        0        0      295 2024-05-30 19:55:10.690682 carbon_python_sdk-0.2.1/carbon/paths/delete_users/__init__.py
--rw-r--r--   0        0        0    14899 2024-05-30 19:55:10.690762 carbon_python_sdk-0.2.1/carbon/paths/delete_users/post.py
--rw-r--r--   0        0        0    14762 2024-05-30 19:55:10.690974 carbon_python_sdk-0.2.1/carbon/paths/delete_users/post.pyi
--rw-r--r--   0        0        0      321 2024-05-30 19:55:10.691328 carbon_python_sdk-0.2.1/carbon/paths/delete_webhook_webhook_id/__init__.py
--rw-r--r--   0        0        0    14359 2024-05-30 19:55:10.691410 carbon_python_sdk-0.2.1/carbon/paths/delete_webhook_webhook_id/delete.py
--rw-r--r--   0        0        0    14222 2024-05-30 19:55:10.691621 carbon_python_sdk-0.2.1/carbon/paths/delete_webhook_webhook_id/delete.pyi
--rw-r--r--   0        0        0      307 2024-05-30 19:55:10.691832 carbon_python_sdk-0.2.1/carbon/paths/deletefile_file_id/__init__.py
--rw-r--r--   0        0        0    14552 2024-05-30 19:55:10.691908 carbon_python_sdk-0.2.1/carbon/paths/deletefile_file_id/delete.py
--rw-r--r--   0        0        0    14378 2024-05-30 19:55:10.692117 carbon_python_sdk-0.2.1/carbon/paths/deletefile_file_id/delete.pyi
--rw-r--r--   0        0        0      291 2024-05-30 19:55:10.692326 carbon_python_sdk-0.2.1/carbon/paths/embeddings/__init__.py
--rw-r--r--   0        0        0    29199 2024-05-30 19:55:10.692420 carbon_python_sdk-0.2.1/carbon/paths/embeddings/post.py
--rw-r--r--   0        0        0    29025 2024-05-30 19:55:10.692517 carbon_python_sdk-0.2.1/carbon/paths/embeddings/post.pyi
--rw-r--r--   0        0        0      291 2024-05-30 19:55:10.692743 carbon_python_sdk-0.2.1/carbon/paths/fetch_urls/__init__.py
--rw-r--r--   0        0        0    14466 2024-05-30 19:55:10.692824 carbon_python_sdk-0.2.1/carbon/paths/fetch_urls/get.py
--rw-r--r--   0        0        0    14292 2024-05-30 19:55:10.693035 carbon_python_sdk-0.2.1/carbon/paths/fetch_urls/get.pyi
--rw-r--r--   0        0        0      319 2024-05-30 19:55:10.693244 carbon_python_sdk-0.2.1/carbon/paths/fetch_youtube_transcript/__init__.py
--rw-r--r--   0        0        0    15695 2024-05-30 19:55:10.693320 carbon_python_sdk-0.2.1/carbon/paths/fetch_youtube_transcript/get.py
--rw-r--r--   0        0        0    15521 2024-05-30 19:55:10.693529 carbon_python_sdk-0.2.1/carbon/paths/fetch_youtube_transcript/get.pyi
--rw-r--r--   0        0        0      283 2024-05-30 19:55:10.693743 carbon_python_sdk-0.2.1/carbon/paths/health/__init__.py
--rw-r--r--   0        0        0    10429 2024-05-30 19:55:10.693823 carbon_python_sdk-0.2.1/carbon/paths/health/get.py
--rw-r--r--   0        0        0    10348 2024-05-30 19:55:10.693955 carbon_python_sdk-0.2.1/carbon/paths/health/get.pyi
--rw-r--r--   0        0        0      327 2024-05-30 19:55:10.694094 carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_list/__init__.py
--rw-r--r--   0        0        0    15289 2024-05-30 19:55:10.694179 carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_list/post.py
--rw-r--r--   0        0        0    15115 2024-05-30 19:55:10.694402 carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_list/post.pyi
--rw-r--r--   0        0        0      327 2024-05-30 19:55:10.694621 carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_sync/__init__.py
--rw-r--r--   0        0        0    29028 2024-05-30 19:55:10.694722 carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_sync/post.py
--rw-r--r--   0        0        0    28854 2024-05-30 19:55:10.694836 carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_sync/post.pyi
--rw-r--r--   0        0        0      311 2024-05-30 19:55:10.694941 carbon_python_sdk-0.2.1/carbon/paths/integrations_connect/__init__.py
--rw-r--r--   0        0        0    20686 2024-05-30 19:55:10.695038 carbon_python_sdk-0.2.1/carbon/paths/integrations_connect/post.py
--rw-r--r--   0        0        0    20512 2024-05-30 19:55:10.695143 carbon_python_sdk-0.2.1/carbon/paths/integrations_connect/post.pyi
--rw-r--r--   0        0        0      317 2024-05-30 19:55:10.695252 carbon_python_sdk-0.2.1/carbon/paths/integrations_files_sync/__init__.py
--rw-r--r--   0        0        0    28913 2024-05-30 19:55:10.695362 carbon_python_sdk-0.2.1/carbon/paths/integrations_files_sync/post.py
--rw-r--r--   0        0        0    28739 2024-05-30 19:55:10.695484 carbon_python_sdk-0.2.1/carbon/paths/integrations_files_sync/post.pyi
--rw-r--r--   0        0        0      315 2024-05-30 19:55:10.695590 carbon_python_sdk-0.2.1/carbon/paths/integrations_freshdesk/__init__.py
--rw-r--r--   0        0        0    26091 2024-05-30 19:55:10.695698 carbon_python_sdk-0.2.1/carbon/paths/integrations_freshdesk/post.py
--rw-r--r--   0        0        0    25917 2024-05-30 19:55:10.695819 carbon_python_sdk-0.2.1/carbon/paths/integrations_freshdesk/post.pyi
--rw-r--r--   0        0        0      311 2024-05-30 19:55:10.695923 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook/__init__.py
--rw-r--r--   0        0        0    24946 2024-05-30 19:55:10.696027 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook/post.py
--rw-r--r--   0        0        0    24772 2024-05-30 19:55:10.696139 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook/post.pyi
--rw-r--r--   0        0        0      325 2024-05-30 19:55:10.696244 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_spaces/__init__.py
--rw-r--r--   0        0        0    14816 2024-05-30 19:55:10.696340 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_spaces/get.py
--rw-r--r--   0        0        0    14642 2024-05-30 19:55:10.696579 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_spaces/get.pyi
--rw-r--r--   0        0        0      321 2024-05-30 19:55:10.696820 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_sync/__init__.py
--rw-r--r--   0        0        0    23173 2024-05-30 19:55:10.696919 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_sync/post.py
--rw-r--r--   0        0        0    22999 2024-05-30 19:55:10.697029 carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_sync/post.pyi
--rw-r--r--   0        0        0      309 2024-05-30 19:55:10.697145 carbon_python_sdk-0.2.1/carbon/paths/integrations_github/__init__.py
--rw-r--r--   0        0        0    15826 2024-05-30 19:55:10.697241 carbon_python_sdk-0.2.1/carbon/paths/integrations_github/post.py
--rw-r--r--   0        0        0    15652 2024-05-30 19:55:10.697475 carbon_python_sdk-0.2.1/carbon/paths/integrations_github/post.pyi
--rw-r--r--   0        0        0      321 2024-05-30 19:55:10.697881 carbon_python_sdk-0.2.1/carbon/paths/integrations_github_repos/__init__.py
--rw-r--r--   0        0        0    17078 2024-05-30 19:55:10.697994 carbon_python_sdk-0.2.1/carbon/paths/integrations_github_repos/get.py
--rw-r--r--   0        0        0    16904 2024-05-30 19:55:10.698115 carbon_python_sdk-0.2.1/carbon/paths/integrations_github_repos/get.pyi
--rw-r--r--   0        0        0      331 2024-05-30 19:55:10.698223 carbon_python_sdk-0.2.1/carbon/paths/integrations_github_sync_repos/__init__.py
--rw-r--r--   0        0        0    15560 2024-05-30 19:55:10.698318 carbon_python_sdk-0.2.1/carbon/paths/integrations_github_sync_repos/post.py
--rw-r--r--   0        0        0    15386 2024-05-30 19:55:10.698559 carbon_python_sdk-0.2.1/carbon/paths/integrations_github_sync_repos/post.pyi
--rw-r--r--   0        0        0      317 2024-05-30 19:55:10.698801 carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_sync/__init__.py
--rw-r--r--   0        0        0    26562 2024-05-30 19:55:10.698904 carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_sync/post.py
--rw-r--r--   0        0        0    26388 2024-05-30 19:55:10.699022 carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_sync/post.pyi
--rw-r--r--   0        0        0      331 2024-05-30 19:55:10.699127 carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_user_labels/__init__.py
--rw-r--r--   0        0        0    15340 2024-05-30 19:55:10.699222 carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_user_labels/get.py
--rw-r--r--   0        0        0    15166 2024-05-30 19:55:10.699620 carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_user_labels/get.pyi
--rw-r--r--   0        0        0      317 2024-05-30 19:55:10.699867 carbon_python_sdk-0.2.1/carbon/paths/integrations_items_list/__init__.py
--rw-r--r--   0        0        0    19585 2024-05-30 19:55:10.699970 carbon_python_sdk-0.2.1/carbon/paths/integrations_items_list/post.py
--rw-r--r--   0        0        0    19411 2024-05-30 19:55:10.700072 carbon_python_sdk-0.2.1/carbon/paths/integrations_items_list/post.pyi
--rw-r--r--   0        0        0      317 2024-05-30 19:55:10.700169 carbon_python_sdk-0.2.1/carbon/paths/integrations_items_sync/__init__.py
--rw-r--r--   0        0        0    14992 2024-05-30 19:55:10.700251 carbon_python_sdk-0.2.1/carbon/paths/integrations_items_sync/post.py
--rw-r--r--   0        0        0    14818 2024-05-30 19:55:10.700481 carbon_python_sdk-0.2.1/carbon/paths/integrations_items_sync/post.pyi
--rw-r--r--   0        0        0      315 2024-05-30 19:55:10.700707 carbon_python_sdk-0.2.1/carbon/paths/integrations_oauth_url/__init__.py
--rw-r--r--   0        0        0    37674 2024-05-30 19:55:10.700815 carbon_python_sdk-0.2.1/carbon/paths/integrations_oauth_url/post.py
--rw-r--r--   0        0        0    37500 2024-05-30 19:55:10.700929 carbon_python_sdk-0.2.1/carbon/paths/integrations_oauth_url/post.pyi
--rw-r--r--   0        0        0      321 2024-05-30 19:55:10.701033 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_sync/__init__.py
--rw-r--r--   0        0        0    27296 2024-05-30 19:55:10.701125 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_sync/post.py
--rw-r--r--   0        0        0    27122 2024-05-30 19:55:10.701225 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_sync/post.pyi
--rw-r--r--   0        0        0      343 2024-05-30 19:55:10.701332 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_categories/__init__.py
--rw-r--r--   0        0        0    15590 2024-05-30 19:55:10.701413 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_categories/get.py
--rw-r--r--   0        0        0    15416 2024-05-30 19:55:10.701639 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_categories/get.pyi
--rw-r--r--   0        0        0      337 2024-05-30 19:55:10.701862 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_folders/__init__.py
--rw-r--r--   0        0        0    15371 2024-05-30 19:55:10.701947 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_folders/get.py
--rw-r--r--   0        0        0    15197 2024-05-30 19:55:10.702169 carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_folders/get.pyi
--rw-r--r--   0        0        0      313 2024-05-30 19:55:10.702390 carbon_python_sdk-0.2.1/carbon/paths/integrations_rss_feed/__init__.py
--rw-r--r--   0        0        0    22218 2024-05-30 19:55:10.702479 carbon_python_sdk-0.2.1/carbon/paths/integrations_rss_feed/post.py
--rw-r--r--   0        0        0    22044 2024-05-30 19:55:10.702582 carbon_python_sdk-0.2.1/carbon/paths/integrations_rss_feed/post.pyi
--rw-r--r--   0        0        0      301 2024-05-30 19:55:10.702690 carbon_python_sdk-0.2.1/carbon/paths/integrations_s3/__init__.py
--rw-r--r--   0        0        0    16130 2024-05-30 19:55:10.702782 carbon_python_sdk-0.2.1/carbon/paths/integrations_s3/post.py
--rw-r--r--   0        0        0    15956 2024-05-30 19:55:10.703019 carbon_python_sdk-0.2.1/carbon/paths/integrations_s3/post.pyi
--rw-r--r--   0        0        0      313 2024-05-30 19:55:10.703413 carbon_python_sdk-0.2.1/carbon/paths/integrations_s3_files/__init__.py
--rw-r--r--   0        0        0    28274 2024-05-30 19:55:10.703522 carbon_python_sdk-0.2.1/carbon/paths/integrations_s3_files/post.py
--rw-r--r--   0        0        0    28100 2024-05-30 19:55:10.703649 carbon_python_sdk-0.2.1/carbon/paths/integrations_s3_files/post.pyi
--rw-r--r--   0        0        0      321 2024-05-30 19:55:10.703759 carbon_python_sdk-0.2.1/carbon/paths/modify_user_configuration/__init__.py
--rw-r--r--   0        0        0    16382 2024-05-30 19:55:10.703851 carbon_python_sdk-0.2.1/carbon/paths/modify_user_configuration/post.py
--rw-r--r--   0        0        0    16208 2024-05-30 19:55:10.704087 carbon_python_sdk-0.2.1/carbon/paths/modify_user_configuration/post.pyi
--rw-r--r--   0        0        0      295 2024-05-30 19:55:10.704321 carbon_python_sdk-0.2.1/carbon/paths/organization/__init__.py
--rw-r--r--   0        0        0    10831 2024-05-30 19:55:10.704415 carbon_python_sdk-0.2.1/carbon/paths/organization/get.py
--rw-r--r--   0        0        0    10724 2024-05-30 19:55:10.704562 carbon_python_sdk-0.2.1/carbon/paths/organization/get.pyi
--rw-r--r--   0        0        0      317 2024-05-30 19:55:10.704713 carbon_python_sdk-0.2.1/carbon/paths/organization_statistics/__init__.py
--rw-r--r--   0        0        0    11092 2024-05-30 19:55:10.704808 carbon_python_sdk-0.2.1/carbon/paths/organization_statistics/post.py
--rw-r--r--   0        0        0    10985 2024-05-30 19:55:10.704956 carbon_python_sdk-0.2.1/carbon/paths/organization_statistics/post.pyi
--rw-r--r--   0        0        0      309 2024-05-30 19:55:10.705105 carbon_python_sdk-0.2.1/carbon/paths/organization_update/__init__.py
--rw-r--r--   0        0        0    15275 2024-05-30 19:55:10.705205 carbon_python_sdk-0.2.1/carbon/paths/organization_update/post.py
--rw-r--r--   0        0        0    15138 2024-05-30 19:55:10.705716 carbon_python_sdk-0.2.1/carbon/paths/organization_update/post.pyi
--rw-r--r--   0        0        0      309 2024-05-30 19:55:10.705947 carbon_python_sdk-0.2.1/carbon/paths/parsed_file_file_id/__init__.py
--rw-r--r--   0        0        0    14654 2024-05-30 19:55:10.706027 carbon_python_sdk-0.2.1/carbon/paths/parsed_file_file_id/get.py
--rw-r--r--   0        0        0    14480 2024-05-30 19:55:10.706247 carbon_python_sdk-0.2.1/carbon/paths/parsed_file_file_id/get.pyi
--rw-r--r--   0        0        0      301 2024-05-30 19:55:10.706469 carbon_python_sdk-0.2.1/carbon/paths/process_sitemap/__init__.py
--rw-r--r--   0        0        0    14363 2024-05-30 19:55:10.706549 carbon_python_sdk-0.2.1/carbon/paths/process_sitemap/get.py
--rw-r--r--   0        0        0    14189 2024-05-30 19:55:10.706767 carbon_python_sdk-0.2.1/carbon/paths/process_sitemap/get.pyi
--rw-r--r--   0        0        0      303 2024-05-30 19:55:10.706992 carbon_python_sdk-0.2.1/carbon/paths/raw_file_file_id/__init__.py
--rw-r--r--   0        0        0    14585 2024-05-30 19:55:10.707083 carbon_python_sdk-0.2.1/carbon/paths/raw_file_file_id/get.py
--rw-r--r--   0        0        0    14411 2024-05-30 19:55:10.707302 carbon_python_sdk-0.2.1/carbon/paths/raw_file_file_id/get.pyi
--rw-r--r--   0        0        0      293 2024-05-30 19:55:10.707524 carbon_python_sdk-0.2.1/carbon/paths/resync_file/__init__.py
--rw-r--r--   0        0        0    16696 2024-05-30 19:55:10.707611 carbon_python_sdk-0.2.1/carbon/paths/resync_file/post.py
--rw-r--r--   0        0        0    16522 2024-05-30 19:55:10.707723 carbon_python_sdk-0.2.1/carbon/paths/resync_file/post.pyi
--rw-r--r--   0        0        0      309 2024-05-30 19:55:10.707828 carbon_python_sdk-0.2.1/carbon/paths/revoke_access_token/__init__.py
--rw-r--r--   0        0        0    14828 2024-05-30 19:55:10.707922 carbon_python_sdk-0.2.1/carbon/paths/revoke_access_token/post.py
--rw-r--r--   0        0        0    14654 2024-05-30 19:55:10.708156 carbon_python_sdk-0.2.1/carbon/paths/revoke_access_token/post.pyi
--rw-r--r--   0        0        0      299 2024-05-30 19:55:10.708377 carbon_python_sdk-0.2.1/carbon/paths/scrape_sitemap/__init__.py
--rw-r--r--   0        0        0    27300 2024-05-30 19:55:10.708481 carbon_python_sdk-0.2.1/carbon/paths/scrape_sitemap/post.py
--rw-r--r--   0        0        0    27126 2024-05-30 19:55:10.708583 carbon_python_sdk-0.2.1/carbon/paths/scrape_sitemap/post.pyi
--rw-r--r--   0        0        0      293 2024-05-30 19:55:10.709024 carbon_python_sdk-0.2.1/carbon/paths/search_urls/__init__.py
--rw-r--r--   0        0        0    14549 2024-05-30 19:55:10.709104 carbon_python_sdk-0.2.1/carbon/paths/search_urls/get.py
--rw-r--r--   0        0        0    14375 2024-05-30 19:55:10.709321 carbon_python_sdk-0.2.1/carbon/paths/search_urls/get.pyi
--rw-r--r--   0        0        0      293 2024-05-30 19:55:10.709671 carbon_python_sdk-0.2.1/carbon/paths/text_chunks/__init__.py
--rw-r--r--   0        0        0    19073 2024-05-30 19:55:10.709755 carbon_python_sdk-0.2.1/carbon/paths/text_chunks/post.py
--rw-r--r--   0        0        0    18899 2024-05-30 19:55:10.709857 carbon_python_sdk-0.2.1/carbon/paths/text_chunks/post.pyi
--rw-r--r--   0        0        0      295 2024-05-30 19:55:10.709953 carbon_python_sdk-0.2.1/carbon/paths/update_users/__init__.py
--rw-r--r--   0        0        0    18200 2024-05-30 19:55:10.710044 carbon_python_sdk-0.2.1/carbon/paths/update_users/post.py
--rw-r--r--   0        0        0    18063 2024-05-30 19:55:10.710142 carbon_python_sdk-0.2.1/carbon/paths/update_users/post.pyi
--rw-r--r--   0        0        0      327 2024-05-30 19:55:10.710245 carbon_python_sdk-0.2.1/carbon/paths/upload_chunks_and_embeddings/__init__.py
--rw-r--r--   0        0        0    20060 2024-05-30 19:55:10.710341 carbon_python_sdk-0.2.1/carbon/paths/upload_chunks_and_embeddings/post.py
--rw-r--r--   0        0        0    19886 2024-05-30 19:55:10.710448 carbon_python_sdk-0.2.1/carbon/paths/upload_chunks_and_embeddings/post.pyi
--rw-r--r--   0        0        0      311 2024-05-30 19:55:10.710552 carbon_python_sdk-0.2.1/carbon/paths/upload_file_from_url/__init__.py
--rw-r--r--   0        0        0    24942 2024-05-30 19:55:10.710654 carbon_python_sdk-0.2.1/carbon/paths/upload_file_from_url/post.py
--rw-r--r--   0        0        0    24768 2024-05-30 19:55:10.710769 carbon_python_sdk-0.2.1/carbon/paths/upload_file_from_url/post.pyi
--rw-r--r--   0        0        0      293 2024-05-30 19:55:10.710859 carbon_python_sdk-0.2.1/carbon/paths/upload_text/__init__.py
--rw-r--r--   0        0        0    20504 2024-05-30 19:55:10.710946 carbon_python_sdk-0.2.1/carbon/paths/upload_text/post.py
--rw-r--r--   0        0        0    20330 2024-05-30 19:55:10.711042 carbon_python_sdk-0.2.1/carbon/paths/upload_text/post.pyi
--rw-r--r--   0        0        0      291 2024-05-30 19:55:10.711137 carbon_python_sdk-0.2.1/carbon/paths/uploadfile/__init__.py
--rw-r--r--   0        0        0    35190 2024-05-30 19:57:32.278568 carbon_python_sdk-0.2.1/carbon/paths/uploadfile/post.py
--rw-r--r--   0        0        0    35016 2024-05-30 19:57:32.279260 carbon_python_sdk-0.2.1/carbon/paths/uploadfile/post.pyi
--rw-r--r--   0        0        0      279 2024-05-30 19:55:10.711454 carbon_python_sdk-0.2.1/carbon/paths/user/__init__.py
--rw-r--r--   0        0        0    14156 2024-05-30 19:55:10.711532 carbon_python_sdk-0.2.1/carbon/paths/user/post.py
--rw-r--r--   0        0        0    14019 2024-05-30 19:55:10.711762 carbon_python_sdk-0.2.1/carbon/paths/user/post.pyi
--rw-r--r--   0        0        0      305 2024-05-30 19:55:10.711988 carbon_python_sdk-0.2.1/carbon/paths/user_data_sources/__init__.py
--rw-r--r--   0        0        0    18865 2024-05-30 19:55:10.712087 carbon_python_sdk-0.2.1/carbon/paths/user_data_sources/post.py
--rw-r--r--   0        0        0    18691 2024-05-30 19:55:10.712205 carbon_python_sdk-0.2.1/carbon/paths/user_data_sources/post.pyi
--rw-r--r--   0        0        0      291 2024-05-30 19:55:10.712297 carbon_python_sdk-0.2.1/carbon/paths/user_files/__init__.py
--rw-r--r--   0        0        0    22374 2024-05-30 19:55:10.712384 carbon_python_sdk-0.2.1/carbon/paths/user_files/post.py
--rw-r--r--   0        0        0    22200 2024-05-30 19:55:10.712486 carbon_python_sdk-0.2.1/carbon/paths/user_files/post.pyi
--rw-r--r--   0        0        0      297 2024-05-30 19:55:10.712583 carbon_python_sdk-0.2.1/carbon/paths/user_files_v2/__init__.py
--rw-r--r--   0        0        0    21370 2024-05-30 19:55:10.712679 carbon_python_sdk-0.2.1/carbon/paths/user_files_v2/post.py
--rw-r--r--   0        0        0    21196 2024-05-30 19:55:10.712789 carbon_python_sdk-0.2.1/carbon/paths/user_files_v2/post.pyi
--rw-r--r--   0        0        0      291 2024-05-30 19:55:10.712890 carbon_python_sdk-0.2.1/carbon/paths/web_scrape/__init__.py
--rw-r--r--   0        0        0    14274 2024-05-30 19:55:10.712979 carbon_python_sdk-0.2.1/carbon/paths/web_scrape/post.py
--rw-r--r--   0        0        0    14100 2024-05-30 19:55:10.713204 carbon_python_sdk-0.2.1/carbon/paths/web_scrape/post.pyi
--rw-r--r--   0        0        0      287 2024-05-30 19:55:10.713555 carbon_python_sdk-0.2.1/carbon/paths/webhooks/__init__.py
--rw-r--r--   0        0        0    17367 2024-05-30 19:55:10.713641 carbon_python_sdk-0.2.1/carbon/paths/webhooks/post.py
--rw-r--r--   0        0        0    17230 2024-05-30 19:55:10.713734 carbon_python_sdk-0.2.1/carbon/paths/webhooks/post.pyi
--rw-r--r--   0        0        0        0 2024-05-30 19:55:10.713869 carbon_python_sdk-0.2.1/carbon/pydantic/__init__.py
--rw-r--r--   0        0        0      559 2024-05-30 19:55:10.713949 carbon_python_sdk-0.2.1/carbon/pydantic/add_webhook_props.py
--rw-r--r--   0        0        0      586 2024-05-30 19:55:10.714034 carbon_python_sdk-0.2.1/carbon/pydantic/body_create_upload_file_uploadfile_post.py
--rw-r--r--   0        0        0      760 2024-05-30 19:55:10.714112 carbon_python_sdk-0.2.1/carbon/pydantic/chunk_properties.py
--rw-r--r--   0        0        0      768 2024-05-30 19:55:10.714199 carbon_python_sdk-0.2.1/carbon/pydantic/chunk_properties_nullable.py
--rw-r--r--   0        0        0      821 2024-05-30 19:55:10.714283 carbon_python_sdk-0.2.1/carbon/pydantic/chunks_and_embeddings.py
--rw-r--r--   0        0        0      469 2024-05-30 19:55:10.714367 carbon_python_sdk-0.2.1/carbon/pydantic/chunks_and_embeddings_embedding.py
--rw-r--r--   0        0        0     1333 2024-05-30 19:55:10.714451 carbon_python_sdk-0.2.1/carbon/pydantic/chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0      438 2024-05-30 19:55:10.714534 carbon_python_sdk-0.2.1/carbon/pydantic/chunks_and_embeddings_upload_input_custom_credentials.py
--rw-r--r--   0        0        0      418 2024-05-30 19:55:10.714613 carbon_python_sdk-0.2.1/carbon/pydantic/configuration_keys.py
--rw-r--r--   0        0        0      835 2024-05-30 19:55:10.714694 carbon_python_sdk-0.2.1/carbon/pydantic/confluence_authentication.py
--rw-r--r--   0        0        0     1791 2024-05-30 19:55:10.714775 carbon_python_sdk-0.2.1/carbon/pydantic/connect_data_source_input.py
--rw-r--r--   0        0        0      765 2024-05-30 19:55:10.714864 carbon_python_sdk-0.2.1/carbon/pydantic/connect_data_source_response.py
--rw-r--r--   0        0        0      481 2024-05-30 19:55:10.714952 carbon_python_sdk-0.2.1/carbon/pydantic/custom_credentials_type.py
--rw-r--r--   0        0        0      424 2024-05-30 19:55:10.715031 carbon_python_sdk-0.2.1/carbon/pydantic/data_source_extended_input.py
--rw-r--r--   0        0        0      456 2024-05-30 19:55:10.715111 carbon_python_sdk-0.2.1/carbon/pydantic/data_source_last_sync_actions.py
--rw-r--r--   0        0        0      472 2024-05-30 19:55:10.715191 carbon_python_sdk-0.2.1/carbon/pydantic/data_source_sync_statuses.py
--rw-r--r--   0        0        0      890 2024-05-30 19:55:10.715273 carbon_python_sdk-0.2.1/carbon/pydantic/data_source_type.py
--rw-r--r--   0        0        0      898 2024-05-30 19:55:10.715357 carbon_python_sdk-0.2.1/carbon/pydantic/data_source_type_nullable.py
--rw-r--r--   0        0        0     1187 2024-05-30 19:55:10.715436 carbon_python_sdk-0.2.1/carbon/pydantic/delete_files_query_input.py
--rw-r--r--   0        0        0      448 2024-05-30 19:55:10.715518 carbon_python_sdk-0.2.1/carbon/pydantic/delete_files_query_input_file_ids.py
--rw-r--r--   0        0        0      809 2024-05-30 19:55:10.715617 carbon_python_sdk-0.2.1/carbon/pydantic/delete_files_v2_query_input.py
--rw-r--r--   0        0        0      690 2024-05-30 19:55:10.715702 carbon_python_sdk-0.2.1/carbon/pydantic/delete_users_input.py
--rw-r--r--   0        0        0      430 2024-05-30 19:55:10.715788 carbon_python_sdk-0.2.1/carbon/pydantic/delete_users_input_customer_ids.py
--rw-r--r--   0        0        0      694 2024-05-30 19:55:10.715867 carbon_python_sdk-0.2.1/carbon/pydantic/directory_item.py
--rw-r--r--   0        0        0     1674 2024-05-30 19:55:10.715952 carbon_python_sdk-0.2.1/carbon/pydantic/document_response.py
--rw-r--r--   0        0        0      665 2024-05-30 19:55:10.716036 carbon_python_sdk-0.2.1/carbon/pydantic/document_response_list.py
--rw-r--r--   0        0        0      411 2024-05-30 19:55:10.716320 carbon_python_sdk-0.2.1/carbon/pydantic/document_response_tags.py
--rw-r--r--   0        0        0      463 2024-05-30 19:55:10.716421 carbon_python_sdk-0.2.1/carbon/pydantic/document_response_vector.py
--rw-r--r--   0        0        0     1021 2024-05-30 19:55:10.716509 carbon_python_sdk-0.2.1/carbon/pydantic/embedding_and_chunk.py
--rw-r--r--   0        0        0      467 2024-05-30 19:55:10.716595 carbon_python_sdk-0.2.1/carbon/pydantic/embedding_and_chunk_embedding.py
--rw-r--r--   0        0        0      743 2024-05-30 19:55:10.716682 carbon_python_sdk-0.2.1/carbon/pydantic/embedding_generators.py
--rw-r--r--   0        0        0      751 2024-05-30 19:55:10.716779 carbon_python_sdk-0.2.1/carbon/pydantic/embedding_generators_nullable.py
--rw-r--r--   0        0        0      666 2024-05-30 19:55:10.716860 carbon_python_sdk-0.2.1/carbon/pydantic/embedding_properties.py
--rw-r--r--   0        0        0      780 2024-05-30 19:55:10.716946 carbon_python_sdk-0.2.1/carbon/pydantic/embeddings_and_chunks_filters.py
--rw-r--r--   0        0        0      470 2024-05-30 19:55:10.717037 carbon_python_sdk-0.2.1/carbon/pydantic/embeddings_and_chunks_order_by_columns.py
--rw-r--r--   0        0        0     1222 2024-05-30 19:55:10.717128 carbon_python_sdk-0.2.1/carbon/pydantic/embeddings_and_chunks_query_input.py
--rw-r--r--   0        0        0      711 2024-05-30 19:55:10.717210 carbon_python_sdk-0.2.1/carbon/pydantic/embeddings_and_chunks_response.py
--rw-r--r--   0        0        0      553 2024-05-30 19:55:10.717289 carbon_python_sdk-0.2.1/carbon/pydantic/external_file_sync_statuses.py
--rw-r--r--   0        0        0     1780 2024-05-30 19:55:10.717373 carbon_python_sdk-0.2.1/carbon/pydantic/external_source_item.py
--rw-r--r--   0        0        0      455 2024-05-30 19:55:10.717457 carbon_python_sdk-0.2.1/carbon/pydantic/external_source_items_order_by.py
--rw-r--r--   0        0        0      781 2024-05-30 19:55:10.717539 carbon_python_sdk-0.2.1/carbon/pydantic/fetch_urls_response.py
--rw-r--r--   0        0        0      424 2024-05-30 19:55:10.717622 carbon_python_sdk-0.2.1/carbon/pydantic/fetch_urls_response_urls.py
--rw-r--r--   0        0        0      445 2024-05-30 19:55:10.717708 carbon_python_sdk-0.2.1/carbon/pydantic/file_content_types.py
--rw-r--r--   0        0        0      453 2024-05-30 19:55:10.717791 carbon_python_sdk-0.2.1/carbon/pydantic/file_content_types_nullable.py
--rw-r--r--   0        0        0      820 2024-05-30 19:55:10.717883 carbon_python_sdk-0.2.1/carbon/pydantic/file_formats.py
--rw-r--r--   0        0        0      828 2024-05-30 19:55:10.717975 carbon_python_sdk-0.2.1/carbon/pydantic/file_formats_nullable.py
--rw-r--r--   0        0        0     1002 2024-05-30 19:55:10.718056 carbon_python_sdk-0.2.1/carbon/pydantic/file_statistics.py
--rw-r--r--   0        0        0     1010 2024-05-30 19:55:10.718136 carbon_python_sdk-0.2.1/carbon/pydantic/file_statistics_nullable.py
--rw-r--r--   0        0        0     1240 2024-05-30 19:55:10.718314 carbon_python_sdk-0.2.1/carbon/pydantic/file_sync_config.py
--rw-r--r--   0        0        0     1248 2024-05-30 19:55:10.718402 carbon_python_sdk-0.2.1/carbon/pydantic/file_sync_config_nullable.py
--rw-r--r--   0        0        0      492 2024-05-30 19:55:10.718486 carbon_python_sdk-0.2.1/carbon/pydantic/files_query_user_files_deprecated_response.py
--rw-r--r--   0        0        0     2096 2024-05-30 19:55:10.718568 carbon_python_sdk-0.2.1/carbon/pydantic/fresh_desk_connect_request.py
--rw-r--r--   0        0        0      723 2024-05-30 19:55:10.718645 carbon_python_sdk-0.2.1/carbon/pydantic/freskdesk_authentication.py
--rw-r--r--   0        0        0      575 2024-05-30 19:55:10.718724 carbon_python_sdk-0.2.1/carbon/pydantic/generic_success_response.py
--rw-r--r--   0        0        0     3379 2024-05-30 19:55:10.718805 carbon_python_sdk-0.2.1/carbon/pydantic/get_embedding_documents_body.py
--rw-r--r--   0        0        0      452 2024-05-30 19:55:10.718883 carbon_python_sdk-0.2.1/carbon/pydantic/get_embedding_documents_body_file_ids.py
--rw-r--r--   0        0        0      458 2024-05-30 19:55:10.718959 carbon_python_sdk-0.2.1/carbon/pydantic/get_embedding_documents_body_parent_file_ids.py
--rw-r--r--   0        0        0      477 2024-05-30 19:55:10.719044 carbon_python_sdk-0.2.1/carbon/pydantic/get_embedding_documents_body_query_vector.py
--rw-r--r--   0        0        0      420 2024-05-30 19:55:10.719124 carbon_python_sdk-0.2.1/carbon/pydantic/get_embedding_documents_body_tags.py
--rw-r--r--   0        0        0      752 2024-05-30 19:55:10.719205 carbon_python_sdk-0.2.1/carbon/pydantic/gitbook_authetication.py
--rw-r--r--   0        0        0     1911 2024-05-30 19:55:10.719284 carbon_python_sdk-0.2.1/carbon/pydantic/gitbook_connect_request.py
--rw-r--r--   0        0        0     1699 2024-05-30 19:55:10.719370 carbon_python_sdk-0.2.1/carbon/pydantic/gitbook_sync_request.py
--rw-r--r--   0        0        0      429 2024-05-30 19:55:10.719464 carbon_python_sdk-0.2.1/carbon/pydantic/gitbook_sync_request_space_ids.py
--rw-r--r--   0        0        0      734 2024-05-30 19:55:10.719556 carbon_python_sdk-0.2.1/carbon/pydantic/github_authentication.py
--rw-r--r--   0        0        0      825 2024-05-30 19:55:10.719644 carbon_python_sdk-0.2.1/carbon/pydantic/github_connect_request.py
--rw-r--r--   0        0        0      783 2024-05-30 19:55:10.719735 carbon_python_sdk-0.2.1/carbon/pydantic/github_fetch_repos_request.py
--rw-r--r--   0        0        0      431 2024-05-30 19:55:10.719830 carbon_python_sdk-0.2.1/carbon/pydantic/github_fetch_repos_request_repos.py
--rw-r--r--   0        0        0     2073 2024-05-30 19:55:10.719918 carbon_python_sdk-0.2.1/carbon/pydantic/gmail_sync_input.py
--rw-r--r--   0        0        0      432 2024-05-30 19:55:10.720008 carbon_python_sdk-0.2.1/carbon/pydantic/helpdesk_file_types.py
--rw-r--r--   0        0        0      678 2024-05-30 19:55:10.720093 carbon_python_sdk-0.2.1/carbon/pydantic/http_validation_error.py
--rw-r--r--   0        0        0      665 2024-05-30 19:55:10.720182 carbon_python_sdk-0.2.1/carbon/pydantic/hybrid_search_tuning_params.py
--rw-r--r--   0        0        0      673 2024-05-30 19:55:10.720274 carbon_python_sdk-0.2.1/carbon/pydantic/hybrid_search_tuning_params_nullable.py
--rw-r--r--   0        0        0     1282 2024-05-30 19:55:10.720366 carbon_python_sdk-0.2.1/carbon/pydantic/list_data_source_items_request.py
--rw-r--r--   0        0        0      710 2024-05-30 19:55:10.720455 carbon_python_sdk-0.2.1/carbon/pydantic/list_data_source_items_response.py
--rw-r--r--   0        0        0     1035 2024-05-30 19:55:10.720546 carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters.py
--rw-r--r--   0        0        0      447 2024-05-30 19:55:10.720642 carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters_external_ids.py
--rw-r--r--   0        0        0      439 2024-05-30 19:55:10.720853 carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters_ids.py
--rw-r--r--   0        0        0     1093 2024-05-30 19:55:10.720946 carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters_nullable.py
--rw-r--r--   0        0        0      455 2024-05-30 19:55:10.721039 carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters_nullable_external_ids.py
--rw-r--r--   0        0        0      447 2024-05-30 19:55:10.721135 carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters_nullable_ids.py
--rw-r--r--   0        0        0      664 2024-05-30 19:55:10.721222 carbon_python_sdk-0.2.1/carbon/pydantic/list_request.py
--rw-r--r--   0        0        0      638 2024-05-30 19:55:10.721314 carbon_python_sdk-0.2.1/carbon/pydantic/list_response.py
--rw-r--r--   0        0        0      733 2024-05-30 19:55:10.721402 carbon_python_sdk-0.2.1/carbon/pydantic/modify_user_configuration_input.py
--rw-r--r--   0        0        0      430 2024-05-30 19:57:32.279498 carbon_python_sdk-0.2.1/carbon/pydantic/multi_modal_embedding_generators.py
--rw-r--r--   0        0        0      742 2024-05-30 19:55:10.721590 carbon_python_sdk-0.2.1/carbon/pydantic/notion_authentication.py
--rw-r--r--   0        0        0      814 2024-05-30 19:55:10.721686 carbon_python_sdk-0.2.1/carbon/pydantic/o_auth_authentication.py
--rw-r--r--   0        0        0     4718 2024-05-30 19:57:32.279709 carbon_python_sdk-0.2.1/carbon/pydantic/o_auth_url_request.py
--rw-r--r--   0        0        0      417 2024-05-30 19:55:10.721891 carbon_python_sdk-0.2.1/carbon/pydantic/order_dir.py
--rw-r--r--   0        0        0      419 2024-05-30 19:55:10.721984 carbon_python_sdk-0.2.1/carbon/pydantic/order_dir_v2.py
--rw-r--r--   0        0        0     2547 2024-05-30 19:55:10.722071 carbon_python_sdk-0.2.1/carbon/pydantic/organization_response.py
--rw-r--r--   0        0        0     2100 2024-05-30 19:55:10.722164 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_api.py
--rw-r--r--   0        0        0      998 2024-05-30 19:55:10.722254 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_filters.py
--rw-r--r--   0        0        0      456 2024-05-30 19:55:10.722352 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_filters_ids.py
--rw-r--r--   0        0        0      462 2024-05-30 19:55:10.722448 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_order_by_columns.py
--rw-r--r--   0        0        0     1213 2024-05-30 19:55:10.722540 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_query_input.py
--rw-r--r--   0        0        0      756 2024-05-30 19:55:10.722627 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_response.py
--rw-r--r--   0        0        0      785 2024-05-30 19:55:10.722706 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_file_tag_create.py
--rw-r--r--   0        0        0      424 2024-05-30 19:55:10.722787 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_file_tag_create_tags.py
--rw-r--r--   0        0        0      789 2024-05-30 19:55:10.722867 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_file_tags_remove.py
--rw-r--r--   0        0        0      437 2024-05-30 19:55:10.722947 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_file_tags_remove_tags.py
--rw-r--r--   0        0        0     5786 2024-05-30 19:55:10.723038 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters.py
--rw-r--r--   0        0        0      469 2024-05-30 19:55:10.723118 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters_external_file_ids.py
--rw-r--r--   0        0        0      457 2024-05-30 19:55:10.723199 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters_ids.py
--rw-r--r--   0        0        0      482 2024-05-30 19:55:10.723283 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters_organization_user_data_source_id.py
--rw-r--r--   0        0        0      467 2024-05-30 19:55:10.723370 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters_parent_file_ids.py
--rw-r--r--   0        0        0      464 2024-05-30 19:55:10.723450 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters_request_ids.py
--rw-r--r--   0        0        0      429 2024-05-30 19:55:10.723531 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters_tags.py
--rw-r--r--   0        0        0      501 2024-05-30 19:55:10.723616 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_order_by_types.py
--rw-r--r--   0        0        0     1554 2024-05-30 19:55:10.723696 carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_query_input.py
--rw-r--r--   0        0        0      571 2024-05-30 19:55:10.723774 carbon_python_sdk-0.2.1/carbon/pydantic/outh_url_response.py
--rw-r--r--   0        0        0     2156 2024-05-30 19:55:10.723851 carbon_python_sdk-0.2.1/carbon/pydantic/outlook_sync_input.py
--rw-r--r--   0        0        0      645 2024-05-30 19:55:10.723930 carbon_python_sdk-0.2.1/carbon/pydantic/pagination.py
--rw-r--r--   0        0        0      584 2024-05-30 19:55:10.724030 carbon_python_sdk-0.2.1/carbon/pydantic/presigned_url_response.py
--rw-r--r--   0        0        0     1341 2024-05-30 19:55:10.724130 carbon_python_sdk-0.2.1/carbon/pydantic/raw_text_input.py
--rw-r--r--   0        0        0      861 2024-05-30 19:55:10.724214 carbon_python_sdk-0.2.1/carbon/pydantic/resync_file_query_input.py
--rw-r--r--   0        0        0      588 2024-05-30 19:55:10.724316 carbon_python_sdk-0.2.1/carbon/pydantic/revoke_access_token_input.py
--rw-r--r--   0        0        0     1515 2024-05-30 19:55:10.724393 carbon_python_sdk-0.2.1/carbon/pydantic/rss_feed_input.py
--rw-r--r--   0        0        0      832 2024-05-30 19:55:10.724477 carbon_python_sdk-0.2.1/carbon/pydantic/s3_auth_request.py
--rw-r--r--   0        0        0      744 2024-05-30 19:55:10.724556 carbon_python_sdk-0.2.1/carbon/pydantic/s3_authentication.py
--rw-r--r--   0        0        0     2360 2024-05-30 19:55:10.724641 carbon_python_sdk-0.2.1/carbon/pydantic/s3_file_sync_input.py
--rw-r--r--   0        0        0      677 2024-05-30 19:55:10.724720 carbon_python_sdk-0.2.1/carbon/pydantic/s3_get_file_input.py
--rw-r--r--   0        0        0      829 2024-05-30 19:55:10.724800 carbon_python_sdk-0.2.1/carbon/pydantic/salesforce_authentication.py
--rw-r--r--   0        0        0      886 2024-05-30 19:55:10.724883 carbon_python_sdk-0.2.1/carbon/pydantic/sharepoint_authentication.py
--rw-r--r--   0        0        0      494 2024-05-30 19:55:10.724969 carbon_python_sdk-0.2.1/carbon/pydantic/simple_o_auth_data_sources.py
--rw-r--r--   0        0        0      942 2024-05-30 19:55:10.725053 carbon_python_sdk-0.2.1/carbon/pydantic/single_chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0     2337 2024-05-30 19:55:10.725190 carbon_python_sdk-0.2.1/carbon/pydantic/sitemap_scrape_request.py
--rw-r--r--   0        0        0      456 2024-05-30 19:55:10.725288 carbon_python_sdk-0.2.1/carbon/pydantic/sitemap_scrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0      458 2024-05-30 19:55:10.725376 carbon_python_sdk-0.2.1/carbon/pydantic/sitemap_scrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0      454 2024-05-30 19:55:10.725462 carbon_python_sdk-0.2.1/carbon/pydantic/sitemap_scrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0      415 2024-05-30 19:55:10.725543 carbon_python_sdk-0.2.1/carbon/pydantic/sitemap_scrape_request_tags.py
--rw-r--r--   0        0        0      586 2024-05-30 19:55:10.725625 carbon_python_sdk-0.2.1/carbon/pydantic/sync_directory_request.py
--rw-r--r--   0        0        0      597 2024-05-30 19:55:10.725704 carbon_python_sdk-0.2.1/carbon/pydantic/sync_files_ids.py
--rw-r--r--   0        0        0     2668 2024-05-30 19:55:10.725786 carbon_python_sdk-0.2.1/carbon/pydantic/sync_files_request.py
--rw-r--r--   0        0        0     2932 2024-05-30 19:55:10.726185 carbon_python_sdk-0.2.1/carbon/pydantic/sync_options.py
--rw-r--r--   0        0        0      726 2024-05-30 19:55:10.726271 carbon_python_sdk-0.2.1/carbon/pydantic/text_embedding_generators.py
--rw-r--r--   0        0        0      630 2024-05-30 19:55:10.726349 carbon_python_sdk-0.2.1/carbon/pydantic/token_response.py
--rw-r--r--   0        0        0      724 2024-05-30 19:55:10.726432 carbon_python_sdk-0.2.1/carbon/pydantic/update_organization_input.py
--rw-r--r--   0        0        0     1746 2024-05-30 19:55:10.726521 carbon_python_sdk-0.2.1/carbon/pydantic/update_users_input.py
--rw-r--r--   0        0        0      430 2024-05-30 19:55:10.726606 carbon_python_sdk-0.2.1/carbon/pydantic/update_users_input_customer_ids.py
--rw-r--r--   0        0        0     1862 2024-05-30 19:55:10.726693 carbon_python_sdk-0.2.1/carbon/pydantic/upload_file_from_url_input.py
--rw-r--r--   0        0        0     1582 2024-05-30 19:55:10.726783 carbon_python_sdk-0.2.1/carbon/pydantic/user_configuration.py
--rw-r--r--   0        0        0     1590 2024-05-30 19:55:10.726878 carbon_python_sdk-0.2.1/carbon/pydantic/user_configuration_nullable.py
--rw-r--r--   0        0        0     3606 2024-05-30 19:55:10.726971 carbon_python_sdk-0.2.1/carbon/pydantic/user_file.py
--rw-r--r--   0        0        0      487 2024-05-30 19:55:10.727065 carbon_python_sdk-0.2.1/carbon/pydantic/user_file_embedding_properties.py
--rw-r--r--   0        0        0      667 2024-05-30 19:55:10.727159 carbon_python_sdk-0.2.1/carbon/pydantic/user_files_v2.py
--rw-r--r--   0        0        0      578 2024-05-30 19:55:10.727247 carbon_python_sdk-0.2.1/carbon/pydantic/user_request_content.py
--rw-r--r--   0        0        0     2736 2024-05-30 19:55:10.727330 carbon_python_sdk-0.2.1/carbon/pydantic/user_response.py
--rw-r--r--   0        0        0      503 2024-05-30 19:55:10.727417 carbon_python_sdk-0.2.1/carbon/pydantic/user_response_auto_sync_enabled_sources.py
--rw-r--r--   0        0        0      432 2024-05-30 19:55:10.727511 carbon_python_sdk-0.2.1/carbon/pydantic/user_response_unique_file_tags.py
--rw-r--r--   0        0        0      504 2024-05-30 19:55:10.727602 carbon_python_sdk-0.2.1/carbon/pydantic/utilities_scrape_web_request.py
--rw-r--r--   0        0        0      714 2024-05-30 19:55:10.727696 carbon_python_sdk-0.2.1/carbon/pydantic/validation_error.py
--rw-r--r--   0        0        0      440 2024-05-30 19:55:10.727793 carbon_python_sdk-0.2.1/carbon/pydantic/validation_error_loc.py
--rw-r--r--   0        0        0      982 2024-05-30 19:55:10.727889 carbon_python_sdk-0.2.1/carbon/pydantic/webhook.py
--rw-r--r--   0        0        0      661 2024-05-30 19:55:10.727985 carbon_python_sdk-0.2.1/carbon/pydantic/webhook_filters.py
--rw-r--r--   0        0        0      437 2024-05-30 19:55:10.728078 carbon_python_sdk-0.2.1/carbon/pydantic/webhook_filters_ids.py
--rw-r--r--   0        0        0      936 2024-05-30 19:55:10.728170 carbon_python_sdk-0.2.1/carbon/pydantic/webhook_no_key.py
--rw-r--r--   0        0        0      443 2024-05-30 19:55:10.728265 carbon_python_sdk-0.2.1/carbon/pydantic/webhook_order_by_columns.py
--rw-r--r--   0        0        0     1074 2024-05-30 19:55:10.728359 carbon_python_sdk-0.2.1/carbon/pydantic/webhook_query_input.py
--rw-r--r--   0        0        0      689 2024-05-30 19:55:10.728453 carbon_python_sdk-0.2.1/carbon/pydantic/webhook_query_response.py
--rw-r--r--   0        0        0      428 2024-05-30 19:55:10.728550 carbon_python_sdk-0.2.1/carbon/pydantic/webhook_status.py
--rw-r--r--   0        0        0     2380 2024-05-30 19:55:10.728643 carbon_python_sdk-0.2.1/carbon/pydantic/webscrape_request.py
--rw-r--r--   0        0        0      452 2024-05-30 19:55:10.728737 carbon_python_sdk-0.2.1/carbon/pydantic/webscrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0      454 2024-05-30 19:55:10.728833 carbon_python_sdk-0.2.1/carbon/pydantic/webscrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0      450 2024-05-30 19:55:10.728928 carbon_python_sdk-0.2.1/carbon/pydantic/webscrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0      411 2024-05-30 19:55:10.729023 carbon_python_sdk-0.2.1/carbon/pydantic/webscrape_request_tags.py
--rw-r--r--   0        0        0      727 2024-05-30 19:55:10.729116 carbon_python_sdk-0.2.1/carbon/pydantic/white_labeling_response.py
--rw-r--r--   0        0        0      887 2024-05-30 19:55:10.729208 carbon_python_sdk-0.2.1/carbon/pydantic/youtube_transcript_response.py
--rw-r--r--   0        0        0      616 2024-05-30 19:55:10.729307 carbon_python_sdk-0.2.1/carbon/pydantic/youtube_transcript_response_raw_transcript.py
--rw-r--r--   0        0        0      433 2024-05-30 19:55:10.729409 carbon_python_sdk-0.2.1/carbon/pydantic/youtube_transcript_response_raw_transcript_item.py
--rw-r--r--   0        0        0      737 2024-05-30 19:55:10.729501 carbon_python_sdk-0.2.1/carbon/pydantic/zendesk_authentication.py
--rw-r--r--   0        0        0      848 2024-05-30 19:55:10.729591 carbon_python_sdk-0.2.1/carbon/pydantic/zotero_authentication.py
--rw-r--r--   0        0        0      654 2024-05-30 19:55:10.729683 carbon_python_sdk-0.2.1/carbon/request_after_hook.py
--rw-r--r--   0        0        0      712 2024-05-30 19:55:10.729783 carbon_python_sdk-0.2.1/carbon/request_before_hook.py
--rw-r--r--   0        0        0      677 2024-05-30 19:55:10.729877 carbon_python_sdk-0.2.1/carbon/request_before_url_hook.py
--rw-r--r--   0        0        0    10974 2024-05-30 19:55:10.729974 carbon_python_sdk-0.2.1/carbon/rest.py
--rw-r--r--   0        0        0    96042 2024-05-30 19:55:10.730197 carbon_python_sdk-0.2.1/carbon/schemas.py
--rw-r--r--   0        0        0        0 2024-05-30 19:55:10.730326 carbon_python_sdk-0.2.1/carbon/type/__init__.py
--rw-r--r--   0        0        0      525 2024-05-30 19:55:10.730426 carbon_python_sdk-0.2.1/carbon/type/add_webhook_props.py
--rw-r--r--   0        0        0      627 2024-05-30 19:55:10.730520 carbon_python_sdk-0.2.1/carbon/type/body_create_upload_file_uploadfile_post.py
--rw-r--r--   0        0        0      628 2024-05-30 19:55:10.730606 carbon_python_sdk-0.2.1/carbon/type/chunk_properties.py
--rw-r--r--   0        0        0      668 2024-05-30 19:55:10.730720 carbon_python_sdk-0.2.1/carbon/type/chunk_properties_nullable.py
--rw-r--r--   0        0        0      725 2024-05-30 19:55:10.730806 carbon_python_sdk-0.2.1/carbon/type/chunks_and_embeddings.py
--rw-r--r--   0        0        0      408 2024-05-30 19:55:10.730895 carbon_python_sdk-0.2.1/carbon/type/chunks_and_embeddings_embedding.py
--rw-r--r--   0        0        0     1117 2024-05-30 19:55:10.730980 carbon_python_sdk-0.2.1/carbon/type/chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0      377 2024-05-30 19:55:10.731081 carbon_python_sdk-0.2.1/carbon/type/chunks_and_embeddings_upload_input_custom_credentials.py
--rw-r--r--   0        0        0      346 2024-05-30 19:55:10.731168 carbon_python_sdk-0.2.1/carbon/type/configuration_keys.py
--rw-r--r--   0        0        0      714 2024-05-30 19:55:10.731257 carbon_python_sdk-0.2.1/carbon/type/confluence_authentication.py
--rw-r--r--   0        0        0     1664 2024-05-30 19:55:10.731345 carbon_python_sdk-0.2.1/carbon/type/connect_data_source_input.py
--rw-r--r--   0        0        0      733 2024-05-30 19:55:10.731432 carbon_python_sdk-0.2.1/carbon/type/connect_data_source_response.py
--rw-r--r--   0        0        0      420 2024-05-30 19:55:10.731697 carbon_python_sdk-0.2.1/carbon/type/custom_credentials_type.py
--rw-r--r--   0        0        0      352 2024-05-30 19:55:10.731816 carbon_python_sdk-0.2.1/carbon/type/data_source_extended_input.py
--rw-r--r--   0        0        0      395 2024-05-30 19:55:10.731917 carbon_python_sdk-0.2.1/carbon/type/data_source_last_sync_actions.py
--rw-r--r--   0        0        0      411 2024-05-30 19:55:10.732012 carbon_python_sdk-0.2.1/carbon/type/data_source_sync_statuses.py
--rw-r--r--   0        0        0      829 2024-05-30 19:55:10.732107 carbon_python_sdk-0.2.1/carbon/type/data_source_type.py
--rw-r--r--   0        0        0      837 2024-05-30 19:55:10.732203 carbon_python_sdk-0.2.1/carbon/type/data_source_type_nullable.py
--rw-r--r--   0        0        0      929 2024-05-30 19:55:10.732307 carbon_python_sdk-0.2.1/carbon/type/delete_files_query_input.py
--rw-r--r--   0        0        0      387 2024-05-30 19:55:10.732403 carbon_python_sdk-0.2.1/carbon/type/delete_files_query_input_file_ids.py
--rw-r--r--   0        0        0      723 2024-05-30 19:55:10.732493 carbon_python_sdk-0.2.1/carbon/type/delete_files_v2_query_input.py
--rw-r--r--   0        0        0      647 2024-05-30 19:55:10.732592 carbon_python_sdk-0.2.1/carbon/type/delete_users_input.py
--rw-r--r--   0        0        0      369 2024-05-30 19:55:10.732688 carbon_python_sdk-0.2.1/carbon/type/delete_users_input_customer_ids.py
--rw-r--r--   0        0        0      574 2024-05-30 19:55:10.732783 carbon_python_sdk-0.2.1/carbon/type/directory_item.py
--rw-r--r--   0        0        0     1356 2024-05-30 19:55:10.733004 carbon_python_sdk-0.2.1/carbon/type/document_response.py
--rw-r--r--   0        0        0      641 2024-05-30 19:55:10.733153 carbon_python_sdk-0.2.1/carbon/type/document_response_list.py
--rw-r--r--   0        0        0      350 2024-05-30 19:55:10.733253 carbon_python_sdk-0.2.1/carbon/type/document_response_tags.py
--rw-r--r--   0        0        0      402 2024-05-30 19:55:10.733344 carbon_python_sdk-0.2.1/carbon/type/document_response_vector.py
--rw-r--r--   0        0        0      877 2024-05-30 19:55:10.733437 carbon_python_sdk-0.2.1/carbon/type/embedding_and_chunk.py
--rw-r--r--   0        0        0      406 2024-05-30 19:55:10.733523 carbon_python_sdk-0.2.1/carbon/type/embedding_and_chunk_embedding.py
--rw-r--r--   0        0        0      682 2024-05-30 19:55:10.733607 carbon_python_sdk-0.2.1/carbon/type/embedding_generators.py
--rw-r--r--   0        0        0      690 2024-05-30 19:55:10.733694 carbon_python_sdk-0.2.1/carbon/type/embedding_generators_nullable.py
--rw-r--r--   0        0        0      610 2024-05-30 19:55:10.733772 carbon_python_sdk-0.2.1/carbon/type/embedding_properties.py
--rw-r--r--   0        0        0      729 2024-05-30 19:55:10.733857 carbon_python_sdk-0.2.1/carbon/type/embeddings_and_chunks_filters.py
--rw-r--r--   0        0        0      409 2024-05-30 19:55:10.733941 carbon_python_sdk-0.2.1/carbon/type/embeddings_and_chunks_order_by_columns.py
--rw-r--r--   0        0        0     1009 2024-05-30 19:55:10.734037 carbon_python_sdk-0.2.1/carbon/type/embeddings_and_chunks_query_input.py
--rw-r--r--   0        0        0      694 2024-05-30 19:55:10.734136 carbon_python_sdk-0.2.1/carbon/type/embeddings_and_chunks_response.py
--rw-r--r--   0        0        0      492 2024-05-30 19:55:10.734219 carbon_python_sdk-0.2.1/carbon/type/external_file_sync_statuses.py
--rw-r--r--   0        0        0     1189 2024-05-30 19:55:10.734300 carbon_python_sdk-0.2.1/carbon/type/external_source_item.py
--rw-r--r--   0        0        0      394 2024-05-30 19:55:10.734383 carbon_python_sdk-0.2.1/carbon/type/external_source_items_order_by.py
--rw-r--r--   0        0        0      689 2024-05-30 19:55:10.734467 carbon_python_sdk-0.2.1/carbon/type/fetch_urls_response.py
--rw-r--r--   0        0        0      363 2024-05-30 19:55:10.734553 carbon_python_sdk-0.2.1/carbon/type/fetch_urls_response_urls.py
--rw-r--r--   0        0        0      384 2024-05-30 19:55:10.734636 carbon_python_sdk-0.2.1/carbon/type/file_content_types.py
--rw-r--r--   0        0        0      392 2024-05-30 19:55:10.734727 carbon_python_sdk-0.2.1/carbon/type/file_content_types_nullable.py
--rw-r--r--   0        0        0      759 2024-05-30 19:55:10.734812 carbon_python_sdk-0.2.1/carbon/type/file_formats.py
--rw-r--r--   0        0        0      767 2024-05-30 19:55:10.734899 carbon_python_sdk-0.2.1/carbon/type/file_formats_nullable.py
--rw-r--r--   0        0        0      823 2024-05-30 19:55:10.734986 carbon_python_sdk-0.2.1/carbon/type/file_statistics.py
--rw-r--r--   0        0        0      863 2024-05-30 19:55:10.735071 carbon_python_sdk-0.2.1/carbon/type/file_statistics_nullable.py
--rw-r--r--   0        0        0     1035 2024-05-30 19:55:10.735149 carbon_python_sdk-0.2.1/carbon/type/file_sync_config.py
--rw-r--r--   0        0        0     1075 2024-05-30 19:55:10.735231 carbon_python_sdk-0.2.1/carbon/type/file_sync_config_nullable.py
--rw-r--r--   0        0        0      427 2024-05-30 19:55:10.735319 carbon_python_sdk-0.2.1/carbon/type/files_query_user_files_deprecated_response.py
--rw-r--r--   0        0        0     1449 2024-05-30 19:55:10.735395 carbon_python_sdk-0.2.1/carbon/type/fresh_desk_connect_request.py
--rw-r--r--   0        0        0      669 2024-05-30 19:55:10.735480 carbon_python_sdk-0.2.1/carbon/type/freskdesk_authentication.py
--rw-r--r--   0        0        0      565 2024-05-30 19:55:10.735567 carbon_python_sdk-0.2.1/carbon/type/generic_success_response.py
--rw-r--r--   0        0        0     2735 2024-05-30 19:55:10.735646 carbon_python_sdk-0.2.1/carbon/type/get_embedding_documents_body.py
--rw-r--r--   0        0        0      391 2024-05-30 19:55:10.735727 carbon_python_sdk-0.2.1/carbon/type/get_embedding_documents_body_file_ids.py
--rw-r--r--   0        0        0      397 2024-05-30 19:55:10.735811 carbon_python_sdk-0.2.1/carbon/type/get_embedding_documents_body_parent_file_ids.py
--rw-r--r--   0        0        0      416 2024-05-30 19:55:10.735893 carbon_python_sdk-0.2.1/carbon/type/get_embedding_documents_body_query_vector.py
--rw-r--r--   0        0        0      359 2024-05-30 19:55:10.735977 carbon_python_sdk-0.2.1/carbon/type/get_embedding_documents_body_tags.py
--rw-r--r--   0        0        0      670 2024-05-30 19:55:10.736057 carbon_python_sdk-0.2.1/carbon/type/gitbook_authetication.py
--rw-r--r--   0        0        0     1272 2024-05-30 19:55:10.736135 carbon_python_sdk-0.2.1/carbon/type/gitbook_connect_request.py
--rw-r--r--   0        0        0     1168 2024-05-30 19:55:10.736210 carbon_python_sdk-0.2.1/carbon/type/gitbook_sync_request.py
--rw-r--r--   0        0        0      368 2024-05-30 19:55:10.736413 carbon_python_sdk-0.2.1/carbon/type/gitbook_sync_request_space_ids.py
--rw-r--r--   0        0        0      661 2024-05-30 19:55:10.736499 carbon_python_sdk-0.2.1/carbon/type/github_authentication.py
--rw-r--r--   0        0        0      709 2024-05-30 19:55:10.736584 carbon_python_sdk-0.2.1/carbon/type/github_connect_request.py
--rw-r--r--   0        0        0      711 2024-05-30 19:55:10.736666 carbon_python_sdk-0.2.1/carbon/type/github_fetch_repos_request.py
--rw-r--r--   0        0        0      370 2024-05-30 19:55:10.736748 carbon_python_sdk-0.2.1/carbon/type/github_fetch_repos_request_repos.py
--rw-r--r--   0        0        0     1351 2024-05-30 19:55:10.736838 carbon_python_sdk-0.2.1/carbon/type/gmail_sync_input.py
--rw-r--r--   0        0        0      371 2024-05-30 19:55:10.736920 carbon_python_sdk-0.2.1/carbon/type/helpdesk_file_types.py
--rw-r--r--   0        0        0      630 2024-05-30 19:55:10.736998 carbon_python_sdk-0.2.1/carbon/type/http_validation_error.py
--rw-r--r--   0        0        0      636 2024-05-30 19:55:10.737075 carbon_python_sdk-0.2.1/carbon/type/hybrid_search_tuning_params.py
--rw-r--r--   0        0        0      676 2024-05-30 19:55:10.737161 carbon_python_sdk-0.2.1/carbon/type/hybrid_search_tuning_params_nullable.py
--rw-r--r--   0        0        0     1025 2024-05-30 19:55:10.737267 carbon_python_sdk-0.2.1/carbon/type/list_data_source_items_request.py
--rw-r--r--   0        0        0      695 2024-05-30 19:55:10.737365 carbon_python_sdk-0.2.1/carbon/type/list_data_source_items_response.py
--rw-r--r--   0        0        0      854 2024-05-30 19:55:10.737453 carbon_python_sdk-0.2.1/carbon/type/list_items_filters.py
--rw-r--r--   0        0        0      386 2024-05-30 19:55:10.737544 carbon_python_sdk-0.2.1/carbon/type/list_items_filters_external_ids.py
--rw-r--r--   0        0        0      378 2024-05-30 19:55:10.737629 carbon_python_sdk-0.2.1/carbon/type/list_items_filters_ids.py
--rw-r--r--   0        0        0      944 2024-05-30 19:55:10.737725 carbon_python_sdk-0.2.1/carbon/type/list_items_filters_nullable.py
--rw-r--r--   0        0        0      394 2024-05-30 19:55:10.737810 carbon_python_sdk-0.2.1/carbon/type/list_items_filters_nullable_external_ids.py
--rw-r--r--   0        0        0      386 2024-05-30 19:55:10.737892 carbon_python_sdk-0.2.1/carbon/type/list_items_filters_nullable_ids.py
--rw-r--r--   0        0        0      544 2024-05-30 19:55:10.737971 carbon_python_sdk-0.2.1/carbon/type/list_request.py
--rw-r--r--   0        0        0      587 2024-05-30 19:55:10.738049 carbon_python_sdk-0.2.1/carbon/type/list_response.py
--rw-r--r--   0        0        0      709 2024-05-30 19:55:10.738140 carbon_python_sdk-0.2.1/carbon/type/modify_user_configuration_input.py
--rw-r--r--   0        0        0      358 2024-05-30 19:57:32.279999 carbon_python_sdk-0.2.1/carbon/type/multi_modal_embedding_generators.py
--rw-r--r--   0        0        0      665 2024-05-30 19:55:10.738325 carbon_python_sdk-0.2.1/carbon/type/notion_authentication.py
--rw-r--r--   0        0        0      696 2024-05-30 19:55:10.738415 carbon_python_sdk-0.2.1/carbon/type/o_auth_authentication.py
--rw-r--r--   0        0        0     3249 2024-05-30 19:57:32.280188 carbon_python_sdk-0.2.1/carbon/type/o_auth_url_request.py
--rw-r--r--   0        0        0      356 2024-05-30 19:55:10.738598 carbon_python_sdk-0.2.1/carbon/type/order_dir.py
--rw-r--r--   0        0        0      358 2024-05-30 19:55:10.738686 carbon_python_sdk-0.2.1/carbon/type/order_dir_v2.py
--rw-r--r--   0        0        0     1922 2024-05-30 19:55:10.738771 carbon_python_sdk-0.2.1/carbon/type/organization_response.py
--rw-r--r--   0        0        0     1567 2024-05-30 19:55:10.738863 carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_api.py
--rw-r--r--   0        0        0      937 2024-05-30 19:55:10.738956 carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_filters.py
--rw-r--r--   0        0        0      395 2024-05-30 19:55:10.739056 carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_filters_ids.py
--rw-r--r--   0        0        0      401 2024-05-30 19:55:10.739155 carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_order_by_columns.py
--rw-r--r--   0        0        0     1070 2024-05-30 19:55:10.739251 carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_query_input.py
--rw-r--r--   0        0        0      767 2024-05-30 19:55:10.739344 carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_response.py
--rw-r--r--   0        0        0      759 2024-05-30 19:55:10.739432 carbon_python_sdk-0.2.1/carbon/type/organization_user_file_tag_create.py
--rw-r--r--   0        0        0      363 2024-05-30 19:55:10.739524 carbon_python_sdk-0.2.1/carbon/type/organization_user_file_tag_create_tags.py
--rw-r--r--   0        0        0      767 2024-05-30 19:55:10.739615 carbon_python_sdk-0.2.1/carbon/type/organization_user_file_tags_remove.py
--rw-r--r--   0        0        0      376 2024-05-30 19:55:10.739708 carbon_python_sdk-0.2.1/carbon/type/organization_user_file_tags_remove_tags.py
--rw-r--r--   0        0        0     5041 2024-05-30 19:55:10.739821 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters.py
--rw-r--r--   0        0        0      408 2024-05-30 19:55:10.739921 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters_external_file_ids.py
--rw-r--r--   0        0        0      396 2024-05-30 19:55:10.740140 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters_ids.py
--rw-r--r--   0        0        0      421 2024-05-30 19:55:10.740237 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters_organization_user_data_source_id.py
--rw-r--r--   0        0        0      406 2024-05-30 19:55:10.740331 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters_parent_file_ids.py
--rw-r--r--   0        0        0      403 2024-05-30 19:55:10.740422 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters_request_ids.py
--rw-r--r--   0        0        0      368 2024-05-30 19:55:10.740513 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters_tags.py
--rw-r--r--   0        0        0      440 2024-05-30 19:55:10.740610 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_order_by_types.py
--rw-r--r--   0        0        0     1228 2024-05-30 19:55:10.740699 carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_query_input.py
--rw-r--r--   0        0        0      531 2024-05-30 19:55:10.740789 carbon_python_sdk-0.2.1/carbon/type/outh_url_response.py
--rw-r--r--   0        0        0     1395 2024-05-30 19:55:10.740877 carbon_python_sdk-0.2.1/carbon/type/outlook_sync_input.py
--rw-r--r--   0        0        0      519 2024-05-30 19:55:10.740972 carbon_python_sdk-0.2.1/carbon/type/pagination.py
--rw-r--r--   0        0        0      560 2024-05-30 19:55:10.741065 carbon_python_sdk-0.2.1/carbon/type/presigned_url_response.py
--rw-r--r--   0        0        0      900 2024-05-30 19:55:10.741147 carbon_python_sdk-0.2.1/carbon/type/raw_text_input.py
--rw-r--r--   0        0        0      662 2024-05-30 19:55:10.741236 carbon_python_sdk-0.2.1/carbon/type/resync_file_query_input.py
--rw-r--r--   0        0        0      571 2024-05-30 19:55:10.741327 carbon_python_sdk-0.2.1/carbon/type/revoke_access_token_input.py
--rw-r--r--   0        0        0     1002 2024-05-30 19:55:10.741416 carbon_python_sdk-0.2.1/carbon/type/rss_feed_input.py
--rw-r--r--   0        0        0      681 2024-05-30 19:55:10.741501 carbon_python_sdk-0.2.1/carbon/type/s3_auth_request.py
--rw-r--r--   0        0        0      648 2024-05-30 19:55:10.741589 carbon_python_sdk-0.2.1/carbon/type/s3_authentication.py
--rw-r--r--   0        0        0     1521 2024-05-30 19:55:10.741681 carbon_python_sdk-0.2.1/carbon/type/s3_file_sync_input.py
--rw-r--r--   0        0        0      570 2024-05-30 19:55:10.741770 carbon_python_sdk-0.2.1/carbon/type/s3_get_file_input.py
--rw-r--r--   0        0        0      711 2024-05-30 19:55:10.741852 carbon_python_sdk-0.2.1/carbon/type/salesforce_authentication.py
--rw-r--r--   0        0        0      736 2024-05-30 19:55:10.741936 carbon_python_sdk-0.2.1/carbon/type/sharepoint_authentication.py
--rw-r--r--   0        0        0      433 2024-05-30 19:55:10.742150 carbon_python_sdk-0.2.1/carbon/type/simple_o_auth_data_sources.py
--rw-r--r--   0        0        0      831 2024-05-30 19:55:10.742234 carbon_python_sdk-0.2.1/carbon/type/single_chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0     1662 2024-05-30 19:55:10.742320 carbon_python_sdk-0.2.1/carbon/type/sitemap_scrape_request.py
--rw-r--r--   0        0        0      395 2024-05-30 19:55:10.742413 carbon_python_sdk-0.2.1/carbon/type/sitemap_scrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0      397 2024-05-30 19:55:10.742506 carbon_python_sdk-0.2.1/carbon/type/sitemap_scrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0      393 2024-05-30 19:55:10.742599 carbon_python_sdk-0.2.1/carbon/type/sitemap_scrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0      354 2024-05-30 19:55:10.742688 carbon_python_sdk-0.2.1/carbon/type/sitemap_scrape_request_tags.py
--rw-r--r--   0        0        0      561 2024-05-30 19:55:10.742772 carbon_python_sdk-0.2.1/carbon/type/sync_directory_request.py
--rw-r--r--   0        0        0      527 2024-05-30 19:55:10.742851 carbon_python_sdk-0.2.1/carbon/type/sync_files_ids.py
--rw-r--r--   0        0        0     1816 2024-05-30 19:55:10.742928 carbon_python_sdk-0.2.1/carbon/type/sync_files_request.py
--rw-r--r--   0        0        0     2058 2024-05-30 19:55:10.743003 carbon_python_sdk-0.2.1/carbon/type/sync_options.py
--rw-r--r--   0        0        0      665 2024-05-30 19:55:10.743083 carbon_python_sdk-0.2.1/carbon/type/text_embedding_generators.py
--rw-r--r--   0        0        0      548 2024-05-30 19:55:10.743156 carbon_python_sdk-0.2.1/carbon/type/token_response.py
--rw-r--r--   0        0        0      697 2024-05-30 19:55:10.743235 carbon_python_sdk-0.2.1/carbon/type/update_organization_input.py
--rw-r--r--   0        0        0     1513 2024-05-30 19:55:10.743311 carbon_python_sdk-0.2.1/carbon/type/update_users_input.py
--rw-r--r--   0        0        0      369 2024-05-30 19:55:10.743392 carbon_python_sdk-0.2.1/carbon/type/update_users_input_customer_ids.py
--rw-r--r--   0        0        0     1133 2024-05-30 19:55:10.743472 carbon_python_sdk-0.2.1/carbon/type/upload_file_from_url_input.py
--rw-r--r--   0        0        0     1396 2024-05-30 19:55:10.743550 carbon_python_sdk-0.2.1/carbon/type/user_configuration.py
--rw-r--r--   0        0        0     1436 2024-05-30 19:55:10.743633 carbon_python_sdk-0.2.1/carbon/type/user_configuration_nullable.py
--rw-r--r--   0        0        0     2555 2024-05-30 19:55:10.743721 carbon_python_sdk-0.2.1/carbon/type/user_file.py
--rw-r--r--   0        0        0      422 2024-05-30 19:55:10.743804 carbon_python_sdk-0.2.1/carbon/type/user_file_embedding_properties.py
--rw-r--r--   0        0        0      586 2024-05-30 19:55:10.743882 carbon_python_sdk-0.2.1/carbon/type/user_files_v2.py
--rw-r--r--   0        0        0      548 2024-05-30 19:55:10.743961 carbon_python_sdk-0.2.1/carbon/type/user_request_content.py
--rw-r--r--   0        0        0     2011 2024-05-30 19:55:10.744037 carbon_python_sdk-0.2.1/carbon/type/user_response.py
--rw-r--r--   0        0        0      442 2024-05-30 19:55:10.744210 carbon_python_sdk-0.2.1/carbon/type/user_response_auto_sync_enabled_sources.py
--rw-r--r--   0        0        0      371 2024-05-30 19:55:10.744288 carbon_python_sdk-0.2.1/carbon/type/user_response_unique_file_tags.py
--rw-r--r--   0        0        0      439 2024-05-30 19:55:10.744368 carbon_python_sdk-0.2.1/carbon/type/utilities_scrape_web_request.py
--rw-r--r--   0        0        0      633 2024-05-30 19:55:10.744444 carbon_python_sdk-0.2.1/carbon/type/validation_error.py
--rw-r--r--   0        0        0      379 2024-05-30 19:55:10.744521 carbon_python_sdk-0.2.1/carbon/type/validation_error_loc.py
--rw-r--r--   0        0        0      719 2024-05-30 19:55:10.744607 carbon_python_sdk-0.2.1/carbon/type/webhook.py
--rw-r--r--   0        0        0      613 2024-05-30 19:55:10.744686 carbon_python_sdk-0.2.1/carbon/type/webhook_filters.py
--rw-r--r--   0        0        0      376 2024-05-30 19:55:10.744761 carbon_python_sdk-0.2.1/carbon/type/webhook_filters_ids.py
--rw-r--r--   0        0        0      722 2024-05-30 19:55:10.744835 carbon_python_sdk-0.2.1/carbon/type/webhook_no_key.py
--rw-r--r--   0        0        0      382 2024-05-30 19:55:10.744922 carbon_python_sdk-0.2.1/carbon/type/webhook_order_by_columns.py
--rw-r--r--   0        0        0      855 2024-05-30 19:55:10.745007 carbon_python_sdk-0.2.1/carbon/type/webhook_query_input.py
--rw-r--r--   0        0        0      644 2024-05-30 19:55:10.745092 carbon_python_sdk-0.2.1/carbon/type/webhook_query_response.py
--rw-r--r--   0        0        0      367 2024-05-30 19:55:10.745172 carbon_python_sdk-0.2.1/carbon/type/webhook_status.py
--rw-r--r--   0        0        0     1633 2024-05-30 19:55:10.745252 carbon_python_sdk-0.2.1/carbon/type/webscrape_request.py
--rw-r--r--   0        0        0      391 2024-05-30 19:55:10.745335 carbon_python_sdk-0.2.1/carbon/type/webscrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0      393 2024-05-30 19:55:10.745418 carbon_python_sdk-0.2.1/carbon/type/webscrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0      389 2024-05-30 19:55:10.745498 carbon_python_sdk-0.2.1/carbon/type/webscrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0      350 2024-05-30 19:55:10.745575 carbon_python_sdk-0.2.1/carbon/type/webscrape_request_tags.py
--rw-r--r--   0        0        0      675 2024-05-30 19:55:10.745769 carbon_python_sdk-0.2.1/carbon/type/white_labeling_response.py
--rw-r--r--   0        0        0      826 2024-05-30 19:55:10.745849 carbon_python_sdk-0.2.1/carbon/type/youtube_transcript_response.py
--rw-r--r--   0        0        0      551 2024-05-30 19:55:10.745926 carbon_python_sdk-0.2.1/carbon/type/youtube_transcript_response_raw_transcript.py
--rw-r--r--   0        0        0      372 2024-05-30 19:55:10.746010 carbon_python_sdk-0.2.1/carbon/type/youtube_transcript_response_raw_transcript_item.py
--rw-r--r--   0        0        0      667 2024-05-30 19:55:10.746088 carbon_python_sdk-0.2.1/carbon/type/zendesk_authentication.py
--rw-r--r--   0        0        0      711 2024-05-30 19:55:10.746171 carbon_python_sdk-0.2.1/carbon/type/zotero_authentication.py
--rw-r--r--   0        0        0      514 2024-05-30 19:55:10.746253 carbon_python_sdk-0.2.1/carbon/type_util.py
--rw-r--r--   0        0        0     3162 2024-05-30 19:55:10.746335 carbon_python_sdk-0.2.1/carbon/validation_metadata.py
--rw-r--r--   0        0        0      746 2024-05-30 19:57:32.280490 carbon_python_sdk-0.2.1/pyproject.toml
--rw-r--r--   0        0        0   113755 1970-01-01 00:00:00.000000 carbon_python_sdk-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-06-01 01:24:51.408113 carbon_python_sdk-0.2.2/LICENSE
+-rw-r--r--   0        0        0   113849 2024-06-01 01:36:07.368170 carbon_python_sdk-0.2.2/README.md
+-rw-r--r--   0        0        0      675 2024-06-01 01:36:07.368410 carbon_python_sdk-0.2.2/carbon/__init__.py
+-rw-r--r--   0        0        0    76940 2024-06-01 01:36:07.369783 carbon_python_sdk-0.2.2/carbon/api_client.py
+-rw-r--r--   0        0        0      663 2024-06-01 01:24:51.273600 carbon_python_sdk-0.2.2/carbon/api_response.py
+-rw-r--r--   0        0        0      214 2024-06-01 01:24:51.273694 carbon_python_sdk-0.2.2/carbon/apis/__init__.py
+-rw-r--r--   0        0        0    11353 2024-06-01 01:36:07.370261 carbon_python_sdk-0.2.2/carbon/apis/path_to_api.py
+-rw-r--r--   0        0        0      233 2024-06-01 01:24:51.273950 carbon_python_sdk-0.2.2/carbon/apis/paths/__init__.py
+-rw-r--r--   0        0        0      101 2024-06-01 01:24:51.274038 carbon_python_sdk-0.2.2/carbon/apis/paths/add_webhook.py
+-rw-r--r--   0        0        0      114 2024-06-01 01:24:51.274122 carbon_python_sdk-0.2.2/carbon/apis/paths/auth_v1_access_token.py
+-rw-r--r--   0        0        0      118 2024-06-01 01:24:51.274206 carbon_python_sdk-0.2.2/carbon/apis/paths/auth_v1_white_labeling.py
+-rw-r--r--   0        0        0      119 2024-06-01 01:24:51.274293 carbon_python_sdk-0.2.2/carbon/apis/paths/create_user_file_tags.py
+-rw-r--r--   0        0        0      103 2024-06-01 01:24:51.274378 carbon_python_sdk-0.2.2/carbon/apis/paths/delete_files.py
+-rw-r--r--   0        0        0      108 2024-06-01 01:24:51.274472 carbon_python_sdk-0.2.2/carbon/apis/paths/delete_files_v2.py
+-rw-r--r--   0        0        0      119 2024-06-01 01:24:51.274563 carbon_python_sdk-0.2.2/carbon/apis/paths/delete_user_file_tags.py
+-rw-r--r--   0        0        0      103 2024-06-01 01:24:51.274651 carbon_python_sdk-0.2.2/carbon/apis/paths/delete_users.py
+-rw-r--r--   0        0        0      133 2024-06-01 01:24:51.274732 carbon_python_sdk-0.2.2/carbon/apis/paths/delete_webhook_webhook_id.py
+-rw-r--r--   0        0        0      120 2024-06-01 01:24:51.274814 carbon_python_sdk-0.2.2/carbon/apis/paths/deletefile_file_id.py
+-rw-r--r--   0        0        0      100 2024-06-01 01:24:51.274891 carbon_python_sdk-0.2.2/carbon/apis/paths/embeddings.py
+-rw-r--r--   0        0        0       96 2024-06-01 01:24:51.274970 carbon_python_sdk-0.2.2/carbon/apis/paths/fetch_urls.py
+-rw-r--r--   0        0        0      123 2024-06-01 01:24:51.275051 carbon_python_sdk-0.2.2/carbon/apis/paths/fetch_youtube_transcript.py
+-rw-r--r--   0        0        0       89 2024-06-01 01:24:51.275131 carbon_python_sdk-0.2.2/carbon/apis/paths/health.py
+-rw-r--r--   0        0        0      134 2024-06-01 01:24:51.275210 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_confluence_list.py
+-rw-r--r--   0        0        0      134 2024-06-01 01:24:51.275291 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_confluence_sync.py
+-rw-r--r--   0        0        0      119 2024-06-01 01:24:51.275373 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_connect.py
+-rw-r--r--   0        0        0      124 2024-06-01 01:24:51.275453 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_files_sync.py
+-rw-r--r--   0        0        0      123 2024-06-01 01:24:51.275533 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_freshdesk.py
+-rw-r--r--   0        0        0      119 2024-06-01 01:24:51.275618 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_gitbook.py
+-rw-r--r--   0        0        0      129 2024-06-01 01:24:51.275702 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_gitbook_spaces.py
+-rw-r--r--   0        0        0      128 2024-06-01 01:24:51.275782 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_gitbook_sync.py
+-rw-r--r--   0        0        0      117 2024-06-01 01:24:51.275870 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_github.py
+-rw-r--r--   0        0        0      125 2024-06-01 01:24:51.275961 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_github_repos.py
+-rw-r--r--   0        0        0      137 2024-06-01 01:24:51.276049 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_github_sync_repos.py
+-rw-r--r--   0        0        0      124 2024-06-01 01:24:51.276133 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_gmail_sync.py
+-rw-r--r--   0        0        0      134 2024-06-01 01:24:51.276232 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_gmail_user_labels.py
+-rw-r--r--   0        0        0      124 2024-06-01 01:24:51.276330 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_items_list.py
+-rw-r--r--   0        0        0      124 2024-06-01 01:24:51.276417 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_items_sync.py
+-rw-r--r--   0        0        0      137 2024-06-01 01:36:07.370664 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_items_sync_cancel.py
+-rw-r--r--   0        0        0      122 2024-06-01 01:24:51.276604 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_oauth_url.py
+-rw-r--r--   0        0        0      128 2024-06-01 01:24:51.276691 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_outlook_sync.py
+-rw-r--r--   0        0        0      146 2024-06-01 01:24:51.276776 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_outlook_user_categories.py
+-rw-r--r--   0        0        0      140 2024-06-01 01:24:51.276869 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_outlook_user_folders.py
+-rw-r--r--   0        0        0      120 2024-06-01 01:24:51.276968 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_rss_feed.py
+-rw-r--r--   0        0        0      109 2024-06-01 01:24:51.277078 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_s3.py
+-rw-r--r--   0        0        0      120 2024-06-01 01:24:51.277178 carbon_python_sdk-0.2.2/carbon/apis/paths/integrations_s3_files.py
+-rw-r--r--   0        0        0      128 2024-06-01 01:24:51.277276 carbon_python_sdk-0.2.2/carbon/apis/paths/modify_user_configuration.py
+-rw-r--r--   0        0        0      101 2024-06-01 01:24:51.277364 carbon_python_sdk-0.2.2/carbon/apis/paths/organization.py
+-rw-r--r--   0        0        0      125 2024-06-01 01:24:51.277480 carbon_python_sdk-0.2.2/carbon/apis/paths/organization_statistics.py
+-rw-r--r--   0        0        0      117 2024-06-01 01:24:51.277594 carbon_python_sdk-0.2.2/carbon/apis/paths/organization_update.py
+-rw-r--r--   0        0        0      112 2024-06-01 01:24:51.277688 carbon_python_sdk-0.2.2/carbon/apis/paths/parsed_file_file_id.py
+-rw-r--r--   0        0        0      106 2024-06-01 01:24:51.277789 carbon_python_sdk-0.2.2/carbon/apis/paths/process_sitemap.py
+-rw-r--r--   0        0        0      106 2024-06-01 01:24:51.277893 carbon_python_sdk-0.2.2/carbon/apis/paths/raw_file_file_id.py
+-rw-r--r--   0        0        0      101 2024-06-01 01:24:51.277986 carbon_python_sdk-0.2.2/carbon/apis/paths/resync_file.py
+-rw-r--r--   0        0        0      116 2024-06-01 01:24:51.278081 carbon_python_sdk-0.2.2/carbon/apis/paths/revoke_access_token.py
+-rw-r--r--   0        0        0      107 2024-06-01 01:24:51.278189 carbon_python_sdk-0.2.2/carbon/apis/paths/scrape_sitemap.py
+-rw-r--r--   0        0        0       98 2024-06-01 01:24:51.278288 carbon_python_sdk-0.2.2/carbon/apis/paths/search_urls.py
+-rw-r--r--   0        0        0      101 2024-06-01 01:24:51.278391 carbon_python_sdk-0.2.2/carbon/apis/paths/text_chunks.py
+-rw-r--r--   0        0        0      103 2024-06-01 01:24:51.278477 carbon_python_sdk-0.2.2/carbon/apis/paths/update_users.py
+-rw-r--r--   0        0        0      133 2024-06-01 01:24:51.278578 carbon_python_sdk-0.2.2/carbon/apis/paths/upload_chunks_and_embeddings.py
+-rw-r--r--   0        0        0      117 2024-06-01 01:24:51.278663 carbon_python_sdk-0.2.2/carbon/apis/paths/upload_file_from_url.py
+-rw-r--r--   0        0        0      101 2024-06-01 01:24:51.278753 carbon_python_sdk-0.2.2/carbon/apis/paths/upload_text.py
+-rw-r--r--   0        0        0      100 2024-06-01 01:24:51.278847 carbon_python_sdk-0.2.2/carbon/apis/paths/uploadfile.py
+-rw-r--r--   0        0        0       88 2024-06-01 01:24:51.278937 carbon_python_sdk-0.2.2/carbon/apis/paths/user.py
+-rw-r--r--   0        0        0      112 2024-06-01 01:24:51.279027 carbon_python_sdk-0.2.2/carbon/apis/paths/user_data_sources.py
+-rw-r--r--   0        0        0       99 2024-06-01 01:24:51.279116 carbon_python_sdk-0.2.2/carbon/apis/paths/user_files.py
+-rw-r--r--   0        0        0      104 2024-06-01 01:24:51.279212 carbon_python_sdk-0.2.2/carbon/apis/paths/user_files_v2.py
+-rw-r--r--   0        0        0       99 2024-06-01 01:24:51.279299 carbon_python_sdk-0.2.2/carbon/apis/paths/web_scrape.py
+-rw-r--r--   0        0        0       96 2024-06-01 01:24:51.279391 carbon_python_sdk-0.2.2/carbon/apis/paths/webhooks.py
+-rw-r--r--   0        0        0     2044 2024-06-01 01:24:51.279477 carbon_python_sdk-0.2.2/carbon/apis/tag_to_api.py
+-rw-r--r--   0        0        0      655 2024-06-01 01:24:51.279577 carbon_python_sdk-0.2.2/carbon/apis/tags/__init__.py
+-rw-r--r--   0        0        0      125 2024-06-01 01:24:51.279660 carbon_python_sdk-0.2.2/carbon/apis/tags/auth_api.py
+-rw-r--r--   0        0        0      671 2024-06-01 01:24:51.279740 carbon_python_sdk-0.2.2/carbon/apis/tags/auth_api_generated.py
+-rw-r--r--   0        0        0      493 2024-06-01 01:24:51.279818 carbon_python_sdk-0.2.2/carbon/apis/tags/auth_api_raw.py
+-rw-r--r--   0        0        0      154 2024-06-01 01:24:51.279899 carbon_python_sdk-0.2.2/carbon/apis/tags/data_sources_api.py
+-rw-r--r--   0        0        0      717 2024-06-01 01:24:51.279985 carbon_python_sdk-0.2.2/carbon/apis/tags/data_sources_api_generated.py
+-rw-r--r--   0        0        0      510 2024-06-01 01:24:51.280070 carbon_python_sdk-0.2.2/carbon/apis/tags/data_sources_api_raw.py
+-rw-r--r--   0        0        0      149 2024-06-01 01:24:51.280159 carbon_python_sdk-0.2.2/carbon/apis/tags/embeddings_api.py
+-rw-r--r--   0        0        0      806 2024-06-01 01:24:51.280314 carbon_python_sdk-0.2.2/carbon/apis/tags/embeddings_api_generated.py
+-rw-r--r--   0        0        0      610 2024-06-01 01:24:51.280429 carbon_python_sdk-0.2.2/carbon/apis/tags/embeddings_api_raw.py
+-rw-r--r--   0        0        0      129 2024-06-01 01:24:51.280532 carbon_python_sdk-0.2.2/carbon/apis/tags/files_api.py
+-rw-r--r--   0        0        0     1495 2024-06-01 01:24:51.280635 carbon_python_sdk-0.2.2/carbon/apis/tags/files_api_generated.py
+-rw-r--r--   0        0        0     1379 2024-06-01 01:24:51.280736 carbon_python_sdk-0.2.2/carbon/apis/tags/files_api_raw.py
+-rw-r--r--   0        0        0      133 2024-06-01 01:24:51.280820 carbon_python_sdk-0.2.2/carbon/apis/tags/health_api.py
+-rw-r--r--   0        0        0      558 2024-06-01 01:24:51.280912 carbon_python_sdk-0.2.2/carbon/apis/tags/health_api_generated.py
+-rw-r--r--   0        0        0      366 2024-06-01 01:24:51.281007 carbon_python_sdk-0.2.2/carbon/apis/tags/health_api_raw.py
+-rw-r--r--   0        0        0      157 2024-06-01 01:24:51.281105 carbon_python_sdk-0.2.2/carbon/apis/tags/integrations_api.py
+-rw-r--r--   0        0        0     2573 2024-06-01 01:36:07.370853 carbon_python_sdk-0.2.2/carbon/apis/tags/integrations_api_generated.py
+-rw-r--r--   0        0        0     2489 2024-06-01 01:36:07.371033 carbon_python_sdk-0.2.2/carbon/apis/tags/integrations_api_raw.py
+-rw-r--r--   0        0        0      161 2024-06-01 01:24:51.281387 carbon_python_sdk-0.2.2/carbon/apis/tags/organizations_api.py
+-rw-r--r--   0        0        0      747 2024-06-01 01:24:51.281478 carbon_python_sdk-0.2.2/carbon/apis/tags/organizations_api_generated.py
+-rw-r--r--   0        0        0      539 2024-06-01 01:24:51.281574 carbon_python_sdk-0.2.2/carbon/apis/tags/organizations_api_raw.py
+-rw-r--r--   0        0        0      129 2024-06-01 01:24:51.281656 carbon_python_sdk-0.2.2/carbon/apis/tags/users_api.py
+-rw-r--r--   0        0        0      781 2024-06-01 01:24:51.281748 carbon_python_sdk-0.2.2/carbon/apis/tags/users_api_generated.py
+-rw-r--r--   0        0        0      611 2024-06-01 01:24:51.281852 carbon_python_sdk-0.2.2/carbon/apis/tags/users_api_raw.py
+-rw-r--r--   0        0        0      145 2024-06-01 01:24:51.281952 carbon_python_sdk-0.2.2/carbon/apis/tags/utilities_api.py
+-rw-r--r--   0        0        0      984 2024-06-01 01:24:51.282045 carbon_python_sdk-0.2.2/carbon/apis/tags/utilities_api_generated.py
+-rw-r--r--   0        0        0      810 2024-06-01 01:24:51.282130 carbon_python_sdk-0.2.2/carbon/apis/tags/utilities_api_raw.py
+-rw-r--r--   0        0        0      141 2024-06-01 01:24:51.282216 carbon_python_sdk-0.2.2/carbon/apis/tags/webhooks_api.py
+-rw-r--r--   0        0        0      713 2024-06-01 01:24:51.282314 carbon_python_sdk-0.2.2/carbon/apis/tags/webhooks_api_generated.py
+-rw-r--r--   0        0        0      525 2024-06-01 01:24:51.282406 carbon_python_sdk-0.2.2/carbon/apis/tags/webhooks_api_raw.py
+-rw-r--r--   0        0        0     1986 2024-06-01 01:24:51.282497 carbon_python_sdk-0.2.2/carbon/client.py
+-rw-r--r--   0        0        0     1986 2024-06-01 01:24:51.282584 carbon_python_sdk-0.2.2/carbon/client.pyi
+-rw-r--r--   0        0        0      676 2024-06-01 01:24:51.282671 carbon_python_sdk-0.2.2/carbon/client_custom.py
+-rw-r--r--   0        0        0    17804 2024-06-01 01:36:07.371264 carbon_python_sdk-0.2.2/carbon/configuration.py
+-rw-r--r--   0        0        0     7679 2024-06-01 01:24:51.282945 carbon_python_sdk-0.2.2/carbon/exceptions.py
+-rw-r--r--   0        0        0     2274 2024-06-01 01:24:51.283031 carbon_python_sdk-0.2.2/carbon/exceptions_base.py
+-rw-r--r--   0        0        0      340 2024-06-01 01:24:51.283278 carbon_python_sdk-0.2.2/carbon/model/__init__.py
+-rw-r--r--   0        0        0     2282 2024-06-01 01:24:51.283368 carbon_python_sdk-0.2.2/carbon/model/add_webhook_props.py
+-rw-r--r--   0        0        0     2282 2024-06-01 01:24:51.283457 carbon_python_sdk-0.2.2/carbon/model/add_webhook_props.pyi
+-rw-r--r--   0        0        0     2371 2024-06-01 01:24:51.283546 carbon_python_sdk-0.2.2/carbon/model/body_create_upload_file_uploadfile_post.py
+-rw-r--r--   0        0        0     2371 2024-06-01 01:24:51.283636 carbon_python_sdk-0.2.2/carbon/model/body_create_upload_file_uploadfile_post.pyi
+-rw-r--r--   0        0        0     4752 2024-06-01 01:24:51.283739 carbon_python_sdk-0.2.2/carbon/model/chunk_properties.py
+-rw-r--r--   0        0        0     4752 2024-06-01 01:24:51.283846 carbon_python_sdk-0.2.2/carbon/model/chunk_properties.pyi
+-rw-r--r--   0        0        0     4359 2024-06-01 01:24:51.283943 carbon_python_sdk-0.2.2/carbon/model/chunk_properties_nullable.py
+-rw-r--r--   0        0        0     4359 2024-06-01 01:24:51.284041 carbon_python_sdk-0.2.2/carbon/model/chunk_properties_nullable.pyi
+-rw-r--r--   0        0        0     4319 2024-06-01 01:24:51.284141 carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings.py
+-rw-r--r--   0        0        0     4319 2024-06-01 01:24:51.284237 carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings.pyi
+-rw-r--r--   0        0        0     1100 2024-06-01 01:24:51.284314 carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings_embedding.py
+-rw-r--r--   0        0        0     1100 2024-06-01 01:24:51.284391 carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings_embedding.pyi
+-rw-r--r--   0        0        0     6672 2024-06-01 01:24:51.284499 carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0     6672 2024-06-01 01:24:51.284609 carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings_upload_input.pyi
+-rw-r--r--   0        0        0     1521 2024-06-01 01:24:51.284706 carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.py
+-rw-r--r--   0        0        0     1521 2024-06-01 01:24:51.284799 carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.pyi
+-rw-r--r--   0        0        0      548 2024-06-01 01:24:51.284890 carbon_python_sdk-0.2.2/carbon/model/configuration_keys.py
+-rw-r--r--   0        0        0      548 2024-06-01 01:24:51.284982 carbon_python_sdk-0.2.2/carbon/model/configuration_keys.pyi
+-rw-r--r--   0        0        0     4861 2024-06-01 01:24:51.285087 carbon_python_sdk-0.2.2/carbon/model/confluence_authentication.py
+-rw-r--r--   0        0        0     4861 2024-06-01 01:24:51.285189 carbon_python_sdk-0.2.2/carbon/model/confluence_authentication.pyi
+-rw-r--r--   0        0        0     6269 2024-06-01 01:24:51.285298 carbon_python_sdk-0.2.2/carbon/model/connect_data_source_input.py
+-rw-r--r--   0        0        0     6269 2024-06-01 01:24:51.285408 carbon_python_sdk-0.2.2/carbon/model/connect_data_source_input.pyi
+-rw-r--r--   0        0        0     3763 2024-06-01 01:24:51.285503 carbon_python_sdk-0.2.2/carbon/model/connect_data_source_response.py
+-rw-r--r--   0        0        0     3763 2024-06-01 01:24:51.285587 carbon_python_sdk-0.2.2/carbon/model/connect_data_source_response.pyi
+-rw-r--r--   0        0        0     1369 2024-06-01 01:24:51.285677 carbon_python_sdk-0.2.2/carbon/model/custom_credentials_type.py
+-rw-r--r--   0        0        0     1114 2024-06-01 01:24:51.285765 carbon_python_sdk-0.2.2/carbon/model/custom_credentials_type.pyi
+-rw-r--r--   0        0        0      554 2024-06-01 01:24:51.285860 carbon_python_sdk-0.2.2/carbon/model/data_source_extended_input.py
+-rw-r--r--   0        0        0      554 2024-06-01 01:24:51.285942 carbon_python_sdk-0.2.2/carbon/model/data_source_extended_input.pyi
+-rw-r--r--   0        0        0     1183 2024-06-01 01:24:51.286020 carbon_python_sdk-0.2.2/carbon/model/data_source_last_sync_actions.py
+-rw-r--r--   0        0        0      998 2024-06-01 01:24:51.286103 carbon_python_sdk-0.2.2/carbon/model/data_source_last_sync_actions.pyi
+-rw-r--r--   0        0        0     1256 2024-06-01 01:24:51.286193 carbon_python_sdk-0.2.2/carbon/model/data_source_sync_statuses.py
+-rw-r--r--   0        0        0     1033 2024-06-01 01:24:51.286284 carbon_python_sdk-0.2.2/carbon/model/data_source_sync_statuses.pyi
+-rw-r--r--   0        0        0     6578 2024-06-01 01:24:51.286389 carbon_python_sdk-0.2.2/carbon/model/data_source_type.py
+-rw-r--r--   0        0        0     4915 2024-06-01 01:24:51.286498 carbon_python_sdk-0.2.2/carbon/model/data_source_type.pyi
+-rw-r--r--   0        0        0     6953 2024-06-01 01:24:51.286605 carbon_python_sdk-0.2.2/carbon/model/data_source_type_nullable.py
+-rw-r--r--   0        0        0     6953 2024-06-01 01:24:51.286716 carbon_python_sdk-0.2.2/carbon/model/data_source_type_nullable.pyi
+-rw-r--r--   0        0        0     6047 2024-06-01 01:24:51.286824 carbon_python_sdk-0.2.2/carbon/model/delete_files_query_input.py
+-rw-r--r--   0        0        0     6047 2024-06-01 01:24:51.286927 carbon_python_sdk-0.2.2/carbon/model/delete_files_query_input.pyi
+-rw-r--r--   0        0        0     1097 2024-06-01 01:24:51.287019 carbon_python_sdk-0.2.2/carbon/model/delete_files_query_input_file_ids.py
+-rw-r--r--   0        0        0     1097 2024-06-01 01:24:51.287124 carbon_python_sdk-0.2.2/carbon/model/delete_files_query_input_file_ids.pyi
+-rw-r--r--   0        0        0     3161 2024-06-01 01:24:51.287213 carbon_python_sdk-0.2.2/carbon/model/delete_files_v2_query_input.py
+-rw-r--r--   0        0        0     3161 2024-06-01 01:24:51.287307 carbon_python_sdk-0.2.2/carbon/model/delete_files_v2_query_input.pyi
+-rw-r--r--   0        0        0     2600 2024-06-01 01:24:51.287397 carbon_python_sdk-0.2.2/carbon/model/delete_users_input.py
+-rw-r--r--   0        0        0     2600 2024-06-01 01:24:51.287489 carbon_python_sdk-0.2.2/carbon/model/delete_users_input.pyi
+-rw-r--r--   0        0        0     1199 2024-06-01 01:24:51.287593 carbon_python_sdk-0.2.2/carbon/model/delete_users_input_customer_ids.py
+-rw-r--r--   0        0        0     1199 2024-06-01 01:24:51.287689 carbon_python_sdk-0.2.2/carbon/model/delete_users_input_customer_ids.pyi
+-rw-r--r--   0        0        0     3902 2024-06-01 01:24:51.287772 carbon_python_sdk-0.2.2/carbon/model/directory_item.py
+-rw-r--r--   0        0        0     3902 2024-06-01 01:24:51.287851 carbon_python_sdk-0.2.2/carbon/model/directory_item.pyi
+-rw-r--r--   0        0        0    16065 2024-06-01 01:24:51.287991 carbon_python_sdk-0.2.2/carbon/model/document_response.py
+-rw-r--r--   0        0        0    16065 2024-06-01 01:24:51.288128 carbon_python_sdk-0.2.2/carbon/model/document_response.pyi
+-rw-r--r--   0        0        0     3350 2024-06-01 01:24:51.288208 carbon_python_sdk-0.2.2/carbon/model/document_response_list.py
+-rw-r--r--   0        0        0     3350 2024-06-01 01:24:51.288299 carbon_python_sdk-0.2.2/carbon/model/document_response_list.pyi
+-rw-r--r--   0        0        0     7489 2024-06-01 01:24:51.288404 carbon_python_sdk-0.2.2/carbon/model/document_response_tags.py
+-rw-r--r--   0        0        0     7489 2024-06-01 01:24:51.288523 carbon_python_sdk-0.2.2/carbon/model/document_response_tags.pyi
+-rw-r--r--   0        0        0     1088 2024-06-01 01:24:51.288603 carbon_python_sdk-0.2.2/carbon/model/document_response_vector.py
+-rw-r--r--   0        0        0     1088 2024-06-01 01:24:51.288683 carbon_python_sdk-0.2.2/carbon/model/document_response_vector.pyi
+-rw-r--r--   0        0        0     6594 2024-06-01 01:24:51.288778 carbon_python_sdk-0.2.2/carbon/model/embedding_and_chunk.py
+-rw-r--r--   0        0        0     6594 2024-06-01 01:24:51.288877 carbon_python_sdk-0.2.2/carbon/model/embedding_and_chunk.pyi
+-rw-r--r--   0        0        0     1096 2024-06-01 01:24:51.288963 carbon_python_sdk-0.2.2/carbon/model/embedding_and_chunk_embedding.py
+-rw-r--r--   0        0        0     1096 2024-06-01 01:24:51.289053 carbon_python_sdk-0.2.2/carbon/model/embedding_and_chunk_embedding.pyi
+-rw-r--r--   0        0        0     3163 2024-06-01 01:24:51.289147 carbon_python_sdk-0.2.2/carbon/model/embedding_generators.py
+-rw-r--r--   0        0        0     2260 2024-06-01 01:24:51.289242 carbon_python_sdk-0.2.2/carbon/model/embedding_generators.pyi
+-rw-r--r--   0        0        0     3543 2024-06-01 01:24:51.289336 carbon_python_sdk-0.2.2/carbon/model/embedding_generators_nullable.py
+-rw-r--r--   0        0        0     3543 2024-06-01 01:24:51.289425 carbon_python_sdk-0.2.2/carbon/model/embedding_generators_nullable.pyi
+-rw-r--r--   0        0        0     4307 2024-06-01 01:24:51.289529 carbon_python_sdk-0.2.2/carbon/model/embedding_properties.py
+-rw-r--r--   0        0        0     4307 2024-06-01 01:24:51.289634 carbon_python_sdk-0.2.2/carbon/model/embedding_properties.pyi
+-rw-r--r--   0        0        0     3267 2024-06-01 01:24:51.289715 carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_filters.py
+-rw-r--r--   0        0        0     3267 2024-06-01 01:24:51.289798 carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_filters.pyi
+-rw-r--r--   0        0        0     1141 2024-06-01 01:24:51.289878 carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_order_by_columns.py
+-rw-r--r--   0        0        0      956 2024-06-01 01:24:51.289960 carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_order_by_columns.pyi
+-rw-r--r--   0        0        0     5194 2024-06-01 01:24:51.290055 carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_query_input.py
+-rw-r--r--   0        0        0     5194 2024-06-01 01:24:51.290158 carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_query_input.pyi
+-rw-r--r--   0        0        0     3847 2024-06-01 01:24:51.290238 carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_response.py
+-rw-r--r--   0        0        0     3847 2024-06-01 01:24:51.290322 carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_response.pyi
+-rw-r--r--   0        0        0     1944 2024-06-01 01:24:51.290408 carbon_python_sdk-0.2.2/carbon/model/external_file_sync_statuses.py
+-rw-r--r--   0        0        0     1503 2024-06-01 01:24:51.290488 carbon_python_sdk-0.2.2/carbon/model/external_file_sync_statuses.pyi
+-rw-r--r--   0        0        0    17950 2024-06-01 01:24:51.290636 carbon_python_sdk-0.2.2/carbon/model/external_source_item.py
+-rw-r--r--   0        0        0    17950 2024-06-01 01:24:51.290781 carbon_python_sdk-0.2.2/carbon/model/external_source_item.pyi
+-rw-r--r--   0        0        0     1102 2024-06-01 01:24:51.290863 carbon_python_sdk-0.2.2/carbon/model/external_source_items_order_by.py
+-rw-r--r--   0        0        0      933 2024-06-01 01:24:51.290939 carbon_python_sdk-0.2.2/carbon/model/external_source_items_order_by.pyi
+-rw-r--r--   0        0        0     4287 2024-06-01 01:24:51.291039 carbon_python_sdk-0.2.2/carbon/model/fetch_urls_response.py
+-rw-r--r--   0        0        0     4287 2024-06-01 01:24:51.291134 carbon_python_sdk-0.2.2/carbon/model/fetch_urls_response.pyi
+-rw-r--r--   0        0        0     1187 2024-06-01 01:24:51.291211 carbon_python_sdk-0.2.2/carbon/model/fetch_urls_response_urls.py
+-rw-r--r--   0        0        0     1187 2024-06-01 01:24:51.291290 carbon_python_sdk-0.2.2/carbon/model/fetch_urls_response_urls.pyi
+-rw-r--r--   0        0        0     1166 2024-06-01 01:24:51.291365 carbon_python_sdk-0.2.2/carbon/model/file_content_types.py
+-rw-r--r--   0        0        0      985 2024-06-01 01:24:51.291448 carbon_python_sdk-0.2.2/carbon/model/file_content_types.pyi
+-rw-r--r--   0        0        0     1543 2024-06-01 01:36:07.371674 carbon_python_sdk-0.2.2/carbon/model/file_content_types_nullable.py
+-rw-r--r--   0        0        0     1543 2024-06-01 01:36:07.371981 carbon_python_sdk-0.2.2/carbon/model/file_content_types_nullable.pyi
+-rw-r--r--   0        0        0     5789 2024-06-01 01:24:51.291706 carbon_python_sdk-0.2.2/carbon/model/file_formats.py
+-rw-r--r--   0        0        0     4344 2024-06-01 01:24:51.291804 carbon_python_sdk-0.2.2/carbon/model/file_formats.pyi
+-rw-r--r--   0        0        0     6161 2024-06-01 01:24:51.291906 carbon_python_sdk-0.2.2/carbon/model/file_formats_nullable.py
+-rw-r--r--   0        0        0     6161 2024-06-01 01:24:51.292001 carbon_python_sdk-0.2.2/carbon/model/file_formats_nullable.pyi
+-rw-r--r--   0        0        0     8647 2024-06-01 01:24:51.292116 carbon_python_sdk-0.2.2/carbon/model/file_statistics.py
+-rw-r--r--   0        0        0     8647 2024-06-01 01:24:51.292233 carbon_python_sdk-0.2.2/carbon/model/file_statistics.pyi
+-rw-r--r--   0        0        0     8000 2024-06-01 01:24:51.292337 carbon_python_sdk-0.2.2/carbon/model/file_statistics_nullable.py
+-rw-r--r--   0        0        0     8000 2024-06-01 01:24:51.292434 carbon_python_sdk-0.2.2/carbon/model/file_statistics_nullable.pyi
+-rw-r--r--   0        0        0     4847 2024-06-01 01:24:51.292529 carbon_python_sdk-0.2.2/carbon/model/file_sync_config.py
+-rw-r--r--   0        0        0     4847 2024-06-01 01:24:51.292626 carbon_python_sdk-0.2.2/carbon/model/file_sync_config.pyi
+-rw-r--r--   0        0        0     5047 2024-06-01 01:24:51.292727 carbon_python_sdk-0.2.2/carbon/model/file_sync_config_nullable.py
+-rw-r--r--   0        0        0     5047 2024-06-01 01:24:51.292831 carbon_python_sdk-0.2.2/carbon/model/file_sync_config_nullable.pyi
+-rw-r--r--   0        0        0     1283 2024-06-01 01:24:51.292919 carbon_python_sdk-0.2.2/carbon/model/files_query_user_files_deprecated_response.py
+-rw-r--r--   0        0        0     1283 2024-06-01 01:24:51.293006 carbon_python_sdk-0.2.2/carbon/model/files_query_user_files_deprecated_response.pyi
+-rw-r--r--   0        0        0    15514 2024-06-01 01:24:51.293139 carbon_python_sdk-0.2.2/carbon/model/fresh_desk_connect_request.py
+-rw-r--r--   0        0        0    15514 2024-06-01 01:24:51.293281 carbon_python_sdk-0.2.2/carbon/model/fresh_desk_connect_request.pyi
+-rw-r--r--   0        0        0     3529 2024-06-01 01:24:51.293373 carbon_python_sdk-0.2.2/carbon/model/freskdesk_authentication.py
+-rw-r--r--   0        0        0     3529 2024-06-01 01:24:51.293458 carbon_python_sdk-0.2.2/carbon/model/freskdesk_authentication.pyi
+-rw-r--r--   0        0        0     2362 2024-06-01 01:24:51.293537 carbon_python_sdk-0.2.2/carbon/model/generic_success_response.py
+-rw-r--r--   0        0        0     2362 2024-06-01 01:24:51.293621 carbon_python_sdk-0.2.2/carbon/model/generic_success_response.pyi
+-rw-r--r--   0        0        0    15782 2024-06-01 01:24:51.293758 carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body.py
+-rw-r--r--   0        0        0    15631 2024-06-01 01:24:51.293896 carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body.pyi
+-rw-r--r--   0        0        0     1159 2024-06-01 01:24:51.293980 carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_file_ids.py
+-rw-r--r--   0        0        0     1159 2024-06-01 01:24:51.294062 carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_file_ids.pyi
+-rw-r--r--   0        0        0     1264 2024-06-01 01:24:51.294149 carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_parent_file_ids.py
+-rw-r--r--   0        0        0     1264 2024-06-01 01:24:51.294234 carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_parent_file_ids.pyi
+-rw-r--r--   0        0        0     1377 2024-06-01 01:24:51.294318 carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_query_vector.py
+-rw-r--r--   0        0        0     1377 2024-06-01 01:24:51.294402 carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_query_vector.pyi
+-rw-r--r--   0        0        0     6490 2024-06-01 01:24:51.294497 carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_tags.py
+-rw-r--r--   0        0        0     6490 2024-06-01 01:24:51.294597 carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_tags.pyi
+-rw-r--r--   0        0        0     3779 2024-06-01 01:24:51.294681 carbon_python_sdk-0.2.2/carbon/model/gitbook_authetication.py
+-rw-r--r--   0        0        0     3779 2024-06-01 01:24:51.294765 carbon_python_sdk-0.2.2/carbon/model/gitbook_authetication.pyi
+-rw-r--r--   0        0        0    14852 2024-06-01 01:24:51.294898 carbon_python_sdk-0.2.2/carbon/model/gitbook_connect_request.py
+-rw-r--r--   0        0        0    14852 2024-06-01 01:24:51.295026 carbon_python_sdk-0.2.2/carbon/model/gitbook_connect_request.pyi
+-rw-r--r--   0        0        0    13012 2024-06-01 01:24:51.295153 carbon_python_sdk-0.2.2/carbon/model/gitbook_sync_request.py
+-rw-r--r--   0        0        0    13012 2024-06-01 01:24:51.295287 carbon_python_sdk-0.2.2/carbon/model/gitbook_sync_request.pyi
+-rw-r--r--   0        0        0     1220 2024-06-01 01:24:51.295369 carbon_python_sdk-0.2.2/carbon/model/gitbook_sync_request_space_ids.py
+-rw-r--r--   0        0        0     1197 2024-06-01 01:24:51.295448 carbon_python_sdk-0.2.2/carbon/model/gitbook_sync_request_space_ids.pyi
+-rw-r--r--   0        0        0     3635 2024-06-01 01:24:51.295530 carbon_python_sdk-0.2.2/carbon/model/github_authentication.py
+-rw-r--r--   0        0        0     3635 2024-06-01 01:24:51.295610 carbon_python_sdk-0.2.2/carbon/model/github_authentication.pyi
+-rw-r--r--   0        0        0     3626 2024-06-01 01:24:51.295691 carbon_python_sdk-0.2.2/carbon/model/github_connect_request.py
+-rw-r--r--   0        0        0     3626 2024-06-01 01:24:51.295773 carbon_python_sdk-0.2.2/carbon/model/github_connect_request.pyi
+-rw-r--r--   0        0        0     3792 2024-06-01 01:24:51.295855 carbon_python_sdk-0.2.2/carbon/model/github_fetch_repos_request.py
+-rw-r--r--   0        0        0     3792 2024-06-01 01:24:51.295936 carbon_python_sdk-0.2.2/carbon/model/github_fetch_repos_request.pyi
+-rw-r--r--   0        0        0     1246 2024-06-01 01:24:51.296019 carbon_python_sdk-0.2.2/carbon/model/github_fetch_repos_request_repos.py
+-rw-r--r--   0        0        0     1201 2024-06-01 01:24:51.296102 carbon_python_sdk-0.2.2/carbon/model/github_fetch_repos_request_repos.pyi
+-rw-r--r--   0        0        0    16085 2024-06-01 01:24:51.296233 carbon_python_sdk-0.2.2/carbon/model/gmail_sync_input.py
+-rw-r--r--   0        0        0    16085 2024-06-01 01:24:51.296365 carbon_python_sdk-0.2.2/carbon/model/gmail_sync_input.pyi
+-rw-r--r--   0        0        0      963 2024-06-01 01:24:51.296450 carbon_python_sdk-0.2.2/carbon/model/helpdesk_file_types.py
+-rw-r--r--   0        0        0      834 2024-06-01 01:24:51.296530 carbon_python_sdk-0.2.2/carbon/model/helpdesk_file_types.pyi
+-rw-r--r--   0        0        0     3251 2024-06-01 01:24:51.296610 carbon_python_sdk-0.2.2/carbon/model/http_validation_error.py
+-rw-r--r--   0        0        0     3251 2024-06-01 01:24:51.296687 carbon_python_sdk-0.2.2/carbon/model/http_validation_error.pyi
+-rw-r--r--   0        0        0     2974 2024-06-01 01:24:51.296768 carbon_python_sdk-0.2.2/carbon/model/hybrid_search_tuning_params.py
+-rw-r--r--   0        0        0     2974 2024-06-01 01:24:51.296849 carbon_python_sdk-0.2.2/carbon/model/hybrid_search_tuning_params.pyi
+-rw-r--r--   0        0        0     2907 2024-06-01 01:24:51.296934 carbon_python_sdk-0.2.2/carbon/model/hybrid_search_tuning_params_nullable.py
+-rw-r--r--   0        0        0     2907 2024-06-01 01:24:51.297021 carbon_python_sdk-0.2.2/carbon/model/hybrid_search_tuning_params_nullable.pyi
+-rw-r--r--   0        0        0     6323 2024-06-01 01:24:51.297125 carbon_python_sdk-0.2.2/carbon/model/list_data_source_items_request.py
+-rw-r--r--   0        0        0     6323 2024-06-01 01:24:51.297232 carbon_python_sdk-0.2.2/carbon/model/list_data_source_items_request.pyi
+-rw-r--r--   0        0        0     3820 2024-06-01 01:24:51.297316 carbon_python_sdk-0.2.2/carbon/model/list_data_source_items_response.py
+-rw-r--r--   0        0        0     3820 2024-06-01 01:24:51.297399 carbon_python_sdk-0.2.2/carbon/model/list_data_source_items_response.pyi
+-rw-r--r--   0        0        0     5498 2024-06-01 01:24:51.297498 carbon_python_sdk-0.2.2/carbon/model/list_items_filters.py
+-rw-r--r--   0        0        0     5498 2024-06-01 01:24:51.297595 carbon_python_sdk-0.2.2/carbon/model/list_items_filters.pyi
+-rw-r--r--   0        0        0     1095 2024-06-01 01:24:51.297682 carbon_python_sdk-0.2.2/carbon/model/list_items_filters_external_ids.py
+-rw-r--r--   0        0        0     1095 2024-06-01 01:24:51.297763 carbon_python_sdk-0.2.2/carbon/model/list_items_filters_external_ids.pyi
+-rw-r--r--   0        0        0     1079 2024-06-01 01:24:51.297843 carbon_python_sdk-0.2.2/carbon/model/list_items_filters_ids.py
+-rw-r--r--   0        0        0     1079 2024-06-01 01:24:51.297920 carbon_python_sdk-0.2.2/carbon/model/list_items_filters_ids.pyi
+-rw-r--r--   0        0        0     5708 2024-06-01 01:24:51.298016 carbon_python_sdk-0.2.2/carbon/model/list_items_filters_nullable.py
+-rw-r--r--   0        0        0     5708 2024-06-01 01:24:51.298110 carbon_python_sdk-0.2.2/carbon/model/list_items_filters_nullable.pyi
+-rw-r--r--   0        0        0     1111 2024-06-01 01:24:51.298195 carbon_python_sdk-0.2.2/carbon/model/list_items_filters_nullable_external_ids.py
+-rw-r--r--   0        0        0     1111 2024-06-01 01:24:51.298281 carbon_python_sdk-0.2.2/carbon/model/list_items_filters_nullable_external_ids.pyi
+-rw-r--r--   0        0        0     1095 2024-06-01 01:24:51.298360 carbon_python_sdk-0.2.2/carbon/model/list_items_filters_nullable_ids.py
+-rw-r--r--   0        0        0     1095 2024-06-01 01:24:51.298440 carbon_python_sdk-0.2.2/carbon/model/list_items_filters_nullable_ids.pyi
+-rw-r--r--   0        0        0     3613 2024-06-01 01:24:51.298517 carbon_python_sdk-0.2.2/carbon/model/list_request.py
+-rw-r--r--   0        0        0     3613 2024-06-01 01:24:51.298596 carbon_python_sdk-0.2.2/carbon/model/list_request.pyi
+-rw-r--r--   0        0        0     3228 2024-06-01 01:24:51.298677 carbon_python_sdk-0.2.2/carbon/model/list_response.py
+-rw-r--r--   0        0        0     3228 2024-06-01 01:24:51.298758 carbon_python_sdk-0.2.2/carbon/model/list_response.pyi
+-rw-r--r--   0        0        0     3129 2024-06-01 01:24:51.298840 carbon_python_sdk-0.2.2/carbon/model/modify_user_configuration_input.py
+-rw-r--r--   0        0        0     3129 2024-06-01 01:24:51.298917 carbon_python_sdk-0.2.2/carbon/model/modify_user_configuration_input.pyi
+-rw-r--r--   0        0        0      560 2024-06-01 01:24:51.298997 carbon_python_sdk-0.2.2/carbon/model/multi_modal_embedding_generators.py
+-rw-r--r--   0        0        0      560 2024-06-01 01:24:51.299075 carbon_python_sdk-0.2.2/carbon/model/multi_modal_embedding_generators.pyi
+-rw-r--r--   0        0        0     3699 2024-06-01 01:24:51.299155 carbon_python_sdk-0.2.2/carbon/model/notion_authentication.py
+-rw-r--r--   0        0        0     3699 2024-06-01 01:24:51.299232 carbon_python_sdk-0.2.2/carbon/model/notion_authentication.pyi
+-rw-r--r--   0        0        0     4300 2024-06-01 01:24:51.299329 carbon_python_sdk-0.2.2/carbon/model/o_auth_authentication.py
+-rw-r--r--   0        0        0     4300 2024-06-01 01:24:51.299426 carbon_python_sdk-0.2.2/carbon/model/o_auth_authentication.pyi
+-rw-r--r--   0        0        0    29598 2024-06-01 01:24:51.299780 carbon_python_sdk-0.2.2/carbon/model/o_auth_url_request.py
+-rw-r--r--   0        0        0    29598 2024-06-01 01:24:51.300028 carbon_python_sdk-0.2.2/carbon/model/o_auth_url_request.pyi
+-rw-r--r--   0        0        0      930 2024-06-01 01:24:51.300124 carbon_python_sdk-0.2.2/carbon/model/order_dir.py
+-rw-r--r--   0        0        0      813 2024-06-01 01:24:51.300212 carbon_python_sdk-0.2.2/carbon/model/order_dir.pyi
+-rw-r--r--   0        0        0      932 2024-06-01 01:24:51.300299 carbon_python_sdk-0.2.2/carbon/model/order_dir_v2.py
+-rw-r--r--   0        0        0      815 2024-06-01 01:24:51.300381 carbon_python_sdk-0.2.2/carbon/model/order_dir_v2.pyi
+-rw-r--r--   0        0        0    18921 2024-06-01 01:24:51.300531 carbon_python_sdk-0.2.2/carbon/model/organization_response.py
+-rw-r--r--   0        0        0    18921 2024-06-01 01:24:51.300684 carbon_python_sdk-0.2.2/carbon/model/organization_response.pyi
+-rw-r--r--   0        0        0    17065 2024-06-01 01:24:51.300851 carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_api.py
+-rw-r--r--   0        0        0    17065 2024-06-01 01:24:51.301007 carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_api.pyi
+-rw-r--r--   0        0        0     4467 2024-06-01 01:24:51.301108 carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_filters.py
+-rw-r--r--   0        0        0     4467 2024-06-01 01:24:51.301204 carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_filters.pyi
+-rw-r--r--   0        0        0     1113 2024-06-01 01:24:51.301288 carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_filters_ids.py
+-rw-r--r--   0        0        0     1113 2024-06-01 01:24:51.301371 carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_filters_ids.pyi
+-rw-r--r--   0        0        0     1014 2024-06-01 01:24:51.301460 carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_order_by_columns.py
+-rw-r--r--   0        0        0      871 2024-06-01 01:24:51.301541 carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_order_by_columns.pyi
+-rw-r--r--   0        0        0     4657 2024-06-01 01:24:51.301643 carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_query_input.py
+-rw-r--r--   0        0        0     4657 2024-06-01 01:24:51.301749 carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_query_input.pyi
+-rw-r--r--   0        0        0     3947 2024-06-01 01:24:51.301835 carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_response.py
+-rw-r--r--   0        0        0     3947 2024-06-01 01:24:51.301919 carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_response.pyi
+-rw-r--r--   0        0        0     3408 2024-06-01 01:24:51.302002 carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tag_create.py
+-rw-r--r--   0        0        0     3408 2024-06-01 01:24:51.302088 carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tag_create.pyi
+-rw-r--r--   0        0        0     6330 2024-06-01 01:24:51.302188 carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tag_create_tags.py
+-rw-r--r--   0        0        0     6330 2024-06-01 01:24:51.302287 carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tag_create_tags.pyi
+-rw-r--r--   0        0        0     3418 2024-06-01 01:24:51.302368 carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tags_remove.py
+-rw-r--r--   0        0        0     3418 2024-06-01 01:24:51.302449 carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tags_remove.pyi
+-rw-r--r--   0        0        0     1213 2024-06-01 01:24:51.302534 carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tags_remove_tags.py
+-rw-r--r--   0        0        0     1213 2024-06-01 01:24:51.302617 carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tags_remove_tags.pyi
+-rw-r--r--   0        0        0    21692 2024-06-01 01:24:51.302799 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters.py
+-rw-r--r--   0        0        0    21692 2024-06-01 01:24:51.303010 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters.pyi
+-rw-r--r--   0        0        0     1238 2024-06-01 01:24:51.303108 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_external_file_ids.py
+-rw-r--r--   0        0        0     1238 2024-06-01 01:24:51.303193 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_external_file_ids.pyi
+-rw-r--r--   0        0        0     1186 2024-06-01 01:24:51.303276 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_ids.py
+-rw-r--r--   0        0        0     1186 2024-06-01 01:24:51.303360 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_ids.pyi
+-rw-r--r--   0        0        0     1296 2024-06-01 01:24:51.303448 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.py
+-rw-r--r--   0        0        0     1296 2024-06-01 01:24:51.303539 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.pyi
+-rw-r--r--   0        0        0     1135 2024-06-01 01:24:51.303623 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.py
+-rw-r--r--   0        0        0     1135 2024-06-01 01:24:51.303709 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.pyi
+-rw-r--r--   0        0        0     1216 2024-06-01 01:24:51.303791 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_request_ids.py
+-rw-r--r--   0        0        0     1192 2024-06-01 01:24:51.303873 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_request_ids.pyi
+-rw-r--r--   0        0        0     6420 2024-06-01 01:24:51.303973 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_tags.py
+-rw-r--r--   0        0        0     6420 2024-06-01 01:24:51.304074 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_tags.pyi
+-rw-r--r--   0        0        0     1469 2024-06-01 01:24:51.304159 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_order_by_types.py
+-rw-r--r--   0        0        0     1198 2024-06-01 01:24:51.304243 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_order_by_types.pyi
+-rw-r--r--   0        0        0     8629 2024-06-01 01:24:51.304361 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_query_input.py
+-rw-r--r--   0        0        0     8629 2024-06-01 01:24:51.304480 carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_query_input.pyi
+-rw-r--r--   0        0        0     2378 2024-06-01 01:24:51.304563 carbon_python_sdk-0.2.2/carbon/model/outh_url_response.py
+-rw-r--r--   0        0        0     2378 2024-06-01 01:24:51.304642 carbon_python_sdk-0.2.2/carbon/model/outh_url_response.pyi
+-rw-r--r--   0        0        0    17193 2024-06-01 01:24:51.304787 carbon_python_sdk-0.2.2/carbon/model/outlook_sync_input.py
+-rw-r--r--   0        0        0    17193 2024-06-01 01:24:51.304942 carbon_python_sdk-0.2.2/carbon/model/outlook_sync_input.pyi
+-rw-r--r--   0        0        0     2807 2024-06-01 01:24:51.305029 carbon_python_sdk-0.2.2/carbon/model/pagination.py
+-rw-r--r--   0        0        0     2807 2024-06-01 01:24:51.305116 carbon_python_sdk-0.2.2/carbon/model/pagination.pyi
+-rw-r--r--   0        0        0     2452 2024-06-01 01:24:51.305194 carbon_python_sdk-0.2.2/carbon/model/presigned_url_response.py
+-rw-r--r--   0        0        0     2452 2024-06-01 01:24:51.305271 carbon_python_sdk-0.2.2/carbon/model/presigned_url_response.pyi
+-rw-r--r--   0        0        0    10223 2024-06-01 01:24:51.305385 carbon_python_sdk-0.2.2/carbon/model/raw_text_input.py
+-rw-r--r--   0        0        0    10151 2024-06-01 01:24:51.305501 carbon_python_sdk-0.2.2/carbon/model/raw_text_input.pyi
+-rw-r--r--   0        0        0     5578 2024-06-01 01:24:51.305599 carbon_python_sdk-0.2.2/carbon/model/resync_file_query_input.py
+-rw-r--r--   0        0        0     5578 2024-06-01 01:24:51.305698 carbon_python_sdk-0.2.2/carbon/model/resync_file_query_input.pyi
+-rw-r--r--   0        0        0     2489 2024-06-01 01:24:51.305782 carbon_python_sdk-0.2.2/carbon/model/revoke_access_token_input.py
+-rw-r--r--   0        0        0     2489 2024-06-01 01:24:51.305864 carbon_python_sdk-0.2.2/carbon/model/revoke_access_token_input.pyi
+-rw-r--r--   0        0        0    12076 2024-06-01 01:24:51.305976 carbon_python_sdk-0.2.2/carbon/model/rss_feed_input.py
+-rw-r--r--   0        0        0    12076 2024-06-01 01:24:51.306091 carbon_python_sdk-0.2.2/carbon/model/rss_feed_input.pyi
+-rw-r--r--   0        0        0     3724 2024-06-01 01:24:51.306174 carbon_python_sdk-0.2.2/carbon/model/s3_auth_request.py
+-rw-r--r--   0        0        0     3724 2024-06-01 01:24:51.306254 carbon_python_sdk-0.2.2/carbon/model/s3_auth_request.pyi
+-rw-r--r--   0        0        0     3739 2024-06-01 01:24:51.306333 carbon_python_sdk-0.2.2/carbon/model/s3_authentication.py
+-rw-r--r--   0        0        0     3739 2024-06-01 01:24:51.306410 carbon_python_sdk-0.2.2/carbon/model/s3_authentication.pyi
+-rw-r--r--   0        0        0    19565 2024-06-01 01:24:51.306559 carbon_python_sdk-0.2.2/carbon/model/s3_file_sync_input.py
+-rw-r--r--   0        0        0    19565 2024-06-01 01:24:51.306713 carbon_python_sdk-0.2.2/carbon/model/s3_file_sync_input.pyi
+-rw-r--r--   0        0        0     3936 2024-06-01 01:24:51.306802 carbon_python_sdk-0.2.2/carbon/model/s3_get_file_input.py
+-rw-r--r--   0        0        0     3936 2024-06-01 01:24:51.306883 carbon_python_sdk-0.2.2/carbon/model/s3_get_file_input.pyi
+-rw-r--r--   0        0        0     4813 2024-06-01 01:24:51.306980 carbon_python_sdk-0.2.2/carbon/model/salesforce_authentication.py
+-rw-r--r--   0        0        0     4813 2024-06-01 01:24:51.307078 carbon_python_sdk-0.2.2/carbon/model/salesforce_authentication.pyi
+-rw-r--r--   0        0        0     5449 2024-06-01 01:24:51.307221 carbon_python_sdk-0.2.2/carbon/model/sharepoint_authentication.py
+-rw-r--r--   0        0        0     5449 2024-06-01 01:24:51.307348 carbon_python_sdk-0.2.2/carbon/model/sharepoint_authentication.pyi
+-rw-r--r--   0        0        0     1566 2024-06-01 01:24:51.307442 carbon_python_sdk-0.2.2/carbon/model/simple_o_auth_data_sources.py
+-rw-r--r--   0        0        0     1263 2024-06-01 01:24:51.307524 carbon_python_sdk-0.2.2/carbon/model/simple_o_auth_data_sources.pyi
+-rw-r--r--   0        0        0     6587 2024-06-01 01:24:51.307635 carbon_python_sdk-0.2.2/carbon/model/single_chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0     6587 2024-06-01 01:24:51.307758 carbon_python_sdk-0.2.2/carbon/model/single_chunks_and_embeddings_upload_input.pyi
+-rw-r--r--   0        0        0    15650 2024-06-01 01:24:51.307909 carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request.py
+-rw-r--r--   0        0        0    15608 2024-06-01 01:24:51.308060 carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request.pyi
+-rw-r--r--   0        0        0     1113 2024-06-01 01:24:51.308161 carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0     1113 2024-06-01 01:24:51.308261 carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_css_classes_to_skip.pyi
+-rw-r--r--   0        0        0     1117 2024-06-01 01:24:51.308360 carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0     1117 2024-06-01 01:24:51.308458 carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_css_selectors_to_skip.pyi
+-rw-r--r--   0        0        0     1109 2024-06-01 01:24:51.308562 carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0     1109 2024-06-01 01:24:51.308660 carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_html_tags_to_skip.pyi
+-rw-r--r--   0        0        0     6392 2024-06-01 01:24:51.308772 carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_tags.py
+-rw-r--r--   0        0        0     6392 2024-06-01 01:24:51.308891 carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_tags.pyi
+-rw-r--r--   0        0        0     2485 2024-06-01 01:24:51.308986 carbon_python_sdk-0.2.2/carbon/model/sync_directory_request.py
+-rw-r--r--   0        0        0     2485 2024-06-01 01:24:51.309081 carbon_python_sdk-0.2.2/carbon/model/sync_directory_request.pyi
+-rw-r--r--   0        0        0     2784 2024-06-01 01:24:51.309176 carbon_python_sdk-0.2.2/carbon/model/sync_files_ids.py
+-rw-r--r--   0        0        0     2784 2024-06-01 01:24:51.309277 carbon_python_sdk-0.2.2/carbon/model/sync_files_ids.pyi
+-rw-r--r--   0        0        0    22189 2024-06-01 01:24:51.309463 carbon_python_sdk-0.2.2/carbon/model/sync_files_request.py
+-rw-r--r--   0        0        0    22189 2024-06-01 01:24:51.309650 carbon_python_sdk-0.2.2/carbon/model/sync_files_request.pyi
+-rw-r--r--   0        0        0    16413 2024-06-01 01:24:51.309814 carbon_python_sdk-0.2.2/carbon/model/sync_options.py
+-rw-r--r--   0        0        0    16413 2024-06-01 01:24:51.309981 carbon_python_sdk-0.2.2/carbon/model/sync_options.pyi
+-rw-r--r--   0        0        0     3009 2024-06-01 01:24:51.310082 carbon_python_sdk-0.2.2/carbon/model/text_embedding_generators.py
+-rw-r--r--   0        0        0     2160 2024-06-01 01:24:51.310180 carbon_python_sdk-0.2.2/carbon/model/text_embedding_generators.pyi
+-rw-r--r--   0        0        0     3042 2024-06-01 01:24:51.310277 carbon_python_sdk-0.2.2/carbon/model/token_response.py
+-rw-r--r--   0        0        0     3042 2024-06-01 01:24:51.310376 carbon_python_sdk-0.2.2/carbon/model/token_response.pyi
+-rw-r--r--   0        0        0     2620 2024-06-01 01:24:51.310474 carbon_python_sdk-0.2.2/carbon/model/update_organization_input.py
+-rw-r--r--   0        0        0     2620 2024-06-01 01:24:51.310569 carbon_python_sdk-0.2.2/carbon/model/update_organization_input.pyi
+-rw-r--r--   0        0        0     9214 2024-06-01 01:24:51.310740 carbon_python_sdk-0.2.2/carbon/model/update_users_input.py
+-rw-r--r--   0        0        0     9128 2024-06-01 01:24:51.310886 carbon_python_sdk-0.2.2/carbon/model/update_users_input.pyi
+-rw-r--r--   0        0        0     1267 2024-06-01 01:24:51.310993 carbon_python_sdk-0.2.2/carbon/model/update_users_input_customer_ids.py
+-rw-r--r--   0        0        0     1243 2024-06-01 01:24:51.311099 carbon_python_sdk-0.2.2/carbon/model/update_users_input_customer_ids.pyi
+-rw-r--r--   0        0        0    13659 2024-06-01 01:36:07.372456 carbon_python_sdk-0.2.2/carbon/model/upload_file_from_url_input.py
+-rw-r--r--   0        0        0    13659 2024-06-01 01:36:07.372595 carbon_python_sdk-0.2.2/carbon/model/upload_file_from_url_input.pyi
+-rw-r--r--   0        0        0     8405 2024-06-01 01:24:51.311555 carbon_python_sdk-0.2.2/carbon/model/user_configuration.py
+-rw-r--r--   0        0        0     8319 2024-06-01 01:24:51.311696 carbon_python_sdk-0.2.2/carbon/model/user_configuration.pyi
+-rw-r--r--   0        0        0     8665 2024-06-01 01:24:51.311828 carbon_python_sdk-0.2.2/carbon/model/user_configuration_nullable.py
+-rw-r--r--   0        0        0     8579 2024-06-01 01:24:51.311958 carbon_python_sdk-0.2.2/carbon/model/user_configuration_nullable.pyi
+-rw-r--r--   0        0        0    35549 2024-06-01 01:24:51.312304 carbon_python_sdk-0.2.2/carbon/model/user_file.py
+-rw-r--r--   0        0        0    35549 2024-06-01 01:24:51.312522 carbon_python_sdk-0.2.2/carbon/model/user_file.pyi
+-rw-r--r--   0        0        0     1650 2024-06-01 01:24:51.312610 carbon_python_sdk-0.2.2/carbon/model/user_file_embedding_properties.py
+-rw-r--r--   0        0        0     1650 2024-06-01 01:24:51.312691 carbon_python_sdk-0.2.2/carbon/model/user_file_embedding_properties.pyi
+-rw-r--r--   0        0        0     3751 2024-06-01 01:24:51.312773 carbon_python_sdk-0.2.2/carbon/model/user_files_v2.py
+-rw-r--r--   0        0        0     3751 2024-06-01 01:24:51.312853 carbon_python_sdk-0.2.2/carbon/model/user_files_v2.pyi
+-rw-r--r--   0        0        0     2416 2024-06-01 01:24:51.312934 carbon_python_sdk-0.2.2/carbon/model/user_request_content.py
+-rw-r--r--   0        0        0     2416 2024-06-01 01:24:51.313012 carbon_python_sdk-0.2.2/carbon/model/user_request_content.pyi
+-rw-r--r--   0        0        0    17500 2024-06-01 01:24:51.313165 carbon_python_sdk-0.2.2/carbon/model/user_response.py
+-rw-r--r--   0        0        0    17500 2024-06-01 01:24:51.313316 carbon_python_sdk-0.2.2/carbon/model/user_response.pyi
+-rw-r--r--   0        0        0     1511 2024-06-01 01:24:51.313402 carbon_python_sdk-0.2.2/carbon/model/user_response_auto_sync_enabled_sources.py
+-rw-r--r--   0        0        0     1511 2024-06-01 01:24:51.313490 carbon_python_sdk-0.2.2/carbon/model/user_response_auto_sync_enabled_sources.pyi
+-rw-r--r--   0        0        0     1246 2024-06-01 01:24:51.313569 carbon_python_sdk-0.2.2/carbon/model/user_response_unique_file_tags.py
+-rw-r--r--   0        0        0     1246 2024-06-01 01:24:51.313656 carbon_python_sdk-0.2.2/carbon/model/user_response_unique_file_tags.pyi
+-rw-r--r--   0        0        0     1315 2024-06-01 01:24:51.313742 carbon_python_sdk-0.2.2/carbon/model/utilities_scrape_web_request.py
+-rw-r--r--   0        0        0     1315 2024-06-01 01:24:51.313825 carbon_python_sdk-0.2.2/carbon/model/utilities_scrape_web_request.pyi
+-rw-r--r--   0        0        0     3352 2024-06-01 01:24:51.313904 carbon_python_sdk-0.2.2/carbon/model/validation_error.py
+-rw-r--r--   0        0        0     3352 2024-06-01 01:24:51.313989 carbon_python_sdk-0.2.2/carbon/model/validation_error.pyi
+-rw-r--r--   0        0        0     3149 2024-06-01 01:24:51.314117 carbon_python_sdk-0.2.2/carbon/model/validation_error_loc.py
+-rw-r--r--   0        0        0     3149 2024-06-01 01:24:51.314200 carbon_python_sdk-0.2.2/carbon/model/validation_error_loc.pyi
+-rw-r--r--   0        0        0     6973 2024-06-01 01:24:51.314304 carbon_python_sdk-0.2.2/carbon/model/webhook.py
+-rw-r--r--   0        0        0     6973 2024-06-01 01:24:51.314407 carbon_python_sdk-0.2.2/carbon/model/webhook.pyi
+-rw-r--r--   0        0        0     2396 2024-06-01 01:24:51.314490 carbon_python_sdk-0.2.2/carbon/model/webhook_filters.py
+-rw-r--r--   0        0        0     2396 2024-06-01 01:24:51.314574 carbon_python_sdk-0.2.2/carbon/model/webhook_filters.pyi
+-rw-r--r--   0        0        0     1075 2024-06-01 01:24:51.314659 carbon_python_sdk-0.2.2/carbon/model/webhook_filters_ids.py
+-rw-r--r--   0        0        0     1075 2024-06-01 01:24:51.314741 carbon_python_sdk-0.2.2/carbon/model/webhook_filters_ids.pyi
+-rw-r--r--   0        0        0     6395 2024-06-01 01:24:51.314859 carbon_python_sdk-0.2.2/carbon/model/webhook_no_key.py
+-rw-r--r--   0        0        0     6395 2024-06-01 01:24:51.314990 carbon_python_sdk-0.2.2/carbon/model/webhook_no_key.pyi
+-rw-r--r--   0        0        0      995 2024-06-01 01:24:51.315097 carbon_python_sdk-0.2.2/carbon/model/webhook_order_by_columns.py
+-rw-r--r--   0        0        0      852 2024-06-01 01:24:51.315198 carbon_python_sdk-0.2.2/carbon/model/webhook_order_by_columns.pyi
+-rw-r--r--   0        0        0     4347 2024-06-01 01:24:51.315331 carbon_python_sdk-0.2.2/carbon/model/webhook_query_input.py
+-rw-r--r--   0        0        0     4347 2024-06-01 01:24:51.315464 carbon_python_sdk-0.2.2/carbon/model/webhook_query_input.pyi
+-rw-r--r--   0        0        0     3798 2024-06-01 01:24:51.315552 carbon_python_sdk-0.2.2/carbon/model/webhook_query_response.py
+-rw-r--r--   0        0        0     3798 2024-06-01 01:24:51.315648 carbon_python_sdk-0.2.2/carbon/model/webhook_query_response.pyi
+-rw-r--r--   0        0        0      959 2024-06-01 01:24:51.315736 carbon_python_sdk-0.2.2/carbon/model/webhook_status.py
+-rw-r--r--   0        0        0      830 2024-06-01 01:24:51.315837 carbon_python_sdk-0.2.2/carbon/model/webhook_status.pyi
+-rw-r--r--   0        0        0    16894 2024-06-01 01:24:51.316051 carbon_python_sdk-0.2.2/carbon/model/webscrape_request.py
+-rw-r--r--   0        0        0    16810 2024-06-01 01:24:51.316277 carbon_python_sdk-0.2.2/carbon/model/webscrape_request.pyi
+-rw-r--r--   0        0        0     1105 2024-06-01 01:24:51.316388 carbon_python_sdk-0.2.2/carbon/model/webscrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0     1105 2024-06-01 01:24:51.316496 carbon_python_sdk-0.2.2/carbon/model/webscrape_request_css_classes_to_skip.pyi
+-rw-r--r--   0        0        0     1109 2024-06-01 01:24:51.316601 carbon_python_sdk-0.2.2/carbon/model/webscrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0     1109 2024-06-01 01:24:51.316704 carbon_python_sdk-0.2.2/carbon/model/webscrape_request_css_selectors_to_skip.pyi
+-rw-r--r--   0        0        0     1101 2024-06-01 01:24:51.316808 carbon_python_sdk-0.2.2/carbon/model/webscrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0     1101 2024-06-01 01:24:51.316912 carbon_python_sdk-0.2.2/carbon/model/webscrape_request_html_tags_to_skip.pyi
+-rw-r--r--   0        0        0     6384 2024-06-01 01:24:51.317038 carbon_python_sdk-0.2.2/carbon/model/webscrape_request_tags.py
+-rw-r--r--   0        0        0     6384 2024-06-01 01:24:51.317156 carbon_python_sdk-0.2.2/carbon/model/webscrape_request_tags.pyi
+-rw-r--r--   0        0        0     3117 2024-06-01 01:24:51.317261 carbon_python_sdk-0.2.2/carbon/model/white_labeling_response.py
+-rw-r--r--   0        0        0     3117 2024-06-01 01:24:51.317366 carbon_python_sdk-0.2.2/carbon/model/white_labeling_response.pyi
+-rw-r--r--   0        0        0     5401 2024-06-01 01:24:51.317510 carbon_python_sdk-0.2.2/carbon/model/youtube_transcript_response.py
+-rw-r--r--   0        0        0     5401 2024-06-01 01:24:51.317701 carbon_python_sdk-0.2.2/carbon/model/youtube_transcript_response.pyi
+-rw-r--r--   0        0        0     1375 2024-06-01 01:24:51.317836 carbon_python_sdk-0.2.2/carbon/model/youtube_transcript_response_raw_transcript.py
+-rw-r--r--   0        0        0     1375 2024-06-01 01:24:51.317953 carbon_python_sdk-0.2.2/carbon/model/youtube_transcript_response_raw_transcript.pyi
+-rw-r--r--   0        0        0     3326 2024-06-01 01:24:51.318051 carbon_python_sdk-0.2.2/carbon/model/youtube_transcript_response_raw_transcript_item.py
+-rw-r--r--   0        0        0     3326 2024-06-01 01:24:51.318185 carbon_python_sdk-0.2.2/carbon/model/youtube_transcript_response_raw_transcript_item.pyi
+-rw-r--r--   0        0        0     3653 2024-06-01 01:24:51.318286 carbon_python_sdk-0.2.2/carbon/model/zendesk_authentication.py
+-rw-r--r--   0        0        0     3653 2024-06-01 01:24:51.318385 carbon_python_sdk-0.2.2/carbon/model/zendesk_authentication.pyi
+-rw-r--r--   0        0        0     4907 2024-06-01 01:24:51.318513 carbon_python_sdk-0.2.2/carbon/model/zotero_authentication.py
+-rw-r--r--   0        0        0     4907 2024-06-01 01:24:51.318661 carbon_python_sdk-0.2.2/carbon/model/zotero_authentication.pyi
+-rw-r--r--   0        0        0    13560 2024-06-01 01:24:51.318943 carbon_python_sdk-0.2.2/carbon/models/__init__.py
+-rw-r--r--   0        0        0    25721 2024-06-01 01:36:07.372958 carbon_python_sdk-0.2.2/carbon/operation_parameter_map.py
+-rw-r--r--   0        0        0     3218 2024-06-01 01:36:07.373155 carbon_python_sdk-0.2.2/carbon/paths/__init__.py
+-rw-r--r--   0        0        0      293 2024-06-01 01:24:51.319393 carbon_python_sdk-0.2.2/carbon/paths/add_webhook/__init__.py
+-rw-r--r--   0        0        0    13948 2024-06-01 01:24:51.319542 carbon_python_sdk-0.2.2/carbon/paths/add_webhook/post.py
+-rw-r--r--   0        0        0    13811 2024-06-01 01:24:51.319727 carbon_python_sdk-0.2.2/carbon/paths/add_webhook/post.pyi
+-rw-r--r--   0        0        0      311 2024-06-01 01:24:51.319837 carbon_python_sdk-0.2.2/carbon/paths/auth_v1_access_token/__init__.py
+-rw-r--r--   0        0        0    11830 2024-06-01 01:24:51.319993 carbon_python_sdk-0.2.2/carbon/paths/auth_v1_access_token/get.py
+-rw-r--r--   0        0        0    11656 2024-06-01 01:24:51.320141 carbon_python_sdk-0.2.2/carbon/paths/auth_v1_access_token/get.pyi
+-rw-r--r--   0        0        0      315 2024-06-01 01:24:51.320258 carbon_python_sdk-0.2.2/carbon/paths/auth_v1_white_labeling/__init__.py
+-rw-r--r--   0        0        0    11193 2024-06-01 01:24:51.320403 carbon_python_sdk-0.2.2/carbon/paths/auth_v1_white_labeling/get.py
+-rw-r--r--   0        0        0    11049 2024-06-01 01:24:51.320560 carbon_python_sdk-0.2.2/carbon/paths/auth_v1_white_labeling/get.pyi
+-rw-r--r--   0        0        0      313 2024-06-01 01:24:51.320668 carbon_python_sdk-0.2.2/carbon/paths/create_user_file_tags/__init__.py
+-rw-r--r--   0        0        0    15880 2024-06-01 01:24:51.320825 carbon_python_sdk-0.2.2/carbon/paths/create_user_file_tags/post.py
+-rw-r--r--   0        0        0    15706 2024-06-01 01:24:51.321029 carbon_python_sdk-0.2.2/carbon/paths/create_user_file_tags/post.pyi
+-rw-r--r--   0        0        0      295 2024-06-01 01:24:51.321291 carbon_python_sdk-0.2.2/carbon/paths/delete_files/__init__.py
+-rw-r--r--   0        0        0    19307 2024-06-01 01:24:51.321509 carbon_python_sdk-0.2.2/carbon/paths/delete_files/post.py
+-rw-r--r--   0        0        0    19133 2024-06-01 01:24:51.321769 carbon_python_sdk-0.2.2/carbon/paths/delete_files/post.pyi
+-rw-r--r--   0        0        0      301 2024-06-01 01:24:51.321896 carbon_python_sdk-0.2.2/carbon/paths/delete_files_v2/__init__.py
+-rw-r--r--   0        0        0    15967 2024-06-01 01:24:51.322174 carbon_python_sdk-0.2.2/carbon/paths/delete_files_v2/post.py
+-rw-r--r--   0        0        0    15793 2024-06-01 01:24:51.322399 carbon_python_sdk-0.2.2/carbon/paths/delete_files_v2/post.pyi
+-rw-r--r--   0        0        0      313 2024-06-01 01:24:51.322508 carbon_python_sdk-0.2.2/carbon/paths/delete_user_file_tags/__init__.py
+-rw-r--r--   0        0        0    15814 2024-06-01 01:24:51.322648 carbon_python_sdk-0.2.2/carbon/paths/delete_user_file_tags/post.py
+-rw-r--r--   0        0        0    15640 2024-06-01 01:24:51.322799 carbon_python_sdk-0.2.2/carbon/paths/delete_user_file_tags/post.pyi
+-rw-r--r--   0        0        0      295 2024-06-01 01:24:51.322897 carbon_python_sdk-0.2.2/carbon/paths/delete_users/__init__.py
+-rw-r--r--   0        0        0    14899 2024-06-01 01:24:51.323039 carbon_python_sdk-0.2.2/carbon/paths/delete_users/post.py
+-rw-r--r--   0        0        0    14762 2024-06-01 01:24:51.323191 carbon_python_sdk-0.2.2/carbon/paths/delete_users/post.pyi
+-rw-r--r--   0        0        0      321 2024-06-01 01:24:51.323283 carbon_python_sdk-0.2.2/carbon/paths/delete_webhook_webhook_id/__init__.py
+-rw-r--r--   0        0        0    14359 2024-06-01 01:24:51.323421 carbon_python_sdk-0.2.2/carbon/paths/delete_webhook_webhook_id/delete.py
+-rw-r--r--   0        0        0    14222 2024-06-01 01:24:51.323563 carbon_python_sdk-0.2.2/carbon/paths/delete_webhook_webhook_id/delete.pyi
+-rw-r--r--   0        0        0      307 2024-06-01 01:24:51.323651 carbon_python_sdk-0.2.2/carbon/paths/deletefile_file_id/__init__.py
+-rw-r--r--   0        0        0    14552 2024-06-01 01:24:51.323786 carbon_python_sdk-0.2.2/carbon/paths/deletefile_file_id/delete.py
+-rw-r--r--   0        0        0    14378 2024-06-01 01:24:51.323919 carbon_python_sdk-0.2.2/carbon/paths/deletefile_file_id/delete.pyi
+-rw-r--r--   0        0        0      291 2024-06-01 01:24:51.324005 carbon_python_sdk-0.2.2/carbon/paths/embeddings/__init__.py
+-rw-r--r--   0        0        0    29199 2024-06-01 01:24:51.324205 carbon_python_sdk-0.2.2/carbon/paths/embeddings/post.py
+-rw-r--r--   0        0        0    29025 2024-06-01 01:24:51.324396 carbon_python_sdk-0.2.2/carbon/paths/embeddings/post.pyi
+-rw-r--r--   0        0        0      291 2024-06-01 01:24:51.324480 carbon_python_sdk-0.2.2/carbon/paths/fetch_urls/__init__.py
+-rw-r--r--   0        0        0    14466 2024-06-01 01:24:51.324607 carbon_python_sdk-0.2.2/carbon/paths/fetch_urls/get.py
+-rw-r--r--   0        0        0    14292 2024-06-01 01:24:51.324746 carbon_python_sdk-0.2.2/carbon/paths/fetch_urls/get.pyi
+-rw-r--r--   0        0        0      319 2024-06-01 01:24:51.324840 carbon_python_sdk-0.2.2/carbon/paths/fetch_youtube_transcript/__init__.py
+-rw-r--r--   0        0        0    15695 2024-06-01 01:24:51.324983 carbon_python_sdk-0.2.2/carbon/paths/fetch_youtube_transcript/get.py
+-rw-r--r--   0        0        0    15521 2024-06-01 01:24:51.325137 carbon_python_sdk-0.2.2/carbon/paths/fetch_youtube_transcript/get.pyi
+-rw-r--r--   0        0        0      283 2024-06-01 01:24:51.325226 carbon_python_sdk-0.2.2/carbon/paths/health/__init__.py
+-rw-r--r--   0        0        0    10429 2024-06-01 01:24:51.325349 carbon_python_sdk-0.2.2/carbon/paths/health/get.py
+-rw-r--r--   0        0        0    10348 2024-06-01 01:24:51.325468 carbon_python_sdk-0.2.2/carbon/paths/health/get.pyi
+-rw-r--r--   0        0        0      327 2024-06-01 01:24:51.325561 carbon_python_sdk-0.2.2/carbon/paths/integrations_confluence_list/__init__.py
+-rw-r--r--   0        0        0    15289 2024-06-01 01:24:51.325695 carbon_python_sdk-0.2.2/carbon/paths/integrations_confluence_list/post.py
+-rw-r--r--   0        0        0    15115 2024-06-01 01:24:51.325831 carbon_python_sdk-0.2.2/carbon/paths/integrations_confluence_list/post.pyi
+-rw-r--r--   0        0        0      327 2024-06-01 01:24:51.325918 carbon_python_sdk-0.2.2/carbon/paths/integrations_confluence_sync/__init__.py
+-rw-r--r--   0        0        0    29028 2024-06-01 01:24:51.326129 carbon_python_sdk-0.2.2/carbon/paths/integrations_confluence_sync/post.py
+-rw-r--r--   0        0        0    28854 2024-06-01 01:24:51.326337 carbon_python_sdk-0.2.2/carbon/paths/integrations_confluence_sync/post.pyi
+-rw-r--r--   0        0        0      311 2024-06-01 01:24:51.326427 carbon_python_sdk-0.2.2/carbon/paths/integrations_connect/__init__.py
+-rw-r--r--   0        0        0    20686 2024-06-01 01:24:51.326600 carbon_python_sdk-0.2.2/carbon/paths/integrations_connect/post.py
+-rw-r--r--   0        0        0    20512 2024-06-01 01:24:51.326775 carbon_python_sdk-0.2.2/carbon/paths/integrations_connect/post.pyi
+-rw-r--r--   0        0        0      317 2024-06-01 01:24:51.326871 carbon_python_sdk-0.2.2/carbon/paths/integrations_files_sync/__init__.py
+-rw-r--r--   0        0        0    28913 2024-06-01 01:24:51.327238 carbon_python_sdk-0.2.2/carbon/paths/integrations_files_sync/post.py
+-rw-r--r--   0        0        0    28739 2024-06-01 01:24:51.327473 carbon_python_sdk-0.2.2/carbon/paths/integrations_files_sync/post.pyi
+-rw-r--r--   0        0        0      315 2024-06-01 01:24:51.327574 carbon_python_sdk-0.2.2/carbon/paths/integrations_freshdesk/__init__.py
+-rw-r--r--   0        0        0    26091 2024-06-01 01:24:51.327777 carbon_python_sdk-0.2.2/carbon/paths/integrations_freshdesk/post.py
+-rw-r--r--   0        0        0    25917 2024-06-01 01:24:51.327978 carbon_python_sdk-0.2.2/carbon/paths/integrations_freshdesk/post.pyi
+-rw-r--r--   0        0        0      311 2024-06-01 01:24:51.328077 carbon_python_sdk-0.2.2/carbon/paths/integrations_gitbook/__init__.py
+-rw-r--r--   0        0        0    24946 2024-06-01 01:24:51.328268 carbon_python_sdk-0.2.2/carbon/paths/integrations_gitbook/post.py
+-rw-r--r--   0        0        0    24772 2024-06-01 01:24:51.328473 carbon_python_sdk-0.2.2/carbon/paths/integrations_gitbook/post.pyi
+-rw-r--r--   0        0        0      325 2024-06-01 01:24:51.328572 carbon_python_sdk-0.2.2/carbon/paths/integrations_gitbook_spaces/__init__.py
+-rw-r--r--   0        0        0    14816 2024-06-01 01:24:51.328726 carbon_python_sdk-0.2.2/carbon/paths/integrations_gitbook_spaces/get.py
+-rw-r--r--   0        0        0    14642 2024-06-01 01:24:51.328878 carbon_python_sdk-0.2.2/carbon/paths/integrations_gitbook_spaces/get.pyi
+-rw-r--r--   0        0        0      321 2024-06-01 01:24:51.328972 carbon_python_sdk-0.2.2/carbon/paths/integrations_gitbook_sync/__init__.py
+-rw-r--r--   0        0        0    23173 2024-06-01 01:24:51.329154 carbon_python_sdk-0.2.2/carbon/paths/integrations_gitbook_sync/post.py
+-rw-r--r--   0        0        0    22999 2024-06-01 01:24:51.329337 carbon_python_sdk-0.2.2/carbon/paths/integrations_gitbook_sync/post.pyi
+-rw-r--r--   0        0        0      309 2024-06-01 01:24:51.329860 carbon_python_sdk-0.2.2/carbon/paths/integrations_github/__init__.py
+-rw-r--r--   0        0        0    15826 2024-06-01 01:24:51.329998 carbon_python_sdk-0.2.2/carbon/paths/integrations_github/post.py
+-rw-r--r--   0        0        0    15652 2024-06-01 01:24:51.330140 carbon_python_sdk-0.2.2/carbon/paths/integrations_github/post.pyi
+-rw-r--r--   0        0        0      321 2024-06-01 01:24:51.330233 carbon_python_sdk-0.2.2/carbon/paths/integrations_github_repos/__init__.py
+-rw-r--r--   0        0        0    17078 2024-06-01 01:24:51.330388 carbon_python_sdk-0.2.2/carbon/paths/integrations_github_repos/get.py
+-rw-r--r--   0        0        0    16904 2024-06-01 01:24:51.330568 carbon_python_sdk-0.2.2/carbon/paths/integrations_github_repos/get.pyi
+-rw-r--r--   0        0        0      331 2024-06-01 01:24:51.330667 carbon_python_sdk-0.2.2/carbon/paths/integrations_github_sync_repos/__init__.py
+-rw-r--r--   0        0        0    15560 2024-06-01 01:24:51.330820 carbon_python_sdk-0.2.2/carbon/paths/integrations_github_sync_repos/post.py
+-rw-r--r--   0        0        0    15386 2024-06-01 01:24:51.330965 carbon_python_sdk-0.2.2/carbon/paths/integrations_github_sync_repos/post.pyi
+-rw-r--r--   0        0        0      317 2024-06-01 01:24:51.331053 carbon_python_sdk-0.2.2/carbon/paths/integrations_gmail_sync/__init__.py
+-rw-r--r--   0        0        0    26562 2024-06-01 01:24:51.331245 carbon_python_sdk-0.2.2/carbon/paths/integrations_gmail_sync/post.py
+-rw-r--r--   0        0        0    26388 2024-06-01 01:24:51.331449 carbon_python_sdk-0.2.2/carbon/paths/integrations_gmail_sync/post.pyi
+-rw-r--r--   0        0        0      331 2024-06-01 01:24:51.331548 carbon_python_sdk-0.2.2/carbon/paths/integrations_gmail_user_labels/__init__.py
+-rw-r--r--   0        0        0    15340 2024-06-01 01:24:51.331695 carbon_python_sdk-0.2.2/carbon/paths/integrations_gmail_user_labels/get.py
+-rw-r--r--   0        0        0    15166 2024-06-01 01:24:51.331836 carbon_python_sdk-0.2.2/carbon/paths/integrations_gmail_user_labels/get.pyi
+-rw-r--r--   0        0        0      317 2024-06-01 01:24:51.331923 carbon_python_sdk-0.2.2/carbon/paths/integrations_items_list/__init__.py
+-rw-r--r--   0        0        0    19585 2024-06-01 01:24:51.332080 carbon_python_sdk-0.2.2/carbon/paths/integrations_items_list/post.py
+-rw-r--r--   0        0        0    19411 2024-06-01 01:24:51.332236 carbon_python_sdk-0.2.2/carbon/paths/integrations_items_list/post.pyi
+-rw-r--r--   0        0        0      317 2024-06-01 01:24:51.332326 carbon_python_sdk-0.2.2/carbon/paths/integrations_items_sync/__init__.py
+-rw-r--r--   0        0        0    14992 2024-06-01 01:24:51.332924 carbon_python_sdk-0.2.2/carbon/paths/integrations_items_sync/post.py
+-rw-r--r--   0        0        0    14818 2024-06-01 01:24:51.333071 carbon_python_sdk-0.2.2/carbon/paths/integrations_items_sync/post.pyi
+-rw-r--r--   0        0        0      331 2024-06-01 01:36:07.373983 carbon_python_sdk-0.2.2/carbon/paths/integrations_items_sync_cancel/__init__.py
+-rw-r--r--   0        0        0    14722 2024-06-01 01:36:07.374762 carbon_python_sdk-0.2.2/carbon/paths/integrations_items_sync_cancel/post.py
+-rw-r--r--   0        0        0    14548 2024-06-01 01:36:07.375397 carbon_python_sdk-0.2.2/carbon/paths/integrations_items_sync_cancel/post.pyi
+-rw-r--r--   0        0        0      315 2024-06-01 01:24:51.333544 carbon_python_sdk-0.2.2/carbon/paths/integrations_oauth_url/__init__.py
+-rw-r--r--   0        0        0    37674 2024-06-01 01:24:51.333800 carbon_python_sdk-0.2.2/carbon/paths/integrations_oauth_url/post.py
+-rw-r--r--   0        0        0    37500 2024-06-01 01:24:51.334065 carbon_python_sdk-0.2.2/carbon/paths/integrations_oauth_url/post.pyi
+-rw-r--r--   0        0        0      321 2024-06-01 01:24:51.334155 carbon_python_sdk-0.2.2/carbon/paths/integrations_outlook_sync/__init__.py
+-rw-r--r--   0        0        0    27296 2024-06-01 01:24:51.334360 carbon_python_sdk-0.2.2/carbon/paths/integrations_outlook_sync/post.py
+-rw-r--r--   0        0        0    27122 2024-06-01 01:24:51.334563 carbon_python_sdk-0.2.2/carbon/paths/integrations_outlook_sync/post.pyi
+-rw-r--r--   0        0        0      343 2024-06-01 01:24:51.334666 carbon_python_sdk-0.2.2/carbon/paths/integrations_outlook_user_categories/__init__.py
+-rw-r--r--   0        0        0    15590 2024-06-01 01:24:51.334807 carbon_python_sdk-0.2.2/carbon/paths/integrations_outlook_user_categories/get.py
+-rw-r--r--   0        0        0    15416 2024-06-01 01:24:51.334964 carbon_python_sdk-0.2.2/carbon/paths/integrations_outlook_user_categories/get.pyi
+-rw-r--r--   0        0        0      337 2024-06-01 01:24:51.335060 carbon_python_sdk-0.2.2/carbon/paths/integrations_outlook_user_folders/__init__.py
+-rw-r--r--   0        0        0    15371 2024-06-01 01:24:51.335207 carbon_python_sdk-0.2.2/carbon/paths/integrations_outlook_user_folders/get.py
+-rw-r--r--   0        0        0    15197 2024-06-01 01:24:51.335351 carbon_python_sdk-0.2.2/carbon/paths/integrations_outlook_user_folders/get.pyi
+-rw-r--r--   0        0        0      313 2024-06-01 01:24:51.335436 carbon_python_sdk-0.2.2/carbon/paths/integrations_rss_feed/__init__.py
+-rw-r--r--   0        0        0    22218 2024-06-01 01:24:51.335612 carbon_python_sdk-0.2.2/carbon/paths/integrations_rss_feed/post.py
+-rw-r--r--   0        0        0    22044 2024-06-01 01:24:51.335801 carbon_python_sdk-0.2.2/carbon/paths/integrations_rss_feed/post.pyi
+-rw-r--r--   0        0        0      301 2024-06-01 01:24:51.335903 carbon_python_sdk-0.2.2/carbon/paths/integrations_s3/__init__.py
+-rw-r--r--   0        0        0    16130 2024-06-01 01:24:51.336047 carbon_python_sdk-0.2.2/carbon/paths/integrations_s3/post.py
+-rw-r--r--   0        0        0    15956 2024-06-01 01:24:51.336190 carbon_python_sdk-0.2.2/carbon/paths/integrations_s3/post.pyi
+-rw-r--r--   0        0        0      313 2024-06-01 01:24:51.336278 carbon_python_sdk-0.2.2/carbon/paths/integrations_s3_files/__init__.py
+-rw-r--r--   0        0        0    28274 2024-06-01 01:24:51.336475 carbon_python_sdk-0.2.2/carbon/paths/integrations_s3_files/post.py
+-rw-r--r--   0        0        0    28100 2024-06-01 01:24:51.336689 carbon_python_sdk-0.2.2/carbon/paths/integrations_s3_files/post.pyi
+-rw-r--r--   0        0        0      321 2024-06-01 01:24:51.336787 carbon_python_sdk-0.2.2/carbon/paths/modify_user_configuration/__init__.py
+-rw-r--r--   0        0        0    16382 2024-06-01 01:24:51.336930 carbon_python_sdk-0.2.2/carbon/paths/modify_user_configuration/post.py
+-rw-r--r--   0        0        0    16208 2024-06-01 01:24:51.337073 carbon_python_sdk-0.2.2/carbon/paths/modify_user_configuration/post.pyi
+-rw-r--r--   0        0        0      295 2024-06-01 01:24:51.337163 carbon_python_sdk-0.2.2/carbon/paths/organization/__init__.py
+-rw-r--r--   0        0        0    10831 2024-06-01 01:24:51.337286 carbon_python_sdk-0.2.2/carbon/paths/organization/get.py
+-rw-r--r--   0        0        0    10724 2024-06-01 01:24:51.337416 carbon_python_sdk-0.2.2/carbon/paths/organization/get.pyi
+-rw-r--r--   0        0        0      317 2024-06-01 01:24:51.337820 carbon_python_sdk-0.2.2/carbon/paths/organization_statistics/__init__.py
+-rw-r--r--   0        0        0    11092 2024-06-01 01:24:51.337970 carbon_python_sdk-0.2.2/carbon/paths/organization_statistics/post.py
+-rw-r--r--   0        0        0    10985 2024-06-01 01:24:51.338109 carbon_python_sdk-0.2.2/carbon/paths/organization_statistics/post.pyi
+-rw-r--r--   0        0        0      309 2024-06-01 01:24:51.338339 carbon_python_sdk-0.2.2/carbon/paths/organization_update/__init__.py
+-rw-r--r--   0        0        0    15275 2024-06-01 01:24:51.338489 carbon_python_sdk-0.2.2/carbon/paths/organization_update/post.py
+-rw-r--r--   0        0        0    15138 2024-06-01 01:24:51.338639 carbon_python_sdk-0.2.2/carbon/paths/organization_update/post.pyi
+-rw-r--r--   0        0        0      309 2024-06-01 01:24:51.338730 carbon_python_sdk-0.2.2/carbon/paths/parsed_file_file_id/__init__.py
+-rw-r--r--   0        0        0    14654 2024-06-01 01:24:51.338885 carbon_python_sdk-0.2.2/carbon/paths/parsed_file_file_id/get.py
+-rw-r--r--   0        0        0    14480 2024-06-01 01:24:51.339029 carbon_python_sdk-0.2.2/carbon/paths/parsed_file_file_id/get.pyi
+-rw-r--r--   0        0        0      301 2024-06-01 01:24:51.339122 carbon_python_sdk-0.2.2/carbon/paths/process_sitemap/__init__.py
+-rw-r--r--   0        0        0    14363 2024-06-01 01:24:51.339266 carbon_python_sdk-0.2.2/carbon/paths/process_sitemap/get.py
+-rw-r--r--   0        0        0    14189 2024-06-01 01:24:51.339416 carbon_python_sdk-0.2.2/carbon/paths/process_sitemap/get.pyi
+-rw-r--r--   0        0        0      303 2024-06-01 01:24:51.339504 carbon_python_sdk-0.2.2/carbon/paths/raw_file_file_id/__init__.py
+-rw-r--r--   0        0        0    14585 2024-06-01 01:24:51.339790 carbon_python_sdk-0.2.2/carbon/paths/raw_file_file_id/get.py
+-rw-r--r--   0        0        0    14411 2024-06-01 01:24:51.340008 carbon_python_sdk-0.2.2/carbon/paths/raw_file_file_id/get.pyi
+-rw-r--r--   0        0        0      293 2024-06-01 01:24:51.340108 carbon_python_sdk-0.2.2/carbon/paths/resync_file/__init__.py
+-rw-r--r--   0        0        0    16696 2024-06-01 01:24:51.340285 carbon_python_sdk-0.2.2/carbon/paths/resync_file/post.py
+-rw-r--r--   0        0        0    16522 2024-06-01 01:24:51.340451 carbon_python_sdk-0.2.2/carbon/paths/resync_file/post.pyi
+-rw-r--r--   0        0        0      309 2024-06-01 01:24:51.340572 carbon_python_sdk-0.2.2/carbon/paths/revoke_access_token/__init__.py
+-rw-r--r--   0        0        0    14828 2024-06-01 01:24:51.340722 carbon_python_sdk-0.2.2/carbon/paths/revoke_access_token/post.py
+-rw-r--r--   0        0        0    14654 2024-06-01 01:24:51.340883 carbon_python_sdk-0.2.2/carbon/paths/revoke_access_token/post.pyi
+-rw-r--r--   0        0        0      299 2024-06-01 01:24:51.340993 carbon_python_sdk-0.2.2/carbon/paths/scrape_sitemap/__init__.py
+-rw-r--r--   0        0        0    27300 2024-06-01 01:24:51.341210 carbon_python_sdk-0.2.2/carbon/paths/scrape_sitemap/post.py
+-rw-r--r--   0        0        0    27126 2024-06-01 01:24:51.341412 carbon_python_sdk-0.2.2/carbon/paths/scrape_sitemap/post.pyi
+-rw-r--r--   0        0        0      293 2024-06-01 01:24:51.341508 carbon_python_sdk-0.2.2/carbon/paths/search_urls/__init__.py
+-rw-r--r--   0        0        0    14549 2024-06-01 01:24:51.341670 carbon_python_sdk-0.2.2/carbon/paths/search_urls/get.py
+-rw-r--r--   0        0        0    14375 2024-06-01 01:24:51.341833 carbon_python_sdk-0.2.2/carbon/paths/search_urls/get.pyi
+-rw-r--r--   0        0        0      293 2024-06-01 01:24:51.341920 carbon_python_sdk-0.2.2/carbon/paths/text_chunks/__init__.py
+-rw-r--r--   0        0        0    19073 2024-06-01 01:24:51.342074 carbon_python_sdk-0.2.2/carbon/paths/text_chunks/post.py
+-rw-r--r--   0        0        0    18899 2024-06-01 01:24:51.342245 carbon_python_sdk-0.2.2/carbon/paths/text_chunks/post.pyi
+-rw-r--r--   0        0        0      295 2024-06-01 01:24:51.342355 carbon_python_sdk-0.2.2/carbon/paths/update_users/__init__.py
+-rw-r--r--   0        0        0    18200 2024-06-01 01:24:51.342517 carbon_python_sdk-0.2.2/carbon/paths/update_users/post.py
+-rw-r--r--   0        0        0    18063 2024-06-01 01:24:51.342696 carbon_python_sdk-0.2.2/carbon/paths/update_users/post.pyi
+-rw-r--r--   0        0        0      327 2024-06-01 01:24:51.342791 carbon_python_sdk-0.2.2/carbon/paths/upload_chunks_and_embeddings/__init__.py
+-rw-r--r--   0        0        0    20060 2024-06-01 01:24:51.342962 carbon_python_sdk-0.2.2/carbon/paths/upload_chunks_and_embeddings/post.py
+-rw-r--r--   0        0        0    19886 2024-06-01 01:24:51.343141 carbon_python_sdk-0.2.2/carbon/paths/upload_chunks_and_embeddings/post.pyi
+-rw-r--r--   0        0        0      311 2024-06-01 01:24:51.343247 carbon_python_sdk-0.2.2/carbon/paths/upload_file_from_url/__init__.py
+-rw-r--r--   0        0        0    26028 2024-06-01 01:36:07.375893 carbon_python_sdk-0.2.2/carbon/paths/upload_file_from_url/post.py
+-rw-r--r--   0        0        0    25854 2024-06-01 01:36:07.376175 carbon_python_sdk-0.2.2/carbon/paths/upload_file_from_url/post.pyi
+-rw-r--r--   0        0        0      293 2024-06-01 01:24:51.343770 carbon_python_sdk-0.2.2/carbon/paths/upload_text/__init__.py
+-rw-r--r--   0        0        0    20504 2024-06-01 01:24:51.343954 carbon_python_sdk-0.2.2/carbon/paths/upload_text/post.py
+-rw-r--r--   0        0        0    20330 2024-06-01 01:24:51.344134 carbon_python_sdk-0.2.2/carbon/paths/upload_text/post.pyi
+-rw-r--r--   0        0        0      291 2024-06-01 01:24:51.344237 carbon_python_sdk-0.2.2/carbon/paths/uploadfile/__init__.py
+-rw-r--r--   0        0        0    35190 2024-06-01 01:24:51.344477 carbon_python_sdk-0.2.2/carbon/paths/uploadfile/post.py
+-rw-r--r--   0        0        0    35016 2024-06-01 01:24:51.344895 carbon_python_sdk-0.2.2/carbon/paths/uploadfile/post.pyi
+-rw-r--r--   0        0        0      279 2024-06-01 01:24:51.345031 carbon_python_sdk-0.2.2/carbon/paths/user/__init__.py
+-rw-r--r--   0        0        0    14156 2024-06-01 01:24:51.345210 carbon_python_sdk-0.2.2/carbon/paths/user/post.py
+-rw-r--r--   0        0        0    14019 2024-06-01 01:24:51.345375 carbon_python_sdk-0.2.2/carbon/paths/user/post.pyi
+-rw-r--r--   0        0        0      305 2024-06-01 01:24:51.345466 carbon_python_sdk-0.2.2/carbon/paths/user_data_sources/__init__.py
+-rw-r--r--   0        0        0    18865 2024-06-01 01:24:51.345625 carbon_python_sdk-0.2.2/carbon/paths/user_data_sources/post.py
+-rw-r--r--   0        0        0    18691 2024-06-01 01:24:51.345798 carbon_python_sdk-0.2.2/carbon/paths/user_data_sources/post.pyi
+-rw-r--r--   0        0        0      291 2024-06-01 01:24:51.345895 carbon_python_sdk-0.2.2/carbon/paths/user_files/__init__.py
+-rw-r--r--   0        0        0    22374 2024-06-01 01:24:51.346083 carbon_python_sdk-0.2.2/carbon/paths/user_files/post.py
+-rw-r--r--   0        0        0    22200 2024-06-01 01:24:51.346273 carbon_python_sdk-0.2.2/carbon/paths/user_files/post.pyi
+-rw-r--r--   0        0        0      297 2024-06-01 01:24:51.346364 carbon_python_sdk-0.2.2/carbon/paths/user_files_v2/__init__.py
+-rw-r--r--   0        0        0    21370 2024-06-01 01:24:51.346547 carbon_python_sdk-0.2.2/carbon/paths/user_files_v2/post.py
+-rw-r--r--   0        0        0    21196 2024-06-01 01:24:51.346738 carbon_python_sdk-0.2.2/carbon/paths/user_files_v2/post.pyi
+-rw-r--r--   0        0        0      291 2024-06-01 01:24:51.346824 carbon_python_sdk-0.2.2/carbon/paths/web_scrape/__init__.py
+-rw-r--r--   0        0        0    14274 2024-06-01 01:24:51.346967 carbon_python_sdk-0.2.2/carbon/paths/web_scrape/post.py
+-rw-r--r--   0        0        0    14100 2024-06-01 01:24:51.347114 carbon_python_sdk-0.2.2/carbon/paths/web_scrape/post.pyi
+-rw-r--r--   0        0        0      287 2024-06-01 01:24:51.347204 carbon_python_sdk-0.2.2/carbon/paths/webhooks/__init__.py
+-rw-r--r--   0        0        0    17367 2024-06-01 01:24:51.347535 carbon_python_sdk-0.2.2/carbon/paths/webhooks/post.py
+-rw-r--r--   0        0        0    17230 2024-06-01 01:24:51.347756 carbon_python_sdk-0.2.2/carbon/paths/webhooks/post.pyi
+-rw-r--r--   0        0        0        0 2024-06-01 01:24:51.347906 carbon_python_sdk-0.2.2/carbon/pydantic/__init__.py
+-rw-r--r--   0        0        0      559 2024-06-01 01:24:51.347997 carbon_python_sdk-0.2.2/carbon/pydantic/add_webhook_props.py
+-rw-r--r--   0        0        0      586 2024-06-01 01:24:51.348093 carbon_python_sdk-0.2.2/carbon/pydantic/body_create_upload_file_uploadfile_post.py
+-rw-r--r--   0        0        0      760 2024-06-01 01:24:51.348179 carbon_python_sdk-0.2.2/carbon/pydantic/chunk_properties.py
+-rw-r--r--   0        0        0      768 2024-06-01 01:24:51.348280 carbon_python_sdk-0.2.2/carbon/pydantic/chunk_properties_nullable.py
+-rw-r--r--   0        0        0      821 2024-06-01 01:24:51.348362 carbon_python_sdk-0.2.2/carbon/pydantic/chunks_and_embeddings.py
+-rw-r--r--   0        0        0      469 2024-06-01 01:24:51.348448 carbon_python_sdk-0.2.2/carbon/pydantic/chunks_and_embeddings_embedding.py
+-rw-r--r--   0        0        0     1333 2024-06-01 01:24:51.348544 carbon_python_sdk-0.2.2/carbon/pydantic/chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0      438 2024-06-01 01:24:51.348635 carbon_python_sdk-0.2.2/carbon/pydantic/chunks_and_embeddings_upload_input_custom_credentials.py
+-rw-r--r--   0        0        0      418 2024-06-01 01:24:51.348729 carbon_python_sdk-0.2.2/carbon/pydantic/configuration_keys.py
+-rw-r--r--   0        0        0      835 2024-06-01 01:24:51.348821 carbon_python_sdk-0.2.2/carbon/pydantic/confluence_authentication.py
+-rw-r--r--   0        0        0     1791 2024-06-01 01:24:51.348916 carbon_python_sdk-0.2.2/carbon/pydantic/connect_data_source_input.py
+-rw-r--r--   0        0        0      765 2024-06-01 01:24:51.348998 carbon_python_sdk-0.2.2/carbon/pydantic/connect_data_source_response.py
+-rw-r--r--   0        0        0      481 2024-06-01 01:24:51.349085 carbon_python_sdk-0.2.2/carbon/pydantic/custom_credentials_type.py
+-rw-r--r--   0        0        0      424 2024-06-01 01:24:51.349168 carbon_python_sdk-0.2.2/carbon/pydantic/data_source_extended_input.py
+-rw-r--r--   0        0        0      456 2024-06-01 01:24:51.349251 carbon_python_sdk-0.2.2/carbon/pydantic/data_source_last_sync_actions.py
+-rw-r--r--   0        0        0      472 2024-06-01 01:24:51.349332 carbon_python_sdk-0.2.2/carbon/pydantic/data_source_sync_statuses.py
+-rw-r--r--   0        0        0      890 2024-06-01 01:24:51.349418 carbon_python_sdk-0.2.2/carbon/pydantic/data_source_type.py
+-rw-r--r--   0        0        0      898 2024-06-01 01:24:51.349506 carbon_python_sdk-0.2.2/carbon/pydantic/data_source_type_nullable.py
+-rw-r--r--   0        0        0     1187 2024-06-01 01:24:51.349587 carbon_python_sdk-0.2.2/carbon/pydantic/delete_files_query_input.py
+-rw-r--r--   0        0        0      448 2024-06-01 01:24:51.349684 carbon_python_sdk-0.2.2/carbon/pydantic/delete_files_query_input_file_ids.py
+-rw-r--r--   0        0        0      809 2024-06-01 01:24:51.349767 carbon_python_sdk-0.2.2/carbon/pydantic/delete_files_v2_query_input.py
+-rw-r--r--   0        0        0      690 2024-06-01 01:24:51.349854 carbon_python_sdk-0.2.2/carbon/pydantic/delete_users_input.py
+-rw-r--r--   0        0        0      430 2024-06-01 01:24:51.349938 carbon_python_sdk-0.2.2/carbon/pydantic/delete_users_input_customer_ids.py
+-rw-r--r--   0        0        0      694 2024-06-01 01:24:51.350016 carbon_python_sdk-0.2.2/carbon/pydantic/directory_item.py
+-rw-r--r--   0        0        0     1674 2024-06-01 01:24:51.350096 carbon_python_sdk-0.2.2/carbon/pydantic/document_response.py
+-rw-r--r--   0        0        0      665 2024-06-01 01:24:51.350178 carbon_python_sdk-0.2.2/carbon/pydantic/document_response_list.py
+-rw-r--r--   0        0        0      411 2024-06-01 01:24:51.350257 carbon_python_sdk-0.2.2/carbon/pydantic/document_response_tags.py
+-rw-r--r--   0        0        0      463 2024-06-01 01:24:51.350339 carbon_python_sdk-0.2.2/carbon/pydantic/document_response_vector.py
+-rw-r--r--   0        0        0     1021 2024-06-01 01:24:51.350430 carbon_python_sdk-0.2.2/carbon/pydantic/embedding_and_chunk.py
+-rw-r--r--   0        0        0      467 2024-06-01 01:24:51.350572 carbon_python_sdk-0.2.2/carbon/pydantic/embedding_and_chunk_embedding.py
+-rw-r--r--   0        0        0      743 2024-06-01 01:24:51.350675 carbon_python_sdk-0.2.2/carbon/pydantic/embedding_generators.py
+-rw-r--r--   0        0        0      751 2024-06-01 01:24:51.350773 carbon_python_sdk-0.2.2/carbon/pydantic/embedding_generators_nullable.py
+-rw-r--r--   0        0        0      666 2024-06-01 01:24:51.350870 carbon_python_sdk-0.2.2/carbon/pydantic/embedding_properties.py
+-rw-r--r--   0        0        0      780 2024-06-01 01:24:51.350964 carbon_python_sdk-0.2.2/carbon/pydantic/embeddings_and_chunks_filters.py
+-rw-r--r--   0        0        0      470 2024-06-01 01:24:51.351067 carbon_python_sdk-0.2.2/carbon/pydantic/embeddings_and_chunks_order_by_columns.py
+-rw-r--r--   0        0        0     1222 2024-06-01 01:24:51.351163 carbon_python_sdk-0.2.2/carbon/pydantic/embeddings_and_chunks_query_input.py
+-rw-r--r--   0        0        0      711 2024-06-01 01:24:51.351258 carbon_python_sdk-0.2.2/carbon/pydantic/embeddings_and_chunks_response.py
+-rw-r--r--   0        0        0      553 2024-06-01 01:24:51.351352 carbon_python_sdk-0.2.2/carbon/pydantic/external_file_sync_statuses.py
+-rw-r--r--   0        0        0     1780 2024-06-01 01:24:51.351447 carbon_python_sdk-0.2.2/carbon/pydantic/external_source_item.py
+-rw-r--r--   0        0        0      455 2024-06-01 01:24:51.351541 carbon_python_sdk-0.2.2/carbon/pydantic/external_source_items_order_by.py
+-rw-r--r--   0        0        0      781 2024-06-01 01:24:51.351636 carbon_python_sdk-0.2.2/carbon/pydantic/fetch_urls_response.py
+-rw-r--r--   0        0        0      424 2024-06-01 01:24:51.351730 carbon_python_sdk-0.2.2/carbon/pydantic/fetch_urls_response_urls.py
+-rw-r--r--   0        0        0      445 2024-06-01 01:24:51.351819 carbon_python_sdk-0.2.2/carbon/pydantic/file_content_types.py
+-rw-r--r--   0        0        0      453 2024-06-01 01:24:51.351914 carbon_python_sdk-0.2.2/carbon/pydantic/file_content_types_nullable.py
+-rw-r--r--   0        0        0      820 2024-06-01 01:24:51.352012 carbon_python_sdk-0.2.2/carbon/pydantic/file_formats.py
+-rw-r--r--   0        0        0      828 2024-06-01 01:24:51.352104 carbon_python_sdk-0.2.2/carbon/pydantic/file_formats_nullable.py
+-rw-r--r--   0        0        0     1002 2024-06-01 01:24:51.352200 carbon_python_sdk-0.2.2/carbon/pydantic/file_statistics.py
+-rw-r--r--   0        0        0     1010 2024-06-01 01:24:51.352297 carbon_python_sdk-0.2.2/carbon/pydantic/file_statistics_nullable.py
+-rw-r--r--   0        0        0     1240 2024-06-01 01:24:51.352393 carbon_python_sdk-0.2.2/carbon/pydantic/file_sync_config.py
+-rw-r--r--   0        0        0     1248 2024-06-01 01:24:51.352491 carbon_python_sdk-0.2.2/carbon/pydantic/file_sync_config_nullable.py
+-rw-r--r--   0        0        0      492 2024-06-01 01:24:51.352586 carbon_python_sdk-0.2.2/carbon/pydantic/files_query_user_files_deprecated_response.py
+-rw-r--r--   0        0        0     2096 2024-06-01 01:24:51.352677 carbon_python_sdk-0.2.2/carbon/pydantic/fresh_desk_connect_request.py
+-rw-r--r--   0        0        0      723 2024-06-01 01:24:51.352769 carbon_python_sdk-0.2.2/carbon/pydantic/freskdesk_authentication.py
+-rw-r--r--   0        0        0      575 2024-06-01 01:24:51.352881 carbon_python_sdk-0.2.2/carbon/pydantic/generic_success_response.py
+-rw-r--r--   0        0        0     3379 2024-06-01 01:24:51.352975 carbon_python_sdk-0.2.2/carbon/pydantic/get_embedding_documents_body.py
+-rw-r--r--   0        0        0      452 2024-06-01 01:24:51.353126 carbon_python_sdk-0.2.2/carbon/pydantic/get_embedding_documents_body_file_ids.py
+-rw-r--r--   0        0        0      458 2024-06-01 01:24:51.353224 carbon_python_sdk-0.2.2/carbon/pydantic/get_embedding_documents_body_parent_file_ids.py
+-rw-r--r--   0        0        0      477 2024-06-01 01:24:51.353319 carbon_python_sdk-0.2.2/carbon/pydantic/get_embedding_documents_body_query_vector.py
+-rw-r--r--   0        0        0      420 2024-06-01 01:24:51.353415 carbon_python_sdk-0.2.2/carbon/pydantic/get_embedding_documents_body_tags.py
+-rw-r--r--   0        0        0      752 2024-06-01 01:24:51.353510 carbon_python_sdk-0.2.2/carbon/pydantic/gitbook_authetication.py
+-rw-r--r--   0        0        0     1911 2024-06-01 01:24:51.353601 carbon_python_sdk-0.2.2/carbon/pydantic/gitbook_connect_request.py
+-rw-r--r--   0        0        0     1699 2024-06-01 01:24:51.353695 carbon_python_sdk-0.2.2/carbon/pydantic/gitbook_sync_request.py
+-rw-r--r--   0        0        0      429 2024-06-01 01:24:51.353789 carbon_python_sdk-0.2.2/carbon/pydantic/gitbook_sync_request_space_ids.py
+-rw-r--r--   0        0        0      734 2024-06-01 01:24:51.353870 carbon_python_sdk-0.2.2/carbon/pydantic/github_authentication.py
+-rw-r--r--   0        0        0      825 2024-06-01 01:24:51.353950 carbon_python_sdk-0.2.2/carbon/pydantic/github_connect_request.py
+-rw-r--r--   0        0        0      783 2024-06-01 01:24:51.354029 carbon_python_sdk-0.2.2/carbon/pydantic/github_fetch_repos_request.py
+-rw-r--r--   0        0        0      431 2024-06-01 01:24:51.354114 carbon_python_sdk-0.2.2/carbon/pydantic/github_fetch_repos_request_repos.py
+-rw-r--r--   0        0        0     2073 2024-06-01 01:24:51.354194 carbon_python_sdk-0.2.2/carbon/pydantic/gmail_sync_input.py
+-rw-r--r--   0        0        0      432 2024-06-01 01:24:51.354271 carbon_python_sdk-0.2.2/carbon/pydantic/helpdesk_file_types.py
+-rw-r--r--   0        0        0      678 2024-06-01 01:24:51.354351 carbon_python_sdk-0.2.2/carbon/pydantic/http_validation_error.py
+-rw-r--r--   0        0        0      665 2024-06-01 01:24:51.354436 carbon_python_sdk-0.2.2/carbon/pydantic/hybrid_search_tuning_params.py
+-rw-r--r--   0        0        0      673 2024-06-01 01:24:51.354520 carbon_python_sdk-0.2.2/carbon/pydantic/hybrid_search_tuning_params_nullable.py
+-rw-r--r--   0        0        0     1282 2024-06-01 01:24:51.354603 carbon_python_sdk-0.2.2/carbon/pydantic/list_data_source_items_request.py
+-rw-r--r--   0        0        0      710 2024-06-01 01:24:51.354684 carbon_python_sdk-0.2.2/carbon/pydantic/list_data_source_items_response.py
+-rw-r--r--   0        0        0     1035 2024-06-01 01:24:51.354762 carbon_python_sdk-0.2.2/carbon/pydantic/list_items_filters.py
+-rw-r--r--   0        0        0      447 2024-06-01 01:24:51.354848 carbon_python_sdk-0.2.2/carbon/pydantic/list_items_filters_external_ids.py
+-rw-r--r--   0        0        0      439 2024-06-01 01:24:51.354933 carbon_python_sdk-0.2.2/carbon/pydantic/list_items_filters_ids.py
+-rw-r--r--   0        0        0     1093 2024-06-01 01:24:51.355019 carbon_python_sdk-0.2.2/carbon/pydantic/list_items_filters_nullable.py
+-rw-r--r--   0        0        0      455 2024-06-01 01:24:51.355103 carbon_python_sdk-0.2.2/carbon/pydantic/list_items_filters_nullable_external_ids.py
+-rw-r--r--   0        0        0      447 2024-06-01 01:24:51.355182 carbon_python_sdk-0.2.2/carbon/pydantic/list_items_filters_nullable_ids.py
+-rw-r--r--   0        0        0      664 2024-06-01 01:24:51.355264 carbon_python_sdk-0.2.2/carbon/pydantic/list_request.py
+-rw-r--r--   0        0        0      638 2024-06-01 01:24:51.355345 carbon_python_sdk-0.2.2/carbon/pydantic/list_response.py
+-rw-r--r--   0        0        0      733 2024-06-01 01:24:51.355427 carbon_python_sdk-0.2.2/carbon/pydantic/modify_user_configuration_input.py
+-rw-r--r--   0        0        0      430 2024-06-01 01:24:51.355504 carbon_python_sdk-0.2.2/carbon/pydantic/multi_modal_embedding_generators.py
+-rw-r--r--   0        0        0      742 2024-06-01 01:24:51.355586 carbon_python_sdk-0.2.2/carbon/pydantic/notion_authentication.py
+-rw-r--r--   0        0        0      814 2024-06-01 01:24:51.355666 carbon_python_sdk-0.2.2/carbon/pydantic/o_auth_authentication.py
+-rw-r--r--   0        0        0     4718 2024-06-01 01:36:07.376567 carbon_python_sdk-0.2.2/carbon/pydantic/o_auth_url_request.py
+-rw-r--r--   0        0        0      417 2024-06-01 01:24:51.355856 carbon_python_sdk-0.2.2/carbon/pydantic/order_dir.py
+-rw-r--r--   0        0        0      419 2024-06-01 01:24:51.355935 carbon_python_sdk-0.2.2/carbon/pydantic/order_dir_v2.py
+-rw-r--r--   0        0        0     2547 2024-06-01 01:24:51.356014 carbon_python_sdk-0.2.2/carbon/pydantic/organization_response.py
+-rw-r--r--   0        0        0     2100 2024-06-01 01:24:51.356100 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_data_source_api.py
+-rw-r--r--   0        0        0      998 2024-06-01 01:24:51.356186 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_data_source_filters.py
+-rw-r--r--   0        0        0      456 2024-06-01 01:24:51.356270 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_data_source_filters_ids.py
+-rw-r--r--   0        0        0      462 2024-06-01 01:24:51.356352 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_data_source_order_by_columns.py
+-rw-r--r--   0        0        0     1213 2024-06-01 01:24:51.356431 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_data_source_query_input.py
+-rw-r--r--   0        0        0      756 2024-06-01 01:24:51.356516 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_data_source_response.py
+-rw-r--r--   0        0        0      785 2024-06-01 01:24:51.356599 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_file_tag_create.py
+-rw-r--r--   0        0        0      424 2024-06-01 01:24:51.356679 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_file_tag_create_tags.py
+-rw-r--r--   0        0        0      789 2024-06-01 01:24:51.356760 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_file_tags_remove.py
+-rw-r--r--   0        0        0      437 2024-06-01 01:24:51.356842 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_file_tags_remove_tags.py
+-rw-r--r--   0        0        0     5786 2024-06-01 01:24:51.356958 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_files_to_sync_filters.py
+-rw-r--r--   0        0        0      469 2024-06-01 01:24:51.357043 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_files_to_sync_filters_external_file_ids.py
+-rw-r--r--   0        0        0      457 2024-06-01 01:24:51.357122 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_files_to_sync_filters_ids.py
+-rw-r--r--   0        0        0      482 2024-06-01 01:24:51.357207 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_files_to_sync_filters_organization_user_data_source_id.py
+-rw-r--r--   0        0        0      467 2024-06-01 01:24:51.357299 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_files_to_sync_filters_parent_file_ids.py
+-rw-r--r--   0        0        0      464 2024-06-01 01:24:51.357383 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_files_to_sync_filters_request_ids.py
+-rw-r--r--   0        0        0      429 2024-06-01 01:24:51.357467 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_files_to_sync_filters_tags.py
+-rw-r--r--   0        0        0      501 2024-06-01 01:24:51.357550 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_files_to_sync_order_by_types.py
+-rw-r--r--   0        0        0     1554 2024-06-01 01:24:51.357633 carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_files_to_sync_query_input.py
+-rw-r--r--   0        0        0      571 2024-06-01 01:24:51.357728 carbon_python_sdk-0.2.2/carbon/pydantic/outh_url_response.py
+-rw-r--r--   0        0        0     2156 2024-06-01 01:24:51.357808 carbon_python_sdk-0.2.2/carbon/pydantic/outlook_sync_input.py
+-rw-r--r--   0        0        0      645 2024-06-01 01:24:51.357886 carbon_python_sdk-0.2.2/carbon/pydantic/pagination.py
+-rw-r--r--   0        0        0      584 2024-06-01 01:24:51.357963 carbon_python_sdk-0.2.2/carbon/pydantic/presigned_url_response.py
+-rw-r--r--   0        0        0     1341 2024-06-01 01:24:51.358043 carbon_python_sdk-0.2.2/carbon/pydantic/raw_text_input.py
+-rw-r--r--   0        0        0      861 2024-06-01 01:24:51.358125 carbon_python_sdk-0.2.2/carbon/pydantic/resync_file_query_input.py
+-rw-r--r--   0        0        0      588 2024-06-01 01:24:51.358204 carbon_python_sdk-0.2.2/carbon/pydantic/revoke_access_token_input.py
+-rw-r--r--   0        0        0     1515 2024-06-01 01:24:51.358281 carbon_python_sdk-0.2.2/carbon/pydantic/rss_feed_input.py
+-rw-r--r--   0        0        0      832 2024-06-01 01:24:51.358365 carbon_python_sdk-0.2.2/carbon/pydantic/s3_auth_request.py
+-rw-r--r--   0        0        0      744 2024-06-01 01:24:51.358445 carbon_python_sdk-0.2.2/carbon/pydantic/s3_authentication.py
+-rw-r--r--   0        0        0     2360 2024-06-01 01:24:51.358524 carbon_python_sdk-0.2.2/carbon/pydantic/s3_file_sync_input.py
+-rw-r--r--   0        0        0      677 2024-06-01 01:24:51.358603 carbon_python_sdk-0.2.2/carbon/pydantic/s3_get_file_input.py
+-rw-r--r--   0        0        0      829 2024-06-01 01:24:51.358685 carbon_python_sdk-0.2.2/carbon/pydantic/salesforce_authentication.py
+-rw-r--r--   0        0        0      886 2024-06-01 01:24:51.358770 carbon_python_sdk-0.2.2/carbon/pydantic/sharepoint_authentication.py
+-rw-r--r--   0        0        0      494 2024-06-01 01:24:51.358855 carbon_python_sdk-0.2.2/carbon/pydantic/simple_o_auth_data_sources.py
+-rw-r--r--   0        0        0      942 2024-06-01 01:24:51.358940 carbon_python_sdk-0.2.2/carbon/pydantic/single_chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0     2337 2024-06-01 01:24:51.359020 carbon_python_sdk-0.2.2/carbon/pydantic/sitemap_scrape_request.py
+-rw-r--r--   0        0        0      456 2024-06-01 01:24:51.359106 carbon_python_sdk-0.2.2/carbon/pydantic/sitemap_scrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0      458 2024-06-01 01:24:51.359192 carbon_python_sdk-0.2.2/carbon/pydantic/sitemap_scrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0      454 2024-06-01 01:24:51.359279 carbon_python_sdk-0.2.2/carbon/pydantic/sitemap_scrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0      415 2024-06-01 01:24:51.359360 carbon_python_sdk-0.2.2/carbon/pydantic/sitemap_scrape_request_tags.py
+-rw-r--r--   0        0        0      586 2024-06-01 01:24:51.359439 carbon_python_sdk-0.2.2/carbon/pydantic/sync_directory_request.py
+-rw-r--r--   0        0        0      597 2024-06-01 01:24:51.359516 carbon_python_sdk-0.2.2/carbon/pydantic/sync_files_ids.py
+-rw-r--r--   0        0        0     2668 2024-06-01 01:24:51.359596 carbon_python_sdk-0.2.2/carbon/pydantic/sync_files_request.py
+-rw-r--r--   0        0        0     2932 2024-06-01 01:24:51.359674 carbon_python_sdk-0.2.2/carbon/pydantic/sync_options.py
+-rw-r--r--   0        0        0      726 2024-06-01 01:24:51.359750 carbon_python_sdk-0.2.2/carbon/pydantic/text_embedding_generators.py
+-rw-r--r--   0        0        0      630 2024-06-01 01:24:51.359828 carbon_python_sdk-0.2.2/carbon/pydantic/token_response.py
+-rw-r--r--   0        0        0      724 2024-06-01 01:24:51.359908 carbon_python_sdk-0.2.2/carbon/pydantic/update_organization_input.py
+-rw-r--r--   0        0        0     1746 2024-06-01 01:24:51.359990 carbon_python_sdk-0.2.2/carbon/pydantic/update_users_input.py
+-rw-r--r--   0        0        0      430 2024-06-01 01:24:51.360069 carbon_python_sdk-0.2.2/carbon/pydantic/update_users_input_customer_ids.py
+-rw-r--r--   0        0        0     2036 2024-06-01 01:36:07.376823 carbon_python_sdk-0.2.2/carbon/pydantic/upload_file_from_url_input.py
+-rw-r--r--   0        0        0     1582 2024-06-01 01:24:51.360227 carbon_python_sdk-0.2.2/carbon/pydantic/user_configuration.py
+-rw-r--r--   0        0        0     1590 2024-06-01 01:24:51.360309 carbon_python_sdk-0.2.2/carbon/pydantic/user_configuration_nullable.py
+-rw-r--r--   0        0        0     3606 2024-06-01 01:24:51.360387 carbon_python_sdk-0.2.2/carbon/pydantic/user_file.py
+-rw-r--r--   0        0        0      487 2024-06-01 01:24:51.360468 carbon_python_sdk-0.2.2/carbon/pydantic/user_file_embedding_properties.py
+-rw-r--r--   0        0        0      667 2024-06-01 01:24:51.360543 carbon_python_sdk-0.2.2/carbon/pydantic/user_files_v2.py
+-rw-r--r--   0        0        0      578 2024-06-01 01:24:51.360622 carbon_python_sdk-0.2.2/carbon/pydantic/user_request_content.py
+-rw-r--r--   0        0        0     2736 2024-06-01 01:24:51.360701 carbon_python_sdk-0.2.2/carbon/pydantic/user_response.py
+-rw-r--r--   0        0        0      503 2024-06-01 01:24:51.360782 carbon_python_sdk-0.2.2/carbon/pydantic/user_response_auto_sync_enabled_sources.py
+-rw-r--r--   0        0        0      432 2024-06-01 01:24:51.360858 carbon_python_sdk-0.2.2/carbon/pydantic/user_response_unique_file_tags.py
+-rw-r--r--   0        0        0      504 2024-06-01 01:24:51.360936 carbon_python_sdk-0.2.2/carbon/pydantic/utilities_scrape_web_request.py
+-rw-r--r--   0        0        0      714 2024-06-01 01:24:51.361018 carbon_python_sdk-0.2.2/carbon/pydantic/validation_error.py
+-rw-r--r--   0        0        0      440 2024-06-01 01:24:51.361096 carbon_python_sdk-0.2.2/carbon/pydantic/validation_error_loc.py
+-rw-r--r--   0        0        0      982 2024-06-01 01:24:51.361177 carbon_python_sdk-0.2.2/carbon/pydantic/webhook.py
+-rw-r--r--   0        0        0      661 2024-06-01 01:24:51.361253 carbon_python_sdk-0.2.2/carbon/pydantic/webhook_filters.py
+-rw-r--r--   0        0        0      437 2024-06-01 01:24:51.361328 carbon_python_sdk-0.2.2/carbon/pydantic/webhook_filters_ids.py
+-rw-r--r--   0        0        0      936 2024-06-01 01:24:51.361408 carbon_python_sdk-0.2.2/carbon/pydantic/webhook_no_key.py
+-rw-r--r--   0        0        0      443 2024-06-01 01:24:51.361488 carbon_python_sdk-0.2.2/carbon/pydantic/webhook_order_by_columns.py
+-rw-r--r--   0        0        0     1074 2024-06-01 01:24:51.361564 carbon_python_sdk-0.2.2/carbon/pydantic/webhook_query_input.py
+-rw-r--r--   0        0        0      689 2024-06-01 01:24:51.361644 carbon_python_sdk-0.2.2/carbon/pydantic/webhook_query_response.py
+-rw-r--r--   0        0        0      428 2024-06-01 01:24:51.361728 carbon_python_sdk-0.2.2/carbon/pydantic/webhook_status.py
+-rw-r--r--   0        0        0     2380 2024-06-01 01:24:51.361810 carbon_python_sdk-0.2.2/carbon/pydantic/webscrape_request.py
+-rw-r--r--   0        0        0      452 2024-06-01 01:24:51.361893 carbon_python_sdk-0.2.2/carbon/pydantic/webscrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0      454 2024-06-01 01:24:51.361972 carbon_python_sdk-0.2.2/carbon/pydantic/webscrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0      450 2024-06-01 01:24:51.362050 carbon_python_sdk-0.2.2/carbon/pydantic/webscrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0      411 2024-06-01 01:24:51.362128 carbon_python_sdk-0.2.2/carbon/pydantic/webscrape_request_tags.py
+-rw-r--r--   0        0        0      727 2024-06-01 01:24:51.362209 carbon_python_sdk-0.2.2/carbon/pydantic/white_labeling_response.py
+-rw-r--r--   0        0        0      887 2024-06-01 01:24:51.362287 carbon_python_sdk-0.2.2/carbon/pydantic/youtube_transcript_response.py
+-rw-r--r--   0        0        0      616 2024-06-01 01:24:51.362367 carbon_python_sdk-0.2.2/carbon/pydantic/youtube_transcript_response_raw_transcript.py
+-rw-r--r--   0        0        0      433 2024-06-01 01:24:51.362450 carbon_python_sdk-0.2.2/carbon/pydantic/youtube_transcript_response_raw_transcript_item.py
+-rw-r--r--   0        0        0      737 2024-06-01 01:24:51.362530 carbon_python_sdk-0.2.2/carbon/pydantic/zendesk_authentication.py
+-rw-r--r--   0        0        0      848 2024-06-01 01:24:51.362609 carbon_python_sdk-0.2.2/carbon/pydantic/zotero_authentication.py
+-rw-r--r--   0        0        0      654 2024-06-01 01:24:51.362687 carbon_python_sdk-0.2.2/carbon/request_after_hook.py
+-rw-r--r--   0        0        0      712 2024-06-01 01:24:51.362768 carbon_python_sdk-0.2.2/carbon/request_before_hook.py
+-rw-r--r--   0        0        0      677 2024-06-01 01:24:51.362846 carbon_python_sdk-0.2.2/carbon/request_before_url_hook.py
+-rw-r--r--   0        0        0    10974 2024-06-01 01:24:51.362971 carbon_python_sdk-0.2.2/carbon/rest.py
+-rw-r--r--   0        0        0    96042 2024-06-01 01:24:51.363503 carbon_python_sdk-0.2.2/carbon/schemas.py
+-rw-r--r--   0        0        0        0 2024-06-01 01:24:51.363628 carbon_python_sdk-0.2.2/carbon/type/__init__.py
+-rw-r--r--   0        0        0      525 2024-06-01 01:24:51.363710 carbon_python_sdk-0.2.2/carbon/type/add_webhook_props.py
+-rw-r--r--   0        0        0      627 2024-06-01 01:24:51.363792 carbon_python_sdk-0.2.2/carbon/type/body_create_upload_file_uploadfile_post.py
+-rw-r--r--   0        0        0      628 2024-06-01 01:24:51.363906 carbon_python_sdk-0.2.2/carbon/type/chunk_properties.py
+-rw-r--r--   0        0        0      668 2024-06-01 01:24:51.364011 carbon_python_sdk-0.2.2/carbon/type/chunk_properties_nullable.py
+-rw-r--r--   0        0        0      725 2024-06-01 01:24:51.364099 carbon_python_sdk-0.2.2/carbon/type/chunks_and_embeddings.py
+-rw-r--r--   0        0        0      408 2024-06-01 01:24:51.364185 carbon_python_sdk-0.2.2/carbon/type/chunks_and_embeddings_embedding.py
+-rw-r--r--   0        0        0     1117 2024-06-01 01:24:51.364275 carbon_python_sdk-0.2.2/carbon/type/chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0      377 2024-06-01 01:24:51.364361 carbon_python_sdk-0.2.2/carbon/type/chunks_and_embeddings_upload_input_custom_credentials.py
+-rw-r--r--   0        0        0      346 2024-06-01 01:24:51.364440 carbon_python_sdk-0.2.2/carbon/type/configuration_keys.py
+-rw-r--r--   0        0        0      714 2024-06-01 01:24:51.364522 carbon_python_sdk-0.2.2/carbon/type/confluence_authentication.py
+-rw-r--r--   0        0        0     1664 2024-06-01 01:24:51.364610 carbon_python_sdk-0.2.2/carbon/type/connect_data_source_input.py
+-rw-r--r--   0        0        0      733 2024-06-01 01:24:51.364691 carbon_python_sdk-0.2.2/carbon/type/connect_data_source_response.py
+-rw-r--r--   0        0        0      420 2024-06-01 01:24:51.364773 carbon_python_sdk-0.2.2/carbon/type/custom_credentials_type.py
+-rw-r--r--   0        0        0      352 2024-06-01 01:24:51.364856 carbon_python_sdk-0.2.2/carbon/type/data_source_extended_input.py
+-rw-r--r--   0        0        0      395 2024-06-01 01:24:51.364942 carbon_python_sdk-0.2.2/carbon/type/data_source_last_sync_actions.py
+-rw-r--r--   0        0        0      411 2024-06-01 01:24:51.365024 carbon_python_sdk-0.2.2/carbon/type/data_source_sync_statuses.py
+-rw-r--r--   0        0        0      829 2024-06-01 01:24:51.365101 carbon_python_sdk-0.2.2/carbon/type/data_source_type.py
+-rw-r--r--   0        0        0      837 2024-06-01 01:24:51.365184 carbon_python_sdk-0.2.2/carbon/type/data_source_type_nullable.py
+-rw-r--r--   0        0        0      929 2024-06-01 01:24:51.365263 carbon_python_sdk-0.2.2/carbon/type/delete_files_query_input.py
+-rw-r--r--   0        0        0      387 2024-06-01 01:24:51.365351 carbon_python_sdk-0.2.2/carbon/type/delete_files_query_input_file_ids.py
+-rw-r--r--   0        0        0      723 2024-06-01 01:24:51.365431 carbon_python_sdk-0.2.2/carbon/type/delete_files_v2_query_input.py
+-rw-r--r--   0        0        0      647 2024-06-01 01:24:51.365510 carbon_python_sdk-0.2.2/carbon/type/delete_users_input.py
+-rw-r--r--   0        0        0      369 2024-06-01 01:24:51.365589 carbon_python_sdk-0.2.2/carbon/type/delete_users_input_customer_ids.py
+-rw-r--r--   0        0        0      574 2024-06-01 01:24:51.365666 carbon_python_sdk-0.2.2/carbon/type/directory_item.py
+-rw-r--r--   0        0        0     1356 2024-06-01 01:24:51.365745 carbon_python_sdk-0.2.2/carbon/type/document_response.py
+-rw-r--r--   0        0        0      641 2024-06-01 01:24:51.365821 carbon_python_sdk-0.2.2/carbon/type/document_response_list.py
+-rw-r--r--   0        0        0      350 2024-06-01 01:24:51.365902 carbon_python_sdk-0.2.2/carbon/type/document_response_tags.py
+-rw-r--r--   0        0        0      402 2024-06-01 01:24:51.365989 carbon_python_sdk-0.2.2/carbon/type/document_response_vector.py
+-rw-r--r--   0        0        0      877 2024-06-01 01:24:51.366081 carbon_python_sdk-0.2.2/carbon/type/embedding_and_chunk.py
+-rw-r--r--   0        0        0      406 2024-06-01 01:24:51.366171 carbon_python_sdk-0.2.2/carbon/type/embedding_and_chunk_embedding.py
+-rw-r--r--   0        0        0      682 2024-06-01 01:24:51.366256 carbon_python_sdk-0.2.2/carbon/type/embedding_generators.py
+-rw-r--r--   0        0        0      690 2024-06-01 01:24:51.366344 carbon_python_sdk-0.2.2/carbon/type/embedding_generators_nullable.py
+-rw-r--r--   0        0        0      610 2024-06-01 01:24:51.366436 carbon_python_sdk-0.2.2/carbon/type/embedding_properties.py
+-rw-r--r--   0        0        0      729 2024-06-01 01:24:51.366526 carbon_python_sdk-0.2.2/carbon/type/embeddings_and_chunks_filters.py
+-rw-r--r--   0        0        0      409 2024-06-01 01:24:51.366615 carbon_python_sdk-0.2.2/carbon/type/embeddings_and_chunks_order_by_columns.py
+-rw-r--r--   0        0        0     1009 2024-06-01 01:24:51.366704 carbon_python_sdk-0.2.2/carbon/type/embeddings_and_chunks_query_input.py
+-rw-r--r--   0        0        0      694 2024-06-01 01:24:51.366792 carbon_python_sdk-0.2.2/carbon/type/embeddings_and_chunks_response.py
+-rw-r--r--   0        0        0      492 2024-06-01 01:24:51.366880 carbon_python_sdk-0.2.2/carbon/type/external_file_sync_statuses.py
+-rw-r--r--   0        0        0     1189 2024-06-01 01:24:51.366971 carbon_python_sdk-0.2.2/carbon/type/external_source_item.py
+-rw-r--r--   0        0        0      394 2024-06-01 01:24:51.367058 carbon_python_sdk-0.2.2/carbon/type/external_source_items_order_by.py
+-rw-r--r--   0        0        0      689 2024-06-01 01:24:51.367151 carbon_python_sdk-0.2.2/carbon/type/fetch_urls_response.py
+-rw-r--r--   0        0        0      363 2024-06-01 01:24:51.367238 carbon_python_sdk-0.2.2/carbon/type/fetch_urls_response_urls.py
+-rw-r--r--   0        0        0      384 2024-06-01 01:24:51.367326 carbon_python_sdk-0.2.2/carbon/type/file_content_types.py
+-rw-r--r--   0        0        0      392 2024-06-01 01:24:51.367413 carbon_python_sdk-0.2.2/carbon/type/file_content_types_nullable.py
+-rw-r--r--   0        0        0      759 2024-06-01 01:24:51.367498 carbon_python_sdk-0.2.2/carbon/type/file_formats.py
+-rw-r--r--   0        0        0      767 2024-06-01 01:24:51.367585 carbon_python_sdk-0.2.2/carbon/type/file_formats_nullable.py
+-rw-r--r--   0        0        0      823 2024-06-01 01:24:51.367684 carbon_python_sdk-0.2.2/carbon/type/file_statistics.py
+-rw-r--r--   0        0        0      863 2024-06-01 01:24:51.367781 carbon_python_sdk-0.2.2/carbon/type/file_statistics_nullable.py
+-rw-r--r--   0        0        0     1035 2024-06-01 01:24:51.367871 carbon_python_sdk-0.2.2/carbon/type/file_sync_config.py
+-rw-r--r--   0        0        0     1075 2024-06-01 01:24:51.367962 carbon_python_sdk-0.2.2/carbon/type/file_sync_config_nullable.py
+-rw-r--r--   0        0        0      427 2024-06-01 01:24:51.368058 carbon_python_sdk-0.2.2/carbon/type/files_query_user_files_deprecated_response.py
+-rw-r--r--   0        0        0     1449 2024-06-01 01:24:51.368146 carbon_python_sdk-0.2.2/carbon/type/fresh_desk_connect_request.py
+-rw-r--r--   0        0        0      669 2024-06-01 01:24:51.368232 carbon_python_sdk-0.2.2/carbon/type/freskdesk_authentication.py
+-rw-r--r--   0        0        0      565 2024-06-01 01:24:51.368318 carbon_python_sdk-0.2.2/carbon/type/generic_success_response.py
+-rw-r--r--   0        0        0     2735 2024-06-01 01:24:51.368404 carbon_python_sdk-0.2.2/carbon/type/get_embedding_documents_body.py
+-rw-r--r--   0        0        0      391 2024-06-01 01:24:51.368495 carbon_python_sdk-0.2.2/carbon/type/get_embedding_documents_body_file_ids.py
+-rw-r--r--   0        0        0      397 2024-06-01 01:24:51.368586 carbon_python_sdk-0.2.2/carbon/type/get_embedding_documents_body_parent_file_ids.py
+-rw-r--r--   0        0        0      416 2024-06-01 01:24:51.368674 carbon_python_sdk-0.2.2/carbon/type/get_embedding_documents_body_query_vector.py
+-rw-r--r--   0        0        0      359 2024-06-01 01:24:51.368763 carbon_python_sdk-0.2.2/carbon/type/get_embedding_documents_body_tags.py
+-rw-r--r--   0        0        0      670 2024-06-01 01:24:51.368851 carbon_python_sdk-0.2.2/carbon/type/gitbook_authetication.py
+-rw-r--r--   0        0        0     1272 2024-06-01 01:24:51.368939 carbon_python_sdk-0.2.2/carbon/type/gitbook_connect_request.py
+-rw-r--r--   0        0        0     1168 2024-06-01 01:24:51.369017 carbon_python_sdk-0.2.2/carbon/type/gitbook_sync_request.py
+-rw-r--r--   0        0        0      368 2024-06-01 01:24:51.369097 carbon_python_sdk-0.2.2/carbon/type/gitbook_sync_request_space_ids.py
+-rw-r--r--   0        0        0      661 2024-06-01 01:24:51.369176 carbon_python_sdk-0.2.2/carbon/type/github_authentication.py
+-rw-r--r--   0        0        0      709 2024-06-01 01:24:51.369257 carbon_python_sdk-0.2.2/carbon/type/github_connect_request.py
+-rw-r--r--   0        0        0      711 2024-06-01 01:24:51.369339 carbon_python_sdk-0.2.2/carbon/type/github_fetch_repos_request.py
+-rw-r--r--   0        0        0      370 2024-06-01 01:24:51.369420 carbon_python_sdk-0.2.2/carbon/type/github_fetch_repos_request_repos.py
+-rw-r--r--   0        0        0     1351 2024-06-01 01:24:51.369501 carbon_python_sdk-0.2.2/carbon/type/gmail_sync_input.py
+-rw-r--r--   0        0        0      371 2024-06-01 01:24:51.369579 carbon_python_sdk-0.2.2/carbon/type/helpdesk_file_types.py
+-rw-r--r--   0        0        0      630 2024-06-01 01:24:51.369659 carbon_python_sdk-0.2.2/carbon/type/http_validation_error.py
+-rw-r--r--   0        0        0      636 2024-06-01 01:24:51.369741 carbon_python_sdk-0.2.2/carbon/type/hybrid_search_tuning_params.py
+-rw-r--r--   0        0        0      676 2024-06-01 01:24:51.369821 carbon_python_sdk-0.2.2/carbon/type/hybrid_search_tuning_params_nullable.py
+-rw-r--r--   0        0        0     1025 2024-06-01 01:24:51.369899 carbon_python_sdk-0.2.2/carbon/type/list_data_source_items_request.py
+-rw-r--r--   0        0        0      695 2024-06-01 01:24:51.369982 carbon_python_sdk-0.2.2/carbon/type/list_data_source_items_response.py
+-rw-r--r--   0        0        0      854 2024-06-01 01:24:51.370061 carbon_python_sdk-0.2.2/carbon/type/list_items_filters.py
+-rw-r--r--   0        0        0      386 2024-06-01 01:24:51.370140 carbon_python_sdk-0.2.2/carbon/type/list_items_filters_external_ids.py
+-rw-r--r--   0        0        0      378 2024-06-01 01:24:51.370221 carbon_python_sdk-0.2.2/carbon/type/list_items_filters_ids.py
+-rw-r--r--   0        0        0      944 2024-06-01 01:24:51.370304 carbon_python_sdk-0.2.2/carbon/type/list_items_filters_nullable.py
+-rw-r--r--   0        0        0      394 2024-06-01 01:24:51.370407 carbon_python_sdk-0.2.2/carbon/type/list_items_filters_nullable_external_ids.py
+-rw-r--r--   0        0        0      386 2024-06-01 01:24:51.370494 carbon_python_sdk-0.2.2/carbon/type/list_items_filters_nullable_ids.py
+-rw-r--r--   0        0        0      544 2024-06-01 01:24:51.370571 carbon_python_sdk-0.2.2/carbon/type/list_request.py
+-rw-r--r--   0        0        0      587 2024-06-01 01:24:51.370649 carbon_python_sdk-0.2.2/carbon/type/list_response.py
+-rw-r--r--   0        0        0      709 2024-06-01 01:24:51.370736 carbon_python_sdk-0.2.2/carbon/type/modify_user_configuration_input.py
+-rw-r--r--   0        0        0      358 2024-06-01 01:24:51.370822 carbon_python_sdk-0.2.2/carbon/type/multi_modal_embedding_generators.py
+-rw-r--r--   0        0        0      665 2024-06-01 01:24:51.371020 carbon_python_sdk-0.2.2/carbon/type/notion_authentication.py
+-rw-r--r--   0        0        0      696 2024-06-01 01:24:51.371406 carbon_python_sdk-0.2.2/carbon/type/o_auth_authentication.py
+-rw-r--r--   0        0        0     3249 2024-06-01 01:36:07.377506 carbon_python_sdk-0.2.2/carbon/type/o_auth_url_request.py
+-rw-r--r--   0        0        0      356 2024-06-01 01:24:51.371577 carbon_python_sdk-0.2.2/carbon/type/order_dir.py
+-rw-r--r--   0        0        0      358 2024-06-01 01:24:51.371655 carbon_python_sdk-0.2.2/carbon/type/order_dir_v2.py
+-rw-r--r--   0        0        0     1922 2024-06-01 01:24:51.371736 carbon_python_sdk-0.2.2/carbon/type/organization_response.py
+-rw-r--r--   0        0        0     1567 2024-06-01 01:24:51.371821 carbon_python_sdk-0.2.2/carbon/type/organization_user_data_source_api.py
+-rw-r--r--   0        0        0      937 2024-06-01 01:24:51.371906 carbon_python_sdk-0.2.2/carbon/type/organization_user_data_source_filters.py
+-rw-r--r--   0        0        0      395 2024-06-01 01:24:51.371992 carbon_python_sdk-0.2.2/carbon/type/organization_user_data_source_filters_ids.py
+-rw-r--r--   0        0        0      401 2024-06-01 01:24:51.372077 carbon_python_sdk-0.2.2/carbon/type/organization_user_data_source_order_by_columns.py
+-rw-r--r--   0        0        0     1070 2024-06-01 01:24:51.372166 carbon_python_sdk-0.2.2/carbon/type/organization_user_data_source_query_input.py
+-rw-r--r--   0        0        0      767 2024-06-01 01:24:51.372247 carbon_python_sdk-0.2.2/carbon/type/organization_user_data_source_response.py
+-rw-r--r--   0        0        0      759 2024-06-01 01:24:51.372330 carbon_python_sdk-0.2.2/carbon/type/organization_user_file_tag_create.py
+-rw-r--r--   0        0        0      363 2024-06-01 01:24:51.372410 carbon_python_sdk-0.2.2/carbon/type/organization_user_file_tag_create_tags.py
+-rw-r--r--   0        0        0      767 2024-06-01 01:24:51.372495 carbon_python_sdk-0.2.2/carbon/type/organization_user_file_tags_remove.py
+-rw-r--r--   0        0        0      376 2024-06-01 01:24:51.372578 carbon_python_sdk-0.2.2/carbon/type/organization_user_file_tags_remove_tags.py
+-rw-r--r--   0        0        0     5041 2024-06-01 01:24:51.372694 carbon_python_sdk-0.2.2/carbon/type/organization_user_files_to_sync_filters.py
+-rw-r--r--   0        0        0      408 2024-06-01 01:24:51.372907 carbon_python_sdk-0.2.2/carbon/type/organization_user_files_to_sync_filters_external_file_ids.py
+-rw-r--r--   0        0        0      396 2024-06-01 01:24:51.372990 carbon_python_sdk-0.2.2/carbon/type/organization_user_files_to_sync_filters_ids.py
+-rw-r--r--   0        0        0      421 2024-06-01 01:24:51.373193 carbon_python_sdk-0.2.2/carbon/type/organization_user_files_to_sync_filters_organization_user_data_source_id.py
+-rw-r--r--   0        0        0      406 2024-06-01 01:24:51.373286 carbon_python_sdk-0.2.2/carbon/type/organization_user_files_to_sync_filters_parent_file_ids.py
+-rw-r--r--   0        0        0      403 2024-06-01 01:24:51.373370 carbon_python_sdk-0.2.2/carbon/type/organization_user_files_to_sync_filters_request_ids.py
+-rw-r--r--   0        0        0      368 2024-06-01 01:24:51.373453 carbon_python_sdk-0.2.2/carbon/type/organization_user_files_to_sync_filters_tags.py
+-rw-r--r--   0        0        0      440 2024-06-01 01:24:51.373649 carbon_python_sdk-0.2.2/carbon/type/organization_user_files_to_sync_order_by_types.py
+-rw-r--r--   0        0        0     1228 2024-06-01 01:24:51.373739 carbon_python_sdk-0.2.2/carbon/type/organization_user_files_to_sync_query_input.py
+-rw-r--r--   0        0        0      531 2024-06-01 01:24:51.373819 carbon_python_sdk-0.2.2/carbon/type/outh_url_response.py
+-rw-r--r--   0        0        0     1395 2024-06-01 01:24:51.374015 carbon_python_sdk-0.2.2/carbon/type/outlook_sync_input.py
+-rw-r--r--   0        0        0      519 2024-06-01 01:24:51.374096 carbon_python_sdk-0.2.2/carbon/type/pagination.py
+-rw-r--r--   0        0        0      560 2024-06-01 01:24:51.374175 carbon_python_sdk-0.2.2/carbon/type/presigned_url_response.py
+-rw-r--r--   0        0        0      900 2024-06-01 01:24:51.374259 carbon_python_sdk-0.2.2/carbon/type/raw_text_input.py
+-rw-r--r--   0        0        0      662 2024-06-01 01:24:51.374338 carbon_python_sdk-0.2.2/carbon/type/resync_file_query_input.py
+-rw-r--r--   0        0        0      571 2024-06-01 01:24:51.374424 carbon_python_sdk-0.2.2/carbon/type/revoke_access_token_input.py
+-rw-r--r--   0        0        0     1002 2024-06-01 01:24:51.374513 carbon_python_sdk-0.2.2/carbon/type/rss_feed_input.py
+-rw-r--r--   0        0        0      681 2024-06-01 01:24:51.374596 carbon_python_sdk-0.2.2/carbon/type/s3_auth_request.py
+-rw-r--r--   0        0        0      648 2024-06-01 01:24:51.374678 carbon_python_sdk-0.2.2/carbon/type/s3_authentication.py
+-rw-r--r--   0        0        0     1521 2024-06-01 01:24:51.374760 carbon_python_sdk-0.2.2/carbon/type/s3_file_sync_input.py
+-rw-r--r--   0        0        0      570 2024-06-01 01:24:51.374841 carbon_python_sdk-0.2.2/carbon/type/s3_get_file_input.py
+-rw-r--r--   0        0        0      711 2024-06-01 01:24:51.374922 carbon_python_sdk-0.2.2/carbon/type/salesforce_authentication.py
+-rw-r--r--   0        0        0      736 2024-06-01 01:24:51.375013 carbon_python_sdk-0.2.2/carbon/type/sharepoint_authentication.py
+-rw-r--r--   0        0        0      433 2024-06-01 01:24:51.375110 carbon_python_sdk-0.2.2/carbon/type/simple_o_auth_data_sources.py
+-rw-r--r--   0        0        0      831 2024-06-01 01:24:51.375203 carbon_python_sdk-0.2.2/carbon/type/single_chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0     1662 2024-06-01 01:24:51.375292 carbon_python_sdk-0.2.2/carbon/type/sitemap_scrape_request.py
+-rw-r--r--   0        0        0      395 2024-06-01 01:24:51.375390 carbon_python_sdk-0.2.2/carbon/type/sitemap_scrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0      397 2024-06-01 01:24:51.375488 carbon_python_sdk-0.2.2/carbon/type/sitemap_scrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0      393 2024-06-01 01:24:51.375582 carbon_python_sdk-0.2.2/carbon/type/sitemap_scrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0      354 2024-06-01 01:24:51.375807 carbon_python_sdk-0.2.2/carbon/type/sitemap_scrape_request_tags.py
+-rw-r--r--   0        0        0      561 2024-06-01 01:24:51.375898 carbon_python_sdk-0.2.2/carbon/type/sync_directory_request.py
+-rw-r--r--   0        0        0      527 2024-06-01 01:24:51.375984 carbon_python_sdk-0.2.2/carbon/type/sync_files_ids.py
+-rw-r--r--   0        0        0     1816 2024-06-01 01:24:51.376076 carbon_python_sdk-0.2.2/carbon/type/sync_files_request.py
+-rw-r--r--   0        0        0     2058 2024-06-01 01:24:51.376165 carbon_python_sdk-0.2.2/carbon/type/sync_options.py
+-rw-r--r--   0        0        0      665 2024-06-01 01:24:51.376253 carbon_python_sdk-0.2.2/carbon/type/text_embedding_generators.py
+-rw-r--r--   0        0        0      548 2024-06-01 01:24:51.376343 carbon_python_sdk-0.2.2/carbon/type/token_response.py
+-rw-r--r--   0        0        0      697 2024-06-01 01:24:51.376440 carbon_python_sdk-0.2.2/carbon/type/update_organization_input.py
+-rw-r--r--   0        0        0     1513 2024-06-01 01:24:51.376532 carbon_python_sdk-0.2.2/carbon/type/update_users_input.py
+-rw-r--r--   0        0        0      369 2024-06-01 01:24:51.376621 carbon_python_sdk-0.2.2/carbon/type/update_users_input_customer_ids.py
+-rw-r--r--   0        0        0     1269 2024-06-01 01:36:07.377801 carbon_python_sdk-0.2.2/carbon/type/upload_file_from_url_input.py
+-rw-r--r--   0        0        0     1396 2024-06-01 01:24:51.376810 carbon_python_sdk-0.2.2/carbon/type/user_configuration.py
+-rw-r--r--   0        0        0     1436 2024-06-01 01:24:51.376904 carbon_python_sdk-0.2.2/carbon/type/user_configuration_nullable.py
+-rw-r--r--   0        0        0     2555 2024-06-01 01:24:51.376993 carbon_python_sdk-0.2.2/carbon/type/user_file.py
+-rw-r--r--   0        0        0      422 2024-06-01 01:24:51.377088 carbon_python_sdk-0.2.2/carbon/type/user_file_embedding_properties.py
+-rw-r--r--   0        0        0      586 2024-06-01 01:24:51.377181 carbon_python_sdk-0.2.2/carbon/type/user_files_v2.py
+-rw-r--r--   0        0        0      548 2024-06-01 01:24:51.377271 carbon_python_sdk-0.2.2/carbon/type/user_request_content.py
+-rw-r--r--   0        0        0     2011 2024-06-01 01:24:51.377367 carbon_python_sdk-0.2.2/carbon/type/user_response.py
+-rw-r--r--   0        0        0      442 2024-06-01 01:24:51.377466 carbon_python_sdk-0.2.2/carbon/type/user_response_auto_sync_enabled_sources.py
+-rw-r--r--   0        0        0      371 2024-06-01 01:24:51.377565 carbon_python_sdk-0.2.2/carbon/type/user_response_unique_file_tags.py
+-rw-r--r--   0        0        0      439 2024-06-01 01:24:51.377663 carbon_python_sdk-0.2.2/carbon/type/utilities_scrape_web_request.py
+-rw-r--r--   0        0        0      633 2024-06-01 01:24:51.377889 carbon_python_sdk-0.2.2/carbon/type/validation_error.py
+-rw-r--r--   0        0        0      379 2024-06-01 01:24:51.378014 carbon_python_sdk-0.2.2/carbon/type/validation_error_loc.py
+-rw-r--r--   0        0        0      719 2024-06-01 01:24:51.378112 carbon_python_sdk-0.2.2/carbon/type/webhook.py
+-rw-r--r--   0        0        0      613 2024-06-01 01:24:51.378219 carbon_python_sdk-0.2.2/carbon/type/webhook_filters.py
+-rw-r--r--   0        0        0      376 2024-06-01 01:24:51.378311 carbon_python_sdk-0.2.2/carbon/type/webhook_filters_ids.py
+-rw-r--r--   0        0        0      722 2024-06-01 01:24:51.378395 carbon_python_sdk-0.2.2/carbon/type/webhook_no_key.py
+-rw-r--r--   0        0        0      382 2024-06-01 01:24:51.378477 carbon_python_sdk-0.2.2/carbon/type/webhook_order_by_columns.py
+-rw-r--r--   0        0        0      855 2024-06-01 01:24:51.378558 carbon_python_sdk-0.2.2/carbon/type/webhook_query_input.py
+-rw-r--r--   0        0        0      644 2024-06-01 01:24:51.378641 carbon_python_sdk-0.2.2/carbon/type/webhook_query_response.py
+-rw-r--r--   0        0        0      367 2024-06-01 01:24:51.378722 carbon_python_sdk-0.2.2/carbon/type/webhook_status.py
+-rw-r--r--   0        0        0     1633 2024-06-01 01:24:51.378805 carbon_python_sdk-0.2.2/carbon/type/webscrape_request.py
+-rw-r--r--   0        0        0      391 2024-06-01 01:24:51.378892 carbon_python_sdk-0.2.2/carbon/type/webscrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0      393 2024-06-01 01:24:51.378980 carbon_python_sdk-0.2.2/carbon/type/webscrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0      389 2024-06-01 01:24:51.379064 carbon_python_sdk-0.2.2/carbon/type/webscrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0      350 2024-06-01 01:24:51.379146 carbon_python_sdk-0.2.2/carbon/type/webscrape_request_tags.py
+-rw-r--r--   0        0        0      675 2024-06-01 01:24:51.379227 carbon_python_sdk-0.2.2/carbon/type/white_labeling_response.py
+-rw-r--r--   0        0        0      826 2024-06-01 01:24:51.379314 carbon_python_sdk-0.2.2/carbon/type/youtube_transcript_response.py
+-rw-r--r--   0        0        0      551 2024-06-01 01:24:51.379408 carbon_python_sdk-0.2.2/carbon/type/youtube_transcript_response_raw_transcript.py
+-rw-r--r--   0        0        0      372 2024-06-01 01:24:51.379505 carbon_python_sdk-0.2.2/carbon/type/youtube_transcript_response_raw_transcript_item.py
+-rw-r--r--   0        0        0      667 2024-06-01 01:24:51.379589 carbon_python_sdk-0.2.2/carbon/type/zendesk_authentication.py
+-rw-r--r--   0        0        0      711 2024-06-01 01:24:51.379682 carbon_python_sdk-0.2.2/carbon/type/zotero_authentication.py
+-rw-r--r--   0        0        0      514 2024-06-01 01:24:51.379778 carbon_python_sdk-0.2.2/carbon/type_util.py
+-rw-r--r--   0        0        0     3162 2024-06-01 01:24:51.379873 carbon_python_sdk-0.2.2/carbon/validation_metadata.py
+-rw-r--r--   0        0        0      746 2024-06-01 01:36:07.378280 carbon_python_sdk-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0   114776 1970-01-01 00:00:00.000000 carbon_python_sdk-0.2.2/PKG-INFO
```

### Comparing `carbon_python_sdk-0.2.1/LICENSE` & `carbon_python_sdk-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/README.md` & `carbon_python_sdk-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![Visit Carbon](https://raw.githubusercontent.com/Carbon-for-Developers/carbon-sdks/HEAD/python/header.png)](https://carbon.ai)
 
 # Carbon<a id="carbon"></a>
 
 Connect external data to LLMs, no matter the source.
 
 
-[![PyPI](https://img.shields.io/badge/PyPI-v0.2.1-blue)](https://pypi.org/project/carbon-python-sdk/0.2.1)
+[![PyPI](https://img.shields.io/badge/PyPI-v0.2.2-blue)](https://pypi.org/project/carbon-python-sdk/0.2.2)
 [![README.md](https://img.shields.io/badge/README-Click%20Here-green)](https://github.com/Carbon-for-Developers/carbon-sdks/tree/main/python#readme)
 
 </div>
 
 ## Table of Contents<a id="table-of-contents"></a>
 
 <!-- toc -->
@@ -39,14 +39,15 @@
   * [`carbon.files.query_user_files`](#carbonfilesquery_user_files)
   * [`carbon.files.query_user_files_deprecated`](#carbonfilesquery_user_files_deprecated)
   * [`carbon.files.resync`](#carbonfilesresync)
   * [`carbon.files.upload`](#carbonfilesupload)
   * [`carbon.files.upload_from_url`](#carbonfilesupload_from_url)
   * [`carbon.files.upload_text`](#carbonfilesupload_text)
   * [`carbon.health.check`](#carbonhealthcheck)
+  * [`carbon.integrations.cancel`](#carbonintegrationscancel)
   * [`carbon.integrations.connect_data_source`](#carbonintegrationsconnect_data_source)
   * [`carbon.integrations.connect_freshdesk`](#carbonintegrationsconnect_freshdesk)
   * [`carbon.integrations.connect_gitbook`](#carbonintegrationsconnect_gitbook)
   * [`carbon.integrations.create_aws_iam_user`](#carbonintegrationscreate_aws_iam_user)
   * [`carbon.integrations.get_oauth_url`](#carbonintegrationsget_oauth_url)
   * [`carbon.integrations.list_confluence_pages`](#carbonintegrationslist_confluence_pages)
   * [`carbon.integrations.list_data_source_items`](#carbonintegrationslist_data_source_items)
@@ -87,15 +88,15 @@
 ## Requirements<a id="requirements"></a>
 
 Python >=3.7
 
 ## Installation<a id="installation"></a>
 
 ```sh
-pip install carbon-python-sdk==0.2.1
+pip install carbon-python-sdk==0.2.2
 ```
 
 ## Getting Started<a id="getting-started"></a>
 
 ```python
 from carbon import Carbon
 
@@ -1192,14 +1193,15 @@
     embedding_model="OPENAI",
     generate_sparse_vectors=False,
     use_textract=False,
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     parse_pdf_tables_with_ocr=False,
     detect_audio_language=False,
+    media_type="TEXT",
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### url: `str`<a id="url-str"></a>
 
@@ -1225,14 +1227,16 @@
 
 Number of objects per chunk. For csv, tsv, xlsx, and json files only.
 
 ##### parse_pdf_tables_with_ocr: `bool`<a id="parse_pdf_tables_with_ocr-bool"></a>
 
 ##### detect_audio_language: `bool`<a id="detect_audio_language-bool"></a>
 
+##### media_type: [`FileContentTypesNullable`](./carbon/type/file_content_types_nullable.py)<a id="media_type-filecontenttypesnullablecarbontypefile_content_types_nullablepy"></a>
+
 #### ⚙️ Request Body<a id="⚙️-request-body"></a>
 
 [`UploadFileFromUrlInput`](./carbon/type/upload_file_from_url_input.py)
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`UserFile`](./carbon/pydantic/user_file.py)
 
@@ -1319,14 +1323,45 @@
 
 `/health` `get`
 
 [🔙 **Back to Table of Contents**](#table-of-contents)
 
 ---
 
+### `carbon.integrations.cancel`<a id="carbonintegrationscancel"></a>
+
+Cancel Data Source Items Sync
+
+#### 🛠️ Usage<a id="🛠️-usage"></a>
+
+```python
+cancel_response = carbon.integrations.cancel(
+    data_source_id=1,
+)
+```
+
+#### ⚙️ Parameters<a id="⚙️-parameters"></a>
+
+##### data_source_id: `int`<a id="data_source_id-int"></a>
+
+#### ⚙️ Request Body<a id="⚙️-request-body"></a>
+
+[`SyncDirectoryRequest`](./carbon/type/sync_directory_request.py)
+#### 🔄 Return<a id="🔄-return"></a>
+
+[`OrganizationUserDataSourceAPI`](./carbon/pydantic/organization_user_data_source_api.py)
+
+#### 🌐 Endpoint<a id="🌐-endpoint"></a>
+
+`/integrations/items/sync/cancel` `post`
+
+[🔙 **Back to Table of Contents**](#table-of-contents)
+
+---
+
 ### `carbon.integrations.connect_data_source`<a id="carbonintegrationsconnect_data_source"></a>
 
 Connect Data Source
 
 #### 🛠️ Usage<a id="🛠️-usage"></a>
 
 ```python
@@ -1340,15 +1375,15 @@
         "chunk_overlap": 20,
         "skip_embedding_generation": False,
         "embedding_model": "OPENAI",
         "generate_sparse_vectors": False,
         "prepend_filename_to_chunks": False,
         "sync_files_on_connection": True,
         "set_page_as_boundary": False,
-        "request_id": "fceb0182-329c-4e45-953b-885c747cf4a3",
+        "request_id": "368135ce-5cca-4fb5-a19d-42b9a409af35",
         "enable_file_picker": True,
         "sync_source_items": True,
         "incremental_sync": False,
     },
 )
 ```
 
@@ -1593,15 +1628,15 @@
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     salesforce_domain="string_example",
     sync_files_on_connection=True,
     set_page_as_boundary=False,
     data_source_id=1,
     connecting_new_account=False,
-    request_id="ce1b1ec8-be64-491c-9159-c40f85fa0073",
+    request_id="2e662fad-1193-4482-a2d7-ec7b821a9d2b",
     use_ocr=False,
     parse_pdf_tables_with_ocr=False,
     enable_file_picker=True,
     sync_source_items=True,
     incremental_sync=False,
     file_sync_config={
         "auto_synced_source_types": ["ARTICLE"],
@@ -1667,15 +1702,15 @@
 
 Enable OCR for files that support it. Supported formats: pdf
 
 ##### parse_pdf_tables_with_ocr: `Optional[bool]`<a id="parse_pdf_tables_with_ocr-optionalbool"></a>
 
 ##### enable_file_picker: `bool`<a id="enable_file_picker-bool"></a>
 
-Enable integration's file picker for sources that support it. Supported sources: DROPBOX, SHAREPOINT, ONEDRIVE, BOX, GOOGLE_DRIVE
+Enable integration's file picker for sources that support it. Supported sources: SHAREPOINT, BOX, ONEDRIVE, GOOGLE_DRIVE, DROPBOX
 
 ##### sync_source_items: `bool`<a id="sync_source_items-bool"></a>
 
 Enabling this flag will fetch all available content from the source to be listed via list items endpoint
 
 ##### incremental_sync: `bool`<a id="incremental_sync-bool"></a>
 
@@ -1938,15 +1973,15 @@
     chunk_overlap=20,
     skip_embedding_generation=False,
     embedding_model="OPENAI",
     generate_sparse_vectors=False,
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     set_page_as_boundary=False,
-    request_id="9fe9190e-384f-4baa-a416-d51ed93d1be7",
+    request_id="dd2130b5-0f9f-4f3a-b450-f3fa458763ae",
     use_ocr=False,
     parse_pdf_tables_with_ocr=False,
     incremental_sync=False,
     file_sync_config={
         "auto_synced_source_types": ["ARTICLE"],
         "sync_attachments": False,
         "detect_audio_language": False,
@@ -2058,15 +2093,15 @@
     chunk_overlap=20,
     skip_embedding_generation=False,
     embedding_model="OPENAI",
     generate_sparse_vectors=False,
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     set_page_as_boundary=False,
-    request_id="9fe9190e-384f-4baa-a416-d51ed93d1be7",
+    request_id="dd2130b5-0f9f-4f3a-b450-f3fa458763ae",
     use_ocr=False,
     parse_pdf_tables_with_ocr=False,
     incremental_sync=False,
     file_sync_config={
         "auto_synced_source_types": ["ARTICLE"],
         "sync_attachments": False,
         "detect_audio_language": False,
```

### Comparing `carbon_python_sdk-0.2.1/carbon/__init__.py` & `carbon_python_sdk-0.2.2/carbon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Connect external data to LLMs, no matter the source.
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 # import ApiClient
 from carbon.api_client import ApiClient
 
 # import Configuration
 from carbon.configuration import Configuration
```

### Comparing `carbon_python_sdk-0.2.1/carbon/api_client.py` & `carbon_python_sdk-0.2.2/carbon/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2961,15 +2961,15 @@
 0000b900: 5f6e 616d 655d 203d 2068 6561 6465 725f  _name] = header_
 0000b910: 7661 6c75 650a 2020 2020 2020 2020 7365  value.        se
 0000b920: 6c66 2e63 6f6f 6b69 6520 3d20 636f 6f6b  lf.cookie = cook
 0000b930: 6965 0a20 2020 2020 2020 2023 2053 6574  ie.        # Set
 0000b940: 2064 6566 6175 6c74 2055 7365 722d 4167   default User-Ag
 0000b950: 656e 742e 0a20 2020 2020 2020 2073 656c  ent..        sel
 0000b960: 662e 7573 6572 5f61 6765 6e74 203d 2027  f.user_agent = '
-0000b970: 4b6f 6e66 6967 2f30 2e32 2e31 2f70 7974  Konfig/0.2.1/pyt
+0000b970: 4b6f 6e66 6967 2f30 2e32 2e32 2f70 7974  Konfig/0.2.2/pyt
 0000b980: 686f 6e27 0a0a 2020 2020 6465 6620 5f5f  hon'..    def __
 0000b990: 656e 7465 725f 5f28 7365 6c66 293a 0a20  enter__(self):. 
 0000b9a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
 0000b9b0: 6c66 0a0a 2020 2020 6465 6620 5f5f 6578  lf..    def __ex
 0000b9c0: 6974 5f5f 2873 656c 662c 2065 7863 5f74  it__(self, exc_t
 0000b9d0: 7970 652c 2065 7863 5f76 616c 7565 2c20  ype, exc_value, 
 0000b9e0: 7472 6163 6562 6163 6b29 3a0a 2020 2020  traceback):.
```

### Comparing `carbon_python_sdk-0.2.1/carbon/api_response.py` & `carbon_python_sdk-0.2.2/carbon/api_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/path_to_api.py` & `carbon_python_sdk-0.2.2/carbon/apis/path_to_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typing_extensions
 
 from carbon.paths import PathValues
 from carbon.apis.paths.integrations_oauth_url import IntegrationsOauthUrl
 from carbon.apis.paths.integrations_connect import IntegrationsConnect
 from carbon.apis.paths.integrations_items_sync import IntegrationsItemsSync
+from carbon.apis.paths.integrations_items_sync_cancel import IntegrationsItemsSyncCancel
 from carbon.apis.paths.integrations_items_list import IntegrationsItemsList
 from carbon.apis.paths.integrations_files_sync import IntegrationsFilesSync
 from carbon.apis.paths.integrations_confluence_list import IntegrationsConfluenceList
 from carbon.apis.paths.integrations_confluence_sync import IntegrationsConfluenceSync
 from carbon.apis.paths.integrations_s3 import IntegrationsS3
 from carbon.apis.paths.integrations_s3_files import IntegrationsS3Files
 from carbon.apis.paths.integrations_gmail_sync import IntegrationsGmailSync
@@ -63,14 +64,15 @@
 
 PathToApi = typing_extensions.TypedDict(
     'PathToApi',
     {
         PathValues.INTEGRATIONS_OAUTH_URL: IntegrationsOauthUrl,
         PathValues.INTEGRATIONS_CONNECT: IntegrationsConnect,
         PathValues.INTEGRATIONS_ITEMS_SYNC: IntegrationsItemsSync,
+        PathValues.INTEGRATIONS_ITEMS_SYNC_CANCEL: IntegrationsItemsSyncCancel,
         PathValues.INTEGRATIONS_ITEMS_LIST: IntegrationsItemsList,
         PathValues.INTEGRATIONS_FILES_SYNC: IntegrationsFilesSync,
         PathValues.INTEGRATIONS_CONFLUENCE_LIST: IntegrationsConfluenceList,
         PathValues.INTEGRATIONS_CONFLUENCE_SYNC: IntegrationsConfluenceSync,
         PathValues.INTEGRATIONS_S3: IntegrationsS3,
         PathValues.INTEGRATIONS_S3_FILES: IntegrationsS3Files,
         PathValues.INTEGRATIONS_GMAIL_SYNC: IntegrationsGmailSync,
@@ -127,14 +129,15 @@
 )
 
 path_to_api = PathToApi(
     {
         PathValues.INTEGRATIONS_OAUTH_URL: IntegrationsOauthUrl,
         PathValues.INTEGRATIONS_CONNECT: IntegrationsConnect,
         PathValues.INTEGRATIONS_ITEMS_SYNC: IntegrationsItemsSync,
+        PathValues.INTEGRATIONS_ITEMS_SYNC_CANCEL: IntegrationsItemsSyncCancel,
         PathValues.INTEGRATIONS_ITEMS_LIST: IntegrationsItemsList,
         PathValues.INTEGRATIONS_FILES_SYNC: IntegrationsFilesSync,
         PathValues.INTEGRATIONS_CONFLUENCE_LIST: IntegrationsConfluenceList,
         PathValues.INTEGRATIONS_CONFLUENCE_SYNC: IntegrationsConfluenceSync,
         PathValues.INTEGRATIONS_S3: IntegrationsS3,
         PathValues.INTEGRATIONS_S3_FILES: IntegrationsS3Files,
         PathValues.INTEGRATIONS_GMAIL_SYNC: IntegrationsGmailSync,
```

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tag_to_api.py` & `carbon_python_sdk-0.2.2/carbon/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/__init__.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/auth_api_generated.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/auth_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/data_sources_api_generated.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/data_sources_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/embeddings_api_generated.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/embeddings_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/embeddings_api_raw.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/embeddings_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/files_api_generated.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/files_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/files_api_raw.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/files_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/health_api_generated.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/health_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/integrations_api_generated.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/integrations_api_generated.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
     Connect external data to LLMs, no matter the source.
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from carbon.paths.integrations_items_sync_cancel.post import Cancel
 from carbon.paths.integrations_connect.post import ConnectDataSource
 from carbon.paths.integrations_freshdesk.post import ConnectFreshdesk
 from carbon.paths.integrations_gitbook.post import ConnectGitbook
 from carbon.paths.integrations_s3.post import CreateAwsIamUser
 from carbon.paths.integrations_oauth_url.post import GetOauthUrl
 from carbon.paths.integrations_confluence_list.post import ListConfluencePages
 from carbon.paths.integrations_items_list.post import ListDataSourceItems
@@ -30,14 +31,15 @@
 from carbon.paths.integrations_github_sync_repos.post import SyncRepos
 from carbon.paths.integrations_rss_feed.post import SyncRssFeed
 from carbon.paths.integrations_s3_files.post import SyncS3Files
 from carbon.apis.tags.integrations_api_raw import IntegrationsApiRaw
 
 
 class IntegrationsApiGenerated(
+    Cancel,
     ConnectDataSource,
     ConnectFreshdesk,
     ConnectGitbook,
     CreateAwsIamUser,
     GetOauthUrl,
     ListConfluencePages,
     ListDataSourceItems,
```

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/integrations_api_raw.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/integrations_api_raw.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
     Connect external data to LLMs, no matter the source.
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from carbon.paths.integrations_items_sync_cancel.post import CancelRaw
 from carbon.paths.integrations_connect.post import ConnectDataSourceRaw
 from carbon.paths.integrations_freshdesk.post import ConnectFreshdeskRaw
 from carbon.paths.integrations_gitbook.post import ConnectGitbookRaw
 from carbon.paths.integrations_s3.post import CreateAwsIamUserRaw
 from carbon.paths.integrations_oauth_url.post import GetOauthUrlRaw
 from carbon.paths.integrations_confluence_list.post import ListConfluencePagesRaw
 from carbon.paths.integrations_items_list.post import ListDataSourceItemsRaw
@@ -30,14 +31,15 @@
 from carbon.paths.integrations_outlook_sync.post import SyncOutlookRaw
 from carbon.paths.integrations_github_sync_repos.post import SyncReposRaw
 from carbon.paths.integrations_rss_feed.post import SyncRssFeedRaw
 from carbon.paths.integrations_s3_files.post import SyncS3FilesRaw
 
 
 class IntegrationsApiRaw(
+    CancelRaw,
     ConnectDataSourceRaw,
     ConnectFreshdeskRaw,
     ConnectGitbookRaw,
     CreateAwsIamUserRaw,
     GetOauthUrlRaw,
     ListConfluencePagesRaw,
     ListDataSourceItemsRaw,
```

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/organizations_api_generated.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/organizations_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/organizations_api_raw.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/organizations_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/users_api_generated.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/users_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/users_api_raw.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/users_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/utilities_api_generated.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/utilities_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/utilities_api_raw.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/utilities_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/webhooks_api_generated.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/webhooks_api_generated.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/apis/tags/webhooks_api_raw.py` & `carbon_python_sdk-0.2.2/carbon/apis/tags/webhooks_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/client.py` & `carbon_python_sdk-0.2.2/carbon/client.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/client.pyi` & `carbon_python_sdk-0.2.2/carbon/client.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/client_custom.py` & `carbon_python_sdk-0.2.2/carbon/client_custom.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/configuration.py` & `carbon_python_sdk-0.2.2/carbon/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 0.2.1".\
+               "SDK Package Version: 0.2.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `carbon_python_sdk-0.2.1/carbon/exceptions.py` & `carbon_python_sdk-0.2.2/carbon/exceptions.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/exceptions_base.py` & `carbon_python_sdk-0.2.2/carbon/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/add_webhook_props.py` & `carbon_python_sdk-0.2.2/carbon/model/add_webhook_props.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/add_webhook_props.pyi` & `carbon_python_sdk-0.2.2/carbon/model/add_webhook_props.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/body_create_upload_file_uploadfile_post.py` & `carbon_python_sdk-0.2.2/carbon/model/body_create_upload_file_uploadfile_post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/body_create_upload_file_uploadfile_post.pyi` & `carbon_python_sdk-0.2.2/carbon/model/body_create_upload_file_uploadfile_post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/chunk_properties.py` & `carbon_python_sdk-0.2.2/carbon/model/chunk_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/chunk_properties.pyi` & `carbon_python_sdk-0.2.2/carbon/model/chunk_properties.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/chunk_properties_nullable.py` & `carbon_python_sdk-0.2.2/carbon/model/chunk_properties_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/chunk_properties_nullable.pyi` & `carbon_python_sdk-0.2.2/carbon/model/chunk_properties_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings.py` & `carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings.pyi` & `carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_embedding.py` & `carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings_embedding.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_embedding.pyi` & `carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings_embedding.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings_upload_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.py` & `carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.pyi` & `carbon_python_sdk-0.2.2/carbon/model/chunks_and_embeddings_upload_input_custom_credentials.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/configuration_keys.py` & `carbon_python_sdk-0.2.2/carbon/model/configuration_keys.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/configuration_keys.pyi` & `carbon_python_sdk-0.2.2/carbon/model/configuration_keys.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/confluence_authentication.py` & `carbon_python_sdk-0.2.2/carbon/model/confluence_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/confluence_authentication.pyi` & `carbon_python_sdk-0.2.2/carbon/model/confluence_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/connect_data_source_input.py` & `carbon_python_sdk-0.2.2/carbon/model/connect_data_source_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/connect_data_source_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/connect_data_source_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/connect_data_source_response.py` & `carbon_python_sdk-0.2.2/carbon/model/connect_data_source_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/connect_data_source_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/connect_data_source_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/custom_credentials_type.py` & `carbon_python_sdk-0.2.2/carbon/model/custom_credentials_type.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/custom_credentials_type.pyi` & `carbon_python_sdk-0.2.2/carbon/model/custom_credentials_type.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/data_source_extended_input.py` & `carbon_python_sdk-0.2.2/carbon/model/data_source_extended_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/data_source_extended_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/data_source_extended_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/data_source_last_sync_actions.py` & `carbon_python_sdk-0.2.2/carbon/model/data_source_last_sync_actions.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/data_source_last_sync_actions.pyi` & `carbon_python_sdk-0.2.2/carbon/model/data_source_last_sync_actions.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/data_source_sync_statuses.py` & `carbon_python_sdk-0.2.2/carbon/model/data_source_sync_statuses.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/data_source_sync_statuses.pyi` & `carbon_python_sdk-0.2.2/carbon/model/data_source_sync_statuses.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/data_source_type.py` & `carbon_python_sdk-0.2.2/carbon/model/data_source_type.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/data_source_type.pyi` & `carbon_python_sdk-0.2.2/carbon/model/data_source_type.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/data_source_type_nullable.py` & `carbon_python_sdk-0.2.2/carbon/model/data_source_type_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/data_source_type_nullable.pyi` & `carbon_python_sdk-0.2.2/carbon/model/data_source_type_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input.py` & `carbon_python_sdk-0.2.2/carbon/model/delete_files_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/delete_files_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input_file_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/delete_files_query_input_file_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/delete_files_query_input_file_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/delete_files_query_input_file_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/delete_files_v2_query_input.py` & `carbon_python_sdk-0.2.2/carbon/model/delete_files_v2_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/delete_files_v2_query_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/delete_files_v2_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/delete_users_input.py` & `carbon_python_sdk-0.2.2/carbon/model/delete_users_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/delete_users_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/delete_users_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/delete_users_input_customer_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/delete_users_input_customer_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/delete_users_input_customer_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/delete_users_input_customer_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/directory_item.py` & `carbon_python_sdk-0.2.2/carbon/model/directory_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/directory_item.pyi` & `carbon_python_sdk-0.2.2/carbon/model/directory_item.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/document_response.py` & `carbon_python_sdk-0.2.2/carbon/model/document_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/document_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/document_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/document_response_list.py` & `carbon_python_sdk-0.2.2/carbon/model/document_response_list.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/document_response_list.pyi` & `carbon_python_sdk-0.2.2/carbon/model/document_response_list.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/document_response_tags.py` & `carbon_python_sdk-0.2.2/carbon/model/document_response_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/document_response_tags.pyi` & `carbon_python_sdk-0.2.2/carbon/model/document_response_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/document_response_vector.py` & `carbon_python_sdk-0.2.2/carbon/model/document_response_vector.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/document_response_vector.pyi` & `carbon_python_sdk-0.2.2/carbon/model/document_response_vector.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk.py` & `carbon_python_sdk-0.2.2/carbon/model/embedding_and_chunk.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk.pyi` & `carbon_python_sdk-0.2.2/carbon/model/embedding_and_chunk.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk_embedding.py` & `carbon_python_sdk-0.2.2/carbon/model/embedding_and_chunk_embedding.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embedding_and_chunk_embedding.pyi` & `carbon_python_sdk-0.2.2/carbon/model/embedding_and_chunk_embedding.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embedding_generators.py` & `carbon_python_sdk-0.2.2/carbon/model/embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embedding_generators.pyi` & `carbon_python_sdk-0.2.2/carbon/model/embedding_generators.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embedding_generators_nullable.py` & `carbon_python_sdk-0.2.2/carbon/model/embedding_generators_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embedding_generators_nullable.pyi` & `carbon_python_sdk-0.2.2/carbon/model/embedding_generators_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embedding_properties.py` & `carbon_python_sdk-0.2.2/carbon/model/embedding_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embedding_properties.pyi` & `carbon_python_sdk-0.2.2/carbon/model/embedding_properties.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_filters.py` & `carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_filters.pyi` & `carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_filters.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_order_by_columns.py` & `carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_order_by_columns.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_order_by_columns.pyi` & `carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_order_by_columns.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_query_input.py` & `carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_query_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_response.py` & `carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/embeddings_and_chunks_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/embeddings_and_chunks_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/external_file_sync_statuses.py` & `carbon_python_sdk-0.2.2/carbon/model/external_file_sync_statuses.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/external_file_sync_statuses.pyi` & `carbon_python_sdk-0.2.2/carbon/model/external_file_sync_statuses.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/external_source_item.py` & `carbon_python_sdk-0.2.2/carbon/model/external_source_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/external_source_item.pyi` & `carbon_python_sdk-0.2.2/carbon/model/external_source_item.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/external_source_items_order_by.py` & `carbon_python_sdk-0.2.2/carbon/model/external_source_items_order_by.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/external_source_items_order_by.pyi` & `carbon_python_sdk-0.2.2/carbon/model/external_source_items_order_by.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response.py` & `carbon_python_sdk-0.2.2/carbon/model/fetch_urls_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/fetch_urls_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response_urls.py` & `carbon_python_sdk-0.2.2/carbon/model/fetch_urls_response_urls.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/fetch_urls_response_urls.pyi` & `carbon_python_sdk-0.2.2/carbon/model/fetch_urls_response_urls.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_content_types.py` & `carbon_python_sdk-0.2.2/carbon/model/file_content_types.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_content_types.pyi` & `carbon_python_sdk-0.2.2/carbon/model/file_content_types.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_content_types_nullable.py` & `carbon_python_sdk-0.2.2/carbon/model/file_content_types_nullable.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,19 +28,14 @@
     schemas.StrBase,
     schemas.NoneBase,
     schemas.Schema,
     schemas.NoneStrMixin
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
-
-    Used to filter the kind of files (e.g. `TEXT` or `IMAGE`) over which to perform the search. Also
-        plays a role in determining what embedding model is used to embed the query. If `IMAGE` is chosen as the media type,
-        then the embedding model used will be an embedding model that is not text-only, *regardless* of what value is passed
-        for `embedding_model`.
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
             "TEXT": "TEXT",
             "IMAGE": "IMAGE",
```

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_content_types_nullable.pyi` & `carbon_python_sdk-0.2.2/carbon/model/file_content_types_nullable.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -28,19 +28,14 @@
     schemas.StrBase,
     schemas.NoneBase,
     schemas.Schema,
     schemas.NoneStrMixin
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
-
-    Used to filter the kind of files (e.g. `TEXT` or `IMAGE`) over which to perform the search. Also
-        plays a role in determining what embedding model is used to embed the query. If `IMAGE` is chosen as the media type,
-        then the embedding model used will be an embedding model that is not text-only, *regardless* of what value is passed
-        for `embedding_model`.
     """
 
 
     class MetaOapg:
         enum_value_to_name = {
             "TEXT": "TEXT",
             "IMAGE": "IMAGE",
```

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_formats.py` & `carbon_python_sdk-0.2.2/carbon/model/file_formats.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_formats.pyi` & `carbon_python_sdk-0.2.2/carbon/model/file_formats.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_formats_nullable.py` & `carbon_python_sdk-0.2.2/carbon/model/file_formats_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_formats_nullable.pyi` & `carbon_python_sdk-0.2.2/carbon/model/file_formats_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_statistics.py` & `carbon_python_sdk-0.2.2/carbon/model/file_statistics.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_statistics.pyi` & `carbon_python_sdk-0.2.2/carbon/model/file_statistics.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_statistics_nullable.py` & `carbon_python_sdk-0.2.2/carbon/model/file_statistics_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_statistics_nullable.pyi` & `carbon_python_sdk-0.2.2/carbon/model/file_statistics_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_sync_config.py` & `carbon_python_sdk-0.2.2/carbon/model/file_sync_config.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_sync_config.pyi` & `carbon_python_sdk-0.2.2/carbon/model/file_sync_config.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_sync_config_nullable.py` & `carbon_python_sdk-0.2.2/carbon/model/file_sync_config_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/file_sync_config_nullable.pyi` & `carbon_python_sdk-0.2.2/carbon/model/file_sync_config_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/files_query_user_files_deprecated_response.py` & `carbon_python_sdk-0.2.2/carbon/model/files_query_user_files_deprecated_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/files_query_user_files_deprecated_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/files_query_user_files_deprecated_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/fresh_desk_connect_request.py` & `carbon_python_sdk-0.2.2/carbon/model/fresh_desk_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/fresh_desk_connect_request.pyi` & `carbon_python_sdk-0.2.2/carbon/model/fresh_desk_connect_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/freskdesk_authentication.py` & `carbon_python_sdk-0.2.2/carbon/model/freskdesk_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/freskdesk_authentication.pyi` & `carbon_python_sdk-0.2.2/carbon/model/freskdesk_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/generic_success_response.py` & `carbon_python_sdk-0.2.2/carbon/model/generic_success_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/generic_success_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/generic_success_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body.py` & `carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body.pyi` & `carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_file_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_file_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_file_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_file_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_parent_file_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_parent_file_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_parent_file_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_parent_file_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_query_vector.py` & `carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_query_vector.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_query_vector.pyi` & `carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_query_vector.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_tags.py` & `carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/get_embedding_documents_body_tags.pyi` & `carbon_python_sdk-0.2.2/carbon/model/get_embedding_documents_body_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/gitbook_authetication.py` & `carbon_python_sdk-0.2.2/carbon/model/gitbook_authetication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/gitbook_authetication.pyi` & `carbon_python_sdk-0.2.2/carbon/model/gitbook_authetication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/gitbook_connect_request.py` & `carbon_python_sdk-0.2.2/carbon/model/gitbook_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/gitbook_connect_request.pyi` & `carbon_python_sdk-0.2.2/carbon/model/gitbook_connect_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request.py` & `carbon_python_sdk-0.2.2/carbon/model/gitbook_sync_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request.pyi` & `carbon_python_sdk-0.2.2/carbon/model/gitbook_sync_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request_space_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/gitbook_sync_request_space_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/gitbook_sync_request_space_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/gitbook_sync_request_space_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/github_authentication.py` & `carbon_python_sdk-0.2.2/carbon/model/github_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/github_authentication.pyi` & `carbon_python_sdk-0.2.2/carbon/model/github_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/github_connect_request.py` & `carbon_python_sdk-0.2.2/carbon/model/github_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/github_connect_request.pyi` & `carbon_python_sdk-0.2.2/carbon/model/github_connect_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request.py` & `carbon_python_sdk-0.2.2/carbon/model/github_fetch_repos_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request.pyi` & `carbon_python_sdk-0.2.2/carbon/model/github_fetch_repos_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request_repos.py` & `carbon_python_sdk-0.2.2/carbon/model/github_fetch_repos_request_repos.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/github_fetch_repos_request_repos.pyi` & `carbon_python_sdk-0.2.2/carbon/model/github_fetch_repos_request_repos.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/gmail_sync_input.py` & `carbon_python_sdk-0.2.2/carbon/model/gmail_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/gmail_sync_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/gmail_sync_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/helpdesk_file_types.py` & `carbon_python_sdk-0.2.2/carbon/model/helpdesk_file_types.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/helpdesk_file_types.pyi` & `carbon_python_sdk-0.2.2/carbon/model/helpdesk_file_types.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/http_validation_error.py` & `carbon_python_sdk-0.2.2/carbon/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/http_validation_error.pyi` & `carbon_python_sdk-0.2.2/carbon/model/http_validation_error.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params.py` & `carbon_python_sdk-0.2.2/carbon/model/hybrid_search_tuning_params.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params.pyi` & `carbon_python_sdk-0.2.2/carbon/model/hybrid_search_tuning_params.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params_nullable.py` & `carbon_python_sdk-0.2.2/carbon/model/hybrid_search_tuning_params_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/hybrid_search_tuning_params_nullable.pyi` & `carbon_python_sdk-0.2.2/carbon/model/hybrid_search_tuning_params_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_request.py` & `carbon_python_sdk-0.2.2/carbon/model/list_data_source_items_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_request.pyi` & `carbon_python_sdk-0.2.2/carbon/model/list_data_source_items_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_response.py` & `carbon_python_sdk-0.2.2/carbon/model/list_data_source_items_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_data_source_items_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/list_data_source_items_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_items_filters.py` & `carbon_python_sdk-0.2.2/carbon/model/list_items_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_items_filters.pyi` & `carbon_python_sdk-0.2.2/carbon/model/list_items_filters.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_external_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/list_items_filters_external_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_external_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/list_items_filters_external_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/list_items_filters_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/list_items_filters_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable.py` & `carbon_python_sdk-0.2.2/carbon/model/list_items_filters_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable.pyi` & `carbon_python_sdk-0.2.2/carbon/model/list_items_filters_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_external_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/list_items_filters_nullable_external_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_external_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/list_items_filters_nullable_external_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/list_items_filters_nullable_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_items_filters_nullable_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/list_items_filters_nullable_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_request.py` & `carbon_python_sdk-0.2.2/carbon/model/list_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_request.pyi` & `carbon_python_sdk-0.2.2/carbon/model/list_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_response.py` & `carbon_python_sdk-0.2.2/carbon/model/list_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/list_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/list_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/modify_user_configuration_input.py` & `carbon_python_sdk-0.2.2/carbon/model/modify_user_configuration_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/modify_user_configuration_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/modify_user_configuration_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/multi_modal_embedding_generators.py` & `carbon_python_sdk-0.2.2/carbon/model/multi_modal_embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/multi_modal_embedding_generators.pyi` & `carbon_python_sdk-0.2.2/carbon/model/multi_modal_embedding_generators.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/notion_authentication.py` & `carbon_python_sdk-0.2.2/carbon/model/notion_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/notion_authentication.pyi` & `carbon_python_sdk-0.2.2/carbon/model/notion_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/o_auth_authentication.py` & `carbon_python_sdk-0.2.2/carbon/model/o_auth_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/o_auth_authentication.pyi` & `carbon_python_sdk-0.2.2/carbon/model/o_auth_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/o_auth_url_request.py` & `carbon_python_sdk-0.2.2/carbon/model/o_auth_url_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/o_auth_url_request.pyi` & `carbon_python_sdk-0.2.2/carbon/model/o_auth_url_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/order_dir.py` & `carbon_python_sdk-0.2.2/carbon/model/order_dir.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/order_dir.pyi` & `carbon_python_sdk-0.2.2/carbon/model/order_dir.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/order_dir_v2.py` & `carbon_python_sdk-0.2.2/carbon/model/order_dir_v2.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/order_dir_v2.pyi` & `carbon_python_sdk-0.2.2/carbon/model/order_dir_v2.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_response.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_api.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_api.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_api.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_filters.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_filters_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_filters_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_filters_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_order_by_columns.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_order_by_columns.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_order_by_columns.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_order_by_columns.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_query_input.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_query_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_response.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_data_source_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_data_source_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tag_create.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tag_create.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create_tags.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tag_create_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tag_create_tags.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tag_create_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tags_remove.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tags_remove.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove_tags.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tags_remove_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_file_tags_remove_tags.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_file_tags_remove_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_external_file_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_external_file_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_external_file_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_external_file_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_request_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_request_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_request_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_request_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_tags.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_filters_tags.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_filters_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_order_by_types.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_order_by_types.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_order_by_types.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_order_by_types.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_query_input.py` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/organization_user_files_to_sync_query_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/organization_user_files_to_sync_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/outh_url_response.py` & `carbon_python_sdk-0.2.2/carbon/model/outh_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/outh_url_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/outh_url_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/outlook_sync_input.py` & `carbon_python_sdk-0.2.2/carbon/model/outlook_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/outlook_sync_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/outlook_sync_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/pagination.py` & `carbon_python_sdk-0.2.2/carbon/model/pagination.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/pagination.pyi` & `carbon_python_sdk-0.2.2/carbon/model/pagination.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/presigned_url_response.py` & `carbon_python_sdk-0.2.2/carbon/model/presigned_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/presigned_url_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/presigned_url_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/raw_text_input.py` & `carbon_python_sdk-0.2.2/carbon/model/raw_text_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/raw_text_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/raw_text_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/resync_file_query_input.py` & `carbon_python_sdk-0.2.2/carbon/model/resync_file_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/resync_file_query_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/resync_file_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/revoke_access_token_input.py` & `carbon_python_sdk-0.2.2/carbon/model/revoke_access_token_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/revoke_access_token_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/revoke_access_token_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/rss_feed_input.py` & `carbon_python_sdk-0.2.2/carbon/model/rss_feed_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/rss_feed_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/rss_feed_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/s3_auth_request.py` & `carbon_python_sdk-0.2.2/carbon/model/s3_auth_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/s3_auth_request.pyi` & `carbon_python_sdk-0.2.2/carbon/model/s3_auth_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/s3_authentication.py` & `carbon_python_sdk-0.2.2/carbon/model/s3_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/s3_authentication.pyi` & `carbon_python_sdk-0.2.2/carbon/model/s3_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/s3_file_sync_input.py` & `carbon_python_sdk-0.2.2/carbon/model/s3_file_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/s3_file_sync_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/s3_file_sync_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/s3_get_file_input.py` & `carbon_python_sdk-0.2.2/carbon/model/s3_get_file_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/s3_get_file_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/s3_get_file_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/salesforce_authentication.py` & `carbon_python_sdk-0.2.2/carbon/model/salesforce_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/salesforce_authentication.pyi` & `carbon_python_sdk-0.2.2/carbon/model/salesforce_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sharepoint_authentication.py` & `carbon_python_sdk-0.2.2/carbon/model/sharepoint_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sharepoint_authentication.pyi` & `carbon_python_sdk-0.2.2/carbon/model/sharepoint_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/simple_o_auth_data_sources.py` & `carbon_python_sdk-0.2.2/carbon/model/simple_o_auth_data_sources.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/simple_o_auth_data_sources.pyi` & `carbon_python_sdk-0.2.2/carbon/model/simple_o_auth_data_sources.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/single_chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.2.2/carbon/model/single_chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/single_chunks_and_embeddings_upload_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/single_chunks_and_embeddings_upload_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request.py` & `carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request.pyi` & `carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_classes_to_skip.py` & `carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_css_classes_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_classes_to_skip.pyi` & `carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_css_classes_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_selectors_to_skip.py` & `carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_css_selectors_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_css_selectors_to_skip.pyi` & `carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_css_selectors_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_html_tags_to_skip.py` & `carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_html_tags_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_html_tags_to_skip.pyi` & `carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_html_tags_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_tags.py` & `carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sitemap_scrape_request_tags.pyi` & `carbon_python_sdk-0.2.2/carbon/model/sitemap_scrape_request_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sync_directory_request.py` & `carbon_python_sdk-0.2.2/carbon/model/sync_directory_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sync_directory_request.pyi` & `carbon_python_sdk-0.2.2/carbon/model/sync_directory_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sync_files_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/sync_files_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sync_files_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/sync_files_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sync_files_request.py` & `carbon_python_sdk-0.2.2/carbon/model/sync_files_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sync_files_request.pyi` & `carbon_python_sdk-0.2.2/carbon/model/sync_files_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sync_options.py` & `carbon_python_sdk-0.2.2/carbon/model/sync_options.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/sync_options.pyi` & `carbon_python_sdk-0.2.2/carbon/model/sync_options.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/text_embedding_generators.py` & `carbon_python_sdk-0.2.2/carbon/model/text_embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/text_embedding_generators.pyi` & `carbon_python_sdk-0.2.2/carbon/model/text_embedding_generators.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/token_response.py` & `carbon_python_sdk-0.2.2/carbon/model/token_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/token_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/token_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/update_organization_input.py` & `carbon_python_sdk-0.2.2/carbon/model/update_organization_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/update_organization_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/update_organization_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/update_users_input.py` & `carbon_python_sdk-0.2.2/carbon/model/update_users_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/update_users_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/update_users_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/update_users_input_customer_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/update_users_input_customer_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/update_users_input_customer_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/update_users_input_customer_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/upload_file_from_url_input.py` & `carbon_python_sdk-0.2.2/carbon/model/upload_file_from_url_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,28 +125,33 @@
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                     )
             parse_pdf_tables_with_ocr = schemas.BoolSchema
             detect_audio_language = schemas.BoolSchema
+        
+            @staticmethod
+            def media_type() -> typing.Type['FileContentTypesNullable']:
+                return FileContentTypesNullable
             __annotations__ = {
                 "url": url,
                 "file_name": file_name,
                 "chunk_size": chunk_size,
                 "chunk_overlap": chunk_overlap,
                 "skip_embedding_generation": skip_embedding_generation,
                 "set_page_as_boundary": set_page_as_boundary,
                 "embedding_model": embedding_model,
                 "generate_sparse_vectors": generate_sparse_vectors,
                 "use_textract": use_textract,
                 "prepend_filename_to_chunks": prepend_filename_to_chunks,
                 "max_items_per_chunk": max_items_per_chunk,
                 "parse_pdf_tables_with_ocr": parse_pdf_tables_with_ocr,
                 "detect_audio_language": detect_audio_language,
+                "media_type": media_type,
             }
     
     url: MetaOapg.properties.url
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["url"]) -> MetaOapg.properties.url: ...
     
@@ -183,17 +188,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["parse_pdf_tables_with_ocr"]) -> MetaOapg.properties.parse_pdf_tables_with_ocr: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["detect_audio_language"]) -> MetaOapg.properties.detect_audio_language: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["media_type"]) -> 'FileContentTypesNullable': ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["url", "file_name", "chunk_size", "chunk_overlap", "skip_embedding_generation", "set_page_as_boundary", "embedding_model", "generate_sparse_vectors", "use_textract", "prepend_filename_to_chunks", "max_items_per_chunk", "parse_pdf_tables_with_ocr", "detect_audio_language", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["url", "file_name", "chunk_size", "chunk_overlap", "skip_embedding_generation", "set_page_as_boundary", "embedding_model", "generate_sparse_vectors", "use_textract", "prepend_filename_to_chunks", "max_items_per_chunk", "parse_pdf_tables_with_ocr", "detect_audio_language", "media_type", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["url"]) -> MetaOapg.properties.url: ...
     
@@ -230,17 +238,20 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["parse_pdf_tables_with_ocr"]) -> typing.Union[MetaOapg.properties.parse_pdf_tables_with_ocr, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["detect_audio_language"]) -> typing.Union[MetaOapg.properties.detect_audio_language, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["media_type"]) -> typing.Union['FileContentTypesNullable', schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["url", "file_name", "chunk_size", "chunk_overlap", "skip_embedding_generation", "set_page_as_boundary", "embedding_model", "generate_sparse_vectors", "use_textract", "prepend_filename_to_chunks", "max_items_per_chunk", "parse_pdf_tables_with_ocr", "detect_audio_language", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["url", "file_name", "chunk_size", "chunk_overlap", "skip_embedding_generation", "set_page_as_boundary", "embedding_model", "generate_sparse_vectors", "use_textract", "prepend_filename_to_chunks", "max_items_per_chunk", "parse_pdf_tables_with_ocr", "detect_audio_language", "media_type", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         url: typing.Union[MetaOapg.properties.url, str, ],
@@ -252,14 +263,15 @@
         embedding_model: typing.Union['EmbeddingGenerators', schemas.Unset] = schemas.unset,
         generate_sparse_vectors: typing.Union[MetaOapg.properties.generate_sparse_vectors, bool, schemas.Unset] = schemas.unset,
         use_textract: typing.Union[MetaOapg.properties.use_textract, bool, schemas.Unset] = schemas.unset,
         prepend_filename_to_chunks: typing.Union[MetaOapg.properties.prepend_filename_to_chunks, bool, schemas.Unset] = schemas.unset,
         max_items_per_chunk: typing.Union[MetaOapg.properties.max_items_per_chunk, None, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         parse_pdf_tables_with_ocr: typing.Union[MetaOapg.properties.parse_pdf_tables_with_ocr, bool, schemas.Unset] = schemas.unset,
         detect_audio_language: typing.Union[MetaOapg.properties.detect_audio_language, bool, schemas.Unset] = schemas.unset,
+        media_type: typing.Union['FileContentTypesNullable', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'UploadFileFromUrlInput':
         return super().__new__(
             cls,
             *args,
             url=url,
@@ -271,12 +283,14 @@
             embedding_model=embedding_model,
             generate_sparse_vectors=generate_sparse_vectors,
             use_textract=use_textract,
             prepend_filename_to_chunks=prepend_filename_to_chunks,
             max_items_per_chunk=max_items_per_chunk,
             parse_pdf_tables_with_ocr=parse_pdf_tables_with_ocr,
             detect_audio_language=detect_audio_language,
+            media_type=media_type,
             _configuration=_configuration,
             **kwargs,
         )
 
 from carbon.model.embedding_generators import EmbeddingGenerators
+from carbon.model.file_content_types_nullable import FileContentTypesNullable
```

### Comparing `carbon_python_sdk-0.2.1/carbon/model/upload_file_from_url_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/upload_file_from_url_input.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -125,28 +125,33 @@
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                     )
             parse_pdf_tables_with_ocr = schemas.BoolSchema
             detect_audio_language = schemas.BoolSchema
+        
+            @staticmethod
+            def media_type() -> typing.Type['FileContentTypesNullable']:
+                return FileContentTypesNullable
             __annotations__ = {
                 "url": url,
                 "file_name": file_name,
                 "chunk_size": chunk_size,
                 "chunk_overlap": chunk_overlap,
                 "skip_embedding_generation": skip_embedding_generation,
                 "set_page_as_boundary": set_page_as_boundary,
                 "embedding_model": embedding_model,
                 "generate_sparse_vectors": generate_sparse_vectors,
                 "use_textract": use_textract,
                 "prepend_filename_to_chunks": prepend_filename_to_chunks,
                 "max_items_per_chunk": max_items_per_chunk,
                 "parse_pdf_tables_with_ocr": parse_pdf_tables_with_ocr,
                 "detect_audio_language": detect_audio_language,
+                "media_type": media_type,
             }
     
     url: MetaOapg.properties.url
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["url"]) -> MetaOapg.properties.url: ...
     
@@ -183,17 +188,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["parse_pdf_tables_with_ocr"]) -> MetaOapg.properties.parse_pdf_tables_with_ocr: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["detect_audio_language"]) -> MetaOapg.properties.detect_audio_language: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["media_type"]) -> 'FileContentTypesNullable': ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["url", "file_name", "chunk_size", "chunk_overlap", "skip_embedding_generation", "set_page_as_boundary", "embedding_model", "generate_sparse_vectors", "use_textract", "prepend_filename_to_chunks", "max_items_per_chunk", "parse_pdf_tables_with_ocr", "detect_audio_language", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["url", "file_name", "chunk_size", "chunk_overlap", "skip_embedding_generation", "set_page_as_boundary", "embedding_model", "generate_sparse_vectors", "use_textract", "prepend_filename_to_chunks", "max_items_per_chunk", "parse_pdf_tables_with_ocr", "detect_audio_language", "media_type", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["url"]) -> MetaOapg.properties.url: ...
     
@@ -230,17 +238,20 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["parse_pdf_tables_with_ocr"]) -> typing.Union[MetaOapg.properties.parse_pdf_tables_with_ocr, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["detect_audio_language"]) -> typing.Union[MetaOapg.properties.detect_audio_language, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["media_type"]) -> typing.Union['FileContentTypesNullable', schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["url", "file_name", "chunk_size", "chunk_overlap", "skip_embedding_generation", "set_page_as_boundary", "embedding_model", "generate_sparse_vectors", "use_textract", "prepend_filename_to_chunks", "max_items_per_chunk", "parse_pdf_tables_with_ocr", "detect_audio_language", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["url", "file_name", "chunk_size", "chunk_overlap", "skip_embedding_generation", "set_page_as_boundary", "embedding_model", "generate_sparse_vectors", "use_textract", "prepend_filename_to_chunks", "max_items_per_chunk", "parse_pdf_tables_with_ocr", "detect_audio_language", "media_type", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         url: typing.Union[MetaOapg.properties.url, str, ],
@@ -252,14 +263,15 @@
         embedding_model: typing.Union['EmbeddingGenerators', schemas.Unset] = schemas.unset,
         generate_sparse_vectors: typing.Union[MetaOapg.properties.generate_sparse_vectors, bool, schemas.Unset] = schemas.unset,
         use_textract: typing.Union[MetaOapg.properties.use_textract, bool, schemas.Unset] = schemas.unset,
         prepend_filename_to_chunks: typing.Union[MetaOapg.properties.prepend_filename_to_chunks, bool, schemas.Unset] = schemas.unset,
         max_items_per_chunk: typing.Union[MetaOapg.properties.max_items_per_chunk, None, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         parse_pdf_tables_with_ocr: typing.Union[MetaOapg.properties.parse_pdf_tables_with_ocr, bool, schemas.Unset] = schemas.unset,
         detect_audio_language: typing.Union[MetaOapg.properties.detect_audio_language, bool, schemas.Unset] = schemas.unset,
+        media_type: typing.Union['FileContentTypesNullable', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'UploadFileFromUrlInput':
         return super().__new__(
             cls,
             *args,
             url=url,
@@ -271,12 +283,14 @@
             embedding_model=embedding_model,
             generate_sparse_vectors=generate_sparse_vectors,
             use_textract=use_textract,
             prepend_filename_to_chunks=prepend_filename_to_chunks,
             max_items_per_chunk=max_items_per_chunk,
             parse_pdf_tables_with_ocr=parse_pdf_tables_with_ocr,
             detect_audio_language=detect_audio_language,
+            media_type=media_type,
             _configuration=_configuration,
             **kwargs,
         )
 
 from carbon.model.embedding_generators import EmbeddingGenerators
+from carbon.model.file_content_types_nullable import FileContentTypesNullable
```

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_configuration.py` & `carbon_python_sdk-0.2.2/carbon/model/user_configuration.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_configuration.pyi` & `carbon_python_sdk-0.2.2/carbon/model/user_configuration.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_configuration_nullable.py` & `carbon_python_sdk-0.2.2/carbon/model/user_configuration_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_configuration_nullable.pyi` & `carbon_python_sdk-0.2.2/carbon/model/user_configuration_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_file.py` & `carbon_python_sdk-0.2.2/carbon/model/user_file.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_file.pyi` & `carbon_python_sdk-0.2.2/carbon/model/user_file.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_file_embedding_properties.py` & `carbon_python_sdk-0.2.2/carbon/model/user_file_embedding_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_file_embedding_properties.pyi` & `carbon_python_sdk-0.2.2/carbon/model/user_file_embedding_properties.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_files_v2.py` & `carbon_python_sdk-0.2.2/carbon/model/user_files_v2.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_files_v2.pyi` & `carbon_python_sdk-0.2.2/carbon/model/user_files_v2.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_request_content.py` & `carbon_python_sdk-0.2.2/carbon/model/user_request_content.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_request_content.pyi` & `carbon_python_sdk-0.2.2/carbon/model/user_request_content.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_response.py` & `carbon_python_sdk-0.2.2/carbon/model/user_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/user_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_response_auto_sync_enabled_sources.py` & `carbon_python_sdk-0.2.2/carbon/model/user_response_auto_sync_enabled_sources.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_response_auto_sync_enabled_sources.pyi` & `carbon_python_sdk-0.2.2/carbon/model/user_response_auto_sync_enabled_sources.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_response_unique_file_tags.py` & `carbon_python_sdk-0.2.2/carbon/model/user_response_unique_file_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/user_response_unique_file_tags.pyi` & `carbon_python_sdk-0.2.2/carbon/model/user_response_unique_file_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/utilities_scrape_web_request.py` & `carbon_python_sdk-0.2.2/carbon/model/utilities_scrape_web_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/utilities_scrape_web_request.pyi` & `carbon_python_sdk-0.2.2/carbon/model/utilities_scrape_web_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/validation_error.py` & `carbon_python_sdk-0.2.2/carbon/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/validation_error.pyi` & `carbon_python_sdk-0.2.2/carbon/model/validation_error.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/validation_error_loc.py` & `carbon_python_sdk-0.2.2/carbon/model/validation_error_loc.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/validation_error_loc.pyi` & `carbon_python_sdk-0.2.2/carbon/model/validation_error_loc.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook.py` & `carbon_python_sdk-0.2.2/carbon/model/webhook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook.pyi` & `carbon_python_sdk-0.2.2/carbon/model/webhook.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook_filters.py` & `carbon_python_sdk-0.2.2/carbon/model/webhook_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook_filters.pyi` & `carbon_python_sdk-0.2.2/carbon/model/webhook_filters.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook_filters_ids.py` & `carbon_python_sdk-0.2.2/carbon/model/webhook_filters_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook_filters_ids.pyi` & `carbon_python_sdk-0.2.2/carbon/model/webhook_filters_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook_no_key.py` & `carbon_python_sdk-0.2.2/carbon/model/webhook_no_key.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook_no_key.pyi` & `carbon_python_sdk-0.2.2/carbon/model/webhook_no_key.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook_order_by_columns.py` & `carbon_python_sdk-0.2.2/carbon/model/webhook_order_by_columns.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook_order_by_columns.pyi` & `carbon_python_sdk-0.2.2/carbon/model/webhook_order_by_columns.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook_query_input.py` & `carbon_python_sdk-0.2.2/carbon/model/webhook_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook_query_input.pyi` & `carbon_python_sdk-0.2.2/carbon/model/webhook_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook_query_response.py` & `carbon_python_sdk-0.2.2/carbon/model/webhook_query_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook_query_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/webhook_query_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook_status.py` & `carbon_python_sdk-0.2.2/carbon/model/webhook_status.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webhook_status.pyi` & `carbon_python_sdk-0.2.2/carbon/model/webhook_status.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webscrape_request.py` & `carbon_python_sdk-0.2.2/carbon/model/webscrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webscrape_request.pyi` & `carbon_python_sdk-0.2.2/carbon/model/webscrape_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_classes_to_skip.py` & `carbon_python_sdk-0.2.2/carbon/model/webscrape_request_css_classes_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_classes_to_skip.pyi` & `carbon_python_sdk-0.2.2/carbon/model/webscrape_request_css_classes_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_selectors_to_skip.py` & `carbon_python_sdk-0.2.2/carbon/model/webscrape_request_css_selectors_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_css_selectors_to_skip.pyi` & `carbon_python_sdk-0.2.2/carbon/model/webscrape_request_css_selectors_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_html_tags_to_skip.py` & `carbon_python_sdk-0.2.2/carbon/model/webscrape_request_html_tags_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_html_tags_to_skip.pyi` & `carbon_python_sdk-0.2.2/carbon/model/webscrape_request_html_tags_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_tags.py` & `carbon_python_sdk-0.2.2/carbon/model/webscrape_request_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/webscrape_request_tags.pyi` & `carbon_python_sdk-0.2.2/carbon/model/webscrape_request_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/white_labeling_response.py` & `carbon_python_sdk-0.2.2/carbon/model/white_labeling_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/white_labeling_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/white_labeling_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response.py` & `carbon_python_sdk-0.2.2/carbon/model/youtube_transcript_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response.pyi` & `carbon_python_sdk-0.2.2/carbon/model/youtube_transcript_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript.py` & `carbon_python_sdk-0.2.2/carbon/model/youtube_transcript_response_raw_transcript.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript.pyi` & `carbon_python_sdk-0.2.2/carbon/model/youtube_transcript_response_raw_transcript.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript_item.py` & `carbon_python_sdk-0.2.2/carbon/model/youtube_transcript_response_raw_transcript_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/youtube_transcript_response_raw_transcript_item.pyi` & `carbon_python_sdk-0.2.2/carbon/model/youtube_transcript_response_raw_transcript_item.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/zendesk_authentication.py` & `carbon_python_sdk-0.2.2/carbon/model/zendesk_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/zendesk_authentication.pyi` & `carbon_python_sdk-0.2.2/carbon/model/zendesk_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/zotero_authentication.py` & `carbon_python_sdk-0.2.2/carbon/model/zotero_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/model/zotero_authentication.pyi` & `carbon_python_sdk-0.2.2/carbon/model/zotero_authentication.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/models/__init__.py` & `carbon_python_sdk-0.2.2/carbon/models/__init__.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/operation_parameter_map.py` & `carbon_python_sdk-0.2.2/carbon/operation_parameter_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,14 +333,17 @@
             },
             {
                 'name': 'parse_pdf_tables_with_ocr'
             },
             {
                 'name': 'detect_audio_language'
             },
+            {
+                'name': 'media_type'
+            },
         ]
     },
     '/upload_text-POST': {
         'parameters': [
             {
                 'name': 'contents'
             },
@@ -367,14 +370,21 @@
             },
         ]
     },
     '/health-GET': {
         'parameters': [
         ]
     },
+    '/integrations/items/sync/cancel-POST': {
+        'parameters': [
+            {
+                'name': 'data_source_id'
+            },
+        ]
+    },
     '/integrations/connect-POST': {
         'parameters': [
             {
                 'name': 'authentication'
             },
             {
                 'name': 'sync_options'
```

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/__init__.py` & `carbon_python_sdk-0.2.2/carbon/paths/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import enum
 
 
 class PathValues(str, enum.Enum):
     INTEGRATIONS_OAUTH_URL = "/integrations/oauth_url"
     INTEGRATIONS_CONNECT = "/integrations/connect"
     INTEGRATIONS_ITEMS_SYNC = "/integrations/items/sync"
+    INTEGRATIONS_ITEMS_SYNC_CANCEL = "/integrations/items/sync/cancel"
     INTEGRATIONS_ITEMS_LIST = "/integrations/items/list"
     INTEGRATIONS_FILES_SYNC = "/integrations/files/sync"
     INTEGRATIONS_CONFLUENCE_LIST = "/integrations/confluence/list"
     INTEGRATIONS_CONFLUENCE_SYNC = "/integrations/confluence/sync"
     INTEGRATIONS_S3 = "/integrations/s3"
     INTEGRATIONS_S3_FILES = "/integrations/s3/files"
     INTEGRATIONS_GMAIL_SYNC = "/integrations/gmail/sync"
```

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/add_webhook/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/add_webhook/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/add_webhook/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/add_webhook/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/auth_v1_access_token/get.py` & `carbon_python_sdk-0.2.2/carbon/paths/auth_v1_access_token/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/auth_v1_access_token/get.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/auth_v1_access_token/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/auth_v1_white_labeling/get.py` & `carbon_python_sdk-0.2.2/carbon/paths/auth_v1_white_labeling/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/auth_v1_white_labeling/get.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/auth_v1_white_labeling/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/create_user_file_tags/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/create_user_file_tags/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/create_user_file_tags/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/create_user_file_tags/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/delete_files/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/delete_files/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/delete_files/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/delete_files/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/delete_files_v2/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/delete_files_v2/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/delete_files_v2/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/delete_files_v2/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/delete_user_file_tags/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/delete_user_file_tags/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/delete_user_file_tags/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/delete_user_file_tags/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/delete_users/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/delete_users/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/delete_users/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/delete_users/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/delete_webhook_webhook_id/delete.py` & `carbon_python_sdk-0.2.2/carbon/paths/delete_webhook_webhook_id/delete.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/delete_webhook_webhook_id/delete.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/delete_webhook_webhook_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/deletefile_file_id/delete.py` & `carbon_python_sdk-0.2.2/carbon/paths/deletefile_file_id/delete.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/deletefile_file_id/delete.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/deletefile_file_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/embeddings/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/embeddings/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/embeddings/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/embeddings/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/fetch_urls/get.py` & `carbon_python_sdk-0.2.2/carbon/paths/fetch_urls/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/fetch_urls/get.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/fetch_urls/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/fetch_youtube_transcript/get.py` & `carbon_python_sdk-0.2.2/carbon/paths/fetch_youtube_transcript/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/fetch_youtube_transcript/get.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/fetch_youtube_transcript/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/health/get.py` & `carbon_python_sdk-0.2.2/carbon/paths/health/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/health/get.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/health/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_list/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_confluence_list/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_list/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_confluence_list/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_sync/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_confluence_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_confluence_sync/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_confluence_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_connect/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_connect/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_connect/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_connect/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_files_sync/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_files_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_files_sync/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_files_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_freshdesk/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_freshdesk/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_freshdesk/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_freshdesk/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_gitbook/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_gitbook/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_spaces/get.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_gitbook_spaces/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_spaces/get.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_gitbook_spaces/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_sync/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_gitbook_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_gitbook_sync/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_gitbook_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_github/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_github/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_github/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_github/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_github_repos/get.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_github_repos/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_github_repos/get.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_github_repos/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_github_sync_repos/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_github_sync_repos/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_github_sync_repos/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_github_sync_repos/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_sync/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_gmail_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_sync/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_gmail_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_user_labels/get.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_gmail_user_labels/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_gmail_user_labels/get.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_gmail_user_labels/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_items_list/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_items_list/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_items_list/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_items_list/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_items_sync/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_items_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_items_sync/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_items_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_oauth_url/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_oauth_url/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_oauth_url/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_oauth_url/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_sync/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_outlook_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_sync/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_outlook_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_categories/get.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_outlook_user_categories/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_categories/get.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_outlook_user_categories/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_folders/get.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_outlook_user_folders/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_outlook_user_folders/get.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_outlook_user_folders/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_rss_feed/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_rss_feed/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_rss_feed/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_rss_feed/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_s3/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_s3/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_s3/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_s3/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_s3_files/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_s3_files/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/integrations_s3_files/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/integrations_s3_files/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/modify_user_configuration/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/modify_user_configuration/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/modify_user_configuration/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/modify_user_configuration/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/organization/get.py` & `carbon_python_sdk-0.2.2/carbon/paths/organization/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/organization/get.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/organization/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/organization_statistics/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/organization_statistics/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/organization_statistics/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/organization_statistics/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/organization_update/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/organization_update/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/organization_update/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/organization_update/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/parsed_file_file_id/get.py` & `carbon_python_sdk-0.2.2/carbon/paths/parsed_file_file_id/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/parsed_file_file_id/get.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/parsed_file_file_id/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/process_sitemap/get.py` & `carbon_python_sdk-0.2.2/carbon/paths/process_sitemap/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/process_sitemap/get.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/process_sitemap/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/raw_file_file_id/get.py` & `carbon_python_sdk-0.2.2/carbon/paths/raw_file_file_id/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/raw_file_file_id/get.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/raw_file_file_id/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/resync_file/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/resync_file/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/resync_file/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/resync_file/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/revoke_access_token/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/revoke_access_token/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/revoke_access_token/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/revoke_access_token/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/scrape_sitemap/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/scrape_sitemap/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/scrape_sitemap/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/scrape_sitemap/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/search_urls/get.py` & `carbon_python_sdk-0.2.2/carbon/paths/search_urls/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/search_urls/get.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/search_urls/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/text_chunks/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/text_chunks/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/text_chunks/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/text_chunks/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/update_users/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/update_users/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/update_users/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/update_users/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/upload_chunks_and_embeddings/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/upload_chunks_and_embeddings/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/upload_chunks_and_embeddings/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/upload_chunks_and_embeddings/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/upload_file_from_url/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/upload_file_from_url/post.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -31,45 +31,41 @@
 import frozendict  # noqa: F401
 
 from carbon import schemas  # noqa: F401
 
 from carbon.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
 from carbon.model.upload_file_from_url_input import UploadFileFromUrlInput as UploadFileFromUrlInputSchema
 from carbon.model.user_file import UserFile as UserFileSchema
+from carbon.model.file_content_types_nullable import FileContentTypesNullable as FileContentTypesNullableSchema
 from carbon.model.embedding_generators import EmbeddingGenerators as EmbeddingGeneratorsSchema
 
 from carbon.type.embedding_generators import EmbeddingGenerators
 from carbon.type.http_validation_error import HTTPValidationError
+from carbon.type.file_content_types_nullable import FileContentTypesNullable
 from carbon.type.upload_file_from_url_input import UploadFileFromUrlInput
 from carbon.type.user_file import UserFile
 
 from ...api_client import Dictionary
+from carbon.pydantic.file_content_types_nullable import FileContentTypesNullable as FileContentTypesNullablePydantic
 from carbon.pydantic.user_file import UserFile as UserFilePydantic
 from carbon.pydantic.upload_file_from_url_input import UploadFileFromUrlInput as UploadFileFromUrlInputPydantic
 from carbon.pydantic.http_validation_error import HTTPValidationError as HTTPValidationErrorPydantic
 from carbon.pydantic.embedding_generators import EmbeddingGenerators as EmbeddingGeneratorsPydantic
 
-from . import path
-
 # body param
 SchemaForRequestBodyApplicationJson = UploadFileFromUrlInputSchema
 
 
 request_body_upload_file_from_url_input = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-_auth = [
-    'accessToken',
-    'apiKey',
-    'customerId',
-]
 SchemaFor200ResponseBodyApplicationJson = UserFileSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: UserFile
 
@@ -104,18 +100,14 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
@@ -130,14 +122,15 @@
         embedding_model: typing.Optional[EmbeddingGenerators] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         use_textract: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
+        media_type: typing.Optional[FileContentTypesNullable] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
         if url is not None:
             _body["url"] = url
         if file_name is not None:
             _body["file_name"] = file_name
@@ -159,14 +152,16 @@
             _body["prepend_filename_to_chunks"] = prepend_filename_to_chunks
         if max_items_per_chunk is not None:
             _body["max_items_per_chunk"] = max_items_per_chunk
         if parse_pdf_tables_with_ocr is not None:
             _body["parse_pdf_tables_with_ocr"] = parse_pdf_tables_with_ocr
         if detect_audio_language is not None:
             _body["detect_audio_language"] = detect_audio_language
+        if media_type is not None:
+            _body["media_type"] = media_type
         args.body = _body
         return args
 
     async def _aupload_from_url_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
@@ -379,14 +374,15 @@
         embedding_model: typing.Optional[EmbeddingGenerators] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         use_textract: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
+        media_type: typing.Optional[FileContentTypesNullable] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._upload_from_url_mapped_args(
@@ -399,14 +395,15 @@
             embedding_model=embedding_model,
             generate_sparse_vectors=generate_sparse_vectors,
             use_textract=use_textract,
             prepend_filename_to_chunks=prepend_filename_to_chunks,
             max_items_per_chunk=max_items_per_chunk,
             parse_pdf_tables_with_ocr=parse_pdf_tables_with_ocr,
             detect_audio_language=detect_audio_language,
+            media_type=media_type,
         )
         return await self._aupload_from_url_oapg(
             body=args.body,
             **kwargs,
         )
     
     def upload_from_url(
@@ -420,14 +417,15 @@
         embedding_model: typing.Optional[EmbeddingGenerators] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         use_textract: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
+        media_type: typing.Optional[FileContentTypesNullable] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._upload_from_url_mapped_args(
             url=url,
             file_name=file_name,
@@ -438,14 +436,15 @@
             embedding_model=embedding_model,
             generate_sparse_vectors=generate_sparse_vectors,
             use_textract=use_textract,
             prepend_filename_to_chunks=prepend_filename_to_chunks,
             max_items_per_chunk=max_items_per_chunk,
             parse_pdf_tables_with_ocr=parse_pdf_tables_with_ocr,
             detect_audio_language=detect_audio_language,
+            media_type=media_type,
         )
         return self._upload_from_url_oapg(
             body=args.body,
         )
 
 class UploadFromUrl(BaseApi):
 
@@ -460,14 +459,15 @@
         embedding_model: typing.Optional[EmbeddingGenerators] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         use_textract: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
+        media_type: typing.Optional[FileContentTypesNullable] = None,
         validate: bool = False,
         **kwargs,
     ) -> UserFilePydantic:
         raw_response = await self.raw.aupload_from_url(
             url=url,
             file_name=file_name,
             chunk_size=chunk_size,
@@ -477,14 +477,15 @@
             embedding_model=embedding_model,
             generate_sparse_vectors=generate_sparse_vectors,
             use_textract=use_textract,
             prepend_filename_to_chunks=prepend_filename_to_chunks,
             max_items_per_chunk=max_items_per_chunk,
             parse_pdf_tables_with_ocr=parse_pdf_tables_with_ocr,
             detect_audio_language=detect_audio_language,
+            media_type=media_type,
             **kwargs,
         )
         if validate:
             return UserFilePydantic(**raw_response.body)
         return api_client.construct_model_instance(UserFilePydantic, raw_response.body)
     
     
@@ -499,14 +500,15 @@
         embedding_model: typing.Optional[EmbeddingGenerators] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         use_textract: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
+        media_type: typing.Optional[FileContentTypesNullable] = None,
         validate: bool = False,
     ) -> UserFilePydantic:
         raw_response = self.raw.upload_from_url(
             url=url,
             file_name=file_name,
             chunk_size=chunk_size,
             chunk_overlap=chunk_overlap,
@@ -515,14 +517,15 @@
             embedding_model=embedding_model,
             generate_sparse_vectors=generate_sparse_vectors,
             use_textract=use_textract,
             prepend_filename_to_chunks=prepend_filename_to_chunks,
             max_items_per_chunk=max_items_per_chunk,
             parse_pdf_tables_with_ocr=parse_pdf_tables_with_ocr,
             detect_audio_language=detect_audio_language,
+            media_type=media_type,
         )
         if validate:
             return UserFilePydantic(**raw_response.body)
         return api_client.construct_model_instance(UserFilePydantic, raw_response.body)
 
 
 class ApiForpost(BaseApi):
@@ -539,14 +542,15 @@
         embedding_model: typing.Optional[EmbeddingGenerators] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         use_textract: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
+        media_type: typing.Optional[FileContentTypesNullable] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._upload_from_url_mapped_args(
@@ -559,14 +563,15 @@
             embedding_model=embedding_model,
             generate_sparse_vectors=generate_sparse_vectors,
             use_textract=use_textract,
             prepend_filename_to_chunks=prepend_filename_to_chunks,
             max_items_per_chunk=max_items_per_chunk,
             parse_pdf_tables_with_ocr=parse_pdf_tables_with_ocr,
             detect_audio_language=detect_audio_language,
+            media_type=media_type,
         )
         return await self._aupload_from_url_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -580,14 +585,15 @@
         embedding_model: typing.Optional[EmbeddingGenerators] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         use_textract: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
+        media_type: typing.Optional[FileContentTypesNullable] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._upload_from_url_mapped_args(
             url=url,
             file_name=file_name,
@@ -598,12 +604,13 @@
             embedding_model=embedding_model,
             generate_sparse_vectors=generate_sparse_vectors,
             use_textract=use_textract,
             prepend_filename_to_chunks=prepend_filename_to_chunks,
             max_items_per_chunk=max_items_per_chunk,
             parse_pdf_tables_with_ocr=parse_pdf_tables_with_ocr,
             detect_audio_language=detect_audio_language,
+            media_type=media_type,
         )
         return self._upload_from_url_oapg(
             body=args.body,
         )
```

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/upload_file_from_url/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/upload_file_from_url/post.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,38 +31,48 @@
 import frozendict  # noqa: F401
 
 from carbon import schemas  # noqa: F401
 
 from carbon.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
 from carbon.model.upload_file_from_url_input import UploadFileFromUrlInput as UploadFileFromUrlInputSchema
 from carbon.model.user_file import UserFile as UserFileSchema
+from carbon.model.file_content_types_nullable import FileContentTypesNullable as FileContentTypesNullableSchema
 from carbon.model.embedding_generators import EmbeddingGenerators as EmbeddingGeneratorsSchema
 
 from carbon.type.embedding_generators import EmbeddingGenerators
 from carbon.type.http_validation_error import HTTPValidationError
+from carbon.type.file_content_types_nullable import FileContentTypesNullable
 from carbon.type.upload_file_from_url_input import UploadFileFromUrlInput
 from carbon.type.user_file import UserFile
 
 from ...api_client import Dictionary
+from carbon.pydantic.file_content_types_nullable import FileContentTypesNullable as FileContentTypesNullablePydantic
 from carbon.pydantic.user_file import UserFile as UserFilePydantic
 from carbon.pydantic.upload_file_from_url_input import UploadFileFromUrlInput as UploadFileFromUrlInputPydantic
 from carbon.pydantic.http_validation_error import HTTPValidationError as HTTPValidationErrorPydantic
 from carbon.pydantic.embedding_generators import EmbeddingGenerators as EmbeddingGeneratorsPydantic
 
+from . import path
+
 # body param
 SchemaForRequestBodyApplicationJson = UploadFileFromUrlInputSchema
 
 
 request_body_upload_file_from_url_input = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
+_auth = [
+    'accessToken',
+    'apiKey',
+    'customerId',
+]
 SchemaFor200ResponseBodyApplicationJson = UserFileSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: UserFile
 
@@ -97,14 +107,18 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '422': _response_for_422,
+}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
@@ -119,14 +133,15 @@
         embedding_model: typing.Optional[EmbeddingGenerators] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         use_textract: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
+        media_type: typing.Optional[FileContentTypesNullable] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
         if url is not None:
             _body["url"] = url
         if file_name is not None:
             _body["file_name"] = file_name
@@ -148,14 +163,16 @@
             _body["prepend_filename_to_chunks"] = prepend_filename_to_chunks
         if max_items_per_chunk is not None:
             _body["max_items_per_chunk"] = max_items_per_chunk
         if parse_pdf_tables_with_ocr is not None:
             _body["parse_pdf_tables_with_ocr"] = parse_pdf_tables_with_ocr
         if detect_audio_language is not None:
             _body["detect_audio_language"] = detect_audio_language
+        if media_type is not None:
+            _body["media_type"] = media_type
         args.body = _body
         return args
 
     async def _aupload_from_url_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
@@ -368,14 +385,15 @@
         embedding_model: typing.Optional[EmbeddingGenerators] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         use_textract: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
+        media_type: typing.Optional[FileContentTypesNullable] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._upload_from_url_mapped_args(
@@ -388,14 +406,15 @@
             embedding_model=embedding_model,
             generate_sparse_vectors=generate_sparse_vectors,
             use_textract=use_textract,
             prepend_filename_to_chunks=prepend_filename_to_chunks,
             max_items_per_chunk=max_items_per_chunk,
             parse_pdf_tables_with_ocr=parse_pdf_tables_with_ocr,
             detect_audio_language=detect_audio_language,
+            media_type=media_type,
         )
         return await self._aupload_from_url_oapg(
             body=args.body,
             **kwargs,
         )
     
     def upload_from_url(
@@ -409,14 +428,15 @@
         embedding_model: typing.Optional[EmbeddingGenerators] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         use_textract: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
+        media_type: typing.Optional[FileContentTypesNullable] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._upload_from_url_mapped_args(
             url=url,
             file_name=file_name,
@@ -427,14 +447,15 @@
             embedding_model=embedding_model,
             generate_sparse_vectors=generate_sparse_vectors,
             use_textract=use_textract,
             prepend_filename_to_chunks=prepend_filename_to_chunks,
             max_items_per_chunk=max_items_per_chunk,
             parse_pdf_tables_with_ocr=parse_pdf_tables_with_ocr,
             detect_audio_language=detect_audio_language,
+            media_type=media_type,
         )
         return self._upload_from_url_oapg(
             body=args.body,
         )
 
 class UploadFromUrl(BaseApi):
 
@@ -449,14 +470,15 @@
         embedding_model: typing.Optional[EmbeddingGenerators] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         use_textract: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
+        media_type: typing.Optional[FileContentTypesNullable] = None,
         validate: bool = False,
         **kwargs,
     ) -> UserFilePydantic:
         raw_response = await self.raw.aupload_from_url(
             url=url,
             file_name=file_name,
             chunk_size=chunk_size,
@@ -466,14 +488,15 @@
             embedding_model=embedding_model,
             generate_sparse_vectors=generate_sparse_vectors,
             use_textract=use_textract,
             prepend_filename_to_chunks=prepend_filename_to_chunks,
             max_items_per_chunk=max_items_per_chunk,
             parse_pdf_tables_with_ocr=parse_pdf_tables_with_ocr,
             detect_audio_language=detect_audio_language,
+            media_type=media_type,
             **kwargs,
         )
         if validate:
             return UserFilePydantic(**raw_response.body)
         return api_client.construct_model_instance(UserFilePydantic, raw_response.body)
     
     
@@ -488,14 +511,15 @@
         embedding_model: typing.Optional[EmbeddingGenerators] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         use_textract: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
+        media_type: typing.Optional[FileContentTypesNullable] = None,
         validate: bool = False,
     ) -> UserFilePydantic:
         raw_response = self.raw.upload_from_url(
             url=url,
             file_name=file_name,
             chunk_size=chunk_size,
             chunk_overlap=chunk_overlap,
@@ -504,14 +528,15 @@
             embedding_model=embedding_model,
             generate_sparse_vectors=generate_sparse_vectors,
             use_textract=use_textract,
             prepend_filename_to_chunks=prepend_filename_to_chunks,
             max_items_per_chunk=max_items_per_chunk,
             parse_pdf_tables_with_ocr=parse_pdf_tables_with_ocr,
             detect_audio_language=detect_audio_language,
+            media_type=media_type,
         )
         if validate:
             return UserFilePydantic(**raw_response.body)
         return api_client.construct_model_instance(UserFilePydantic, raw_response.body)
 
 
 class ApiForpost(BaseApi):
@@ -528,14 +553,15 @@
         embedding_model: typing.Optional[EmbeddingGenerators] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         use_textract: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
+        media_type: typing.Optional[FileContentTypesNullable] = None,
         **kwargs,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._upload_from_url_mapped_args(
@@ -548,14 +574,15 @@
             embedding_model=embedding_model,
             generate_sparse_vectors=generate_sparse_vectors,
             use_textract=use_textract,
             prepend_filename_to_chunks=prepend_filename_to_chunks,
             max_items_per_chunk=max_items_per_chunk,
             parse_pdf_tables_with_ocr=parse_pdf_tables_with_ocr,
             detect_audio_language=detect_audio_language,
+            media_type=media_type,
         )
         return await self._aupload_from_url_oapg(
             body=args.body,
             **kwargs,
         )
     
     def post(
@@ -569,14 +596,15 @@
         embedding_model: typing.Optional[EmbeddingGenerators] = None,
         generate_sparse_vectors: typing.Optional[bool] = None,
         use_textract: typing.Optional[bool] = None,
         prepend_filename_to_chunks: typing.Optional[bool] = None,
         max_items_per_chunk: typing.Optional[typing.Optional[int]] = None,
         parse_pdf_tables_with_ocr: typing.Optional[bool] = None,
         detect_audio_language: typing.Optional[bool] = None,
+        media_type: typing.Optional[FileContentTypesNullable] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._upload_from_url_mapped_args(
             url=url,
             file_name=file_name,
@@ -587,12 +615,13 @@
             embedding_model=embedding_model,
             generate_sparse_vectors=generate_sparse_vectors,
             use_textract=use_textract,
             prepend_filename_to_chunks=prepend_filename_to_chunks,
             max_items_per_chunk=max_items_per_chunk,
             parse_pdf_tables_with_ocr=parse_pdf_tables_with_ocr,
             detect_audio_language=detect_audio_language,
+            media_type=media_type,
         )
         return self._upload_from_url_oapg(
             body=args.body,
         )
```

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/upload_text/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/upload_text/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/upload_text/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/upload_text/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/uploadfile/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/uploadfile/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/uploadfile/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/uploadfile/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/user/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/user/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/user/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/user/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/user_data_sources/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/user_data_sources/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/user_data_sources/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/user_data_sources/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/user_files/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/user_files/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/user_files/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/user_files/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/user_files_v2/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/user_files_v2/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/user_files_v2/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/user_files_v2/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/web_scrape/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/web_scrape/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/web_scrape/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/web_scrape/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/webhooks/post.py` & `carbon_python_sdk-0.2.2/carbon/paths/webhooks/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/paths/webhooks/post.pyi` & `carbon_python_sdk-0.2.2/carbon/paths/webhooks/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/add_webhook_props.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/add_webhook_props.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/body_create_upload_file_uploadfile_post.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/body_create_upload_file_uploadfile_post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/chunk_properties.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/chunk_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/chunk_properties_nullable.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/chunk_properties_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/chunks_and_embeddings.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/chunks_and_embeddings.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/confluence_authentication.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/confluence_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/connect_data_source_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/connect_data_source_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/connect_data_source_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/connect_data_source_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/data_source_type.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/data_source_type.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/data_source_type_nullable.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/data_source_type_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/delete_files_query_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/delete_files_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/delete_files_v2_query_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/delete_files_v2_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/delete_users_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/delete_users_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/directory_item.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/directory_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/document_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/document_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/document_response_list.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/document_response_list.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/embedding_and_chunk.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/embedding_and_chunk.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/embedding_generators.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/embedding_generators_nullable.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/embedding_generators_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/embedding_properties.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/embedding_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/embeddings_and_chunks_filters.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/embeddings_and_chunks_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/embeddings_and_chunks_query_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/embeddings_and_chunks_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/embeddings_and_chunks_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/embeddings_and_chunks_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/external_file_sync_statuses.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/external_file_sync_statuses.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/external_source_item.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/external_source_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/fetch_urls_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/fetch_urls_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/file_formats.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/file_formats.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/file_formats_nullable.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/file_formats_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/file_statistics.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/file_statistics.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/file_statistics_nullable.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/file_statistics_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/file_sync_config.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/file_sync_config.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/file_sync_config_nullable.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/file_sync_config_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/fresh_desk_connect_request.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/fresh_desk_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/freskdesk_authentication.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/freskdesk_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/generic_success_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/generic_success_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/get_embedding_documents_body.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/get_embedding_documents_body.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/gitbook_authetication.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/gitbook_authetication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/gitbook_connect_request.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/gitbook_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/gitbook_sync_request.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/gitbook_sync_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/github_authentication.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/github_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/github_connect_request.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/github_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/github_fetch_repos_request.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/github_fetch_repos_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/gmail_sync_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/gmail_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/http_validation_error.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/hybrid_search_tuning_params.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/hybrid_search_tuning_params.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/hybrid_search_tuning_params_nullable.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/hybrid_search_tuning_params_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/list_data_source_items_request.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/list_data_source_items_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/list_data_source_items_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/list_data_source_items_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/list_items_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/list_items_filters_nullable.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/list_items_filters_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/list_request.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/list_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/list_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/list_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/modify_user_configuration_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/modify_user_configuration_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/notion_authentication.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/notion_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/o_auth_authentication.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/o_auth_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/o_auth_url_request.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/o_auth_url_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     request_id: typing.Optional[str] = Field(None, alias='request_id')
 
     # Enable OCR for files that support it. Supported formats: pdf
     use_ocr: typing.Optional[typing.Optional[bool]] = Field(None, alias='use_ocr')
 
     parse_pdf_tables_with_ocr: typing.Optional[typing.Optional[bool]] = Field(None, alias='parse_pdf_tables_with_ocr')
 
-    # Enable integration's file picker for sources that support it. Supported sources: DROPBOX, SHAREPOINT, ONEDRIVE, BOX, GOOGLE_DRIVE
+    # Enable integration's file picker for sources that support it. Supported sources: SHAREPOINT, BOX, ONEDRIVE, GOOGLE_DRIVE, DROPBOX
     enable_file_picker: typing.Optional[bool] = Field(None, alias='enable_file_picker')
 
     # Enabling this flag will fetch all available content from the source to be listed via list items endpoint
     sync_source_items: typing.Optional[bool] = Field(None, alias='sync_source_items')
 
     # Only sync files if they have not already been synced or if the embedding properties have changed.         This flag is currently supported by ONEDRIVE, GOOGLE_DRIVE, BOX, DROPBOX. It will be ignored for other data sources.
     incremental_sync: typing.Optional[bool] = Field(None, alias='incremental_sync')
```

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/organization_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/organization_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_api.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_data_source_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_filters.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_data_source_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_query_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_data_source_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_data_source_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_data_source_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_file_tag_create.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_file_tag_create.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_file_tags_remove.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_file_tags_remove.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_filters.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_files_to_sync_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/organization_user_files_to_sync_query_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/organization_user_files_to_sync_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/outh_url_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/outh_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/outlook_sync_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/outlook_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/pagination.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/pagination.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/presigned_url_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/presigned_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/raw_text_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/raw_text_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/resync_file_query_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/resync_file_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/revoke_access_token_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/revoke_access_token_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/rss_feed_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/rss_feed_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/s3_auth_request.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/s3_auth_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/s3_authentication.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/s3_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/s3_file_sync_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/s3_file_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/s3_get_file_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/s3_get_file_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/salesforce_authentication.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/salesforce_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/sharepoint_authentication.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/sharepoint_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/single_chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/single_chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/sitemap_scrape_request.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/sitemap_scrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/sync_directory_request.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/sync_directory_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/sync_files_ids.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/sync_files_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/sync_files_request.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/sync_files_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/sync_options.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/sync_options.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/text_embedding_generators.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/text_embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/token_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/token_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/update_organization_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/update_organization_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/update_users_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/update_users_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/upload_file_from_url_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/upload_file_from_url_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal, TYPE_CHECKING
 from pydantic import BaseModel, Field, RootModel, ConfigDict
 
 from carbon.pydantic.embedding_generators import EmbeddingGenerators
+from carbon.pydantic.file_content_types_nullable import FileContentTypesNullable
 
 class UploadFileFromUrlInput(BaseModel):
     url: str = Field(alias='url')
 
     file_name: typing.Optional[typing.Optional[str]] = Field(None, alias='file_name')
 
     chunk_size: typing.Optional[typing.Optional[int]] = Field(None, alias='chunk_size')
@@ -41,11 +42,13 @@
     # Number of objects per chunk. For csv, tsv, xlsx, and json files only.
     max_items_per_chunk: typing.Optional[typing.Optional[int]] = Field(None, alias='max_items_per_chunk')
 
     parse_pdf_tables_with_ocr: typing.Optional[bool] = Field(None, alias='parse_pdf_tables_with_ocr')
 
     detect_audio_language: typing.Optional[bool] = Field(None, alias='detect_audio_language')
 
+    media_type: typing.Optional[FileContentTypesNullable] = Field(None, alias='media_type')
+
     model_config = ConfigDict(
         protected_namespaces=(),
         arbitrary_types_allowed=True
     )
```

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/user_configuration.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/user_configuration.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/user_configuration_nullable.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/user_configuration_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/user_file.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/user_file.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/user_files_v2.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/user_files_v2.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/user_request_content.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/user_request_content.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/user_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/user_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/validation_error.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/webhook.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/webhook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/webhook_filters.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/webhook_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/webhook_no_key.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/webhook_no_key.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/webhook_query_input.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/webhook_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/webhook_query_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/webhook_query_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/webscrape_request.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/webscrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/white_labeling_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/white_labeling_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/youtube_transcript_response.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/youtube_transcript_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/youtube_transcript_response_raw_transcript.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/youtube_transcript_response_raw_transcript.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/zendesk_authentication.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/zendesk_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/pydantic/zotero_authentication.py` & `carbon_python_sdk-0.2.2/carbon/pydantic/zotero_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/request_after_hook.py` & `carbon_python_sdk-0.2.2/carbon/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/request_before_hook.py` & `carbon_python_sdk-0.2.2/carbon/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/request_before_url_hook.py` & `carbon_python_sdk-0.2.2/carbon/request_before_url_hook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/rest.py` & `carbon_python_sdk-0.2.2/carbon/rest.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/schemas.py` & `carbon_python_sdk-0.2.2/carbon/schemas.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/add_webhook_props.py` & `carbon_python_sdk-0.2.2/carbon/type/add_webhook_props.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/body_create_upload_file_uploadfile_post.py` & `carbon_python_sdk-0.2.2/carbon/type/body_create_upload_file_uploadfile_post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/chunk_properties.py` & `carbon_python_sdk-0.2.2/carbon/type/chunk_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/chunk_properties_nullable.py` & `carbon_python_sdk-0.2.2/carbon/type/chunk_properties_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/chunks_and_embeddings.py` & `carbon_python_sdk-0.2.2/carbon/type/chunks_and_embeddings.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.2.2/carbon/type/chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/confluence_authentication.py` & `carbon_python_sdk-0.2.2/carbon/type/confluence_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/connect_data_source_input.py` & `carbon_python_sdk-0.2.2/carbon/type/connect_data_source_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/connect_data_source_response.py` & `carbon_python_sdk-0.2.2/carbon/type/connect_data_source_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/data_source_type.py` & `carbon_python_sdk-0.2.2/carbon/type/data_source_type.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/data_source_type_nullable.py` & `carbon_python_sdk-0.2.2/carbon/type/data_source_type_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/delete_files_query_input.py` & `carbon_python_sdk-0.2.2/carbon/type/delete_files_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/delete_files_v2_query_input.py` & `carbon_python_sdk-0.2.2/carbon/type/delete_files_v2_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/delete_users_input.py` & `carbon_python_sdk-0.2.2/carbon/type/delete_users_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/directory_item.py` & `carbon_python_sdk-0.2.2/carbon/type/directory_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/document_response.py` & `carbon_python_sdk-0.2.2/carbon/type/document_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/document_response_list.py` & `carbon_python_sdk-0.2.2/carbon/type/document_response_list.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/embedding_and_chunk.py` & `carbon_python_sdk-0.2.2/carbon/type/embedding_and_chunk.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/embedding_generators.py` & `carbon_python_sdk-0.2.2/carbon/type/embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/embedding_generators_nullable.py` & `carbon_python_sdk-0.2.2/carbon/type/embedding_generators_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/embedding_properties.py` & `carbon_python_sdk-0.2.2/carbon/type/embedding_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/embeddings_and_chunks_filters.py` & `carbon_python_sdk-0.2.2/carbon/type/embeddings_and_chunks_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/embeddings_and_chunks_query_input.py` & `carbon_python_sdk-0.2.2/carbon/type/embeddings_and_chunks_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/embeddings_and_chunks_response.py` & `carbon_python_sdk-0.2.2/carbon/type/embeddings_and_chunks_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/external_source_item.py` & `carbon_python_sdk-0.2.2/carbon/type/external_source_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/fetch_urls_response.py` & `carbon_python_sdk-0.2.2/carbon/type/fetch_urls_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/file_formats.py` & `carbon_python_sdk-0.2.2/carbon/type/file_formats.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/file_formats_nullable.py` & `carbon_python_sdk-0.2.2/carbon/type/file_formats_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/file_statistics.py` & `carbon_python_sdk-0.2.2/carbon/type/file_statistics.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/file_statistics_nullable.py` & `carbon_python_sdk-0.2.2/carbon/type/file_statistics_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/file_sync_config.py` & `carbon_python_sdk-0.2.2/carbon/type/file_sync_config.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/file_sync_config_nullable.py` & `carbon_python_sdk-0.2.2/carbon/type/file_sync_config_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/fresh_desk_connect_request.py` & `carbon_python_sdk-0.2.2/carbon/type/fresh_desk_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/freskdesk_authentication.py` & `carbon_python_sdk-0.2.2/carbon/type/freskdesk_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/generic_success_response.py` & `carbon_python_sdk-0.2.2/carbon/type/generic_success_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/get_embedding_documents_body.py` & `carbon_python_sdk-0.2.2/carbon/type/get_embedding_documents_body.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/gitbook_authetication.py` & `carbon_python_sdk-0.2.2/carbon/type/gitbook_authetication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/gitbook_connect_request.py` & `carbon_python_sdk-0.2.2/carbon/type/gitbook_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/gitbook_sync_request.py` & `carbon_python_sdk-0.2.2/carbon/type/gitbook_sync_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/github_authentication.py` & `carbon_python_sdk-0.2.2/carbon/type/github_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/github_connect_request.py` & `carbon_python_sdk-0.2.2/carbon/type/github_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/github_fetch_repos_request.py` & `carbon_python_sdk-0.2.2/carbon/type/github_fetch_repos_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/gmail_sync_input.py` & `carbon_python_sdk-0.2.2/carbon/type/gmail_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/http_validation_error.py` & `carbon_python_sdk-0.2.2/carbon/type/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/hybrid_search_tuning_params.py` & `carbon_python_sdk-0.2.2/carbon/type/hybrid_search_tuning_params.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/hybrid_search_tuning_params_nullable.py` & `carbon_python_sdk-0.2.2/carbon/type/hybrid_search_tuning_params_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/list_data_source_items_request.py` & `carbon_python_sdk-0.2.2/carbon/type/list_data_source_items_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/list_data_source_items_response.py` & `carbon_python_sdk-0.2.2/carbon/type/list_data_source_items_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/list_items_filters.py` & `carbon_python_sdk-0.2.2/carbon/type/list_items_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/list_items_filters_nullable.py` & `carbon_python_sdk-0.2.2/carbon/type/list_items_filters_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/list_request.py` & `carbon_python_sdk-0.2.2/carbon/type/list_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/list_response.py` & `carbon_python_sdk-0.2.2/carbon/type/list_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/modify_user_configuration_input.py` & `carbon_python_sdk-0.2.2/carbon/type/modify_user_configuration_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/notion_authentication.py` & `carbon_python_sdk-0.2.2/carbon/type/notion_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/o_auth_authentication.py` & `carbon_python_sdk-0.2.2/carbon/type/o_auth_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/o_auth_url_request.py` & `carbon_python_sdk-0.2.2/carbon/type/o_auth_url_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     request_id: str
 
     # Enable OCR for files that support it. Supported formats: pdf
     use_ocr: typing.Optional[bool]
 
     parse_pdf_tables_with_ocr: typing.Optional[bool]
 
-    # Enable integration's file picker for sources that support it. Supported sources: DROPBOX, SHAREPOINT, ONEDRIVE, BOX, GOOGLE_DRIVE
+    # Enable integration's file picker for sources that support it. Supported sources: SHAREPOINT, BOX, ONEDRIVE, GOOGLE_DRIVE, DROPBOX
     enable_file_picker: bool
 
     # Enabling this flag will fetch all available content from the source to be listed via list items endpoint
     sync_source_items: bool
 
     # Only sync files if they have not already been synced or if the embedding properties have changed.         This flag is currently supported by ONEDRIVE, GOOGLE_DRIVE, BOX, DROPBOX. It will be ignored for other data sources.
     incremental_sync: bool
```

### Comparing `carbon_python_sdk-0.2.1/carbon/type/organization_response.py` & `carbon_python_sdk-0.2.2/carbon/type/organization_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_api.py` & `carbon_python_sdk-0.2.2/carbon/type/organization_user_data_source_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_filters.py` & `carbon_python_sdk-0.2.2/carbon/type/organization_user_data_source_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_query_input.py` & `carbon_python_sdk-0.2.2/carbon/type/organization_user_data_source_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/organization_user_data_source_response.py` & `carbon_python_sdk-0.2.2/carbon/type/organization_user_data_source_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/organization_user_file_tag_create.py` & `carbon_python_sdk-0.2.2/carbon/type/organization_user_file_tag_create.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/organization_user_file_tags_remove.py` & `carbon_python_sdk-0.2.2/carbon/type/organization_user_file_tags_remove.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_filters.py` & `carbon_python_sdk-0.2.2/carbon/type/organization_user_files_to_sync_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/organization_user_files_to_sync_query_input.py` & `carbon_python_sdk-0.2.2/carbon/type/organization_user_files_to_sync_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/outh_url_response.py` & `carbon_python_sdk-0.2.2/carbon/type/outh_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/outlook_sync_input.py` & `carbon_python_sdk-0.2.2/carbon/type/outlook_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/pagination.py` & `carbon_python_sdk-0.2.2/carbon/type/pagination.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/presigned_url_response.py` & `carbon_python_sdk-0.2.2/carbon/type/presigned_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/raw_text_input.py` & `carbon_python_sdk-0.2.2/carbon/type/raw_text_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/resync_file_query_input.py` & `carbon_python_sdk-0.2.2/carbon/type/resync_file_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/revoke_access_token_input.py` & `carbon_python_sdk-0.2.2/carbon/type/revoke_access_token_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/rss_feed_input.py` & `carbon_python_sdk-0.2.2/carbon/type/rss_feed_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/s3_auth_request.py` & `carbon_python_sdk-0.2.2/carbon/type/s3_auth_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/s3_authentication.py` & `carbon_python_sdk-0.2.2/carbon/type/s3_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/s3_file_sync_input.py` & `carbon_python_sdk-0.2.2/carbon/type/s3_file_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/s3_get_file_input.py` & `carbon_python_sdk-0.2.2/carbon/type/s3_get_file_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/salesforce_authentication.py` & `carbon_python_sdk-0.2.2/carbon/type/salesforce_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/sharepoint_authentication.py` & `carbon_python_sdk-0.2.2/carbon/type/sharepoint_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/single_chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.2.2/carbon/type/single_chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/sitemap_scrape_request.py` & `carbon_python_sdk-0.2.2/carbon/type/sitemap_scrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/sync_directory_request.py` & `carbon_python_sdk-0.2.2/carbon/type/sync_directory_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/sync_files_ids.py` & `carbon_python_sdk-0.2.2/carbon/type/sync_files_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/sync_files_request.py` & `carbon_python_sdk-0.2.2/carbon/type/sync_files_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/sync_options.py` & `carbon_python_sdk-0.2.2/carbon/type/sync_options.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/text_embedding_generators.py` & `carbon_python_sdk-0.2.2/carbon/type/text_embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/token_response.py` & `carbon_python_sdk-0.2.2/carbon/type/token_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/update_organization_input.py` & `carbon_python_sdk-0.2.2/carbon/type/update_organization_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/update_users_input.py` & `carbon_python_sdk-0.2.2/carbon/type/update_users_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/upload_file_from_url_input.py` & `carbon_python_sdk-0.2.2/carbon/type/upload_file_from_url_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal, TYPE_CHECKING
 
 from carbon.type.embedding_generators import EmbeddingGenerators
+from carbon.type.file_content_types_nullable import FileContentTypesNullable
 
 class RequiredUploadFileFromUrlInput(TypedDict):
     url: str
 
 
 class OptionalUploadFileFromUrlInput(TypedDict, total=False):
     file_name: typing.Optional[str]
@@ -42,9 +43,11 @@
     # Number of objects per chunk. For csv, tsv, xlsx, and json files only.
     max_items_per_chunk: typing.Optional[int]
 
     parse_pdf_tables_with_ocr: bool
 
     detect_audio_language: bool
 
+    media_type: typing.Optional[FileContentTypesNullable]
+
 class UploadFileFromUrlInput(RequiredUploadFileFromUrlInput, OptionalUploadFileFromUrlInput):
     pass
```

### Comparing `carbon_python_sdk-0.2.1/carbon/type/user_configuration.py` & `carbon_python_sdk-0.2.2/carbon/type/user_configuration.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/user_configuration_nullable.py` & `carbon_python_sdk-0.2.2/carbon/type/user_configuration_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/user_file.py` & `carbon_python_sdk-0.2.2/carbon/type/user_file.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/user_files_v2.py` & `carbon_python_sdk-0.2.2/carbon/type/user_files_v2.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/user_request_content.py` & `carbon_python_sdk-0.2.2/carbon/type/user_request_content.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/user_response.py` & `carbon_python_sdk-0.2.2/carbon/type/user_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/validation_error.py` & `carbon_python_sdk-0.2.2/carbon/type/validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/webhook.py` & `carbon_python_sdk-0.2.2/carbon/type/webhook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/webhook_filters.py` & `carbon_python_sdk-0.2.2/carbon/type/webhook_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/webhook_no_key.py` & `carbon_python_sdk-0.2.2/carbon/type/webhook_no_key.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/webhook_query_input.py` & `carbon_python_sdk-0.2.2/carbon/type/webhook_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/webhook_query_response.py` & `carbon_python_sdk-0.2.2/carbon/type/webhook_query_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/webscrape_request.py` & `carbon_python_sdk-0.2.2/carbon/type/webscrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/white_labeling_response.py` & `carbon_python_sdk-0.2.2/carbon/type/white_labeling_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/youtube_transcript_response.py` & `carbon_python_sdk-0.2.2/carbon/type/youtube_transcript_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/youtube_transcript_response_raw_transcript.py` & `carbon_python_sdk-0.2.2/carbon/type/youtube_transcript_response_raw_transcript.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/zendesk_authentication.py` & `carbon_python_sdk-0.2.2/carbon/type/zendesk_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type/zotero_authentication.py` & `carbon_python_sdk-0.2.2/carbon/type/zotero_authentication.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/type_util.py` & `carbon_python_sdk-0.2.2/carbon/type_util.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/carbon/validation_metadata.py` & `carbon_python_sdk-0.2.2/carbon/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.2.1/pyproject.toml` & `carbon_python_sdk-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "carbon-python-sdk"
-version = "0.2.1"
+version = "0.2.2"
 description = "Client for Carbon"
 authors = ["Konfig <engineering@konfigthis.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "carbon"}]
 
 [tool.poetry.dependencies]
```

### Comparing `carbon_python_sdk-0.2.1/PKG-INFO` & `carbon_python_sdk-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbon-python-sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: Client for Carbon
 License: MIT
 Author: Konfig
 Author-email: engineering@konfigthis.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -28,15 +28,15 @@
 [![Visit Carbon](https://raw.githubusercontent.com/Carbon-for-Developers/carbon-sdks/HEAD/python/header.png)](https://carbon.ai)
 
 # Carbon<a id="carbon"></a>
 
 Connect external data to LLMs, no matter the source.
 
 
-[![PyPI](https://img.shields.io/badge/PyPI-v0.2.1-blue)](https://pypi.org/project/carbon-python-sdk/0.2.1)
+[![PyPI](https://img.shields.io/badge/PyPI-v0.2.2-blue)](https://pypi.org/project/carbon-python-sdk/0.2.2)
 [![README.md](https://img.shields.io/badge/README-Click%20Here-green)](https://github.com/Carbon-for-Developers/carbon-sdks/tree/main/python#readme)
 
 </div>
 
 ## Table of Contents<a id="table-of-contents"></a>
 
 <!-- toc -->
@@ -64,14 +64,15 @@
   * [`carbon.files.query_user_files`](#carbonfilesquery_user_files)
   * [`carbon.files.query_user_files_deprecated`](#carbonfilesquery_user_files_deprecated)
   * [`carbon.files.resync`](#carbonfilesresync)
   * [`carbon.files.upload`](#carbonfilesupload)
   * [`carbon.files.upload_from_url`](#carbonfilesupload_from_url)
   * [`carbon.files.upload_text`](#carbonfilesupload_text)
   * [`carbon.health.check`](#carbonhealthcheck)
+  * [`carbon.integrations.cancel`](#carbonintegrationscancel)
   * [`carbon.integrations.connect_data_source`](#carbonintegrationsconnect_data_source)
   * [`carbon.integrations.connect_freshdesk`](#carbonintegrationsconnect_freshdesk)
   * [`carbon.integrations.connect_gitbook`](#carbonintegrationsconnect_gitbook)
   * [`carbon.integrations.create_aws_iam_user`](#carbonintegrationscreate_aws_iam_user)
   * [`carbon.integrations.get_oauth_url`](#carbonintegrationsget_oauth_url)
   * [`carbon.integrations.list_confluence_pages`](#carbonintegrationslist_confluence_pages)
   * [`carbon.integrations.list_data_source_items`](#carbonintegrationslist_data_source_items)
@@ -112,15 +113,15 @@
 ## Requirements<a id="requirements"></a>
 
 Python >=3.7
 
 ## Installation<a id="installation"></a>
 
 ```sh
-pip install carbon-python-sdk==0.2.1
+pip install carbon-python-sdk==0.2.2
 ```
 
 ## Getting Started<a id="getting-started"></a>
 
 ```python
 from carbon import Carbon
 
@@ -1217,14 +1218,15 @@
     embedding_model="OPENAI",
     generate_sparse_vectors=False,
     use_textract=False,
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     parse_pdf_tables_with_ocr=False,
     detect_audio_language=False,
+    media_type="TEXT",
 )
 ```
 
 #### ⚙️ Parameters<a id="⚙️-parameters"></a>
 
 ##### url: `str`<a id="url-str"></a>
 
@@ -1250,14 +1252,16 @@
 
 Number of objects per chunk. For csv, tsv, xlsx, and json files only.
 
 ##### parse_pdf_tables_with_ocr: `bool`<a id="parse_pdf_tables_with_ocr-bool"></a>
 
 ##### detect_audio_language: `bool`<a id="detect_audio_language-bool"></a>
 
+##### media_type: [`FileContentTypesNullable`](./carbon/type/file_content_types_nullable.py)<a id="media_type-filecontenttypesnullablecarbontypefile_content_types_nullablepy"></a>
+
 #### ⚙️ Request Body<a id="⚙️-request-body"></a>
 
 [`UploadFileFromUrlInput`](./carbon/type/upload_file_from_url_input.py)
 #### 🔄 Return<a id="🔄-return"></a>
 
 [`UserFile`](./carbon/pydantic/user_file.py)
 
@@ -1344,14 +1348,45 @@
 
 `/health` `get`
 
 [🔙 **Back to Table of Contents**](#table-of-contents)
 
 ---
 
+### `carbon.integrations.cancel`<a id="carbonintegrationscancel"></a>
+
+Cancel Data Source Items Sync
+
+#### 🛠️ Usage<a id="🛠️-usage"></a>
+
+```python
+cancel_response = carbon.integrations.cancel(
+    data_source_id=1,
+)
+```
+
+#### ⚙️ Parameters<a id="⚙️-parameters"></a>
+
+##### data_source_id: `int`<a id="data_source_id-int"></a>
+
+#### ⚙️ Request Body<a id="⚙️-request-body"></a>
+
+[`SyncDirectoryRequest`](./carbon/type/sync_directory_request.py)
+#### 🔄 Return<a id="🔄-return"></a>
+
+[`OrganizationUserDataSourceAPI`](./carbon/pydantic/organization_user_data_source_api.py)
+
+#### 🌐 Endpoint<a id="🌐-endpoint"></a>
+
+`/integrations/items/sync/cancel` `post`
+
+[🔙 **Back to Table of Contents**](#table-of-contents)
+
+---
+
 ### `carbon.integrations.connect_data_source`<a id="carbonintegrationsconnect_data_source"></a>
 
 Connect Data Source
 
 #### 🛠️ Usage<a id="🛠️-usage"></a>
 
 ```python
@@ -1365,15 +1400,15 @@
         "chunk_overlap": 20,
         "skip_embedding_generation": False,
         "embedding_model": "OPENAI",
         "generate_sparse_vectors": False,
         "prepend_filename_to_chunks": False,
         "sync_files_on_connection": True,
         "set_page_as_boundary": False,
-        "request_id": "fceb0182-329c-4e45-953b-885c747cf4a3",
+        "request_id": "368135ce-5cca-4fb5-a19d-42b9a409af35",
         "enable_file_picker": True,
         "sync_source_items": True,
         "incremental_sync": False,
     },
 )
 ```
 
@@ -1618,15 +1653,15 @@
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     salesforce_domain="string_example",
     sync_files_on_connection=True,
     set_page_as_boundary=False,
     data_source_id=1,
     connecting_new_account=False,
-    request_id="ce1b1ec8-be64-491c-9159-c40f85fa0073",
+    request_id="2e662fad-1193-4482-a2d7-ec7b821a9d2b",
     use_ocr=False,
     parse_pdf_tables_with_ocr=False,
     enable_file_picker=True,
     sync_source_items=True,
     incremental_sync=False,
     file_sync_config={
         "auto_synced_source_types": ["ARTICLE"],
@@ -1692,15 +1727,15 @@
 
 Enable OCR for files that support it. Supported formats: pdf
 
 ##### parse_pdf_tables_with_ocr: `Optional[bool]`<a id="parse_pdf_tables_with_ocr-optionalbool"></a>
 
 ##### enable_file_picker: `bool`<a id="enable_file_picker-bool"></a>
 
-Enable integration's file picker for sources that support it. Supported sources: DROPBOX, SHAREPOINT, ONEDRIVE, BOX, GOOGLE_DRIVE
+Enable integration's file picker for sources that support it. Supported sources: SHAREPOINT, BOX, ONEDRIVE, GOOGLE_DRIVE, DROPBOX
 
 ##### sync_source_items: `bool`<a id="sync_source_items-bool"></a>
 
 Enabling this flag will fetch all available content from the source to be listed via list items endpoint
 
 ##### incremental_sync: `bool`<a id="incremental_sync-bool"></a>
 
@@ -1963,15 +1998,15 @@
     chunk_overlap=20,
     skip_embedding_generation=False,
     embedding_model="OPENAI",
     generate_sparse_vectors=False,
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     set_page_as_boundary=False,
-    request_id="9fe9190e-384f-4baa-a416-d51ed93d1be7",
+    request_id="dd2130b5-0f9f-4f3a-b450-f3fa458763ae",
     use_ocr=False,
     parse_pdf_tables_with_ocr=False,
     incremental_sync=False,
     file_sync_config={
         "auto_synced_source_types": ["ARTICLE"],
         "sync_attachments": False,
         "detect_audio_language": False,
@@ -2083,15 +2118,15 @@
     chunk_overlap=20,
     skip_embedding_generation=False,
     embedding_model="OPENAI",
     generate_sparse_vectors=False,
     prepend_filename_to_chunks=False,
     max_items_per_chunk=1,
     set_page_as_boundary=False,
-    request_id="9fe9190e-384f-4baa-a416-d51ed93d1be7",
+    request_id="dd2130b5-0f9f-4f3a-b450-f3fa458763ae",
     use_ocr=False,
     parse_pdf_tables_with_ocr=False,
     incremental_sync=False,
     file_sync_config={
         "auto_synced_source_types": ["ARTICLE"],
         "sync_attachments": False,
         "detect_audio_language": False,
```

