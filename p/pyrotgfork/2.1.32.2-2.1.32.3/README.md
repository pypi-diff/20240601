# Comparing `tmp/pyrotgfork-2.1.32.2.tar.gz` & `tmp/pyrotgfork-2.1.32.3.tar.gz`

## Comparing `pyrotgfork-2.1.32.2.tar` & `pyrotgfork-2.1.32.3.tar`

### file list

```diff
@@ -1,514 +1,516 @@
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/__init__.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/api/__init__.py
--rw-r--r--   0        0        0    22468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/api/compiler.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/api/source/auth_key.tl
--rw-r--r--   0        0        0   212645 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/api/source/main_api.tl
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/api/source/sys_msgs.tl
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/api/template/combinator.txt
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/api/template/type.txt
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/errors/__init__.py
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/errors/compiler.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/errors/sort.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0        0        0    34482 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/errors/template/class.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/compiler/errors/template/sub_class.txt
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/__init__.py
--rw-r--r--   0        0        0    46619 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/client.py
--rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/dispatcher.py
--rw-r--r--   0        0        0   208021 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/emoji.py
--rw-r--r--   0        0        0    16314 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/file_id.py
--rw-r--r--   0        0        0    28542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/filters.py
--rw-r--r--   0        0        0    62000 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/mime_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/py.typed
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/sync.py
--rw-r--r--   0        0        0    17490 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/utils.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/connection/__init__.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/connection/connection.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/connection/transport/__init__.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/crypto/__init__.py
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/crypto/aes.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/crypto/mtproto.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/crypto/prime.py
--rw-r--r--   0        0        0    13437 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/crypto/rsa.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/accent_color.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/auto_name.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/chat_action.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/chat_event_action.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/chat_member_status.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/chat_type.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/client_platform.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/message_entity_type.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/message_media_type.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/message_service_type.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/messages_filter.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/next_code_type.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/parse_mode.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/poll_type.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/profile_color.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/sent_code_type.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/enums/user_status.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/errors/__init__.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/errors/rpc_error.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/__init__.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/handler.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/message_handler.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/message_reaction_count_updated_handler.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/message_reaction_updated_handler.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/poll_handler.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/handlers/user_status_handler.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/__init__.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/advanced/save_file.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/__init__.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/check_password.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/connect.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/initialize.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/log_out.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/send_code.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/auth/terminate.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/__init__.py
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_bot_info_description.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_bot_info_short_description.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_bot_name.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/send_game.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/set_bot_info_description.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/set_bot_info_short_description.py
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/set_bot_name.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/bots/set_game_score.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/business/__init__.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/business/get_business_connection.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/business/get_collectible_item_info.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/__init__.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/close_forum_topic.py
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/create_forum_topic.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/delete_forum_topic.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/edit_forum_topic.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/get_forum_topic.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/get_forum_topics.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/hide_forum_topic.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/reopen_forum_topic.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/unhide_forum_topic.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/__init__.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/create_group.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_created_chats.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/search_chats.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_chat_ttl.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/chats/unpin_chat_message.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/contacts/import_contacts.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_message_reaction_count_updated.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_message_reaction_updated.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_user_status.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/revoke_chat_invite_link.py
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/__init__.py
--rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/download_media.py
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_cached_media.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0        0        0    14177 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_chat_sponsored_messages.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/search_global.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0        0        0    16243 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0        0        0    14185 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0        0        0     7024 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0        0        0     7017 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0        0        0    13679 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_document.py
--rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_location.py
--rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0        0        0    14869 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_message.py
--rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0        0        0    11549 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0        0        0    12230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0        0        0    15395 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_video.py
--rw-r--r--   0        0        0    13957 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0        0        0    13542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/set_reaction.py
--rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/view_messages.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/messages/vote_poll.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/password/__init__.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/password/remove_cloud_password.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/phone/__init__.py
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/phone/load_group_call_participants.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/stickers/get_stickers.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/__init__.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/block_user.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/get_me.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/get_users.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/set_birthdate.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/set_personal_chat.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/set_username.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/users/update_profile.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/utilities/compose.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/utilities/idle.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/utilities/restart.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/utilities/run.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/utilities/start.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/utilities/stop.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/parser/__init__.py
--rw-r--r--   0        0        0     9094 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/parser/html.py
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/parser/markdown.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/parser/parser.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/parser/utils.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/__init__.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/core/__init__.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/core/future_salt.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/core/future_salts.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/core/list.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/core/message.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/core/msg_container.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/core/tl_object.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/session/__init__.py
--rw-r--r--   0        0        0    11446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/session/auth.py
--rw-r--r--   0        0        0    14423 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/session/session.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/session/internals/__init__.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/session/internals/data_center.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/session/internals/msg_id.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/session/internals/seq_no.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/storage/__init__.py
--rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/storage/aio_sqlite_storage.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/storage/file_storage.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/storage/memory_storage.py
--rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/storage/storage.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/list.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/object.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/update.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/authorization/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/authorization/terms_of_service.py
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0        0        0    14613 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/web_app_info.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/business/__init__.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/business/business_connection.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/business/business_intro.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/business/business_location.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/business/business_opening_hours.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/business/business_opening_hours_interval.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/business/collectible_item_info.py
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/business/invoice.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/__init__.py
--rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/forum_topic.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/forum_topic_closed.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/forum_topic_created.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/forum_topic_edited.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/forum_topic_reopened.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/general_forum_topic_hidden.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/general_forum_topic_unhidden.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0        0        0     6093 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_voice.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_media/__init__.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_media/input_media.py
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_media/input_phone_contact.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_media/link_preview_options.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0        0        0    14382 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_message_content/external_reply_info.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_message_content/input_poll_option.py
--rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_message_content/reply_parameters.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/input_message_content/text_quote.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/message_origin/__init__.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/message_origin/message_import_info.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/message_origin/message_origin.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/message_origin/message_origin_channel.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/message_origin/message_origin_chat.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/message_origin/message_origin_hidden_user.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/message_origin/message_origin_user.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/chat_boost_added.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/gift_code.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/gifted_premium.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/giveaway.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/giveaway_completed.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/giveaway_winners.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0        0        0   198954 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/message_reaction_count_updated.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/message_reaction_updated.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0        0        0     9239 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/sponsored_message.py
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/story.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/birthdate.py
--rw-r--r--   0        0        0    47521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_color.py
--rw-r--r--   0        0        0    19921 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_shared.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/group_call_participant.py
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0        0        0    18749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/users_shared.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/video_chat_participants_invited.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/COPYING
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/COPYING.lesser
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/NOTICE
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/README.md
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/hatch_build.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/pyproject.toml
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.2/PKG-INFO
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/__init__.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/api/__init__.py
+-rw-r--r--   0        0        0    22468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/api/compiler.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/api/source/auth_key.tl
+-rw-r--r--   0        0        0   212645 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/api/source/main_api.tl
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/api/source/sys_msgs.tl
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/api/template/combinator.txt
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/api/template/type.txt
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/errors/__init__.py
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/errors/compiler.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/errors/sort.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0        0        0    34482 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/errors/template/class.txt
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/compiler/errors/template/sub_class.txt
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/__init__.py
+-rw-r--r--   0        0        0    47022 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/client.py
+-rw-r--r--   0        0        0    15902 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/dispatcher.py
+-rw-r--r--   0        0        0   208021 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/emoji.py
+-rw-r--r--   0        0        0    16314 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/file_id.py
+-rw-r--r--   0        0        0    28542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/filters.py
+-rw-r--r--   0        0        0    62000 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/mime_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/py.typed
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/sync.py
+-rw-r--r--   0        0        0    17557 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/utils.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/connection/__init__.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/connection/connection.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/connection/transport/__init__.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/crypto/__init__.py
+-rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/crypto/aes.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/crypto/mtproto.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/crypto/prime.py
+-rw-r--r--   0        0        0    13437 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/crypto/rsa.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/accent_color.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/auto_name.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/chat_action.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/chat_type.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/client_platform.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/message_media_type.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/message_service_type.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/messages_filter.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/next_code_type.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/parse_mode.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/poll_type.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/profile_color.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/enums/user_status.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/errors/__init__.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/errors/rpc_error.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/__init__.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/handler.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/message_handler.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/message_reaction_count_updated_handler.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/message_reaction_updated_handler.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/handlers/user_status_handler.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/__init__.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/advanced/save_file.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/connect.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/auth/terminate.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_bot_info_description.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_bot_info_short_description.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_bot_name.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/set_bot_info_description.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/set_bot_info_short_description.py
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/set_bot_name.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/bots/set_game_score.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/business/__init__.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/business/get_business_connection.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/business/get_collectible_item_info.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/__init__.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/close_forum_topic.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/create_forum_topic.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/delete_forum_topic.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/edit_forum_topic.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/get_forum_topic.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/get_forum_topics.py
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/hide_forum_topic.py
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/reopen_forum_topic.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/unhide_forum_topic.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_created_chats.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/search_chats.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_chat_ttl.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/chats/unpin_chat_message.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/contacts/import_contacts.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_message_reaction_count_updated.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_message_reaction_updated.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_user_status.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0        0        0     8309 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_cached_media.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0        0        0    14217 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_chat_sponsored_messages.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0        0        0    16591 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0        0        0    14288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0        0        0     7096 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0        0        0    13782 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0        0        0     6833 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0        0        0    14917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0        0        0    13135 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0        0        0    12333 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0        0        0     7615 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0        0        0    15743 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0        0        0    13645 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/set_reaction.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/view_messages.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/messages/vote_poll.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/password/__init__.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/password/remove_cloud_password.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/phone/__init__.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/phone/load_group_call_participants.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/stickers/get_message_effects.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/stickers/get_stickers.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/__init__.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/block_user.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/get_me.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/get_users.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/set_birthdate.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/set_personal_chat.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/set_username.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/users/update_profile.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/utilities/run.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/utilities/start.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/parser/__init__.py
+-rw-r--r--   0        0        0     9094 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/parser/html.py
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/parser/markdown.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/parser/parser.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/parser/utils.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/__init__.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/core/__init__.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/core/list.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/core/message.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/core/msg_container.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/core/tl_object.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/session/__init__.py
+-rw-r--r--   0        0        0    11446 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/session/auth.py
+-rw-r--r--   0        0        0    14936 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/session/session.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/session/internals/__init__.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/session/internals/data_center.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/storage/__init__.py
+-rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/storage/aio_sqlite_storage.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/storage/file_storage.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/storage/memory_storage.py
+-rw-r--r--   0        0        0    10521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/storage/storage.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/list.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/object.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/update.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/authorization/terms_of_service.py
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0        0        0    14613 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0        0        0    10597 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/web_app_info.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/business/__init__.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/business/business_connection.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/business/business_intro.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/business/business_location.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/business/business_opening_hours.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/business/business_opening_hours_interval.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/business/collectible_item_info.py
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/business/invoice.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/__init__.py
+-rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/forum_topic.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/forum_topic_closed.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/forum_topic_created.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/forum_topic_edited.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/forum_topic_reopened.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/general_forum_topic_hidden.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/general_forum_topic_unhidden.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0        0        0     6093 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0        0        0     5240 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_voice.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_media/input_phone_contact.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_media/link_preview_options.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0        0        0    14382 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_message_content/external_reply_info.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_message_content/input_poll_option.py
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_message_content/reply_parameters.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/input_message_content/text_quote.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/message_origin/__init__.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/message_origin/message_import_info.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/message_origin/message_origin.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/message_origin/message_origin_channel.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/message_origin/message_origin_chat.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/message_origin/message_origin_hidden_user.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/message_origin/message_origin_user.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/chat_boost_added.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/gift_code.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/gifted_premium.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/giveaway.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/giveaway_completed.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/giveaway_winners.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0        0        0   205279 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/message_effect.py
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/message_reaction_count_updated.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/message_reaction_updated.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0        0        0     9239 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/sponsored_message.py
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/story.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/birthdate.py
+-rw-r--r--   0        0        0    47521 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_color.py
+-rw-r--r--   0        0        0    20181 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0        0        0     7020 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_shared.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/group_call_participant.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0        0        0    18749 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/users_shared.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/video_chat_participants_invited.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/COPYING
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/COPYING.lesser
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/NOTICE
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/README.md
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/hatch_build.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/pyproject.toml
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 pyrotgfork-2.1.32.3/PKG-INFO
```

