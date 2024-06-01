# Comparing `tmp/skibidi_orm-0.1.21.tar.gz` & `tmp/skibidi_orm-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skibidi_orm-0.1.21.tar", last modified: Fri May 31 12:48:48 2024, max compression
+gzip compressed data, was "skibidi_orm-0.1.22.tar", last modified: Sat Jun  1 02:14:09 2024, max compression
```

## Comparing `skibidi_orm-0.1.21.tar` & `skibidi_orm-0.1.22.tar`

### file list

```diff
@@ -1,110 +1,123 @@
--rw-r--r--   0        0        0       26 2024-05-31 12:48:35.997451 skibidi_orm-0.1.21/README.md
--rw-r--r--   0        0        0      776 2024-05-31 12:48:48.045357 skibidi_orm-0.1.21/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/__init__.py
--rw-r--r--   0        0        0     2653 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/cli/run.py
--rw-r--r--   0        0        0      596 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/cli/utils.py
--rw-r--r--   0        0        0      136 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/exceptions/cli_exceptions.py
--rw-r--r--   0        0        0      190 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/exceptions/constraints.py
--rw-r--r--   0        0        0      172 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/exceptions/db_mutator_exceptions.py
--rw-r--r--   0        0        0      309 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/exceptions/operations.py
--rw-r--r--   0        0        0        0 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/__init__.py
--rw-r--r--   0        0        0        0 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/__init__.py
--rw-r--r--   0        0        0     1299 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/base_adapter.py
--rw-r--r--   0        0        0        0 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/database_objects/__init__.py
--rw-r--r--   0        0        0     2192 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py
--rw-r--r--   0        0        0      901 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py
--rw-r--r--   0        0        0     1614 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py
--rw-r--r--   0        0        0      515 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py
--rw-r--r--   0        0        0     3410 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/base/interfaces.py
--rw-r--r--   0        0        0     1065 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/all.py
--rw-r--r--   0        0        0     3904 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py
--rw-r--r--   0        0        0     1974 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py
--rw-r--r--   0        0        0     5440 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py
--rw-r--r--   0        0        0     1053 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py
--rw-r--r--   0        0        0     2508 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py
--rw-r--r--   0        0        0     1062 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_config/base_config.py
--rw-r--r--   0        0        0      192 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_config/postgres_config.py
--rw-r--r--   0        0        0      392 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_config/sqlite3_config.py
--rw-r--r--   0        0        0      671 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py
--rw-r--r--   0        0        0     6025 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py
--rw-r--r--   0        0        0     6589 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/operations/column_operations.py
--rw-r--r--   0        0        0      280 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/operations/operation_type.py
--rw-r--r--   0        0        0     2286 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/operations/table_operations.py
--rw-r--r--   0        0        0      585 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py
--rw-r--r--   0        0        0     2173 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py
--rw-r--r--   0        0        0      694 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py
--rw-r--r--   0        0        0     5556 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/state_manager/state_manager.py
--rw-r--r--   0        0        0     3113 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/server.py
--rw-r--r--   0        0        0      436 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.eslintrc.cjs
--rw-r--r--   0        0        0      248 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.gitignore
--rw-r--r--   0        0        0     1300 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md
--rw-r--r--   0        0        0      339 2024-05-31 12:48:36.001451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/components.json
--rw-r--r--   0        0        0  2063635 2024-05-31 12:48:36.009451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js
--rw-r--r--   0        0        0   318663 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css
--rw-r--r--   0        0        0      283 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index.lazy-CokS8x6w.js
--rw-r--r--   0        0        0      464 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/index.html
--rw-r--r--   0        0        0     1497 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg
--rw-r--r--   0        0        0      366 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/index.html
--rw-r--r--   0        0        0     1617 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json
--rw-r--r--   0        0        0   134211 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0       80 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/postcss.config.js
--rw-r--r--   0        0        0     1497 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg
--rw-r--r--   0        0        0     4126 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg
--rw-r--r--   0        0        0      926 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx
--rw-r--r--   0        0        0     1038 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx
--rw-r--r--   0        0        0     1337 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx
--rw-r--r--   0        0        0     2121 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx
--rw-r--r--   0        0        0     1377 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx
--rw-r--r--   0        0        0     1322 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx
--rw-r--r--   0        0        0     1730 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx
--rw-r--r--   0        0        0     1835 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx
--rw-r--r--   0        0        0      315 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/collapsible.tsx
--rw-r--r--   0        0        0     3835 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx
--rw-r--r--   0        0        0     7295 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx
--rw-r--r--   0        0        0     1709 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx
--rw-r--r--   0        0        0      772 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx
--rw-r--r--   0        0        0     1361 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts
--rw-r--r--   0        0        0     1529 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts
--rw-r--r--   0        0        0     1224 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts
--rw-r--r--   0        0        0     1054 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts
--rw-r--r--   0        0        0      945 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts
--rw-r--r--   0        0        0     1140 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx
--rw-r--r--   0        0        0     1726 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx
--rw-r--r--   0        0        0     1595 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css
--rw-r--r--   0        0        0      764 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts
--rw-r--r--   0        0        0      355 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/table-data-utils.ts
--rw-r--r--   0        0        0      166 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/utils.ts
--rw-r--r--   0        0        0      790 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx
--rw-r--r--   0        0        0     1409 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts
--rw-r--r--   0        0        0     1173 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx
--rw-r--r--   0        0        0      343 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/index.lazy.tsx
--rw-r--r--   0        0        0     7445 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx
--rw-r--r--   0        0        0     1211 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css
--rw-r--r--   0        0        0       38 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/vite-env.d.ts
--rw-r--r--   0        0        0     2143 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js
--rw-r--r--   0        0        0      711 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json
--rw-r--r--   0        0        0      233 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.node.json
--rw-r--r--   0        0        0      378 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/vite.config.ts
--rw-r--r--   0        0        0      617 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py
--rw-r--r--   0        0        0      784 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py
--rw-r--r--   0        0        0      566 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py
--rw-r--r--   0        0        0     3476 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/table_example.py
--rw-r--r--   0        0        0        0 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/tests/skibidi-orm/__init__.py
--rw-r--r--   0        0        0        0 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/tests/skibidi-orm/cli/schema.py
--rw-r--r--   0        0        0     2136 2024-05-31 12:48:36.013451 skibidi_orm-0.1.21/tests/skibidi-orm/cli/test_run.py
--rw-r--r--   0        0        0     1654 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/conftest.py
--rw-r--r--   0        0        0     7281 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py
--rw-r--r--   0        0        0     2619 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py
--rw-r--r--   0        0        0     4963 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py
--rw-r--r--   0        0        0     1447 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/db_config/test_config.py
--rw-r--r--   0        0        0     6182 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/db_inspector/test_db_inspectors.py
--rw-r--r--   0        0        0     9737 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py
--rw-r--r--   0        0        0     7425 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/operations/test_operations.py
--rw-r--r--   0        0        0      967 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py
--rw-r--r--   0        0        0    17111 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py
--rw-r--r--   0        0        0     2146 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py
--rw-r--r--   0        0        0      805 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py
--rw-r--r--   0        0        0      736 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py
--rw-r--r--   0        0        0     4268 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_routes.py
--rw-r--r--   0        0        0    17767 2024-05-31 12:48:36.017451 skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/test_module_cooperation.py
--rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 skibidi_orm-0.1.21/PKG-INFO
+-rw-r--r--   0        0        0       26 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/README.md
+-rw-r--r--   0        0        0      912 2024-06-01 02:14:09.029414 skibidi_orm-0.1.22/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/__init__.py
+-rw-r--r--   0        0        0     3929 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/cli/run.py
+-rw-r--r--   0        0        0     1976 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/cli/utils.py
+-rw-r--r--   0        0        0      136 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/exceptions/cli_exceptions.py
+-rw-r--r--   0        0        0       93 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/exceptions/config_exceptions.py
+-rw-r--r--   0        0        0      190 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/exceptions/constraints.py
+-rw-r--r--   0        0        0      172 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/exceptions/db_mutator_exceptions.py
+-rw-r--r--   0        0        0      309 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/exceptions/operations.py
+-rw-r--r--   0        0        0        0 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/__init__.py
+-rw-r--r--   0        0        0     1501 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/base_adapter.py
+-rw-r--r--   0        0        0        0 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/database_objects/__init__.py
+-rw-r--r--   0        0        0     2567 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py
+-rw-r--r--   0        0        0      901 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py
+-rw-r--r--   0        0        0     1384 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/postgres_adapter.py
+-rw-r--r--   0        0        0     1227 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/postgres_typing.py
+-rw-r--r--   0        0        0     1614 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py
+-rw-r--r--   0        0        0      515 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py
+-rw-r--r--   0        0        0     3410 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/base/interfaces.py
+-rw-r--r--   0        0        0     1065 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/sqlite3/all.py
+-rw-r--r--   0        0        0     3904 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py
+-rw-r--r--   0        0        0     1974 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py
+-rw-r--r--   0        0        0     5440 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py
+-rw-r--r--   0        0        0     1053 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py
+-rw-r--r--   0        0        0     2508 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py
+-rw-r--r--   0        0        0     1062 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_config/base_config.py
+-rw-r--r--   0        0        0     1624 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_config/postgres_config.py
+-rw-r--r--   0        0        0      419 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_config/sqlite3_config.py
+-rw-r--r--   0        0        0      671 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py
+-rw-r--r--   0        0        0     8810 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_inspectors/postgres_inspector.py
+-rw-r--r--   0        0        0     6025 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py
+-rw-r--r--   0        0        0     6589 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/operations/column_operations.py
+-rw-r--r--   0        0        0      280 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/operations/operation_type.py
+-rw-r--r--   0        0        0     2286 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/operations/table_operations.py
+-rw-r--r--   0        0        0      585 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py
+-rw-r--r--   0        0        0     2173 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py
+-rw-r--r--   0        0        0      694 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py
+-rw-r--r--   0        0        0     5556 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/state_manager/state_manager.py
+-rw-r--r--   0        0        0     3113 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/server.py
+-rw-r--r--   0        0        0      436 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.eslintrc.cjs
+-rw-r--r--   0        0        0      248 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.gitignore
+-rw-r--r--   0        0        0     1300 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md
+-rw-r--r--   0        0        0      339 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/components.json
+-rw-r--r--   0        0        0  2063635 2024-06-01 02:13:56.609404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js
+-rw-r--r--   0        0        0   318663 2024-06-01 02:13:56.609404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css
+-rw-r--r--   0        0        0      283 2024-06-01 02:13:56.609404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index.lazy-CokS8x6w.js
+-rw-r--r--   0        0        0      464 2024-06-01 02:13:56.609404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/index.html
+-rw-r--r--   0        0        0     1497 2024-06-01 02:13:56.609404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg
+-rw-r--r--   0        0        0      366 2024-06-01 02:13:56.609404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/index.html
+-rw-r--r--   0        0        0     1617 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json
+-rw-r--r--   0        0        0   134211 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0       80 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/postcss.config.js
+-rw-r--r--   0        0        0     1497 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg
+-rw-r--r--   0        0        0     4126 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg
+-rw-r--r--   0        0        0      926 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx
+-rw-r--r--   0        0        0     1038 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0     1337 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx
+-rw-r--r--   0        0        0     2121 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx
+-rw-r--r--   0        0        0     1377 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx
+-rw-r--r--   0        0        0     1322 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx
+-rw-r--r--   0        0        0     1730 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx
+-rw-r--r--   0        0        0     1835 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx
+-rw-r--r--   0        0        0      315 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/collapsible.tsx
+-rw-r--r--   0        0        0     3835 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx
+-rw-r--r--   0        0        0     7295 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx
+-rw-r--r--   0        0        0     1709 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx
+-rw-r--r--   0        0        0      772 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx
+-rw-r--r--   0        0        0     1361 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts
+-rw-r--r--   0        0        0     1529 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts
+-rw-r--r--   0        0        0     1224 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts
+-rw-r--r--   0        0        0     1054 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts
+-rw-r--r--   0        0        0      945 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts
+-rw-r--r--   0        0        0     1140 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx
+-rw-r--r--   0        0        0     1726 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx
+-rw-r--r--   0        0        0     1595 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css
+-rw-r--r--   0        0        0      764 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts
+-rw-r--r--   0        0        0      355 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/table-data-utils.ts
+-rw-r--r--   0        0        0      166 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/utils.ts
+-rw-r--r--   0        0        0      790 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx
+-rw-r--r--   0        0        0     1409 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts
+-rw-r--r--   0        0        0     1173 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx
+-rw-r--r--   0        0        0      343 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/index.lazy.tsx
+-rw-r--r--   0        0        0     7445 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx
+-rw-r--r--   0        0        0     1211 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css
+-rw-r--r--   0        0        0       38 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0     2143 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js
+-rw-r--r--   0        0        0      711 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json
+-rw-r--r--   0        0        0      233 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.node.json
+-rw-r--r--   0        0        0      378 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/vite.config.ts
+-rw-r--r--   0        0        0      617 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py
+-rw-r--r--   0        0        0      784 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py
+-rw-r--r--   0        0        0      566 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py
+-rw-r--r--   0        0        0     3476 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/table_example.py
+-rw-r--r--   0        0        0        0 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/cli/schema.py
+-rw-r--r--   0        0        0     2136 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/cli/test_run.py
+-rw-r--r--   0        0        0        0 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/__init__.py
+-rw-r--r--   0        0        0     3175 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/conftest.py
+-rw-r--r--   0        0        0      758 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/constraints/test_constraints.py
+-rw-r--r--   0        0        0     7281 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py
+-rw-r--r--   0        0        0     2619 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py
+-rw-r--r--   0        0        0     4963 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py
+-rw-r--r--   0        0        0     1632 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_config/test_config.py
+-rw-r--r--   0        0        0     1590 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_config/test_postgres_config.py
+-rw-r--r--   0        0        0        0 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_inspector/__init__.py
+-rw-r--r--   0        0        0     5122 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_inspector/test_db_inspectors.py
+-rw-r--r--   0        0        0    33839 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_inspector/test_postgres_inspector.py
+-rw-r--r--   0        0        0        0 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_mutators/__init__.py
+-rw-r--r--   0        0        0     9681 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py
+-rw-r--r--   0        0        0     7425 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/operations/test_operations.py
+-rw-r--r--   0        0        0     7372 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/sql_data.py
+-rw-r--r--   0        0        0      967 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py
+-rw-r--r--   0        0        0        0 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/state_manager/__init__.py
+-rw-r--r--   0        0        0    16079 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py
+-rw-r--r--   0        0        0        0 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/__init__.py
+-rw-r--r--   0        0        0     2200 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py
+-rw-r--r--   0        0        0      805 2024-06-01 02:13:56.617404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py
+-rw-r--r--   0        0        0      736 2024-06-01 02:13:56.617404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py
+-rw-r--r--   0        0        0     3281 2024-06-01 02:13:56.617404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_routes.py
+-rw-r--r--   0        0        0    17534 2024-06-01 02:13:56.617404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/test_module_cooperation.py
+-rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 skibidi_orm-0.1.22/PKG-INFO
```

### Comparing `skibidi_orm-0.1.21/pyproject.toml` & `skibidi_orm-0.1.22/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "SkiBiDi-ORM"
-version = "0.1.21"
+version = "0.1.22"
 description = "Python ORM"
 authors = [
     { name = "xDepcio", email = "olek.drwal@gmail.com" },
     { name = "jedrzej-grabski", email = "jedrzej@grabski.pl" },
     { name = "mbienkowski", email = "bienkowski.maksym@gmail.com" },
 ]
 dependencies = [
     "typer>=0.11.0",
     "colorama>=0.4.6",
     "fastapi>=0.111.0",
+    "psycopg2-binary>=2.9.9",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
@@ -33,7 +34,12 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=8.1.1",
 ]
 
 [tool.pdm.scripts]
 tests = "pytest --verbose --color=yes --ignore ./tmp"
