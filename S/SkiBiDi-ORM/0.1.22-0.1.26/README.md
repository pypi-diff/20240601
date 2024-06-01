# Comparing `tmp/skibidi_orm-0.1.22.tar.gz` & `tmp/skibidi_orm-0.1.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skibidi_orm-0.1.22.tar", last modified: Sat Jun  1 02:14:09 2024, max compression
+gzip compressed data, was "skibidi_orm-0.1.26.tar", last modified: Sat Jun  1 19:16:10 2024, max compression
```

## Comparing `skibidi_orm-0.1.22.tar` & `skibidi_orm-0.1.26.tar`

### file list

```diff
@@ -1,123 +1,140 @@
--rw-r--r--   0        0        0       26 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/README.md
--rw-r--r--   0        0        0      912 2024-06-01 02:14:09.029414 skibidi_orm-0.1.22/pyproject.toml
--rw-r--r--   0        0        0        0 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/__init__.py
--rw-r--r--   0        0        0     3929 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/cli/run.py
--rw-r--r--   0        0        0     1976 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/cli/utils.py
--rw-r--r--   0        0        0      136 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/exceptions/cli_exceptions.py
--rw-r--r--   0        0        0       93 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/exceptions/config_exceptions.py
--rw-r--r--   0        0        0      190 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/exceptions/constraints.py
--rw-r--r--   0        0        0      172 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/exceptions/db_mutator_exceptions.py
--rw-r--r--   0        0        0      309 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/exceptions/operations.py
--rw-r--r--   0        0        0        0 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/__init__.py
--rw-r--r--   0        0        0        0 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/__init__.py
--rw-r--r--   0        0        0     1501 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/base_adapter.py
--rw-r--r--   0        0        0        0 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/database_objects/__init__.py
--rw-r--r--   0        0        0     2567 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py
--rw-r--r--   0        0        0      901 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py
--rw-r--r--   0        0        0     1384 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/postgres_adapter.py
--rw-r--r--   0        0        0     1227 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/postgres_typing.py
--rw-r--r--   0        0        0     1614 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py
--rw-r--r--   0        0        0      515 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py
--rw-r--r--   0        0        0     3410 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/base/interfaces.py
--rw-r--r--   0        0        0     1065 2024-06-01 02:13:56.597404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/sqlite3/all.py
--rw-r--r--   0        0        0     3904 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py
--rw-r--r--   0        0        0     1974 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py
--rw-r--r--   0        0        0     5440 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py
--rw-r--r--   0        0        0     1053 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py
--rw-r--r--   0        0        0     2508 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py
--rw-r--r--   0        0        0     1062 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_config/base_config.py
--rw-r--r--   0        0        0     1624 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_config/postgres_config.py
--rw-r--r--   0        0        0      419 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_config/sqlite3_config.py
--rw-r--r--   0        0        0      671 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py
--rw-r--r--   0        0        0     8810 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_inspectors/postgres_inspector.py
--rw-r--r--   0        0        0     6025 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py
--rw-r--r--   0        0        0     6589 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/operations/column_operations.py
--rw-r--r--   0        0        0      280 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/operations/operation_type.py
--rw-r--r--   0        0        0     2286 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/operations/table_operations.py
--rw-r--r--   0        0        0      585 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py
--rw-r--r--   0        0        0     2173 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py
--rw-r--r--   0        0        0      694 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py
--rw-r--r--   0        0        0     5556 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/state_manager/state_manager.py
--rw-r--r--   0        0        0     3113 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/server.py
--rw-r--r--   0        0        0      436 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.eslintrc.cjs
--rw-r--r--   0        0        0      248 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.gitignore
--rw-r--r--   0        0        0     1300 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md
--rw-r--r--   0        0        0      339 2024-06-01 02:13:56.601404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/components.json
--rw-r--r--   0        0        0  2063635 2024-06-01 02:13:56.609404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js
--rw-r--r--   0        0        0   318663 2024-06-01 02:13:56.609404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css
--rw-r--r--   0        0        0      283 2024-06-01 02:13:56.609404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index.lazy-CokS8x6w.js
--rw-r--r--   0        0        0      464 2024-06-01 02:13:56.609404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/index.html
--rw-r--r--   0        0        0     1497 2024-06-01 02:13:56.609404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg
--rw-r--r--   0        0        0      366 2024-06-01 02:13:56.609404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/index.html
--rw-r--r--   0        0        0     1617 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json
--rw-r--r--   0        0        0   134211 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0       80 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/postcss.config.js
--rw-r--r--   0        0        0     1497 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg
--rw-r--r--   0        0        0     4126 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg
--rw-r--r--   0        0        0      926 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx
--rw-r--r--   0        0        0     1038 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx
--rw-r--r--   0        0        0     1337 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx
--rw-r--r--   0        0        0     2121 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx
--rw-r--r--   0        0        0     1377 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx
--rw-r--r--   0        0        0     1322 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx
--rw-r--r--   0        0        0     1730 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx
--rw-r--r--   0        0        0     1835 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx
--rw-r--r--   0        0        0      315 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/collapsible.tsx
--rw-r--r--   0        0        0     3835 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx
--rw-r--r--   0        0        0     7295 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx
--rw-r--r--   0        0        0     1709 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx
--rw-r--r--   0        0        0      772 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx
--rw-r--r--   0        0        0     1361 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts
--rw-r--r--   0        0        0     1529 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts
--rw-r--r--   0        0        0     1224 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts
--rw-r--r--   0        0        0     1054 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts
--rw-r--r--   0        0        0      945 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts
--rw-r--r--   0        0        0     1140 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx
--rw-r--r--   0        0        0     1726 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx
--rw-r--r--   0        0        0     1595 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css
--rw-r--r--   0        0        0      764 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts
--rw-r--r--   0        0        0      355 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/table-data-utils.ts
--rw-r--r--   0        0        0      166 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/utils.ts
--rw-r--r--   0        0        0      790 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx
--rw-r--r--   0        0        0     1409 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts
--rw-r--r--   0        0        0     1173 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx
--rw-r--r--   0        0        0      343 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/index.lazy.tsx
--rw-r--r--   0        0        0     7445 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx
--rw-r--r--   0        0        0     1211 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css
--rw-r--r--   0        0        0       38 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/vite-env.d.ts
--rw-r--r--   0        0        0     2143 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js
--rw-r--r--   0        0        0      711 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json
--rw-r--r--   0        0        0      233 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.node.json
--rw-r--r--   0        0        0      378 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/vite.config.ts
--rw-r--r--   0        0        0      617 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py
--rw-r--r--   0        0        0      784 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py
--rw-r--r--   0        0        0      566 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py
--rw-r--r--   0        0        0     3476 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/table_example.py
--rw-r--r--   0        0        0        0 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/__init__.py
--rw-r--r--   0        0        0        0 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/cli/schema.py
--rw-r--r--   0        0        0     2136 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/cli/test_run.py
--rw-r--r--   0        0        0        0 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/__init__.py
--rw-r--r--   0        0        0     3175 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/conftest.py
--rw-r--r--   0        0        0      758 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/constraints/test_constraints.py
--rw-r--r--   0        0        0     7281 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py
--rw-r--r--   0        0        0     2619 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py
--rw-r--r--   0        0        0     4963 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py
--rw-r--r--   0        0        0     1632 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_config/test_config.py
--rw-r--r--   0        0        0     1590 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_config/test_postgres_config.py
--rw-r--r--   0        0        0        0 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_inspector/__init__.py
--rw-r--r--   0        0        0     5122 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_inspector/test_db_inspectors.py
--rw-r--r--   0        0        0    33839 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_inspector/test_postgres_inspector.py
--rw-r--r--   0        0        0        0 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_mutators/__init__.py
--rw-r--r--   0        0        0     9681 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py
--rw-r--r--   0        0        0     7425 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/operations/test_operations.py
--rw-r--r--   0        0        0     7372 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/sql_data.py
--rw-r--r--   0        0        0      967 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py
--rw-r--r--   0        0        0        0 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/state_manager/__init__.py
--rw-r--r--   0        0        0    16079 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py
--rw-r--r--   0        0        0        0 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/__init__.py
--rw-r--r--   0        0        0     2200 2024-06-01 02:13:56.613404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py
--rw-r--r--   0        0        0      805 2024-06-01 02:13:56.617404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py
--rw-r--r--   0        0        0      736 2024-06-01 02:13:56.617404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py
--rw-r--r--   0        0        0     3281 2024-06-01 02:13:56.617404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_routes.py
--rw-r--r--   0        0        0    17534 2024-06-01 02:13:56.617404 skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/test_module_cooperation.py
--rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 skibidi_orm-0.1.22/PKG-INFO
+-rw-r--r--   0        0        0       26 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/README.md
+-rw-r--r--   0        0        0      988 2024-06-01 19:16:10.568018 skibidi_orm-0.1.26/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/__init__.py
+-rw-r--r--   0        0        0     6714 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/cli/migration_file_creator.py
+-rw-r--r--   0        0        0     4357 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/cli/run.py
+-rw-r--r--   0        0        0     1976 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/cli/utils.py
+-rw-r--r--   0        0        0      136 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/exceptions/cli_exceptions.py
+-rw-r--r--   0        0        0       93 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/exceptions/config_exceptions.py
+-rw-r--r--   0        0        0      190 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/exceptions/constraints.py
+-rw-r--r--   0        0        0      172 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/exceptions/db_mutator_exceptions.py
+-rw-r--r--   0        0        0      309 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/exceptions/operations.py
+-rw-r--r--   0        0        0        0 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/__init__.py
+-rw-r--r--   0        0        0     1501 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/base_adapter.py
+-rw-r--r--   0        0        0        0 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/database_objects/__init__.py
+-rw-r--r--   0        0        0     3393 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py
+-rw-r--r--   0        0        0      901 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py
+-rw-r--r--   0        0        0     1384 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/postgres_adapter.py
+-rw-r--r--   0        0        0     1227 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/postgres_typing.py
+-rw-r--r--   0        0        0      108 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/providers.py
+-rw-r--r--   0        0        0     1614 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py
+-rw-r--r--   0        0        0      528 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py
+-rw-r--r--   0        0        0     4781 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/converters/base/interfaces.py
+-rw-r--r--   0        0        0     1076 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/converters/postgres/all.py
+-rw-r--r--   0        0        0     3922 2024-06-01 19:15:58.915967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/converters/postgres/columns.py
+-rw-r--r--   0        0        0     1980 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/converters/postgres/constraints.py
+-rw-r--r--   0        0        0     5447 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/converters/postgres/tables.py
+-rw-r--r--   0        0        0     1589 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/converters/sqlite3/all.py
+-rw-r--r--   0        0        0     3904 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py
+-rw-r--r--   0        0        0     1974 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py
+-rw-r--r--   0        0        0      809 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/converters/sqlite3/queries.py
+-rw-r--r--   0        0        0     5902 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py
+-rw-r--r--   0        0        0     1053 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py
+-rw-r--r--   0        0        0     1389 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/data_mutator/postgres_data_mutator.py
+-rw-r--r--   0        0        0     2508 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py
+-rw-r--r--   0        0        0     1179 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/db_config/base_config.py
+-rw-r--r--   0        0        0     1755 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/db_config/postgres_config.py
+-rw-r--r--   0        0        0      593 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/db_config/sqlite3_config.py
+-rw-r--r--   0        0        0      671 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py
+-rw-r--r--   0        0        0     8810 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/db_inspectors/postgres_inspector.py
+-rw-r--r--   0        0        0     6385 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py
+-rw-r--r--   0        0        0     7139 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/operations/column_operations.py
+-rw-r--r--   0        0        0      280 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/operations/operation_type.py
+-rw-r--r--   0        0        0     2728 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/operations/table_operations.py
+-rw-r--r--   0        0        0      492 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/revisions/constants.py
+-rw-r--r--   0        0        0     3784 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/revisions/manager.py
+-rw-r--r--   0        0        0     1677 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/revisions/revision.py
+-rw-r--r--   0        0        0     1172 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/sql_executor/base_sql_executor.py
+-rw-r--r--   0        0        0     3083 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py
+-rw-r--r--   0        0        0      694 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py
+-rw-r--r--   0        0        0     5556 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/state_manager/state_manager.py
+-rw-r--r--   0        0        0     3300 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/server.py
+-rw-r--r--   0        0        0      436 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.eslintrc.cjs
+-rw-r--r--   0        0        0      248 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/.gitignore
+-rw-r--r--   0        0        0     1300 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md
+-rw-r--r--   0        0        0      339 2024-06-01 19:15:58.919967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/components.json
+-rw-r--r--   0        0        0  2063635 2024-06-01 19:15:58.927967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js
+-rw-r--r--   0        0        0   318663 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css
+-rw-r--r--   0        0        0      283 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index.lazy-CokS8x6w.js
+-rw-r--r--   0        0        0      464 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/index.html
+-rw-r--r--   0        0        0     1497 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg
+-rw-r--r--   0        0        0      366 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/index.html
+-rw-r--r--   0        0        0     1617 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json
+-rw-r--r--   0        0        0   134211 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0       80 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/postcss.config.js
+-rw-r--r--   0        0        0     1497 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg
+-rw-r--r--   0        0        0     4126 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg
+-rw-r--r--   0        0        0      926 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx
+-rw-r--r--   0        0        0     1038 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0     1337 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx
+-rw-r--r--   0        0        0     2121 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx
+-rw-r--r--   0        0        0     1377 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx
+-rw-r--r--   0        0        0     1322 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx
+-rw-r--r--   0        0        0     1730 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx
+-rw-r--r--   0        0        0     1835 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx
+-rw-r--r--   0        0        0      315 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/collapsible.tsx
+-rw-r--r--   0        0        0     3835 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx
+-rw-r--r--   0        0        0     7295 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx
+-rw-r--r--   0        0        0     1709 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx
+-rw-r--r--   0        0        0      772 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx
+-rw-r--r--   0        0        0     1361 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts
+-rw-r--r--   0        0        0     1529 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts
+-rw-r--r--   0        0        0     1224 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts
+-rw-r--r--   0        0        0     1054 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts
+-rw-r--r--   0        0        0      945 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts
+-rw-r--r--   0        0        0     1140 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx
+-rw-r--r--   0        0        0     1726 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx
+-rw-r--r--   0        0        0     1595 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css
+-rw-r--r--   0        0        0      764 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts
+-rw-r--r--   0        0        0      355 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/table-data-utils.ts
+-rw-r--r--   0        0        0      166 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/utils.ts
+-rw-r--r--   0        0        0      790 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx
+-rw-r--r--   0        0        0     1409 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts
+-rw-r--r--   0        0        0     1173 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx
+-rw-r--r--   0        0        0      343 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/index.lazy.tsx
+-rw-r--r--   0        0        0     7445 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx
+-rw-r--r--   0        0        0     1211 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css
+-rw-r--r--   0        0        0       38 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0     2143 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js
+-rw-r--r--   0        0        0      711 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json
+-rw-r--r--   0        0        0      233 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.node.json
+-rw-r--r--   0        0        0      378 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/vite.config.ts
+-rw-r--r--   0        0        0      617 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py
+-rw-r--r--   0        0        0      785 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py
+-rw-r--r--   0        0        0      798 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py
+-rw-r--r--   0        0        0     3476 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/table_example.py
+-rw-r--r--   0        0        0        0 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/cli/schema.py
+-rw-r--r--   0        0        0     2108 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/cli/test_run.py
+-rw-r--r--   0        0        0        0 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/__init__.py
+-rw-r--r--   0        0        0     3529 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/conftest.py
+-rw-r--r--   0        0        0      758 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/constraints/test_constraints.py
+-rw-r--r--   0        0        0     5780 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/converters/postgres/test_postgres_column_operations_conversion.py
+-rw-r--r--   0        0        0     1908 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/converters/postgres/test_postgres_constraint_conversion.py
+-rw-r--r--   0        0        0     3114 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/converters/postgres/test_postgres_table_operations_conversion.py
+-rw-r--r--   0        0        0     7281 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py
+-rw-r--r--   0        0        0     2619 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py
+-rw-r--r--   0        0        0      960 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/converters/sqlite3/test_query_conversion.py
+-rw-r--r--   0        0        0     5355 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py
+-rw-r--r--   0        0        0     1632 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/db_config/test_config.py
+-rw-r--r--   0        0        0     1590 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/db_config/test_postgres_config.py
+-rw-r--r--   0        0        0        0 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/db_inspector/__init__.py
+-rw-r--r--   0        0        0     8994 2024-06-01 19:15:58.931967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/db_inspector/test_db_inspectors.py
+-rw-r--r--   0        0        0    32628 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/db_inspector/test_postgres_inspector.py
+-rw-r--r--   0        0        0        0 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/db_mutators/__init__.py
+-rw-r--r--   0        0        0     3113 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/db_mutators/test_postgres_mutator.py
+-rw-r--r--   0        0        0     9681 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py
+-rw-r--r--   0        0        0     7425 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/operations/test_operations.py
+-rw-r--r--   0        0        0     5958 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/revisions/test_manager_sqlite.py
+-rw-r--r--   0        0        0     8439 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/sql_data.py
+-rw-r--r--   0        0        0     1530 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/sql_executor/test_sqlite3_executor.py
+-rw-r--r--   0        0        0        0 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/state_manager/__init__.py
+-rw-r--r--   0        0        0    16043 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py
+-rw-r--r--   0        0        0        0 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/studio/__init__.py
+-rw-r--r--   0        0        0     2200 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py
+-rw-r--r--   0        0        0      890 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py
+-rw-r--r--   0        0        0      693 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py
+-rw-r--r--   0        0        0     3281 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/studio/test_routes.py
+-rw-r--r--   0        0        0    17534 2024-06-01 19:15:58.935967 skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/test_module_cooperation.py
+-rw-r--r--   0        0        0      536 1970-01-01 00:00:00.000000 skibidi_orm-0.1.26/PKG-INFO
```

### Comparing `skibidi_orm-0.1.22/pyproject.toml` & `skibidi_orm-0.1.26/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [project]
 name = "SkiBiDi-ORM"