### Comparing `pyrotgfork-2.1.32.2/compiler/__init__.py` & `pyrotgfork-2.1.32.3/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/api/__init__.py` & `pyrotgfork-2.1.32.3/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/api/compiler.py` & `pyrotgfork-2.1.32.3/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/api/source/auth_key.tl` & `pyrotgfork-2.1.32.3/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/api/source/main_api.tl` & `pyrotgfork-2.1.32.3/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/api/source/sys_msgs.tl` & `pyrotgfork-2.1.32.3/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/api/template/combinator.txt` & `pyrotgfork-2.1.32.3/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/api/template/type.txt` & `pyrotgfork-2.1.32.3/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/errors/__init__.py` & `pyrotgfork-2.1.32.3/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/errors/compiler.py` & `pyrotgfork-2.1.32.3/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/errors/sort.py` & `pyrotgfork-2.1.32.3/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/errors/source/400_BAD_REQUEST.tsv` & `pyrotgfork-2.1.32.3/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/errors/source/401_UNAUTHORIZED.tsv` & `pyrotgfork-2.1.32.3/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/errors/source/403_FORBIDDEN.tsv` & `pyrotgfork-2.1.32.3/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `pyrotgfork-2.1.32.3/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/errors/source/420_FLOOD.tsv` & `pyrotgfork-2.1.32.3/compiler/errors/source/420_FLOOD.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `pyrotgfork-2.1.32.3/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 __fork_name__ = "pyrotgfork"
-__version__ = "2.1.32.2"
+__version__ = "2.1.32.3"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/client.py` & `pyrotgfork-2.1.32.3/pyrogram/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,18 @@
         client_platform (:obj:`~pyrogram.enums.ClientPlatform`, *optional*):
             The platform where this client is running.
             Defaults to 'other'
         
         link_preview_options (:obj:`~pyrogram.types.LinkPreviewOptions`, *optional*):
             Set the global link preview options for the client. By default, no link preview option is set.
 
+        fetch_replies (``int``, *optional*):
+            Set the number of replies to be fetched when parsing the :obj:`~pyrogram.types.Message` object. Defaults to 1.
+            :doc:`More on Errors <../../api/errors/index>`
+
     """
 
     APP_VERSION = f"Pyrogram {__version__}"
     DEVICE_MODEL = f"{platform.python_implementation()} {platform.python_version()}"
     SYSTEM_VERSION = f"{platform.system()} {platform.release()}"
 
     LANG_PACK = ""
@@ -273,14 +277,15 @@
         max_concurrent_transmissions: int = MAX_CONCURRENT_TRANSMISSIONS,
         max_message_cache_size: int = MAX_CACHE_SIZE,
         max_business_user_connection_cache_size: int = MAX_CACHE_SIZE,
         storage_engine: Storage = None,
         no_joined_notifications: bool = False,
         client_platform: enums.ClientPlatform = enums.ClientPlatform.OTHER,
         link_preview_options: "types.LinkPreviewOptions" = None,
+        fetch_replies: int = 1,
         _un_docu_gnihts: List = []
     ):
         super().__init__()
 
         self.name = name
         self.api_id = int(api_id) if api_id else None
         self.api_hash = api_hash
@@ -311,14 +316,15 @@
         self.max_concurrent_transmissions = max_concurrent_transmissions
         self.max_message_cache_size = max_message_cache_size
         self.max_business_user_connection_cache_size = max_business_user_connection_cache_size
         self.no_joined_notifications = no_joined_notifications
         self.client_platform = client_platform
         self._un_docu_gnihts = _un_docu_gnihts
         self.link_preview_options = link_preview_options
+        self.fetch_replies = fetch_replies
 
         self.executor = ThreadPoolExecutor(self.workers, thread_name_prefix="Handler")
 
         if self.session_string:
             self.storage = MemoryStorage(self.name, self.session_string)
         elif self.in_memory:
             self.storage = MemoryStorage(self.name)
@@ -619,15 +625,15 @@
                         ), "peer_id", None
                     ), "channel_id", None
                 ) or getattr(update, "channel_id", None)
 
                 pts = getattr(update, "pts", None)
                 pts_count = getattr(update, "pts_count", None)
 
-                if pts:
+                if pts and not self.skip_updates:
                     await self.storage.update_state(
                         (
                             utils.get_channel_id(channel_id) if channel_id else 0,
                             pts,
                             None,
                             updates.date,
                             updates.seq
@@ -660,23 +666,24 @@
                         else:
                             if not isinstance(diff, raw.types.updates.ChannelDifferenceEmpty):
                                 users.update({u.id: u for u in diff.users})
                                 chats.update({c.id: c for c in diff.chats})
 
                 self.dispatcher.updates_queue.put_nowait((update, users, chats))
         elif isinstance(updates, (raw.types.UpdateShortMessage, raw.types.UpdateShortChatMessage)):
-            await self.storage.update_state(
-                (
-                    0,
-                    updates.pts,
-                    None,
-                    updates.date,
-                    None
+            if not self.skip_updates:
+                await self.storage.update_state(
+                    (
+                        0,
+                        updates.pts,
+                        None,
+                        updates.date,
+                        None
+                    )
                 )
-            )
 
             diff = await self.invoke(
                 raw.functions.updates.GetDifference(
                     pts=updates.pts - updates.pts_count,
                     date=updates.date,
                     qts=-1
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/dispatcher.py` & `pyrotgfork-2.1.32.3/pyrogram/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,23 +84,25 @@
         self.handler_worker_tasks = []
         self.locks_list = []
 
         self.updates_queue = asyncio.Queue()
         self.groups = OrderedDict()
 
         async def message_parser(update, users, chats):
+            business_connection_id = getattr(update, "connection_id", None)
             return (
                 await pyrogram.types.Message._parse(
                     self.client,
                     update.message,
                     users,
                     chats,
                     is_scheduled=isinstance(update, UpdateNewScheduledMessage),
-                    business_connection_id=getattr(update, "connection_id", None),
-                    raw_reply_to_message=getattr(update, "reply_to_message", None)
+                    business_connection_id=business_connection_id,
+                    raw_reply_to_message=getattr(update, "reply_to_message", None),
+                    replies=0 if business_connection_id else self.client.fetch_replies
                 ),
                 MessageHandler
             )
 
         async def edited_message_parser(update, users, chats):
             # Edited messages are parsed the same way as new messages, but the handler is different
             parsed, _ = await message_parser(update, users, chats)
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/emoji.py` & `pyrotgfork-2.1.32.3/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/file_id.py` & `pyrotgfork-2.1.32.3/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/filters.py` & `pyrotgfork-2.1.32.3/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/mime_types.py` & `pyrotgfork-2.1.32.3/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/sync.py` & `pyrotgfork-2.1.32.3/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/utils.py` & `pyrotgfork-2.1.32.3/pyrogram/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                 parsed_messages.append(
                     await types.Message._parse(
                         client,
                         u.message,
                         users,
                         chats,
                         is_scheduled=isinstance(u, raw.types.UpdateNewScheduledMessage),
-                        replies=0
+                        replies=client.fetch_replies
                     )
                 )
 
             elif isinstance(
                 u,
                 (
                     raw.types.UpdateBotNewBusinessMessage,
@@ -131,15 +131,16 @@
                 parsed_messages.append(
                     await types.Message._parse(
                         client,
                         u.message,
                         users,
                         chats,
                         business_connection_id=getattr(u, "connection_id", business_connection_id),
-                        raw_reply_to_message=u.reply_to_message
+                        raw_reply_to_message=u.reply_to_message,
+                        replies=0
                     )
                 )
 
         return types.List(parsed_messages)
 
     users = {i.id: i for i in messages.users}
     chats = {i.id: i for i in messages.chats}
@@ -151,15 +152,15 @@
         parsed_messages.append(
             await types.Message._parse(
                 client,
                 message,
                 users,
                 chats,
                 is_scheduled=is_scheduled,
-                replies=replies
+                replies=client.fetch_replies
             )
         )
 
     if replies and False:  # TODO
         messages_with_replies = {
             # TODO: fix this logic someday
             i.id: i.reply_to.reply_to_msg_id
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/connection/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/connection/connection.py` & `pyrotgfork-2.1.32.3/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/connection/transport/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/connection/transport/tcp/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/connection/transport/tcp/tcp.py` & `pyrotgfork-2.1.32.3/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/connection/transport/tcp/tcp_abridged.py` & `pyrotgfork-2.1.32.3/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `pyrotgfork-2.1.32.3/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/connection/transport/tcp/tcp_full.py` & `pyrotgfork-2.1.32.3/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `pyrotgfork-2.1.32.3/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `pyrotgfork-2.1.32.3/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/crypto/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/crypto/aes.py` & `pyrotgfork-2.1.32.3/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/crypto/mtproto.py` & `pyrotgfork-2.1.32.3/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/crypto/prime.py` & `pyrotgfork-2.1.32.3/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/crypto/rsa.py` & `pyrotgfork-2.1.32.3/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/accent_color.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/accent_color.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/auto_name.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/chat_action.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/chat_event_action.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/chat_member_status.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/chat_members_filter.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/chat_type.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/client_platform.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/client_platform.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/message_entity_type.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/message_media_type.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/message_service_type.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/messages_filter.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/next_code_type.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/parse_mode.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/poll_type.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/profile_color.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/profile_color.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/sent_code_type.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/enums/user_status.py` & `pyrotgfork-2.1.32.3/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/errors/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/errors/rpc_error.py` & `pyrotgfork-2.1.32.3/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/callback_query_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/chat_join_request_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/chat_member_updated_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/chosen_inline_result_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/deleted_messages_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/disconnect_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/edited_message_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/handler.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/inline_query_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/message_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/message_reaction_count_updated_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/message_reaction_count_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/message_reaction_updated_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/message_reaction_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/poll_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/raw_update_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/handlers/user_status_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/advanced/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/advanced/invoke.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/advanced/resolve_peer.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/advanced/save_file.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/accept_terms_of_service.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/check_password.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/connect.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/disconnect.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/get_password_hint.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/initialize.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/log_out.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/recover_password.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/resend_code.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/send_code.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/send_recovery_code.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/sign_in.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/sign_in_bot.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/sign_up.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/auth/terminate.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/answer_callback_query.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/answer_inline_query.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/answer_web_app_query.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/delete_bot_commands.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_bot_commands.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_bot_default_privileges.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_bot_info_description.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_bot_info_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_bot_info_short_description.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_bot_info_short_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_bot_name.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_bot_name.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_chat_menu_button.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_game_high_scores.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/get_inline_bot_results.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/request_callback_answer.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/send_game.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/send_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,23 +131,25 @@
             r = await self.invoke(rpc)
 
         for i in r.updates:
             if isinstance(i, (raw.types.UpdateNewMessage, raw.types.UpdateNewChannelMessage)):
                 return await types.Message._parse(
                     self, i.message,
                     {i.id: i for i in r.users},
-                    {i.id: i for i in r.chats}
+                    {i.id: i for i in r.chats},
+                    replies=self.fetch_replies
                 )
             elif isinstance(
                 i,
                 (
                     raw.types.UpdateBotNewBusinessMessage
                 )
             ):
                 return await types.Message._parse(
                     self,
                     i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     business_connection_id=i.connection_id,
-                    raw_reply_to_message=i.reply_to_message
+                    raw_reply_to_message=i.reply_to_message,
+                    replies=0
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/send_inline_bot_result.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/set_bot_commands.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/set_bot_default_privileges.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/set_bot_info_description.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/set_bot_info_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/set_bot_info_short_description.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/set_bot_info_short_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/set_bot_name.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/set_bot_name.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/set_chat_menu_button.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/bots/set_game_score.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/bots/set_game_score.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,11 +90,12 @@
 
         for i in r.updates:
             if isinstance(i, (raw.types.UpdateEditMessage,
                               raw.types.UpdateEditChannelMessage)):
                 return await types.Message._parse(
                     self, i.message,
                     {i.id: i for i in r.users},
-                    {i.id: i for i in r.chats}
+                    {i.id: i for i in r.chats},
+                    replies=self.fetch_replies
                 )
 
         return True
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/business/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/business/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/business/get_business_connection.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/business/get_business_connection.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/business/get_collectible_item_info.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/business/get_collectible_item_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/close_forum_topic.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/close_forum_topic.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,9 +76,9 @@
             ):
                 return await types.Message._parse(
                     self,
                     i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
-                    replies=2
+                    replies=self.fetch_replies
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/create_forum_topic.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/create_forum_topic.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,9 +90,9 @@
             ):
                 return await types.Message._parse(
                     self,
                     i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
-                    replies=2
+                    replies=self.fetch_replies
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/delete_forum_topic.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/edit_forum_topic.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/edit_forum_topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,9 +86,9 @@
             ):
                 return await types.Message._parse(
                     self,
                     i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
-                    replies=2
+                    replies=self.fetch_replies
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/get_forum_topic.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/get_forum_topic.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,19 @@
 
         users = {i.id: i for i in r.users}
         chats = {i.id: i for i in r.chats}
 
         messages = {}
         for message in getattr(r, "messages", []):
             messages[message.id] = await types.Message._parse(
-                self, message, users, chats, replies=0
+                self,
+                message,
+                users,
+                chats,
+                replies=self.fetch_replies
             )
 
         topics = types.List()
         for i in getattr(r, "topics"):
             topics.append(
                 types.ForumTopic._parse(
                     self, i, messages, users, chats
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/get_forum_topic_icon_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/get_forum_topics.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/get_forum_topics.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,19 @@
 
             users = {i.id: i for i in r.users}
             chats = {i.id: i for i in r.chats}
             messages = {}
 
             for message in getattr(r, "messages", []):
                 messages[message.id] = await types.Message._parse(
-                    self, message, users, chats, replies=0
+                    self,
+                    message,
+                    users,
+                    chats,
+                    replies=self.fetch_replies
                 )
 
             topics = []
 
             for topic in getattr(r, "topics", []):
                 topics.append(
                     types.ForumTopic._parse(
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/hide_forum_topic.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/hide_forum_topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,9 +74,9 @@
             ):
                 return await types.Message._parse(
                     self,
                     i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
-                    replies=2
+                    replies=self.fetch_replies
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/reopen_forum_topic.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/reopen_forum_topic.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,9 +78,9 @@
             ):
                 return await types.Message._parse(
                     self,
                     i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
-                    replies=2
+                    replies=self.fetch_replies
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chat_topics/unhide_forum_topic.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chat_topics/unhide_forum_topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,9 +74,9 @@
             ):
                 return await types.Message._parse(
                     self,
                     i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
-                    replies=2
+                    replies=self.fetch_replies
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/add_chat_members.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/add_chat_members.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,17 +102,19 @@
                     (
                         raw.types.UpdateNewMessage,
                         raw.types.UpdateNewChannelMessage
                     )
                 ):
                     _rc.append(
                         await types.Message._parse(
-                            self, i.message,
+                            self,
+                            i.message,
                             {i.id: i for i in rr.updates.users},
                             {i.id: i for i in rr.updates.chats},
+                            replies=self.fetch_replies
                         )
                     )
                     break
 
         if len(_rc) > 0:
             if len(_rc) == 1:
                 return _rc[0]
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/archive_chats.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/ban_chat_member.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/ban_chat_member.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,13 +105,15 @@
                     revoke_history=revoke_messages
                 )
             )
 
         for i in r.updates:
             if isinstance(i, (raw.types.UpdateNewMessage, raw.types.UpdateNewChannelMessage)):
                 return await types.Message._parse(
-                    self, i.message,
+                    self,
+                    i.message,
                     {i.id: i for i in r.users},
-                    {i.id: i for i in r.chats}
+                    {i.id: i for i in r.chats},
+                    replies=self.fetch_replies
                 )
         else:
             return True
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/create_channel.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/create_group.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/create_supergroup.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/delete_channel.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/delete_chat_photo.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/delete_supergroup.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/delete_user_history.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_chat.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_chat_event_log.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_chat_member.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_chat_members.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_chat_members_count.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_chat_online_count.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_created_chats.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_created_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_dialogs.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_dialogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,21 @@
             messages = {}
 
             for message in r.messages:
                 if isinstance(message, raw.types.MessageEmpty):
                     continue
 
                 chat_id = utils.get_peer_id(message.peer_id)
-                messages[chat_id] = await types.Message._parse(self, message, users, chats)
+                messages[chat_id] = await types.Message._parse(
+                    self,
+                    message,
+                    users,
+                    chats,
+                    replies=self.fetch_replies
+                )
 
             dialogs = []
 
             for dialog in r.dialogs:
                 if not isinstance(dialog, raw.types.Dialog):
                     continue
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_dialogs_count.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_nearby_chats.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/get_send_as_chats.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/join_chat.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/leave_chat.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/mark_chat_unread.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/pin_chat_message.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/pin_chat_message.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,8 +74,14 @@
 
         users = {u.id: u for u in r.users}
         chats = {c.id: c for c in r.chats}
 
         for i in r.updates:
             if isinstance(i, (raw.types.UpdateNewMessage,
                               raw.types.UpdateNewChannelMessage)):
-                return await types.Message._parse(self, i.message, users, chats)
+                return await types.Message._parse(
+                    self,
+                    i.message,
+                    users,
+                    chats,
+                    replies=self.fetch_replies
+                )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/promote_chat_member.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/promote_chat_member.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,11 +94,12 @@
                     raw.types.UpdateNewMessage,
                     raw.types.UpdateNewChannelMessage
                 )
             ):
                 return await types.Message._parse(
                     self, i.message,
                     {i.id: i for i in r.users},
-                    {i.id: i for i in r.chats}
+                    {i.id: i for i in r.chats},
+                    replies=self.fetch_replies
                 )
         else:
             return True
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/restrict_chat_member.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/search_chats.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/search_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_administrator_title.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_chat_description.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_chat_permissions.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_chat_photo.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_chat_protected_content.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_chat_title.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_chat_ttl.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_chat_ttl.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,8 +65,9 @@
             if isinstance(i, (raw.types.UpdateNewMessage,
                               raw.types.UpdateNewChannelMessage)):
                 return await types.Message._parse(
                     self,
                     i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
+                    replies=self.fetch_replies
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_chat_username.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_send_as_chat.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/set_slow_mode.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/unarchive_chats.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/unban_chat_member.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/unpin_all_chat_messages.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/chats/unpin_chat_message.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/contacts/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/contacts/add_contact.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/contacts/delete_contacts.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/contacts/get_contacts.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/contacts/get_contacts_count.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/contacts/import_contacts.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/decorators/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_callback_query.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_chat_join_request.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_chat_member_updated.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_chosen_inline_result.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_deleted_messages.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_disconnect.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_edited_message.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_inline_query.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_message.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_message_reaction_count_updated.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_message_reaction_updated.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_poll.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_raw_update.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/decorators/on_user_status.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/approve_chat_join_request.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/create_chat_invite_link.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/decline_chat_join_request.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/export_chat_invite_link.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/get_chat_invite_link.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/get_chat_join_requests.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/copy_media_group.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/copy_message.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/copy_message.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         self: "pyrogram.Client",
         chat_id: Union[int, str],
         from_chat_id: Union[int, str],
         message_id: int,
         caption: str = None,
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
+        show_caption_above_media: bool = None,
         disable_notification: bool = None,
         reply_parameters: "types.ReplyParameters" = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
             "types.ReplyKeyboardRemove",
             "types.ForceReply"
@@ -78,14 +79,17 @@
             parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
                 By default, texts are parsed using both Markdown and HTML styles.
                 You can combine both syntaxes together.
 
             caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
                 List of special entities that appear in the new caption, which can be specified instead of *parse_mode*.
 
+            show_caption_above_media (``bool``, *optional*):
+                Pass True, if the caption must be shown above the message media. Ignored if a new caption isn't specified.
+
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
@@ -135,14 +139,15 @@
         )
 
         return await message.copy(
             chat_id=chat_id,
             caption=caption,
             parse_mode=parse_mode,
             caption_entities=caption_entities,
+            show_caption_above_media=show_caption_above_media,
             disable_notification=disable_notification,
             reply_parameters=reply_parameters,
             reply_markup=reply_markup,
             schedule_date=schedule_date,
             business_connection_id=business_connection_id,
             protect_content=protect_content,
             message_thread_id=message_thread_id
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/delete_messages.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/download_media.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_cached_media.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_cached_media.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         self: "pyrogram.Client",
         chat_id: Union[int, str],
         message_id: int,
         file_id: str,
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
+        show_caption_above_media: bool = None,
         schedule_date: datetime = None,
         has_spoiler: bool = None,
         reply_markup: "types.InlineKeyboardMarkup" = None
     ) -> Optional["types.Message"]:
         """Edit a media stored on the Telegram servers using a file_id.
 
         This convenience method works with any valid file_id only.
