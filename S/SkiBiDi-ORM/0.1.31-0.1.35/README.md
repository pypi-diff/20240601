# Comparing `tmp/skibidi_orm-0.1.31.tar.gz` & `tmp/skibidi_orm-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skibidi_orm-0.1.31.tar", last modified: Sat Jun  1 21:08:05 2024, max compression
+gzip compressed data, was "skibidi_orm-0.1.35.tar", last modified: Sat Jun  1 21:50:29 2024, max compression
```

## Comparing `skibidi_orm-0.1.31.tar` & `skibidi_orm-0.1.35.tar`

### file list

```diff
@@ -1,140 +1,141 @@
--rw-r--r--   0        0        0     3985 2024-06-01 21:07:51.886153 skibidi_orm-0.1.31/README.md
--rw-r--r--   0        0        0     1028 2024-06-01 21:08:05.102117 skibidi_orm-0.1.31/pyproject.toml
--rw-r--r--   0        0        0        0 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/__init__.py
--rw-r--r--   0        0        0     6714 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/cli/migration_file_creator.py
--rw-r--r--   0        0        0     4357 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/cli/run.py
--rw-r--r--   0        0        0     1976 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/cli/utils.py
--rw-r--r--   0        0        0      136 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/exceptions/cli_exceptions.py
--rw-r--r--   0        0        0       93 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/exceptions/config_exceptions.py
--rw-r--r--   0        0        0      190 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/exceptions/constraints.py
--rw-r--r--   0        0        0      172 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/exceptions/db_mutator_exceptions.py
--rw-r--r--   0        0        0      309 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/exceptions/operations.py
--rw-r--r--   0        0        0        0 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/__init__.py
--rw-r--r--   0        0        0        0 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/__init__.py
--rw-r--r--   0        0        0     1501 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/base_adapter.py
--rw-r--r--   0        0        0        0 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/database_objects/__init__.py
--rw-r--r--   0        0        0     3393 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py
--rw-r--r--   0        0        0      901 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py
--rw-r--r--   0        0        0     1384 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/postgres_adapter.py
--rw-r--r--   0        0        0     1227 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/postgres_typing.py
--rw-r--r--   0        0        0      108 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/providers.py
--rw-r--r--   0        0        0     1614 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py
--rw-r--r--   0        0        0      528 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py
--rw-r--r--   0        0        0     4781 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/base/interfaces.py
--rw-r--r--   0        0        0     1076 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/postgres/all.py
--rw-r--r--   0        0        0     3922 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/postgres/columns.py
--rw-r--r--   0        0        0     1980 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/postgres/constraints.py
--rw-r--r--   0        0        0     5447 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/postgres/tables.py
--rw-r--r--   0        0        0     1589 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/sqlite3/all.py
--rw-r--r--   0        0        0     3904 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py
--rw-r--r--   0        0        0     1974 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py
--rw-r--r--   0        0        0      809 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/sqlite3/queries.py
--rw-r--r--   0        0        0     5902 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py
--rw-r--r--   0        0        0     1053 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py
--rw-r--r--   0        0        0     1389 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/data_mutator/postgres_data_mutator.py
--rw-r--r--   0        0        0     2508 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py
--rw-r--r--   0        0        0     1179 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/db_config/base_config.py
--rw-r--r--   0        0        0     1755 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/db_config/postgres_config.py
--rw-r--r--   0        0        0      593 2024-06-01 21:07:51.894152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/db_config/sqlite3_config.py
--rw-r--r--   0        0        0      671 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py
--rw-r--r--   0        0        0     8810 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/db_inspectors/postgres_inspector.py
--rw-r--r--   0        0        0     6385 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py
--rw-r--r--   0        0        0     7139 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/operations/column_operations.py
--rw-r--r--   0        0        0      280 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/operations/operation_type.py
--rw-r--r--   0        0        0     2728 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/operations/table_operations.py
--rw-r--r--   0        0        0      492 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/revisions/constants.py
--rw-r--r--   0        0        0     3784 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/revisions/manager.py
--rw-r--r--   0        0        0     1677 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/revisions/revision.py
--rw-r--r--   0        0        0     1172 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py
--rw-r--r--   0        0        0     3083 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py
--rw-r--r--   0        0        0      694 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py
--rw-r--r--   0        0        0     5556 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/state_manager/state_manager.py
--rw-r--r--   0        0        0     3300 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/server.py
--rw-r--r--   0        0        0      436 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.eslintrc.cjs
--rw-r--r--   0        0        0      248 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.gitignore
--rw-r--r--   0        0        0     1300 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md
--rw-r--r--   0        0        0      339 2024-06-01 21:07:51.898152 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/components.json
--rw-r--r--   0        0        0  2063635 2024-06-01 21:07:51.906153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js
--rw-r--r--   0        0        0   318663 2024-06-01 21:07:51.906153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css
--rw-r--r--   0        0        0      283 2024-06-01 21:07:51.906153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index.lazy-CokS8x6w.js
--rw-r--r--   0        0        0      464 2024-06-01 21:07:51.906153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/index.html
--rw-r--r--   0        0        0     1497 2024-06-01 21:07:51.906153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg
--rw-r--r--   0        0        0      366 2024-06-01 21:07:51.906153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/index.html
--rw-r--r--   0        0        0     1617 2024-06-01 21:07:51.906153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json
--rw-r--r--   0        0        0   134211 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0       80 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/postcss.config.js
--rw-r--r--   0        0        0     1497 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg
--rw-r--r--   0        0        0     4126 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg
--rw-r--r--   0        0        0      926 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx
--rw-r--r--   0        0        0     1038 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx
--rw-r--r--   0        0        0     1337 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx
--rw-r--r--   0        0        0     2121 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx
--rw-r--r--   0        0        0     1377 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx
--rw-r--r--   0        0        0     1322 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx
--rw-r--r--   0        0        0     1730 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx
--rw-r--r--   0        0        0     1835 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx
--rw-r--r--   0        0        0      315 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/collapsible.tsx
--rw-r--r--   0        0        0     3835 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx
--rw-r--r--   0        0        0     7295 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx
--rw-r--r--   0        0        0     1709 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx
--rw-r--r--   0        0        0      772 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx
--rw-r--r--   0        0        0     1361 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts
--rw-r--r--   0        0        0     1529 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts
--rw-r--r--   0        0        0     1224 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts
--rw-r--r--   0        0        0     1054 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts
--rw-r--r--   0        0        0      945 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts
--rw-r--r--   0        0        0     1140 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx
--rw-r--r--   0        0        0     1726 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx
--rw-r--r--   0        0        0     1595 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css
--rw-r--r--   0        0        0      764 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts
--rw-r--r--   0        0        0      355 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/table-data-utils.ts
--rw-r--r--   0        0        0      166 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/utils.ts
--rw-r--r--   0        0        0      790 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx
--rw-r--r--   0        0        0     1409 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts
--rw-r--r--   0        0        0     1173 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx
--rw-r--r--   0        0        0      343 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/index.lazy.tsx
--rw-r--r--   0        0        0     7445 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx
--rw-r--r--   0        0        0     1211 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css
--rw-r--r--   0        0        0       38 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/vite-env.d.ts
--rw-r--r--   0        0        0     2143 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js
--rw-r--r--   0        0        0      711 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json
--rw-r--r--   0        0        0      233 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.node.json
--rw-r--r--   0        0        0      378 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/vite.config.ts
--rw-r--r--   0        0        0      617 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py
--rw-r--r--   0        0        0      785 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py
--rw-r--r--   0        0        0      798 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py
--rw-r--r--   0        0        0     3476 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/table_example.py
--rw-r--r--   0        0        0        0 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/__init__.py
--rw-r--r--   0        0        0        0 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/cli/schema.py
--rw-r--r--   0        0        0     2108 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/cli/test_run.py
--rw-r--r--   0        0        0        0 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/__init__.py
--rw-r--r--   0        0        0     3529 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/conftest.py
--rw-r--r--   0        0        0      758 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/constraints/test_constraints.py
--rw-r--r--   0        0        0     5780 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/converters/postgres/test_postgres_column_operations_conversion.py
--rw-r--r--   0        0        0     1908 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/converters/postgres/test_postgres_constraint_conversion.py
--rw-r--r--   0        0        0     3114 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/converters/postgres/test_postgres_table_operations_conversion.py
--rw-r--r--   0        0        0     7281 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py
--rw-r--r--   0        0        0     2619 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py
--rw-r--r--   0        0        0      960 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/converters/sqlite3/test_query_conversion.py
--rw-r--r--   0        0        0     5355 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py
--rw-r--r--   0        0        0     1632 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/db_config/test_config.py
--rw-r--r--   0        0        0     1590 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/db_config/test_postgres_config.py
--rw-r--r--   0        0        0        0 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/db_inspector/__init__.py
--rw-r--r--   0        0        0     8994 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/db_inspector/test_db_inspectors.py
--rw-r--r--   0        0        0    32628 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/db_inspector/test_postgres_inspector.py
--rw-r--r--   0        0        0        0 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/db_mutators/__init__.py
--rw-r--r--   0        0        0     3113 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/db_mutators/test_postgres_mutator.py
--rw-r--r--   0        0        0     9681 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py
--rw-r--r--   0        0        0     7425 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/operations/test_operations.py
--rw-r--r--   0        0        0     5958 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/revisions/test_manager_sqlite.py
--rw-r--r--   0        0        0     8439 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/sql_data.py
--rw-r--r--   0        0        0     1530 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py
--rw-r--r--   0        0        0        0 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/state_manager/__init__.py
--rw-r--r--   0        0        0    16043 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py
--rw-r--r--   0        0        0        0 2024-06-01 21:07:51.910153 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/studio/__init__.py
--rw-r--r--   0        0        0     2200 2024-06-01 21:07:51.914152 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py
--rw-r--r--   0        0        0      890 2024-06-01 21:07:51.914152 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py
--rw-r--r--   0        0        0      693 2024-06-01 21:07:51.914152 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py
--rw-r--r--   0        0        0     3281 2024-06-01 21:07:51.914152 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/studio/test_routes.py
--rw-r--r--   0        0        0    17534 2024-06-01 21:07:51.914152 skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/test_module_cooperation.py
--rw-r--r--   0        0        0     4524 1970-01-01 00:00:00.000000 skibidi_orm-0.1.31/PKG-INFO
+-rw-r--r--   0        0        0     3961 2024-06-01 21:50:16.700729 skibidi_orm-0.1.35/README.md
+-rw-r--r--   0        0        0     1058 2024-06-01 21:50:29.852750 skibidi_orm-0.1.35/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/__init__.py
+-rw-r--r--   0        0        0     2417 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/cli/log/revision_inspection.py
+-rw-r--r--   0        0        0     8148 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/cli/log/tree.py
+-rw-r--r--   0        0        0     6714 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/cli/migration_file_creator.py
+-rw-r--r--   0        0        0     5586 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/cli/run.py
+-rw-r--r--   0        0        0     1976 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/cli/utils.py
+-rw-r--r--   0        0        0      136 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/exceptions/cli_exceptions.py
+-rw-r--r--   0        0        0       93 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/exceptions/config_exceptions.py
+-rw-r--r--   0        0        0      190 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/exceptions/constraints.py
+-rw-r--r--   0        0        0      172 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/exceptions/db_mutator_exceptions.py
+-rw-r--r--   0        0        0      309 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/exceptions/operations.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/__init__.py
+-rw-r--r--   0        0        0     1640 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/base_adapter.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/database_objects/__init__.py
+-rw-r--r--   0        0        0     3477 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py
+-rw-r--r--   0        0        0      974 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py
+-rw-r--r--   0        0        0     1384 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/postgres_adapter.py
+-rw-r--r--   0        0        0     1227 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/postgres_typing.py
+-rw-r--r--   0        0        0      108 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/providers.py
+-rw-r--r--   0        0        0     1621 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py
+-rw-r--r--   0        0        0      528 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py
+-rw-r--r--   0        0        0     4781 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/base/interfaces.py
+-rw-r--r--   0        0        0     1076 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/postgres/all.py
+-rw-r--r--   0        0        0     4175 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/postgres/columns.py
+-rw-r--r--   0        0        0     1932 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/postgres/constraints.py
+-rw-r--r--   0        0        0     5440 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/postgres/tables.py
+-rw-r--r--   0        0        0     1589 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/sqlite3/all.py
+-rw-r--r--   0        0        0     4156 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py
+-rw-r--r--   0        0        0     1926 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py
+-rw-r--r--   0        0        0      809 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/sqlite3/queries.py
+-rw-r--r--   0        0        0     4053 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py
+-rw-r--r--   0        0        0     1053 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py
+-rw-r--r--   0        0        0     1389 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/data_mutator/postgres_data_mutator.py
+-rw-r--r--   0        0        0     2508 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py
+-rw-r--r--   0        0        0     1179 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/db_config/base_config.py
+-rw-r--r--   0        0        0     1755 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/db_config/postgres_config.py
+-rw-r--r--   0        0        0      593 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/db_config/sqlite3_config.py
+-rw-r--r--   0        0        0      671 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py
+-rw-r--r--   0        0        0     8754 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/db_inspectors/postgres_inspector.py
+-rw-r--r--   0        0        0    10396 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/db_inspectors/sqlite/sqlite3_inspector.py
+-rw-r--r--   0        0        0     2965 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/db_inspectors/sqlite/supporting_objects.py
+-rw-r--r--   0        0        0     7390 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/operations/column_operations.py
+-rw-r--r--   0        0        0      280 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/operations/operation_type.py
+-rw-r--r--   0        0        0     2684 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/operations/table_operations.py
+-rw-r--r--   0        0        0      492 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/revisions/constants.py
+-rw-r--r--   0        0        0     3784 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/revisions/manager.py
+-rw-r--r--   0        0        0     1818 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/revisions/revision.py
+-rw-r--r--   0        0        0     1172 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py
+-rw-r--r--   0        0        0     3083 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py
+-rw-r--r--   0        0        0      694 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py
+-rw-r--r--   0        0        0     5556 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/state_manager/state_manager.py
+-rw-r--r--   0        0        0     3300 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/server.py
+-rw-r--r--   0        0        0      436 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.eslintrc.cjs
+-rw-r--r--   0        0        0      248 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.gitignore
+-rw-r--r--   0        0        0     1300 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md
+-rw-r--r--   0        0        0      339 2024-06-01 21:50:16.708729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/components.json
+-rw-r--r--   0        0        0  2063635 2024-06-01 21:50:16.720729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js
+-rw-r--r--   0        0        0   318663 2024-06-01 21:50:16.720729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css
+-rw-r--r--   0        0        0      283 2024-06-01 21:50:16.720729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index.lazy-CokS8x6w.js
+-rw-r--r--   0        0        0      464 2024-06-01 21:50:16.720729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/index.html
+-rw-r--r--   0        0        0     1497 2024-06-01 21:50:16.720729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg
+-rw-r--r--   0        0        0      366 2024-06-01 21:50:16.720729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/index.html
+-rw-r--r--   0        0        0     1617 2024-06-01 21:50:16.720729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json
+-rw-r--r--   0        0        0   134211 2024-06-01 21:50:16.720729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0       80 2024-06-01 21:50:16.720729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/postcss.config.js
+-rw-r--r--   0        0        0     1497 2024-06-01 21:50:16.720729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg
+-rw-r--r--   0        0        0     4126 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg
+-rw-r--r--   0        0        0      926 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx
+-rw-r--r--   0        0        0     1038 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0     1337 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx
+-rw-r--r--   0        0        0     2121 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx
+-rw-r--r--   0        0        0     1377 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx
+-rw-r--r--   0        0        0     1322 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx
+-rw-r--r--   0        0        0     1730 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx
+-rw-r--r--   0        0        0     1835 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx
+-rw-r--r--   0        0        0      315 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/collapsible.tsx
+-rw-r--r--   0        0        0     3835 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx
+-rw-r--r--   0        0        0     7295 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx
+-rw-r--r--   0        0        0     1709 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx
+-rw-r--r--   0        0        0      772 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx
+-rw-r--r--   0        0        0     1361 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts
+-rw-r--r--   0        0        0     1529 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts
+-rw-r--r--   0        0        0     1224 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts
+-rw-r--r--   0        0        0     1054 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts
+-rw-r--r--   0        0        0      945 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts
+-rw-r--r--   0        0        0     1140 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx
+-rw-r--r--   0        0        0     1726 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx
+-rw-r--r--   0        0        0     1595 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css
+-rw-r--r--   0        0        0      764 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts
+-rw-r--r--   0        0        0      355 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/table-data-utils.ts
+-rw-r--r--   0        0        0      166 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/utils.ts
+-rw-r--r--   0        0        0      790 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx
+-rw-r--r--   0        0        0     1409 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts
+-rw-r--r--   0        0        0     1173 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx
+-rw-r--r--   0        0        0      343 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/index.lazy.tsx
+-rw-r--r--   0        0        0     7445 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx
+-rw-r--r--   0        0        0     1211 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css
+-rw-r--r--   0        0        0       38 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0     2143 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js
+-rw-r--r--   0        0        0      711 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json
+-rw-r--r--   0        0        0      233 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.node.json
+-rw-r--r--   0        0        0      378 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/vite.config.ts
+-rw-r--r--   0        0        0      617 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py
+-rw-r--r--   0        0        0      792 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py
+-rw-r--r--   0        0        0      798 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py
+-rw-r--r--   0        0        0     3544 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/table_example.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/__init__.py
+-rw-r--r--   0        0        0     3529 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/conftest.py
+-rw-r--r--   0        0        0      569 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/constraints/test_constraints.py
+-rw-r--r--   0        0        0     6038 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/converters/postgres/test_postgres_column_operations_conversion.py
+-rw-r--r--   0        0        0     1905 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/converters/postgres/test_postgres_constraint_conversion.py
+-rw-r--r--   0        0        0     3116 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/converters/postgres/test_postgres_table_operations_conversion.py
+-rw-r--r--   0        0        0     6937 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py
+-rw-r--r--   0        0        0     2625 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py
+-rw-r--r--   0        0        0      960 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/converters/sqlite3/test_query_conversion.py
+-rw-r--r--   0        0        0     3994 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py
+-rw-r--r--   0        0        0     1632 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/db_config/test_config.py
+-rw-r--r--   0        0        0     1590 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/db_config/test_postgres_config.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/db_inspector/__init__.py
+-rw-r--r--   0        0        0    12602 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/db_inspector/test_db_inspectors.py
+-rw-r--r--   0        0        0    31222 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/db_inspector/test_postgres_inspector.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/db_mutators/__init__.py
+-rw-r--r--   0        0        0     3113 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/db_mutators/test_postgres_mutator.py
+-rw-r--r--   0        0        0     9688 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py
+-rw-r--r--   0        0        0     7425 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/operations/test_operations.py
+-rw-r--r--   0        0        0     5965 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/revisions/test_manager_sqlite.py
+-rw-r--r--   0        0        0     8439 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/sql_data.py
+-rw-r--r--   0        0        0     1537 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/state_manager/__init__.py
+-rw-r--r--   0        0        0    16043 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/studio/__init__.py
+-rw-r--r--   0        0        0     2200 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py
+-rw-r--r--   0        0        0      897 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py
+-rw-r--r--   0        0        0      693 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py
+-rw-r--r--   0        0        0     3288 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/studio/test_routes.py
+-rw-r--r--   0        0        0    17541 2024-06-01 21:50:16.724729 skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/test_module_cooperation.py
+-rw-r--r--   0        0        0     4538 1970-01-01 00:00:00.000000 skibidi_orm-0.1.35/PKG-INFO
```

### Comparing `skibidi_orm-0.1.31/README.md` & `skibidi_orm-0.1.35/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 Above we defined simple implementation of `Table` class which works as a base model for all SQL tables in our databse.
 
 Normally `Table` class would be abstracted away by proprietary library, but for the sake of example we defined it here.
 
 When he have defined our schema all interactions of end-user with the migration engine are done through CLI.
 
