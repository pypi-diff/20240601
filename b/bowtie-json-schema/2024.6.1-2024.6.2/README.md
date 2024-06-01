# Comparing `tmp/bowtie_json_schema-2024.6.1.tar.gz` & `tmp/bowtie_json_schema-2024.6.2.tar.gz`

## Comparing `bowtie_json_schema-2024.6.1.tar` & `bowtie_json_schema-2024.6.2.tar`

### file list

```diff
@@ -1,296 +1,296 @@
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.gitpod.Dockerfile
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.gitpod.yml
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.prettierrc.json
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.readthedocs.yaml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/action.yml
--rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/noxfile.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/requirements.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/test-requirements.in
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/test-requirements.txt
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.devcontainer/devcontainer.json
--rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.pre-commit-hooks/check-dependabot
--rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.pre-commit-hooks/check-lintsonschema-schema
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/__main__.py
--rw-r--r--   0        0        0    53438 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_cli.py
--rw-r--r--   0        0        0    12045 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_commands.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_connectables.py
--rw-r--r--   0        0        0    11585 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_containers.py
--rw-r--r--   0        0        0    21846 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_core.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_direct_connectable.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_registry.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_report.py
--rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_suite.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/exceptions.py
--rw-r--r--   0        0        0     9633 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/hypothesis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/py.typed
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/connectables.json
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/report.json
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/cli/filter-implementations.json
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/cli/info.json
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/cli/smoke.json
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/cli/statistics.json
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/cli/summary.json
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/models/dialect.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/models/group.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/models/implementation-id.json
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/models/implementation.json
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/models/registry.json
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/models/test.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/data/dialects.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/Makefile
--rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/cli.rst
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/conf.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/contributing.rst
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/github-actions.rst
--rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/implementers.rst
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/index.rst
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/motd.txt
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/requirements.in
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/requirements.txt
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/_static/bowtie_diagram_dark.svg
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/_static/bowtie_diagram_light.svg
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/_static/logo.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/index.html
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/package.json
--rw-r--r--   0        0        0   163693 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/tsconfig.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/vite.config.ts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/public/favicon.svg
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/DialectReportView.tsx
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/MainContainer.tsx
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/ReportDataHandler.tsx
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/global.css
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/index.tsx
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/assets/landscape-logo.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/CopyToClipboard.tsx
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/FilterSection.module.css
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/FilterSection.tsx
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/LoadingAnimation.tsx
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/NavBar.tsx
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/OtherImplementations.tsx
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CaseItem.tsx
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CaseResultSvg.test.tsx
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CaseResultSvg.tsx
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CasesSection.tsx
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Cases/SchemaDisplay.tsx
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/DragAndDrop/DragAndDrop.module.css
--rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/DragAndDrop/DragAndDrop.tsx
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/ImplementationReportView/EmbedBadges.module.css
--rw-r--r--   0        0        0     5956 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Modals/DetailsButtonModal.tsx
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/RunInfo/RunInfoSection.tsx
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Summary/ImplementationRow.tsx
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Summary/SummarySection.tsx
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Summary/SummaryTable.tsx
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/context/BowtieVersionContext.tsx
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/context/ThemeContext.tsx
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/Badge.test.ts
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/Badge.ts
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/Dialect.test.ts
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/Dialect.ts
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/Site.test.ts
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/Site.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/mapLanguage.ts
--rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/parseReportData.test.ts
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/hooks/useSearchParams.ts
--rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/.java-implementations-pmd-ruleset.xml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/clojure-json-schema/Dockerfile
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/clojure-json-schema/project.clj
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/cpp-valijson/.dockerignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/cpp-valijson/.gitignore
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/cpp-valijson/Dockerfile
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/cpp-valijson/bowtie_valijson.cpp
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/cpp-valijson/compile_flags.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/.clang-format
--rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/.editorconfig
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/.gitignore
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/Dockerfile
--rw-r--r--   0        0        0    22323 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/Program.cs
--rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/bowtie_corvus_jsonschema.csproj
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/schema.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/applicator.json
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/content.json
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/core.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/format.json
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/hyper-schema.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/meta-data.json
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/validation.json
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/schema.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/applicator.json
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/content.json
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/core.json
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/format-annotation.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/format-assertion.json
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/hyper-schema.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/meta-data.json
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/unevaluated.json
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/validation.json
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft4/schema.json
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft6/schema.json
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft7/schema.json
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-jsonschema-net/.clang-format
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-jsonschema-net/.gitignore
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-jsonschema-net/Dockerfile
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-jsonschema-net/Program.cs
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-gojsonschema/Dockerfile
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-gojsonschema/bowtie_gojsonschema.go
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-gojsonschema/go.mod
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-gojsonschema/go.sum
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-jsonschema/Dockerfile
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-jsonschema/bowtie_jsonschema.go
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-jsonschema/go.mod
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-jsonschema/go.sum
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-json-schema/BowtieJsonSchema.java
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-json-schema/Dockerfile
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-json-schema/build.gradle
--rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-json-tools-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-json-tools-json-schema-validator/build.gradle
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-jsonschemafriend/Dockerfile
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-jsonschemafriend/build.gradle
--rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-networknt-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-networknt-json-schema-validator/build.gradle
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/.dockerignore
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/.editorconfig
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/Dockerfile
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/build.gradle.kts
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/gradle.properties
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/justfile
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/settings.gradle.kts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/gradle/libs.versions.toml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-ajv/Dockerfile
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-ajv/bowtie_ajv.js
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-ajv/package-lock.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-ajv/package.json
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-hyperjump/Dockerfile
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-hyperjump/bowtie_hyperjump.js
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-hyperjump/package.json
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-json-schema/Dockerfile
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-json-schema/bowtie_json_schema.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-json-schema/package.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-jsonschema/bowtie_jsonschema.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-jsonschema/package.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-schemasafe/Dockerfile
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-schemasafe/bowtie_schemasafe.js
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-schemasafe/package.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/.gitignore
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/lua-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/lua-jsonschema/bowtie_jsonschema.lua
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/lua-jsonschema/json.lua
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/lua-jsonschema/stylua.toml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/php-opis-json-schema/Dockerfile
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/php-opis-json-schema/bowtieJsonSchema.php
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/php-opis-json-schema/composer.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/python-fastjsonschema/Dockerfile
--rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/python-jschon/Dockerfile
--rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/python-jschon/bowtie_jschon.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/python-jsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/python-jsonschema/bowtie_jsonschema.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ruby-json_schemer/.rubocop.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ruby-json_schemer/Dockerfile
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ruby-json_schemer/Gemfile
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ruby-json_schemer/Gemfile.lock
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ruby-json_schemer/bowtie_json_schemer.rb
--rw-r--r--   0        0        0    13409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-boon/Cargo.lock
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-boon/Cargo.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-boon/Dockerfile
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-boon/build.rs
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-boon/src/main.rs
--rw-r--r--   0        0        0    39299 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/Cargo.lock
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/Cargo.toml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/Dockerfile
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/build.rs
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/src/main.rs
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-mjs-validator/Dockerfile
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-mjs-validator/Harness.scala
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-mjs-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-mjs-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-mjs-validator/project/plugins.sbt
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-rc-circe-json-validator/Dockerfile
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-rc-circe-json-validator/Harness.scala
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-rc-circe-json-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-rc-circe-json-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-rc-circe-json-validator/project/plugins.sbt
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ts-vscode-json-languageservice/Dockerfile
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ts-vscode-json-languageservice/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ts-vscode-json-languageservice/tsconfig.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/conftest.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_cli.py
--rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_connectables.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_dialect.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_github.py
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_hypothesis.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_implementation.py
--rw-r--r--   0        0        0    74314 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_integration.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_registry.py
--rw-r--r--   0        0        0    10199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_report.py
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_schemas.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3069 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/.gitattributes
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/connectables.json
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/report.json
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/filter-implementations.json
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/info.json
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/statistics.json
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/group.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/implementation-id.json
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/test.json
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/LICENSE
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/README.rst
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/hatch_build.py
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/pyproject.toml
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/PKG-INFO
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/.gitpod.Dockerfile
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/.gitpod.yml
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/.prettierrc.json
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/action.yml
+-rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/noxfile.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/requirements.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/test-requirements.in
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/test-requirements.txt
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/.devcontainer/devcontainer.json
+-rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/.pre-commit-hooks/check-dependabot
+-rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/.pre-commit-hooks/check-lintsonschema-schema
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/__main__.py
+-rw-r--r--   0        0        0    53438 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/_cli.py
+-rw-r--r--   0        0        0    12045 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/_commands.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/_connectables.py
+-rw-r--r--   0        0        0    11585 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/_containers.py
+-rw-r--r--   0        0        0    21846 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/_core.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/_direct_connectable.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/_registry.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/_report.py
+-rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/_suite.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/exceptions.py
+-rw-r--r--   0        0        0     9633 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/hypothesis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/py.typed
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/connectables.json
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/report.json
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/cli/filter-implementations.json
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/cli/info.json
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/cli/statistics.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/cli/summary.json
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/models/dialect.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/bowtie/schemas/models/test.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/data/dialects.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/docs/Makefile
+-rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/docs/cli.rst
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/docs/conf.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/docs/contributing.rst
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/docs/github-actions.rst
+-rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/docs/implementers.rst
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/docs/index.rst
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/docs/motd.txt
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/docs/requirements.in
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/docs/requirements.txt
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/docs/_static/bowtie_diagram_dark.svg
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/docs/_static/bowtie_diagram_light.svg
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/docs/_static/logo.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/index.html
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/package.json
+-rw-r--r--   0        0        0   163693 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/tsconfig.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/vite.config.ts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/public/favicon.svg
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/DialectReportView.tsx
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/MainContainer.tsx
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/ReportDataHandler.tsx
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/global.css
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/index.tsx
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/assets/landscape-logo.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/CopyToClipboard.tsx
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/FilterSection.module.css
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/FilterSection.tsx
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/LoadingAnimation.tsx
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/NavBar.tsx
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/OtherImplementations.tsx
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/Cases/CaseItem.tsx
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/Cases/CaseResultSvg.test.tsx
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/Cases/CaseResultSvg.tsx
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/Cases/CasesSection.tsx
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/Cases/SchemaDisplay.tsx
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/DragAndDrop/DragAndDrop.module.css
+-rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/DragAndDrop/DragAndDrop.tsx
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/ImplementationReportView/EmbedBadges.module.css
+-rw-r--r--   0        0        0     5956 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/Modals/DetailsButtonModal.tsx
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/RunInfo/RunInfoSection.tsx
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/Summary/ImplementationRow.tsx
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/Summary/SummarySection.tsx
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/components/Summary/SummaryTable.tsx
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/context/BowtieVersionContext.tsx
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/context/ThemeContext.tsx
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/data/Badge.test.ts
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/data/Badge.ts
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/data/Dialect.test.ts
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/data/Dialect.ts
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/data/Site.test.ts
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/data/Site.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/data/mapLanguage.ts
+-rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/data/parseReportData.test.ts
+-rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/frontend/src/hooks/useSearchParams.ts
+-rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/.java-implementations-pmd-ruleset.xml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/clojure-json-schema/Dockerfile
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/clojure-json-schema/project.clj
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/cpp-valijson/.dockerignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/cpp-valijson/.gitignore
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/cpp-valijson/Dockerfile
+-rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/cpp-valijson/bowtie_valijson.cpp
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/cpp-valijson/compile_flags.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/.clang-format
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/.editorconfig
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/.gitignore
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/Dockerfile
+-rw-r--r--   0        0        0    22323 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/Program.cs
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/bowtie_corvus_jsonschema.csproj
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/schema.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/applicator.json
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/content.json
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/core.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/format.json
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/hyper-schema.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/meta-data.json
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/validation.json
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/schema.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/applicator.json
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/content.json
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/core.json
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/format-annotation.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/format-assertion.json
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/hyper-schema.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/meta-data.json
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/unevaluated.json
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/validation.json
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft4/schema.json
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft6/schema.json
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft7/schema.json
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-jsonschema-net/.clang-format
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-jsonschema-net/.gitignore
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-jsonschema-net/Dockerfile
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-jsonschema-net/Program.cs
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/go-gojsonschema/Dockerfile
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/go-gojsonschema/bowtie_gojsonschema.go
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/go-gojsonschema/go.mod
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/go-gojsonschema/go.sum
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/go-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/go-jsonschema/bowtie_jsonschema.go
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/go-jsonschema/go.mod
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/go-jsonschema/go.sum
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-json-schema/BowtieJsonSchema.java
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-json-schema/Dockerfile
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-json-schema/build.gradle
+-rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-json-tools-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-json-tools-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-jsonschemafriend/Dockerfile
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-jsonschemafriend/build.gradle
+-rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-networknt-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-networknt-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/.dockerignore
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/.editorconfig
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/Dockerfile
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/build.gradle.kts
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/gradle.properties
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/justfile
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/settings.gradle.kts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/gradle/libs.versions.toml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-ajv/Dockerfile
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-ajv/bowtie_ajv.js
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-ajv/package-lock.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-ajv/package.json
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-hyperjump/Dockerfile
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-hyperjump/bowtie_hyperjump.js
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-hyperjump/package.json
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-json-schema/Dockerfile
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-json-schema/bowtie_json_schema.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-json-schema/package.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-jsonschema/bowtie_jsonschema.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-jsonschema/package.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-schemasafe/Dockerfile
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-schemasafe/bowtie_schemasafe.js
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/js-schemasafe/package.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/kotlin-kmp-json-schema-validator/.gitignore
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/kotlin-kmp-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/lua-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/lua-jsonschema/bowtie_jsonschema.lua
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/lua-jsonschema/json.lua
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/lua-jsonschema/stylua.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/php-opis-json-schema/Dockerfile
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/php-opis-json-schema/bowtieJsonSchema.php
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/php-opis-json-schema/composer.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/python-fastjsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/python-jschon/Dockerfile
+-rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/python-jschon/bowtie_jschon.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/python-jsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/python-jsonschema/bowtie_jsonschema.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/ruby-json_schemer/.rubocop.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/ruby-json_schemer/Dockerfile
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/ruby-json_schemer/Gemfile
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/ruby-json_schemer/Gemfile.lock
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/ruby-json_schemer/bowtie_json_schemer.rb
+-rw-r--r--   0        0        0    13409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/rust-boon/Cargo.lock
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/rust-boon/Cargo.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/rust-boon/Dockerfile
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/rust-boon/build.rs
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/rust-boon/src/main.rs
+-rw-r--r--   0        0        0    39299 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/rust-jsonschema/Cargo.lock
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/rust-jsonschema/Cargo.toml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/rust-jsonschema/Dockerfile
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/rust-jsonschema/build.rs
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/rust-jsonschema/src/main.rs
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/scala-mjs-validator/Dockerfile
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/scala-mjs-validator/Harness.scala
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/scala-mjs-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/scala-mjs-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/scala-mjs-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/scala-rc-circe-json-validator/Dockerfile
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/scala-rc-circe-json-validator/Harness.scala
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/scala-rc-circe-json-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/scala-rc-circe-json-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/scala-rc-circe-json-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/ts-vscode-json-languageservice/Dockerfile
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/ts-vscode-json-languageservice/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/implementations/ts-vscode-json-languageservice/tsconfig.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/conftest.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/test_cli.py
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/test_connectables.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/test_dialect.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/test_github.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/test_hypothesis.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/test_implementation.py
+-rw-r--r--   0        0        0    74314 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/test_integration.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/test_registry.py
+-rw-r--r--   0        0        0    10199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/test_report.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/test_schemas.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3069 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/.gitattributes
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/connectables.json
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/report.json
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/cli/filter-implementations.json
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/cli/info.json
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/cli/statistics.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/models/test.json
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/LICENSE
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/README.rst
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/hatch_build.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.2/PKG-INFO
```