-version = "0.1.22"
+version = "0.1.26"
 description = "Python ORM"
 authors = [
     { name = "xDepcio", email = "olek.drwal@gmail.com" },
-    { name = "jedrzej-grabski", email = "jedrzej@grabski.pl" },
+    { name = "jedrzej-grabski", email = "grabski.dev@gmail.com" },
     { name = "mbienkowski", email = "bienkowski.maksym@gmail.com" },
 ]
 dependencies = [
     "typer>=0.11.0",
     "colorama>=0.4.6",
+    "python-dotenv>=1.0.1",
+    "freezegun>=1.5.1",
     "fastapi>=0.111.0",
+    "black>=24.4.2",
     "psycopg2-binary>=2.9.9",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/cli/run.py` & `skibidi_orm-0.1.26/src/skibidi_orm/cli/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pathlib import Path
 import typer
 from typing import Union
 import os
 
 # import shutil
 import sys
+from skibidi_orm.cli.migration_file_creator import create_migration_file
 from skibidi_orm.cli.utils import find_schema_file, load_schema_from_path
 from skibidi_orm.exceptions.cli_exceptions import MultipleSchemaFilesError
 from skibidi_orm.migration_engine.adapters.database_objects.migration_element import (
     MigrationElement,
 )
 from skibidi_orm.migration_engine.studio.server import run_server
 from colorama import Fore
@@ -71,23 +72,34 @@
 @app.command()
 def migrate(
     message: str = typer.Option(
         None,
         "--message",
         "-m",
         help="Description of migration",
-    )
+    ),
+    direct: bool = typer.Option(
+        False,
+        "--direct",
+        "-d",
+        help="Use --direct to run the migration directly. Without the flag, it will create a python migration file.",
+    ),
 ):
     """
     Used to run migration for current schema file. Can accept an optional message as a description of the migration.
     """