+
+[tool.pytest.ini_options]
+markers = [
+    "slow: mark test as slow (deselect with '-m \"not slow\"')",
+]
```

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/cli/run.py` & `skibidi_orm-0.1.22/src/skibidi_orm/cli/run.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,112 @@
 # This file can by run by executing `skibidi-orm` in the terminal, after the package is installed.
 # `skibidi-orm migrate [--message <STRING>]`
 # `skibidi-orm list-migrations`
 # `skibidi-orm go <MIGRATION_ID>`
 
 
+from pathlib import Path
 import typer
 from typing import Union
 import os
 
 # import shutil
 import sys
-from skibidi_orm.cli.utils import find_schema_file
+from skibidi_orm.cli.utils import find_schema_file, load_schema_from_path
 from skibidi_orm.exceptions.cli_exceptions import MultipleSchemaFilesError
 from skibidi_orm.migration_engine.adapters.database_objects.migration_element import (
     MigrationElement,
 )
 from skibidi_orm.migration_engine.studio.server import run_server
 from colorama import Fore
 
 sys.path.insert(0, os.getcwd())
 
 
 app = typer.Typer(
     help="CLI tool for managing schema creations and migrations in Skibidi ORM."
 )
+state = {"schema_path": Path()}
+
+
+@app.callback()
+def schema_callback(
+    schema_path: Union[None, Path] = typer.Option(
+        None,
+        "--schema-file",
+        "-s",
+        help="Specify an external schema file path",
+        show_default=False,
+    )
+):
+    """
+    Specify a path to the schema file to use.
+    """
+
+    if schema_path is not None:
+        state["schema_path"] = schema_path
+
+        try:
+            load_schema_from_path(str(schema_path))
+            print("\nSchema file successfully loaded.\n")
+
+        except FileNotFoundError:
+            print("\nSchema file could not be found. Aborting.\n")
+            raise typer.Exit(code=1)
+
+        except ImportError:
+            print("\nSchema file could not be loaded. Aborting.\n")
+            raise typer.Exit(code=1)
+
+    else:
+        try:
+            import schema as schema  # type: ignore
+
+            print("\nSchema file successfully loaded.\n")
+
+        except ImportError:
+            print("\nSchema file could not be loaded. Aborting.\n")
+            raise typer.Exit(code=1)
 
 
 @app.command()
 def migrate(
     message: str = typer.Option(
-        None, "--message", "-m", help="Description of migration"
+        None,
+        "--message",
+        "-m",
+        help="Description of migration",
     )
 ):
     """
     Used to run migration for current schema file. Can accept an optional message as a description of the migration.
     """
     m = MigrationElement()
     m.migrate(preview=False)
+
+    print("\nMigration complete. \n")
+
     pass
 
 
 @app.command(name="preview-migration")
 def preview_migration():
     """
     Preview the migration that will be executed.
     """
+
     m = MigrationElement()
     m.migrate(preview=True)
 
     if not m.operations:
         print("No changes to be made.")
     else:
+        print("Migration preview:")
         for i, operation in enumerate(m.operations):
-            print(f"{i+1}) {operation}")
+            print(f"\t{i+1}) {operation}")
     pass
 
 
 @app.command(name="list-migrations")
 def migrate_list():
     """
     List all made migrations with their descriptions and ID.
@@ -83,28 +133,31 @@
     schema_file: Union[str, None] = typer.Option(
         None, "--schema-file", "-s", help="Schema file path"
     )
 ):
     """
     Run web UI for CRUD operations on current DB.
     """
-    if schema_file is not None:
-        run_server(schema_file=schema_file)
-        return
 
     try:
-        schema_file = find_schema_file()
-        run_server(schema_file=schema_file)
+        if schema_file is None:
+            schema_file = find_schema_file()
     except MultipleSchemaFilesError:
         print(
             Fore.RED
             + "Multiple schema files found. Please specify the schema file to use: --schema-file <PATH>"
         )
         raise typer.Exit(code=1)
 
+    try:
+        run_server(schema_file=schema_file)
+    except Exception as e:
+        print(Fore.RED + f"Error: {e}")
+        raise typer.Exit(code=1)
+
 
 def main():
     app()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/base_adapter.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/base_adapter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
+from functools import total_ordering
 from typing import Any
 
 from skibidi_orm.migration_engine.adapters.database_objects.constraints import (
     ColumnSpecificConstraint,
     ForeignKeyConstraint,
 )
 
 
+@total_ordering
 @dataclass(unsafe_hash=True)
 class BaseColumn[TDataTypes]:
     """
     Base column class that has to be properly implemented by the database specific column class.
     """
 
     name: str
     data_type: TDataTypes
     column_constraints: list[ColumnSpecificConstraint] = field(
         default_factory=list, hash=False
     )
 
+    def __lt__(self, other: Any):
+        if isinstance(other, BaseColumn):
+            return self.name < other.name
+        return NotImplemented
+
 
 @dataclass
 class BaseTable[TCol]:
     """
     Base table class that has to be properly implemented by the database specific table class.
     """
```

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+from __future__ import annotations
 from abc import ABC
 import enum
 from dataclasses import dataclass, field