-# `skibidi-orm CLI`
+# `skibidi-orm`
 
 CLI tool for managing schema creations and migrations in Skibidi ORM.
 
 **Usage**:
 
 ```console
 $ skibidi-orm [OPTIONS] COMMAND [ARGS]...
@@ -80,45 +80,45 @@
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `go`: Go back (and forward) to specific migration.
-* `list-migrations`: List all made migrations with their...
+* `log`: List all migration revisions with their...
 * `migrate`: Used to run migration for current schema...
 * `preview-migration`: Preview the migration that will be executed.
 * `studio`: Run web UI for CRUD operations on current DB.
 
 ## `skibidi-orm go`
 
 Go back (and forward) to specific migration.
 
 **Usage**:
 
 ```console
-$ skibidi-orm go [OPTIONS] [MIGRATION_ID]
+$ skibidi-orm go [OPTIONS] MIGRATION_ID
 ```
 
 **Arguments**:
 
-* `[MIGRATION_ID]`: Migration ID
+* `MIGRATION_ID`: Migration ID  [required]
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
-## `skibidi-orm list-migrations`
+## `skibidi-orm log`
 
-List all made migrations with their descriptions and ID.
+List all migration revisions with their descriptions and ID.
 
 **Usage**:
 
 ```console
-$ skibidi-orm list-migrations [OPTIONS]
+$ skibidi-orm log [OPTIONS]
 ```
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 ## `skibidi-orm migrate`
```

### Comparing `skibidi_orm-0.1.31/pyproject.toml` & `skibidi_orm-0.1.35/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [project]
 name = "SkiBiDi-ORM"