-    m = MigrationElement()
-    m.migrate(preview=False)
 
-    print("\nMigration complete. \n")
+    if direct:
+        m = MigrationElement()
+        m.migrate(preview=False)
+        print("\nMigration complete. \n")
+    else:
+        m = MigrationElement()
+        create_migration_file(m)
+        print("\nMigration file created. \n")
 
     pass
 
 
 @app.command(name="preview-migration")
 def preview_migration():
     """
```

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/cli/utils.py` & `skibidi_orm-0.1.26/src/skibidi_orm/cli/utils.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/base_adapter.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/database_objects/constraints.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,73 +20,88 @@
 @dataclass(frozen=True)
 class Constraint(ABC):
     """Base class for all constraints"""
 
     constraint_type: ConstraintType = field(init=False)
     table_name: str
 
+    def __repr__(self):
+        return f"{self.__class__.__name__}('{self.constraint_type.value}', '{self.table_name}')"
+
 
 @total_ordering
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class ColumnSpecificConstraint(Constraint):
     """Base class for constraints that apply to a column instead of multiple (e.g. composite foreign keys)"""
 
     column_name: str
 
+    def __repr__(self):
+        return f"{self.__class__.__name__}('{self.constraint_type.value}', '{self.column_name}')"
+
     def __lt__(self, other: Any):
         if isinstance(other, ColumnSpecificConstraint):
-            return (self.column_name + self.__class__.__name__) < (
-                other.column_name + other.__class__.__name__
+            return (self.column_name + self.__class__.__name__ + str(self.__dict__)) < (
+                other.column_name + other.__class__.__name__ + str(other.__dict__)
             )
         return NotImplemented
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class NotNullConstraint(ColumnSpecificConstraint):
     """Class for the NOT NULL constraint"""
 
     constraint_type: ConstraintType = field(init=False, default=ConstraintType.NOT_NULL)
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class UniqueConstraint(ColumnSpecificConstraint):
     """Class for the UNIQUE constraint"""
 
     constraint_type: ConstraintType = field(init=False, default=ConstraintType.UNIQUE)
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, repr=False)
 class PrimaryKeyConstraint(ColumnSpecificConstraint):
     """Class for the PRIMARY KEY constraint"""
 
     constraint_type: ConstraintType = field(
         init=False, default=ConstraintType.PRIMARY_KEY
     )
 
 
-@dataclass(frozen=True, unsafe_hash=True)
+@dataclass(frozen=True, unsafe_hash=True, repr=False)
 class ForeignKeyConstraint(Constraint):
     """Class for the FOREIGN KEY constraint"""
 
     constraint_type: ConstraintType = field(
         init=False, default=ConstraintType.FOREIGN_KEY
     )
     referenced_table: str
     column_mapping: dict[str, str] = field(
         hash=False
     )  # maps the corresponding column names: {referencing_column1: referenced_column1, ...}
 
+    def __repr__(self):
+        return f"{self.__class__.__name__}('{self.constraint_type.value}', '{self.table_name}', '{self.referenced_table}', {self.column_mapping})"
 
-@dataclass(frozen=True)
+
+@dataclass(frozen=True, repr=False)
 class CheckConstraint(ColumnSpecificConstraint):
     """Class for the CHECK constraint"""
 
     constraint_type: ConstraintType = field(init=False, default=ConstraintType.CHECK)
     condition: str
 
+    def __repr__(self):
+        return f"{self.__class__.__name__}('{self.constraint_type.value}', '{self.column_name}', '{self.condition}')"
 
-@dataclass(frozen=True)
+
+@dataclass(frozen=True, repr=False)
 class DefaultConstraint(ColumnSpecificConstraint):
     """Class for the DEFAULT constraint"""
 
     constraint_type: ConstraintType = field(init=False, default=ConstraintType.DEFAULT)
     value: str
+
+    def __repr__(self):
+        return f"{self.__class__.__name__}('{self.constraint_type.value}', '{self.column_name}', '{self.value}')"
```

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/database_objects/migration_element.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/postgres_adapter.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/postgres_adapter.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/postgres_typing.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/postgres_typing.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/sqlite3_adapter.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/adapters/sqlite3_typing.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 
 
 class SQLite3Typing:
     """
     Class defining the typing for SQLite3 database objects.
     """
 
-    DataTypes = Literal["TEXT", "INTEGER", "REAL", "BLOB", "NULL"]
+    DataTypes = Literal["TEXT", "INTEGER", "REAL", "BLOB", "NULL", "TIMESTAMP"]
     Constraints = Constraint
     Column = BaseColumn[DataTypes]
     Table = BaseTable[Column]
     tables: list[Table] = []
```

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/converters/sqlite3/columns.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/converters/sqlite3/constraints.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/converters/sqlite3/tables.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     TableOperation,
     CreateTableOperation,
 )
 from skibidi_orm.exceptions.operations import UnsupportedOperationError
 from typing import cast
 from itertools import chain
 
+from skibidi_orm.migration_engine.revisions.constants import get_revision_table_name
+
 
 class SQLite3TableOperationConverter(TableOperationSQLConverter):
     """Class responsible for converting table operation objects to raw SQLite3 SQL strings"""
 
     @staticmethod
     def convert_table_operation_to_SQL(operation: TableOperation) -> str:
         """Convert a given table operation to a SQLite3 SQL string"""
@@ -48,14 +50,21 @@
             )
         else:
             raise UnsupportedOperationError(
                 "The given operation is not supported in SQLite3."
             )
 
     @staticmethod
+    def get_revision_table_creation_query() -> str:
+        """Return the SQL string which creates a special internal table
+        used to hold revision data"""
+        table_name = get_revision_table_name()
+        return f"CREATE TABLE {table_name} (rev REVISION NOT NULL);"
+
+    @staticmethod
     def _convert_create_table_operation_to_SQL(operation: CreateTableOperation) -> str:
         """Convert a given create table operation to a SQLite3 SQL string"""
         definition_string = f"CREATE TABLE {operation.table.name} "
         constraints_at_end, constraints_at_columns = (
             SQLite3TableOperationConverter.split_constraints(operation.table)
         )
 
@@ -113,15 +122,19 @@
         )
 
         """These constraints have to be added at the end of the table definition, not by the
         columns they correspond to"""
         constraints_at_end = set(
             filter(
                 lambda c: c.constraint_type
-                not in [ConstraintType.PRIMARY_KEY, ConstraintType.UNIQUE, ConstraintType.NOT_NULL],
+                not in [
+                    ConstraintType.PRIMARY_KEY,
+                    ConstraintType.UNIQUE,
+                    ConstraintType.NOT_NULL,
+                ],
                 all_constraints,
             )
         )
 
         # These constraints have to be added in the column definition
         constraints_at_columns = all_constraints - constraints_at_end
```

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/data_mutator/base_data_mutator.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/data_mutator/sqlite3_data_mutatorr.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_config/base_config.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/db_config/base_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 from typing import Any, Self
+from skibidi_orm.migration_engine.adapters.providers import DatabaseProvider
 
 
 class BaseDbConfig:
     """
     Base class for all database configurations.
     Ensures that only one instance of all subclasses of this class can be created.
     """
 
     __instance: Any = None
+    database_provider: DatabaseProvider
 
     @classmethod
     def get_instance(cls) -> Self:
         if BaseDbConfig.__instance is None:
             raise ReferenceError("Instance does not exist")
         return BaseDbConfig.__instance
```

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_config/postgres_config.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/db_config/postgres_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import psycopg2
 from skibidi_orm.exceptions.config_exceptions import DbConnectionError
+from skibidi_orm.migration_engine.adapters.providers import DatabaseProvider
 from skibidi_orm.migration_engine.db_config.base_config import (
     BaseDbConfig,
 )
 from psycopg2.extensions import connection as Connection
 
 
 class PostgresConfig(BaseDbConfig):
+
+    database_provider = DatabaseProvider.POSTGRESQL
+
     """
     Configuration class for Postgres database.
     Instantiating it means choosing Postgres as the database.
     """
 
     def __init__(
         self, db_name: str, db_user: str, db_password: str, db_host: str, db_port: int
```

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/db_inspectors/base_inspector.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_inspectors/postgres_inspector.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/db_inspectors/postgres_inspector.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/db_inspectors/sqlite3_inspector.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 from skibidi_orm.migration_engine.db_inspectors.base_inspector import BaseDbInspector
 from skibidi_orm.migration_engine.adapters.sqlite3_typing import (
     SQLite3Typing,
 )
 import skibidi_orm.migration_engine.adapters.database_objects.constraints as c
+from skibidi_orm.migration_engine.revisions.constants import get_revision_table_name
 
 type SQLite3PragmaTableInfo = list[
     tuple[int, str, str, Literal[0, 1], Any, Literal[0, 1]]
 ]
 
 
 @dataclass(frozen=True)
@@ -26,15 +27,14 @@
     on_delete: str
     match: str
 
     @classmethod
     def from_tuple(
         cls,
         values: tuple[str, str, str, str, str, str, str, str],
-        # todo: better typing?
     ) -> PragmaForeignKeyListEntry:
         id, seq, table, from_column, to_column, on_update, on_delete, match = values
         return cls(
             int(id),
             int(seq),
             table,
             from_column,
@@ -62,29 +62,37 @@
     ) -> list[SQLite3Typing.Table]:
         """
         Retrieve all tables from the database.
         """
 
         tables: list[SQLite3Typing.Table] = []
         tables_names = self.get_tables_names()
+        foreign_keys = self.get_foreign_key_constraints()
         for table_name in tables_names:
             table_columns = self.get_table_columns(table_name)
-            tables.append(SQLite3Typing.Table(name=table_name, columns=table_columns))
+            related_fks = {fk for fk in foreign_keys if fk.table_name == table_name}
+            tables.append(
+                SQLite3Typing.Table(
+                    name=table_name, columns=table_columns, foreign_keys=related_fks
+                )
+            )
 
         return tables
 
     def get_tables_names(self) -> list[str]:
         """
         Retrieve just tables names from the database.
         """
 
         tables = self._sqlite_execute(
             "SELECT name FROM sqlite_master WHERE type='table';"
         )
-        return [table[0] for table in tables]
+        return [
+            name for table in tables if (name := table[0]) != get_revision_table_name()
+        ]
 
     @staticmethod
     def foreign_keys_from_pragma_entries(
         table_entry_mapping: dict[str, list[PragmaForeignKeyListEntry]]
     ) -> set[c.ForeignKeyConstraint]:
         """Creates all of the ForeignKeyConstraint objects based on the entries
         gathered from the pragma table"""
```

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/operations/column_operations.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/operations/column_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,18 @@
         """
         return [
             fk
             for fk in self.table.foreign_keys
             if self.column.name in fk.column_mapping
         ]
 