+from functools import total_ordering
+from typing import Any
 
 
 class ConstraintType(enum.Enum):
     """All supported constraint types"""
 
     NOT_NULL = "NOT NULL"
     UNIQUE = "UNIQUE"
@@ -18,20 +21,28 @@
 class Constraint(ABC):
     """Base class for all constraints"""
 
     constraint_type: ConstraintType = field(init=False)
     table_name: str
 
 
+@total_ordering
 @dataclass(frozen=True)
 class ColumnSpecificConstraint(Constraint):
     """Base class for constraints that apply to a column instead of multiple (e.g. composite foreign keys)"""
 
     column_name: str
 
+    def __lt__(self, other: Any):
+        if isinstance(other, ColumnSpecificConstraint):
+            return (self.column_name + self.__class__.__name__) < (
+                other.column_name + other.__class__.__name__
+            )
+        return NotImplemented
+
 
 @dataclass(frozen=True)
 class NotNullConstraint(ColumnSpecificConstraint):
     """Class for the NOT NULL constraint"""
 
     constraint_type: ConstraintType = field(init=False, default=ConstraintType.NOT_NULL)
```

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/base/interfaces.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/base/interfaces.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/all.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/sqlite3/all.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_config/base_config.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_config/base_config.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/operations/column_operations.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/operations/column_operations.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/operations/table_operations.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/operations/table_operations.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/state_manager/state_manager.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/state_manager/state_manager.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/server.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/server.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/src/skibidi_orm/migration_engine/table_example.py` & `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/table_example.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/tests/skibidi-orm/cli/test_run.py` & `skibidi_orm-0.1.22/tests/skibidi-orm/cli/test_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,9 +63,9 @@
     file_path = tmpdir.join("schema.py")  # type: ignore
     file_path.write("")  # type: ignore
 
     result = runner.invoke(
         app, ["studio", "--schema-file", file_path.strpath]  # type: ignore
     )
 
-    assert "Success test" == result.stdout
+    assert "Success test" in result.stdout
     tmpdir.remove()
```