### Comparing `bowtie_json_schema-2024.6.1/.gitpod.yml` & `bowtie_json_schema-2024.6.2/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/.pre-commit-config.yaml` & `bowtie_json_schema-2024.6.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -68,27 +68,29 @@
       - name: cargo clippy rust-jsonschema
         id: clippy
         args:
           [
             "--manifest-path",
             "implementations/rust-jsonschema/Cargo.toml",
             "--allow-dirty",
+            "--allow-staged",
             "--fix",
             "--",
           ]
       - name: cargo fmt rust-boon
         id: fmt
         args: ["--manifest-path", "implementations/rust-boon/Cargo.toml", "--"]
       - name: cargo clippy rust-boon
         id: clippy
         args:
           [
             "--manifest-path",
             "implementations/rust-boon/Cargo.toml",
             "--allow-dirty",
+            "--allow-staged",
             "--fix",
             "--",
           ]
   - repo: https://github.com/syntaqx/git-hooks
     rev: v0.0.18
     hooks:
       - name: go fmt (golang implementations)
```

### Comparing `bowtie_json_schema-2024.6.1/CONTRIBUTING.rst` & `bowtie_json_schema-2024.6.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/action.yml` & `bowtie_json_schema-2024.6.2/action.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/noxfile.py` & `bowtie_json_schema-2024.6.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/requirements.txt` & `bowtie_json_schema-2024.6.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/test-requirements.txt` & `bowtie_json_schema-2024.6.2/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/.pre-commit-hooks/check-dependabot` & `bowtie_json_schema-2024.6.2/.pre-commit-hooks/check-dependabot`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/.pre-commit-hooks/check-lintsonschema-schema` & `bowtie_json_schema-2024.6.2/.pre-commit-hooks/check-lintsonschema-schema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/_cli.py` & `bowtie_json_schema-2024.6.2/bowtie/_cli.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/_commands.py` & `bowtie_json_schema-2024.6.2/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/_connectables.py` & `bowtie_json_schema-2024.6.2/bowtie/_connectables.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/_containers.py` & `bowtie_json_schema-2024.6.2/bowtie/_containers.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/_core.py` & `bowtie_json_schema-2024.6.2/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/_direct_connectable.py` & `bowtie_json_schema-2024.6.2/bowtie/_direct_connectable.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/_registry.py` & `bowtie_json_schema-2024.6.2/bowtie/_registry.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/_report.py` & `bowtie_json_schema-2024.6.2/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/_suite.py` & `bowtie_json_schema-2024.6.2/bowtie/_suite.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/exceptions.py` & `bowtie_json_schema-2024.6.2/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/hypothesis.py` & `bowtie_json_schema-2024.6.2/bowtie/hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/schemas/connectables.json` & `bowtie_json_schema-2024.6.2/bowtie/schemas/connectables.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/schemas/report.json` & `bowtie_json_schema-2024.6.2/bowtie/schemas/report.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/schemas/cli/info.json` & `bowtie_json_schema-2024.6.2/bowtie/schemas/cli/info.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/schemas/cli/smoke.json` & `bowtie_json_schema-2024.6.2/bowtie/schemas/cli/smoke.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/schemas/cli/statistics.json` & `bowtie_json_schema-2024.6.2/bowtie/schemas/cli/statistics.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/schemas/cli/summary.json` & `bowtie_json_schema-2024.6.2/bowtie/schemas/cli/summary.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/schemas/io/v1.json` & `bowtie_json_schema-2024.6.2/bowtie/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.6.2/bowtie/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/schemas/io/commands/run.json` & `bowtie_json_schema-2024.6.2/bowtie/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/schemas/io/commands/start.json` & `bowtie_json_schema-2024.6.2/bowtie/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/schemas/models/dialect.json` & `bowtie_json_schema-2024.6.2/bowtie/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/schemas/models/group.json` & `bowtie_json_schema-2024.6.2/bowtie/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/schemas/models/implementation.json` & `bowtie_json_schema-2024.6.2/bowtie/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/bowtie/schemas/models/test.json` & `bowtie_json_schema-2024.6.2/bowtie/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/data/dialects.json` & `bowtie_json_schema-2024.6.2/data/dialects.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/docs/Makefile` & `bowtie_json_schema-2024.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/docs/cli.rst` & `bowtie_json_schema-2024.6.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/docs/conf.py` & `bowtie_json_schema-2024.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/docs/contributing.rst` & `bowtie_json_schema-2024.6.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/docs/github-actions.rst` & `bowtie_json_schema-2024.6.2/docs/github-actions.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/docs/implementers.rst` & `bowtie_json_schema-2024.6.2/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/docs/index.rst` & `bowtie_json_schema-2024.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/docs/motd.txt` & `bowtie_json_schema-2024.6.2/docs/motd.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/docs/requirements.txt` & `bowtie_json_schema-2024.6.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/docs/_static/bowtie_diagram_dark.svg` & `bowtie_json_schema-2024.6.2/docs/_static/bowtie_diagram_dark.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/docs/_static/bowtie_diagram_light.svg` & `bowtie_json_schema-2024.6.2/docs/_static/bowtie_diagram_light.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/docs/_static/logo.svg` & `bowtie_json_schema-2024.6.2/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/package.json` & `bowtie_json_schema-2024.6.2/frontend/package.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2024.6.2/frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/tsconfig.json` & `bowtie_json_schema-2024.6.2/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/public/favicon.svg` & `bowtie_json_schema-2024.6.2/frontend/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/DialectReportView.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/DialectReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/ReportDataHandler.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/ReportDataHandler.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/index.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/assets/landscape-logo.svg` & `bowtie_json_schema-2024.6.2/frontend/src/assets/landscape-logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/CopyToClipboard.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/CopyToClipboard.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/FilterSection.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/FilterSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/NavBar.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/NavBar.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/OtherImplementations.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/OtherImplementations.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CaseItem.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/Cases/CaseItem.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CaseResultSvg.test.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/Cases/CaseResultSvg.test.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CaseResultSvg.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/Cases/CaseResultSvg.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CasesSection.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/Cases/CasesSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/Cases/SchemaDisplay.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/Cases/SchemaDisplay.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/DragAndDrop/DragAndDrop.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/DragAndDrop/DragAndDrop.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/ImplementationReportView/DialectCompliance.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/ImplementationReportView/DialectCompliance.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/ImplementationReportView/EmbedBadges.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/ImplementationReportView/EmbedBadges.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/Modals/DetailsButtonModal.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/Modals/DetailsButtonModal.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/RunInfo/RunInfoSection.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/RunInfo/RunInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2024.6.2/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/Summary/ImplementationRow.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/Summary/ImplementationRow.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/Summary/SummarySection.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/Summary/SummarySection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/components/Summary/SummaryTable.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/components/Summary/SummaryTable.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/context/BowtieVersionContext.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/context/BowtieVersionContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/context/ThemeContext.tsx` & `bowtie_json_schema-2024.6.2/frontend/src/context/ThemeContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/data/Badge.test.ts` & `bowtie_json_schema-2024.6.2/frontend/src/data/Badge.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/data/Badge.ts` & `bowtie_json_schema-2024.6.2/frontend/src/data/Badge.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/data/Dialect.ts` & `bowtie_json_schema-2024.6.2/frontend/src/data/Dialect.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/data/Site.test.ts` & `bowtie_json_schema-2024.6.2/frontend/src/data/Site.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/data/parseReportData.test.ts` & `bowtie_json_schema-2024.6.2/frontend/src/data/parseReportData.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2024.6.2/frontend/src/data/parseReportData.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/.java-implementations-pmd-ruleset.xml` & `bowtie_json_schema-2024.6.2/implementations/.java-implementations-pmd-ruleset.xml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/clojure-json-schema/Dockerfile` & `bowtie_json_schema-2024.6.2/implementations/clojure-json-schema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj` & `bowtie_json_schema-2024.6.2/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/cpp-valijson/bowtie_valijson.cpp` & `bowtie_json_schema-2024.6.2/implementations/cpp-valijson/bowtie_valijson.cpp`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/.editorconfig` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/.editorconfig`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/.gitignore` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/Program.cs` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/Program.cs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/bowtie_corvus_jsonschema.csproj` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/bowtie_corvus_jsonschema.csproj`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/schema.json` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/applicator.json` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/applicator.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/core.json` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/core.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/hyper-schema.json` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/hyper-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/meta-data.json` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/meta-data.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/validation.json` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/validation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/schema.json` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/applicator.json` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/applicator.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/core.json` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/core.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/hyper-schema.json` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/hyper-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/meta-data.json` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/meta-data.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/validation.json` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/validation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft4/schema.json` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft4/schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft6/schema.json` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft6/schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft7/schema.json` & `bowtie_json_schema-2024.6.2/implementations/dotnet-corvus-jsonschema/metaschema/draft7/schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-jsonschema-net/.gitignore` & `bowtie_json_schema-2024.6.2/implementations/dotnet-jsonschema-net/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/dotnet-jsonschema-net/Program.cs` & `bowtie_json_schema-2024.6.2/implementations/dotnet-jsonschema-net/Program.cs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/go-gojsonschema/bowtie_gojsonschema.go` & `bowtie_json_schema-2024.6.2/implementations/go-gojsonschema/bowtie_gojsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/go-gojsonschema/go.sum` & `bowtie_json_schema-2024.6.2/implementations/go-gojsonschema/go.sum`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/go-jsonschema/bowtie_jsonschema.go` & `bowtie_json_schema-2024.6.2/implementations/go-jsonschema/bowtie_jsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-json-schema/BowtieJsonSchema.java` & `bowtie_json_schema-2024.6.2/implementations/java-json-schema/BowtieJsonSchema.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-json-schema/build.gradle` & `bowtie_json_schema-2024.6.2/implementations/java-json-schema/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.6.2/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-json-tools-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.6.2/implementations/java-json-tools-json-schema-validator/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java` & `bowtie_json_schema-2024.6.2/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-jsonschemafriend/build.gradle` & `bowtie_json_schema-2024.6.2/implementations/java-jsonschemafriend/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.6.2/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-networknt-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.6.2/implementations/java-networknt-json-schema-validator/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/build.gradle.kts` & `bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/justfile` & `bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/justfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/gradle/libs.versions.toml` & `bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/gradle/libs.versions.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt` & `bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/Support.kt` & `bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/src/main/kotlin/Support.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt` & `bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt` & `bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt` & `bowtie_json_schema-2024.6.2/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/js-ajv/bowtie_ajv.js` & `bowtie_json_schema-2024.6.2/implementations/js-ajv/bowtie_ajv.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/js-ajv/package-lock.json` & `bowtie_json_schema-2024.6.2/implementations/js-ajv/package-lock.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/js-hyperjump/bowtie_hyperjump.js` & `bowtie_json_schema-2024.6.2/implementations/js-hyperjump/bowtie_hyperjump.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/js-json-schema/bowtie_json_schema.js` & `bowtie_json_schema-2024.6.2/implementations/js-json-schema/bowtie_json_schema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/js-jsonschema/bowtie_jsonschema.js` & `bowtie_json_schema-2024.6.2/implementations/js-jsonschema/bowtie_jsonschema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/js-schemasafe/bowtie_schemasafe.js` & `bowtie_json_schema-2024.6.2/implementations/js-schemasafe/bowtie_schemasafe.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts` & `bowtie_json_schema-2024.6.2/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt` & `bowtie_json_schema-2024.6.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt` & `bowtie_json_schema-2024.6.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt` & `bowtie_json_schema-2024.6.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt` & `bowtie_json_schema-2024.6.2/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/lua-jsonschema/Dockerfile` & `bowtie_json_schema-2024.6.2/implementations/lua-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/lua-jsonschema/bowtie_jsonschema.lua` & `bowtie_json_schema-2024.6.2/implementations/lua-jsonschema/bowtie_jsonschema.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/lua-jsonschema/json.lua` & `bowtie_json_schema-2024.6.2/implementations/lua-jsonschema/json.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/php-opis-json-schema/bowtieJsonSchema.php` & `bowtie_json_schema-2024.6.2/implementations/php-opis-json-schema/bowtieJsonSchema.php`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/python-fastjsonschema/bowtie_fastjsonschema.py` & `bowtie_json_schema-2024.6.2/implementations/python-fastjsonschema/bowtie_fastjsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/python-jschon/bowtie_jschon.py` & `bowtie_json_schema-2024.6.2/implementations/python-jschon/bowtie_jschon.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/python-jsonschema/bowtie_jsonschema.py` & `bowtie_json_schema-2024.6.2/implementations/python-jsonschema/bowtie_jsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/ruby-json_schemer/bowtie_json_schemer.rb` & `bowtie_json_schema-2024.6.2/implementations/ruby-json_schemer/bowtie_json_schemer.rb`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/rust-boon/Cargo.lock` & `bowtie_json_schema-2024.6.2/implementations/rust-boon/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/rust-boon/Dockerfile` & `bowtie_json_schema-2024.6.2/implementations/rust-boon/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/rust-boon/src/main.rs` & `bowtie_json_schema-2024.6.2/implementations/rust-boon/src/main.rs`

 * *Files 9% similar despite different names*