+    @abstractmethod
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(table={self.table}, is_reversible={self.is_reversible})"
+
 
 @dataclass(frozen=True)
 class AddColumnOperation(ColumnOperation):
     """Class for adding a column"""
 
     operation_type: OperationType = field(init=False, default=OperationType.CREATE)
     is_reversible: bool = field(init=False, default=True)
@@ -69,17 +73,22 @@
                     "The only possible key value for the column mapping in an AddColumnOperation is the added column name"
                 )
             if self.table.name != self.related_foreign_key.table_name:
                 raise ValueError(
                     f"""Foreign key constraint initialized with invalid source table name: {self.related_foreign_key.table_name}.
                     Expected: {self.table.name}"""
                 )
+
     def __str__(self) -> str:
         return f"Add Column {self.column.name} to Table {self.table.name}"
 
+    def __repr__(self) -> str:
+        return super().__repr__()
+
+
 @dataclass(frozen=True)
 class DeleteColumnOperation(ColumnOperation):
     """Class for deleting a column"""
 
     operation_type: OperationType = field(init=False, default=OperationType.DELETE)
     is_reversible: bool = field(init=False, default=False)
 
@@ -87,14 +96,17 @@
         raise IrreversibleOperationError(
             f"Reversing a {self.__class__.__name__} is currently not supported."
         )
 
     def __str__(self) -> str:
         return f"Delete Column {self.column.name} from Table {self.table.name}"
 