### Comparing `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py` & `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py` & `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py` & `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/db_config/test_config.py` & `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_config/test_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 from skibidi_orm.migration_engine.db_config.postgres_config import PostgresConfig
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
+import os
 
 
 def test_should_raise_error_on_invalid_insantiation():
     """
     We cannot instantiate more than one config
     """
     with pytest.raises(RuntimeError) as exc_info:
@@ -15,26 +16,32 @@
 
 def test_should_raise_error_when_instantiating_other_config():
     """
     Should raise error when trying to instantiate other config after one has been instantiated
     """
     SQLite3Config(db_path="first_path")
     with pytest.raises(RuntimeError) as exc_info:
-        PostgresConfig(db_path="first_path")
+        PostgresConfig(
+            db_name="db_name",
+            db_user="db_user",
+            db_password="db_password",
+            db_host="db_host",
+            db_port=5432,
+        )
     assert str(exc_info.value) == "Only one instance of this class is allowed"
 
 
 def test_accessing_through_instance_method_should_throw_error_when_instance_does_not_exist():
     """
     Should raise error when trying to access instance method when instance does not exist
     """
     with pytest.raises(ReferenceError) as exc_info:
         SQLite3Config.get_instance()
     assert str(exc_info.value) == "Instance does not exist"
 
 
 def test_check_argument_saving():
     """
-    Shoud raise error when arugments are not saved
+    Should raise error when arguments are not saved
     """
     config = SQLite3Config(db_path="first_path")