-version = "0.1.31"
+version = "0.1.35"
 description = "Python ORM"
 authors = [
     { name = "xDepcio", email = "olek.drwal@gmail.com" },
     { name = "jedrzej-grabski", email = "grabski.dev@gmail.com" },
     { name = "mbienkowski", email = "bienkowski.maksym@gmail.com" },
 ]
 dependencies = [
     "typer>=0.11.0",
     "colorama>=0.4.6",
     "python-dotenv>=1.0.1",
     "freezegun>=1.5.1",
     "fastapi>=0.111.0",
+    "prompt-toolkit>=3.0.45",
     "black>=24.4.2",
     "psycopg2-binary>=2.9.9",
     "pdoc3>=0.10.0",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/cli/migration_file_creator.py` & `skibidi_orm-0.1.35/src/skibidi_orm/cli/migration_file_creator.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/cli/utils.py` & `skibidi_orm-0.1.35/src/skibidi_orm/cli/utils.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/base_adapter.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/base_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from functools import total_ordering
 from typing import Any
 
 from skibidi_orm.migration_engine.adapters.database_objects.constraints import (
-    ColumnSpecificConstraint,
-    ForeignKeyConstraint,
+    ColumnWideConstraint,
+    TableWideConstraint,
 )
 
 
 @total_ordering
 @dataclass(unsafe_hash=True)
 class BaseColumn[TDataTypes]:
     """
     Base column class that has to be properly implemented by the database specific column class.
     """
 
     name: str
     data_type: TDataTypes
-    column_constraints: list[ColumnSpecificConstraint] = field(
+    column_constraints: list[ColumnWideConstraint] = field(
         default_factory=list, hash=False
     )
 
+    def __str__(self) -> str:
+        return f"{self.name.ljust(15)} {self.data_type}"
+
     def __lt__(self, other: Any):
         if isinstance(other, BaseColumn):
             return self.name < other.name
         return NotImplemented
 
 
 @dataclass
 class BaseTable[TCol]:
     """
     Base table class that has to be properly implemented by the database specific table class.
     """
 
     name: str
     columns: list[TCol] = field(default_factory=list)
-    foreign_keys: set[ForeignKeyConstraint] = field(default_factory=set)
+    table_constraints: set[TableWideConstraint] = field(default_factory=set)
+
+    def __str__(self) -> str:
+        return self.name
 
 
 class BaseAdapter(ABC):
     """
     Base adapter class that has to be properly implemented by the database specific adapter class.
     """
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from __future__ import annotations
 from abc import ABC
 import enum
 from dataclasses import dataclass, field
 from functools import total_ordering
 from typing import Any
 
 
@@ -25,56 +24,61 @@
     table_name: str
 
     def __repr__(self):
         return f"{self.__class__.__name__}('{self.constraint_type.value}', '{self.table_name}')"
 
 
 @total_ordering
-@dataclass(frozen=True, repr=False)
-class ColumnSpecificConstraint(Constraint):
+@dataclass(frozen=True)
+class ColumnWideConstraint(Constraint):
     """Base class for constraints that apply to a column instead of multiple (e.g. composite foreign keys)"""
 
     column_name: str
 
     def __repr__(self):
         return f"{self.__class__.__name__}('{self.constraint_type.value}', '{self.column_name}')"
 
     def __lt__(self, other: Any):
-        if isinstance(other, ColumnSpecificConstraint):
+        if isinstance(other, ColumnWideConstraint):
             return (self.column_name + self.__class__.__name__ + str(self.__dict__)) < (
                 other.column_name + other.__class__.__name__ + str(other.__dict__)
             )
         return NotImplemented
 
 
 @dataclass(frozen=True, repr=False)
-class NotNullConstraint(ColumnSpecificConstraint):
+class TableWideConstraint(Constraint):
+    """Base class for constraints that apply to a table - foreign keys and check constraints"""
+
+
+@dataclass(frozen=True, repr=False)
+class NotNullConstraint(ColumnWideConstraint):
     """Class for the NOT NULL constraint"""
 
     constraint_type: ConstraintType = field(init=False, default=ConstraintType.NOT_NULL)
 
 
 @dataclass(frozen=True, repr=False)
-class UniqueConstraint(ColumnSpecificConstraint):
+class UniqueConstraint(ColumnWideConstraint):
     """Class for the UNIQUE constraint"""
 
     constraint_type: ConstraintType = field(init=False, default=ConstraintType.UNIQUE)
 
 
 @dataclass(frozen=True, repr=False)
-class PrimaryKeyConstraint(ColumnSpecificConstraint):
+class PrimaryKeyConstraint(ColumnWideConstraint):
     """Class for the PRIMARY KEY constraint"""
 
     constraint_type: ConstraintType = field(
         init=False, default=ConstraintType.PRIMARY_KEY
     )
 
 
 @dataclass(frozen=True, unsafe_hash=True, repr=False)
-class ForeignKeyConstraint(Constraint):
+class ForeignKeyConstraint(TableWideConstraint):
     """Class for the FOREIGN KEY constraint"""
 
     constraint_type: ConstraintType = field(
         init=False, default=ConstraintType.FOREIGN_KEY
     )
     referenced_table: str
     column_mapping: dict[str, str] = field(
@@ -82,26 +86,26 @@
     )  # maps the corresponding column names: {referencing_column1: referenced_column1, ...}
 
     def __repr__(self):
         return f"{self.__class__.__name__}('{self.constraint_type.value}', '{self.table_name}', '{self.referenced_table}', {self.column_mapping})"
 
 
 @dataclass(frozen=True, repr=False)
-class CheckConstraint(ColumnSpecificConstraint):
+class CheckConstraint(TableWideConstraint):
     """Class for the CHECK constraint"""
 
     constraint_type: ConstraintType = field(init=False, default=ConstraintType.CHECK)
     condition: str
 
     def __repr__(self):
-        return f"{self.__class__.__name__}('{self.constraint_type.value}', '{self.column_name}', '{self.condition}')"
+        return f"{self.__class__.__name__}('{self.constraint_type.value}', '{self.condition}')"
 
 
 @dataclass(frozen=True, repr=False)
-class DefaultConstraint(ColumnSpecificConstraint):
+class DefaultConstraint(ColumnWideConstraint):
     """Class for the DEFAULT constraint"""
 
     constraint_type: ConstraintType = field(init=False, default=ConstraintType.DEFAULT)
     value: str
 
     def __repr__(self):
         return f"{self.__class__.__name__}('{self.constraint_type.value}', '{self.column_name}', '{self.value}')"
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 
     def migrate(self, preview: bool = False):
         """
         This will execute the migration for all the migration elements.
 
         """
         table = MigrationElement.__subclasses__()
+        self.adapter = table[0]().adapter # todo: do this in a nicer way
 
         for cls in table:
             table_instance = cls()
             table_instance.adapter.execute_migration(preview)
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/postgres_adapter.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/postgres_adapter.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/postgres_typing.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/postgres_typing.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from skibidi_orm.migration_engine.adapters.base_adapter import BaseAdapter
 from skibidi_orm.migration_engine.adapters.database_objects.migration_element import (
     MigrationElement,
 )
 from skibidi_orm.migration_engine.adapters.sqlite3_typing import (
     SQLite3Typing,
 )
-from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
+from skibidi_orm.migration_engine.db_inspectors.sqlite.sqlite3_inspector import (
     SQLite3Inspector,
 )
 from skibidi_orm.migration_engine.state_manager.state_manager import StateManager
 
 from skibidi_orm.migration_engine.sql_executor.sqlite3_executor import SQLite3Executor
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/base/interfaces.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/base/interfaces.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/postgres/all.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/postgres/all.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/postgres/columns.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/postgres/columns.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from skibidi_orm.migration_engine.operations.column_operations import (
     AddColumnOperation,
     ColumnOperation,
     DeleteColumnOperation,
     RenameColumnOperation,
 )
 from skibidi_orm.migration_engine.adapters.database_objects.constraints import (
-    ColumnSpecificConstraint,
+    ColumnWideConstraint,
 )
 from skibidi_orm.migration_engine.operations.operation_type import OperationType
 from skibidi_orm.exceptions.operations import UnsupportedOperationError
 from typing import cast
 
 
 class PostgresColumnOperationConverter(ColumnOperationSQLConverter):
@@ -59,14 +59,19 @@
         if operation.related_foreign_key is not None:
             referenced_column = operation.related_foreign_key.column_mapping[
                 operation.column.name
             ]
             fk_definition = f"REFERENCES {operation.related_foreign_key.referenced_table} ({referenced_column})"
             return_value += f" {fk_definition}"
 
+        if operation.related_check_constraint is not None:
+            check_definition = PostgresConstraintConverter.convert_constraint_to_SQL(
+                operation.related_check_constraint
+            )
+            return_value += f" {check_definition}"
         return f"{return_value};"
 
     @staticmethod
     def convert_delete_column_operation_to_SQL(operation: DeleteColumnOperation) -> str:
         """Convert a given delete column operation to a Postgres SQL string"""
         return (
             f"ALTER TABLE {operation.table.name} DROP COLUMN {operation.column.name};"
@@ -75,15 +80,15 @@
     @staticmethod
     def convert_rename_column_operation_to_SQL(operation: RenameColumnOperation) -> str:
         """Convert a given rename column operation to a Postgres SQL string"""
         return f"ALTER TABLE {operation.table.name} RENAME COLUMN {operation.column.name} TO {operation.new_name};"
 
     @staticmethod
     def convert_column_definition_to_SQL(
-        column: PostgresTyping.Column, constraints: list[ColumnSpecificConstraint]
+        column: PostgresTyping.Column, constraints: list[ColumnWideConstraint]
     ) -> str:
         """Convert a given column definition to a Postgres SQL string"""
         return_value = f"{column.name} {column.data_type}"
         for constraint in constraints:
             return_value += (
                 f" {PostgresConstraintConverter.convert_constraint_to_SQL(constraint)}"
             )
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/postgres/constraints.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,38 +7,38 @@
     Constraint,
     ConstraintType,
     ForeignKeyConstraint,
 )
 from typing import cast
 
 
-class PostgresConstraintConverter(ConstraintSQLConverter):
-    """Class responsible for converting constraint objects to raw Postgres SQL strings"""
+class SQLite3ConstraintConverter(ConstraintSQLConverter):
+    """Class responsible for converting constraint objects to raw SQLite3 SQL strings"""
 
     @staticmethod
     def convert_constraint_change_operation_to_SQL(_: Constraint) -> str:
-        """Convert a given constraint change operation to a Postgres SQL string"""
+        """Convert a given constraint change operation to a SQLite3 SQL string"""
         raise NotImplementedError(
-            "Constraint change operations are not supported in Postgres yet."
+            "Constraint change operations are not supported in SQLite3 yet."
         )
 
     @staticmethod
     def convert_constraint_to_SQL(constraint: Constraint) -> str:
-        """Convert a given constraint to a Postgres SQL string"""
+        """Convert a given constraint to a SQLite3 SQL string"""
         if constraint.constraint_type == ConstraintType.PRIMARY_KEY:
             return "PRIMARY KEY"
         elif constraint.constraint_type == ConstraintType.UNIQUE:
             return "UNIQUE"
         elif constraint.constraint_type == ConstraintType.FOREIGN_KEY:
             constraint = cast(ForeignKeyConstraint, constraint)
             return (
                 f"FOREIGN KEY ({', '.join(constraint.column_mapping.keys())}) REFERENCES"
                 f" {constraint.referenced_table} ({', '.join(constraint.column_mapping.values())})"
             )
         elif constraint.constraint_type == ConstraintType.CHECK:
-            return f"CHECK ({cast(CheckConstraint, constraint).column_name} {cast(CheckConstraint, constraint).condition})"
+            return f"CHECK ({cast(CheckConstraint, constraint).condition})"
         elif constraint.constraint_type == ConstraintType.NOT_NULL:
             return "NOT NULL"
         else:
             raise UnsupportedConstraintError(
-                f"Constraints of type {constraint.constraint_type} are not supported by Postgres"
+                f"Constraints of type {constraint.constraint_type} are not supported by SQLite3"
             )
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/postgres/tables.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/postgres/tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from skibidi_orm.migration_engine.adapters.postgres_typing import PostgresTyping
 from skibidi_orm.migration_engine.converters.base.interfaces import (
     TableOperationSQLConverter,
 )
 from skibidi_orm.migration_engine.converters.postgres.columns import PostgresColumnOperationConverter
 from skibidi_orm.migration_engine.converters.postgres.constraints import PostgresConstraintConverter
 from skibidi_orm.migration_engine.adapters.database_objects.constraints import (
-    ColumnSpecificConstraint,
+    ColumnWideConstraint,
     ConstraintType,
 )
 from skibidi_orm.migration_engine.operations.operation_type import OperationType
 from skibidi_orm.migration_engine.operations.table_operations import (
     DeleteTableOperation,
     RenameTableOperation,
     TableOperation,
@@ -66,15 +66,15 @@
                     column, constraints_at_column)}, "
 
         for constraint in constraints_at_end:
             definition_string += (
                 f"{PostgresConstraintConverter.convert_constraint_to_SQL(constraint)}, "
             )
 
-        for key in operation.table.foreign_keys:
+        for key in operation.table.table_constraints:
             definition_string += (
                 f"{PostgresConstraintConverter.convert_constraint_to_SQL(key)}, "
             )
 
         return definition_string.strip(", ") + ");"
 
     @staticmethod
@@ -96,15 +96,15 @@
             + " "
             + PostgresTableOperationConverter.convert_table_operation_to_SQL(create_op)
         )
 
     @staticmethod
     def split_constraints(
         table: PostgresTyping.Table,
-    ) -> tuple[set[ColumnSpecificConstraint], set[ColumnSpecificConstraint]]:
+    ) -> tuple[set[ColumnWideConstraint], set[ColumnWideConstraint]]:
         """Split the constraints of a table into those that have to be added at the end of the
         table definition and those that have to be added in the definitions of their resective columns
         """
         all_constraints = set(
             chain.from_iterable(column.column_constraints for column in table.columns)
         )
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/sqlite3/all.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/sqlite3/all.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from skibidi_orm.migration_engine.operations.column_operations import (
     AddColumnOperation,
     ColumnOperation,
     DeleteColumnOperation,
     RenameColumnOperation,
 )
 from skibidi_orm.migration_engine.adapters.database_objects.constraints import (
-    ColumnSpecificConstraint,
+    ColumnWideConstraint,
 )
 from skibidi_orm.migration_engine.operations.operation_type import OperationType
 from skibidi_orm.exceptions.operations import UnsupportedOperationError
 from typing import cast
 
 
 class SQLite3ColumnOperationConverter(ColumnOperationSQLConverter):