+    def __repr__(self) -> str:
+        return super().__repr__()
+
 
 @dataclass(frozen=True)
 class RenameColumnOperation(ColumnOperation):
     """Class for renaming a column"""
 
     operation_type: OperationType = field(init=False, default=OperationType.RENAME)
     is_reversible: bool = field(init=False, default=True)
@@ -107,14 +119,17 @@
             column=self.column,
             new_name=self.column.name,
         )
 
     def __str__(self) -> str:
         return f"Rename Column {self.column.name} to {self.new_name} in Table {self.table.name}"
 
+    def __repr__(self) -> str:
+        return super().__repr__()
+
 
 @dataclass(frozen=True)
 class AddConstraintOperation(ColumnOperation):
     """Class for adding a constraint on a column"""
 
     operation_type: OperationType = field(
         init=False, default=OperationType.CONSTRAINT_CHANGE
@@ -129,14 +144,17 @@
             column=self.column,
             constraint=self.constraint,
         )
 
     def __str__(self) -> str:
         return f"Add Constraint {self.constraint.constraint_type.value} to Column {self.column.name} in Table {self.table.name}"
 
+    def __repr__(self) -> str:
+        return super().__repr__()
+
 
 @dataclass(frozen=True)
 class DeleteConstraintOperation(ColumnOperation):
     """Class for deleting a constraint on a column"""
 
     operation_type: OperationType = field(
         init=False, default=OperationType.CONSTRAINT_CHANGE
@@ -151,14 +169,17 @@
             column=self.column,
             constraint=self.constraint,
         )
 
     def __str__(self) -> str:
         return f"Delete Constraint {self.constraint.constraint_type.value} from Column {self.column.name} in Table {self.table.name}"
 
+    def __repr__(self) -> str:
+        return super().__repr__()
+
 
 @dataclass(frozen=True)
 class ChangeDataTypeOperation(ColumnOperation):
     """Class for changing the data type of a column"""
 
     operation_type: OperationType = field(
         init=False, default=OperationType.DTYPE_CHANGE
@@ -171,7 +192,10 @@
             table=self.table,
             column=self.column,
             new_dtype=self.column.data_type,
         )
 
     def __str__(self) -> str:
         return f"Change Data Type of Column {self.column.name} in Table {self.table.name} to {self.new_dtype}"
+
+    def __repr__(self) -> str:
+        return super().__repr__()
```

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/operations/table_operations.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/operations/table_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,28 +17,35 @@
     is_reversible: bool
 
     @abstractmethod
     def reverse(self) -> TableOperation:
         """Generates a table operation that reverses
         the calling instance if possible. Else, throws an exception"""
 
+    @abstractmethod
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(table={self.table}, is_reversible={self.is_reversible})"
 
-@dataclass(frozen=True)
+
+@dataclass(frozen=True, repr=False)
 class CreateTableOperation(TableOperation):
     """Class for creating a table"""
 
     operation_type: OperationType = field(init=False, default=OperationType.CREATE)
     is_reversible: bool = field(init=False, default=True)
 
     def reverse(self) -> TableOperation:
         return DeleteTableOperation(table=self.table)
 
     def __str__(self) -> str:
         return f"Create Table {self.table.name} with columns: {', '.join([col.name for col in self.table.columns])}"
 
+    def __repr__(self) -> str:
+        return super().__repr__()
+
 
 @dataclass(frozen=True)
 class DeleteTableOperation(TableOperation):
     """Class for deleting a table"""
 
     operation_type: OperationType = field(init=False, default=OperationType.DELETE)
     is_reversible: bool = field(init=False, default=False)
@@ -47,14 +54,17 @@
         raise IrreversibleOperationError(
             f"Reversing a {self.__class__.__name__} is currently not supported."
         )
 
     def __str__(self) -> str:
         return f"Delete Table {self.table.name}"
 
+    def __repr__(self) -> str:
+        return super().__repr__()
+
 
 @dataclass(frozen=True)
 class RenameTableOperation(TableOperation):
     """Class for renaming a table"""
 
     operation_type: OperationType = field(init=False, default=OperationType.RENAME)
     is_reversible: bool = field(init=False, default=True)
@@ -62,7 +72,12 @@
 
     def reverse(self) -> TableOperation:
         # todo: make sure it works properly
         return RenameTableOperation(table=self.table, new_name=self.table.name)
 
     def __str__(self) -> str:
         return f"Rename Table {self.table.name} to {self.new_name}"
+
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}(table={self.table}, new_name={self.new_name})"
+        )
```

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/sql_executor/sqlite3_executor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import sqlite3
+from typing import Any
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
+from skibidi_orm.migration_engine.revisions.revision import Revision
 from skibidi_orm.migration_engine.sql_executor.base_sql_executor import BaseSQLExecutor
 from skibidi_orm.migration_engine.operations.column_operations import ColumnOperation
 from skibidi_orm.migration_engine.operations.table_operations import TableOperation
 
 from skibidi_orm.migration_engine.converters.sqlite3.all import SQLite3Converter
 
 