-    assert config.db_path == "first_path"
+    assert config.db_path == os.path.join(os.getcwd(), "first_path")
```

### Comparing `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py` & `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,46 +16,20 @@
 from skibidi_orm.migration_engine.data_mutator.sqlite3_data_mutatorr import (
     SQLite3DataMutator,
 )
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
     SQLite3Inspector,
 )
+from ..sql_data import SQLite3InsertData, SQLite3TablesData
 
-sql_simple_db = [
-    """
-    CREATE TABLE users (
-        user_id INTEGER PRIMARY KEY,
-        username TEXT NOT NULL
-    );
-"""
-]
-
-sql_double_pk_db = [
-    """
-    CREATE TABLE Orders (
-        order_id INTEGER,
-        product_id INTEGER,
-        PRIMARY KEY (order_id, product_id)
-    );
-"""
-]
-
-sql_simple_insert = [
-    """
-    INSERT INTO users (user_id, username) VALUES
-    (1, 'test1'),
-    (2, 'test2'),
-    (3, 'test3')
-;
-"""
-]
 
-
-@pytest.mark.parametrize("make_database", [[*sql_simple_db]], indirect=True)
+@pytest.mark.parametrize(
+    "make_database", [[*SQLite3TablesData.sql_simple_db]], indirect=True
+)
 def test_insert_row(make_database: str):
     SQLite3Config(db_path=make_database)
     db_seeder = SQLite3DataMutator()
     db_seeder.insert_row(
         table_name="users",
         row=[
             InsertRowColumn(name="user_id", value=str(1)),
@@ -82,15 +56,17 @@
                     NotNullConstraint(table_name="users", column_name="username"),
                 ],
             ),
         ],
     )
 
 
