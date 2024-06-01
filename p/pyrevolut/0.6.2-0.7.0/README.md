# Comparing `tmp/pyrevolut-0.6.2.tar.gz` & `tmp/pyrevolut-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrevolut-0.6.2.tar", max compression
+gzip compressed data, was "pyrevolut-0.7.0.tar", max compression
```

## Comparing `pyrevolut-0.6.2.tar` & `pyrevolut-0.7.0.tar`

### file list

```diff
@@ -1,191 +1,192 @@
--rw-r--r--   0        0        0     1070 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/LICENSE
--rw-r--r--   0        0        0     6350 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/README.md
--rw-r--r--   0        0        0     2906 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/__init__.py
--rw-r--r--   0        0        0      391 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/__init__.py
--rw-r--r--   0        0        0      249 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/accounts/__init__.py
--rw-r--r--   0        0        0      173 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/accounts/endpoint/__init__.py
--rw-r--r--   0        0        0     2550 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/accounts/endpoint/asynchronous.py
--rw-r--r--   0        0        0     2505 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/accounts/endpoint/synchronous.py
--rw-r--r--   0        0        0      244 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/accounts/get/__init__.py
--rw-r--r--   0        0        0      432 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/accounts/get/retrieve_all_accounts.py
--rw-r--r--   0        0        0      489 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/accounts/get/retrieve_an_account.py
--rw-r--r--   0        0        0     4310 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/accounts/get/retrieve_full_bank_details.py
--rw-r--r--   0        0        0      114 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/accounts/resources/__init__.py
--rw-r--r--   0        0        0     1353 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/accounts/resources/account.py
--rw-r--r--   0        0        0      378 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/__init__.py
--rw-r--r--   0        0        0      115 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/delete/__init__.py
--rw-r--r--   0        0        0      468 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/delete/terminate_card.py
--rw-r--r--   0        0        0      164 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/endpoint/__init__.py
--rw-r--r--   0        0        0    21903 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/endpoint/asynchronous.py
--rw-r--r--   0        0        0    21798 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/endpoint/synchronous.py
--rw-r--r--   0        0        0      255 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/get/__init__.py
--rw-r--r--   0        0        0      450 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/get/retrieve_card_details.py
--rw-r--r--   0        0        0     1534 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/get/retrieve_list_of_cards.py
--rw-r--r--   0        0        0      854 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/get/retrieve_sensitive_card_details.py
--rw-r--r--   0        0        0      123 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/patch/__init__.py
--rw-r--r--   0        0        0     5567 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/patch/update_card_details.py
--rw-r--r--   0        0        0      183 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/post/__init__.py
--rw-r--r--   0        0        0     6523 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/post/create_card.py
--rw-r--r--   0        0        0      562 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/post/freeze_card.py
--rw-r--r--   0        0        0      565 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/post/unfreeze_card.py
--rw-r--r--   0        0        0      104 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/resources/__init__.py
--rw-r--r--   0        0        0     3954 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/cards/resources/card.py
--rw-r--r--   0        0        0      191 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/common/__init__.py
--rw-r--r--   0        0        0      741 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/common/endpoint.py
--rw-r--r--   0        0        0     1351 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/common/enums/__init__.py
--rw-r--r--   0        0        0     1046 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/common/enums/account_name_match_code.py
--rw-r--r--   0        0        0     1908 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/common/enums/account_name_match_reason_code.py
--rw-r--r--   0        0        0      232 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/common/enums/account_name_match_reason_type.py
--rw-r--r--   0        0        0      138 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/common/enums/account_state.py
--rw-r--r--   0        0        0      156 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/common/enums/account_type.py
--rw-r--r--   0        0        0      134 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/common/enums/card_scheme.py
--rw-r--r--   0        0        0      205 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/common/enums/card_state.py
--rw-r--r--   0        0        0      176 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/common/enums/charge_bearer.py
--rw-r--r--   0        0        0      651 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/common/enums/merchant_category.py
--rw-r--r--   0        0        0      313 2024-05-20 13:21:01.511818 pyrevolut-0.6.2/pyrevolut/api/common/enums/payment_draft_state.py
--rw-r--r--   0        0        0      336 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/enums/payment_scheme.py
--rw-r--r--   0        0        0      345 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/enums/payout_link_cancellation_reason.py
--rw-r--r--   0        0        0      443 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/enums/payout_link_payment_method.py
--rw-r--r--   0        0        0     1061 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/enums/payout_link_state.py
--rw-r--r--   0        0        0      162 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/enums/profile_state.py
--rw-r--r--   0        0        0      140 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/enums/profile_type.py
--rw-r--r--   0        0        0      138 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/enums/recipient_charges.py
--rw-r--r--   0        0        0      226 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/enums/simulate_transfer_state_action.py
--rw-r--r--   0        0        0      247 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/enums/team_member_state.py
--rw-r--r--   0        0        0      120 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/enums/time_unit.py
--rw-r--r--   0        0        0     1251 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/enums/transaction_state.py
--rw-r--r--   0        0        0      489 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/enums/transaction_type.py
--rw-r--r--   0        0        0     1093 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/enums/transfer_reason_code.py
--rw-r--r--   0        0        0      318 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/enums/webhook_event.py
--rw-r--r--   0        0        0      126 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/models/__init__.py
--rw-r--r--   0        0        0      386 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/common/models/amount.py
--rw-r--r--   0        0        0      772 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/counterparties/__init__.py
--rw-r--r--   0        0        0      135 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/counterparties/delete/__init__.py
--rw-r--r--   0        0        0      474 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/counterparties/delete/delete_counterparty.py
--rw-r--r--   0        0        0      191 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/counterparties/endpoint/__init__.py
--rw-r--r--   0        0        0    14383 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/counterparties/endpoint/asynchronous.py
--rw-r--r--   0        0        0    14313 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/counterparties/endpoint/synchronous.py
--rw-r--r--   0        0        0      210 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/counterparties/get/__init__.py
--rw-r--r--   0        0        0      485 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/counterparties/get/retrieve_counterparty.py
--rw-r--r--   0        0        0     3888 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/counterparties/get/retrieve_list_of_counterparties.py
--rw-r--r--   0        0        0      188 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/counterparties/post/__init__.py
--rw-r--r--   0        0        0     8872 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/counterparties/post/create_counterparty.py
--rw-r--r--   0        0        0     8378 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/counterparties/post/validate_account_name.py
--rw-r--r--   0        0        0      130 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/counterparties/resources/__init__.py
--rw-r--r--   0        0        0     5381 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/counterparties/resources/counterparty.py
--rw-r--r--   0        0        0      271 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/foreign_exchange/__init__.py
--rw-r--r--   0        0        0      195 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/foreign_exchange/endpoint/__init__.py
--rw-r--r--   0        0        0     4364 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/foreign_exchange/endpoint/asynchronous.py
--rw-r--r--   0        0        0     4331 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/foreign_exchange/endpoint/synchronous.py
--rw-r--r--   0        0        0      129 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/foreign_exchange/get/__init__.py
--rw-r--r--   0        0        0     1231 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/foreign_exchange/get/get_exchange_rate.py
--rw-r--r--   0        0        0      125 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/foreign_exchange/post/__init__.py
--rw-r--r--   0        0        0     6574 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/foreign_exchange/post/exchange_money.py
--rw-r--r--   0        0        0      139 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/foreign_exchange/resources/__init__.py
--rw-r--r--   0        0        0     1158 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/foreign_exchange/resources/foreign_exchange.py
--rw-r--r--   0        0        0      475 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payment_drafts/__init__.py
--rw-r--r--   0        0        0      136 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payment_drafts/delete/__init__.py
--rw-r--r--   0        0        0      462 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payment_drafts/delete/delete_payment_draft.py
--rw-r--r--   0        0        0      189 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payment_drafts/endpoint/__init__.py
--rw-r--r--   0        0        0     6986 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payment_drafts/endpoint/asynchronous.py
--rw-r--r--   0        0        0     6929 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payment_drafts/endpoint/synchronous.py
--rw-r--r--   0        0        0      203 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payment_drafts/get/__init__.py
--rw-r--r--   0        0        0     1328 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payment_drafts/get/retrieve_all_payment_drafts.py
--rw-r--r--   0        0        0     6034 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payment_drafts/get/retrieve_payment_draft.py
--rw-r--r--   0        0        0      134 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payment_drafts/post/__init__.py
--rw-r--r--   0        0        0     3944 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payment_drafts/post/create_payment_draft.py
--rw-r--r--   0        0        0      331 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payout_links/__init__.py
--rw-r--r--   0        0        0      183 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payout_links/endpoint/__init__.py
--rw-r--r--   0        0        0     9350 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payout_links/endpoint/asynchronous.py
--rw-r--r--   0        0        0     9436 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payout_links/endpoint/synchronous.py
--rw-r--r--   0        0        0      200 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payout_links/get/__init__.py
--rw-r--r--   0        0        0     3198 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payout_links/get/retrieve_list_of_payout_links.py
--rw-r--r--   0        0        0      560 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payout_links/get/retrieve_payout_link.py
--rw-r--r--   0        0        0      177 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payout_links/post/__init__.py
--rw-r--r--   0        0        0      580 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payout_links/post/cancel_payout_link.py
--rw-r--r--   0        0        0     4911 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payout_links/post/create_payout_link.py
--rw-r--r--   0        0        0      125 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payout_links/resources/__init__.py
--rw-r--r--   0        0        0     5949 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/payout_links/resources/payout_link.py
--rw-r--r--   0        0        0      398 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/simulations/__init__.py
--rw-r--r--   0        0        0      182 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/simulations/endpoint/__init__.py
--rw-r--r--   0        0        0     4995 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/simulations/endpoint/asynchronous.py
--rw-r--r--   0        0        0     4962 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/simulations/endpoint/synchronous.py
--rw-r--r--   0        0        0      206 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/simulations/post/__init__.py
--rw-r--r--   0        0        0     4930 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/simulations/post/simulate_account_topup.py
--rw-r--r--   0        0        0     2195 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/simulations/post/simulate_transfer_state_update.py
--rw-r--r--   0        0        0      363 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/team_members/__init__.py
--rw-r--r--   0        0        0      183 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/team_members/endpoint/__init__.py
--rw-r--r--   0        0        0     5782 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/team_members/endpoint/asynchronous.py
--rw-r--r--   0        0        0     5737 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/team_members/endpoint/synchronous.py
--rw-r--r--   0        0        0      198 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/team_members/get/__init__.py
--rw-r--r--   0        0        0     2852 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/team_members/get/retrieve_list_of_team_members.py
--rw-r--r--   0        0        0     2218 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/team_members/get/retrieve_team_roles.py
--rw-r--r--   0        0        0      128 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/team_members/post/__init__.py
--rw-r--r--   0        0        0     1670 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/team_members/post/invite_team_member.py
--rw-r--r--   0        0        0      291 2024-05-20 13:21:01.515818 pyrevolut-0.6.2/pyrevolut/api/transactions/__init__.py
--rw-r--r--   0        0        0      185 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transactions/endpoint/__init__.py
--rw-r--r--   0        0        0     5902 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transactions/endpoint/asynchronous.py
--rw-r--r--   0        0        0     5869 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transactions/endpoint/synchronous.py
--rw-r--r--   0        0        0      202 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transactions/get/__init__.py
--rw-r--r--   0        0        0     3868 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transactions/get/retrieve_list_of_transactions.py
--rw-r--r--   0        0        0     1393 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transactions/get/retrieve_transaction.py
--rw-r--r--   0        0        0      126 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transactions/resources/__init__.py
--rw-r--r--   0        0        0     6725 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transactions/resources/transaction.py
--rw-r--r--   0        0        0      276 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transfers/__init__.py
--rw-r--r--   0        0        0      176 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transfers/endpoint/__init__.py
--rw-r--r--   0        0        0     8101 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transfers/endpoint/asynchronous.py
--rw-r--r--   0        0        0     8056 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transfers/endpoint/synchronous.py
--rw-r--r--   0        0        0      128 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transfers/get/__init__.py
--rw-r--r--   0        0        0     1804 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transfers/get/get_transfer_reasons.py
--rw-r--r--   0        0        0      221 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transfers/post/__init__.py
--rw-r--r--   0        0        0     5738 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transfers/post/create_transfer_to_another_account.py
--rw-r--r--   0        0        0     2090 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transfers/post/move_money_between_accounts.py
--rw-r--r--   0        0        0      117 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transfers/resources/__init__.py
--rw-r--r--   0        0        0     1897 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/transfers/resources/transfer.py
--rw-r--r--   0        0        0      666 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/__init__.py
--rw-r--r--   0        0        0      119 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/delete/__init__.py
--rw-r--r--   0        0        0      429 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/delete/delete_webhook.py
--rw-r--r--   0        0        0      173 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/endpoint/__init__.py
--rw-r--r--   0        0        0     9270 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/endpoint/asynchronous.py
--rw-r--r--   0        0        0     9177 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/endpoint/synchronous.py
--rw-r--r--   0        0        0      257 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/get/__init__.py
--rw-r--r--   0        0        0     3139 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/get/retrieve_list_of_failed_webhooks.py
--rw-r--r--   0        0        0      470 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/get/retrieve_list_of_webhooks.py
--rw-r--r--   0        0        0      691 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/get/retrieve_webhook.py
--rw-r--r--   0        0        0      118 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/patch/__init__.py
--rw-r--r--   0        0        0     1228 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/patch/update_webhook.py
--rw-r--r--   0        0        0      172 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/post/__init__.py
--rw-r--r--   0        0        0     1531 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/post/create_webhook.py
--rw-r--r--   0        0        0     1252 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/post/rotate_webhook_secret.py
--rw-r--r--   0        0        0      426 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/resources/__init__.py
--rw-r--r--   0        0        0      589 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/resources/payout_link_created.py
--rw-r--r--   0        0        0      738 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/resources/payout_link_state_changed.py
--rw-r--r--   0        0        0     4801 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/resources/transaction_created.py
--rw-r--r--   0        0        0      737 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/resources/transaction_state_changed.py
--rw-r--r--   0        0        0      633 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/resources/webhook.py
--rw-r--r--   0        0        0      937 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/api/webhooks/resources/webhook_payload.py
--rw-r--r--   0        0        0       71 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/cli/__init__.py
--rw-r--r--   0        0        0       50 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/cli/__main__.py
--rw-r--r--   0        0        0     2498 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/cli/main.py
--rw-r--r--   0        0        0      195 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/client/__init__.py
--rw-r--r--   0        0        0     7416 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/client/asynchronous.py
--rw-r--r--   0        0        0    19996 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/client/base.py
--rw-r--r--   0        0        0     7217 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/client/synchronous.py
--rw-r--r--   0        0        0      312 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/exceptions/__init__.py
--rw-r--r--   0        0        0      177 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/exceptions/bad_request.py
--rw-r--r--   0        0        0      105 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/exceptions/common.py
--rw-r--r--   0        0        0      241 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/exceptions/internal_revolut_error.py
--rw-r--r--   0        0        0      161 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/exceptions/invalid_environment.py
--rw-r--r--   0        0        0       75 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/utils/__init__.py
--rw-r--r--   0        0        0      452 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/utils/auth/__init__.py
--rw-r--r--   0        0        0    10702 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/utils/auth/auth_manual.py
--rw-r--r--   0        0        0     2630 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/utils/auth/create_client_assert_jwt.py
--rw-r--r--   0        0        0     5204 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/utils/auth/creds.py
--rw-r--r--   0        0        0      858 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/utils/auth/enum_auth_scope.py
--rw-r--r--   0        0        0     4409 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/utils/auth/gen_public_private_cert.py
--rw-r--r--   0        0        0     3346 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/utils/auth/get_auth_tokens.py
--rw-r--r--   0        0        0     3273 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/utils/auth/refresh_access_token.py
--rw-r--r--   0        0        0     3038 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/utils/date.py
--rw-r--r--   0        0        0     4162 2024-05-20 13:21:01.519818 pyrevolut-0.6.2/pyrevolut/utils/datetime.py
--rw-r--r--   0        0        0     7218 1970-01-01 00:00:00.000000 pyrevolut-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-06-01 13:49:29.114070 pyrevolut-0.7.0/LICENSE
+-rw-r--r--   0        0        0     6350 2024-06-01 13:49:29.114070 pyrevolut-0.7.0/README.md
+-rw-r--r--   0        0        0     2962 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/__init__.py
+-rw-r--r--   0        0        0      391 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/__init__.py
+-rw-r--r--   0        0        0      249 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/__init__.py
+-rw-r--r--   0        0        0      173 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/endpoint/__init__.py
+-rw-r--r--   0        0        0     2550 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     2505 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/endpoint/synchronous.py
+-rw-r--r--   0        0        0      244 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/get/__init__.py
+-rw-r--r--   0        0        0      432 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/get/retrieve_all_accounts.py
+-rw-r--r--   0        0        0      489 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/get/retrieve_an_account.py
+-rw-r--r--   0        0        0     4310 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/get/retrieve_full_bank_details.py
+-rw-r--r--   0        0        0      114 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/resources/__init__.py
+-rw-r--r--   0        0        0     1353 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/resources/account.py
+-rw-r--r--   0        0        0      378 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/__init__.py
+-rw-r--r--   0        0        0      115 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/delete/__init__.py
+-rw-r--r--   0        0        0      468 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/delete/terminate_card.py
+-rw-r--r--   0        0        0      164 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/endpoint/__init__.py
+-rw-r--r--   0        0        0    21903 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/endpoint/asynchronous.py
+-rw-r--r--   0        0        0    21798 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/endpoint/synchronous.py
+-rw-r--r--   0        0        0      255 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/get/__init__.py
+-rw-r--r--   0        0        0      450 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/get/retrieve_card_details.py
+-rw-r--r--   0        0        0     1534 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/get/retrieve_list_of_cards.py
+-rw-r--r--   0        0        0      854 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/get/retrieve_sensitive_card_details.py
+-rw-r--r--   0        0        0      123 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/patch/__init__.py
+-rw-r--r--   0        0        0     5567 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/patch/update_card_details.py
+-rw-r--r--   0        0        0      183 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/post/__init__.py
+-rw-r--r--   0        0        0     6523 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/post/create_card.py
+-rw-r--r--   0        0        0      562 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/post/freeze_card.py
+-rw-r--r--   0        0        0      565 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/post/unfreeze_card.py
+-rw-r--r--   0        0        0      104 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/resources/__init__.py
+-rw-r--r--   0        0        0     3954 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/resources/card.py
+-rw-r--r--   0        0        0      191 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/common/__init__.py
+-rw-r--r--   0        0        0      741 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/common/endpoint.py
+-rw-r--r--   0        0        0     1351 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/__init__.py
+-rw-r--r--   0        0        0     1046 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/account_name_match_code.py
+-rw-r--r--   0        0        0     1908 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/account_name_match_reason_code.py
+-rw-r--r--   0        0        0      232 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/account_name_match_reason_type.py
+-rw-r--r--   0        0        0      138 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/account_state.py
+-rw-r--r--   0        0        0      156 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/account_type.py
+-rw-r--r--   0        0        0      134 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/card_scheme.py
+-rw-r--r--   0        0        0      205 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/card_state.py
+-rw-r--r--   0        0        0      176 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/charge_bearer.py
+-rw-r--r--   0        0        0      651 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/merchant_category.py
+-rw-r--r--   0        0        0      313 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/payment_draft_state.py
+-rw-r--r--   0        0        0      336 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/payment_scheme.py
+-rw-r--r--   0        0        0      345 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/payout_link_cancellation_reason.py
+-rw-r--r--   0        0        0      443 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/payout_link_payment_method.py
+-rw-r--r--   0        0        0     1061 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/payout_link_state.py
+-rw-r--r--   0        0        0      162 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/profile_state.py
+-rw-r--r--   0        0        0      140 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/profile_type.py
+-rw-r--r--   0        0        0      138 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/recipient_charges.py
+-rw-r--r--   0        0        0      226 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/simulate_transfer_state_action.py
+-rw-r--r--   0        0        0      247 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/team_member_state.py
+-rw-r--r--   0        0        0      120 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/time_unit.py
+-rw-r--r--   0        0        0     1251 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/transaction_state.py
+-rw-r--r--   0        0        0      489 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/transaction_type.py
+-rw-r--r--   0        0        0     1093 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/transfer_reason_code.py
+-rw-r--r--   0        0        0      318 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/webhook_event.py
+-rw-r--r--   0        0        0      126 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/models/__init__.py
+-rw-r--r--   0        0        0      386 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/models/amount.py
+-rw-r--r--   0        0        0      772 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/__init__.py
+-rw-r--r--   0        0        0      135 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/delete/__init__.py
+-rw-r--r--   0        0        0      474 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/delete/delete_counterparty.py
+-rw-r--r--   0        0        0      191 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/endpoint/__init__.py
+-rw-r--r--   0        0        0    14383 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/endpoint/asynchronous.py
+-rw-r--r--   0        0        0    14313 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/endpoint/synchronous.py
+-rw-r--r--   0        0        0      210 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/get/__init__.py
+-rw-r--r--   0        0        0      485 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/get/retrieve_counterparty.py
+-rw-r--r--   0        0        0     3888 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/get/retrieve_list_of_counterparties.py
+-rw-r--r--   0        0        0      188 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/post/__init__.py
+-rw-r--r--   0        0        0     8872 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/post/create_counterparty.py
+-rw-r--r--   0        0        0     8378 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/post/validate_account_name.py
+-rw-r--r--   0        0        0      130 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/resources/__init__.py
+-rw-r--r--   0        0        0     5381 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/resources/counterparty.py
+-rw-r--r--   0        0        0      271 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/__init__.py
+-rw-r--r--   0        0        0      195 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/endpoint/__init__.py
+-rw-r--r--   0        0        0     4364 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     4331 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/endpoint/synchronous.py
+-rw-r--r--   0        0        0      129 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/get/__init__.py
+-rw-r--r--   0        0        0     1231 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/get/get_exchange_rate.py
+-rw-r--r--   0        0        0      125 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/post/__init__.py
+-rw-r--r--   0        0        0     6574 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/post/exchange_money.py
+-rw-r--r--   0        0        0      139 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/resources/__init__.py
+-rw-r--r--   0        0        0     1158 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/resources/foreign_exchange.py
+-rw-r--r--   0        0        0      475 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/__init__.py
+-rw-r--r--   0        0        0      136 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/delete/__init__.py
+-rw-r--r--   0        0        0      462 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/delete/delete_payment_draft.py
+-rw-r--r--   0        0        0      189 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/endpoint/__init__.py
+-rw-r--r--   0        0        0     6986 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     6929 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/endpoint/synchronous.py
+-rw-r--r--   0        0        0      203 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/get/__init__.py
+-rw-r--r--   0        0        0     1328 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/get/retrieve_all_payment_drafts.py
+-rw-r--r--   0        0        0     6034 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/get/retrieve_payment_draft.py
+-rw-r--r--   0        0        0      134 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/post/__init__.py
+-rw-r--r--   0        0        0     3944 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/post/create_payment_draft.py
+-rw-r--r--   0        0        0      331 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/__init__.py
+-rw-r--r--   0        0        0      183 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/endpoint/__init__.py
+-rw-r--r--   0        0        0     9350 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     9436 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/endpoint/synchronous.py
+-rw-r--r--   0        0        0      200 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/get/__init__.py
+-rw-r--r--   0        0        0     3198 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/get/retrieve_list_of_payout_links.py
+-rw-r--r--   0        0        0      560 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/get/retrieve_payout_link.py
+-rw-r--r--   0        0        0      177 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/post/__init__.py
+-rw-r--r--   0        0        0      580 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/post/cancel_payout_link.py
+-rw-r--r--   0        0        0     4911 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/post/create_payout_link.py
+-rw-r--r--   0        0        0      125 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/resources/__init__.py
+-rw-r--r--   0        0        0     5949 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/resources/payout_link.py
+-rw-r--r--   0        0        0      398 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/simulations/__init__.py
+-rw-r--r--   0        0        0      182 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/simulations/endpoint/__init__.py
+-rw-r--r--   0        0        0     4995 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/simulations/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     4962 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/simulations/endpoint/synchronous.py
+-rw-r--r--   0        0        0      206 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/simulations/post/__init__.py
+-rw-r--r--   0        0        0     4930 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/simulations/post/simulate_account_topup.py
+-rw-r--r--   0        0        0     2195 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/simulations/post/simulate_transfer_state_update.py
+-rw-r--r--   0        0        0      363 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/__init__.py
+-rw-r--r--   0        0        0      183 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/endpoint/__init__.py
+-rw-r--r--   0        0        0     5782 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     5737 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/endpoint/synchronous.py
+-rw-r--r--   0        0        0      198 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/get/__init__.py
+-rw-r--r--   0        0        0     2852 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/get/retrieve_list_of_team_members.py
+-rw-r--r--   0        0        0     2218 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/get/retrieve_team_roles.py
+-rw-r--r--   0        0        0      128 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/post/__init__.py
+-rw-r--r--   0        0        0     1670 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/post/invite_team_member.py
+-rw-r--r--   0        0        0      291 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/__init__.py
+-rw-r--r--   0        0        0      185 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/endpoint/__init__.py
+-rw-r--r--   0        0        0     5902 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     5869 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/endpoint/synchronous.py
+-rw-r--r--   0        0        0      202 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/get/__init__.py
+-rw-r--r--   0        0        0     3868 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/get/retrieve_list_of_transactions.py
+-rw-r--r--   0        0        0     1393 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/get/retrieve_transaction.py
+-rw-r--r--   0        0        0      126 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/resources/__init__.py
+-rw-r--r--   0        0        0     6725 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/resources/transaction.py
+-rw-r--r--   0        0        0      276 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transfers/__init__.py
+-rw-r--r--   0        0        0      176 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transfers/endpoint/__init__.py
+-rw-r--r--   0        0        0     8101 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     8056 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/endpoint/synchronous.py
+-rw-r--r--   0        0        0      128 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/get/__init__.py
+-rw-r--r--   0        0        0     1804 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/get/get_transfer_reasons.py
+-rw-r--r--   0        0        0      221 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/post/__init__.py
+-rw-r--r--   0        0        0     5738 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/post/create_transfer_to_another_account.py
+-rw-r--r--   0        0        0     2090 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/post/move_money_between_accounts.py
+-rw-r--r--   0        0        0      117 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/resources/__init__.py
+-rw-r--r--   0        0        0     1897 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/resources/transfer.py
+-rw-r--r--   0        0        0      666 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/__init__.py
+-rw-r--r--   0        0        0      119 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/delete/__init__.py
+-rw-r--r--   0        0        0      429 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/delete/delete_webhook.py
+-rw-r--r--   0        0        0      173 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/endpoint/__init__.py
+-rw-r--r--   0        0        0     9281 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     1494 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/endpoint/base.py
+-rw-r--r--   0        0        0     9190 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/endpoint/synchronous.py
+-rw-r--r--   0        0        0      257 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/get/__init__.py
+-rw-r--r--   0        0        0     3139 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/get/retrieve_list_of_failed_webhooks.py
+-rw-r--r--   0        0        0      470 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/get/retrieve_list_of_webhooks.py
+-rw-r--r--   0        0        0      691 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/get/retrieve_webhook.py
+-rw-r--r--   0        0        0      118 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/patch/__init__.py
+-rw-r--r--   0        0        0     1228 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/patch/update_webhook.py
+-rw-r--r--   0        0        0      172 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/post/__init__.py
+-rw-r--r--   0        0        0     1531 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/post/create_webhook.py
+-rw-r--r--   0        0        0     1252 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/post/rotate_webhook_secret.py
+-rw-r--r--   0        0        0      426 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/__init__.py
+-rw-r--r--   0        0        0      589 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/payout_link_created.py
+-rw-r--r--   0        0        0      738 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/payout_link_state_changed.py
+-rw-r--r--   0        0        0     4801 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/transaction_created.py
+-rw-r--r--   0        0        0      737 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/transaction_state_changed.py
+-rw-r--r--   0        0        0      633 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/webhook.py
+-rw-r--r--   0        0        0      937 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/webhook_payload.py
+-rw-r--r--   0        0        0       71 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/cli/__init__.py
+-rw-r--r--   0        0        0       50 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/cli/__main__.py
+-rw-r--r--   0        0        0     2498 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/cli/main.py
+-rw-r--r--   0        0        0      195 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/client/__init__.py
+-rw-r--r--   0        0        0     7406 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/client/asynchronous.py
+-rw-r--r--   0        0        0    19986 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/client/base.py
+-rw-r--r--   0        0        0     7207 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/client/synchronous.py
+-rw-r--r--   0        0        0      312 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/exceptions/__init__.py
+-rw-r--r--   0        0        0      177 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/exceptions/bad_request.py
+-rw-r--r--   0        0        0      105 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/exceptions/common.py
+-rw-r--r--   0        0        0      241 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/exceptions/internal_revolut_error.py
+-rw-r--r--   0        0        0      161 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/exceptions/invalid_environment.py
+-rw-r--r--   0        0        0       75 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/utils/__init__.py
+-rw-r--r--   0        0        0      452 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/utils/auth/__init__.py
+-rw-r--r--   0        0        0    10702 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/utils/auth/auth_manual.py
+-rw-r--r--   0        0        0     2630 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/utils/auth/create_client_assert_jwt.py
+-rw-r--r--   0        0        0     5204 2024-06-01 13:49:29.134070 pyrevolut-0.7.0/pyrevolut/utils/auth/creds.py
+-rw-r--r--   0        0        0      858 2024-06-01 13:49:29.134070 pyrevolut-0.7.0/pyrevolut/utils/auth/enum_auth_scope.py
+-rw-r--r--   0        0        0     4409 2024-06-01 13:49:29.134070 pyrevolut-0.7.0/pyrevolut/utils/auth/gen_public_private_cert.py
+-rw-r--r--   0        0        0     3346 2024-06-01 13:49:29.134070 pyrevolut-0.7.0/pyrevolut/utils/auth/get_auth_tokens.py
+-rw-r--r--   0        0        0     3273 2024-06-01 13:49:29.134070 pyrevolut-0.7.0/pyrevolut/utils/auth/refresh_access_token.py
+-rw-r--r--   0        0        0     3269 2024-06-01 13:49:29.134070 pyrevolut-0.7.0/pyrevolut/utils/date.py
+-rw-r--r--   0        0        0     4391 2024-06-01 13:49:29.134070 pyrevolut-0.7.0/pyrevolut/utils/datetime.py
+-rw-r--r--   0        0        0     7218 1970-01-01 00:00:00.000000 pyrevolut-0.7.0/PKG-INFO
```

### Comparing `pyrevolut-0.6.2/LICENSE` & `pyrevolut-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/README.md` & `pyrevolut-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyproject.toml` & `pyrevolut-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyrevolut"
-version = "0.6.2"
+version = "0.7.0"
 description = "An unofficial Python API Wrapper for the Revolut Business API"
 authors = ["Trevor Visser <trevor.visser@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/Trevypants/pyrevolut"
 readme = "README.md"
 
 [tool.poetry.scripts]
@@ -41,14 +41,15 @@
 pytest-randomly = "3.*"
 pytest-clarity = "1.*"
 pytest-split = "0.*"
 pytest-env = "1.*"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "9.*"
+mkdocstrings = { extras = ["python"], version = "0.*" }
 
 [tool.pytest.ini_options]
 pythonpath = ["."]
 filterwarnings = []
 addopts = "--instafail -vv"
 env = ["TEST_MODE=True"]
 asyncio_mode = "auto"
@@ -108,15 +109,15 @@
 docstring-code-format = true
 
 [tool.ruff.lint.isort]
 known-first-party = ["pyrevolut", "tests"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.6.2"
+version = "0.7.0"
 tag_format = "v$major.$minor.$patch$prerelease"
 version_scheme = "pep440"
 version_provider = "poetry"
 update_changelog_on_bump = true
 major_version_zero = true
 version_files = ["pyrevolut/__init__.py:__version__", "pyproject.toml:^version"]
```

### Comparing `pyrevolut-0.6.2/pyrevolut/api/accounts/endpoint/asynchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/accounts/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/accounts/endpoint/synchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/accounts/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/accounts/get/retrieve_full_bank_details.py` & `pyrevolut-0.7.0/pyrevolut/api/accounts/get/retrieve_full_bank_details.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/accounts/resources/account.py` & `pyrevolut-0.7.0/pyrevolut/api/accounts/resources/account.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/cards/endpoint/asynchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/cards/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/cards/endpoint/synchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/cards/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/cards/get/retrieve_list_of_cards.py` & `pyrevolut-0.7.0/pyrevolut/api/cards/get/retrieve_list_of_cards.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/cards/get/retrieve_sensitive_card_details.py` & `pyrevolut-0.7.0/pyrevolut/api/cards/get/retrieve_sensitive_card_details.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/cards/patch/update_card_details.py` & `pyrevolut-0.7.0/pyrevolut/api/cards/patch/update_card_details.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/cards/post/create_card.py` & `pyrevolut-0.7.0/pyrevolut/api/cards/post/create_card.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/cards/post/freeze_card.py` & `pyrevolut-0.7.0/pyrevolut/api/cards/post/freeze_card.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/cards/post/unfreeze_card.py` & `pyrevolut-0.7.0/pyrevolut/api/cards/post/unfreeze_card.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/cards/resources/card.py` & `pyrevolut-0.7.0/pyrevolut/api/cards/resources/card.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/common/endpoint.py` & `pyrevolut-0.7.0/pyrevolut/api/common/endpoint.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/common/enums/__init__.py` & `pyrevolut-0.7.0/pyrevolut/api/common/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/common/enums/account_name_match_code.py` & `pyrevolut-0.7.0/pyrevolut/api/common/enums/account_name_match_code.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/common/enums/account_name_match_reason_code.py` & `pyrevolut-0.7.0/pyrevolut/api/common/enums/account_name_match_reason_code.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/common/enums/merchant_category.py` & `pyrevolut-0.7.0/pyrevolut/api/common/enums/merchant_category.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/common/enums/payout_link_state.py` & `pyrevolut-0.7.0/pyrevolut/api/common/enums/payout_link_state.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/common/enums/transaction_state.py` & `pyrevolut-0.7.0/pyrevolut/api/common/enums/transaction_state.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/common/enums/transfer_reason_code.py` & `pyrevolut-0.7.0/pyrevolut/api/common/enums/transfer_reason_code.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/counterparties/__init__.py` & `pyrevolut-0.7.0/pyrevolut/api/counterparties/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/counterparties/endpoint/asynchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/counterparties/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/counterparties/endpoint/synchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/counterparties/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/counterparties/get/retrieve_list_of_counterparties.py` & `pyrevolut-0.7.0/pyrevolut/api/counterparties/get/retrieve_list_of_counterparties.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/counterparties/post/create_counterparty.py` & `pyrevolut-0.7.0/pyrevolut/api/counterparties/post/create_counterparty.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/counterparties/post/validate_account_name.py` & `pyrevolut-0.7.0/pyrevolut/api/counterparties/post/validate_account_name.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/counterparties/resources/counterparty.py` & `pyrevolut-0.7.0/pyrevolut/api/counterparties/resources/counterparty.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/foreign_exchange/endpoint/asynchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/foreign_exchange/endpoint/synchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/foreign_exchange/get/get_exchange_rate.py` & `pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/get/get_exchange_rate.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/foreign_exchange/post/exchange_money.py` & `pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/post/exchange_money.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/foreign_exchange/resources/foreign_exchange.py` & `pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/resources/foreign_exchange.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/payment_drafts/endpoint/asynchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/payment_drafts/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/payment_drafts/endpoint/synchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/payment_drafts/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/payment_drafts/get/retrieve_all_payment_drafts.py` & `pyrevolut-0.7.0/pyrevolut/api/payment_drafts/get/retrieve_all_payment_drafts.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/payment_drafts/get/retrieve_payment_draft.py` & `pyrevolut-0.7.0/pyrevolut/api/payment_drafts/get/retrieve_payment_draft.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/payment_drafts/post/create_payment_draft.py` & `pyrevolut-0.7.0/pyrevolut/api/payment_drafts/post/create_payment_draft.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/payout_links/endpoint/asynchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/payout_links/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/payout_links/endpoint/synchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/payout_links/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/payout_links/get/retrieve_list_of_payout_links.py` & `pyrevolut-0.7.0/pyrevolut/api/payout_links/get/retrieve_list_of_payout_links.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/payout_links/get/retrieve_payout_link.py` & `pyrevolut-0.7.0/pyrevolut/api/payout_links/get/retrieve_payout_link.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/payout_links/post/cancel_payout_link.py` & `pyrevolut-0.7.0/pyrevolut/api/payout_links/post/cancel_payout_link.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/payout_links/post/create_payout_link.py` & `pyrevolut-0.7.0/pyrevolut/api/payout_links/post/create_payout_link.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/payout_links/resources/payout_link.py` & `pyrevolut-0.7.0/pyrevolut/api/payout_links/resources/payout_link.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/simulations/endpoint/asynchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/simulations/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/simulations/endpoint/synchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/simulations/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/simulations/post/simulate_account_topup.py` & `pyrevolut-0.7.0/pyrevolut/api/simulations/post/simulate_account_topup.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/simulations/post/simulate_transfer_state_update.py` & `pyrevolut-0.7.0/pyrevolut/api/simulations/post/simulate_transfer_state_update.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/team_members/endpoint/asynchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/team_members/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/team_members/endpoint/synchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/team_members/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/team_members/get/retrieve_list_of_team_members.py` & `pyrevolut-0.7.0/pyrevolut/api/team_members/get/retrieve_list_of_team_members.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/team_members/get/retrieve_team_roles.py` & `pyrevolut-0.7.0/pyrevolut/api/team_members/get/retrieve_team_roles.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/team_members/post/invite_team_member.py` & `pyrevolut-0.7.0/pyrevolut/api/team_members/post/invite_team_member.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/transactions/endpoint/asynchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/transactions/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/transactions/endpoint/synchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/transactions/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/transactions/get/retrieve_list_of_transactions.py` & `pyrevolut-0.7.0/pyrevolut/api/transactions/get/retrieve_list_of_transactions.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/transactions/get/retrieve_transaction.py` & `pyrevolut-0.7.0/pyrevolut/api/transactions/get/retrieve_transaction.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/transactions/resources/transaction.py` & `pyrevolut-0.7.0/pyrevolut/api/transactions/resources/transaction.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/transfers/endpoint/asynchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/transfers/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/transfers/endpoint/synchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/transfers/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/transfers/get/get_transfer_reasons.py` & `pyrevolut-0.7.0/pyrevolut/api/transfers/get/get_transfer_reasons.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/transfers/post/create_transfer_to_another_account.py` & `pyrevolut-0.7.0/pyrevolut/api/transfers/post/create_transfer_to_another_account.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/transfers/post/move_money_between_accounts.py` & `pyrevolut-0.7.0/pyrevolut/api/transfers/post/move_money_between_accounts.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/transfers/resources/transfer.py` & `pyrevolut-0.7.0/pyrevolut/api/transfers/resources/transfer.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/webhooks/__init__.py` & `pyrevolut-0.7.0/pyrevolut/api/webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/webhooks/endpoint/asynchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/webhooks/endpoint/asynchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from uuid import UUID
 from datetime import datetime
 
 from pydantic_extra_types.pendulum_dt import Duration
 
 from pyrevolut.utils import DateTime
-from pyrevolut.api.common import (
-    BaseEndpointAsync,
-    EnumWebhookEvent,
-)
+from pyrevolut.api.common import EnumWebhookEvent
 
 from pyrevolut.api.webhooks.get import (
     RetrieveListOfWebhooks,
     RetrieveWebhook,
     RetrieveListOfFailedWebhooks,
 )
 from pyrevolut.api.webhooks.post import CreateWebhook, RotateWebhookSecret
 from pyrevolut.api.webhooks.patch import UpdateWebhook
 from pyrevolut.api.webhooks.delete import DeleteWebhook
 
+from .base import BaseEndpointWebhooks
+
 
-class EndpointWebhooksAsync(BaseEndpointAsync):
+class EndpointWebhooksAsync(BaseEndpointWebhooks):
     """The async Webhooks API
 
     A webhook (also called a web callback) allows your system to receive
     updates about your account to an HTTPS endpoint that you provide.
     When a supported event occurs, a notification is posted via HTTP POST method
     to the specified endpoint.
```

### Comparing `pyrevolut-0.6.2/pyrevolut/api/webhooks/endpoint/synchronous.py` & `pyrevolut-0.7.0/pyrevolut/api/webhooks/endpoint/synchronous.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from uuid import UUID
 from datetime import datetime
 
 from pydantic_extra_types.pendulum_dt import Duration
 
 from pyrevolut.utils import DateTime
-from pyrevolut.api.common import (
-    BaseEndpointSync,
-    EnumWebhookEvent,
-)
+from pyrevolut.api.common import EnumWebhookEvent
 
 from pyrevolut.api.webhooks.get import (
     RetrieveListOfWebhooks,
     RetrieveWebhook,
     RetrieveListOfFailedWebhooks,
 )
 from pyrevolut.api.webhooks.post import CreateWebhook, RotateWebhookSecret
 from pyrevolut.api.webhooks.patch import UpdateWebhook
 from pyrevolut.api.webhooks.delete import DeleteWebhook
 
+from .base import BaseEndpointWebhooks
+
 
-class EndpointWebhooksSync(BaseEndpointSync):
+class EndpointWebhooksSync(BaseEndpointWebhooks):
     """The Webhooks API
 
     A webhook (also called a web callback) allows your system to receive
     updates about your account to an HTTPS endpoint that you provide.
     When a supported event occurs, a notification is posted via HTTP POST method
     to the specified endpoint.
```

### Comparing `pyrevolut-0.6.2/pyrevolut/api/webhooks/get/retrieve_list_of_failed_webhooks.py` & `pyrevolut-0.7.0/pyrevolut/api/webhooks/get/retrieve_list_of_failed_webhooks.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/webhooks/get/retrieve_webhook.py` & `pyrevolut-0.7.0/pyrevolut/api/webhooks/get/retrieve_webhook.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/webhooks/patch/update_webhook.py` & `pyrevolut-0.7.0/pyrevolut/api/webhooks/patch/update_webhook.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/webhooks/post/create_webhook.py` & `pyrevolut-0.7.0/pyrevolut/api/webhooks/post/create_webhook.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/webhooks/post/rotate_webhook_secret.py` & `pyrevolut-0.7.0/pyrevolut/api/webhooks/post/rotate_webhook_secret.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/webhooks/resources/payout_link_created.py` & `pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/payout_link_created.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/webhooks/resources/payout_link_state_changed.py` & `pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/payout_link_state_changed.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/webhooks/resources/transaction_created.py` & `pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/transaction_created.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/webhooks/resources/transaction_state_changed.py` & `pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/transaction_state_changed.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/webhooks/resources/webhook.py` & `pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/webhook.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/api/webhooks/resources/webhook_payload.py` & `pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/webhook_payload.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/cli/main.py` & `pyrevolut-0.7.0/pyrevolut/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/client/asynchronous.py` & `pyrevolut-0.7.0/pyrevolut/client/asynchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     async def open(self):
         """Opens the client connection"""
         if self.client is not None:
             return
 
         self.client = HTTPClient()
-        self.__load_resources()
+        self.load_endpoints()
 
     async def close(self):
         """Closes the client connection"""
         if self.client is None:
             return
 
         await self.client.aclose()
@@ -234,16 +234,16 @@
         return self.process_response(
             response=resp,
             response_model=response_model,
             return_type=None,
             error_response=None,
         )
 
-    def __load_resources(self):
-        """Loads all the resources from the resources directory"""
+    def load_endpoints(self):
+        """Loads all the endpoints from the api directory"""
         self.Accounts = EndpointAccountsAsync(client=self)
         self.Cards = EndpointCardsAsync(client=self)
         self.Counterparties = EndpointCounterpartiesAsync(client=self)
         self.ForeignExchange = EndpointForeignExchangeAsync(client=self)
         self.PaymentDrafts = EndpointPaymentDraftsAsync(client=self)
         self.PayoutLinks = EndpointPayoutLinksAsync(client=self)
         self.Simulations = EndpointSimulationsAsync(client=self)
```

### Comparing `pyrevolut-0.6.2/pyrevolut/client/base.py` & `pyrevolut-0.7.0/pyrevolut/client/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         # Set domain based on environment
         if self.sandbox:
             self.domain = "https://sandbox-b2b.revolut.com/api"
         else:
             self.domain = "https://b2b.revolut.com/api"
 
         # Load the credentials
-        self.__load_credentials()
+        self.load_credentials()
 
     def process_response(
         self,
         response: Response,
         response_model: BM,
         return_type: Literal["raw", "dict", "model"] | None = None,
         error_response: Literal["raw", "raise", "dict", "model"] | None = "raise",
@@ -480,15 +480,15 @@
         if self.credentials.credentials_expired:
             raise ValueError(
                 "Long-term credentials have expired. "
                 "\n\nPlease reauthenticate using the `pyrevolut auth-manual` command."
             )
 
         if self.credentials.access_token_expired:
-            self.__refresh_access_token()
+            self.refresh_access_token()
 
     def __process_path(self, path: str) -> str:
         """Process the path.
 
         If 'http' not in the path:
             Removing the leading slash if it exists
         Else:
@@ -560,15 +560,15 @@
                 elif data[i] == "null":
                     data[i] = None
         else:
             raise ValueError("Data must be either a dictionary or a list")
 
         return data
 
-    def __load_credentials(self):
+    def load_credentials(self):
         """Load the credentials from the credentials file.
 
         - If the credentials file does not exist, raise an error.
         - If the credentials file is invalid, raise an error.
         - If the credentials are expired, raise an error.
         - If the access token is expired, refresh it.
 
@@ -588,17 +588,17 @@
 
         # Check if the credentials are still valid
         if self.credentials.credentials_expired:
             raise ValueError(f"Credentials are expired. {solution_msg}")
 
         # Check if the access token is expired
         if self.credentials.access_token_expired:
-            self.__refresh_access_token()
+            self.refresh_access_token()
 
-    def __refresh_access_token(self):
+    def refresh_access_token(self):
         """Refresh the access token using the refresh token.
         Will call the endpoint to refresh the access token.
         Then it will save the new access token to the credentials file.
 
         Parameters
         ----------
         None
```

### Comparing `pyrevolut-0.6.2/pyrevolut/client/synchronous.py` & `pyrevolut-0.7.0/pyrevolut/client/synchronous.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     def open(self):
         """Opens the client connection"""
         if self.client is not None:
             return
 
         self.client = HTTPClient()
-        self.__load_resources()
+        self.load_endpoints()
 
     def close(self):
         """Closes the client connection"""
         if self.client is None:
             return
 
         self.client.close()
@@ -233,16 +233,16 @@
         return self.process_response(
             response=resp,
             response_model=response_model,
             return_type=None,
             error_response=None,
         )
 
-    def __load_resources(self):
-        """Loads all the resources from the resources directory"""
+    def load_endpoints(self):
+        """Loads all the endpoints from the api directory"""
         self.Accounts = EndpointAccountsSync(client=self)
         self.Cards = EndpointCardsSync(client=self)
         self.Counterparties = EndpointCounterpartiesSync(client=self)
         self.ForeignExchange = EndpointForeignExchangeSync(client=self)
         self.PaymentDrafts = EndpointPaymentDraftsSync(client=self)
         self.PayoutLinks = EndpointPayoutLinksSync(client=self)
         self.Simulations = EndpointSimulationsSync(client=self)
```

### Comparing `pyrevolut-0.6.2/pyrevolut/utils/auth/auth_manual.py` & `pyrevolut-0.7.0/pyrevolut/utils/auth/auth_manual.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/utils/auth/create_client_assert_jwt.py` & `pyrevolut-0.7.0/pyrevolut/utils/auth/create_client_assert_jwt.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/utils/auth/creds.py` & `pyrevolut-0.7.0/pyrevolut/utils/auth/creds.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/utils/auth/enum_auth_scope.py` & `pyrevolut-0.7.0/pyrevolut/utils/auth/enum_auth_scope.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/utils/auth/gen_public_private_cert.py` & `pyrevolut-0.7.0/pyrevolut/utils/auth/gen_public_private_cert.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/utils/auth/get_auth_tokens.py` & `pyrevolut-0.7.0/pyrevolut/utils/auth/get_auth_tokens.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/utils/auth/refresh_access_token.py` & `pyrevolut-0.7.0/pyrevolut/utils/auth/refresh_access_token.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.6.2/pyrevolut/utils/date.py` & `pyrevolut-0.7.0/pyrevolut/utils/date.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,37 +16,47 @@
     @classmethod
     def __get_pydantic_core_schema__(
         cls, source: Type[Any], handler: GetCoreSchemaHandler
     ) -> core_schema.CoreSchema:
         """
         Return a Pydantic CoreSchema with the Date validation
 
-        Args:
-            source: The source type to be converted.
-            handler: The handler to get the CoreSchema.
-
-        Returns:
+        Parameters
+        ----------
+        source : Type[Any]
+            The source type to be converted.
+        handler : GetCoreSchemaHandler
+            The handler to get the CoreSchema.
+
+        Returns
+        -------
+        core_schema.CoreSchema
             A Pydantic CoreSchema with the Date validation.
         """
         return core_schema.no_info_wrap_validator_function(
             cls._validate, core_schema.datetime_schema()
         )
 
     @classmethod
     def _validate(
         cls, value: Any, handler: core_schema.ValidatorFunctionWrapHandler
     ) -> Any:
         """
         Validate the date object and return it.
 
-        Args:
-            value: The value to validate.
-            handler: The handler to get the CoreSchema.
-
-        Returns:
+        Parameters
+        ----------
+        value: Any
+            The value to validate.
+        handler: core_schema.ValidatorFunctionWrapHandler
+            The handler to get the CoreSchema.
+
+        Returns
+        -------
+        Any
             The validated value or raises a PydanticCustomError.
         """
         # if we are passed an existing instance, pass it straight through.
         if isinstance(value, _Date):
             return handler(value)
 
         # otherwise, parse it.
```

### Comparing `pyrevolut-0.6.2/pyrevolut/utils/datetime.py` & `pyrevolut-0.7.0/pyrevolut/utils/datetime.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,37 +20,47 @@
     @classmethod
     def __get_pydantic_core_schema__(
         cls, source: Type[Any], handler: GetCoreSchemaHandler
     ) -> core_schema.CoreSchema:
         """
         Return a Pydantic CoreSchema with the DateTime validation
 
-        Args:
-            source: The source type to be converted.
-            handler: The handler to get the CoreSchema.
-
-        Returns:
+        Parameters
+        ----------
+        source: Type[Any]
+            The source type to be converted.
+        handler: GetCoreSchemaHandler
+            The handler to get the CoreSchema.
+
+        Returns
+        -------
+        core_schema.CoreSchema
             A Pydantic CoreSchema with the DateTime validation.
         """
         return core_schema.no_info_wrap_validator_function(
             cls._validate, core_schema.datetime_schema()
         )
 
     @classmethod
     def _validate(
         cls, value: Any, handler: core_schema.ValidatorFunctionWrapHandler
     ) -> Any:
         """
         Validate the datetime object and return it.
 
-        Args:
-            value: The value to validate.
-            handler: The handler to get the CoreSchema.
-
-        Returns:
+        Parameters
+        ----------
+        value: Any
+            The value to validate.
+        handler: core_schema.ValidatorFunctionWrapHandler
+            The handler to get the CoreSchema.
+
+        Returns
+        -------
+        Any
             The validated value or raises a PydanticCustomError.
         """
         # if we are passed an existing instance, pass it straight through.
         if isinstance(value, _DateTime):
             return handler(value)
 
         # otherwise, parse it.
```

### Comparing `pyrevolut-0.6.2/PKG-INFO` & `pyrevolut-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrevolut
-Version: 0.6.2
+Version: 0.7.0
 Summary: An unofficial Python API Wrapper for the Revolut Business API
 Home-page: https://github.com/Trevypants/pyrevolut
 License: MIT
 Author: Trevor Visser
 Author-email: trevor.visser@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