@@ -66,14 +67,17 @@
             parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
                 By default, texts are parsed using both Markdown and HTML styles.
                 You can combine both syntaxes together.
 
             caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
                 List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
+            show_caption_above_media (``bool``, *optional*):
+                Pass True, if the caption must be shown above the message media. Supported only for animation, photo and video messages.
+
             schedule_date (:py:obj:`~datetime.datetime`, *optional*):
                 Date when the message will be automatically sent.
 
             has_spoiler (``bool``, *optional*):
                 True, if the message media is covered by a spoiler animation.
 
             reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
@@ -90,14 +94,15 @@
 
         rpc = raw.functions.messages.EditMessage(
             peer=await self.resolve_peer(chat_id),
             id=message_id,
             media=utils.get_input_media_from_file_id(file_id, has_spoiler=has_spoiler),
             reply_markup=await reply_markup.write(self) if reply_markup else None,
             schedule_date=utils.datetime_to_timestamp(schedule_date),
+            invert_media=show_caption_above_media,
             **await utils.parse_text_entities(self, caption, parse_mode, caption_entities)
         )
         r = await self.invoke(rpc)
 
         for i in r.updates:
             if isinstance(
                 i,
@@ -108,9 +113,9 @@
                 )
             ):
                 return await types.Message._parse(
                     self, i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
-                    replies=0
+                    replies=self.fetch_replies
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_inline_caption.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_inline_media.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_inline_reply_markup.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_inline_text.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_message_caption.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_message_caption.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     async def edit_message_caption(
         self: "pyrogram.Client",
         chat_id: Union[int, str],
         message_id: int,
         caption: str,
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
+        show_caption_above_media: bool = None,
         reply_markup: "types.InlineKeyboardMarkup" = None,
         schedule_date: datetime = None
     ) -> "types.Message":
         """Edit the caption of media messages.
 
         .. include:: /_includes/usable-by/users-bots.rst
 
@@ -53,30 +54,40 @@
             parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
                 By default, texts are parsed using both Markdown and HTML styles.
                 You can combine both syntaxes together.
 
             caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
                 List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
+            show_caption_above_media (``bool``, *optional*):
+                Pass True, if the caption must be shown above the message media. Supported only for animation, photo and video messages.
+
             reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
                 An InlineKeyboardMarkup object.
 
             schedule_date (:py:obj:`~datetime.datetime`, *optional*):
                 Date when the message will be automatically sent.
 
         Returns:
             :obj:`~pyrogram.types.Message`: On success, the edited message is returned.
 
         Example:
             .. code-block:: python
 
                 await app.edit_message_caption(chat_id, message_id, "new media caption")
         """
+        link_preview_options = None
+        if show_caption_above_media:
+            link_preview_options = types.LinkPreviewOptions(
+                show_above_text=show_caption_above_media
+            )
+
         return await self.edit_message_text(
             chat_id=chat_id,
             message_id=message_id,
             text=caption,
             parse_mode=parse_mode,
             entities=caption_entities,
             reply_markup=reply_markup,
+            link_preview_options=link_preview_options,
             schedule_date=schedule_date
         )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_message_media.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_message_media.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,14 +283,15 @@
             raw.functions.messages.EditMessage(
                 peer=await self.resolve_peer(chat_id),
                 id=message_id,
                 media=media,
                 reply_markup=await reply_markup.write(self) if reply_markup else None,
                 message=message,
                 entities=entities,
+                # TODO
                 schedule_date=utils.datetime_to_timestamp(schedule_date)
             )
         )
 
         for i in r.updates:
             if isinstance(
                 i,
@@ -301,9 +302,9 @@
                 )
             ):
                 return await types.Message._parse(
                     self, i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
-                    replies=0
+                    replies=self.fetch_replies
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_message_reply_markup.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,9 +69,10 @@
         )
 
         for i in r.updates:
             if isinstance(i, (raw.types.UpdateEditMessage, raw.types.UpdateEditChannelMessage)):
                 return await types.Message._parse(
                     self, i.message,
                     {i.id: i for i in r.users},
-                    {i.id: i for i in r.chats}
+                    {i.id: i for i in r.chats},
+                    replies=self.fetch_replies
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/edit_message_text.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/edit_message_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,9 +138,9 @@
                 )
             ):
                 return await types.Message._parse(
                     self, i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
-                    replies=0
+                    replies=self.fetch_replies
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/forward_messages.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/forward_messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,12 +124,13 @@
             ):
                 forwarded_messages.append(
                     await types.Message._parse(
                         self,
                         i.message,
                         users,
                         chats,
-                        is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage)
+                        is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
+                        replies=self.fetch_replies
                     )
                 )
 
         return types.List(forwarded_messages) if is_iterable else forwarded_messages[0]
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_chat_history.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_chat_history_count.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_chat_sponsored_messages.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_chat_sponsored_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from typing import List
 
 import pyrogram
-from pyrogram import raw
-from pyrogram import types
+from pyrogram import raw, types
 
 
 class GetCustomEmojiStickers:
     async def get_custom_emoji_stickers(
         self: "pyrogram.Client",
         custom_emoji_ids: List[int],
     ) -> List["types.Sticker"]:
@@ -48,8 +47,8 @@
 
         stickers = []
         for item in result:
             attributes = {type(i): i for i in item.attributes}
             sticker = await types.Sticker._parse(self, item, attributes)
             stickers.append(sticker)
 
-        return pyrogram.types.List(stickers)
+        return types.List(stickers)
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_discussion_message.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_discussion_message.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,8 +58,14 @@
                 msg_id=message_id
             )
         )
 
         users = {u.id: u for u in r.users}
         chats = {c.id: c for c in r.chats}
 
-        return await types.Message._parse(self, r.messages[0], users, chats)
+        return await types.Message._parse(
+            self,
+            r.messages[0],
+            users,
+            chats,
+            replies=self.fetch_replies
+        )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_discussion_replies.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,13 +74,19 @@
             chats = {c.id: c for c in r.chats}
             messages = r.messages
 
             if not messages:
                 return
 
             for message in messages:
-                yield await types.Message._parse(self, message, users, chats, replies=0)
+                yield await types.Message._parse(
+                    self,
+                    message,
+                    users,
+                    chats,
+                    replies=self.fetch_replies
+                )
 
                 current += 1
 
                 if current >= total:
                     return
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_discussion_replies_count.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_media_group.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/get_messages.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/inline_session.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/read_chat_history.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/retract_vote.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/search_global.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/search_global_count.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/search_messages.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/search_messages_count.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_animation.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_animation.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     async def send_animation(
         self: "pyrogram.Client",
         chat_id: Union[int, str],
         animation: Union[str, BinaryIO],
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
+        show_caption_above_media: bool = None,
         unsave: bool = False,
         has_spoiler: bool = None,
         duration: int = 0,
         width: int = 0,
         height: int = 0,
         thumb: Union[str, BinaryIO] = None,
         file_name: str = None,
@@ -87,14 +88,17 @@
             parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
                 By default, texts are parsed using both Markdown and HTML styles.
                 You can combine both syntaxes together.
 
             caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
                 List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
+            show_caption_above_media (``bool``, *optional*):
+                Pass True, if the caption must be shown above the message media.
+
             unsave (``bool``, *optional*):
                 By default, the server will save into your own collection any new animation you send.
                 Pass True to automatically unsave the sent animation. Defaults to False.
 
             has_spoiler (``bool``, *optional*):
                 Pass True if the animation needs to be covered with a spoiler animation.
 
@@ -279,14 +283,15 @@
                 silent=disable_notification or None,
                 reply_to=reply_to,
                 random_id=self.rnd_id(),
                 schedule_date=utils.datetime_to_timestamp(schedule_date),
                 noforwards=protect_content,
                 reply_markup=await reply_markup.write(self) if reply_markup else None,
                 effect=message_effect_id,
+                invert_media=show_caption_above_media,
                 **await utils.parse_text_entities(self, caption, parse_mode, caption_entities)
             )
             session = None
             business_connection = None
             if business_connection_id:
                 business_connection = self.business_user_connection_cache[business_connection_id]
                 if not business_connection:
@@ -321,15 +326,16 @@
                             )
                         ):
                             message = await types.Message._parse(
                                 self,
                                 i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
-                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage)
+                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
+                                replies=self.fetch_replies
                             )
 
                             if unsave:
                                 document = message.animation or message.document
                                 document_id = utils.get_input_media_from_file_id(
                                     document.file_id, FileType.ANIMATION
                                 ).id
@@ -350,13 +356,14 @@
                         ):
                             return await types.Message._parse(
                                 self,
                                 i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
                                 business_connection_id=getattr(i, "connection_id", business_connection_id),
-                                raw_reply_to_message=i.reply_to_message
+                                raw_reply_to_message=i.reply_to_message,
+                                replies=0
                             )
 
 
         except StopTransmission:
             return None
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_audio.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_audio.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,25 +292,27 @@
                                 raw.types.UpdateNewScheduledMessage
                             )
                         ):
                             return await types.Message._parse(
                                 self, i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
-                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage)
+                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
+                                replies=self.fetch_replies
                             )
                         elif isinstance(
                             i,
                             (
                                 raw.types.UpdateBotNewBusinessMessage
                             )
                         ):
                             return await types.Message._parse(
                                 self,
                                 i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
                                 business_connection_id=getattr(i, "connection_id", business_connection_id),
-                                raw_reply_to_message=i.reply_to_message
+                                raw_reply_to_message=i.reply_to_message,
+                                replies=0
                             )
         except StopTransmission:
             return None
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_cached_media.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_cached_media.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,17 @@
     async def send_cached_media(
         self: "pyrogram.Client",
         chat_id: Union[int, str],
         file_id: str,
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
+        show_caption_above_media: bool = None,
         disable_notification: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         message_thread_id: int = None,
         business_connection_id: str = None,
         schedule_date: datetime = None,
         protect_content: bool = None,
         has_spoiler: bool = None,
         reply_markup: Union[
@@ -73,18 +75,24 @@
             parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
                 By default, texts are parsed using both Markdown and HTML styles.
                 You can combine both syntaxes together.
 
             caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
                 List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
+            show_caption_above_media (``bool``, *optional*):
+                Pass True, if the caption must be shown above the message media. Supported only for animation, photo and video messages.
+
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             message_thread_id (``int``, *optional*):
                 If the message is in a thread, ID of the original message.
 
             business_connection_id (``str``, *optional*):
@@ -135,14 +143,16 @@
             media=utils.get_input_media_from_file_id(file_id, has_spoiler=has_spoiler),
             silent=disable_notification or None,
             reply_to=reply_to,
             random_id=self.rnd_id(),
             schedule_date=utils.datetime_to_timestamp(schedule_date),
             noforwards=protect_content,
             reply_markup=await reply_markup.write(self) if reply_markup else None,
+            effect=message_effect_id,
+            invert_media=show_caption_above_media,
             **await utils.parse_text_entities(self, caption, parse_mode, caption_entities)
         )
 
         if business_connection_id:
             r = await self.invoke(
                 raw.functions.InvokeWithBusinessConnection(
                     query=rpc,
@@ -161,15 +171,16 @@
                     raw.types.UpdateNewScheduledMessage
                 )
             ):
                 return await types.Message._parse(
                     self, i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
-                    is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage)
+                    is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
+                    replies=self.fetch_replies
                 )
             elif isinstance(
                 i,
                 (
                     raw.types.UpdateBotNewBusinessMessage,
                     # raw.types.UpdateBotEditBusinessMessage,
                     # raw.types.UpdateBotDeleteBusinessMessage
@@ -177,9 +188,10 @@
             ):
                 return await types.Message._parse(
                     self,
                     i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     business_connection_id=getattr(i, "connection_id", business_connection_id),
-                    raw_reply_to_message=i.reply_to_message
+                    raw_reply_to_message=i.reply_to_message,
+                    replies=0
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_chat_action.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_contact.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_contact.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,23 +160,25 @@
                     raw.types.UpdateNewScheduledMessage
                 )
             ):
                 return await types.Message._parse(
                     self, i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
-                    is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage)
+                    is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
+                    replies=self.fetch_replies
                 )
             elif isinstance(
                 i,
                 (
                     raw.types.UpdateBotNewBusinessMessage
                 )
             ):
                 return await types.Message._parse(
                     self,
                     i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     business_connection_id=getattr(i, "connection_id", business_connection_id),
-                    raw_reply_to_message=i.reply_to_message
+                    raw_reply_to_message=i.reply_to_message,
+                    replies=0
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_dice.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_dice.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,23 +154,25 @@
                     raw.types.UpdateNewScheduledMessage
                 )
             ):
                 return await types.Message._parse(
                     self, i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
-                    is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage)
+                    is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
+                    replies=self.fetch_replies
                 )
             elif isinstance(
                 i,
                 (
                     raw.types.UpdateBotNewBusinessMessage
                 )
             ):
                 return await types.Message._parse(
                     self,
                     i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     business_connection_id=getattr(i, "connection_id", business_connection_id),
-                    raw_reply_to_message=i.reply_to_message
+                    raw_reply_to_message=i.reply_to_message,
+                    replies=0
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_document.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,26 +270,28 @@
                                 raw.types.UpdateNewScheduledMessage
                             )
                         ):
                             return await types.Message._parse(
                                 self, i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
-                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage)
+                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
+                                replies=self.fetch_replies
                             )
                         elif isinstance(
                             i,
                             (
                                 raw.types.UpdateBotNewBusinessMessage
                             )
                         ):
                             return await types.Message._parse(
                                 self,
                                 i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
                                 business_connection_id=getattr(i, "connection_id", business_connection_id),
-                                raw_reply_to_message=i.reply_to_message
+                                raw_reply_to_message=i.reply_to_message,
+                                replies=0
                             )
 
         except StopTransmission:
             return None
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_location.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_location.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,23 +153,25 @@
                     raw.types.UpdateNewScheduledMessage
                 )
             ):
                 return await types.Message._parse(
                     self, i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
-                    is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage)
+                    is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
+                    replies=self.fetch_replies
                 )
             elif isinstance(
                 i,
                 (
                     raw.types.UpdateBotNewBusinessMessage
                 )
             ):
                 return await types.Message._parse(
                     self,
                     i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     business_connection_id=getattr(i, "connection_id", business_connection_id),
-                    raw_reply_to_message=i.reply_to_message
+                    raw_reply_to_message=i.reply_to_message,
+                    replies=0
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_media_group.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_message.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,23 +339,24 @@
                 )
             ):
                 return await types.Message._parse(
                     self, i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
-                    replies=0
+                    replies=self.fetch_replies
                 )
             elif isinstance(
                 i,
                 (
                     raw.types.UpdateBotNewBusinessMessage
                 )
             ):
                 return await types.Message._parse(
                     self,
                     i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     business_connection_id=getattr(i, "connection_id", business_connection_id),
-                    raw_reply_to_message=i.reply_to_message
+                    raw_reply_to_message=i.reply_to_message,
+                    replies=0
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_photo.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_photo.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     async def send_photo(
         self: "pyrogram.Client",
         chat_id: Union[int, str],
         photo: Union[str, BinaryIO],
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
+        show_caption_above_media: bool = None,
         has_spoiler: bool = None,
         ttl_seconds: int = None,
         disable_notification: bool = None,
         reply_parameters: "types.ReplyParameters" = None,
         message_thread_id: int = None,
         business_connection_id: str = None,
         schedule_date: datetime = None,
@@ -82,14 +83,17 @@
             parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
                 By default, texts are parsed using both Markdown and HTML styles.
                 You can combine both syntaxes together.
 
             caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
                 List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
+            show_caption_above_media (``bool``, *optional*):
+                Pass True, if the caption must be shown above the message media.
+
             has_spoiler (``bool``, *optional*):
                 Pass True if the photo needs to be covered with a spoiler animation.
 
             ttl_seconds (``int``, *optional*):
                 Self-Destruct Timer.
                 If you set a timer, the photo will self-destruct in *ttl_seconds*
                 seconds after it was viewed.
@@ -222,14 +226,15 @@
                 silent=disable_notification or None,
                 reply_to=reply_to,
                 random_id=self.rnd_id(),
                 schedule_date=utils.datetime_to_timestamp(schedule_date),
                 noforwards=protect_content,
                 reply_markup=await reply_markup.write(self) if reply_markup else None,
                 effect=message_effect_id,
+                invert_media=show_caption_above_media,
                 **await utils.parse_text_entities(self, caption, parse_mode, caption_entities)
             )
             session = None
             business_connection = None
             if business_connection_id:
                 business_connection = self.business_user_connection_cache[business_connection_id]
                 if not business_connection:
@@ -263,25 +268,27 @@
                                 raw.types.UpdateNewScheduledMessage
                             )
                         ):
                             return await types.Message._parse(
                                 self, i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
-                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage)
+                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
+                                replies=self.fetch_replies
                             )
                         elif isinstance(
                             i,
                             (
                                 raw.types.UpdateBotNewBusinessMessage
                             )
                         ):
                             return await types.Message._parse(
                                 self,
                                 i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
                                 business_connection_id=getattr(i, "connection_id", business_connection_id),
-                                raw_reply_to_message=i.reply_to_message
+                                raw_reply_to_message=i.reply_to_message,
+                                replies=0
                             )
         except pyrogram.StopTransmission:
             return None
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_poll.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_poll.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,23 +248,25 @@
                     raw.types.UpdateNewScheduledMessage
                 )
             ):
                 return await types.Message._parse(
                     self, i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
-                    is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage)
+                    is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
+                    replies=self.fetch_replies
                 )
             elif isinstance(
                 i,
                 (
                     raw.types.UpdateBotNewBusinessMessage
                 )
             ):
                 return await types.Message._parse(
                     self,
                     i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     business_connection_id=getattr(i, "connection_id", business_connection_id),
-                    raw_reply_to_message=i.reply_to_message
+                    raw_reply_to_message=i.reply_to_message,
+                    replies=0
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_sticker.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_sticker.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,25 +250,27 @@
                                 raw.types.UpdateNewScheduledMessage
                             )
                         ):
                             return await types.Message._parse(
                                 self, i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
-                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage)
+                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
+                                replies=self.fetch_replies
                             )
                         elif isinstance(
                             i,
                             (
                                 raw.types.UpdateBotNewBusinessMessage
                             )
                         ):
                             return await types.Message._parse(
                                 self,
                                 i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
                                 business_connection_id=getattr(i, "connection_id", business_connection_id),
-                                raw_reply_to_message=i.reply_to_message
+                                raw_reply_to_message=i.reply_to_message,
+                                replies=0
                             )
         except StopTransmission:
             return None
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_venue.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_venue.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,23 +177,25 @@
                     raw.types.UpdateNewScheduledMessage
                 )
             ):
                 return await types.Message._parse(
                     self, i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
-                    is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage)
+                    is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
+                    replies=self.fetch_replies
                 )
             elif isinstance(
                 i,
                 (
                     raw.types.UpdateBotNewBusinessMessage
                 )
             ):
                 return await types.Message._parse(
                     self,
                     i.message,
                     {i.id: i for i in r.users},
                     {i.id: i for i in r.chats},
                     business_connection_id=getattr(i, "connection_id", business_connection_id),
-                    raw_reply_to_message=i.reply_to_message
+                    raw_reply_to_message=i.reply_to_message,
+                    replies=0
                 )
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_video.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_video.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     async def send_video(
         self: "pyrogram.Client",
         chat_id: Union[int, str],
         video: Union[str, BinaryIO],
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
+        show_caption_above_media: bool = None,
         duration: int = 0,
         width: int = 0,
         height: int = 0,
         thumb: Union[str, BinaryIO] = None,
         has_spoiler: bool = None,
         supports_streaming: bool = True,
         disable_notification: bool = None,
@@ -88,14 +89,17 @@
             parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
                 By default, texts are parsed using both Markdown and HTML styles.
                 You can combine both syntaxes together.
 
             caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
                 List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
+            show_caption_above_media (``bool``, *optional*):
+                Pass True, if the caption must be shown above the message media.
+
             duration (``int``, *optional*):
                 Duration of sent video in seconds.
 
             width (``int``, *optional*):
                 Video width.
 
             height (``int``, *optional*):
@@ -281,14 +285,15 @@
                 silent=disable_notification or None,
                 reply_to=reply_to,
                 random_id=self.rnd_id(),
                 schedule_date=utils.datetime_to_timestamp(schedule_date),
                 noforwards=protect_content,
                 reply_markup=await reply_markup.write(self) if reply_markup else None,
                 effect=message_effect_id,
+                invert_media=show_caption_above_media,
                 **await utils.parse_text_entities(self, caption, parse_mode, caption_entities)
             )
             session = None
             business_connection = None
             if business_connection_id:
                 business_connection = self.business_user_connection_cache[business_connection_id]
                 if not business_connection:
@@ -322,25 +327,27 @@
                                 raw.types.UpdateNewScheduledMessage
                             )
                         ):
                             return await types.Message._parse(
                                 self, i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
-                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage)
+                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
+                                replies=self.fetch_replies
                             )
                         elif isinstance(
                             i,
                             (
                                 raw.types.UpdateBotNewBusinessMessage
                             )
                         ):
                             return await types.Message._parse(
                                 self,
                                 i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
                                 business_connection_id=getattr(i, "connection_id", business_connection_id),
-                                raw_reply_to_message=i.reply_to_message
+                                raw_reply_to_message=i.reply_to_message,
+                                replies=0
                             )
         except StopTransmission:
             return None
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_video_note.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_video_note.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,25 +287,27 @@
                                 raw.types.UpdateNewScheduledMessage
                             )
                         ):
                             return await types.Message._parse(
                                 self, i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
-                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage)
+                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
+                                replies=self.fetch_replies
                             )
                         elif isinstance(
                             i,
                             (
                                 raw.types.UpdateBotNewBusinessMessage
                             )
                         ):
                             return await types.Message._parse(
                                 self,
                                 i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
                                 business_connection_id=getattr(i, "connection_id", business_connection_id),
-                                raw_reply_to_message=i.reply_to_message
+                                raw_reply_to_message=i.reply_to_message,
+                                replies=0
                             )
         except StopTransmission:
             return None
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/send_voice.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/send_voice.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,25 +282,27 @@
                                 raw.types.UpdateNewScheduledMessage
                             )
                         ):
                             return await types.Message._parse(
                                 self, i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
-                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage)
+                                is_scheduled=isinstance(i, raw.types.UpdateNewScheduledMessage),
+                                replies=self.fetch_replies
                             )
                         elif isinstance(
                             i,
                             (
                                 raw.types.UpdateBotNewBusinessMessage
                             )
                         ):
                             return await types.Message._parse(
                                 self,
                                 i.message,
                                 {i.id: i for i in r.users},
                                 {i.id: i for i in r.chats},
                                 business_connection_id=getattr(i, "connection_id", business_connection_id),
-                                raw_reply_to_message=i.reply_to_message
+                                raw_reply_to_message=i.reply_to_message,
+                                replies=0
                             )
         except StopTransmission:
             return None
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/set_reaction.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/set_reaction.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/stop_poll.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/stream_media.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/view_messages.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/view_messages.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/messages/vote_poll.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/password/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/password/change_cloud_password.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/password/enable_cloud_password.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/password/remove_cloud_password.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/phone/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/phone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/phone/load_group_call_participants.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/phone/load_group_call_participants.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/stickers/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/parser/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,8 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from .get_stickers import GetStickers
-
-
-class Stickers(
-    GetStickers,
-):
-    pass
+from .parser import Parser
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/stickers/get_stickers.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/stickers/get_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/block_user.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/delete_profile_photos.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/get_chat_photos.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/get_chat_photos_count.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/get_common_chats.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/get_default_emoji_statuses.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/get_me.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/get_users.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/set_birthdate.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/set_birthdate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/set_emoji_status.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/set_personal_chat.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/set_personal_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/set_profile_photo.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/set_username.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/unblock_user.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/users/update_profile.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/utilities/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/utilities/add_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/utilities/compose.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/utilities/export_session_string.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/utilities/idle.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/utilities/remove_handler.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/utilities/restart.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/utilities/run.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/utilities/start.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/utilities/stop.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/methods/utilities/stop_transmission.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/parser/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/session/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from .parser import Parser
+from .auth import Auth
+from .session import Session
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/parser/html.py` & `pyrotgfork-2.1.32.3/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/parser/markdown.py` & `pyrotgfork-2.1.32.3/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/parser/parser.py` & `pyrotgfork-2.1.32.3/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/parser/utils.py` & `pyrotgfork-2.1.32.3/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/core/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/core/future_salt.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/core/future_salts.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/core/gzip_packed.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/core/list.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/core/message.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/core/msg_container.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/core/tl_object.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/core/primitives/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/core/primitives/bool.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/core/primitives/bytes.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/core/primitives/double.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/core/primitives/int.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/core/primitives/string.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/raw/core/primitives/vector.py` & `pyrotgfork-2.1.32.3/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/session/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/session/internals/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from .auth import Auth
-from .session import Session
+from .data_center import DataCenter
+from .msg_factory import MsgFactory
+from .msg_id import MsgId
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/session/auth.py` & `pyrotgfork-2.1.32.3/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/session/session.py` & `pyrotgfork-2.1.32.3/pyrogram/session/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 import asyncio
 import bisect
 import logging
 import os
+from datetime import datetime, timedelta
 from hashlib import sha1
 from io import BytesIO
 
 import pyrogram
 from pyrogram import raw
 from pyrogram.connection import Connection
 from pyrogram.crypto import mtproto
@@ -50,14 +51,15 @@
     START_TIMEOUT = 2
     WAIT_TIMEOUT = 15
     SLEEP_THRESHOLD = 10
     MAX_RETRIES = 10
     ACKS_THRESHOLD = 10
     PING_INTERVAL = 5
     STORED_MSG_IDS_MAX_SIZE = 1000 * 2
+    RECONNECT_THRESHOLD = timedelta(seconds=10)
 
     TRANSPORT_ERRORS = {
         404: "auth key not found",
         429: "transport flood",
         444: "invalid DC"
     }
 
@@ -103,14 +105,16 @@
 
         self.recv_task = None
 
         self.is_started = asyncio.Event()
 
         self.loop = asyncio.get_event_loop()
 