-@pytest.mark.parametrize("make_database", [[*sql_simple_db]], indirect=True)
+@pytest.mark.parametrize(
+    "make_database", [[*SQLite3TablesData.sql_simple_db]], indirect=True
+)
 def test_delete_row_one_pk(make_database: str):
     config = SQLite3Config(db_path=make_database)
     db_seeder = SQLite3DataMutator()
 
     db_seeder.insert_row(
         table_name="users",
         row=[
@@ -119,15 +95,17 @@
         cursor.execute("SELECT * FROM users")
         data = cursor.fetchall()
         cursor.close()
 
     assert len(data) == 0
 
 
-@pytest.mark.parametrize("make_database", [[*sql_double_pk_db]], indirect=True)
+@pytest.mark.parametrize(
+    "make_database", [[*SQLite3TablesData.sql_double_pk_db]], indirect=True
+)
 def test_delete_row_two_pk(make_database: str):
     config = SQLite3Config(db_path=make_database)
     db_seeder = SQLite3DataMutator()
     db_seeder.insert_row(
         table_name="Orders",
         row=[
             InsertRowColumn(name="order_id", value=str(1)),
@@ -156,15 +134,17 @@
         cursor.execute("SELECT * FROM Orders")
         data = cursor.fetchall()
         cursor.close()
 
     assert len(data) == 0
 
 
-@pytest.mark.parametrize("make_database", [[*sql_double_pk_db]], indirect=True)
+@pytest.mark.parametrize(
+    "make_database", [[*SQLite3TablesData.sql_double_pk_db]], indirect=True
+)
 def test_delete_row_table_two_pk_one_pk_given_ok(make_database: str):
     config = SQLite3Config(db_path=make_database)
     db_seeder = SQLite3DataMutator()
     db_seeder.insert_row(
         table_name="Orders",
         row=[
             InsertRowColumn(name="order_id", value=str(1)),
@@ -200,15 +180,17 @@
         data = cursor.fetchall()
         cursor.close()
 
     assert len(data) == 1
     assert data[0] == (1, 1)
 
 
-@pytest.mark.parametrize("make_database", [[*sql_double_pk_db]], indirect=True)
+@pytest.mark.parametrize(
+    "make_database", [[*SQLite3TablesData.sql_double_pk_db]], indirect=True
+)
 def test_delete_row_table_two_pk_two_pk_given_ok(make_database: str):
     config = SQLite3Config(db_path=make_database)
     db_seeder = SQLite3DataMutator()
     db_seeder.insert_row(
         table_name="Orders",
         row=[
             InsertRowColumn(name="order_id", value=str(1)),
@@ -245,15 +227,17 @@
         data = cursor.fetchall()
         cursor.close()
 
     assert len(data) == 1
     assert data[0] == (1, 1)
 
 
-@pytest.mark.parametrize("make_database", [[*sql_double_pk_db]], indirect=True)
+@pytest.mark.parametrize(
+    "make_database", [[*SQLite3TablesData.sql_double_pk_db]], indirect=True
+)
 def test_delete_row_table_two_pk_one_pk_given_ambigious(make_database: str):
     config = SQLite3Config(db_path=make_database)
     db_seeder = SQLite3DataMutator()
     db_seeder.insert_row(
         table_name="Orders",
         row=[
             InsertRowColumn(name="order_id", value=str(1)),
@@ -282,49 +266,57 @@
             pks=[
                 DeleteRowPk(name="order_id", value=str(1)),
             ],
         )
 
 
 @pytest.mark.parametrize(
-    "make_database", [[*sql_simple_db, *sql_simple_insert]], indirect=True
+    "make_database",
+    [[*SQLite3TablesData.sql_simple_db, *SQLite3InsertData.sql_simple_insert]],
+    indirect=True,
 )
 def test_raw_query(make_database: str):
     SQLite3Config(db_path=make_database)
     db_mutator = SQLite3DataMutator()
     data = db_mutator.raw_query("SELECT * FROM users;")
     assert data == [(1, "test1"), (2, "test2"), (3, "test3")]
 
 
 @pytest.mark.parametrize(
-    "make_database", [[*sql_simple_db, *sql_simple_insert]], indirect=True
+    "make_database",
+    [[*SQLite3TablesData.sql_simple_db, *SQLite3InsertData.sql_simple_insert]],
+    indirect=True,
 )
 def test_get_rows_normal(make_database: str):
     SQLite3Config(db_path=make_database)
     db_mutator = SQLite3DataMutator()
     data = db_mutator.get_rows("users")
     assert data == [(1, "test1"), (2, "test2"), (3, "test3")]
 
 
 @pytest.mark.parametrize(
-    "make_database", [[*sql_simple_db, *sql_simple_insert]], indirect=True
+    "make_database",
+    [[*SQLite3TablesData.sql_simple_db, *SQLite3InsertData.sql_simple_insert]],
+    indirect=True,
 )
 def test_get_rows_offset(make_database: str):
     SQLite3Config(db_path=make_database)
     db_mutator = SQLite3DataMutator()
     data = db_mutator.get_rows("users", offset=1)
     assert data == [(2, "test2"), (3, "test3")]
     data = db_mutator.get_rows("users", offset=2)
     assert data == [(3, "test3")]
     data = db_mutator.get_rows("users", offset=3)
     assert data == []
 
 
 @pytest.mark.parametrize(
-    "make_database", [[*sql_simple_db, *sql_simple_insert]], indirect=True
+    "make_database",
+    [[*SQLite3TablesData.sql_simple_db, *SQLite3InsertData.sql_simple_insert]],
+    indirect=True,
 )
 def test_get_rows_limit(make_database: str):
     SQLite3Config(db_path=make_database)
     db_mutator = SQLite3DataMutator()
     data = db_mutator.get_rows("users", limit=1)
     assert data == [(1, "test1")]
     data = db_mutator.get_rows("users", limit=2)
```

### Comparing `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/operations/test_operations.py` & `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/operations/test_operations.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py` & `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py` & `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,75 +21,15 @@
 )
 
 # from tmp.mock_schema import Table
 
 from pathlib import Path
 import pytest
 import sqlite3
-
-sql_table_user = """
-    CREATE TABLE User (
-        user_id INTEGER PRIMARY KEY,
-        user_name TEXT NOT NULL
-    );
-"""
-sql_table_post = """
-    CREATE TABLE Post (
-        post_id INTEGER PRIMARY KEY,
-        post_name TEXT NOT NULL
-    );
-"""
-
-sql_table_comment = """
-    CREATE TABLE Comment (
-        comment_id INTEGER PRIMARY KEY,
-        comment_name TEXT NOT NULL
-    );
-"""
-
-sql_table_primary_key_not_null = """
-    CREATE TABLE table_primary_key_not_null (
-        id INTEGER PRIMARY KEY NOT NULL
-    );
-"""
-
-
-# TODO: what is this?
-# sql_schema_with_fks = [
-#     """
-#     CREATE TABLE users (
-#         user_id INTEGER PRIMARY KEY,
-#         username TEXT NOT NULL UNIQUE,
-#         email TEXT NOT NULL UNIQUE,
-#         password_hash TEXT NOT NULL,
-#         registration_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
-#     );
-# """,
-#     """
-#     CREATE TABLE posts (
-#         post_id INTEGER PRIMARY KEY,
-#         user_id INTEGER NOT NULL,
-#         title TEXT NOT NULL,
-#         content TEXT NOT NULL,
-#         post_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
-#         FOREIGN KEY (user_id) REFERENCES users(user_id)
-#     );
-# """,
-#     """
-#     CREATE TABLE comments (
-#         comment_id INTEGER PRIMARY KEY,
-#         user_idd INTEGER NOT NULL,
-#         post_id INTEGER NOT NULL,
-#         comment_text TEXT NOT NULL,
-#         comment_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
-#         FOREIGN KEY (user_idd) REFERENCES users(user_id),
-#         FOREIGN KEY (post_id) REFERENCES posts(post_id)
-#     );
-# """,
-# ]
+from ..sql_data import SQLite3TablesData
 
 
 def execute_sqlite3_commands(db_path: str, commands: list[str]):
     """Executes the given commands in a SQLite DB living under db_path"""
     with sqlite3.connect(db_path) as conn:
         cursor = conn.cursor()
         for command in commands:
@@ -123,15 +63,17 @@
         SQLite3Executor,
         "execute_operations",
         do_nothing,  # type: ignore
     )
 
 
 @pytest.mark.parametrize(
-    "tmp_database", [[sql_table_user, sql_table_post]], indirect=True
+    "tmp_database",
+    [[SQLite3TablesData.sql_table_user, SQLite3TablesData.sql_table_post]],
+    indirect=True,
 )
 def test_rename_table_operation_needed(
     tmp_database: str, capfd: pytest.CaptureFixture[str]
 ):
     from skibidi_orm.migration_engine.adapters.database_objects.migration_element import (
         MigrationElement,
     )
@@ -184,15 +126,17 @@
     m.migrate(preview=True)
 
     assert type(MigrationElement.operations[0]) == RenameTableOperation
     assert len(MigrationElement.operations) == 1
 
 
 @pytest.mark.parametrize(
-    "tmp_database", [[sql_table_user, sql_table_post]], indirect=True
+    "tmp_database",
+    [[SQLite3TablesData.sql_table_user, SQLite3TablesData.sql_table_post]],
+    indirect=True,
 )
 def test_no_operation_needed(
     tmp_database: str, mock_execute_operations: pytest.MonkeyPatch
 ):
     # TODO: refactor to avoid duplicating the setup multiple times
     class Table(MigrationElement):
 
@@ -241,15 +185,17 @@
     m = MigrationElement()
     m.migrate(preview=True)
 
     assert len(MigrationElement.operations) == 0
 
 
 @pytest.mark.parametrize(
-    "tmp_database", [[sql_table_user, sql_table_post]], indirect=True
+    "tmp_database",
+    [[SQLite3TablesData.sql_table_user, SQLite3TablesData.sql_table_post]],
+    indirect=True,
 )
 def test_create_table_operation_needed(
     tmp_database: str, mock_execute_operations: pytest.MonkeyPatch
 ):
 
     class Table(MigrationElement):
 
@@ -316,15 +262,23 @@
     m.migrate(preview=True)
 
     assert type(MigrationElement.operations[0]) == CreateTableOperation
     assert len(MigrationElement.operations) == 1
 
 
 @pytest.mark.parametrize(
-    "tmp_database", [[sql_table_user, sql_table_post, sql_table_comment]], indirect=True
+    "tmp_database",
+    [
+        [
+            SQLite3TablesData.sql_table_user,
+            SQLite3TablesData.sql_table_post,
+            SQLite3TablesData.sql_table_comment,
+        ]
+    ],
+    indirect=True,
 )
 def test_delete_table_operation_needed(
     tmp_database: str, mock_execute_operations: pytest.MonkeyPatch
 ):
 
     class Table(MigrationElement):
 
@@ -374,15 +328,17 @@
     m.migrate(preview=True)
 
     assert len(MigrationElement.operations) == 1
     assert type(MigrationElement.operations[0]) == DeleteTableOperation
 
 
 @pytest.mark.parametrize(
-    "tmp_database", [[sql_table_user, sql_table_post]], indirect=True
+    "tmp_database",
+    [[SQLite3TablesData.sql_table_user, SQLite3TablesData.sql_table_post]],
+    indirect=True,
 )
 def test_create_column_operation_needed(
     tmp_database: str, mock_execute_operations: pytest.MonkeyPatch
 ):
 
     class Table(MigrationElement):
 
@@ -437,15 +393,17 @@
     m.migrate(preview=True)
 
     assert type(MigrationElement.operations[0]) == AddColumnOperation
     assert len(MigrationElement.operations) == 1
 
 
 @pytest.mark.parametrize(
-    "tmp_database", [[sql_table_user, sql_table_post]], indirect=True
+    "tmp_database",
+    [[SQLite3TablesData.sql_table_user, SQLite3TablesData.sql_table_post]],
+    indirect=True,
 )
 def test_delete_column_operation_needed(
     tmp_database: str, mock_execute_operations: pytest.MonkeyPatch
 ):
 
     class Table(MigrationElement):
 
@@ -490,15 +448,23 @@
     m.migrate(preview=True)
 
     assert type(MigrationElement.operations[0]) == DeleteColumnOperation
     assert len(MigrationElement.operations) == 1
 
 
 @pytest.mark.parametrize(
-    "tmp_database", [[sql_table_user, sql_table_post, sql_table_comment]], indirect=True
+    "tmp_database",
+    [
+        [
+            SQLite3TablesData.sql_table_user,
+            SQLite3TablesData.sql_table_post,
+            SQLite3TablesData.sql_table_comment,
+        ]
+    ],
+    indirect=True,
 )
 def test_add_column_and_delete_tabe_operation_needed(
     tmp_database: str, mock_execute_operations: pytest.MonkeyPatch
 ):
     class Table(MigrationElement):
 
         def __init__(self) -> None:
```

### Comparing `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py` & `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,28 +24,28 @@
         """from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 SQLite3Config(db_path="some/path/to/db.db")"""
     )
     str(schema_file)
     db_config = db_config_dynamic_import(schema_file_path=str(schema_file))
 
     assert isinstance(db_config, SQLite3Config)
-    assert db_config.db_path == "some/path/to/db.db"
+    assert db_config.db_path == os.path.join(os.getcwd(), "some/path/to/db.db")
     assert BaseDbConfig.get_instance() == db_config
 
 
 def test_db_config_dynamic_import_normal2(tmp_path: pathlib.Path):
     schema_file = tmp_path.joinpath("schema_test_db_config_dynamic_import_normal2.py")
     schema_file.write_text(
         """from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 SQLite3Config(db_path="some/path/to/db.db")"""
     )
     db_config = db_config_dynamic_import(schema_file_path=str(schema_file))
 
     assert isinstance(db_config, SQLite3Config)
-    assert db_config.db_path == "some/path/to/db.db"
+    assert db_config.db_path == os.path.join(os.getcwd(), "some/path/to/db.db")
     assert BaseDbConfig.get_instance() == db_config
 
 
 def test_db_config_dynamic_import_file_not_exists():
     schema_file = os.getcwd() + "/tmp/not_existant.py"
     with pytest.raises(FileNotFoundError):
         db_config_dynamic_import(schema_file_path=schema_file)
```

### Comparing `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py` & `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py` & `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/studio/test_routes.py` & `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_routes.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,62 +7,22 @@
 )
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
     SQLite3Inspector,
 )
 from skibidi_orm.migration_engine.studio.server import app
 import pathlib
-
+from ..sql_data import SQLite3TablesData
 
 client = TestClient(app)
 
-sql_schema_with_fks = [
-    """
-    CREATE TABLE users (
-        user_id INTEGER PRIMARY KEY,
-        username TEXT NOT NULL UNIQUE,
-        email TEXT NOT NULL UNIQUE,
-        password_hash TEXT NOT NULL,
-        registration_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
-    );
-""",
-    """
-    CREATE TABLE posts (
-        post_id INTEGER PRIMARY KEY,
-        user_id INTEGER NOT NULL,
-        title TEXT NOT NULL,
-        content TEXT NOT NULL,
-        post_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
-        FOREIGN KEY (user_id) REFERENCES users(user_id)
-    );
-""",
-    """
-    CREATE TABLE comments (
-        comment_id INTEGER PRIMARY KEY,
-        user_idd INTEGER NOT NULL,
-        post_id INTEGER NOT NULL,
-        comment_text TEXT NOT NULL,
-        comment_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
-        FOREIGN KEY (user_idd) REFERENCES users(user_id),
-        FOREIGN KEY (post_id) REFERENCES posts(post_id)
-    );
-""",
-]
-
-sql_simple_db = [
-    """
-    CREATE TABLE users (
-        user_id INTEGER PRIMARY KEY,
-        username TEXT NOT NULL UNIQUE
-    );
-"""
-]
-
 
-@pytest.mark.parametrize("make_database", [[*sql_simple_db]], indirect=True)
+@pytest.mark.parametrize(
+    "make_database", [[*SQLite3TablesData.sql_simple_db]], indirect=True
+)
 def test_GET_db(
     monkeypatch: pytest.MonkeyPatch, tmp_path: pathlib.Path, make_database: str
 ):
     import skibidi_orm.migration_engine.studio.server  # type: ignore
 
     importlib.import_module("skibidi_orm.migration_engine.studio.server")
 
@@ -104,15 +64,17 @@
                     ],
                 }
             ]
         }
     )
 
 