```diff
@@ -54,16 +54,15 @@
                 let case = &request["case"];
                 let mut schemas = Schemas::default();
                 let mut compiler = Compiler::default();
                 if let Some(draft) = draft {
                     compiler.set_default_draft(draft);
                 }
                 if let Value::Object(obj) = &case["registry"] {
-                    compiler.register_url_loader("http", Box::new(MapUrlLoader(obj.clone())));
-                    compiler.register_url_loader("https", Box::new(MapUrlLoader(obj.clone())));
+                    compiler.use_loader(Box::new(MapUrlLoader(obj.clone())));
                 }
                 let fake_url = "http://fake.com/schema.json";
                 if let Err(e) = compiler.add_resource(fake_url, case["schema"].clone()) {
                     print_error(seq, e);
                     continue;
                 }
                 let schema = match compiler.compile(fake_url, &mut schemas) {
```

### Comparing `bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/Cargo.lock` & `bowtie_json_schema-2024.6.2/implementations/rust-jsonschema/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/Dockerfile` & `bowtie_json_schema-2024.6.2/implementations/rust-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/src/main.rs` & `bowtie_json_schema-2024.6.2/implementations/rust-jsonschema/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/scala-mjs-validator/Harness.scala` & `bowtie_json_schema-2024.6.2/implementations/scala-mjs-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/scala-mjs-validator/build.sbt` & `bowtie_json_schema-2024.6.2/implementations/scala-mjs-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/scala-rc-circe-json-validator/Harness.scala` & `bowtie_json_schema-2024.6.2/implementations/scala-rc-circe-json-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/scala-rc-circe-json-validator/build.sbt` & `bowtie_json_schema-2024.6.2/implementations/scala-rc-circe-json-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts` & `bowtie_json_schema-2024.6.2/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/test_cli.py` & `bowtie_json_schema-2024.6.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/test_connectables.py` & `bowtie_json_schema-2024.6.2/tests/test_connectables.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/test_github.py` & `bowtie_json_schema-2024.6.2/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/test_hypothesis.py` & `bowtie_json_schema-2024.6.2/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/test_integration.py` & `bowtie_json_schema-2024.6.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/test_registry.py` & `bowtie_json_schema-2024.6.2/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/test_report.py` & `bowtie_json_schema-2024.6.2/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/test_schemas.py` & `bowtie_json_schema-2024.6.2/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/connectables.json` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/connectables.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/report.json` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/report.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/info.json` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/cli/info.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/statistics.json` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/cli/statistics.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/v1.json` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/group.json` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/test.json` & `bowtie_json_schema-2024.6.2/tests/fauxmplementations/lintsonschema/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/.gitignore` & `bowtie_json_schema-2024.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/LICENSE` & `bowtie_json_schema-2024.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/README.rst` & `bowtie_json_schema-2024.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/hatch_build.py` & `bowtie_json_schema-2024.6.2/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/pyproject.toml` & `bowtie_json_schema-2024.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.1/PKG-INFO` & `bowtie_json_schema-2024.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bowtie-json-schema
-Version: 2024.6.1
+Version: 2024.6.2
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://docs.bowtie.report/
 Project-URL: Homepage, https://bowtie.report/
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author-email: Julian Berman <Julian+bowtie@GrayVines.com>
```