@@ -58,14 +58,19 @@
         )
         if operation.related_foreign_key is not None:
             referenced_column = operation.related_foreign_key.column_mapping[
                 operation.column.name
             ]
             fk_definition = f"REFERENCES {operation.related_foreign_key.referenced_table} ({referenced_column})"
             return_value += f" {fk_definition}"
+        if operation.related_check_constraint is not None:
+            check_definition = SQLite3ConstraintConverter.convert_constraint_to_SQL(
+                operation.related_check_constraint
+            )
+            return_value += f" {check_definition}"
 
         return f"{return_value};"
 
     @staticmethod
     def convert_delete_column_operation_to_SQL(operation: DeleteColumnOperation) -> str:
         """Convert a given delete column operation to a SQLite3 SQL string"""
         return (
@@ -75,15 +80,15 @@
     @staticmethod
     def convert_rename_column_operation_to_SQL(operation: RenameColumnOperation) -> str:
         """Convert a given rename column operation to a SQLite3 SQL string"""
         return f"ALTER TABLE {operation.table.name} RENAME COLUMN {operation.column.name} TO {operation.new_name};"
 
     @staticmethod
     def convert_column_definition_to_SQL(
-        column: SQLite3Typing.Column, constraints: list[ColumnSpecificConstraint]
+        column: SQLite3Typing.Column, constraints: list[ColumnWideConstraint]
     ) -> str:
         """Convert a given column definition to a SQLite3 SQL string"""
         return_value = f"{column.name} {column.data_type}"
         for constraint in constraints:
             return_value += (
                 f" {SQLite3ConstraintConverter.convert_constraint_to_SQL(constraint)}"
             )
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/postgres/constraints.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,38 +7,38 @@
     Constraint,
     ConstraintType,
     ForeignKeyConstraint,
 )
 from typing import cast
 
 
-class SQLite3ConstraintConverter(ConstraintSQLConverter):
-    """Class responsible for converting constraint objects to raw SQLite3 SQL strings"""
+class PostgresConstraintConverter(ConstraintSQLConverter):
+    """Class responsible for converting constraint objects to raw Postgres SQL strings"""
 
     @staticmethod
     def convert_constraint_change_operation_to_SQL(_: Constraint) -> str:
-        """Convert a given constraint change operation to a SQLite3 SQL string"""
+        """Convert a given constraint change operation to a Postgres SQL string"""
         raise NotImplementedError(
-            "Constraint change operations are not supported in SQLite3 yet."
+            "Constraint change operations are not supported in Postgres yet."
         )
 
     @staticmethod
     def convert_constraint_to_SQL(constraint: Constraint) -> str:
-        """Convert a given constraint to a SQLite3 SQL string"""
+        """Convert a given constraint to a Postgres SQL string"""
         if constraint.constraint_type == ConstraintType.PRIMARY_KEY:
             return "PRIMARY KEY"
         elif constraint.constraint_type == ConstraintType.UNIQUE:
             return "UNIQUE"
         elif constraint.constraint_type == ConstraintType.FOREIGN_KEY:
             constraint = cast(ForeignKeyConstraint, constraint)
             return (
                 f"FOREIGN KEY ({', '.join(constraint.column_mapping.keys())}) REFERENCES"
                 f" {constraint.referenced_table} ({', '.join(constraint.column_mapping.values())})"
             )
         elif constraint.constraint_type == ConstraintType.CHECK:
-            return f"CHECK ({cast(CheckConstraint, constraint).column_name} {cast(CheckConstraint, constraint).condition})"
+            return f"CHECK ({cast(CheckConstraint, constraint).condition})"
         elif constraint.constraint_type == ConstraintType.NOT_NULL:
             return "NOT NULL"
         else:
             raise UnsupportedConstraintError(
-                f"Constraints of type {constraint.constraint_type} are not supported by SQLite3"
+                f"Constraints of type {constraint.constraint_type} are not supported by Postgres"
             )
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/converters/sqlite3/queries.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/converters/sqlite3/queries.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/data_mutator/postgres_data_mutator.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/data_mutator/postgres_data_mutator.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/db_config/base_config.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/db_config/base_config.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/db_config/postgres_config.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/db_config/postgres_config.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/db_config/sqlite3_config.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/db_config/sqlite3_config.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/db_inspectors/postgres_inspector.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/db_inspectors/postgres_inspector.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,17 @@
         Get all tables from the database.
         """
 
         return [
             PostgresTyping.Table(
                 name=table_name,
                 columns=self.get_table_columns(table_name),
-                foreign_keys=self._get_foreign_keys(table_name),
+                table_constraints=cast(
+                    set[c.TableWideConstraint], self._get_foreign_keys(table_name)
+                ),
             )
             for table_name in self.get_tables_names()
         ]
 
     def get_table_columns(self, table_name: str) -> list[PostgresTyping.Column]:
         """
         Get all columns from the table.