-@pytest.mark.parametrize("make_database", [[*sql_simple_db]], indirect=True)
+@pytest.mark.parametrize(
+    "make_database", [[*SQLite3TablesData.sql_simple_db]], indirect=True
+)
 def test_POST_route_db_table_name_row_correct(
     monkeypatch: pytest.MonkeyPatch, make_database: str
 ):
     import skibidi_orm.migration_engine.studio.server  # type: ignore
 
     importlib.import_module("skibidi_orm.migration_engine.studio.server")
```

### Comparing `skibidi_orm-0.1.21/tests/skibidi-orm/migration_engine/test_module_cooperation.py` & `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/test_module_cooperation.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,47 +7,21 @@
 )
 from skibidi_orm.migration_engine.sql_executor.sqlite3_executor import SQLite3Executor
 from skibidi_orm.migration_engine.adapters.sqlite3_adapter import SQLite3Adapter
 from skibidi_orm.migration_engine.adapters.database_objects.migration_element import (
     MigrationElement,
 )
 from skibidi_orm.migration_engine.adapters.database_objects import constraints as c
-
-
-sql_table_user = """
-    CREATE TABLE User (
-        user_id INTEGER PRIMARY KEY,
-        user_name TEXT NOT NULL
-    );
-"""
-sql_table_post = """
-    CREATE TABLE Post (
-        post_id INTEGER PRIMARY KEY,
-        post_name TEXT NOT NULL
-    );
-"""
-
-sql_table_comment = """
-    CREATE TABLE Comment (
-        comment_id INTEGER PRIMARY KEY,
-        comment_name TEXT NOT NULL
-    );
-"""
-
-sql_table_primary_key_not_null = """
-    CREATE TABLE table_primary_key_not_null (
-        id INTEGER PRIMARY KEY NOT NULL
-    );
-"""
+from .sql_data import SQLite3TablesData
 
 
 def test_adding_table_to_database(make_database: str):
     SQLite3Config(make_database)