@@ -39,27 +41,51 @@
             for command in commands:
                 if not command:
                     continue
                 cursor.execute(command.strip())
             conn.commit()
 
     @staticmethod
+    def execute_sql_query(sql: str) -> list[Any]:
+        sqlite_config = SQLite3Config.get_instance()
+        with sqlite3.connect(sqlite_config.db_path) as conn:
+            cursor = conn.cursor()
+            result = cursor.execute(sql)
+
+        return result.fetchall()
+
+    @staticmethod
+    def save_revision(revision: Revision):
+        query = SQLite3Converter.get_revision_insertion_query()
+        with sqlite3.connect(
+            SQLite3Config.get_instance().db_path, detect_types=sqlite3.PARSE_DECLTYPES
+        ) as conn:
+            cursor = conn.cursor()
+            cursor.execute(query, (revision,))
+            conn.commit()
+
+    @staticmethod
+    def get_all_revisions() -> list[tuple[int, Revision]]:
+        query = SQLite3Converter.get_revision_data_query()
+        with sqlite3.connect(
+            SQLite3Config.get_instance().db_path, detect_types=sqlite3.PARSE_DECLTYPES
+        ) as conn:
+            cursor = conn.cursor()
+            result = cursor.execute(query)
+            return result.fetchall()
+
+    @staticmethod
     def execute_operations(operations: list[TableOperation | ColumnOperation]):
         """
         Executes a list of table or column operations.
 
         Args:
             operations (list[TableOperation | ColumnOperation]): The list of table or column operations to be executed.
 
         Returns:
             None
 
         """
         for operation in operations:
-            if isinstance(operation, TableOperation):
-                SQLite3Executor.execute_sql(
-                    SQLite3Converter.convert_table_operation_to_SQL(operation)
-                )
-            else:
-                SQLite3Executor.execute_sql(
-                    SQLite3Converter.convert_column_operation_to_SQL(operation)
-                )
+            SQLite3Executor.execute_sql(
+                SQLite3Converter.convert_operation_to_SQL(operation)
+            )
```

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/state_manager/i_state_manager.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/state_manager/state_manager.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/state_manager/state_manager.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/server.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from skibidi_orm.migration_engine.data_mutator.base_data_mutator import (
     BaseDataMutator,
     DeleteRowPk,
     InsertRowColumn,
 )
 from fastapi.middleware.cors import CORSMiddleware
 from skibidi_orm.migration_engine.db_inspectors.base_inspector import BaseDbInspector
+from skibidi_orm.migration_engine.studio.utils.db_config_dynamic_import import (
+    db_config_dynamic_import,
+)
 from skibidi_orm.migration_engine.studio.utils.get_db_inspector import get_db_inspector
 from skibidi_orm.migration_engine.studio.utils.get_db_seeder import get_db_mutator
 
 app = FastAPI()
 db_inspector: BaseDbInspector = cast(
     BaseDbInspector, {}
 )  # to add db_inspector to modules namespace
@@ -40,16 +43,17 @@
     name="static",
 )
 
 
 def run_server(schema_file: str):
     global db_inspector
     global db_mutator
-    db_inspector = get_db_inspector(schema_file=schema_file)
-    db_mutator = get_db_mutator(db_inspector)
+    db_config = db_config_dynamic_import(schema_file_path=schema_file)
+    db_inspector = get_db_inspector(db_config=db_config)
+    db_mutator = get_db_mutator(db_config=db_config)
     uvicorn.run(app, host="0.0.0.0", port=8000)
 
 
 @app.get("/")
 def read_index():
     return FileResponse(
         os.path.join(
```

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/README.md`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CT5dnm0u.js`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/assets/index-CU2I10C2.css`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/package.json`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/public/vite.svg`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Providers.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/Sidebar.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/WorkspaceEditor.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/commands-hisotry-dialog.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/mode-toggle.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/queryResultsTable.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/theme-provider.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/button.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dialog.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/dropdown-menu.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/resizable.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/components/ui/textarea.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/delete-table-row.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/edit-row.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-data.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/get-table-info.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/features/run-command.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandResult.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/hooks/useCommandsHistory.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/index.css`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/lib/react-query.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/main.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routeTree.gen.ts`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/__root.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/routes/table/$tableName.tsx`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/src/styles/ag-custom.css`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/skibidi-orm-studio-frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/utils/db_config_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/utils/get_db_inspector.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+from skibidi_orm.migration_engine.db_config.base_config import BaseDbConfig
 from skibidi_orm.migration_engine.db_config.postgres_config import PostgresConfig
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 from skibidi_orm.migration_engine.db_inspectors.base_inspector import BaseDbInspector
+from skibidi_orm.migration_engine.db_inspectors.postgres_inspector import (
+    PostgresInspector,
+)
 from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
     SQLite3Inspector,
 )
-from skibidi_orm.migration_engine.studio.utils.db_config_dynamic_import import (
-    db_config_dynamic_import,
-)
 
 
-def get_db_inspector(schema_file: str) -> BaseDbInspector:
-    db_config = db_config_dynamic_import(schema_file_path=schema_file)
+def get_db_inspector(db_config: BaseDbConfig) -> BaseDbInspector:
     if isinstance(db_config, SQLite3Config):
         return SQLite3Inspector()
     elif isinstance(db_config, PostgresConfig):
-        raise NotImplementedError
+        return PostgresInspector()
 
     raise NotImplementedError
```

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/studio/utils/get_db_seeder.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from skibidi_orm.migration_engine.data_mutator.base_data_mutator import BaseDataMutator
+from skibidi_orm.migration_engine.data_mutator.postgres_data_mutator import (
+    PostgresDataMutator,
+)
 from skibidi_orm.migration_engine.data_mutator.sqlite3_data_mutatorr import (
     SQLite3DataMutator,
 )
-from skibidi_orm.migration_engine.db_inspectors.base_inspector import BaseDbInspector
-from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
-    SQLite3Inspector,
-)
+from skibidi_orm.migration_engine.db_config.base_config import BaseDbConfig
+from skibidi_orm.migration_engine.db_config.postgres_config import PostgresConfig
+from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 
 