@@ -113,15 +115,15 @@
                 )
             )
 
         return res
 
     def _get_column_constraints(
         self, table_name: str, column_name: str
-    ) -> list[c.ColumnSpecificConstraint]:
+    ) -> list[c.ColumnWideConstraint]:
         """
         Get all column constraints from the table.
         """
 
         with self.config.connection.cursor() as cursor:
             cursor.execute(
                 f"""
@@ -158,20 +160,18 @@
 
             rows = cursor.fetchall()
             if len(rows) == 0:
                 raise ValueError(
                     f"Column '{column_name}' does not exist in table '{table_name}'"
                 )
 
-        res: list[c.ColumnSpecificConstraint] = []
+        res: list[c.ColumnWideConstraint] = []
         for row in rows:  # loop because we can have many constraints for one column
-            _, _, constraint_type, _, check_clause, column_default = row
+            _, _, constraint_type, _, _, column_default = row
 
-            if check_clause:
-                res.append(c.CheckConstraint(table_name, column_name, check_clause))
             if constraint_type == "PRIMARY KEY":
                 res.append(c.PrimaryKeyConstraint(table_name, column_name))
             if constraint_type == "UNIQUE":
                 res.append(c.UniqueConstraint(table_name, column_name))
             if not self._is_column_nullable(
                 table_name, column_name
             ) and not self.__holds_instance(res, c.NotNullConstraint):
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/db_inspectors/sqlite/sqlite3_inspector.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,25 @@
-from __future__ import annotations
-from dataclasses import dataclass
-from typing import Any, Literal, cast
+from typing import cast
+from skibidi_orm.migration_engine.db_inspectors.sqlite.supporting_objects import (
+    PragmaIndexInfoEntry,
+    PragmaIndexListEntry,
+    PragmaTableInfoEntry,
+    PragmaForeignKeyListEntry,
+)
 import sqlite3
+import re
 
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 from skibidi_orm.migration_engine.db_inspectors.base_inspector import BaseDbInspector
 from skibidi_orm.migration_engine.adapters.sqlite3_typing import (
     SQLite3Typing,
 )
 import skibidi_orm.migration_engine.adapters.database_objects.constraints as c
 from skibidi_orm.migration_engine.revisions.constants import get_revision_table_name
 
-type SQLite3PragmaTableInfo = list[
-    tuple[int, str, str, Literal[0, 1], Any, Literal[0, 1]]
-]
-
-
-@dataclass(frozen=True)
-class PragmaForeignKeyListEntry:
-    id: int
-    seq: int
-    table: str
-    from_column: str
-    to_column: str
-    on_update: str
-    on_delete: str
-    match: str
-
-    @classmethod
-    def from_tuple(
-        cls,
-        values: tuple[str, str, str, str, str, str, str, str],
-    ) -> PragmaForeignKeyListEntry:
-        id, seq, table, from_column, to_column, on_update, on_delete, match = values
-        return cls(
-            int(id),
-            int(seq),
-            table,
-            from_column,
-            to_column,
-            on_update,
-            on_delete,
-            match,
-        )
-
-
 type SQLite3PragmaForeignKeyList = list[PragmaForeignKeyListEntry]
 
 
 class SQLite3Inspector(BaseDbInspector):
     """
     Used to get data from live SQLite3 database.
     Should only be instantiated when SQLite3 is choosen as the database.
@@ -68,15 +39,17 @@
         tables_names = self.get_tables_names()
         foreign_keys = self.get_foreign_key_constraints()
         for table_name in tables_names:
             table_columns = self.get_table_columns(table_name)
             related_fks = {fk for fk in foreign_keys if fk.table_name == table_name}
             tables.append(
                 SQLite3Typing.Table(
-                    name=table_name, columns=table_columns, foreign_keys=related_fks
+                    name=table_name,
+                    columns=table_columns,
+                    table_constraints=cast(set[c.TableWideConstraint], related_fks),
                 )
             )
 
         return tables
 
     def get_tables_names(self) -> list[str]:
         """
@@ -116,14 +89,106 @@
                         for entry in corresponding_entries
                     },
                 )
                 return_value.add(corresponding_constraint)
 
         return return_value
 
+    def get_index_details(
+        self, index: PragmaIndexListEntry
+    ) -> list[PragmaIndexInfoEntry]:
+        """Get all details regarding a specific index"""
+        raw_pragma_index_info = self._sqlite_execute(
+            f"PRAGMA index_info({index.name});"
+        )
+        return [
+            PragmaIndexInfoEntry.from_tuple(entry) for entry in raw_pragma_index_info
+        ]
+
+    def get_all_indices_and_details(
+        self, table_name: str
+    ) -> dict[PragmaIndexListEntry, list[PragmaIndexInfoEntry]]:
+        """Get all indices regarding a specific table and their details."""
+
+        raw_pragma_index_list = self._sqlite_execute(
+            f"PRAGMA index_list({table_name});"
+        )
+        indices = [
+            PragmaIndexListEntry.from_tuple(entry) for entry in raw_pragma_index_list
+        ]
+        details = [self.get_index_details(index) for index in indices]
+        return {index: detail for index, detail in zip(indices, details)}
+
+    def get_all_unique_non_composite_indices(
+        self, table_name: str
+    ) -> dict[PragmaIndexListEntry, PragmaIndexInfoEntry]:
+        """Get all non-composite indices created by the UNIQUE keyword from a table
+        as well as their info entry objects."""
+        indices_with_details = self.get_all_indices_and_details(table_name)
+        # filter out only the indices created by the UNIQUE keyword, skip primary keys and artificial indices
+        return {
+            index: details.pop()
+            for index, details in indices_with_details.items()
+            if index.creation_method == "u" and len(details) == 1
+        }
+
+    # todo: could refactor for this to only return column names instead
+    def get_all_unique_constraints(self, table_name: str) -> list[c.UniqueConstraint]:
+        """Get all unique constraints from a given table. This only detects the unique constraints
+        based on non-composite indices explicitly created from the UNIQUE keyword."""
+        valid_indices = self.get_all_unique_non_composite_indices(table_name)
+        if not valid_indices:
+            return []
+        return [
+            c.UniqueConstraint(table_name, cast(str, entry.column_name))
+            # casting since indices created by UNIQUE can't contain null as the column name
+            for entry in valid_indices.values()
+        ]
+
+    def _get_all_check_conditions(self, table_creation_sql: str) -> list[str]:
+        """Get all check conditions from the table creation SQL."""
+        pattern = re.compile(r"CHECK\s*\(", re.IGNORECASE)
+
+        # Find all the positions of 'CHECK' statements
+        check_positions = [
+            match.start() for match in pattern.finditer(table_creation_sql)
+        ]
+
+        conditions: list[str] = []
+
+        for pos in check_positions:
+            # Start position of the constraint
+            start = pos + len("CHECK(") + 1  # move past the opening parenthesis
+            balance = 1
+            end = start
+
+            while balance > 0 and end < len(table_creation_sql):
+                if table_creation_sql[end] == "(":
+                    balance += 1
+                elif table_creation_sql[end] == ")":
+                    balance -= 1
+                end += 1
+
+            # Extracting the constraint without the outer parentheses
+            end -= 1
+            condition = table_creation_sql[start:end].strip()
+            conditions.append(condition)
+
+        return conditions
+
+    def get_all_check_constraints(self, table_name: str) -> list[c.CheckConstraint]:
+        """Get all check constraints from the database."""
+        query = f"SELECT * from sqlite_master where tbl_name = '{table_name}' and type = 'table';"
+        query_result = self._sqlite_execute(query).pop()
+
+        sql = query_result[4]
+
+        check_conditions = self._get_all_check_conditions(sql)
+        return [c.CheckConstraint(table_name, content) for content in check_conditions]
+
     def get_foreign_key_constraints(self) -> set[c.ForeignKeyConstraint]:
         """Get all foreign key constraints from the database."""
 
         tables_names = self.get_tables_names()
         pragma_results: dict[str, list[PragmaForeignKeyListEntry]] = {
             # Map tables to their pragma entries
             table: [
@@ -138,46 +203,61 @@
         pragma_results = pragma_results  # todo: remove
 
         constraints: set[c.ForeignKeyConstraint] = (
             SQLite3Inspector.foreign_keys_from_pragma_entries(pragma_results)
         )
         return constraints
 
+    def get_column_constraints(
+        self, table_name: str, entry: PragmaTableInfoEntry
+    ) -> list[c.ColumnWideConstraint]:
+        """Get all constraints for a column determined by the pragma table info entry.
+        and a name of the table."""
+        constraints: list[c.ColumnWideConstraint] = []
+        column_name = entry.name
+        if entry.pk:
+            constraints.append(
+                c.PrimaryKeyConstraint(table_name=table_name, column_name=column_name)
+            )
+        if entry.notnull:
+            constraints.append(
+                c.NotNullConstraint(table_name=table_name, column_name=column_name)
+            )
+        if entry.dflt_value is not None:
+            constraints.append(
+                c.DefaultConstraint(
+                    table_name=table_name,
+                    column_name=column_name,
+                    value=entry.dflt_value,
+                )
+            )
+        unique_constraints_for_table = self.get_all_unique_constraints(table_name)
+        constraints.extend(
+            [c for c in unique_constraints_for_table if c.column_name == column_name]
+        )
+        return constraints
+
     def get_table_columns(self, table_name: str) -> list[SQLite3Typing.Column]:
-        columns: SQLite3PragmaTableInfo = self._sqlite_execute(
+        raw_pragma_table_info = self._sqlite_execute(
             f"PRAGMA table_info({table_name});"
         )
+        pragma_entries = [
+            PragmaTableInfoEntry.from_tuple(entry) for entry in raw_pragma_table_info
+        ]
         """
         When given a table name, returns a list of Column objects inside it.
         """
 
         return [
             SQLite3Typing.Column(
-                name=name,
-                data_type=cast(SQLite3Typing.DataTypes, data_type),
-                column_constraints=[
-                    cast(c.ColumnSpecificConstraint, constraint)
-                    for constraint in [
-                        (
-                            c.PrimaryKeyConstraint(
-                                table_name=table_name, column_name=name
-                            )
-                            if pk
-                            else None
-                        ),
-                        (
-                            c.NotNullConstraint(table_name=table_name, column_name=name)
-                            if notnull
-                            else None
-                        ),
-                    ]
-                    if constraint is not None
-                ],
+                name=entry.name,
+                data_type=cast(SQLite3Typing.DataTypes, entry.data_type),
+                column_constraints=self.get_column_constraints(table_name, entry),
             )
-            for _, name, data_type, notnull, _, pk in columns
+            for entry in pragma_entries
         ]
 
     def _sqlite_execute(self, query: str):
         """
         Execute a query in the SQLite3 database, returns its result.
         """
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/operations/column_operations.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/operations/column_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from skibidi_orm.migration_engine.operations.operation_type import OperationType
 from skibidi_orm.migration_engine.adapters.database_objects.constraints import (
     Constraint,
     ForeignKeyConstraint,
+    CheckConstraint,
 )
 from skibidi_orm.exceptions.operations import IrreversibleOperationError
 from skibidi_orm.migration_engine.adapters.base_adapter import BaseTable, BaseColumn
 from typing import Any
 from dataclasses import dataclass, field
 from typing import Optional
 
@@ -28,33 +29,36 @@
 
     def get_related_foreign_keys(self) -> list[ForeignKeyConstraint]:
         """Returns the foreign keys that are related to the column operation.
         If the column is already instantiated and is a part of a foreign key,
         it has to be taken into acount when removing and adding it back to the schema.
         """
         return [
-            fk
-            for fk in self.table.foreign_keys
-            if self.column.name in fk.column_mapping
+            c
+            for c in self.table.table_constraints
+            if isinstance(c, ForeignKeyConstraint)
+            and self.column.name in c.column_mapping
         ]
 
     @abstractmethod
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(table={self.table}, is_reversible={self.is_reversible})"
 
 
 @dataclass(frozen=True)
 class AddColumnOperation(ColumnOperation):
     """Class for adding a column"""
 
     operation_type: OperationType = field(init=False, default=OperationType.CREATE)
     is_reversible: bool = field(init=False, default=True)
 
-    # if the column to be added references another table, it has to be set here
+    # these fields serve as a way to add new table-level constraints to the table when
+    # adding the column after creating it. they can only reference the column to be added!
     related_foreign_key: Optional[ForeignKeyConstraint] = field(default=None)
+    related_check_constraint: Optional[CheckConstraint] = field(default=None)
 
     def reverse(self) -> ColumnOperation:
         return DeleteColumnOperation(table=self.table, column=self.column)
 
     def __post_init__(self):
         self.validate_related_foreign_key()
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/operations/table_operations.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/operations/table_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     """Class for renaming a table"""
 
     operation_type: OperationType = field(init=False, default=OperationType.RENAME)
     is_reversible: bool = field(init=False, default=True)
     new_name: str
 
     def reverse(self) -> TableOperation:
-        # todo: make sure it works properly
         return RenameTableOperation(table=self.table, new_name=self.table.name)
 
     def __str__(self) -> str:
         return f"Rename Table {self.table.name} to {self.new_name}"
 
     def __repr__(self) -> str:
         return (
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/revisions/manager.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/revisions/manager.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/revisions/revision.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/revisions/revision.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,10 +40,13 @@
             return pickle.dumps(self)
 
     @staticmethod
     def deserialize(data: bytes):
         """Deserializes the data from the database."""
         return pickle.loads(data)
 
+    def __str__(self) -> str:
+        return f"{self.timestamp.strftime("%Y-%m-%d %H:%M:%S")} - {self.description} ({self.provider.value})"
+
 
 # register the converter function which deserializes the object
 sqlite3.register_converter("REVISION", Revision.deserialize)
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/state_manager/state_manager.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/state_manager/state_manager.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/server.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/server.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from skibidi_orm.migration_engine.db_config.base_config import BaseDbConfig
 from skibidi_orm.migration_engine.db_config.postgres_config import PostgresConfig
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 from skibidi_orm.migration_engine.db_inspectors.base_inspector import BaseDbInspector
 from skibidi_orm.migration_engine.db_inspectors.postgres_inspector import (
     PostgresInspector,
 )
-from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
+from skibidi_orm.migration_engine.db_inspectors.sqlite.sqlite3_inspector import (
     SQLite3Inspector,
 )
 
 
 def get_db_inspector(db_config: BaseDbConfig) -> BaseDbInspector:
     if isinstance(db_config, SQLite3Config):
         return SQLite3Inspector()
```

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/src/skibidi_orm/migration_engine/table_example.py` & `skibidi_orm-0.1.35/src/skibidi_orm/migration_engine/table_example.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,24 +32,24 @@
         if self.__class__ == Table:
             for cls in models:
                 table: SQLite3Typing.Table
                 data_type: SQLite3Typing.DataTypes
                 columns: list[SQLite3Typing.Column] = []
                 all_constraints = cls.__dict__["constraints"]
 
-                fks: set[c.ForeignKeyConstraint] = set(
+                table_constraints: set[c.TableWideConstraint] = set(
                     constraint
                     for constraint in all_constraints
-                    if isinstance(constraint, c.ForeignKeyConstraint)
+                    if isinstance(constraint, c.TableWideConstraint)
                 )
 
                 column_constraints = [
                     constraint
                     for constraint in all_constraints
-                    if isinstance(constraint, c.ColumnSpecificConstraint)
+                    if isinstance(constraint, c.ColumnWideConstraint)
                 ]
 
                 if cls.__dict__["data_type"] == "my_definition_of_data_type":
                     data_type = "INTEGER"
                 elif cls.__dict__["data_type"] == "my_other_definition":
                     data_type = "TEXT"
                 elif cls.__dict__["data_type"] == "and_other":
@@ -61,15 +61,17 @@
                     SQLite3Typing.Column(
                         name=cls.__dict__["name"],
                         data_type=data_type,
                         column_constraints=column_constraints,
                     )
                 )
                 table = SQLite3Typing.Table(
-                    name=cls.__name__, columns=columns, foreign_keys=fks
+                    name=cls.__name__,
+                    columns=columns,
+                    table_constraints=table_constraints,
                 )
 
                 # Table, for each instance should properly inform the adapter about being created
                 self.adapter.create_table(table)
 
 
 class User(Table):
```

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/conftest.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/conftest.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/constraints/test_constraints.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/constraints/test_constraints.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,16 +10,11 @@
                     table_name="table_name",
                     column_name="column_name",
                 ),
                 c.NotNullConstraint(
                     table_name="table_name",
                     column_name="column_name",
                 ),
-                c.CheckConstraint(
-                    table_name="table_name",
-                    column_name="column_name",
-                    condition="condition",
-                ),
             ]
         )
     except TypeError as e:
         pytest.fail(f"TypeError: {e}")
```

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/converters/postgres/test_postgres_column_operations_conversion.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/converters/postgres/test_postgres_column_operations_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     CheckConstraint,
     ForeignKeyConstraint,
     NotNullConstraint,
     PrimaryKeyConstraint,
     UniqueConstraint,
 )
 
-
 simple_column_no_constraints = PostgresTyping.Column("name", "TEXT")
 column_primary_key_unique = PostgresTyping.Column(
     "user_id",
     "INTEGER",
     column_constraints=[
         PrimaryKeyConstraint("users", "user_id"),
         UniqueConstraint("users", "user_id"),
@@ -38,141 +37,141 @@
         UniqueConstraint("users", "user_id"),
     ],
 )
 
 column_check_constraint = PostgresTyping.Column(
     "age",
     "INTEGER",
-    column_constraints=[CheckConstraint("users", "age", "> 18")],
 )
 
 empty_users_table = PostgresTyping.Table("users", columns=[])
 
 
 @pytest.mark.parametrize(
     "column, constraints_list, expected",
     [
         (simple_column_no_constraints, [], "name TEXT"),
         (
-            column_primary_key_unique,
-            column_primary_key_unique.column_constraints,
-            "user_id INTEGER PRIMARY KEY UNIQUE NOT NULL",
+                column_primary_key_unique,
+                column_primary_key_unique.column_constraints,
+                "user_id INTEGER PRIMARY KEY UNIQUE NOT NULL",
         ),
         (
-            column_unique,
-            column_unique.column_constraints,
-            "user_id INTEGER UNIQUE",
+                column_unique,
+                column_unique.column_constraints,
+                "user_id INTEGER UNIQUE",
         ),
         (
-            column_check_constraint,
-            column_check_constraint.column_constraints,
-            "age INTEGER CHECK (age > 18)",
+                column_check_constraint,
+                column_check_constraint.column_constraints,
+                "age INTEGER",
         ),
     ],
 )
 def test_convert_column_definition_to_SQL(column, constraints_list, expected):  # type: ignore
     assert (
-        PostgresColumnOperationConverter.convert_column_definition_to_SQL(
-            column, constraints_list  # type: ignore
-        )
-        == expected
+            PostgresColumnOperationConverter.convert_column_definition_to_SQL(
+                column, constraints_list  # type: ignore
+            )
+            == expected
     )
 
 
 @pytest.mark.parametrize(
     "operation, expected",
     [
         (
-            AddColumnOperation(empty_users_table, simple_column_no_constraints),
-            "ALTER TABLE users ADD COLUMN name TEXT;",
+                AddColumnOperation(empty_users_table, simple_column_no_constraints),
+                "ALTER TABLE users ADD COLUMN name TEXT;",
         ),
         (
-            AddColumnOperation(empty_users_table, column_primary_key_unique),
-            "ALTER TABLE users ADD COLUMN user_id INTEGER PRIMARY KEY UNIQUE NOT NULL;",
+                AddColumnOperation(empty_users_table, column_primary_key_unique),
+                "ALTER TABLE users ADD COLUMN user_id INTEGER PRIMARY KEY UNIQUE NOT NULL;",
         ),
         (
-            AddColumnOperation(
-                empty_users_table,
-                column_unique,
-                related_foreign_key=ForeignKeyConstraint(
-                    empty_users_table.name, "people", {"user_id": "person_id"}
+                AddColumnOperation(
+                    empty_users_table,
+                    column_unique,
+                    related_foreign_key=ForeignKeyConstraint(
+                        empty_users_table.name, "people", {"user_id": "person_id"}
+                    ),
                 ),
-            ),
-            "ALTER TABLE users ADD COLUMN user_id INTEGER UNIQUE REFERENCES people (person_id);",
+                "ALTER TABLE users ADD COLUMN user_id INTEGER UNIQUE REFERENCES people (person_id);",
         ),
         (
-            AddColumnOperation(empty_users_table, column_check_constraint),
-            "ALTER TABLE users ADD COLUMN age INTEGER CHECK (age > 18);",
+                AddColumnOperation(empty_users_table, column_check_constraint,
+                                   related_check_constraint=CheckConstraint("users", "age > 18")),
+                "ALTER TABLE users ADD COLUMN age INTEGER CHECK (age > 18);",
         ),
         (
-            DeleteColumnOperation(empty_users_table, simple_column_no_constraints),
-            "ALTER TABLE users DROP COLUMN name;",
+                DeleteColumnOperation(empty_users_table, simple_column_no_constraints),
+                "ALTER TABLE users DROP COLUMN name;",
         ),
         (
-            DeleteColumnOperation(empty_users_table, column_primary_key_unique),
-            "ALTER TABLE users DROP COLUMN user_id;",
+                DeleteColumnOperation(empty_users_table, column_primary_key_unique),
+                "ALTER TABLE users DROP COLUMN user_id;",
         ),
         (
-            DeleteColumnOperation(empty_users_table, column_unique),
-            "ALTER TABLE users DROP COLUMN user_id;",
+                DeleteColumnOperation(empty_users_table, column_unique),
+                "ALTER TABLE users DROP COLUMN user_id;",
         ),
         (
-            DeleteColumnOperation(empty_users_table, column_check_constraint),
-            "ALTER TABLE users DROP COLUMN age;",
+                DeleteColumnOperation(empty_users_table, column_check_constraint),
+                "ALTER TABLE users DROP COLUMN age;",
         ),
         (
-            RenameColumnOperation(
-                empty_users_table, simple_column_no_constraints, "name2"
-            ),
-            "ALTER TABLE users RENAME COLUMN name TO name2;",
+                RenameColumnOperation(
+                    empty_users_table, simple_column_no_constraints, "name2"
+                ),
+                "ALTER TABLE users RENAME COLUMN name TO name2;",
         ),
         (
-            RenameColumnOperation(
-                empty_users_table, column_primary_key_unique, "user_id2"
-            ),
-            "ALTER TABLE users RENAME COLUMN user_id TO user_id2;",
+                RenameColumnOperation(
+                    empty_users_table, column_primary_key_unique, "user_id2"
+                ),
+                "ALTER TABLE users RENAME COLUMN user_id TO user_id2;",
         ),
         (
-            RenameColumnOperation(empty_users_table, column_unique, "user_id2"),
-            "ALTER TABLE users RENAME COLUMN user_id TO user_id2;",
+                RenameColumnOperation(empty_users_table, column_unique, "user_id2"),
+                "ALTER TABLE users RENAME COLUMN user_id TO user_id2;",
         ),
         (
-            RenameColumnOperation(empty_users_table, column_check_constraint, "age2"),
-            "ALTER TABLE users RENAME COLUMN age TO age2;",
+                RenameColumnOperation(empty_users_table, column_check_constraint, "age2"),
+                "ALTER TABLE users RENAME COLUMN age TO age2;",
         ),
     ],
 )
 def test_convert_column_operation_to_SQL(operation, expected):  # type: ignore
     assert (
-        PostgresColumnOperationConverter.convert_column_operation_to_SQL(operation)  # type: ignore
-        == expected
+            PostgresColumnOperationConverter.convert_column_operation_to_SQL(operation)  # type: ignore
+            == expected
     )
 
 
 @pytest.mark.parametrize(
     "operation, expected_error",
     [
         (
-            ChangeDataTypeOperation(
-                empty_users_table, simple_column_no_constraints, "INTEGER"
-            ),
-            UnsupportedOperationError,
+                ChangeDataTypeOperation(
+                    empty_users_table, simple_column_no_constraints, "INTEGER"
+                ),
+                UnsupportedOperationError,
         ),
         (
-            ChangeDataTypeOperation(
-                empty_users_table, column_primary_key_unique, "TEXT"
-            ),
-            UnsupportedOperationError,
+                ChangeDataTypeOperation(
+                    empty_users_table, column_primary_key_unique, "TEXT"
+                ),
+                UnsupportedOperationError,
         ),
         (
-            ChangeDataTypeOperation(empty_users_table, column_unique, "TEXT"),
-            UnsupportedOperationError,
+                ChangeDataTypeOperation(empty_users_table, column_unique, "TEXT"),
+                UnsupportedOperationError,
         ),
         (
-            ChangeDataTypeOperation(empty_users_table, column_check_constraint, "TEXT"),
-            UnsupportedOperationError,
+                ChangeDataTypeOperation(empty_users_table, column_check_constraint, "TEXT"),
+                UnsupportedOperationError,
         ),
     ],
 )
 def test_convert_column_operation_to_SQL_errors(operation, expected_error):  # type: ignore
     with raises(expected_error):  # type: ignore
         PostgresColumnOperationConverter.convert_column_operation_to_SQL(operation)  # type: ignore
```

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/converters/postgres/test_postgres_constraint_conversion.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/converters/postgres/test_postgres_constraint_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             ForeignKeyConstraint(
                 "admins",
                 "users",
                 {"user_id": "id", "address": "address", "group_id": "group"},
             ),
             "FOREIGN KEY (user_id, address, group_id) REFERENCES users (id, address, group)",
         ),
-        (CheckConstraint("users", "age", "> 18"), "CHECK (age > 18)"),
+        (CheckConstraint("users", "age > 18"), "CHECK (age > 18)"),
     ],
 )
 def test_convert_constraint_to_SQL(constraint, expected):  # type: ignore
     """Test the conversion of various constraints to SQL."""
     assert SQLite3ConstraintConverter.convert_constraint_to_SQL(constraint) == expected  # type: ignore
```

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/converters/postgres/test_postgres_table_operations_conversion.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/converters/postgres/test_postgres_table_operations_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,18 +48,18 @@
         PostgresTyping.Column(
             "email", "TEXT", column_constraints=[UniqueConstraint("users", "email")]
         ),
         PostgresTyping.Column("active", "BYTEA", column_constraints=list()),
         PostgresTyping.Column(
             "age",
             "INTEGER",
-            column_constraints=[CheckConstraint("users", "age", "> 18")],
+            column_constraints=[CheckConstraint("users", "age > 18")],
         ),
     ],
-    foreign_keys={
+    table_constraints={
         ForeignKeyConstraint(
             "admin_users", "users", {"active": "active", "name": "name"}
         )
     },
 )
```

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,18 +34,17 @@
     "user_id",
     "INTEGER",
     column_constraints=[
         UniqueConstraint("users", "user_id"),
     ],
 )
 
-column_check_constraint = SQLite3Typing.Column(
+age_column = SQLite3Typing.Column(
     "age",
     "INTEGER",
-    column_constraints=[CheckConstraint("users", "age", "> 18")],
 )
 
 empty_users_table = SQLite3Typing.Table("users", columns=[])
 
 
 def test_simple_column_definition():
     assert (
@@ -70,23 +69,14 @@
         SQLite3ColumnOperationConverter.convert_column_definition_to_SQL(
             column_unique, column_unique.column_constraints
         )
         == "user_id INTEGER UNIQUE"
     )
 
 
-def test_column_definition_with_check_constraint():
-    assert (
-        SQLite3ColumnOperationConverter.convert_column_definition_to_SQL(
-            column_check_constraint, column_check_constraint.column_constraints
-        )
-        == "age INTEGER CHECK (age > 18)"
-    )
-
-
 def test_add_simple_column():
     operation = AddColumnOperation(empty_users_table, simple_column_no_constraints)
     assert (
         SQLite3ColumnOperationConverter.convert_column_operation_to_SQL(operation)
         == "ALTER TABLE users ADD COLUMN name TEXT;"
     )
 
@@ -110,15 +100,19 @@
     assert (
         SQLite3ColumnOperationConverter.convert_column_operation_to_SQL(operation)
         == "ALTER TABLE users ADD COLUMN user_id INTEGER UNIQUE REFERENCES people (person_id);"
     )
 
 
 def test_add_column_with_check_constraint():
-    operation = AddColumnOperation(empty_users_table, column_check_constraint)
+    operation = AddColumnOperation(
+        empty_users_table,
+        age_column,
+        related_check_constraint=CheckConstraint("users", "age > 18"),
+    )
     assert (
         SQLite3ColumnOperationConverter.convert_column_operation_to_SQL(operation)
         == "ALTER TABLE users ADD COLUMN age INTEGER CHECK (age > 18);"
     )
 
 
 def test_drop_simple_column():
@@ -142,15 +136,15 @@
     assert (
         SQLite3ColumnOperationConverter.convert_column_operation_to_SQL(operation)
         == "ALTER TABLE users DROP COLUMN user_id;"
     )
 
 
 def test_drop_column_with_check_constraint():
-    operation = DeleteColumnOperation(empty_users_table, column_check_constraint)
+    operation = DeleteColumnOperation(empty_users_table, age_column)
     assert (
         SQLite3ColumnOperationConverter.convert_column_operation_to_SQL(operation)
         == "ALTER TABLE users DROP COLUMN age;"
     )
 
 
 def test_rename_simple_column():
@@ -178,17 +172,15 @@
     assert (
         SQLite3ColumnOperationConverter.convert_column_operation_to_SQL(operation)
         == "ALTER TABLE users RENAME COLUMN user_id TO user_id2;"
     )
 
 
 def test_rename_column_with_check_constraint():
-    operation = RenameColumnOperation(
-        empty_users_table, column_check_constraint, "age2"
-    )
+    operation = RenameColumnOperation(empty_users_table, age_column, "age2")
     assert (
         SQLite3ColumnOperationConverter.convert_column_operation_to_SQL(operation)
         == "ALTER TABLE users RENAME COLUMN age TO age2;"
     )
 
 
 def test_change_data_type_simple_column():
@@ -211,12 +203,10 @@
     operation = ChangeDataTypeOperation(empty_users_table, column_unique, "TEXT")
 
     with raises(UnsupportedOperationError):
         SQLite3ColumnOperationConverter.convert_column_operation_to_SQL(operation)
 
 
 def test_change_data_type_column_with_check_constraint():
-    operation = ChangeDataTypeOperation(
-        empty_users_table, column_check_constraint, "TEXT"
-    )
+    operation = ChangeDataTypeOperation(empty_users_table, age_column, "TEXT")
     with raises(UnsupportedOperationError):
         SQLite3ColumnOperationConverter.convert_column_operation_to_SQL(operation)
```

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from pytest import raises
 from skibidi_orm.exceptions.constraints import UnsupportedConstraintError
-from skibidi_orm.migration_engine.converters.sqlite3.constraints import SQLite3ConstraintConverter
+from skibidi_orm.migration_engine.converters.sqlite3.constraints import (
+    SQLite3ConstraintConverter,
+)
 from skibidi_orm.migration_engine.adapters.database_objects.constraints import (
     PrimaryKeyConstraint,
     UniqueConstraint,
     ForeignKeyConstraint,
     CheckConstraint,
     DefaultConstraint,
     NotNullConstraint,
@@ -59,12 +61,12 @@
         SQLite3ConstraintConverter.convert_constraint_to_SQL(constraint)
         == "FOREIGN KEY (user_id, address, group_id) REFERENCES users (id, address, group)"
     )
 
 
 def test_check_constraint_conversion():
     """Test the conversion of a CheckConstraint to SQL.""" ""
-    constraint = CheckConstraint("users", "age", "> 18")
+    constraint = CheckConstraint("users", "age > 18")
     assert (
         SQLite3ConstraintConverter.convert_constraint_to_SQL(constraint)
         == "CHECK (age > 18)"
     )
```

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/converters/sqlite3/test_query_conversion.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/converters/sqlite3/test_query_conversion.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py`

 * *Files 19% similar despite different names*

```diff
@@ -53,64 +53,25 @@
         SQLite3Typing.Column(
             "email", "TEXT", column_constraints=[UniqueConstraint("users", "email")]
         ),
         SQLite3Typing.Column("active", "BLOB", column_constraints=list()),
         SQLite3Typing.Column(
             "age",
             "INTEGER",
-            column_constraints=[CheckConstraint("users", "age", "> 18")],
         ),
     ],
-    foreign_keys={
+    table_constraints=[
         ForeignKeyConstraint(
             "admin_users", "users", {"active": "active", "name": "name"}
-        )
-    },
+        ),
+        CheckConstraint("admin_users", "age > 18"),
+    ],
 )
 
 
-@pytest.fixture
-def non_random_constraint_order(monkeypatch: pytest.MonkeyPatch):
-    """Since the actual split_constraints method works on sets, so the
-    order of constraints is not guaranteed, we have to mock it using lists"""
-
-    def split_using_lists(
-        table: SQLite3Typing.Table,
-    ) -> tuple[list[Constraint], list[Constraint]]:
-        all_constraints = list(
-            chain.from_iterable(column.column_constraints for column in table.columns)
-        )
-
-        # TODO: make this dependent on the implementation of the TableOperationConverter instead of
-        #  doing it here
-        constraints_at_end = list(
-            filter(
-                lambda c: c.constraint_type
-                not in [
-                    ConstraintType.PRIMARY_KEY,
-                    ConstraintType.UNIQUE,
-                    ConstraintType.NOT_NULL,
-                ],
-                all_constraints,
-            )
-        )
-
-        constraints_at_columns = [
-            constraint
-            for constraint in all_constraints
-            if constraint not in constraints_at_end
-        ]
-
-        return list(constraints_at_end), list(constraints_at_columns)
-
-    monkeypatch.setattr(
-        SQLite3TableOperationConverter, "split_constraints", split_using_lists
-    )
-
-
 def test_create_table_conversion_simple():
     """Create a simple table"""
     operation = CreateTableOperation(simple_table_no_constraints)
     assert (
         SQLite3TableOperationConverter.convert_table_operation_to_SQL(operation)
         == "CREATE TABLE users (name TEXT);"
     )
@@ -121,23 +82,22 @@
     operation = CreateTableOperation(complex_table_no_constraints)
     assert (
         SQLite3TableOperationConverter.convert_table_operation_to_SQL(operation)
         == "CREATE TABLE users (name TEXT, age INTEGER, email TEXT, active BLOB);"
     )
 
 
-@pytest.mark.usefixtures("non_random_constraint_order")
 def test_create_table_conversion_complex_with_constraints():
     """Create a complex table with multiple constraints"""
     operation = CreateTableOperation(complex_table_with_constraints)
     assert (
         SQLite3TableOperationConverter.convert_table_operation_to_SQL(operation)
         == "CREATE TABLE admin_users (user_id INTEGER PRIMARY KEY NOT NULL, name TEXT, "
-        "email TEXT UNIQUE, active BLOB, age INTEGER, CHECK (age > 18), FOREIGN KEY (active, name) REFERENCES users ("
-        "active, name));"
+        "email TEXT UNIQUE, active BLOB, age INTEGER, FOREIGN KEY (active, name) REFERENCES users ("
+        "active, name), CHECK (age > 18));"
     )
 
 
 def test_delete_table_conversion():
     """Delete a simple table"""
     operation = DeleteTableOperation(simple_table_no_constraints)
     assert (
```

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/db_config/test_config.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/db_config/test_config.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/db_config/test_postgres_config.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/db_config/test_postgres_config.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/db_inspector/test_postgres_inspector.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/db_inspector/test_postgres_inspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,19 +322,14 @@
             [PostgresTablesData.SQL_TABLE_DIFFERECT_CONSTRAINTS],
             "table_different_constraints",
             "integer_not_nullable",
             [
                 c.NotNullConstraint(
                     "table_different_constraints", "integer_not_nullable"
                 ),
-                c.CheckConstraint(
-                    "table_different_constraints",
-                    "integer_not_nullable",
-                    "((integer_not_nullable > 100))",
-                ),
             ],
         ),
         (  # 3
             [PostgresTablesData.SQL_TABLE_DIFFERECT_CONSTRAINTS],
             "table_different_constraints",
             "unique_column",
             [c.UniqueConstraint("table_different_constraints", "unique_column")],
@@ -371,19 +366,14 @@
             [
                 c.NotNullConstraint(
                     "table_different_constraints", "not_null_unique_check_column"
                 ),
                 c.UniqueConstraint(
                     "table_different_constraints", "not_null_unique_check_column"
                 ),
-                c.CheckConstraint(
-                    "table_different_constraints",
-                    "not_null_unique_check_column",
-                    "((not_null_unique_check_column > 100))",
-                ),
             ],
         ),
         (  # 8
             PostgresTablesData.SQL_TABLE_SIMPLE_FOREIGN_KEYS,
             "authors",
             "id",
             [
@@ -430,19 +420,14 @@
                 ),
                 c.UniqueConstraint(
                     "table_different_constraints", "not_null_unique_check_default"
                 ),
                 c.DefaultConstraint(
                     "table_different_constraints", "not_null_unique_check_default", "1"
                 ),
-                c.CheckConstraint(
-                    "table_different_constraints",
-                    "not_null_unique_check_default",
-                    "((not_null_unique_check_default > 100))",
-                ),
             ],
         ),
         (  # 13
             [PostgresTablesData.SQL_TABLE_SERIALS],
             "table_serials",
             "serial_pk",
             [
@@ -707,19 +692,14 @@
                 PostgresTyping.Column(
                     name="integer_not_nullable",
                     data_type="INTEGER",
                     column_constraints=[
                         c.NotNullConstraint(
                             "table_different_constraints", "integer_not_nullable"
                         ),
-                        c.CheckConstraint(
-                            "table_different_constraints",
-                            "integer_not_nullable",
-                            "((integer_not_nullable > 100))",
-                        ),
                     ],
                 ),
                 PostgresTyping.Column(
                     name="text_nullable",
                     data_type="TEXT",
                     column_constraints=[],
                 ),
@@ -766,19 +746,14 @@
                             "table_different_constraints",
                             "not_null_unique_check_column",
                         ),
                         c.UniqueConstraint(
                             "table_different_constraints",
                             "not_null_unique_check_column",
                         ),
-                        c.CheckConstraint(
-                            "table_different_constraints",
-                            "not_null_unique_check_column",
-                            "((not_null_unique_check_column > 100))",
-                        ),
                     ],
                 ),
                 PostgresTyping.Column(
                     name="not_null_unique",
                     data_type="INTEGER",
                     column_constraints=[
                         c.NotNullConstraint(
@@ -814,19 +789,14 @@
                             "not_null_unique_check_default",
                         ),
                         c.DefaultConstraint(
                             "table_different_constraints",
                             "not_null_unique_check_default",
                             "1",
                         ),
-                        c.CheckConstraint(
-                            "table_different_constraints",
-                            "not_null_unique_check_default",
-                            "((not_null_unique_check_default > 100))",
-                        ),
                     ],
                 ),
             ],
         ),
     ],
 )
 def test_get_table_columns(query, table_name, expected_columns):  # type: ignore
```

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/db_mutators/test_postgres_mutator.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/db_mutators/test_postgres_mutator.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     DeleteRowPk,
     InsertRowColumn,
 )
 from skibidi_orm.migration_engine.data_mutator.sqlite3_data_mutatorr import (
     SQLite3DataMutator,
 )
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
-from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
+from skibidi_orm.migration_engine.db_inspectors.sqlite.sqlite3_inspector import (
     SQLite3Inspector,
 )
 from ..sql_data import SQLite3InsertData, SQLite3TablesData
 
 
 @pytest.mark.parametrize(
     "make_database", [[*SQLite3TablesData.sql_simple_db]], indirect=True
```

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/operations/test_operations.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/operations/test_operations.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/revisions/test_manager_sqlite.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/revisions/test_manager_sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     ForeignKeyConstraint,
 )
 from skibidi_orm.migration_engine.adapters.sqlite3_typing import (
     SQLite3Typing,
 )
 from skibidi_orm.migration_engine.adapters.providers import DatabaseProvider
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
-from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
+from skibidi_orm.migration_engine.db_inspectors.sqlite.sqlite3_inspector import (
     SQLite3Inspector,
 )
 from skibidi_orm.migration_engine.revisions.manager import RevisionManager
 from skibidi_orm.migration_engine.revisions.revision import Revision
 import pytest
 
 sql_schema_with_fks = [
```

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/sql_data.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/sql_data.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
-from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
+from skibidi_orm.migration_engine.db_inspectors.sqlite.sqlite3_inspector import (
     SQLite3Inspector,
 )
 from skibidi_orm.migration_engine.adapters.database_objects.constraints import (
     PrimaryKeyConstraint,
 )
 from skibidi_orm.migration_engine.sql_executor.sqlite3_executor import SQLite3Executor
```

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pathlib
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
-from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
+from skibidi_orm.migration_engine.db_inspectors.sqlite.sqlite3_inspector import (
     SQLite3Inspector,
 )
 from skibidi_orm.migration_engine.studio.utils.get_db_inspector import get_db_inspector
 import py  # type: ignore
 
 
 def write_temp_schema_file(file_path: str, file_content: str):
```

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/studio/test_routes.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/studio/test_routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from fastapi.testclient import TestClient
 import pytest
 from skibidi_orm.migration_engine.data_mutator.sqlite3_data_mutatorr import (
     SQLite3DataMutator,
 )
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
-from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
+from skibidi_orm.migration_engine.db_inspectors.sqlite.sqlite3_inspector import (
     SQLite3Inspector,
 )
 from skibidi_orm.migration_engine.studio.server import app
 import pathlib
 from ..sql_data import SQLite3TablesData
 
 client = TestClient(app)
```

### Comparing `skibidi_orm-0.1.31/tests/skibidi-orm/migration_engine/test_module_cooperation.py` & `skibidi_orm-0.1.35/tests/skibidi-orm/migration_engine/test_module_cooperation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from skibidi_orm.migration_engine.adapters.sqlite3_typing import (
     SQLite3Typing,
 )
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
-from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
+from skibidi_orm.migration_engine.db_inspectors.sqlite.sqlite3_inspector import (
     SQLite3Inspector,
 )
 from skibidi_orm.migration_engine.sql_executor.sqlite3_executor import SQLite3Executor
 from skibidi_orm.migration_engine.adapters.sqlite3_adapter import SQLite3Adapter
 from skibidi_orm.migration_engine.adapters.database_objects.migration_element import (
     MigrationElement,
 )
```

### Comparing `skibidi_orm-0.1.31/PKG-INFO` & `skibidi_orm-0.1.35/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: SkiBiDi-ORM
-Version: 0.1.31
+Version: 0.1.35
 Summary: Python ORM
 Author-Email: xDepcio <olek.drwal@gmail.com>, jedrzej-grabski <grabski.dev@gmail.com>, mbienkowski <bienkowski.maksym@gmail.com>
 License: MIT
 Requires-Python: >=3.12
 Requires-Dist: typer>=0.11.0
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: python-dotenv>=1.0.1
 Requires-Dist: freezegun>=1.5.1
 Requires-Dist: fastapi>=0.111.0
+Requires-Dist: prompt-toolkit>=3.0.45
 Requires-Dist: black>=24.4.2
 Requires-Dist: psycopg2-binary>=2.9.9
 Requires-Dist: pdoc3>=0.10.0
 Description-Content-Type: text/markdown
 
 # zprp-23z-python-orm
 * [Migration engine](#migration-engine)
@@ -77,15 +78,15 @@
 
 Above we defined simple implementation of `Table` class which works as a base model for all SQL tables in our databse.
 
 Normally `Table` class would be abstracted away by proprietary library, but for the sake of example we defined it here.
 
 When he have defined our schema all interactions of end-user with the migration engine are done through CLI.
 
-# `skibidi-orm CLI`
+# `skibidi-orm`
 
 CLI tool for managing schema creations and migrations in Skibidi ORM.
 
 **Usage**:
 
 ```console
 $ skibidi-orm [OPTIONS] COMMAND [ARGS]...
@@ -97,45 +98,45 @@
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `go`: Go back (and forward) to specific migration.
-* `list-migrations`: List all made migrations with their...
+* `log`: List all migration revisions with their...
 * `migrate`: Used to run migration for current schema...
 * `preview-migration`: Preview the migration that will be executed.
 * `studio`: Run web UI for CRUD operations on current DB.
 
 ## `skibidi-orm go`
 
 Go back (and forward) to specific migration.
 
 **Usage**:
 
 ```console
-$ skibidi-orm go [OPTIONS] [MIGRATION_ID]
+$ skibidi-orm go [OPTIONS] MIGRATION_ID
 ```
 
 **Arguments**:
 
-* `[MIGRATION_ID]`: Migration ID
+* `MIGRATION_ID`: Migration ID  [required]
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
-## `skibidi-orm list-migrations`
+## `skibidi-orm log`
 
-List all made migrations with their descriptions and ID.
+List all migration revisions with their descriptions and ID.
 
 **Usage**:
 
 ```console
-$ skibidi-orm list-migrations [OPTIONS]
+$ skibidi-orm log [OPTIONS]
 ```
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 ## `skibidi-orm migrate`
```