-    SQLite3Executor.execute_sql(sql_table_user)
-    SQLite3Executor.execute_sql(sql_table_post)
+    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_user)
+    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_post)
 
     class Table(MigrationElement):
         def __init__(self) -> None:
             self.adapter = SQLite3Adapter()
 
             models = Table.__subclasses__()
             if self.__class__ == Table:
@@ -120,17 +94,17 @@
     assert tables[2].columns[1].column_constraints == [
         c.NotNullConstraint("Comment", "comment_name")
     ]
 
 
 def test_removing_table_from_database(make_database: str):
     SQLite3Config(make_database)
-    SQLite3Executor.execute_sql(sql_table_user)
-    SQLite3Executor.execute_sql(sql_table_post)
-    SQLite3Executor.execute_sql(sql_table_comment)
+    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_user)
+    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_post)
+    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_comment)
 
     class Table(MigrationElement):
 
         def __init__(self) -> None:
             self.adapter = SQLite3Adapter()
 
             models = Table.__subclasses__()
@@ -201,16 +175,16 @@
     assert tables[1].columns[1].column_constraints == [
         c.NotNullConstraint("Post", "post_name")
     ]
 
 
 def test_add_column_to_database(make_database: str):
     SQLite3Config(make_database)
-    SQLite3Executor.execute_sql(sql_table_user)
-    SQLite3Executor.execute_sql(sql_table_post)
+    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_user)
+    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_post)
 
     class Table(MigrationElement):
 
         def __init__(self) -> None:
             self.adapter = SQLite3Adapter()
 
             models = Table.__subclasses__()
@@ -291,16 +265,16 @@
     assert tables[1].columns[2].column_constraints == [
         c.NotNullConstraint("Post", "post_content")
     ]
 
 
 def test_removing_column_from_database(make_database: str):
     SQLite3Config(make_database)
-    SQLite3Executor.execute_sql(sql_table_user)
-    SQLite3Executor.execute_sql(sql_table_post)
+    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_user)
+    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_post)
 
     class Table(MigrationElement):
         def __init__(self) -> None:
             self.adapter = SQLite3Adapter()
 
             models = Table.__subclasses__()
             if self.__class__ == Table:
@@ -361,16 +335,16 @@
     assert tables[1].columns[0].column_constraints == [
         c.PrimaryKeyConstraint("Post", "post_id")
     ]
 
 
 def test_renaming_table_in_database(make_database: str):
     SQLite3Config(make_database)
-    SQLite3Executor.execute_sql(sql_table_user)
-    SQLite3Executor.execute_sql(sql_table_post)
+    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_user)
+    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_post)
 
     class Table(MigrationElement):
 
         def __init__(self) -> None:
             self.adapter = SQLite3Adapter()
 
             models = Table.__subclasses__()
@@ -439,17 +413,17 @@
     assert tables[1].columns[1].column_constraints == [
         c.NotNullConstraint("NewNamePost", "post_name")
     ]
 
 
 def test_add_column_to_database_and_remove_table_from_database(make_database: str):
     SQLite3Config(make_database)
-    SQLite3Executor.execute_sql(sql_table_user)
-    SQLite3Executor.execute_sql(sql_table_post)
-    SQLite3Executor.execute_sql(sql_table_comment)
+    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_user)
+    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_post)
+    SQLite3Executor.execute_sql(SQLite3TablesData.sql_table_comment)
 
     class Table(MigrationElement):
 
         def __init__(self) -> None:
             self.adapter = SQLite3Adapter()
 
             models = Table.__subclasses__()
```