-def get_db_mutator(db_inspector: BaseDbInspector) -> BaseDataMutator:
-    if isinstance(db_inspector, SQLite3Inspector):
+def get_db_mutator(db_config: BaseDbConfig) -> BaseDataMutator:
+    if isinstance(db_config, SQLite3Config):
         return SQLite3DataMutator()
+    elif isinstance(db_config, PostgresConfig):
+        return PostgresDataMutator()
+
     raise NotImplementedError
```

### Comparing `skibidi_orm-0.1.22/src/skibidi_orm/migration_engine/table_example.py` & `skibidi_orm-0.1.26/src/skibidi_orm/migration_engine/table_example.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/cli/test_run.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/cli/test_run.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Callable
 from typer.testing import CliRunner
 import typer
 import pytest
 from skibidi_orm.cli.run import app
 import importlib
 import py  # type: ignore
```

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/conftest.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 from colorama import Style
 import psycopg2
 import pytest
 
 from skibidi_orm.migration_engine.db_config.base_config import (
     BaseDbConfig,
 )
-import py  # type: ignore
+import py
+
+from skibidi_orm.migration_engine.db_config.postgres_config import PostgresConfig
+from skibidi_orm.migration_engine.db_inspectors.postgres_inspector import PostgresInspector  # type: ignore
 
 
 @pytest.fixture(autouse=True)
 def reset_config_singleton(monkeypatch: pytest.MonkeyPatch):
-    # monkeypatch.setattr(ConfigSingleton, "_instances", {})
-    # monkeypatch.setattr(BaseDbConfig, "_BaseDbConfig__instances_count", 0)
     monkeypatch.setattr(BaseDbConfig, "_BaseDbConfig__instance", None)
 
 
 @pytest.hookimpl(hookwrapper=True)
 def pytest_runtest_makereport(item: Any) -> Any:
     """Print tests' docstring when running the test."""
     outcome: Any = yield
@@ -105,19 +106,27 @@
     db_name: str,
     db_user: str,
     db_password: str,
     db_host: str,
     db_port: int,
     queries: list[str],
 ):
-    def decorator(func: Callable[..., Any]):
+    def decorator(func: Callable[[PostgresConfig, PostgresInspector], Any]):
         @wraps(func)
         def wrapper():
+            config = PostgresConfig(
+                db_name=db_name,
+                db_user=db_user,
+                db_password=db_password,
+                db_host=db_host,
+                db_port=db_port,
+            )
+            inspector = PostgresInspector()
             clear_postgres_database(db_name, db_user, db_password, db_host, db_port)
             create_postgres_database(
                 db_name, db_user, db_password, db_host, db_port, queries
             )
-            func()
+            func(config, inspector)
 
         return wrapper
 
     return decorator
```

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/constraints/test_constraints.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/constraints/test_constraints.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/converters/sqlite3/test_column_operations_conversion.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/converters/sqlite3/test_constraint_conversion.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/converters/sqlite3/test_table_operations_conversion.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from skibidi_orm.migration_engine.operations.table_operations import (
     CreateTableOperation,
     DeleteTableOperation,
     RenameTableOperation,
 )
 from itertools import chain
 