+        self.last_reconnect_attempt = None
+
     async def start(self):
         while True:
             self.connection = Connection(
                 self.dc_id,
                 self.test_mode,
                 self.client.ipv6,
                 self.client.proxy,
@@ -189,14 +193,24 @@
                 await self.client.disconnect_handler(self.client)
             except Exception as e:
                 log.exception(e)
 
         log.info("Session stopped")
 
     async def restart(self):
+        now = datetime.now()
+        if (
+            self.last_reconnect_attempt
+            and now - self.last_reconnect_attempt < self.RECONNECT_THRESHOLD
+        ):
+            log.info("Reconnecting too frequently, sleeping for a while")
+            await asyncio.sleep(5)
+
+        self.last_reconnect_attempt = now
+
         await self.stop()
         await self.start()
 
     async def handle_packet(self, packet):
         data = await self.loop.run_in_executor(
             pyrogram.crypto_executor,
             mtproto.unpack,
@@ -396,40 +410,44 @@
         if isinstance(query, Session.CUR_ALWD_INNR_QRYS):
             inner_query = query.query
         else:
             inner_query = query
 
         query_name = ".".join(inner_query.QUALNAME.split(".")[1:])
 
-        while True:
+        while retries > 0:
             try:
                 return await self.send(query, timeout=timeout)
             except (FloodWait, FloodPremiumWait) as e:
                 amount = e.value
 
                 if amount > sleep_threshold >= 0:
                     raise
 
                 log.warning('[%s] Waiting for %s seconds before continuing (required by "%s")',
                             self.client.name, amount, query_name)
 
                 await asyncio.sleep(amount)
             except (OSError, InternalServerError, ServiceUnavailable) as e:
-                if retries == 0 \
-                        or (
-                            isinstance(e, InternalServerError)
-                            and getattr(e, "code", 0) == 500
-                            and (e.ID or e.NAME) in [
-                                "HISTORY_GET_FAILED"
-                            ]
-                        ):
+                retries -= 1
+                if (
+                    retries == 0 or
+                    (
+                        isinstance(e, InternalServerError)
+                        and getattr(e, "code", 0) == 500
+                        and (e.ID or e.NAME) in [
+                            "HISTORY_GET_FAILED"
+                        ]
+                    )
+                ):
                     raise e from None
 
                 (log.warning if retries < 2 else log.info)(
                     '[%s] Retrying "%s" due to: %s',
-                    Session.MAX_RETRIES - retries + 1,
-                    query_name, str(e) or repr(e)
+                    Session.MAX_RETRIES - retries,
+                    query_name,
+                    str(e) or repr(e)
                 )
 
                 await asyncio.sleep(3)
 
-                return await self.invoke(query, retries - 1, timeout)
+        raise TimeoutError("Exceeded maximum number of retries")
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/session/internals/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,10 +12,18 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from .data_center import DataCenter
-from .msg_factory import MsgFactory
-from .msg_id import MsgId
+from ..object import Object
+
+
+class VideoChatStarted(Object):
+    """A service message about a voice chat started in the chat.
+
+    Currently holds no information.
+    """
+
+    def __init__(self):
+        super().__init__()
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/session/internals/data_center.py` & `pyrotgfork-2.1.32.3/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/session/internals/msg_factory.py` & `pyrotgfork-2.1.32.3/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/session/internals/msg_id.py` & `pyrotgfork-2.1.32.3/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/session/internals/seq_no.py` & `pyrotgfork-2.1.32.3/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/storage/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/storage/aio_sqlite_storage.py` & `pyrotgfork-2.1.32.3/pyrogram/storage/aio_sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/storage/file_storage.py` & `pyrotgfork-2.1.32.3/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/storage/memory_storage.py` & `pyrotgfork-2.1.32.3/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/storage/sqlite_storage.py` & `pyrotgfork-2.1.32.3/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/storage/storage.py` & `pyrotgfork-2.1.32.3/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/list.py` & `pyrotgfork-2.1.32.3/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/object.py` & `pyrotgfork-2.1.32.3/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/update.py` & `pyrotgfork-2.1.32.3/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/authorization/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/authorization/sent_code.py` & `pyrotgfork-2.1.32.3/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/authorization/terms_of_service.py` & `pyrotgfork-2.1.32.3/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/callback_game.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/callback_query.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/force_reply.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/game_high_score.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/keyboard_button_poll_type.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/keyboard_button_request_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/keyboard_button_request_users.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/login_url.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/menu_button.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/switch_inline_query_chosen_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/bots_and_keyboards/web_app_info.py` & `pyrotgfork-2.1.32.3/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/business/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/types/business/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/business/business_connection.py` & `pyrotgfork-2.1.32.3/pyrogram/types/business/business_connection.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/business/business_intro.py` & `pyrotgfork-2.1.32.3/pyrogram/types/business/business_intro.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/business/business_location.py` & `pyrotgfork-2.1.32.3/pyrogram/types/business/business_location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/business/business_opening_hours.py` & `pyrotgfork-2.1.32.3/pyrogram/types/business/business_opening_hours.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/business/business_opening_hours_interval.py` & `pyrotgfork-2.1.32.3/pyrogram/types/business/business_opening_hours_interval.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/business/collectible_item_info.py` & `pyrotgfork-2.1.32.3/pyrogram/types/business/collectible_item_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/business/invoice.py` & `pyrotgfork-2.1.32.3/pyrogram/types/business/invoice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/forum_topic.py` & `pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/forum_topic_closed.py` & `pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/forum_topic_created.py` & `pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/forum_topic_edited.py` & `pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/forum_topic_reopened.py` & `pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/general_forum_topic_hidden.py` & `pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/chat_topics/general_forum_topic_unhidden.py` & `pyrotgfork-2.1.32.3/pyrogram/types/chat_topics/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/chosen_inline_result.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_animation.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_article.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_audio.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_contact.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_document.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_location.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_photo.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_venue.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_video.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/inline_mode/inline_query_result_voice.py` & `pyrotgfork-2.1.32.3/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_media/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_media/input_media.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_media/input_media_animation.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_media/input_media_audio.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_media/input_media_document.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_media/input_media_photo.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_media/input_media_video.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_media/input_phone_contact.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_media/link_preview_options.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_media/link_preview_options.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_message_content/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_message_content/external_reply_info.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_message_content/external_reply_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_message_content/input_message_content.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_message_content/input_poll_option.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_message_content/input_poll_option.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_message_content/input_text_message_content.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_message_content/reply_parameters.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_message_content/reply_parameters.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/input_message_content/text_quote.py` & `pyrotgfork-2.1.32.3/pyrogram/types/input_message_content/text_quote.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/message_origin/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/types/message_origin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/message_origin/message_import_info.py` & `pyrotgfork-2.1.32.3/pyrogram/types/message_origin/message_import_info.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/message_origin/message_origin.py` & `pyrotgfork-2.1.32.3/pyrogram/types/message_origin/message_origin.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/message_origin/message_origin_channel.py` & `pyrotgfork-2.1.32.3/pyrogram/types/message_origin/message_origin_channel.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/message_origin/message_origin_chat.py` & `pyrotgfork-2.1.32.3/pyrogram/types/message_origin/message_origin_chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/message_origin/message_origin_hidden_user.py` & `pyrotgfork-2.1.32.3/pyrogram/types/message_origin/message_origin_hidden_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/message_origin/message_origin_user.py` & `pyrotgfork-2.1.32.3/pyrogram/types/message_origin/message_origin_user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 from .chat_boost_added import ChatBoostAdded
 from .story import Story
 from .giveaway import Giveaway
 from .giveaway_completed import GiveawayCompleted
 from .giveaway_winners import GiveawayWinners
 from .gift_code import GiftCode
 from .gifted_premium import GiftedPremium
+from .message_effect import MessageEffect
 
 __all__ = [
     "Animation",
     "Audio",
     "ChatBoostAdded",
     "Contact",
     "Dice",
@@ -67,14 +68,15 @@
     "GiftCode",
     "GiftedPremium",
     "Giveaway",
     "GiveawayCompleted",
     "GiveawayWinners",
     "Location",
     "Message",
+    "MessageEffect",
     "MessageEntity",
     "MessageReactionCountUpdated",
     "MessageReactionUpdated",
     "MessageReactions",
     "Photo",
     "Reaction",
     "ReactionCount",
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/animation.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/audio.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/chat_boost_added.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/chat_boost_added.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/contact.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/dice.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/document.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/game.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/gift_code.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/gift_code.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/gifted_premium.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/gifted_premium.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/giveaway.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/giveaway.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/giveaway_completed.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/giveaway_completed.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/giveaway_winners.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/giveaway_winners.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/location.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/message.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         entities (List of :obj:`~pyrogram.types.MessageEntity`, *optional*):
             For text messages, special entities like usernames, URLs, bot commands, etc. that appear in the text.
 
         link_preview_options (:obj:`~pyrogram.types.LinkPreviewOptions`, *optional*):
             Options used for link preview generation for the message, if it is a text message and link preview options were changed
 
         effect_id (``str``, *optional*):
-            Unique identifier of the message effect added to the message.
+            Unique identifier of the message effect added to the message. Use :meth:`~pyrogram.Client.get_message_effects` to get the list of available message effect ids.
 
         animation (:obj:`~pyrogram.types.Animation`, *optional*):
             Message is an animation, information about the animation.
 
         audio (:obj:`~pyrogram.types.Audio`, *optional*):
             Message is an audio file, information about the file.
 
@@ -1279,15 +1279,16 @@
             parsed_message.business_connection_id = business_connection_id
         if raw_reply_to_message:
             parsed_message.reply_to_message = await types.Message._parse(
                 client,
                 raw_reply_to_message,
                 users,
                 chats,
-                business_connection_id=business_connection_id
+                business_connection_id=business_connection_id,
+                replies=0
             )
 
         if not parsed_message.poll:  # Do not cache poll messages
             client.message_cache[(parsed_message.chat.id, parsed_message.id)] = parsed_message
 
         parsed_message._raw = message
 
@@ -1451,22 +1452,24 @@
     async def reply_animation(
         self,
         animation: Union[str, BinaryIO],
         quote: bool = None,
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
+        show_caption_above_media: bool = None,
         unsave: bool = False,
         has_spoiler: bool = None,
         duration: int = 0,
         width: int = 0,
         height: int = 0,
         thumb: str = None,
         file_name: str = None,
         disable_notification: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         schedule_date: datetime = None,
         protect_content: bool = None,
         ttl_seconds: int = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
@@ -1511,14 +1514,17 @@
             parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
                 By default, texts are parsed using both Markdown and HTML styles.
                 You can combine both syntaxes together.
 
             caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
                 List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
+            show_caption_above_media (``bool``, *optional*):
+                Pass True, if the caption must be shown above the message media.
+
             unsave (``bool``, *optional*):
                 By default, the server will save into your own collection any new animation you send.
                 Pass True to automatically unsave the sent animation. Defaults to False.
 
             has_spoiler (``bool``, *optional*):
                 Pass True if the animation needs to be covered with a spoiler animation.
 
@@ -1541,14 +1547,17 @@
                 File name of the animation sent.
                 Defaults to file's path basename.
 
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             schedule_date (:py:obj:`~datetime.datetime`, *optional*):
                 Date when the message will be automatically sent.
 
             protect_content (``bool``, *optional*):
@@ -1603,22 +1612,24 @@
 
         return await self._client.send_animation(
             chat_id=self.chat.id,
             animation=animation,
             caption=caption,
             parse_mode=parse_mode,
             caption_entities=caption_entities,
+            show_caption_above_media=show_caption_above_media,
             unsave=unsave,
             has_spoiler=has_spoiler,
             duration=duration,
             width=width,
             height=height,
             thumb=thumb,
             file_name=file_name,
             disable_notification=disable_notification,
+            message_effect_id=message_effect_id,
             reply_parameters=reply_parameters,
             message_thread_id=self.message_thread_id,
             business_connection_id=self.business_connection_id,
             schedule_date=schedule_date,
             protect_content=protect_content,
             ttl_seconds=ttl_seconds,
             reply_markup=reply_markup,
@@ -1636,14 +1647,15 @@
         caption_entities: List["types.MessageEntity"] = None,
         duration: int = 0,
         performer: str = None,
         title: str = None,
         thumb: str = None,
         file_name: str = None,
         disable_notification: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         schedule_date: datetime = None,
         protect_content: bool = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
             "types.ReplyKeyboardRemove",
@@ -1710,14 +1722,17 @@
                 File name of the audio sent.
                 Defaults to file's path basename.
 
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             schedule_date (:py:obj:`~datetime.datetime`, *optional*):
                 Date when the message will be automatically sent.
 
             protect_content (``bool``, *optional*):
@@ -1773,14 +1788,15 @@
             caption_entities=caption_entities,
             duration=duration,
             performer=performer,
             title=title,
             thumb=thumb,
             file_name=file_name,
             disable_notification=disable_notification,
+            message_effect_id=message_effect_id,
             reply_parameters=reply_parameters,
             message_thread_id=self.message_thread_id,
             business_connection_id=self.business_connection_id,
             schedule_date=schedule_date,
             protect_content=protect_content,
             reply_markup=reply_markup,
             reply_to_message_id=reply_to_message_id,
@@ -1791,15 +1807,17 @@
     async def reply_cached_media(
         self,
         file_id: str,
         quote: bool = None,
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
+        show_caption_above_media: bool = None,
         disable_notification: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         schedule_date: datetime = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
             "types.ReplyKeyboardRemove",
             "types.ForceReply"
@@ -1838,18 +1856,24 @@
             parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
                 By default, texts are parsed using both Markdown and HTML styles.
                 You can combine both syntaxes together.
 
             caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
                 List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
+            show_caption_above_media (``bool``, *optional*):
+                Pass True, if the caption must be shown above the message media. Supported only for animation, photo and video messages.
+
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             schedule_date (:py:obj:`~datetime.datetime`, *optional*):
                 Date when the message will be automatically sent.
 
             reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardRemove` | :obj:`~pyrogram.types.ForceReply`, *optional*):
@@ -1872,15 +1896,17 @@
 
         return await self._client.send_cached_media(
             chat_id=self.chat.id,
             file_id=file_id,
             caption=caption,
             parse_mode=parse_mode,
             caption_entities=caption_entities,
+            show_caption_above_media=show_caption_above_media,
             disable_notification=disable_notification,
+            message_effect_id=message_effect_id,
             reply_parameters=reply_parameters,
             message_thread_id=self.message_thread_id,
             business_connection_id=self.business_connection_id,
             schedule_date=schedule_date,
             protect_content=self.has_protected_content,
             has_spoiler=self.has_media_spoiler,
             reply_markup=reply_markup,
@@ -1953,14 +1979,15 @@
         self,
         phone_number: str,
         first_name: str,
         quote: bool = None,
         last_name: str = "",
         vcard: str = "",
         disable_notification: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         schedule_date: datetime = None,
         protect_content: bool = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
             "types.ReplyKeyboardRemove",
@@ -2003,14 +2030,17 @@
             vcard (``str``, *optional*):
                 Additional data about the contact in the form of a vCard, 0-2048 bytes
 
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             schedule_date (:py:obj:`~datetime.datetime`, *optional*):
                 Date when the message will be automatically sent.
 
             protect_content (``bool``, *optional*):
@@ -2037,14 +2067,15 @@
         return await self._client.send_contact(
             chat_id=self.chat.id,
             phone_number=phone_number,
             first_name=first_name,
             last_name=last_name,
             vcard=vcard,
             disable_notification=disable_notification,
+            message_effect_id=message_effect_id,
             reply_parameters=reply_parameters,
             message_thread_id=self.message_thread_id,
             business_connection_id=self.business_connection_id,
             schedule_date=schedule_date,
             protect_content=protect_content,
             reply_markup=reply_markup,
             reply_to_message_id=reply_to_message_id
@@ -2057,14 +2088,15 @@
         thumb: str = None,
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
         file_name: str = None,
         disable_content_type_detection: bool = None,
         disable_notification: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         schedule_date: datetime = None,
         protect_content: bool = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
             "types.ReplyKeyboardRemove",
@@ -2128,14 +2160,17 @@
                 document messages instead of video messages.
                 Defaults to False.
 
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             schedule_date (:py:obj:`~datetime.datetime`, *optional*):
                 Date when the message will be automatically sent.
 
             protect_content (``bool``, *optional*):
@@ -2189,14 +2224,15 @@
             thumb=thumb,
             caption=caption,
             parse_mode=parse_mode,
             caption_entities=caption_entities,
             file_name=file_name,
             disable_content_type_detection=disable_content_type_detection,
             disable_notification=disable_notification,
+            message_effect_id=message_effect_id,
             reply_parameters=reply_parameters,
             message_thread_id=self.message_thread_id,
             business_connection_id=self.business_connection_id,
             schedule_date=schedule_date,
             protect_content=protect_content,
             reply_markup=reply_markup,
             reply_to_message_id=reply_to_message_id,
@@ -2206,14 +2242,15 @@
 
     async def reply_game(
         self,
         game_short_name: str,
         quote: bool = None,
         disable_notification: bool = None,
         protect_content: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
             "types.ReplyKeyboardRemove",
             "types.ForceReply"
         ] = None,
@@ -2244,14 +2281,17 @@
                 If *reply_to_message_id* is passed, this parameter will be ignored.
                 Defaults to ``True`` in group chats and ``False`` in private chats.
 
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             protect_content (``bool``, *optional*):
                 Protects the contents of the sent message from forwarding and saving.
 
             reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
@@ -2272,14 +2312,15 @@
                 message_id=self.id
             )
 
         return await self._client.send_game(
             chat_id=self.chat.id,
             game_short_name=game_short_name,
             disable_notification=disable_notification,
+            message_effect_id=message_effect_id,
             reply_parameters=reply_parameters,
             protect_content=protect_content,
             message_thread_id=self.message_thread_id,
             business_connection_id=self.business_connection_id,
             reply_markup=reply_markup,
             reply_to_message_id=reply_to_message_id
         )
@@ -2354,14 +2395,15 @@
 
     async def reply_location(
         self,
         latitude: float,
         longitude: float,
         quote: bool = None,
         disable_notification: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         schedule_date: datetime = None,
         protect_content: bool = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
             "types.ReplyKeyboardRemove",
@@ -2398,14 +2440,17 @@
                 If *reply_to_message_id* is passed, this parameter will be ignored.
                 Defaults to ``True`` in group chats and ``False`` in private chats.
 
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             schedule_date (:py:obj:`~datetime.datetime`, *optional*):
                 Date when the message will be automatically sent.
 
             protect_content (``bool``, *optional*):
@@ -2430,28 +2475,30 @@
             )
 
         return await self._client.send_location(
             chat_id=self.chat.id,
             latitude=latitude,
             longitude=longitude,
             disable_notification=disable_notification,
+            message_effect_id=message_effect_id,
             reply_parameters=reply_parameters,
             message_thread_id=self.message_thread_id,
             business_connection_id=self.business_connection_id,
             schedule_date=schedule_date,
             protect_content=protect_content,
             reply_markup=reply_markup,
             reply_to_message_id=reply_to_message_id
         )
 
     async def reply_media_group(
         self,
         media: List[Union["types.InputMediaPhoto", "types.InputMediaVideo"]],
         quote: bool = None,
         disable_notification: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         schedule_date: datetime = None,
         protect_content: bool = None,
         reply_to_message_id: int = None
     ) -> List["types.Message"]:
         """Bound method *reply_media_group* of :obj:`~pyrogram.types.Message`.
 
@@ -2480,14 +2527,17 @@
                 If *reply_to_message_id* is passed, this parameter will be ignored.
                 Defaults to ``True`` in group chats and ``False`` in private chats.
 
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             schedule_date (:py:obj:`~datetime.datetime`, *optional*):
                 Date when the message will be automatically sent.
 
             protect_content (``bool``, *optional*):
@@ -2508,14 +2558,15 @@
                 message_id=self.id
             )
 
         return await self._client.send_media_group(
             chat_id=self.chat.id,
             media=media,
             disable_notification=disable_notification,
+            message_effect_id=message_effect_id,
             reply_parameters=reply_parameters,
             message_thread_id=self.message_thread_id,
             business_connection_id=self.business_connection_id,
             schedule_date=schedule_date,
             protect_content=protect_content,
             reply_to_message_id=reply_to_message_id
         )
@@ -2523,17 +2574,19 @@
     async def reply_photo(
         self,
         photo: Union[str, BinaryIO],
         quote: bool = None,
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
+        show_caption_above_media: bool = None,
         has_spoiler: bool = None,
         ttl_seconds: int = None,
         disable_notification: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         schedule_date: datetime = None,
         protect_content: bool = None,
         view_once: bool = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
@@ -2578,26 +2631,32 @@
             parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
                 By default, texts are parsed using both Markdown and HTML styles.
                 You can combine both syntaxes together.
 
             caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
                 List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
+            show_caption_above_media (``bool``, *optional*):
+                Pass True, if the caption must be shown above the message media.
+
             has_spoiler (``bool``, *optional*):
                 Pass True if the photo needs to be covered with a spoiler animation.
 
             ttl_seconds (``int``, *optional*):
                 Self-Destruct Timer.
                 If you set a timer, the photo will self-destruct in *ttl_seconds*
                 seconds after it was viewed.
 
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             schedule_date (:py:obj:`~datetime.datetime`, *optional*):
                 Date when the message will be automatically sent.
 
             protect_content (``bool``, *optional*):
@@ -2650,17 +2709,19 @@
 
         return await self._client.send_photo(
             chat_id=self.chat.id,
             photo=photo,
             caption=caption,
             parse_mode=parse_mode,
             caption_entities=caption_entities,
+            show_caption_above_media=show_caption_above_media,
             has_spoiler=has_spoiler,
             ttl_seconds=ttl_seconds,
             disable_notification=disable_notification,
+            message_effect_id=message_effect_id,
             reply_parameters=reply_parameters,
             message_thread_id=self.message_thread_id,
             business_connection_id=self.business_connection_id,
             schedule_date=schedule_date,
             protect_content=protect_content,
             view_once=view_once,
             reply_markup=reply_markup,
@@ -2669,27 +2730,30 @@
             progress_args=progress_args
         )
 
     async def reply_poll(
         self,
         question: str,
         options: List[str],
+        question_parse_mode: "enums.ParseMode" = None,
+        question_entities: List["types.MessageEntity"] = None,
         is_anonymous: bool = True,
         type: "enums.PollType" = enums.PollType.REGULAR,
         allows_multiple_answers: bool = None,
         correct_option_id: int = None,
         explanation: str = None,
         explanation_parse_mode: "enums.ParseMode" = None,
         explanation_entities: List["types.MessageEntity"] = None,
         open_period: int = None,
         close_date: datetime = None,
         is_closed: bool = None,
         quote: bool = None,
         disable_notification: bool = None,
         protect_content: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         schedule_date: datetime = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
             "types.ReplyKeyboardRemove",
             "types.ForceReply"
@@ -2716,14 +2780,21 @@
         Parameters:
             question (``str``):
                 Poll question, 1-255 characters.
 
             options (List of ``str``):
                 List of answer options, 2-10 strings 1-100 characters each.
 
+            question_parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
+                By default, texts are parsed using both Markdown and HTML styles.
+                You can combine both syntaxes together.
+
+            question_entities (List of :obj:`~pyrogram.types.MessageEntity`):
+                List of special entities that appear in the poll question, which can be specified instead of *question_parse_mode*.
+
             is_anonymous (``bool``, *optional*):
                 True, if the poll needs to be anonymous.
                 Defaults to True.
 
             type (:obj`~pyrogram.enums.PollType`, *optional*):
                 Poll type, :obj:`~pyrogram.enums.PollType.QUIZ` or :obj:`~pyrogram.enums.PollType.REGULAR`.
                 Defaults to :obj:`~pyrogram.enums.PollType.REGULAR`.
@@ -2768,14 +2839,17 @@
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
             protect_content (``bool``, *optional*):
                 Protects the contents of the sent message from forwarding and saving.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             schedule_date (:py:obj:`~datetime.datetime`, *optional*):
                 Date when the message will be automatically sent.
 
             reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardRemove` | :obj:`~pyrogram.types.ForceReply`, *optional*):
@@ -2808,28 +2882,30 @@
             explanation_parse_mode=explanation_parse_mode,
             explanation_entities=explanation_entities,
             open_period=open_period,
             close_date=close_date,
             is_closed=is_closed,
             disable_notification=disable_notification,
             protect_content=protect_content,
+            message_effect_id=message_effect_id,
             reply_parameters=reply_parameters,
             message_thread_id=self.message_thread_id,
             business_connection_id=self.business_connection_id,
             schedule_date=schedule_date,
             reply_to_message_id=reply_to_message_id,
             reply_markup=reply_markup
         )
 
     async def reply_sticker(
         self,
         sticker: Union[str, BinaryIO],
         quote: bool = None,
         disable_notification: bool = None,
         protect_content: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
             "types.ReplyKeyboardRemove",
             "types.ForceReply"
         ] = None,
@@ -2869,14 +2945,17 @@
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
             protect_content (``bool``, *optional*):
                 Protects the contents of the sent message from forwarding and saving.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardRemove` | :obj:`~pyrogram.types.ForceReply`, *optional*):
                 Additional interface options. An object for an inline keyboard, custom reply keyboard,
                 instructions to remove reply keyboard or to force a reply from the user.
 
@@ -2924,14 +3003,15 @@
         return await self._client.send_sticker(
             chat_id=self.chat.id,
             sticker=sticker,
             disable_notification=disable_notification,
             protect_content=protect_content,
             message_thread_id=self.message_thread_id,
             business_connection_id=self.business_connection_id,
+            message_effect_id=message_effect_id,
             reply_parameters=reply_parameters,
             reply_markup=reply_markup,
             schedule_date=schedule_date,
             reply_to_message_id=reply_to_message_id,
             progress=progress,
             progress_args=progress_args
         )
@@ -2942,14 +3022,15 @@
         longitude: float,
         title: str,
         address: str,
         quote: bool = None,
         foursquare_id: str = "",
         foursquare_type: str = "",
         disable_notification: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         schedule_date: datetime = None,
         protect_content: bool = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
             "types.ReplyKeyboardRemove",
@@ -3007,14 +3088,17 @@
 
             schedule_date (:py:obj:`~datetime.datetime`, *optional*):
                 Date when the message will be automatically sent.
 
             protect_content (``bool``, *optional*):
                 Protects the contents of the sent message from forwarding and saving.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardRemove` | :obj:`~pyrogram.types.ForceReply`, *optional*):
                 Additional interface options. An object for an inline keyboard, custom reply keyboard,
                 instructions to remove reply keyboard or to force a reply from the user.
 
@@ -3037,14 +3121,15 @@
             latitude=latitude,
             longitude=longitude,
             title=title,
             address=address,
             foursquare_id=foursquare_id,
             foursquare_type=foursquare_type,
             disable_notification=disable_notification,
+            message_effect_id=message_effect_id,
             reply_parameters=reply_parameters,
             message_thread_id=self.message_thread_id,
             business_connection_id=self.business_connection_id,
             schedule_date=schedule_date,
             protect_content=protect_content,
             reply_to_message_id=reply_to_message_id,
             reply_markup=reply_markup
@@ -3053,22 +3138,24 @@
     async def reply_video(
         self,
         video: Union[str, BinaryIO],
         quote: bool = None,
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
+        show_caption_above_media: bool = None,
         duration: int = 0,
         width: int = 0,
         height: int = 0,
         thumb: str = None,
         has_spoiler: bool = None,
         supports_streaming: bool = True,
         disable_notification: bool = None,
         protect_content: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
             "types.ReplyKeyboardRemove",
             "types.ForceReply"
         ] = None,
@@ -3114,14 +3201,17 @@
             parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
                 By default, texts are parsed using both Markdown and HTML styles.
                 You can combine both syntaxes together.
 
             caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
                 List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
+            show_caption_above_media (``bool``, *optional*):
+                Pass True, if the caption must be shown above the message media.
+
             duration (``int``, *optional*):
                 Duration of sent video in seconds.
 
             width (``int``, *optional*):
                 Video width.
 
             height (``int``, *optional*):
@@ -3143,14 +3233,17 @@
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
             protect_content (``bool``, *optional*):
                 Protects the contents of the sent message from forwarding and saving.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardRemove` | :obj:`~pyrogram.types.ForceReply`, *optional*):
                 Additional interface options. An object for an inline keyboard, custom reply keyboard,
                 instructions to remove reply keyboard or to force a reply from the user.
 
@@ -3209,24 +3302,26 @@
 
         return await self._client.send_video(
             chat_id=self.chat.id,
             video=video,
             caption=caption,
             parse_mode=parse_mode,
             caption_entities=caption_entities,
+            show_caption_above_media=show_caption_above_media,
             duration=duration,
             width=width,
             height=height,
             thumb=thumb,
             has_spoiler=has_spoiler,
             supports_streaming=supports_streaming,
             disable_notification=disable_notification,
             protect_content=protect_content,
             message_thread_id=self.message_thread_id,
             business_connection_id=self.business_connection_id,
+            message_effect_id=message_effect_id,
             reply_parameters=reply_parameters,
             reply_markup=reply_markup,
             ttl_seconds=ttl_seconds,
             view_once=view_once,
             file_name=file_name,
             schedule_date=schedule_date,
             reply_to_message_id=reply_to_message_id,
@@ -3239,14 +3334,15 @@
         video_note: Union[str, BinaryIO],
         quote: bool = None,
         duration: int = 0,
         length: int = 1,
         thumb: str = None,
         disable_notification: bool = None,
         protect_content: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
             "types.ReplyKeyboardRemove",
             "types.ForceReply"
         ] = None,
@@ -3303,14 +3399,17 @@
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
             protect_content (``bool``, *optional*):
                 Protects the contents of the sent message from forwarding and saving.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardRemove` | :obj:`~pyrogram.types.ForceReply`, *optional*):
                 Additional interface options. An object for an inline keyboard, custom reply keyboard,
                 instructions to remove reply keyboard or to force a reply from the user.
 
@@ -3379,14 +3478,15 @@
             duration=duration,
             length=length,
             thumb=thumb,
             disable_notification=disable_notification,
             protect_content=protect_content,
             message_thread_id=self.message_thread_id,
             business_connection_id=self.business_connection_id,
+            message_effect_id=message_effect_id,
             reply_parameters=reply_parameters,
             reply_markup=reply_markup,
             caption=caption,
             parse_mode=parse_mode,
             caption_entities=caption_entities,
             schedule_date=schedule_date,
             ttl_seconds=ttl_seconds,
@@ -3402,14 +3502,15 @@
         quote: bool = None,
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
         duration: int = 0,
         disable_notification: bool = None,
         protect_content: bool = None,
+        message_effect_id: int = None,
         reply_parameters: "types.ReplyParameters" = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
             "types.ReplyKeyboardRemove",
             "types.ForceReply"
         ] = None,
@@ -3465,14 +3566,17 @@
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
             protect_content (``bool``, *optional*):
                 Protects the contents of the sent message from forwarding and saving.
 
+            message_effect_id (``int`` ``64-bit``, *optional*):
+                Unique identifier of the message effect to be added to the message; for private chats only.
+
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
             reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardMarkup` | :obj:`~pyrogram.types.ReplyKeyboardRemove` | :obj:`~pyrogram.types.ForceReply`, *optional*):
                 Additional interface options. An object for an inline keyboard, custom reply keyboard,
                 instructions to remove reply keyboard or to force a reply from the user.
 
@@ -3535,14 +3639,15 @@
             parse_mode=parse_mode,
             caption_entities=caption_entities,
             duration=duration,
             disable_notification=disable_notification,
             protect_content=protect_content,
             message_thread_id=self.message_thread_id,
             business_connection_id=self.business_connection_id,
+            message_effect_id=message_effect_id,
             reply_parameters=reply_parameters,
             reply_markup=reply_markup,
             schedule_date=schedule_date,
             ttl_seconds=ttl_seconds,
             view_once=view_once,
             waveform=waveform,
             reply_to_message_id=reply_to_message_id,
@@ -3886,14 +3991,15 @@
 
     async def copy(
         self,
         chat_id: Union[int, str],
         caption: str = None,
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
+        show_caption_above_media: bool = None,
         disable_notification: bool = None,
         reply_parameters: "types.ReplyParameters" = None,
         reply_markup: Union[
             "types.InlineKeyboardMarkup",
             "types.ReplyKeyboardMarkup",
             "types.ReplyKeyboardRemove",
             "types.ForceReply"
@@ -3935,14 +4041,17 @@
             parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
                 By default, texts are parsed using both Markdown and HTML styles.
                 You can combine both syntaxes together.
 
             caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
                 List of special entities that appear in the new caption, which can be specified instead of *parse_mode*.
 
+            show_caption_above_media (``bool``, *optional*):
+                Pass True, if the caption must be shown above the message media. Ignored if a new caption isn't specified.
+
             disable_notification (``bool``, *optional*):
                 Sends the message silently.
                 Users will receive a notification with no sound.
 
             reply_parameters (:obj:`~pyrogram.types.ReplyParameters`, *optional*):
                 Description of the message to reply to
 
@@ -3985,24 +4094,27 @@
                 business_connection_id=business_connection_id or self.business_connection_id,
                 text=self.text,
                 parse_mode=enums.ParseMode.DISABLED,
                 entities=self.entities,
                 link_preview_options=self.link_preview_options,
                 disable_notification=disable_notification,
                 protect_content=protect_content or self.has_protected_content,
+                message_effect_id=self.effect_id,
                 reply_parameters=reply_parameters,
                 reply_markup=self.reply_markup if reply_markup is object else reply_markup,
                 reply_to_message_id=reply_to_message_id,
                 schedule_date=schedule_date
             )
         elif self.media:
             send_media = partial(
                 self._client.send_cached_media,
                 chat_id=chat_id,
                 disable_notification=disable_notification,
+                message_effect_id=self.effect_id,
+                show_caption_above_media=show_caption_above_media,
                 reply_parameters=reply_parameters,
                 message_thread_id=message_thread_id or self.message_thread_id,
                 business_connection_id=business_connection_id or self.business_connection_id,
                 schedule_date=schedule_date,
                 protect_content=protect_content or self.has_protected_content,
                 has_spoiler=self.has_media_spoiler,
                 reply_to_message_id=reply_to_message_id,
@@ -4029,28 +4141,30 @@
                 return await self._client.send_contact(
                     chat_id,
                     phone_number=self.contact.phone_number,
                     first_name=self.contact.first_name,
                     last_name=self.contact.last_name,
                     vcard=self.contact.vcard,
                     disable_notification=disable_notification,
+                    message_effect_id=self.effect_id,
                     reply_parameters=reply_parameters,
                     message_thread_id=message_thread_id or self.message_thread_id,
                     business_connection_id=business_connection_id or self.business_connection_id,
                     schedule_date=schedule_date,
                     protect_content=protect_content or self.has_protected_content,
                     reply_to_message_id=reply_to_message_id,
                     reply_markup=self.reply_markup if reply_markup is object else reply_markup
                 )
             elif self.location:
                 return await self._client.send_location(
                     chat_id,
                     latitude=self.location.latitude,
                     longitude=self.location.longitude,
                     disable_notification=disable_notification,
+                    message_effect_id=self.effect_id,
                     reply_parameters=reply_parameters,
                     message_thread_id=message_thread_id or self.message_thread_id,
                     business_connection_id=business_connection_id or self.business_connection_id,
                     schedule_date=schedule_date,
                     protect_content=protect_content or self.has_protected_content,
                     reply_to_message_id=reply_to_message_id,
                     reply_markup=self.reply_markup if reply_markup is object else reply_markup
@@ -4061,14 +4175,15 @@
                     latitude=self.venue.location.latitude,
                     longitude=self.venue.location.longitude,
                     title=self.venue.title,
                     address=self.venue.address,
                     foursquare_id=self.venue.foursquare_id,
                     foursquare_type=self.venue.foursquare_type,
                     disable_notification=disable_notification,
+                    message_effect_id=self.effect_id,
                     reply_parameters=reply_parameters,
                     message_thread_id=message_thread_id or self.message_thread_id,
                     business_connection_id=business_connection_id or self.business_connection_id,
                     schedule_date=schedule_date,
                     protect_content=protect_content or self.has_protected_content,
                     reply_to_message_id=reply_to_message_id,
                     reply_markup=self.reply_markup if reply_markup is object else reply_markup
@@ -4090,14 +4205,15 @@
                     correct_option_id=self.poll.correct_option_id,
                     explanation=self.poll.explanation,
                     explanation_entities=self.poll.explanation_entities,
                     open_period=self.poll.open_period,
                     close_date=self.poll.close_date,
                     disable_notification=disable_notification,
                     protect_content=protect_content or self.has_protected_content,
+                    message_effect_id=self.effect_id,
                     reply_parameters=reply_parameters,
                     message_thread_id=message_thread_id or self.message_thread_id,
                     business_connection_id=business_connection_id or self.business_connection_id,
                     schedule_date=schedule_date,
                     reply_to_message_id=reply_to_message_id,
                     reply_markup=self.reply_markup if reply_markup is object else reply_markup
                 )
@@ -4105,14 +4221,15 @@
                 return await self._client.send_game(
                     chat_id,
                     game_short_name=self.game.short_name,
                     disable_notification=disable_notification,
                     protect_content=protect_content or self.has_protected_content,
                     message_thread_id=message_thread_id or self.message_thread_id,
                     business_connection_id=business_connection_id or self.business_connection_id,
+                    message_effect_id=self.effect_id,
                     reply_parameters=reply_parameters,
                     reply_to_message_id=reply_to_message_id,
                     reply_markup=self.reply_markup if reply_markup is object else reply_markup
                 )
             else:
                 raise ValueError("Unknown media type")
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/message_entity.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/message_reaction_count_updated.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/message_reaction_updated.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/message_reactions.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/photo.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/poll.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/poll_option.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/reaction.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/sponsored_message.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/sponsored_message.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/sticker.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/story.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/story.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/thumbnail.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/venue.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/video.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/video_note.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/voice.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/web_app_data.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/messages_and_media/web_page.py` & `pyrotgfork-2.1.32.3/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/__init__.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/birthdate.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/birthdate.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_color.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_color.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_event.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,20 +350,29 @@
 
         elif isinstance(action, raw.types.ChannelAdminLogEventActionDefaultBannedRights):
             old_chat_permissions = types.ChatPermissions._parse(action.prev_banned_rights)
             new_chat_permissions = types.ChatPermissions._parse(action.new_banned_rights)
             action = enums.ChatEventAction.CHAT_PERMISSIONS_CHANGED
 
         elif isinstance(action, raw.types.ChannelAdminLogEventActionDeleteMessage):
-            deleted_message = await types.Message._parse(client, action.message, users, chats)
+            deleted_message = await types.Message._parse(
+                client,
+                action.message,
+                users,
+                chats
+            )
             action = enums.ChatEventAction.MESSAGE_DELETED
 
         elif isinstance(action, raw.types.ChannelAdminLogEventActionEditMessage):
-            old_message = await types.Message._parse(client, action.prev_message, users, chats)
-            new_message = await types.Message._parse(client, action.new_message, users, chats)
+            old_message = await types.Message._parse(
+                client, action.prev_message, users, chats
+            )
+            new_message = await types.Message._parse(
+                client, action.new_message, users, chats
+            )
             action = enums.ChatEventAction.MESSAGE_EDITED
 
         elif isinstance(action, raw.types.ChannelAdminLogEventActionParticipantInvite):
             invited_member = types.ChatMember._parse(client, action.participant, users, chats)
             action = enums.ChatEventAction.MEMBER_INVITED
 
         elif isinstance(action, raw.types.ChannelAdminLogEventActionParticipantToggleAdmin):
@@ -373,15 +382,17 @@
 
         elif isinstance(action, raw.types.ChannelAdminLogEventActionParticipantToggleBan):
             old_member_permissions = types.ChatMember._parse(client, action.prev_participant, users, chats)
             new_member_permissions = types.ChatMember._parse(client, action.new_participant, users, chats)
             action = enums.ChatEventAction.MEMBER_PERMISSIONS_CHANGED
 
         elif isinstance(action, raw.types.ChannelAdminLogEventActionStopPoll):
-            stopped_poll = await types.Message._parse(client, action.message, users, chats)
+            stopped_poll = await types.Message._parse(
+                client, action.message, users, chats
+            )
             action = enums.ChatEventAction.POLL_STOPPED
 
         elif isinstance(action, raw.types.ChannelAdminLogEventActionParticipantJoin):
             action = enums.ChatEventAction.MEMBER_JOINED
 
         elif isinstance(action, raw.types.ChannelAdminLogEventActionParticipantLeave):
             action = enums.ChatEventAction.MEMBER_LEFT
@@ -404,18 +415,22 @@
             action = enums.ChatEventAction.SLOW_MODE_CHANGED
 
         elif isinstance(action, raw.types.ChannelAdminLogEventActionUpdatePinned):
             message = action.message
 
             if isinstance(action.message, raw.types.Message):
                 if message.pinned:
-                    pinned_message = await types.Message._parse(client, message, users, chats)
+                    pinned_message = await types.Message._parse(
+                        client, message, users, chats
+                    )
                     action = enums.ChatEventAction.MESSAGE_PINNED
                 else:
-                    unpinned_message = await types.Message._parse(client, message, users, chats)
+                    unpinned_message = await types.Message._parse(
+                        client, message, users, chats
+                    )
                     action = enums.ChatEventAction.MESSAGE_UNPINNED
 
         elif isinstance(action, raw.types.ChannelAdminLogEventActionExportedInviteEdit):
             old_invite_link = types.ChatInviteLink._parse(client, action.prev_invite, users)
             new_invite_link = types.ChatInviteLink._parse(client, action.new_invite, users)
             action = enums.ChatEventAction.INVITE_LINK_EDITED
```

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_event_filter.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_invite_link.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_join_request.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_joiner.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_member.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_member_updated.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_permissions.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_photo.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_privileges.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_reactions.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/chat_shared.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/chat_shared.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/dialog.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/emoji_status.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/group_call_participant.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/group_call_participant.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/invite_link_importer.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/restriction.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/user.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/username.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/users_shared.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/users_shared.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/video_chat_ended.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/video_chat_participants_invited.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/video_chat_participants_invited.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `pyrotgfork-2.1.32.3/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyrogram/types/user_and_chats/video_chat_started.py` & `pyrotgfork-2.1.32.3/pyrogram/methods/stickers/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,18 +12,16 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from ..object import Object
+from .get_message_effects import GetMessageEffects
+from .get_stickers import GetStickers
 
 
-class VideoChatStarted(Object):
-    """A service message about a voice chat started in the chat.
-
-    Currently holds no information.
-    """
-
-    def __init__(self):
-        super().__init__()
+class Stickers(
+    GetMessageEffects,
+    GetStickers,
+):
+    pass
```

### Comparing `pyrotgfork-2.1.32.2/.gitignore` & `pyrotgfork-2.1.32.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/COPYING` & `pyrotgfork-2.1.32.3/COPYING`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/COPYING.lesser` & `pyrotgfork-2.1.32.3/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/NOTICE` & `pyrotgfork-2.1.32.3/NOTICE`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/README.md` & `pyrotgfork-2.1.32.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/hatch_build.py` & `pyrotgfork-2.1.32.3/hatch_build.py`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/pyproject.toml` & `pyrotgfork-2.1.32.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrotgfork-2.1.32.2/PKG-INFO` & `pyrotgfork-2.1.32.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyrotgfork
-Version: 2.1.32.2
+Version: 2.1.32.3
 Summary: Fork of Pyrogram. Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Project-URL: Homepage, https://telegramplayground.github.io/pyrogram/releases/
 Project-URL: Tracker, https://github.com/TelegramPlayGround/Pyrogram/issues
 Project-URL: Source, https://github.com/TelegramPlayGround/Pyrogram
 Project-URL: Documentation, https://telegramplayground.github.io/pyrogram/
 Author-email: SpEcHIDe <pyrogram@iamidiotareyoutoo.com>
 License-Expression: LGPL-3.0-or-later
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: pyrotgfork Version: 2.1.32.2 Summary: Fork of
+Metadata-Version: 2.3 Name: pyrotgfork Version: 2.1.32.3 Summary: Fork of
 Pyrogram. Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots Project-URL: Homepage, https://
 telegramplayground.github.io/pyrogram/releases/ Project-URL: Tracker, https://
 github.com/TelegramPlayGround/Pyrogram/issues Project-URL: Source, https://
 github.com/TelegramPlayGround/Pyrogram Project-URL: Documentation, https://
 telegramplayground.github.io/pyrogram/ Author-email: SpEcHIDe
 iamidiotareyoutoo.com> License-Expression: LGPL-3.0-or-later License-File:
```