+from skibidi_orm.migration_engine.revisions.constants import get_revision_table_name
+
 
 simple_table_no_constraints = SQLite3Typing.Table(
     "users", columns=[SQLite3Typing.Column("name", "TEXT")]
 )
 
 
 complex_table_no_constraints = SQLite3Typing.Table(
@@ -147,7 +149,14 @@
 def test_rename_table_conversion_simple():
     """Rename a table"""
     operation = RenameTableOperation(simple_table_no_constraints, "users2")
     assert (
         SQLite3TableOperationConverter.convert_table_operation_to_SQL(operation)
         == "DROP TABLE users; CREATE TABLE users2 (name TEXT);"
     )
+
+
+def test_correct_revision_table_SQL_conversion():
+    """Tests whether the query used to create the internal revision table is correct"""
+    assert SQLite3TableOperationConverter.get_revision_table_creation_query() == (
+        f"CREATE TABLE {get_revision_table_name()} (rev REVISION NOT NULL);"
+    )
```

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_config/test_config.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/db_config/test_config.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_config/test_postgres_config.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/db_config/test_postgres_config.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_inspector/test_postgres_inspector.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/db_inspector/test_postgres_inspector.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,23 +52,15 @@
         db_name="postgres",
         db_user="admin",
         db_password="admin",
         db_host="0.0.0.0",
         db_port=5432,
         queries=query,  # type: ignore
     )
-    def test_fn():
-        PostgresConfig(
-            db_name="postgres",
-            db_user="admin",
-            db_password="admin",
-            db_host="0.0.0.0",
-            db_port=5432,
-        )
-        inspector = PostgresInspector()
+    def test_fn(config: PostgresConfig, inspector: PostgresInspector):
         tables = inspector.get_tables_names()
         assert len(tables) == expected_tables_len
         assert sorted(expected_tables_list) == sorted(tables)  # type: ignore
 
     test_fn()
 
 
@@ -77,23 +69,15 @@
         db_name="postgres",
         db_user="admin",
         db_password="admin",
         db_host="0.0.0.0",
         db_port=5432,
         queries=[PostgresTablesData.SQL_TABLE_MANY_COLUMNS1],
     )
-    def test_fn():
-        PostgresConfig(
-            db_name="postgres",
-            db_user="admin",
-            db_password="admin",
-            db_host="0.0.0.0",
-            db_port=5432,
-        )
-        inspector = PostgresInspector()
+    def test_fn(config: PostgresConfig, inspector: PostgresInspector):
         columns_names = inspector._get_table_columns_names("table_many_columns1")  # type: ignore
         assert len(columns_names) == 7
         assert sorted(columns_names) == sorted(
             [
                 "primary_key",
                 "text_not_null",
                 "text_nullabe",
@@ -243,23 +227,15 @@
         db_name="postgres",
         db_user="admin",
         db_password="admin",
         db_host="0.0.0.0",
         db_port=5432,
         queries=query,  # type: ignore
     )
-    def test_fn():
-        PostgresConfig(
-            db_name="postgres",
-            db_user="admin",
-            db_password="admin",
-            db_host="0.0.0.0",
-            db_port=5432,
-        )
-        inspector = PostgresInspector()
+    def test_fn(config: PostgresConfig, inspector: PostgresInspector):
         data_type = inspector._get_column_data_type(table_name, column_name)  # type: ignore
         assert data_type == expected_data_type
 
     test_fn()
 
 
 @pytest.mark.parametrize(
@@ -314,23 +290,15 @@
         db_name="postgres",
         db_user="admin",
         db_password="admin",
         db_host="0.0.0.0",
         db_port=5432,
         queries=query,  # type: ignore
     )
-    def test_fn():
-        PostgresConfig(
-            db_name="postgres",
-            db_user="admin",
-            db_password="admin",
-            db_host="0.0.0.0",
-            db_port=5432,
-        )
-        inspector = PostgresInspector()
+    def test_fn(config: PostgresConfig, inspector: PostgresInspector):
         assert inspector._is_column_nullable(table_name, column_name) is expected_nullable  # type: ignore
 
     test_fn()
 
 
 @pytest.mark.parametrize(
     "query, table_name, column_name, expected_constraints",
@@ -567,23 +535,15 @@
         db_name="postgres",
         db_user="admin",
         db_password="admin",
         db_host="0.0.0.0",
         db_port=5432,
         queries=query,  # type: ignore
     )
-    def test_fn():
-        PostgresConfig(
-            db_name="postgres",
-            db_user="admin",
-            db_password="admin",
-            db_host="0.0.0.0",
-            db_port=5432,
-        )
-        inspector = PostgresInspector()
+    def test_fn(config: PostgresConfig, inspector: PostgresInspector):
         constraints = inspector._get_column_constraints(table_name, column_name)  # type: ignore
         assert sorted(constraints) == sorted(expected_constraints)  # type: ignore
 
     test_fn()
 
 
 @pytest.mark.parametrize(
@@ -874,23 +834,15 @@
         db_name="postgres",
         db_user="admin",
         db_password="admin",
         db_host="0.0.0.0",
         db_port=5432,
         queries=query,  # type: ignore
     )
-    def test_fn():
-        PostgresConfig(
-            db_name="postgres",
-            db_user="admin",
-            db_password="admin",
-            db_host="0.0.0.0",
-            db_port=5432,
-        )
-        inspector = PostgresInspector()
+    def test_fn(config: PostgresConfig, inspector: PostgresInspector):
         columns = inspector.get_table_columns(table_name)  # type: ignore
         for column in columns:
             column.column_constraints = sorted(column.column_constraints)
         for column in expected_columns:  # type: ignore
             column.column_constraints = sorted(column.column_constraints)  # type: ignore
         assert sorted(columns) == sorted(expected_columns)  # type: ignore
 
@@ -949,20 +901,12 @@
         db_name="postgres",
         db_user="admin",
         db_password="admin",
         db_host="0.0.0.0",
         db_port=5432,
         queries=query,  # type: ignore
     )
-    def test_fn():
-        PostgresConfig(
-            db_name="postgres",
-            db_user="admin",
-            db_password="admin",
-            db_host="0.0.0.0",
-            db_port=5432,
-        )
-        inspector = PostgresInspector()
+    def test_fn(config: PostgresConfig, inspector: PostgresInspector):
         foreign_keys = inspector._get_foreign_keys(table_name)  # type: ignore
         assert foreign_keys == expected_foreign_keys
 
     test_fn()
```

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/db_mutators/test_sqlite3_mutator.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/operations/test_operations.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/operations/test_operations.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/sql_data.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/sql_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,46 @@
 
     sql_table_primary_key_not_null = """
         CREATE TABLE table_primary_key_not_null (
             id INTEGER PRIMARY KEY NOT NULL
         );
     """
 
+    sql_simple_schema_with_fks = [
+        """
+        CREATE TABLE users (
+            user_id INTEGER PRIMARY KEY,
+            username TEXT NOT NULL,
+            email TEXT NOT NULL,
+            password_hash TEXT NOT NULL,
+            registration_date TIMESTAMP NOT NULL
+            );
+        """,
+        """
+        CREATE TABLE posts (
+            post_id INTEGER PRIMARY KEY,
+            user_id INTEGER NOT NULL,
+            title TEXT NOT NULL,
+            content TEXT NOT NULL,
+            post_date TIMESTAMP NOT NULL,
+            FOREIGN KEY (user_id) REFERENCES users(user_id)
+        );
+        """,
+        """CREATE TABLE comments (
+            comment_id INTEGER PRIMARY KEY,
+            username TEXT NOT NULL,
+            user_idd INTEGER NOT NULL,
+            post_id INTEGER NOT NULL,
+            comment_text TEXT NOT NULL,
+            comment_date TIMESTAMP NOT NULL,
+            FOREIGN KEY (user_idd, username) REFERENCES users(user_id, username),
+            FOREIGN KEY (post_id) REFERENCES posts(post_id)
+        );
+        """,
+    ]
     sql_schema_with_fks = [
         """
         CREATE TABLE users (
             user_id INTEGER PRIMARY KEY,
             username TEXT NOT NULL UNIQUE,
             email TEXT NOT NULL UNIQUE,
             password_hash TEXT NOT NULL,
```

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/state_manager/test_state_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     RenameTableOperation,
 )
 
 from skibidi_orm.migration_engine.adapters.database_objects.migration_element import (
     MigrationElement,
 )
 
-# from tmp.mock_schema import Table
 
 from pathlib import Path
 import pytest
 import sqlite3
 from ..sql_data import SQLite3TablesData
```

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/studio/test_db_config_dynamic_import.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/studio/test_get_db_inspector.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+import pathlib
+from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
     SQLite3Inspector,
 )
 from skibidi_orm.migration_engine.studio.utils.get_db_inspector import get_db_inspector
 import py  # type: ignore
 
 
 def write_temp_schema_file(file_path: str, file_content: str):
     with open(file_path, "w") as f:
         f.write(file_content)
 
 
-def test_get_db_inspector_sqlite3(tmpdir: py.path.local):
-    p = tmpdir.join("schema_test_get_db_inspector_sqlite3.py")  # type: ignore
-    p.write(  # type: ignore
+def test_get_db_inspector_sqlite3(tmp_path: pathlib.Path):
+    p = tmp_path.joinpath("schema_test_get_db_inspector_sqlite3.py")
+    p.write_text(
         """from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
 SQLite3Config(db_path="some/path/to/db.db")"""
     )
-    db_inspector = get_db_inspector(schema_file=p.strpath)  # type: ignore
+    db_inspector = get_db_inspector(
+        db_config=SQLite3Config(db_path="some/path/to/db.db")
+    )
     assert isinstance(db_inspector, SQLite3Inspector)
-    tmpdir.remove()
```

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/studio/test_get_db_mutator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import pytest
 from skibidi_orm.migration_engine.data_mutator.sqlite3_data_mutatorr import (
     SQLite3DataMutator,
 )
+from skibidi_orm.migration_engine.db_config.base_config import BaseDbConfig
 from skibidi_orm.migration_engine.db_config.sqlite3_config import SQLite3Config
-from skibidi_orm.migration_engine.db_inspectors.sqlite3_inspector import (
-    SQLite3Inspector,
-)
 from skibidi_orm.migration_engine.studio.utils.get_db_seeder import get_db_mutator
 
 
 def test_get_db_seeder_sqlite3_error_when_config_not_exists():
     with pytest.raises(ReferenceError):
-        get_db_mutator(db_inspector=SQLite3Inspector())
+        get_db_mutator(db_config=BaseDbConfig.get_instance())
 
 
 def test_get_db_seeder_sqlite3():
-    SQLite3Config(db_path="some/path/to/db.db")
-    seeder = get_db_mutator(db_inspector=SQLite3Inspector())
+    seeder = get_db_mutator(db_config=SQLite3Config(db_path="some/path/to/db.db"))
     assert isinstance(seeder, SQLite3DataMutator)
```

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/studio/test_routes.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/studio/test_routes.py`

 * *Files identical despite different names*

### Comparing `skibidi_orm-0.1.22/tests/skibidi-orm/migration_engine/test_module_cooperation.py` & `skibidi_orm-0.1.26/tests/skibidi-orm/migration_engine/test_module_cooperation.py`

 * *Files identical despite different names*

