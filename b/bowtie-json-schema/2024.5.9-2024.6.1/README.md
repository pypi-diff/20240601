# Comparing `tmp/bowtie_json_schema-2024.5.9.tar.gz` & `tmp/bowtie_json_schema-2024.6.1.tar.gz`

## Comparing `bowtie_json_schema-2024.5.9.tar` & `bowtie_json_schema-2024.6.1.tar`

### file list

```diff
@@ -1,261 +1,296 @@
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/.gitpod.Dockerfile
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/.gitpod.yml
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/.prettierrc.json
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/.readthedocs.yaml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/action.yml
--rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/noxfile.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/requirements.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/test-requirements.in
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/test-requirements.txt
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/.devcontainer/devcontainer.json
--rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/.pre-commit-hooks/check-dependabot
--rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/.pre-commit-hooks/check-lintsonschema-schema
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/__main__.py
--rw-r--r--   0        0        0    48261 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/_cli.py
--rw-r--r--   0        0        0    12066 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/_commands.py
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/_connectables.py
--rw-r--r--   0        0        0    11145 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/_containers.py
--rw-r--r--   0        0        0    22876 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/_core.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/_registry.py
--rw-r--r--   0        0        0    11625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/_report.py
--rw-r--r--   0        0        0     7817 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/_suite.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/exceptions.py
--rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/hypothesis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/py.typed
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/connectables.json
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/report.json
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/cli/info.json
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/cli/smoke.json
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/cli/summary.json
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/models/dialect.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/models/group.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/models/implementation-id.json
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/models/implementation.json
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/models/registry.json
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/bowtie/schemas/models/test.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/data/dialects.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/docs/Makefile
--rw-r--r--   0        0        0     8253 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/docs/cli.rst
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/docs/conf.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/docs/contributing.rst
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/docs/github-actions.rst
--rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/docs/implementers.rst
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/docs/index.rst
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/docs/motd.txt
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/docs/requirements.in
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/docs/requirements.txt
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/docs/_static/bowtie_diagram_dark.svg
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/docs/_static/bowtie_diagram_light.svg
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/docs/_static/logo.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/index.html
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/package.json
--rw-r--r--   0        0        0   163423 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/tsconfig.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/vite.config.ts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/public/favicon.svg
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/DialectReportView.tsx
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/MainContainer.tsx
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/ReportDataHandler.tsx
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/global.css
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/index.tsx
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/assets/landscape-logo.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/CopyToClipboard.tsx
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/FilterSection.css
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/FilterSection.tsx
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/LoadingAnimation.tsx
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/NavBar.tsx
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/OtherImplementations.tsx
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/Cases/CaseItem.tsx
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/Cases/CaseResultSvg.test.tsx
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/Cases/CaseResultSvg.tsx
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/Cases/CasesSection.tsx
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/Cases/SchemaDisplay.tsx
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/DragAndDrop/DragAndDrop.css
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/DragAndDrop/DragAndDrop.tsx
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/ImplementationReportView/EmbedBadges.css
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/Modals/DetailsButtonModal.tsx
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/RunInfo/RunInfoSection.tsx
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/Summary/ImplementationRow.tsx
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/Summary/SummarySection.tsx
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/components/Summary/SummaryTable.tsx
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/context/BowtieVersionContext.tsx
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/context/ThemeContext.tsx
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/data/Badge.test.ts
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/data/Badge.ts
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/data/Dialect.test.ts
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/data/Dialect.ts
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/data/Site.test.ts
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/data/Site.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/data/mapLanguage.ts
--rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/data/parseReportData.test.ts
--rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/frontend/src/hooks/useSearchParams.ts
--rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/.java-implementations-pmd-ruleset.xml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/clojure-json-schema/Dockerfile
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/clojure-json-schema/project.clj
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/cpp-valijson/.dockerignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/cpp-valijson/.gitignore
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/cpp-valijson/Dockerfile
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/cpp-valijson/bowtie_valijson.cpp
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/cpp-valijson/compile_flags.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/dotnet-jsonschema-net/.clang-format
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/dotnet-jsonschema-net/.gitignore
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/dotnet-jsonschema-net/Dockerfile
--rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/dotnet-jsonschema-net/Program.cs
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/go-gojsonschema/Dockerfile
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/go-gojsonschema/bowtie_gojsonschema.go
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/go-gojsonschema/go.mod
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/go-gojsonschema/go.sum
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/go-jsonschema/Dockerfile
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/go-jsonschema/bowtie_jsonschema.go
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/go-jsonschema/go.mod
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/go-jsonschema/go.sum
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-json-schema/BowtieJsonSchema.java
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-json-schema/Dockerfile
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-json-schema/build.gradle
--rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-json-tools-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-json-tools-json-schema-validator/build.gradle
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-jsonschemafriend/Dockerfile
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-jsonschemafriend/build.gradle
--rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-networknt-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-networknt-json-schema-validator/build.gradle
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/.dockerignore
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/.editorconfig
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/Dockerfile
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/build.gradle.kts
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/gradle.properties
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/justfile
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/settings.gradle.kts
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/gradle/libs.versions.toml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/js-ajv/Dockerfile
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/js-ajv/bowtie_ajv.js
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/js-ajv/package-lock.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/js-ajv/package.json
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/js-hyperjump/Dockerfile
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/js-hyperjump/bowtie_hyperjump.js
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/js-hyperjump/package.json
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/js-json-schema/Dockerfile
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/js-json-schema/bowtie_json_schema.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/js-json-schema/package.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/js-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/js-jsonschema/bowtie_jsonschema.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/js-jsonschema/package.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/kotlin-kmp-json-schema-validator/.gitignore
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/kotlin-kmp-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/lua-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/lua-jsonschema/bowtie_jsonschema.lua
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/lua-jsonschema/json.lua
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/lua-jsonschema/stylua.toml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/php-opis-json-schema/Dockerfile
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/php-opis-json-schema/bowtieJsonSchema.php
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/php-opis-json-schema/composer.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/python-fastjsonschema/Dockerfile
--rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/python-jschon/Dockerfile
--rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/python-jschon/bowtie_jschon.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/python-jsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/python-jsonschema/bowtie_jsonschema.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/ruby-json_schemer/.rubocop.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/ruby-json_schemer/Dockerfile
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/ruby-json_schemer/Gemfile
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/ruby-json_schemer/Gemfile.lock
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/ruby-json_schemer/bowtie_json_schemer.rb
--rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/rust-boon/Cargo.lock
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/rust-boon/Cargo.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/rust-boon/Dockerfile
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/rust-boon/build.rs
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/rust-boon/src/main.rs
--rw-r--r--   0        0        0    39299 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/rust-jsonschema/Cargo.lock
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/rust-jsonschema/Cargo.toml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/rust-jsonschema/Dockerfile
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/rust-jsonschema/build.rs
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/rust-jsonschema/src/main.rs
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/scala-mjs-validator/Dockerfile
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/scala-mjs-validator/Harness.scala
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/scala-mjs-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/scala-mjs-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/scala-mjs-validator/project/plugins.sbt
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/scala-rc-circe-json-validator/Dockerfile
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/scala-rc-circe-json-validator/Harness.scala
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/scala-rc-circe-json-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/scala-rc-circe-json-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/scala-rc-circe-json-validator/project/plugins.sbt
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/ts-vscode-json-languageservice/Dockerfile
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/ts-vscode-json-languageservice/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/implementations/ts-vscode-json-languageservice/tsconfig.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/conftest.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/test_cli.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/test_connectables.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/test_dialect.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/test_github.py
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/test_hypothesis.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/test_implementation.py
--rw-r--r--   0        0        0    65238 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/test_integration.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/test_registry.py
--rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/test_report.py
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/test_schemas.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/.gitattributes
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/connectables.json
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/report.json
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/cli/info.json
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/models/group.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/models/implementation-id.json
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/models/test.json
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/LICENSE
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/README.rst
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/hatch_build.py
--rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/pyproject.toml
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.5.9/PKG-INFO
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.gitpod.Dockerfile
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.gitpod.yml
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.prettierrc.json
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/action.yml
+-rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/noxfile.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/requirements.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/test-requirements.in
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/test-requirements.txt
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.devcontainer/devcontainer.json
+-rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.pre-commit-hooks/check-dependabot
+-rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.pre-commit-hooks/check-lintsonschema-schema
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/__main__.py
+-rw-r--r--   0        0        0    53438 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_cli.py
+-rw-r--r--   0        0        0    12045 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_commands.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_connectables.py
+-rw-r--r--   0        0        0    11585 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_containers.py
+-rw-r--r--   0        0        0    21846 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_core.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_direct_connectable.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_registry.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_report.py
+-rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/_suite.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/exceptions.py
+-rw-r--r--   0        0        0     9633 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/hypothesis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/py.typed
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/connectables.json
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/report.json
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/cli/filter-implementations.json
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/cli/info.json
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/cli/statistics.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/cli/summary.json
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/models/dialect.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/bowtie/schemas/models/test.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/data/dialects.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/Makefile
+-rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/cli.rst
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/conf.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/contributing.rst
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/github-actions.rst
+-rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/implementers.rst
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/index.rst
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/motd.txt
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/requirements.in
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/requirements.txt
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/_static/bowtie_diagram_dark.svg
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/_static/bowtie_diagram_light.svg
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/docs/_static/logo.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/index.html
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/package.json
+-rw-r--r--   0        0        0   163693 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/tsconfig.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/vite.config.ts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/public/favicon.svg
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/DialectReportView.tsx
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/MainContainer.tsx
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/ReportDataHandler.tsx
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/global.css
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/index.tsx
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/assets/landscape-logo.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/CopyToClipboard.tsx
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/FilterSection.module.css
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/FilterSection.tsx
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/LoadingAnimation.tsx
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/NavBar.tsx
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/OtherImplementations.tsx
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CaseItem.tsx
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CaseResultSvg.test.tsx
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CaseResultSvg.tsx
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CasesSection.tsx
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Cases/SchemaDisplay.tsx
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/DragAndDrop/DragAndDrop.module.css
+-rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/DragAndDrop/DragAndDrop.tsx
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/ImplementationReportView/EmbedBadges.module.css
+-rw-r--r--   0        0        0     5956 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Modals/DetailsButtonModal.tsx
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/RunInfo/RunInfoSection.tsx
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Summary/ImplementationRow.tsx
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Summary/SummarySection.tsx
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/components/Summary/SummaryTable.tsx
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/context/BowtieVersionContext.tsx
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/context/ThemeContext.tsx
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/Badge.test.ts
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/Badge.ts
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/Dialect.test.ts
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/Dialect.ts
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/Site.test.ts
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/Site.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/mapLanguage.ts
+-rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/parseReportData.test.ts
+-rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/frontend/src/hooks/useSearchParams.ts
+-rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/.java-implementations-pmd-ruleset.xml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/clojure-json-schema/Dockerfile
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/clojure-json-schema/project.clj
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/cpp-valijson/.dockerignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/cpp-valijson/.gitignore
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/cpp-valijson/Dockerfile
+-rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/cpp-valijson/bowtie_valijson.cpp
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/cpp-valijson/compile_flags.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/.clang-format
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/.editorconfig
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/.gitignore
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/Dockerfile
+-rw-r--r--   0        0        0    22323 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/Program.cs
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/bowtie_corvus_jsonschema.csproj
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/schema.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/applicator.json
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/content.json
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/core.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/format.json
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/hyper-schema.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/meta-data.json
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/validation.json
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/schema.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/applicator.json
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/content.json
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/core.json
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/format-annotation.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/format-assertion.json
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/hyper-schema.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/meta-data.json
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/unevaluated.json
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/validation.json
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft4/schema.json
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft6/schema.json
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/metaschema/draft7/schema.json
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-jsonschema-net/.clang-format
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-jsonschema-net/.gitignore
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-jsonschema-net/Dockerfile
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-jsonschema-net/Program.cs
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-gojsonschema/Dockerfile
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-gojsonschema/bowtie_gojsonschema.go
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-gojsonschema/go.mod
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-gojsonschema/go.sum
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-jsonschema/bowtie_jsonschema.go
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-jsonschema/go.mod
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/go-jsonschema/go.sum
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-json-schema/BowtieJsonSchema.java
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-json-schema/Dockerfile
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-json-schema/build.gradle
+-rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-json-tools-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-json-tools-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-jsonschemafriend/Dockerfile
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-jsonschemafriend/build.gradle
+-rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-networknt-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-networknt-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/.dockerignore
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/.editorconfig
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/Dockerfile
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/build.gradle.kts
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/gradle.properties
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/justfile
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/settings.gradle.kts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/gradle/libs.versions.toml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-ajv/Dockerfile
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-ajv/bowtie_ajv.js
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-ajv/package-lock.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-ajv/package.json
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-hyperjump/Dockerfile
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-hyperjump/bowtie_hyperjump.js
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-hyperjump/package.json
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-json-schema/Dockerfile
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-json-schema/bowtie_json_schema.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-json-schema/package.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-jsonschema/bowtie_jsonschema.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-jsonschema/package.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-schemasafe/Dockerfile
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-schemasafe/bowtie_schemasafe.js
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/js-schemasafe/package.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/.gitignore
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/lua-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/lua-jsonschema/bowtie_jsonschema.lua
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/lua-jsonschema/json.lua
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/lua-jsonschema/stylua.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/php-opis-json-schema/Dockerfile
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/php-opis-json-schema/bowtieJsonSchema.php
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/php-opis-json-schema/composer.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/python-fastjsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/python-jschon/Dockerfile
+-rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/python-jschon/bowtie_jschon.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/python-jsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/python-jsonschema/bowtie_jsonschema.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ruby-json_schemer/.rubocop.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ruby-json_schemer/Dockerfile
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ruby-json_schemer/Gemfile
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ruby-json_schemer/Gemfile.lock
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ruby-json_schemer/bowtie_json_schemer.rb
+-rw-r--r--   0        0        0    13409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-boon/Cargo.lock
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-boon/Cargo.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-boon/Dockerfile
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-boon/build.rs
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-boon/src/main.rs
+-rw-r--r--   0        0        0    39299 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/Cargo.lock
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/Cargo.toml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/Dockerfile
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/build.rs
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/src/main.rs
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-mjs-validator/Dockerfile
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-mjs-validator/Harness.scala
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-mjs-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-mjs-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-mjs-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-rc-circe-json-validator/Dockerfile
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-rc-circe-json-validator/Harness.scala
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-rc-circe-json-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-rc-circe-json-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/scala-rc-circe-json-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ts-vscode-json-languageservice/Dockerfile
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ts-vscode-json-languageservice/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/implementations/ts-vscode-json-languageservice/tsconfig.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/conftest.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_cli.py
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_connectables.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_dialect.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_github.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_hypothesis.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_implementation.py
+-rw-r--r--   0        0        0    74314 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_integration.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_registry.py
+-rw-r--r--   0        0        0    10199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_report.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/test_schemas.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3069 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/.gitattributes
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/connectables.json
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/report.json
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/filter-implementations.json
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/info.json
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/statistics.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/test.json
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/LICENSE
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/README.rst
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/hatch_build.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.1/PKG-INFO
```

### Comparing `bowtie_json_schema-2024.5.9/.gitpod.yml` & `bowtie_json_schema-2024.6.1/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/.pre-commit-config.yaml` & `bowtie_json_schema-2024.6.1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -14,20 +14,20 @@
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.4.3"
+    rev: "v0.4.5"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.2
+    rev: 0.28.4
     hooks:
       - name: ensure bowtie's own schemas are valid
         id: check-metaschema
         files: ^bowtie/schemas/.*\.json$
   - repo: local
     hooks:
       - id: check-dependabot
@@ -47,15 +47,16 @@
       - name: black (python implementations & bowtie internals)
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v4.0.0-alpha.8"
     hooks:
       - name: prettier (javascript implementations & bowtie internals)
-        exclude: frontend/pnpm-lock.yaml
+        # REMOVEME: Once we remove Corvus's vendored metaschemas
+        exclude: ^frontend/pnpm-lock.yaml|implementations/dotnet-corvus-jsonschema/metaschema/.*.json$
         id: prettier
   - repo: https://github.com/doublify/pre-commit-rust
     rev: "v1.0"
     hooks:
       - name: cargo fmt rust-jsonschema
         id: fmt
         args:
@@ -102,15 +103,15 @@
     rev: v0.20.0
     hooks:
       - name: stylua (lua implementations)
         id: stylua
         exclude: .*/json.lua
         args: ["--config-path", "implementations/lua-jsonschema/stylua.toml"]
   - repo: https://github.com/pre-commit/mirrors-clang-format
-    rev: v18.1.4
+    rev: v18.1.5
     hooks:
       - name: clang-format (c/c++/c#/java implementations)
         id: clang-format
         types_or: [c++, c, c#, java, objective-c]
   - repo: https://github.com/dustinsand/pre-commit-jvm
     rev: v0.11.0
     hooks:
```

### Comparing `bowtie_json_schema-2024.5.9/CONTRIBUTING.rst` & `bowtie_json_schema-2024.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/action.yml` & `bowtie_json_schema-2024.6.1/action.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/noxfile.py` & `bowtie_json_schema-2024.6.1/noxfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 
 @session(default=False, tags=["build"])
 def app(session):
     """
     Build a PyApp which will run Bowtie.
     """
     session.install("hatch")
-    session.run("hatch", "build", "-t", "app", *session.posargs)
+    session.run("hatch", "build", "-t", "binary", *session.posargs)
 
 
 @session(tags=["style"])
 def style(session):
     """
     Lint for style on Bowtie's Python codebase.
     """
```

### Comparing `bowtie_json_schema-2024.5.9/.pre-commit-hooks/check-dependabot` & `bowtie_json_schema-2024.6.1/.pre-commit-hooks/check-dependabot`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/.pre-commit-hooks/check-lintsonschema-schema` & `bowtie_json_schema-2024.6.1/.pre-commit-hooks/check-lintsonschema-schema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/bowtie/_cli.py` & `bowtie_json_schema-2024.6.1/bowtie/_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from collections.abc import Callable, Iterable
 from contextlib import AsyncExitStack, asynccontextmanager
 from fnmatch import fnmatch
 from functools import wraps
 from pathlib import Path
 from pprint import pformat
+from statistics import mean, median, quantiles
 from textwrap import dedent
 from typing import TYPE_CHECKING, Literal, ParamSpec, Protocol
 import asyncio
 import json
 import logging
 import os
 import sys
@@ -53,48 +54,58 @@
         Sequence,
         Set,
     )
     from os import PathLike
     from typing import IO, Any, TextIO
 
     from click.decorators import FC
+    from httpx import Response
     from referencing.jsonschema import Schema, SchemaResource
 
-    from bowtie._commands import AnyTestResult, ImplementationId
+    from bowtie._commands import AnyTestResult
+    from bowtie._connectables import ConnectableId
     from bowtie._core import DialectRunner, ImplementationInfo, MakeValidator
 
 
 class _EX:
     def __getattr__(self, attr: str) -> int:
         return getattr(os, f"EX_{attr}", 1)  # Windows fallbacks...
 
 
 EX = _EX()
 
 STDERR = console.Console(stderr=True)
 
 
+# Evade ewels/rich-click#201
+_PROG = "main" if sys.argv[0].endswith("__main__.py") else "bowtie"
 # rich-click's CommandGroupDict seems to be missing some covariance, as using a
 # regular dict here makes pyright complain.
-_COMMAND_GROUPS = dict(
-    bowtie=[
+_COMMAND_GROUPS = {
+    _PROG: [
         CommandGroupDict(
             name="Basic Commands",
             commands=["validate", "suite", "summary", "info"],
         ),
         CommandGroupDict(
             name="Advanced Usage",
-            commands=["filter-dialects", "filter-implementations", "run"],
+            commands=[
+                "filter-dialects",
+                "filter-implementations",
+                "latest-report",
+                "run",
+                "statistics",
+            ],
         ),
         CommandGroupDict(
             name="Plumbing Commands",
             commands=["badges", "smoke"],
         ),
     ],
-)
+}
 _OPTION_GROUPS = {
     f"bowtie {command}": [
         *[
             OptionGroupDict(name=group, options=[f"--{o}" for o in options])
             for group, options in groups
         ],
         OptionGroupDict(
@@ -225,15 +236,15 @@
 
 
 class ImplementationSubcommand(Protocol):
     def __call__(
         self,
         start: Callable[
             [],
-            AsyncIterator[tuple[ImplementationId, Implementation]],
+            AsyncIterator[tuple[ConnectableId, Implementation]],
         ],
         **kwargs: Any,
     ) -> Awaitable[int | None]: ...
 
 
 SILENT = _report.Reporter(write=lambda **_: None)  # type: ignore[reportUnknownArgumentType])
 
@@ -303,15 +314,21 @@
             default=lambda: (
                 default_implementations
                 if sys.stdin.isatty() or "CI" in os.environ
                 else [line.strip() for line in sys.stdin]
             ),
             multiple=True,
             metavar="IMPLEMENTATION",
-            help="A container image which implements the bowtie IO protocol.",
+            help=(
+                "A connectable ID for a JSON Schema implementation supported "
+                "by Bowtie. May be repeated multiple times to select multiple "
+                "implementations to run."
+                "Run `bowtie filter-implementations` for the full list of "
+                "supported implementations."
+            ),
         )
         @TIMEOUT
         @wraps(fn)
         def cmd(
             connectables: Iterable[_connectables.Connectable],
             **kwargs: Any,
         ) -> int:
@@ -415,128 +432,154 @@
         badge = _report.supported_version_badge(dialects=dialects)
         dir.joinpath("supported_versions.json").write_text(json.dumps(badge))
 
 
 _F = Literal["json", "pretty", "markdown"]
 
 
-def format_option(fn: FC) -> FC:
-    def show_schema(
-        ctx: click.Context,
+def format_option(**option_kwargs: Any) -> Callable[[FC], FC]:
+    if not option_kwargs:
+        option_kwargs = dict(
+            default=lambda: "pretty" if sys.stdout.isatty() else "json",
+            show_default="pretty if stdout is a tty, otherwise JSON",
+            type=click.Choice(["json", "pretty", "markdown"]),
+        )
+
+    def _format_option(fn: FC) -> FC:
+        def show_schema(
+            ctx: click.Context,
+            param: click.Parameter | None,
+            value: bool,
+        ) -> None:
+            if not value or ctx.resilient_parsing:
+                return
+            uri = f"tag:bowtie.report,2024:cli:{ctx.command.name}"
+            schema = validator_registry().schema(uri)
+            # FIXME: Syntax highlight? But rich appears to be doing some
+            #        bizarre line wrapping, even if I disable a bunch of random
+            #        options (crop, no_wrap, word_wrap in Syntax, ...) which
+            #        fails the integration tests.
+            click.echo(json.dumps(schema, indent=2))
+            ctx.exit()
+
+        return click.option(
+            "--format",
+            "-f",
+            "format",
+            help="What format to use for the output",
+            **option_kwargs,
+        )(
+            click.option(
+                "--schema",
+                callback=show_schema,
+                expose_value=False,
+                is_eager=True,
+                is_flag=True,
+                help="Show the JSON Schema for this command's JSON output.",
+            )(fn),
+        )
+
+    return _format_option
+
+
+class _Report(click.File):
+    """
+    Select a previously produced Bowtie report.
+    """
+
+    name = "report"
+    mode = "r"
+
+    def convert(  # type: ignore[reportIncompatibleMethodOverride]
+        self,
+        value: str | PathLike[str] | IO[Any] | _report.Report,
         param: click.Parameter | None,
-        value: bool,
-    ) -> None:
-        if not value or ctx.resilient_parsing:
-            return
-        uri = f"tag:bowtie.report,2024:cli:{ctx.command.name}"
-        schema = validator_registry().schema(uri)
-        # FIXME: Syntax highlight? But rich appears to be doing some bizarre
-        #        line wrapping, even if I disable a bunch of random options
-        #        (crop, no_wrap, word_wrap in Syntax, ...) which fails the
-        #        integration tests.
-        click.echo(json.dumps(schema, indent=2))
-        ctx.exit()
+        ctx: click.Context,
+    ) -> _report.Report:
+        if isinstance(value, _report.Report):
+            return value
 
-    return click.option(
-        "--format",
-        "-f",
-        "format",
-        help="What format to use for the output",
-        default=lambda: "pretty" if sys.stdout.isatty() else "json",
-        show_default="pretty if stdout is a tty, otherwise JSON",
-        type=click.Choice(["json", "pretty", "markdown"]),
-    )(
-        click.option(
-            "--schema",
-            callback=show_schema,
-            expose_value=False,
-            is_eager=True,
-            is_flag=True,
-            help="Show the JSON Schema for this command's JSON output.",
-        )(fn),
-    )
+        input = super().convert(value, param, ctx)
+        try:
+            return _report.Report.from_serialized(input)
+        except _report.EmptyReport:
+            error = DiagnosticError(
+                code="empty-report",
+                message="The Bowtie report is empty.",
+                causes=[f"{input.name} contains no test result data."],
+                hint_stmt=(
+                    "If you are piping in report data, "
+                    "check to ensure that what you've run has succeeded, "
+                    "otherwise it may be emitting no report data."
+                ),
+            )
+            STDERR.print(error)
+            ctx.exit(EX.NOINPUT)
+        except json.JSONDecodeError as err:
+            error = DiagnosticError(
+                code="report-not-json",
+                message="The Bowtie report looks corrupt.",
+                causes=[f"{input.name} is not valid JSON.", str(err)],
+                hint_stmt=(
+                    "If you are piping in report data, "
+                    "the command producing the report has likely failed "
+                    "and the real error is above this one. "
+                    "Otherwise, ensure you are passing in a report generated "
+                    "by Bowtie."
+                ),
+            )
+            STDERR.print(error)
+            ctx.exit(EX.DATAERR)
+        except _report.MissingFooter:
+            error = DiagnosticError(
+                code="truncated-report",
+                message="The Bowtie report looks corrupt.",
+                causes=[
+                    f"{input.name} is missing its footer, which usually means "
+                    "it has been somehow truncated.",
+                ],
+                hint_stmt=(
+                    "Try running the command you used to produce the report, "
+                    "without piping it. If it crashes, file a bug report!"
+                ),
+            )
+            STDERR.print(error)
+            ctx.exit(EX.DATAERR)
 
 
 @subcommand
-@format_option
+@format_option()
 @click.option(
     "--show",
     "-s",
     default="validation",
     show_default=True,
     type=click.Choice(["failures", "validation"]),
     help=(
         "Configure whether to display validation results "
         "(whether instances are valid or not) or test failure results "
         "(whether the validation results match expected validation results)"
     ),
 )
-@click.argument(
-    "input",
-    default="-",
-    type=click.File(mode="r"),
-)
-def summary(input: TextIO, format: _F, show: str):
+@click.argument("report", default="-", type=_Report())
+def summary(report: _report.Report, format: _F, show: str):
     """
     Generate an (in-terminal) summary of a Bowtie run.
     """
-    try:
-        report = _report.Report.from_serialized(input)
-    except _report.EmptyReport:
-        error = DiagnosticError(
-            code="empty-report",
-            message="The Bowtie report is empty.",
-            causes=[f"{input.name} contains no test result data."],
-            hint_stmt=(
-                "If you are piping data into bowtie summary, "
-                "check to ensure that what you've run has succeeded, "
-                "otherwise it may be emitting no report data."
-            ),
-        )
-        STDERR.print(error)
-        return EX.NOINPUT
-    except json.JSONDecodeError as err:
-        error = DiagnosticError(
-            code="report-not-json",
-            message="The Bowtie report looks corrupt.",
-            causes=[f"{input.name} is not valid JSON.", str(err)],
-            hint_stmt=(
-                "If you are piping data, the command producing the report "
-                "has likely failed and the real error is above this one. "
-                "Otherwise, ensure you are passing in a report generated by "
-                "Bowtie."
-            ),
-        )
-        STDERR.print(error)
-        return EX.DATAERR
-    except _report.MissingFooter:
-        error = DiagnosticError(
-            code="truncated-report",
-            message="The Bowtie report looks corrupt.",
-            causes=[
-                f"{input.name} is missing its footer, which usually means "
-                "it has been somehow truncated.",
-            ],
-            hint_stmt=(
-                "Try running the command you used to produce the report, "
-                "without piping it. If it crashes, file a bug report!"
-            ),
-        )
-        STDERR.print(error)
-        return EX.DATAERR
-
     if show == "failures":
         results = report.worst_to_best()
         to_table = _failure_table
         to_markdown_table = _failure_table_in_markdown
 
         def to_serializable(  # type: ignore[reportRedeclaration]
-            value: Iterable[tuple[ImplementationInfo, Unsuccessful]],
+            value: Iterable[
+                tuple[ConnectableId, ImplementationInfo, Unsuccessful],
+            ],
         ):
-            return [(each.id, asdict(counts)) for each, counts in value]
+            return [(id, asdict(counts)) for id, _, counts in value]
 
     else:
         results = report.cases_with_results()
         to_table = _validation_results_table
         to_markdown_table = _validation_results_table_in_markdown
 
         def to_serializable(
@@ -569,17 +612,15 @@
             console.Console().print(table)
         case "markdown":
             table = to_markdown_table(report, results)  # type: ignore[reportGeneralTypeIssues]
             console.Console().print(table)
 
 
 def _convert_table_to_markdown(columns: list[str], rows: list[list[str]]):
-    widths = [
-        max(len(line[i]) for line in columns) for i in range(len(columns))
-    ]
+    widths = [max(len(row[i]) for row in rows) for i in range(len(columns))]
     rows = [[elt.center(w) for elt, w in zip(line, widths)] for line in rows]
 
     header = "| " + " | ".join(columns) + " |"
     border_left = "|:"
     border_center = ":|:"
     border_right = ":|"
 
@@ -592,68 +633,70 @@
     # body of the table
     body = [""] * len(rows)  # empty string list that we fill after
     for idx, line in enumerate(rows):
         # for each line, change the body at the correct index
         body[idx] = "| " + " | ".join(line) + " |"
     body = "\n".join(body)
 
-    return f"\n\n{header}\n{separator}\n{body}\n\n"
+    return f"\n{header}\n{separator}\n{body}"
 
 
 def _failure_table(
     report: _report.Report,
-    results: list[tuple[ImplementationInfo, Unsuccessful]],
+    results: list[tuple[ConnectableId, ImplementationInfo, Unsuccessful]],
 ):
     test = "tests" if report.total_tests != 1 else "test"
     table = Table(
         "Implementation",
         "Skips",
         "Errors",
         "Failures",
         title="Bowtie",
         caption=f"{report.total_tests} {test} ran\n",
     )
-    for each, unsuccessful in results:
+    for _, each, unsuccessful in results:
         table.add_row(
             Text.assemble(each.name, (f" ({each.language})", "dim")),
             str(unsuccessful.skipped),
             str(unsuccessful.errored),
             str(unsuccessful.failed),
         )
     return table
 
 
 def _failure_table_in_markdown(
     report: _report.Report,
-    results: list[tuple[ImplementationInfo, Unsuccessful]],
+    results: list[tuple[ConnectableId, ImplementationInfo, Unsuccessful]],
 ):
     test = "tests" if report.total_tests != 1 else "test"
     rows: list[list[str]] = []
     columns = [
         "Implementation",
         "Skips",
         "Errors",
         "Failures",
     ]
 
-    for each, unsuccessful in results:
+    for _, each, unsuccessful in results:
         rows.append(
             [
                 f"{each.name} ({each.language})",
                 str(unsuccessful.skipped),
                 str(unsuccessful.errored),
                 str(unsuccessful.failed),
             ],
         )
 
-    markdown_table = _convert_table_to_markdown(columns, rows)
-    return (
-        "# Bowtie Failures Summary"
-        + markdown_table
-        + f"**{report.total_tests} {test} ran**\n"
+    return "\n".join(
+        [
+            "# Bowtie Failures Summary",
+            _convert_table_to_markdown(columns, rows),
+            "",
+            f"**{report.total_tests} {test} ran**",
+        ],
     )
 
 
 def _validation_results_table(
     report: _report.Report,
     results: Iterable[
         tuple[TestCase, Iterable[tuple[Test, Mapping[str, AnyTestResult]]]],
@@ -668,15 +711,15 @@
     )
 
     # TODO: sort the columns by results?
     implementations = report.implementations
 
     for case, test_results in results:
         subtable = Table("Instance", box=box.SIMPLE_HEAD)
-        for implementation in implementations:
+        for implementation in implementations.values():
             subtable.add_column(
                 Text.assemble(
                     implementation.name,
                     (f" ({implementation.language})", "dim"),
                 ),
             )
 
@@ -684,18 +727,15 @@
             subtable.add_row(
                 Syntax(
                     json.dumps(test.instance),
                     lexer=JsonLexer(),
                     background_color="default",
                     word_wrap=True,
                 ),
-                *(
-                    Text(test_result[each.id].description)
-                    for each in implementations
-                ),
+                *(Text(test_result[id].description) for id in implementations),
             )
 
         table.add_row(
             Syntax(
                 json.dumps(case.schema, indent=2),
                 lexer=JSONSchemaLexer(str(report.metadata.dialect.uri)),
                 background_color="default",
@@ -716,28 +756,25 @@
 ):
     rows_data: list[list[str]] = []
     final_content = ""
 
     inner_table_columns = ["Instance"]
     implementations = report.implementations
     inner_table_columns.extend(
-        f"{implementation.name} ({implementation.language})"
-        for implementation in implementations
+        f"{id} ({implementation.language})"
+        for id, implementation in implementations.items()
     )
 
     for case, test_results in results:
         inner_table_rows: list[list[str]] = []
         for test, test_result in test_results:
             inner_table_rows.append(
                 [
                     json.dumps(test.instance),
-                    *(
-                        test_result[each.id].description
-                        for each in implementations
-                    ),
+                    *(test_result[id].description for id in implementations),
                 ],
             )
         inner_markdown_table = _convert_table_to_markdown(
             inner_table_columns,
             inner_table_rows,
         )
         schema_name = json.dumps(case.schema, indent=2)
@@ -748,24 +785,106 @@
         final_content += f"### {idx+1}. Schema:\n {row_data[0]}\n\n"
         final_content += "### Results:"
         final_content += row_data[1]
 
     return final_content
 
 
-def make_validator(*more_schemas: SchemaResource):
-    validators = more_schemas @ validator_registry()
+@subcommand
+@format_option()
+@click.option(
+    "--quantiles",
+    "n",
+    default=4,
+    type=int,
+    help=(
+        "How many quantiles should be emitted for the compliance numbers? "
+        "Computing quantiles only is sensical if this number is more than the "
+        "number of implementations reported on. By default, we compute "
+        "quartiles."
+    ),
+)
+@click.argument(
+    "report",
+    default=lambda: (
+        "-"
+        if not sys.stdin.isatty()
+        else _report.Report.from_serialized(
+            asyncio.run(Dialect.latest().latest_report()).iter_lines(),
+        )
+    ),
+    type=_Report(),
+)
+def statistics(
+    report: _report.Report,
+    n: int,
+    format: _F,
+):
+    """
+    Show summary statistics for a Bowtie generated report.
+
+    If stdin is a TTY, the most recent public report for the latest JSON Schema
+    dialect is downloaded.
+    Otherwise, if it *is not* a TTY (e.g. if it is a pipe) then it should
+    contain report data.
+
+    Piping input via:
+
+      $ bowtie latest-report --dialect <some-dialect> | bowtie statistics
+
+    can be useful to retrieve the latest report for a specific dialect.
+    """
+    dialect, ran_on_date = report.metadata.dialect, report.metadata.started
+    unsuccessful = report.compliance_by_implementation().values()
+    statistics = dict(
+        median=median(unsuccessful),
+        mean=mean(unsuccessful),
+        **(  # quantiles only make sense for n < len(data)
+            {"quantiles": quantiles(unsuccessful, n=n)}
+            if n < len(unsuccessful)
+            else {}
+        ),
+    )
+    match format:
+        case "json":
+            statistics = {
+                "dialect": str(dialect.uri),
+                "ran_on": ran_on_date.isoformat(),
+                **statistics,
+            }
+            click.echo(json.dumps(statistics, indent=2))
+        case "pretty":
+            click.echo(
+                f"Dialect: {dialect.pretty_name}\n"
+                f"Ran on: {ran_on_date.strftime('%x %X %Z')}\n",
+            )
+            for k, v in statistics.items():
+                click.echo(f"{k}: {v}")
+        case "markdown":
+            heading = (
+                f"## Dialect: {dialect.pretty_name}\n\n"
+                f"### Ran on: {ran_on_date.strftime('%x %X %Z')}\n"
+            )
+            markdown = _convert_table_to_markdown(
+                columns=["Metric", "Value"],
+                rows=[[k, str(v)] for k, v in statistics.items()],
+            )
+            click.echo(heading + markdown)
+
+
+def make_validator():
+    validators = validator_registry()
 
     def validate(instance: Any, schema: Schema) -> None:
         # FIXME: There's work to do upstream in referencing, but we still are
         # probably able to make this a bit better here as well
         validator = validators.for_schema(schema)
         errors = list(validator.errors_for(instance))
         if errors:
-            raise ProtocolError(errors=errors)  # type: ignore[reportPrivateUsage]
+            raise ProtocolError(errors=errors)
 
     return validate
 
 
 def do_not_validate(*ignored: SchemaResource) -> Callable[..., None]:
     return lambda *args, **kwargs: None
 
@@ -849,30 +968,30 @@
         ctx: click.Context | None,
     ) -> CaseTransform:
         return lambda cases: (
             case for case in cases if fnmatch(case.description, f"*{value}*")
         )
 
 
-def _set_dialect(ctx: click.Context, _, value: _Dialect):
+def _set_dialect_via_schema(ctx: click.Context, _, value: _Dialect):
     """
     Set the dialect according to a possibly present :kw:`$schema` keyword.
     """
     if value:
         return value
     schema = ctx.params.get("schema")
     dialect_from_schema: str | None = (  # type: ignore[reportUnknownVariableType]
         schema.get("$schema")  # type: ignore[reportUnknownMemberType]
         if isinstance(schema, dict)
         else None
     )
     return (
         Dialect.from_str(dialect_from_schema)  # type: ignore[reportUnknownArgumentType]
         if dialect_from_schema
-        else max(Dialect.known())
+        else Dialect.latest()
     )
 
 
 def _set_schema(dialect: Dialect) -> CaseTransform:
     """
     Explicitly set a dialect on schemas passing through by setting ``$schema``.
     """
@@ -887,27 +1006,20 @@
     "--implementation",
     "-i",
     "connectables",
     type=_connectables.ClickParam(),
     required=True,
     multiple=True,
     metavar="IMPLEMENTATION",
-    help="A container image which implements the bowtie IO protocol.",
-)
-DIALECT = click.option(
-    "--dialect",
-    "-D",
-    "dialect",
-    type=_Dialect(),
-    callback=_set_dialect,
-    show_default=True,
-    metavar="URI_OR_NAME",
     help=(
-        "A URI or shortname identifying the dialect of each test. Possible "
-        f"shortnames include: {', '.join(sorted(Dialect.by_alias()))}."
+        "A connectable ID for a JSON Schema implementation supported "
+        "by Bowtie. May be repeated multiple times to select multiple "
+        "implementations to run."
+        "Run `bowtie filter-implementations` for the full list of "
+        "supported implementations."
     ),
 )
 FILTER = click.option(
     "--filter",
     "-k",
     default="",
     type=_Filter(),
@@ -960,14 +1072,36 @@
         "specification. Generally, this option protects against broken Bowtie "
         "implementations and can be left at its default (of off) unless "
         "you are developing a new implementation container."
     ),
 )
 
 
+def dialect_option(
+    default: Dialect | None = Dialect.latest(),
+    **kwargs: Any,
+):
+    if default is not None:
+        kwargs.update(default=default, show_default=default.pretty_name)
+
+    shortnames = ", ".join(sorted(Dialect.by_alias()))
+    return click.option(
+        "--dialect",
+        "-D",
+        "dialect",
+        type=_Dialect(),
+        metavar="URI_OR_NAME",
+        help=(
+            "A URI or shortname identifying the dialect of each test. "
+            f"Possible shortnames include: {shortnames}."
+        ),
+        **kwargs,
+    )
+
+
 def fail_fast(fn: FC) -> FC:
     conflict = "don't provide both --fail-fast and --max-fail / --max-error"
 
     # Both are these are needed because parsing is order dependent :/
     def disallow_fail_fast(
         ctx: click.Context,
         _,
@@ -1026,16 +1160,16 @@
         param: click.Parameter | None,
         ctx: click.Context | None,
     ) -> Any:
         return json.load(super().convert(value, param, ctx))
 
 
 @subcommand
+@dialect_option()
 @IMPLEMENTATION
-@DIALECT
 @FILTER
 @fail_fast
 @SET_SCHEMA
 @TIMEOUT
 @VALIDATE
 @click.argument(
     "input",
@@ -1059,16 +1193,16 @@
         TestCase.from_dict(dialect=dialect, **json.loads(line))
         for line in input
     )
     return asyncio.run(_run(**kwargs, cases=cases, dialect=dialect))
 
 
 @subcommand
+@dialect_option(default=None, callback=_set_dialect_via_schema)
 @IMPLEMENTATION
-@DIALECT
 @SET_SCHEMA
 @TIMEOUT
 @VALIDATE
 @click.option(
     "-d",
     "--description",
     default="bowtie validate",
@@ -1118,14 +1252,19 @@
 KNOWN_LANGUAGES = {
     *LANGUAGE_ALIASES.values(),
     *(i.partition("-")[0] for i in Implementation.known()),
 }
 
 
 @implementation_subcommand()  # type: ignore[reportArgumentType]
+@format_option(
+    default="plain",
+    show_default=True,
+    type=click.Choice(["plain", "json"]),
+)
 @click.option(
     "--supports-dialect",
     "-d",
     "dialects",
     type=_Dialect(),
     default=frozenset(),
     metavar="URI_OR_NAME",
@@ -1151,33 +1290,41 @@
     multiple=True,
     metavar="LANGUAGE",
     help="Only include implementations in the given programming language",
 )
 async def filter_implementations(
     start: Callable[
         [],
-        AsyncIterator[tuple[ImplementationId, Implementation]],
+        AsyncIterator[tuple[ConnectableId, Implementation]],
     ],
     dialects: Sequence[Dialect],
     languages: Set[str],
+    format: Literal["plain", "json"],
 ):
     """
     Output implementations which match the given criteria.
 
     Useful for piping or otherwise using the resulting output for further
     Bowtie commands.
     """
     if not dialects and languages == KNOWN_LANGUAGES:
-        for name in start.connectables:  # type: ignore[reportFunctionMemberAccess]
-            click.echo(name)
-        return
-
-    async for name, each in start():
-        if each.supports(*dialects) and each.info.language in languages:
-            click.echo(name)
+        matching = start.connectables  # type: ignore[reportFunctionMemberAccess]
+    else:
+        matching = [
+            name
+            async for name, each in start()
+            if each.supports(*dialects) and each.info.language in languages
+        ]
+
+    match format:
+        case "json":
+            click.echo(json.dumps(matching, indent=2))
+        case "plain":
+            for name in matching:
+                click.echo(name)
 
 
 @implementation_subcommand(default_implementations=frozenset())  # type: ignore[reportArgumentType]
 @click.option(
     "--dialect",
     "-d",
     "dialects",
@@ -1204,15 +1351,15 @@
         "If provided, show only dialects which do (or do not) "
         "support boolean schemas. Otherwise show either kind."
     ),
 )
 async def filter_dialects(
     start: Callable[
         [],
-        AsyncIterator[tuple[ImplementationId, Implementation]],
+        AsyncIterator[tuple[ConnectableId, Implementation]],
     ],
     dialects: Iterable[Dialect],
     latest: bool,
     booleans: bool | None,
 ):
     """
     Output dialect URIs matching a given criteria.
@@ -1235,27 +1382,41 @@
 
     for dialect in sorted(matching, reverse=True):
         click.echo(dialect.uri)
         if latest:
             break
 
 
+@subcommand
+@dialect_option()
+def latest_report(dialect: Dialect):
+    """
+    Output the latest published report from Bowtie's website.
+    """
+
+    async def write(response: Awaitable[Response]):
+        async for chunk in (await response).aiter_bytes():
+            click.echo(chunk)
+
+    asyncio.run(write(dialect.latest_report()))
+
+
 @implementation_subcommand()  # type: ignore[reportArgumentType]
-@format_option
+@format_option()
 async def info(
     start: Callable[
         [],
-        AsyncIterator[tuple[ImplementationId, Implementation]],
+        AsyncIterator[tuple[ConnectableId, Implementation]],
     ],
     format: _F,
 ):
     """
     Show information about a supported implementation.
     """
-    serializable: dict[ImplementationId, dict[str, Any]] = {}
+    serializable: dict[ConnectableId, dict[str, Any]] = {}
 
     async for _, each in start():
         metadata = [(k, v) for k, v in each.info.serializable().items() if v]
         metadata.sort(
             key=lambda kv: (
                 kv[0] != "name",
                 kv[0] != "language",
@@ -1264,15 +1425,15 @@
                 kv[0] == "dialects",
                 kv[0],
             ),
         )
 
         match format:
             case "json":
-                serializable[each.name] = dict(metadata)
+                serializable[each.id] = dict(metadata)
             case "pretty":
                 click.echo(
                     "\n".join(
                         f"{k}: {json.dumps(v, indent=2)}" for k, v in metadata
                     ),
                 )
             case "markdown":
@@ -1299,30 +1460,30 @@
     # I have no idea why Click makes this so hard, but no combination of:
     #     type, default, is_flag, flag_value, nargs, ...
     # makes this work without doing it manually with callback.
     callback=lambda _, __, v: click.echo if not v else lambda *_, **__: None,  # type: ignore[reportUnknownLambdaType]
     is_flag=True,
     help="Don't print any output, just exit with nonzero status on failure.",
 )
-@format_option
+@format_option()
 async def smoke(
     start: Callable[
         [],
-        AsyncIterator[tuple[ImplementationId, Implementation]],
+        AsyncIterator[tuple[ConnectableId, Implementation]],
     ],
     format: _F,
     echo: Callable[..., None],
 ) -> int:
     """
     Smoke test implementations for basic correctness against Bowtie's protocol.
     """
     exit_code = 0
 
     async for _, implementation in start():
-        echo(f"Testing {implementation.name!r}...\n", file=sys.stderr)
+        echo(f"Testing {implementation.id!r}...\n", file=sys.stderr)
         serializable: list[dict[str, Any]] = []
         implementation_exit_code = 0
 
         async for _, results in implementation.smoke():
             async for case, result in results:
                 if result.unsuccessful():
                     implementation_exit_code |= EX.DATAERR
@@ -1421,15 +1582,15 @@
     max_fail: int | None = None,
     max_error: int | None = None,
     run_metadata: dict[str, Any] = {},
     reporter: _report.Reporter = _report.Reporter(),
     **kwargs: Any,
 ) -> int:
     exit_code = 0
-    acknowledged: list[ImplementationInfo] = []
+    acknowledged: Mapping[ConnectableId, ImplementationInfo] = {}
     runners: list[DialectRunner] = []
     async with _start(
         connectables=connectables,
         reporter=reporter,
         **kwargs,
     ) as starting:
         for each in starting:
@@ -1444,15 +1605,15 @@
                 runner = await implementation.start_speaking(dialect)
             except DialectError as error:
                 exit_code |= EX.CONFIG
                 STDERR.print(error)
             except UnsupportedDialect as error:
                 STDERR.print(error)
             else:
-                acknowledged.append(implementation.info)
+                acknowledged[implementation.id] = implementation.info
                 runners.append(runner)
 
         if not runners:
             STDERR.print(
                 "[bold red]No implementations started successfully![/]",
             )
             return exit_code | EX.CONFIG
```

### Comparing `bowtie_json_schema-2024.5.9/bowtie/_commands.py` & `bowtie_json_schema-2024.6.1/bowtie/_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,37 +5,35 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Protocol, TypeVar
 import re
 
 try:
     from typing import dataclass_transform
-except ImportError:
+except ImportError:  # pragma: no cover
     from typing_extensions import dataclass_transform
 
 from attrs import asdict, field, filters, frozen
 from url import URL
 
 from bowtie import HOMEPAGE, exceptions
 
 if TYPE_CHECKING:
     from collections.abc import Awaitable, Callable, Mapping, Sequence
     from typing import ClassVar, Self
 
     from structlog.stdlib import BoundLogger
 
+    from bowtie._connectables import ConnectableId
     from bowtie._core import Dialect as _Dialect, DialectRunner, TestCase
 
 
 #: A unique identifier for a test case within a run or report.
 Seq = int | str
 
-#: A unique identifier for an implementation within a run or report.
-ImplementationId = str
-
 #: A JSON representation of the command
 Message = dict[str, Any]
 
 
 @frozen
 class Unsuccessful:
     failed: int = 0
@@ -293,15 +291,15 @@
 
     Knows how long the result was *supposed* to be, and what the expected
     validation results were supposed to be if that information was provided at
     run-time.
     """
 
     seq: Seq
-    implementation: ImplementationId
+    implementation: ConnectableId
 
     result: AnyCaseResult
     expected: Sequence[bool | None]
 
     @classmethod
     def from_dict(
         cls,
@@ -354,15 +352,15 @@
 
 @frozen
 class CaseResult:
     """
     A test case which at least was run by the implementation.
     """
 
-    results: list[AnyTestResult]
+    results: Sequence[AnyTestResult]
 
     @classmethod
     def from_results(cls, results: list[dict[str, Any]]):
         return cls(results=[TestResult.from_dict(t) for t in results])
 
     def serializable(self) -> Message:
         return dict(results=[result.serializable() for result in self.results])
```

### Comparing `bowtie_json_schema-2024.5.9/bowtie/_connectables.py` & `bowtie_json_schema-2024.6.1/bowtie/_connectables.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,79 @@
 """
 Connectables implement a mini-language for connecting to supported harnesses.
-
-They allow connecting to various kinds of harnesses over different
-"connectors", for example:
-
-    * in a container which Bowtie manages (starts and stops)
-    * in a pre-existing / externally managed container (not yet implemented)
-    * in-memory within Bowtie itself, with no IPC (not yet implemented)
-
-The general form of a connectable is:
-
-    [<connector>:]<id>[:<arguments>*]
-
-where the connector indicates how to connect to the harness.
-
-The currently supported connectors are:
-
-    * ``image``: a container image which Bowtie will start, stop and delete
-                 which must speak Bowtie's harness protocol
-
-If no connector is specified, ``image`` is assumed.
-
-The ``id`` is interpreted in a connector-specific manner and should indicate
-the specific intended implementation. For example, for container images, it
-must be the name of a container image which will be pulled if needed.
-It need not be fully qualified (i.e. include the repository),
-and will default to pulling from Bowtie's own image repository.
-
-Connectables are loosely inspired by `Twisted's strports
-<twisted.internet.endpoints.clientFromString`.
 """
 
 from __future__ import annotations
 
 from contextlib import asynccontextmanager
 from typing import TYPE_CHECKING, Any, Protocol
 
 from attrs import field, frozen
 from click.shell_completion import CompletionItem
 from rpds import HashTrieMap
 import click
 
-from bowtie import _containers
+from bowtie import _containers, _direct_connectable
 from bowtie._core import Implementation
 
 if TYPE_CHECKING:
     from collections.abc import AsyncIterator
     from contextlib import AbstractAsyncContextManager
 
-    from bowtie._commands import ImplementationId
     from bowtie._core import Connection
 
 
 class UnknownConnector(Exception):
     """
     The connector provided does not exist.
     """
 
 
 class Connector(Protocol):
 
     #: The string name of this connector type.
     connector: str
 
+    def __init__(self, id: str): ...
+
     def connect(self) -> AbstractAsyncContextManager[Connection]: ...
 
 
+#: A string identifying an implementation supporting Bowtie's harness protocol.
+#: Connectable IDs should be unique within a run or report.
+ConnectableId = str
+
+
 @frozen
 class Connectable:
+    """
+    A parsed connectable description.
+
+    In this internal codebase and in docstrings, "connectable" refers to
+    instances of this object, and we use "connectable description" to refer
+    to the string which specifies the connectable.
+
+    In user-facing documentation, we simplify talking about connectables by
+    simply referring to the string as being the connectable itself.
+    """
 
-    _id: str = field(alias="id", repr=False)
+    _id: ConnectableId = field(alias="id", repr=False)
     _connector: Connector = field(alias="connector")
 
     _connectors = HashTrieMap(
         (cls.connector, cls)
         for cls in [
             _containers.ConnectableImage,
+            _containers.ConnectableContainer,
+            _direct_connectable.Direct,
         ]
     )
 
     @classmethod
-    def from_str(cls, fqid: ImplementationId):
+    def from_str(cls, fqid: ConnectableId):
         connector, sep, id = fqid.partition(":")
         if not sep:
             connector, id = "image", connector
         Connector = cls._connectors.get(connector)
         if Connector is None:
             if "/" in connector:
                 return cls(id=fqid, connector=cls._connectors["image"](fqid))
@@ -99,15 +88,15 @@
                 id=self._id,
                 connection=connection,
                 **kwargs,
             ) as implementation,
         ):
             yield implementation
 
-    def to_terse(self) -> ImplementationId:
+    def to_terse(self) -> ConnectableId:
         """
         The tersest connectable description someone could write.
         """
         return self._id.removeprefix("image:").removeprefix(
             f"{_containers.IMAGE_REPOSITORY}/",
         )
```

### Comparing `bowtie_json_schema-2024.5.9/bowtie/_containers.py` & `bowtie_json_schema-2024.6.1/bowtie/_containers.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Some of this is warts from aiodocker, but mixed in with fun
 special-to-this-package logic occasionally.
 """
 
 from __future__ import annotations
 
 from collections import deque
-from contextlib import asynccontextmanager, suppress
+from contextlib import AsyncExitStack, asynccontextmanager, suppress
 from typing import TYPE_CHECKING
 import asyncio
 import json
 
 from aiodocker import Docker
 from attrs import field, frozen, mutable
 import aiodocker.exceptions
@@ -22,20 +22,18 @@
     InvalidResponse,
     NoSuchImplementation,
     Restarted,
     StartupFailed,
 )
 
 if TYPE_CHECKING:
-    from collections.abc import AsyncIterator, Awaitable
-    from contextlib import AbstractAsyncContextManager
-    from typing import Any, Self
+    from collections.abc import AsyncIterator, Awaitable, Callable
+    from typing import Any
 
     import aiodocker.containers
-    import aiodocker.docker
     import aiodocker.stream  # noqa: TCH004 ??? no it's not?
 
     from bowtie._commands import Message
 
 
 IMAGE_REPOSITORY = "ghcr.io/bowtie-json-schema"
 
@@ -132,150 +130,57 @@
                 return line.decode()  # type: ignore[reportUnknownVariableType]
 
             message = None
             while message is None:
                 message = await self._read_with_timeout()
             self._last += line  # type: ignore[reportUnknownMemberType]
 
-    async def ensure_deleted(self):
-        with suppress(aiodocker.exceptions.DockerError):
-            await self._container.delete(force=True)  # type: ignore[reportUnknownMemberType]
-
 
 @mutable
 class Connection:
     """
     A connection with a restartable container over stdio via request/responses.
 
     Requests and responses are JSON-serializable messages, with serialization
     handled here.
     """
 
-    _image: str = field(alias="image")
-
-    _docker: aiodocker.docker.Docker = field(repr=False, alias="docker")
-    _stream: Stream = field(default=None, repr=False, alias="stream")
+    _new_stream: Callable[[], Awaitable[Stream]] = field(
+        repr=False,
+        alias="new_stream",
+    )
 
     # Maybe second versions of these will be useful also at the Implementation
     # level again, to control for non-protocol-related flakiness or slowness
     _restarts: int = field(default=10, repr=False, alias="restarts")
-    _read_timeout_sec: float | None = field(
-        default=2.0,
-        converter=lambda value: value or None,  # type: ignore[reportUnknownLambdaType]
-        repr=False,
-    )
 
     #: A per-request number of retries, before giving up
     _retry: int = field(default=3, repr=False)
 
-    @classmethod
-    @asynccontextmanager
-    async def open(
-        cls,
-        image_name: str,
-        **kwargs: Any,
-    ) -> AsyncIterator[Self]:
-        async with Docker() as docker:
-            self = cls(docker=docker, image=image_name, **kwargs)
+    _connected_to: Stream | None = None
 
-            try:
-                await self._start_container_maybe_pull()
-            except GotStderr as error:
-                err = StartupFailed(
-                    name=image_name,
-                    stderr=error.stderr.decode(),
-                )
-                raise err from None
-            except _ClosedStream:
-                raise StartupFailed(name=image_name) from None
-
-            yield self
-            await self._stream.ensure_deleted()
-
-    async def _start_container_maybe_pull(self):
-        # You would think we would use aiodocker's container.start() function
-        # which essentially does the below. You would think wrong.
-        # That function will pull the *entire* image repository if it ends up
-        # pulling our harness image -- so here we reimplement it, but only
-        # pull :latest when the image is missing.
-        try:
-            await self._start_container()
-        except aiodocker.exceptions.DockerError as err:
-            if err.status != 404:  # noqa: PLR2004
-                raise
-            try:
-                await self._docker.pull(from_image=self._image, tag="latest")  # type: ignore[reportUnknownMemberType]
-            except aiodocker.exceptions.DockerError as err:
-                # This craziness can go wrong in various ways, none of them
-                # machine parseable.
-
-                status, data, *_ = err.args
-                if data.get("cause") == "image not known":
-                    raise NoSuchImplementation(self._image) from err
-
-                message = ghcr = data.get("message", "")
-
-                if status == 500:  # noqa: PLR2004
-                    try:
-                        # GitHub Registry saying an image doesn't exist as
-                        # reported within GitHub Actions' version of Podman...
-                        # This is some crazy string like:
-                        #   Head "https://ghcr.io/v2/bowtie-json-schema/image-name/manifests/latest": denied  # noqa: E501
-                        # with seemingly no other indication elsewhere and
-                        # obviously no good way to detect this specific case
-                        no_image = message.endswith('/latest": denied')
-                    except Exception:  # noqa: BLE001, S110
-                        pass
-                    else:
-                        if no_image:
-                            raise NoSuchImplementation(self._image)
-
-                    try:
-                        # GitHub Registry saying an image doesn't exist as
-                        # reported locally via podman on macOS...
-
-                        # message will be ... a JSON string !?! ...
-                        error = json.loads(ghcr).get("message", "")
-                    except Exception:  # noqa: BLE001, S110
-                        pass  # nonJSON / missing key
-                    else:
-                        if "403 (forbidden)" in error.casefold():
-                            raise NoSuchImplementation(self._image)
-
-                raise StartupFailed(name=self._image, data=data) from err
-            await self._start_container()
-
-    async def _start_container(self):
-        config = dict(
-            Image=self._image,
-            OpenStdin=True,
-            HostConfig=dict(NetworkMode="none"),
-        )
-        # FIXME: name + labels
-        container = await self._docker.containers.create(config=config)  # type: ignore[reportUnknownMemberType]
-        await container.start()  # type: ignore[reportUnknownMemberType]
-        self._stream = Stream.attached_to(
-            container,
-            read_timeout_sec=self._read_timeout_sec,
-        )
+    @property
+    async def _stream(self) -> Stream:
+        if self._connected_to is None:
+            self._connected_to = await self._new_stream()
+        return self._connected_to
 
     async def request(self, message: Message) -> Message | None:
         request = f"{json.dumps(message)}\n"
 
         try:
-            await self._stream.send(request)
+            await (await self._stream).send(request)
         except _ClosedStream:
             self._restarts -= 1
-            await self._stream.ensure_deleted()
-            await self._start_container()
+            self._connected_to = None
             raise Restarted() from None
 
         for _ in range(self._retry):
             try:
-                response = await self._stream.receive()
+                response = await (await self._stream).receive()
             except asyncio.exceptions.TimeoutError:
                 continue
             except _ClosedStream as err:
                 stderr: list[str] = await err.container.log(stderr=True)  # type: ignore[reportUnknownVariableType]
                 if stderr:
                     raise GotStderr("".join(stderr).encode())  # type: ignore[reportUnknownVariableType]
                 return
@@ -284,24 +189,140 @@
                 return json.loads(response)
             except json.JSONDecodeError as err:
                 raise InvalidResponse(contents=response) from err
 
     async def poison(self, message: dict[str, Any]) -> None:
         request = f"{json.dumps(message)}\n"
         with suppress(_ClosedStream):
-            await self._stream.send(request)
+            await (await self._stream).send(request)
 
 
 @frozen
 class ConnectableImage:
 
     _id: str = field(
-        converter=lambda value: (  # type: ignore[reportUnknownLambdaType]
+        converter=lambda value: (
             value if "/" in value else f"{IMAGE_REPOSITORY}/{value}"
         ),
         alias="id",
     )
 
     connector = "image"
 
-    def connect(self) -> AbstractAsyncContextManager[Connection]:
-        return Connection.open(image_name=self._id)
+    @asynccontextmanager
+    async def connect(self) -> AsyncIterator[Connection]:
+        async with AsyncExitStack() as stack:
+            docker = await stack.enter_async_context(Docker())
+            create = start_container_maybe_pull
+
+            async def new_stream():
+                nonlocal create
+
+                container = await create(docker=docker, image_name=self._id)
+                stack.push_async_callback(container.delete, force=True)  # type: ignore[reportUnknownMemberType]
+                create = start_container
+
+                try:
+                    return Stream.attached_to(
+                        container,
+                        read_timeout_sec=2.0,  # FIXME: Parameters
+                    )
+                except GotStderr as error:
+                    err = StartupFailed(
+                        id=self._id,
+                        stderr=error.stderr.decode(),
+                    )
+                    raise err from None
+                except _ClosedStream:
+                    raise StartupFailed(id=self._id) from None
+
+            yield Connection(new_stream=new_stream)
+
+
+async def start_container_maybe_pull(docker: Docker, image_name: str):
+    # You would think we would use aiodocker's container.start() function
+    # which essentially does the below. You would think wrong.
+    # That function will pull the *entire* image repository if it ends up
+    # pulling our harness image -- so here we reimplement it, but only
+    # pull :latest when the image is missing.
+    try:
+        return await start_container(docker=docker, image_name=image_name)
+    except aiodocker.exceptions.DockerError as err:
+        if err.status != 404:  # noqa: PLR2004
+            raise
+        try:
+            await docker.pull(from_image=image_name, tag="latest")  # type: ignore[reportUnknownMemberType]
+        except aiodocker.exceptions.DockerError as err:
+            # This craziness can go wrong in various ways, none of them
+            # machine parseable.
+
+            status, data, *_ = err.args
+            if data.get("cause") == "image not known":
+                raise NoSuchImplementation(image_name) from err
+
+            message = ghcr = data.get("message", "")
+
+            if status == 500:  # noqa: PLR2004
+                try:
+                    # GitHub Registry saying an image doesn't exist as
+                    # reported within GitHub Actions' version of Podman...
+                    # This is some crazy string like:
+                    #   Head "https://ghcr.io/v2/bowtie-json-schema/image-name/manifests/latest": denied  # noqa: E501
+                    # with seemingly no other indication elsewhere and
+                    # obviously no good way to detect this specific case
+                    no_image = message.endswith('/latest": denied')
+                except Exception:  # noqa: BLE001, S110
+                    pass
+                else:
+                    if no_image:
+                        raise NoSuchImplementation(image_name)
+
+                try:
+                    # GitHub Registry saying an image doesn't exist as
+                    # reported locally via podman on macOS...
+
+                    # message will be ... a JSON string !?! ...
+                    error = json.loads(ghcr).get("message", "")
+                except Exception:  # noqa: BLE001, S110
+                    pass  # nonJSON / missing key
+                else:
+                    if "403 (forbidden)" in error.casefold():
+                        raise NoSuchImplementation(image_name)
+
+            raise StartupFailed(id=image_name, data=data) from err
+        return await start_container(docker=docker, image_name=image_name)
+
+
+async def start_container(docker: Docker, image_name: str):
+    config = dict(
+        Image=image_name,
+        OpenStdin=True,
+        HostConfig=dict(NetworkMode="none"),
+    )
+    # FIXME: name + labels
+    container = await docker.containers.create(config=config)  # type: ignore[reportUnknownMemberType]
+    await container.start()  # type: ignore[reportUnknownMemberType]
+    return container
+
+
+@frozen
+class ConnectableContainer:
+
+    _id: str = field(alias="id")
+
+    connector = "container"
+
+    @asynccontextmanager
+    async def connect(self) -> AsyncIterator[Connection]:
+        async with Docker() as docker:
+            try:
+                container = await docker.containers.get(self._id)  # type: ignore[reportUnknownMemberType]
+            except aiodocker.exceptions.DockerError as err:
+                raise NoSuchImplementation(id=self._id) from err
+
+            async def new_stream():
+                return Stream.attached_to(
+                    container,
+                    read_timeout_sec=2.0,  # FIXME: Parameters
+                )
+
+            yield Connection(new_stream=new_stream)
```

### Comparing `bowtie_json_schema-2024.5.9/bowtie/_core.py` & `bowtie_json_schema-2024.6.1/bowtie/_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from __future__ import annotations
 
+from collections.abc import Callable
 from contextlib import asynccontextmanager
 from datetime import date
 from functools import cache
 from importlib.resources import files
 from pathlib import Path
-from typing import TYPE_CHECKING, Protocol, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Protocol, TypeVar, cast
 from uuid import uuid4
 import json
 
 from attrs import asdict, evolve, field, frozen, mutable
 from diagnostic import DiagnosticError
 from referencing.jsonschema import EMPTY_REGISTRY, Schema, specification_with
 from rich.panel import Panel
 from rpds import HashTrieMap
 from url import URL
+import httpx
 import referencing_loaders
 
+from bowtie import HOMEPAGE
 from bowtie._commands import (
     START_V1,
     STOP,
     CaseErrored,
     Dialect as DialectCommand,
     SeqCase,
     SeqResult,
@@ -28,34 +31,33 @@
 )
 from bowtie._registry import ValidatorRegistry
 from bowtie.exceptions import DialectError, ProtocolError, UnsupportedDialect
 
 if TYPE_CHECKING:
     from collections.abc import (
         AsyncIterator,
-        Callable,
         Iterable,
         Mapping,
         Sequence,
         Set,
     )
-    from typing import Any, Self
+    from typing import Self
 
     from referencing import Specification
     from referencing.jsonschema import SchemaRegistry, SchemaResource
     from rich.console import Console, ConsoleOptions, RenderResult
 
     from bowtie._commands import (
         AnyCaseResult,
         Command,
-        ImplementationId,
         Message,
         Run,
         Seq,
     )
+    from bowtie._connectables import ConnectableId
     from bowtie._report import Reporter
 
 
 @frozen
 class Dialect:
     """
     A dialect of JSON Schema.
@@ -104,14 +106,22 @@
 
         return frozenset(
             Dialect.from_dict(**each)
             for each in json.loads(data.joinpath("dialects.json").read_text())
         )
 
     @classmethod
+    @cache
+    def latest(cls):
+        """
+        The latest dialect known to Bowtie.
+        """
+        return max(cls.known())
+
+    @classmethod
     def from_dict(
         cls,
         firstPublicationDate: str,
         prettyName: str,
         shortName: str,
         uri: str,
         aliases: Iterable[str] = (),
@@ -128,48 +138,38 @@
             has_boolean_schemas=hasBooleanSchemas,
         )
 
     @classmethod
     def from_str(cls, uri: str):
         return cls.by_uri()[URL.parse(uri)]
 
+    async def latest_report(self):
+        url = HOMEPAGE / f"{self.short_name}.json"
+        async with httpx.AsyncClient() as client:
+            return await client.get(str(url))
+
     def serializable(self):
         return str(self.uri)
 
     def specification(self, **kwargs: Any) -> Specification[SchemaResource]:
         return specification_with(str(self.uri), **kwargs)
 
-    def current_dialect_resource(self) -> SchemaResource:
-        referrer = validator_registry().schema(
-            "tag:bowtie.report,2024:ihop:schemaInCurrentDialect",
-        )
-
-        # it's of course unimportant what dialect is used for this referencing
-        # schema, what matters is that the target dialect is applied
-        from referencing.jsonschema import DRAFT202012
-
-        return DRAFT202012.create_resource(
-            {
-                "$id": referrer["$ref"],  # type: ignore[reportIndexIssue]
-            },
-        )
-
 
 @frozen
 class NoSuchImplementation(Exception):
     """
     An implementation with the given name does not exist.
     """
 
-    name: str
+    id: str
 
     def __rich__(self):
         return DiagnosticError(
             code="no-such-implementation",
-            message=f"{self.name!r} is not a known Bowtie implementation.",
+            message=f"{self.id!r} is not a known Bowtie implementation.",
             causes=[],
             hint_stmt=(
                 "Check Bowtie's supported list of implementations "
                 "to ensure you have the name correct. "
                 "If you are developing a new harness, ensure you have "
                 "built and tagged it properly."
             ),
@@ -207,15 +207,15 @@
     """
 
     contents: str
 
 
 @frozen
 class StartupFailed(Exception):
-    name: str
+    id: ConnectableId
     stderr: str = ""
     data: Any = None
 
     def __rich_console__(
         self,
         console: Console,
         options: ConsoleOptions,
@@ -237,30 +237,26 @@
                 "if you are not, this is a bug in Bowtie's harness for this "
                 "implementation! File an issue on Bowtie's issue tracker."
             )
             causes.extend(str(error) for error in errors)
 
         yield DiagnosticError(
             code="startup-failed",
-            message=f"{self.name!r} failed to start.",
+            message=f"{self.id!r} failed to start.",
             causes=causes,
             hint_stmt=hint,
         )
         if self.stderr:
             yield Panel(self.stderr, title="stderr")
 
 
 R = TypeVar("R")
 
 
-class MakeValidator(Protocol):
-    def __call__(
-        self,
-        *more_schemas: SchemaResource,
-    ) -> Callable[..., None]: ...
+MakeValidator = Callable[[], Callable[[Any, Schema], None]]
 
 
 @frozen
 class Link:
     description: str
     url: URL
 
@@ -272,16 +268,14 @@
         return dict(description=self.description, url=str(self.url))
 
 
 @frozen(order=True)
 class ImplementationInfo:
     # FIXME: Combine with / separate out more from `Implementation`
 
-    _image: ImplementationId = field(alias="image")
-
     name: str
     language: str
     homepage: URL
     issues: URL
     source: URL
     dialects: frozenset[Dialect]
 
@@ -307,33 +301,37 @@
             issues=URL.parse(issues),
             source=URL.parse(source),
             dialects=frozenset(Dialect.from_str(each) for each in dialects),
             links=[Link.from_dict(**each) for each in links],
             **kwargs,
         )
 
-    @property
-    def id(self):
-        return self._image
-
     def serializable(self):
-        as_dict = {
-            k: v
-            for k, v in asdict(self, recurse=False).items()
-            if not k.startswith("_") and v
+        return {
+            **{
+                k: (
+                    str(v)
+                    if k
+                    in {
+                        "homepage",
+                        "issues",
+                        "source",
+                        "documentation",
+                    }
+                    else v
+                )
+                for k, v in asdict(self, recurse=False).items()
+                if v
+            },
+            "dialects": sorted(
+                (str(dialect.uri) for dialect in self.dialects),
+                reverse=True,
+            ),
+            "links": [link.serializable() for link in self.links],
         }
-        dialects = (str(dialect.uri) for dialect in as_dict["dialects"])
-        as_dict.update(
-            homepage=str(as_dict["homepage"]),
-            issues=str(as_dict["issues"]),
-            source=str(as_dict["source"]),
-            dialects=sorted(dialects, reverse=True),
-            links=[link.serializable() for link in self.links],
-        )
-        return as_dict
 
 
 class Connection(Protocol):
     """
     A connection to a specific JSON Schema implementation.
 
     Concrete implementations of this protocol will decide what means of
@@ -360,45 +358,33 @@
     """
     A client which speaks to a specific running implementation harness.
     """
 
     _connection: Connection = field(alias="connection")
 
     _make_validator: MakeValidator = field(alias="make_validator")
-    _resources_for_validation: Sequence[SchemaResource] = field(
-        default=(),
-        alias="resources_for_validation",
-    )
 
     # FIXME: Remove this somehow by making the state machine even more explicit
     #: A sequence of commands to replay if we end up restarting the connection.
     _if_replaying: Sequence[Command[Any]] = ()
 
     async def _get_back_up_to_date(self):
         for each in self._if_replaying:
             await self.request(each)  # TODO: response assert?
 
-    async def transition(
-        self,
-        cmd: Command[R],
-        resources: Sequence[SchemaResource] = (),
-    ) -> tuple[Self, R | None]:
+    async def transition(self, cmd: Command[R]) -> tuple[Self, R | None]:
         response = await self.request(cmd)
-        harness = evolve(
-            self,
-            if_replaying=[*self._if_replaying, cmd],
-            resources_for_validation=resources,
-        )
+        harness = evolve(self, if_replaying=[*self._if_replaying, cmd])
         return harness, response
 
     async def request(self, cmd: Command[R]) -> R | None:
         """
         Send a given command to the implementation and return its response.
         """
-        validate = self._make_validator(*self._resources_for_validation)
+        validate = self._make_validator()
         request = cmd.to_request(validate=validate)
         try:
             response = await self._connection.request(request)
         except Restarted:
             await self._get_back_up_to_date()
             # FIXME: Probably handle infinitely restarting harnesses
             response = await self._connection.request(request)
@@ -413,30 +399,29 @@
 @frozen
 class DialectRunner:
     """
     A running implementation which is speaking a specific dialect.
     """
 
     dialect: Dialect
-    implementation: ImplementationId
+    implementation: ConnectableId
     _harness: HarnessClient = field(repr=False, alias="harness")
 
     @classmethod
     async def for_dialect(
         cls,
         dialect: Dialect,
-        implementation: ImplementationId,
+        implementation: ConnectableId,
         harness: HarnessClient,
         reporter: Reporter,
     ):
         new_harness: HarnessClient
         response: StartedDialect
         new_harness, response = await harness.transition(
             DialectCommand(dialect=str(dialect.uri)),  # type: ignore[reportArgumentType]
-            resources=[dialect.current_dialect_resource()],
         )
 
         if response != StartedDialect.OK:
             reporter.unacknowledged_dialect(
                 implementation=implementation,
                 dialect=dialect,
                 response=response,
@@ -482,61 +467,54 @@
 
 @mutable
 class Implementation:
     """
     A running implementation under test.
     """
 
+    id: ConnectableId
     info: ImplementationInfo
     _harness: HarnessClient = field(repr=False, alias="harness")
     _reporter: Reporter = field(alias="reporter")
 
     @classmethod
-    def known(cls) -> Set[str]:
-        # TODO: Possibly this should return running instances.
-        #       For now it just returns image names clearly.
+    def known(cls) -> Set[ConnectableId]:
         data = files("bowtie") / "data"
         if data.is_dir():
             path = data / "known_implementations.json"
             known = json.loads(path.read_text())
         else:
             root = Path(__file__).parent.parent
             dir = root.joinpath("implementations").iterdir()
             known = (d.name for d in dir if not d.name.startswith("."))
         return frozenset(known)
 
     @classmethod
     @asynccontextmanager
     async def start(
         cls,
-        id: ImplementationId,
+        id: ConnectableId,
         reporter: Reporter,
         **kwargs: Any,
     ) -> AsyncIterator[Self]:
         _harness = HarnessClient(**kwargs)
 
         try:
             harness, started = await _harness.transition(START_V1)  # type: ignore[reportArgumentType]
         except ProtocolError as err:
-            raise StartupFailed(name=id) from err
+            raise StartupFailed(id=id) from err
         except GotStderr as err:
-            raise StartupFailed(name=id, stderr=err.stderr.decode()) from err
+            raise StartupFailed(id=id, stderr=err.stderr.decode()) from err
         else:
             if started is None:
-                raise StartupFailed(name=id)
-
-        info = ImplementationInfo.from_dict(image=id, **started.implementation)  # type: ignore[reportUnknownArgumentType]
+                raise StartupFailed(id=id)
 
-        yield cls(harness=harness, info=info, reporter=reporter)
+        info = ImplementationInfo.from_dict(**started.implementation)  # type: ignore[reportUnknownArgumentType]
 
-        await _harness.poison()
-
-    @property
-    def name(self):
-        return self.info.id
+        yield cls(harness=harness, id=id, info=info, reporter=reporter)
 
     def supports(self, *dialects: Dialect) -> bool:
         """
         Does the implementation support (all of) the given dialect(s)?
         """
         return self.info.dialects.issuperset(dialects)
 
@@ -555,15 +533,15 @@
             yield case, await seq_case.run(runner=runner)
 
     async def start_speaking(self, dialect: Dialect) -> DialectRunner:
         if not self.supports(dialect):
             raise UnsupportedDialect(implementation=self, dialect=dialect)
         try:
             return await DialectRunner.for_dialect(
-                implementation=self.name,
+                implementation=self.id,
                 dialect=dialect,
                 harness=self._harness,
                 reporter=self._reporter,
             )
         except GotStderr as error:
             # the implementation failed on the dialect request.
             # there's likely no reason to continue, so we throw an exception
@@ -764,18 +742,11 @@
             }
             for test in serializable.pop("tests")
         ]
         return serializable
 
 
 @cache
-def validator_registry() -> ValidatorRegistry:
+def validator_registry():
     resources = referencing_loaders.from_traversable(files("bowtie.schemas"))
     registry = EMPTY_REGISTRY.with_resources(resources).crawl()
-
-    from referencing.jsonschema import DRAFT202012  # XXX
-
-    ignore_current_dialect = registry.with_resource(
-        uri="tag:bowtie.report,2023:ihop:__dialect__",
-        resource=DRAFT202012.create_resource({}),
-    )
-    return ValidatorRegistry.jsonschema(registry=ignore_current_dialect)
+    return ValidatorRegistry.jsonschema(registry=registry)
```

### Comparing `bowtie_json_schema-2024.5.9/bowtie/_registry.py` & `bowtie_json_schema-2024.6.1/bowtie/_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,108 +1,117 @@
 """
 Validator registries, likely for eventual upstreaming into referencing.
 """
 
 from __future__ import annotations
 
 from collections.abc import Callable, Iterable
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Generic, TypeVar
 
 from attrs import evolve, field, frozen
-from referencing.jsonschema import EMPTY_REGISTRY
+from referencing.jsonschema import EMPTY_REGISTRY, Schema, SchemaRegistry
 
 if TYPE_CHECKING:
-    from referencing.jsonschema import Schema, SchemaRegistry, SchemaResource
+    from jsonschema.exceptions import ValidationError
+    from referencing.jsonschema import SchemaResource
 
 
-ErrorsFor = Callable[[Any], Iterable[Exception]]
+E_co = TypeVar("E_co", bound=Exception, covariant=True)
+ErrorsFor = Callable[[Any], Iterable[E_co]]
+SchemaCompiler = Callable[
+    [Schema, SchemaRegistry],
+    Callable[[Any], ErrorsFor[E_co]],
+]
 
 
 class UnexpectedlyValid(Exception):
     """
     An instance which was expected to be invalid just isn't.
     """
 
 
 @frozen
-class Validator:
+class Validator(Generic[E_co]):
     """
     A compiled schema, ready to validate instances.
     """
 
-    errors_for: ErrorsFor
-    _raises: tuple[type[Exception], ...] = field(alias="raises")
-    _registry: ValidatorRegistry = field(alias="registry")
+    errors_for: ErrorsFor[E_co]
+    _raises: tuple[type[E_co], ...] = field(alias="raises")
+    _registry: ValidatorRegistry[E_co] = field(alias="registry")
 
     def __rmatmul__(
         self,
         resources: SchemaResource | Iterable[SchemaResource],
-    ) -> Validator:
+    ) -> Validator[E_co]:
         return evolve(self, registry=resources @ self._registry)
 
     def validate(self, instance: Any):
         exception = next(iter(self.errors_for(instance)), None)
         if exception is not None:
             raise exception
 
     def invalidate(self, instance: Any):
         exception = next(iter(self.errors_for(instance)), None)
         if not isinstance(exception, self._raises):
             raise UnexpectedlyValid(instance)
 
 
 @frozen
-class ValidatorRegistry:
+class ValidatorRegistry(Generic[E_co]):
 
-    _compile: Callable[[Schema, SchemaRegistry], ErrorsFor] = field(
+    _compile: Callable[[Schema, SchemaRegistry], ErrorsFor[E_co]] = field(
         alias="compile",
     )
-    _raises: tuple[type[Exception], ...] = field(
+    _raises: tuple[type[E_co], ...] = field(  # type: ignore[reportAssignmentType]  ?!?
         default=(Exception,),
         alias="raises",
     )
     _registry: SchemaRegistry = field(default=EMPTY_REGISTRY, alias="registry")
 
     def __rmatmul__(
         self,
         resources: SchemaResource | Iterable[SchemaResource],
-    ) -> ValidatorRegistry:
+    ) -> ValidatorRegistry[E_co]:
         return evolve(self, registry=resources @ self._registry)
 
     @classmethod
-    def jsonschema(cls, **kwargs: Any) -> ValidatorRegistry:
+    def jsonschema(cls, **kwargs: Any) -> ValidatorRegistry[ValidationError]:
         """
         A registry which uses the `jsonschema` module to do validation.
         """
         from jsonschema.exceptions import ValidationError
         from jsonschema.validators import (
             validator_for,  # type: ignore[reportUnknownVariableType]
         )
 
-        def compile(schema: Schema, registry: SchemaRegistry) -> ErrorsFor:
+        def compile(
+            schema: Schema,
+            registry: SchemaRegistry,
+        ) -> ErrorsFor[ValidationError]:
             _Validator = validator_for(schema)  # type: ignore[reportUnknownVariableType]
             return _Validator(schema, registry=registry).iter_errors  # type: ignore[reportUnknownVariableType]
 
-        return cls(compile=compile, raises=(ValidationError,), **kwargs)
+        return cls(compile=compile, raises=(ValidationError,), **kwargs)  # type: ignore[reportAssignmentType]  ?!?
 
     def schema(self, uri: str) -> Schema:
         """
         Return the schema identified by the given URI.
         """
         return self._registry.contents(uri)
 
-    def for_uri(self, uri: str) -> Validator:
+    def for_uri(self, uri: str) -> Validator[E_co]:
         """
         Return a `Validator` using the schema at the given URI.
         """
         return self.for_schema(self.schema(uri))
 
-    def for_schema(self, schema: Schema) -> Validator:
+    def for_schema(self, schema: Schema) -> Validator[E_co]:
         """
         Return a `Validator` using the given schema.
         """
-        errors_for: ErrorsFor = self._compile(schema, self._registry)
+        errors_for: ErrorsFor[E_co] = self._compile(schema, self._registry)
         return Validator(
             errors_for=errors_for,
             raises=self._raises,
             registry=self,
         )
```

### Comparing `bowtie_json_schema-2024.5.9/bowtie/_report.py` & `bowtie_json_schema-2024.6.1/bowtie/_report.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,18 +17,19 @@
     SeqResult,
     StartedDialect,
     Unsuccessful,
 )
 from bowtie._core import Dialect, TestCase, validator_registry
 
 if TYPE_CHECKING:
-    from collections.abc import Callable, Iterable, Mapping, Sequence
+    from collections.abc import Callable, Iterable, Mapping
     from typing import Any, Literal, Self, TextIO
 
-    from bowtie._commands import AnyTestResult, ImplementationId
+    from bowtie._commands import AnyTestResult
+    from bowtie._connectables import ConnectableId
     from bowtie._core import Example, ImplementationInfo, Test
 
 
 class InvalidReport(Exception):
     """
     The report is invalid.
     """
@@ -110,15 +111,15 @@
 
         return got_result
 
 
 @frozen
 class RunMetadata:
     dialect: Dialect
-    implementations: Sequence[ImplementationInfo] = field(
+    implementations: Mapping[ConnectableId, ImplementationInfo] = field(
         repr=lambda value: (
             f"({len(value)} implementation{'s' if len(value) != 1 else ''})"
         ),
         alias="implementations",
     )
     bowtie_version: str = field(
         default=importlib.metadata.version("bowtie-json-schema"),
@@ -142,33 +143,34 @@
     ) -> RunMetadata:
         from bowtie._core import ImplementationInfo
 
         if started is not None:
             kwargs["started"] = datetime.fromisoformat(started)
         return cls(
             dialect=Dialect.from_str(dialect),
-            implementations=[
-                ImplementationInfo.from_dict(image=image, **data)
-                for image, data in implementations.items()
-            ],
+            implementations={
+                id: ImplementationInfo.from_dict(**data)
+                for id, data in implementations.items()
+            },
             **kwargs,
         )
 
     def serializable(self):
         as_dict = asdict(
             self,
             filter=exclude("dialect"),
             recurse=False,
         )
         as_dict.update(
             dialect=self.dialect.serializable(),
             started=as_dict.pop("started").isoformat(),
             # FIXME: This transformation is to support the UI parsing
             implementations={
-                i.id: i.serializable() for i in self.implementations
+                id: implementation.serializable()
+                for id, implementation in self.implementations.items()
             },
         )
         return as_dict
 
 
 @frozen(eq=False)
 class Report:
@@ -181,15 +183,15 @@
 
     When comparing reports (e.g. for equality), only the relative order of
     test cases is considered, not the exact `Seq`\ s used in the run.
     """
 
     _cases: HashTrieMap[Seq, TestCase] = field(alias="cases", repr=False)
     _results: HashTrieMap[
-        ImplementationId,
+        ConnectableId,
         HashTrieMap[Seq, SeqResult],
     ] = field(
         repr=False,
         alias="results",
     )
     metadata: RunMetadata
     did_fail_fast: bool
@@ -227,21 +229,19 @@
         iterator = iter(input)
         header = next(iterator, None)
         if header is None:
             raise EmptyReport()
         validator.validate(header)
         metadata = RunMetadata.from_dict(**header)
 
-        validator = metadata.dialect.current_dialect_resource() @ validator
-
         results: HashTrieMap[
-            ImplementationId,
+            ConnectableId,
             HashTrieMap[Seq, SeqResult],
         ] = HashTrieMap.fromkeys(  # type: ignore[reportUnknownMemberType]
-            (each.id for each in metadata.implementations),
+            metadata.implementations,
             HashTrieMap(),
         )
         cases: HashTrieMap[Seq, TestCase] = HashTrieMap()
 
         for data in iterator:
             validator.validate(data)
             match data:
@@ -272,57 +272,66 @@
     @classmethod
     def from_serialized(cls, serialized: Iterable[str]) -> Self:
         return cls.from_input(json.loads(line) for line in serialized)
 
     @classmethod
     def empty(
         cls,
-        implementations: Sequence[ImplementationInfo] = (),
+        implementations: Mapping[ConnectableId, ImplementationInfo] = {},
         **kwargs: Any,
     ):
         """
         'The' empty report.
         """
         return cls(
             cases=HashTrieMap(),
             results=HashTrieMap(),
             metadata=RunMetadata(implementations=implementations, **kwargs),
             did_fail_fast=False,
         )
 
     @property
-    def implementations(self) -> Sequence[ImplementationInfo]:
+    def implementations(self) -> Mapping[ConnectableId, ImplementationInfo]:
         return self.metadata.implementations
 
     @property
     def is_empty(self):
         return not self._cases
 
     @property
     def total_tests(self):
         return sum(len(case.tests) for case in self._cases.values())
 
-    def unsuccessful(self, implementation: ImplementationId) -> Unsuccessful:
+    def compliance_by_implementation(self):
+        """
+        Return the fraction of passing tests for each reported implementation.
+        """
+        return {
+            id: 1 - (unsuccessful.total / self.total_tests)
+            for id, _, unsuccessful in self.worst_to_best()
+        }
+
+    def unsuccessful(self, implementation: ConnectableId) -> Unsuccessful:
         """
         A count of the unsuccessful tests for the given implementation.
         """
         results = self._results[implementation].values()
         return sum((each.unsuccessful() for each in results), Unsuccessful())
 
     def worst_to_best(self):
         """
         All implementations ordered by number of unsuccessful tests.
 
         Ties are then broken alphabetically.
         """
         unsuccessful = [
-            (implementation, self.unsuccessful(implementation.id))
-            for implementation in self.implementations
+            (id, implementation, self.unsuccessful(id))
+            for id, implementation in self.implementations.items()
         ]
-        unsuccessful.sort(key=lambda each: (each[1].total, each[0].name))
+        unsuccessful.sort(key=lambda each: (each[2].total, each[1].name))
         return unsuccessful
 
     def cases_with_results(
         self,
     ) -> Iterable[
         tuple[
             TestCase,
@@ -331,23 +340,23 @@
     ]:
         for seq, case in sorted(self._cases.items()):
             test_results: list[
                 tuple[Example | Test, Mapping[str, AnyTestResult]]
             ] = []
             for i, test in enumerate(case.tests):
                 test_result = {
-                    each.id: self._results[each.id][seq].result_for(i)
-                    for each in self.implementations
+                    id: self._results[id][seq].result_for(i)
+                    for id in self.implementations
                 }
                 test_results.append((test, test_result))
             yield case, test_results
 
     def compliance_badges(self) -> Iterable[tuple[ImplementationInfo, Badge]]:
-        for implementation in self.implementations:
-            unsuccessful = self.unsuccessful(implementation.id)
+        for id, implementation in self.implementations.items():
+            unsuccessful = self.unsuccessful(id)
             passed = self.total_tests - unsuccessful.total
             percentage = 100 * (passed / self.total_tests)
             r, g, b = 100 - int(percentage), int(percentage), 0
             yield implementation, Badge(
                 schemaVersion=1,
                 label=self.metadata.dialect.pretty_name,
                 message="%d%% Passing" % int(percentage),
```

### Comparing `bowtie_json_schema-2024.5.9/bowtie/_suite.py` & `bowtie_json_schema-2024.6.1/bowtie/_suite.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 
             gh = GitHub(token=os.environ.get("GITHUB_TOKEN", ""))
             org, repo_name, *rest = value.path_segments
             repo = gh.repository(org, repo_name)  # type: ignore[reportUnknownMemberType]
 
             path, ref = path_and_ref_from_gh_path(rest)
             data = BytesIO()
+            data.name = ""
             succeeded = repo.archive(format="zipball", path=data, ref=ref)  # type: ignore[reportUnknownMemberType]
             if not succeeded:
                 message = "Fetching the test suite from GitHub failed."
                 error = DiagnosticError(
                     code="suite-fetch-failed",
                     message=message,
                     causes=[
@@ -129,36 +130,29 @@
 
         return cases, dialect
 
 
 _P = Path | zipfile.Path
 
 
-class PathError(Exception):
-    pass
-
-
 def remotes_in(
     path: Path,
     dialect: _core.Dialect,
 ) -> Iterable[tuple[URL, Any]]:
     # This messy logic is because the test suite is terrible at indicating
     # what remotes are needed for what drafts, and mixes in schemas which
     # have no $schema and which are invalid under earlier versions, in with
     # other schemas which are needed for tests.
     #
     # FIXME: #40: for draft-next support
 
     for each in _rglob(path, "*.json"):
         schema = json.loads(each.read_text())
 
-        try:
-            relative = str(_relative_to(each, path)).replace("\\", "/")
-        except Exception as error:  # noqa: BLE001
-            raise PathError((each, path, error))
+        relative = str(_relative_to(each, path)).replace("\\", "/")
 
         if (
             ("$schema" in schema and schema["$schema"] != str(dialect.uri))
             or (  # draft<NotThisDialect>/*.json
                 relative.startswith("draft")
                 and not relative.startswith(dialect.short_name)
             )
```

### Comparing `bowtie_json_schema-2024.5.9/bowtie/exceptions.py` & `bowtie_json_schema-2024.6.1/bowtie/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         supports = ", ".join(
             each.pretty_name
             for each in sorted(self.implementation.info.dialects, reverse=True)
         )
         return DiagnosticWarning(
             code="unsupported-dialect",
             message=(
-                f"{self.implementation.name!r} does not "
+                f"{self.implementation.id!r} does not "
                 f"support {self.dialect.pretty_name}."
             ),
             causes=[],
             hint_stmt=None,
             note_stmt=f"its supported dialects are: {supports}\n",
         )
 
@@ -102,15 +102,15 @@
     dialect: Dialect
     stderr: bytes
 
     def __rich__(self):
         return DiagnosticError(
             code="dialect-error",
             message=(
-                f"{self.implementation.name!r} failed as we were beginning to "
+                f"{self.implementation.id!r} failed as we were beginning to "
                 f"send {self.dialect.pretty_name} tests."
             ),
             causes=[],
             hint_stmt=(
                 "The error may be transient, so you may want to try again. "
                 "If it does not appear to be, it may indicate a bug both in "
                 "the implementation as well as in Bowtie's test harness. "
```

### Comparing `bowtie_json_schema-2024.5.9/bowtie/hypothesis.py` & `bowtie_json_schema-2024.6.1/bowtie/hypothesis.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         max_leaves=3,
     ),
     max_size=5,
 )
 schemas = booleans() | object_schemas
 
 seqs = uuids().map(lambda uuid: uuid.hex)
+connectable_ids = text()
 implementation_names = pattern_from(
     "tag:bowtie.report,2024:models:implementation:name",
 )
 languages = pattern_from(
     "tag:bowtie.report,2024:models:implementation:language",
 )
 
@@ -105,15 +106,14 @@
 ):
     """
     Generate an implementation (info).
     """
     name = draw(names)
     language = draw(languages)
     return ImplementationInfo(
-        image=f"bowtie-hypothesis-generated/{language}/{name}",
         name=name,
         language=language,
         homepage=draw(urls().map(URL.parse)),
         issues=draw(urls().map(URL.parse)),
         source=draw(urls().map(URL.parse)),
         dialects=draw(dialects),
     )
@@ -123,19 +123,19 @@
     infos=implementation_infos(),
     min_size=1,
     max_size=5,
 ):
     """
     Generate (unique) collections of implementations.
     """
-    return lists(
+    return dictionaries(
+        connectable_ids,
         infos,
         min_size=min_size,
         max_size=max_size,
-        unique_by=lambda info: info.id,
     )
 
 
 def examples(
     description=text(),
     instance=integers(),  # FIXME: probably via hypothesis-jsonschema
     comment=text() | none(),
@@ -303,21 +303,21 @@
     )
     seq_cases = draw(strategy)
 
     return seq_cases, [
         draw(
             seq_results(
                 seqs=just(seq_case.seq),
-                implementations=just(implementation.id),
+                implementations=just(id),
                 min_tests=len(seq_case.case.tests),
                 max_tests=len(seq_case.case.tests),
             ),
         )
         for seq_case in seq_cases
-        for implementation in draw(responding(seq_case))
+        for id in draw(responding(seq_case))
     ]
 
 
 _cases_and_results = cases_and_results
 
 
 @composite
```

### Comparing `bowtie_json_schema-2024.5.9/bowtie/schemas/connectables.json` & `bowtie_json_schema-2024.6.1/bowtie/schemas/connectables.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9503968253968254%*

 * *Differences: {"'$defs'": "{'container': OrderedDict([('title', 'External Container'), ('description', 'An "*

 * *            "already running OCI container which Bowtie will connect to'), ('$anchor', "*

 * *            "'container'), ('pattern', '^container:*')]), 'direct': OrderedDict([('title', 'Direct "*

 * *            "Python Connection'), ('description', 'A directly importable (from Python) "*

 * *            "implementation which Bowtie will speak to'), ('$anchor', 'direct'), ('pattern', "*

 * *            "'^direct:[^.]*')])}",*

 * * "'oneOf […]*

```diff
@@ -1,9 +1,21 @@
 {
     "$defs": {
+        "container": {
+            "$anchor": "container",
+            "description": "An already running OCI container which Bowtie will connect to",
+            "pattern": "^container:*",
+            "title": "External Container"
+        },
+        "direct": {
+            "$anchor": "direct",
+            "description": "A directly importable (from Python) implementation which Bowtie will speak to",
+            "pattern": "^direct:[^.]*",
+            "title": "Direct Python Connection"
+        },
         "image": {
             "$anchor": "image",
             "description": "An OCI container image which Bowtie will spin up and manage",
             "pattern": "^image:*",
             "title": "Container Image"
         }
     },
@@ -20,14 +32,20 @@
             "title": "Implicit Image With Repository & Tag"
         },
         {
             "description": "A connectable with explicit connector.",
             "oneOf": [
                 {
                     "$ref": "#image"
+                },
+                {
+                    "$ref": "#container"
+                },
+                {
+                    "$ref": "#direct"
                 }
             ],
             "pattern": "^[^:]+:[^:]+(:[^:]+)?$",
             "title": "Fully Qualified Connectable"
         }
     ],
     "title": "Connectables",
```

### Comparing `bowtie_json_schema-2024.5.9/bowtie/schemas/report.json` & `bowtie_json_schema-2024.6.1/bowtie/schemas/report.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/bowtie/schemas/cli/info.json` & `bowtie_json_schema-2024.6.1/bowtie/schemas/cli/info.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/bowtie/schemas/cli/smoke.json` & `bowtie_json_schema-2024.6.1/bowtie/schemas/cli/smoke.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/bowtie/schemas/cli/summary.json` & `bowtie_json_schema-2024.6.1/bowtie/schemas/cli/summary.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/bowtie/schemas/io/v1.json` & `bowtie_json_schema-2024.6.1/bowtie/schemas/io/v1.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999479166666667%*

 * *Differences: {"'$defs'": '{\'case\': {\'properties\': {\'schema\': {\'$comment\': "We do no current validation '*

 * *            "here, as we may want to send schemas which truly aren't valid, but some day we likely "*

 * *            'will again.", delete: [\'$ref\']}}}}'}*

```diff
@@ -17,17 +17,16 @@
                     "description": "A collection of schemas (with URIs) which tests may reference (via $ref) and expect to be retrievable. They should be registered in whatever mechanism is expected by the implementation.",
                     "propertyNames": {
                         "format": "uri"
                     },
                     "type": "object"
                 },
                 "schema": {
-                    "$comment": "the URI used here is a sort of 'magic' URI set by Bowtie during runs, which will resolve to (effectively) the meta-schema for the current dialect being run by Bowtie. E.g. when running tests using the Draft 2020-12 dialect, the URI will resolve to the schema `{\"$ref\": \"https://json-schema.org/draft/2020-12/schema\"}`. This sort of dynamically set value is necessary, as schemas are supposed to be valid under the current dialect being spoken by Bowtie, but that's not known until runtime.",
+                    "$comment": "We do no current validation here, as we may want to send schemas which truly aren't valid, but some day we likely will again.",
                     "$id": "tag:bowtie.report,2024:ihop:schemaInCurrentDialect",
-                    "$ref": "tag:bowtie.report,2023:ihop:__dialect__",
                     "description": "A valid JSON Schema."
                 },
                 "tests": {
                     "description": "A set of related tests all using the same schema",
                     "items": {
                         "$ref": "tag:bowtie.report,2023:models:test"
                     },
```

### Comparing `bowtie_json_schema-2024.5.9/bowtie/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.6.1/bowtie/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/bowtie/schemas/io/commands/run.json` & `bowtie_json_schema-2024.6.1/bowtie/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/bowtie/schemas/io/commands/start.json` & `bowtie_json_schema-2024.6.1/bowtie/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/bowtie/schemas/models/dialect.json` & `bowtie_json_schema-2024.6.1/bowtie/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/bowtie/schemas/models/group.json` & `bowtie_json_schema-2024.6.1/bowtie/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/bowtie/schemas/models/implementation.json` & `bowtie_json_schema-2024.6.1/bowtie/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/bowtie/schemas/models/test.json` & `bowtie_json_schema-2024.6.1/bowtie/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/data/dialects.json` & `bowtie_json_schema-2024.6.1/data/dialects.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/docs/Makefile` & `bowtie_json_schema-2024.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/docs/conf.py` & `bowtie_json_schema-2024.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/docs/contributing.rst` & `bowtie_json_schema-2024.6.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/docs/github-actions.rst` & `bowtie_json_schema-2024.6.1/docs/github-actions.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/docs/implementers.rst` & `bowtie_json_schema-2024.6.1/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/docs/index.rst` & `bowtie_json_schema-2024.6.1/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -47,25 +47,14 @@
 
 Bowtie is available in a `tap <https://docs.brew.sh/Taps>`_ which is located :github:`here <bowtie-json-schema/homebrew-tap>`, and can be installed via:
 
 .. code:: sh
 
     brew install bowtie-json-schema/tap/bowtie
 
-As a Single Executable
-^^^^^^^^^^^^^^^^^^^^^^
-
-There is an experimental `PyApp <https://ofek.dev/pyapp/latest/>`_ of Bowtie published to GitHub on each release.
-
-You can find the :gh:`latest one here <releases/latest/>`.
-
-Once downloading it, run ``chmod +x`` on it and you should be able to use it as-is if you have an existing Python installation.
-
-If you use it (successfully or otherwise) please provide feedback.
-
 Manual Installation via PyPI
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Bowtie is written in Python, and uses a container runtime to execute JSON Schema implementations, so you'll need both Python and a suitable container runtime installed.
 
 If you have no previous container runtime installed (e.g. Docker), follow the `installation instructions for podman <https://podman.io/docs/installation>`_ specific to your operating system.
 Ensure you've started a Podman VM if you are on macOS.
```

### Comparing `bowtie_json_schema-2024.5.9/docs/motd.txt` & `bowtie_json_schema-2024.6.1/docs/motd.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/docs/requirements.txt` & `bowtie_json_schema-2024.6.1/docs/requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile --output-file docs/requirements.txt docs/requirements.in
+#    uv pip compile --output-file /Users/julian/Development/bowtie/docs/requirements.txt docs/requirements.in
 aiodocker==0.21.0
     # via bowtie-json-schema
 aiohttp==3.9.5
     # via aiodocker
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
+anyio==4.4.0
+    # via httpx
 attrs==23.2.0
     # via
     #   aiohttp
     #   bowtie-json-schema
     #   jsonschema
     #   referencing
 babel==2.15.0
     # via sphinx
 beautifulsoup4==4.12.3
     # via furo
-bowtie-json-schema @ file:.#egg=bowtie-json-schema
+file:.
+    # via -r docs/requirements.in
 certifi==2024.2.2
-    # via requests
+    # via
+    #   httpcore
+    #   httpx
+    #   requests
 cffi==1.16.0
     # via cryptography
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   rich-click
@@ -42,31 +48,40 @@
     #   sphinx-substitution-extensions
     #   sphinx-tabs
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
 furo==2024.5.6
+    # via -r docs/requirements.in
 github3-py==4.0.1
     # via bowtie-json-schema
+h11==0.14.0
+    # via httpcore
+httpcore==1.0.5
+    # via httpx
+httpx==0.27.0
+    # via bowtie-json-schema
 idna==3.7
     # via
+    #   anyio
+    #   httpx
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.4
     # via sphinx
 jsonschema==4.22.0
     # via bowtie-json-schema
 jsonschema-lexer==0.2.1
     # via bowtie-json-schema
 jsonschema-specifications==2023.12.1
     # via jsonschema
-lxml==5.2.1
+lxml==5.2.2
     # via sphinx-json-schema-spec
 markdown-it-py==3.0.0
     # via
     #   diagnostic
     #   rich
 markupsafe==2.1.5
     # via jinja2
@@ -88,90 +103,105 @@
     #   jsonschema-lexer
     #   pygments-github-lexers
     #   rich
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
 pygments-github-lexers==0.0.5
+    # via -r docs/requirements.in
 pyjwt==2.8.0
     # via github3-py
 python-dateutil==2.9.0.post0
     # via github3-py
 referencing==0.35.1
     # via
     #   bowtie-json-schema
     #   jsonschema
     #   jsonschema-specifications
     #   referencing-loaders
 referencing-loaders==2024.5.2
     # via bowtie-json-schema
-requests==2.31.0
+requests==2.32.3
     # via
     #   github3-py
     #   sphinx
 rich==13.7.1
     # via
     #   bowtie-json-schema
     #   diagnostic
     #   rich-click
-rich-click==1.8.1
+rich-click==1.8.2
     # via bowtie-json-schema
 rpds-py==0.18.1
     # via
     #   bowtie-json-schema
     #   jsonschema
     #   referencing
 six==1.16.0
     # via python-dateutil
+sniffio==1.3.1
+    # via
+    #   anyio
+    #   httpx
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
 sphinx==7.3.7
     # via
+    #   -r docs/requirements.in
     #   furo
     #   sphinx-basic-ng
     #   sphinx-click
     #   sphinx-copybutton
     #   sphinx-json-schema-spec
     #   sphinx-prompt
     #   sphinx-substitution-extensions
     #   sphinx-tabs
     #   sphinxcontrib-spelling
     #   sphinxext-opengraph
 sphinx-basic-ng==1.0.0b2
     # via furo
-sphinx-click==5.1.0
+sphinx-click==6.0.0
+    # via -r docs/requirements.in
 sphinx-copybutton==0.5.2
+    # via -r docs/requirements.in
 sphinx-json-schema-spec==2024.1.1
+    # via -r docs/requirements.in
 sphinx-prompt==1.8.0
     # via sphinx-substitution-extensions
 sphinx-substitution-extensions==2024.2.25
+    # via -r docs/requirements.in
 sphinx-tabs==3.4.5
+    # via -r docs/requirements.in
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
 sphinxcontrib-devhelp==1.0.6
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 sphinxcontrib-spelling==8.0.0
+    # via -r docs/requirements.in
 sphinxext-opengraph==0.9.1
-structlog==24.1.0
+    # via -r docs/requirements.in
+structlog==24.2.0
     # via bowtie-json-schema
-typing-extensions==4.11.0
+typing-extensions==4.12.0
     # via
     #   aiodocker
     #   rich-click
 uritemplate==4.1.1
     # via github3-py
 url-py==0.10.0
-    # via bowtie-json-schema
+    # via
+    #   -r docs/requirements.in
+    #   bowtie-json-schema
 urllib3==2.2.1
     # via requests
 yarl==1.9.4
     # via aiohttp
```

### Comparing `bowtie_json_schema-2024.5.9/docs/_static/bowtie_diagram_dark.svg` & `bowtie_json_schema-2024.6.1/docs/_static/bowtie_diagram_dark.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/docs/_static/bowtie_diagram_light.svg` & `bowtie_json_schema-2024.6.1/docs/_static/bowtie_diagram_light.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/docs/_static/logo.svg` & `bowtie_json_schema-2024.6.1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/package.json` & `bowtie_json_schema-2024.6.1/frontend/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.939327485380117%*

 * *Differences: {"'dependencies'": "{'react-router-dom': '^6.23.1'}",*

 * * "'devDependencies'": "{'@types/react': '^18.3.3', '@typescript-eslint/eslint-plugin': '^7.10.0', "*

 * *                      "'@typescript-eslint/parser': '^7.10.0', '@vitejs/plugin-react': '^4.3.0', "*

 * *                      "'jsdom': '^24.1.0', 'vite-bundle-visualizer': '^1.2.1'}",*

 * * "'packageManager'": "'pnpm@9.1.2'"}*

```diff
@@ -2,38 +2,38 @@
     "dependencies": {
         "bootstrap": "^5.3.3",
         "dayjs": "^1.11.11",
         "react": "^18.3.1",
         "react-bootstrap": "^2.10.2",
         "react-bootstrap-icons": "^1.11.4",
         "react-dom": "^18.3.1",
-        "react-router-dom": "^6.23.0",
+        "react-router-dom": "^6.23.1",
         "react-syntax-highlighter": "^15.5.0",
         "urijs": "^1.19.11"
     },
     "description": "The UI displays the outcomes generated by Bowtie, which serves as a meta-validator for the JSON Schema specification",
     "devDependencies": {
-        "@types/react": "^18.3.1",
+        "@types/react": "^18.3.3",
         "@types/react-dom": "^18.3.0",
         "@types/react-syntax-highlighter": "^15.5.13",
         "@types/react-test-renderer": "^18.3.0",
         "@types/urijs": "^1.19.25",
-        "@typescript-eslint/eslint-plugin": "^7.8.0",
-        "@typescript-eslint/parser": "^7.8.0",
-        "@vitejs/plugin-react": "^4.2.1",
+        "@typescript-eslint/eslint-plugin": "^7.10.0",
+        "@typescript-eslint/parser": "^7.10.0",
+        "@vitejs/plugin-react": "^4.3.0",
         "eslint": "8.57.0",
         "eslint-plugin-react": "7.34.1",
         "eslint-plugin-react-hooks": "4.6.2",
-        "jsdom": "^24.0.0",
+        "jsdom": "^24.1.0",
         "react-test-renderer": "^18.3.1",
         "ts-loader": "^9.5.1",
         "ts-node": "^10.9.2",
         "typescript": "^5.4.5",
         "vite": "^5.2.11",
-        "vite-bundle-visualizer": "^1.1.0",
+        "vite-bundle-visualizer": "^1.2.1",
         "vitest": "^1.6.0"
     },
     "engines": {
         "node": ">=21.0.0"
     },
     "eslintConfig": {
         "env": {
@@ -70,15 +70,15 @@
         "settings": {
             "react": {
                 "version": "18.2"
             }
         }
     },
     "name": "bowtie",
-    "packageManager": "pnpm@9.1.0",
+    "packageManager": "pnpm@9.1.2",
     "scripts": {
         "build": "tsc && vite build",
         "bundle-visualizer": "vite-bundle-visualizer",
         "lint": "eslint src --max-warnings 0",
         "preview": "vite preview",
         "start": "vite --no-clearScreen",
         "test": "vitest run",
```

### Comparing `bowtie_json_schema-2024.5.9/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2024.6.1/frontend/pnpm-lock.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -15,67 +15,67 @@
         specifier: ^1.11.11
         version: 1.11.11
       react:
         specifier: ^18.3.1
         version: 18.3.1
       react-bootstrap:
         specifier: ^2.10.2
-        version: 2.10.2(@types/react@18.3.1)(react-dom@18.3.1(react@18.3.1))(react@18.3.1)
+        version: 2.10.2(@types/react@18.3.3)(react-dom@18.3.1(react@18.3.1))(react@18.3.1)
       react-bootstrap-icons:
         specifier: ^1.11.4
         version: 1.11.4(react@18.3.1)
       react-dom:
         specifier: ^18.3.1
         version: 18.3.1(react@18.3.1)
       react-router-dom:
-        specifier: ^6.23.0
-        version: 6.23.0(react-dom@18.3.1(react@18.3.1))(react@18.3.1)
+        specifier: ^6.23.1
+        version: 6.23.1(react-dom@18.3.1(react@18.3.1))(react@18.3.1)
       react-syntax-highlighter:
         specifier: ^15.5.0
         version: 15.5.0(react@18.3.1)
       urijs:
         specifier: ^1.19.11
         version: 1.19.11
     devDependencies:
       '@types/react':
-        specifier: ^18.3.1
-        version: 18.3.1
+        specifier: ^18.3.3
+        version: 18.3.3
       '@types/react-dom':
         specifier: ^18.3.0
         version: 18.3.0
       '@types/react-syntax-highlighter':
         specifier: ^15.5.13
         version: 15.5.13
       '@types/react-test-renderer':
         specifier: ^18.3.0
         version: 18.3.0
       '@types/urijs':
         specifier: ^1.19.25
         version: 1.19.25
       '@typescript-eslint/eslint-plugin':
-        specifier: ^7.8.0
-        version: 7.8.0(@typescript-eslint/parser@7.8.0(eslint@8.57.0)(typescript@5.4.5))(eslint@8.57.0)(typescript@5.4.5)
+        specifier: ^7.10.0
+        version: 7.10.0(@typescript-eslint/parser@7.10.0(eslint@8.57.0)(typescript@5.4.5))(eslint@8.57.0)(typescript@5.4.5)
       '@typescript-eslint/parser':
-        specifier: ^7.8.0
-        version: 7.8.0(eslint@8.57.0)(typescript@5.4.5)
+        specifier: ^7.10.0
+        version: 7.10.0(eslint@8.57.0)(typescript@5.4.5)
       '@vitejs/plugin-react':
-        specifier: ^4.2.1
-        version: 4.2.1(vite@5.2.11(@types/node@20.11.5)(terser@5.27.0))
+        specifier: ^4.3.0
+        version: 4.3.0(vite@5.2.11(@types/node@20.11.5)(terser@5.27.0))
       eslint:
         specifier: 8.57.0
         version: 8.57.0
       eslint-plugin-react:
         specifier: 7.34.1
         version: 7.34.1(eslint@8.57.0)
       eslint-plugin-react-hooks:
         specifier: 4.6.2
         version: 4.6.2(eslint@8.57.0)
       jsdom:
-        specifier: ^24.0.0
-        version: 24.0.0
+        specifier: ^24.1.0
+        version: 24.1.0
       react-test-renderer:
         specifier: ^18.3.1
         version: 18.3.1(react@18.3.1)
       ts-loader:
         specifier: ^9.5.1
         version: 9.5.1(typescript@5.4.5)(webpack@5.89.0)
       ts-node:
@@ -84,19 +84,19 @@
       typescript:
         specifier: ^5.4.5
         version: 5.4.5
       vite:
         specifier: ^5.2.11
         version: 5.2.11(@types/node@20.11.5)(terser@5.27.0)
       vite-bundle-visualizer:
-        specifier: ^1.1.0
-        version: 1.1.0(rollup@4.17.2)
+        specifier: ^1.2.1
+        version: 1.2.1(rollup@4.17.2)
       vitest:
         specifier: ^1.6.0
-        version: 1.6.0(@types/node@20.11.5)(jsdom@24.0.0)(terser@5.27.0)
+        version: 1.6.0(@types/node@20.11.5)(jsdom@24.1.0)(terser@5.27.0)
 
 packages:
 
   '@ampproject/remapping@2.3.0':
     resolution: {integrity: sha512-30iZtAPgz+LTIYoeivqYo853f02jBYSd5uGnGpkFV0M3xOt9aN73erkgYAmZU43x4VfqcnLxW9Kpg3R5LC4YYw==}
     engines: {node: '>=6.0.0'}
 
@@ -423,16 +423,16 @@
 
   '@react-aria/ssr@3.9.3':
     resolution: {integrity: sha512-5bUZ93dmvHFcmfUcEN7qzYe8yQQ8JY+nHN6m9/iSDCQ/QmCiE0kWXYwhurjw5ch6I8WokQzx66xKIMHBAa4NNA==}
     engines: {node: '>= 12'}
     peerDependencies:
       react: ^16.8.0 || ^17.0.0-rc.1 || ^18.0.0
 
-  '@remix-run/router@1.16.0':
-    resolution: {integrity: sha512-Quz1KOffeEf/zwkCBM3kBtH4ZoZ+pT3xIXBG4PPW/XFtDP7EGhtTiC2+gpL9GnR7+Qdet5Oa6cYSvwKYg6kN9Q==}
+  '@remix-run/router@1.16.1':
+    resolution: {integrity: sha512-es2g3dq6Nb07iFxGk5GuHN20RwBZOsuDQN7izWIisUcv9r+d2C5jQxqmgkdebXgReWfiyUabcki6Fg77mSNrig==}
     engines: {node: '>=14.0.0'}
 
   '@restart/hooks@0.4.16':
     resolution: {integrity: sha512-f7aCv7c+nU/3mF7NWLtVVr0Ra80RqsO89hO72r+Y/nvQr5+q0UFGkocElTH6MJApvReVh6JHUFYn2cw1WdHF3w==}
     peerDependencies:
       react: '>=16.8.0'
 
@@ -581,92 +581,89 @@
 
   '@types/react-test-renderer@18.3.0':
     resolution: {integrity: sha512-HW4MuEYxfDbOHQsVlY/XtOvNHftCVEPhJF2pQXXwcUiUF+Oyb0usgp48HSgpK5rt8m9KZb22yqOeZm+rrVG8gw==}
 
   '@types/react-transition-group@4.4.10':
     resolution: {integrity: sha512-hT/+s0VQs2ojCX823m60m5f0sL5idt9SO6Tj6Dg+rdphGPIeJbJ6CxvBYkgkGKrYeDjvIpKTR38UzmtHJOGW3Q==}
 
-  '@types/react@18.3.1':
-    resolution: {integrity: sha512-V0kuGBX3+prX+DQ/7r2qsv1NsdfnCLnTgnRJ1pYnxykBhGMz+qj+box5lq7XsO5mtZsBqpjwwTu/7wszPfMBcw==}
-
-  '@types/semver@7.5.8':
-    resolution: {integrity: sha512-I8EUhyrgfLrcTkzV3TSsGyl1tSuPrEDzr0yd5m90UgNxQkyDXULk3b6MlQqTCpZpNtWe1K0hzclnZkTcLBe2UQ==}
+  '@types/react@18.3.3':
+    resolution: {integrity: sha512-hti/R0pS0q1/xx+TsI73XIqk26eBsISZ2R0wUijXIngRK9R/e7Xw/cXVxQK7R5JjW+SV4zGcn5hXjudkN/pLIw==}
 
   '@types/unist@2.0.10':
     resolution: {integrity: sha512-IfYcSBWE3hLpBg8+X2SEa8LVkJdJEkT2Ese2aaLs3ptGdVtABxndrMaxuFlQ1qdFf9Q5rDvDpxI3WwgvKFAsQA==}
 
   '@types/urijs@1.19.25':
     resolution: {integrity: sha512-XOfUup9r3Y06nFAZh3WvO0rBU4OtlfPB/vgxpjg+NRdGU6CN6djdc6OEiH+PcqHCY6eFLo9Ista73uarf4gnBg==}
 
   '@types/warning@3.0.3':
     resolution: {integrity: sha512-D1XC7WK8K+zZEveUPY+cf4+kgauk8N4eHr/XIHXGlGYkHLud6hK9lYfZk1ry1TNh798cZUCgb6MqGEG8DkJt6Q==}
 
-  '@typescript-eslint/eslint-plugin@7.8.0':
-    resolution: {integrity: sha512-gFTT+ezJmkwutUPmB0skOj3GZJtlEGnlssems4AjkVweUPGj7jRwwqg0Hhg7++kPGJqKtTYx+R05Ftww372aIg==}
+  '@typescript-eslint/eslint-plugin@7.10.0':
+    resolution: {integrity: sha512-PzCr+a/KAef5ZawX7nbyNwBDtM1HdLIT53aSA2DDlxmxMngZ43O8SIePOeX8H5S+FHXeI6t97mTt/dDdzY4Fyw==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       '@typescript-eslint/parser': ^7.0.0
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
 
-  '@typescript-eslint/parser@7.8.0':
-    resolution: {integrity: sha512-KgKQly1pv0l4ltcftP59uQZCi4HUYswCLbTqVZEJu7uLX8CTLyswqMLqLN+2QFz4jCptqWVV4SB7vdxcH2+0kQ==}
+  '@typescript-eslint/parser@7.10.0':
+    resolution: {integrity: sha512-2EjZMA0LUW5V5tGQiaa2Gys+nKdfrn2xiTIBLR4fxmPmVSvgPcKNW+AE/ln9k0A4zDUti0J/GZXMDupQoI+e1w==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
 
-  '@typescript-eslint/scope-manager@7.8.0':
-    resolution: {integrity: sha512-viEmZ1LmwsGcnr85gIq+FCYI7nO90DVbE37/ll51hjv9aG+YZMb4WDE2fyWpUR4O/UrhGRpYXK/XajcGTk2B8g==}
+  '@typescript-eslint/scope-manager@7.10.0':
+    resolution: {integrity: sha512-7L01/K8W/VGl7noe2mgH0K7BE29Sq6KAbVmxurj8GGaPDZXPr8EEQ2seOeAS+mEV9DnzxBQB6ax6qQQ5C6P4xg==}
     engines: {node: ^18.18.0 || >=20.0.0}
 
-  '@typescript-eslint/type-utils@7.8.0':
-    resolution: {integrity: sha512-H70R3AefQDQpz9mGv13Uhi121FNMh+WEaRqcXTX09YEDky21km4dV1ZXJIp8QjXc4ZaVkXVdohvWDzbnbHDS+A==}
+  '@typescript-eslint/type-utils@7.10.0':
+    resolution: {integrity: sha512-D7tS4WDkJWrVkuzgm90qYw9RdgBcrWmbbRkrLA4d7Pg3w0ttVGDsvYGV19SH8gPR5L7OtcN5J1hTtyenO9xE9g==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
 
-  '@typescript-eslint/types@7.8.0':
-    resolution: {integrity: sha512-wf0peJ+ZGlcH+2ZS23aJbOv+ztjeeP8uQ9GgwMJGVLx/Nj9CJt17GWgWWoSmoRVKAX2X+7fzEnAjxdvK2gqCLw==}
+  '@typescript-eslint/types@7.10.0':
+    resolution: {integrity: sha512-7fNj+Ya35aNyhuqrA1E/VayQX9Elwr8NKZ4WueClR3KwJ7Xx9jcCdOrLW04h51de/+gNbyFMs+IDxh5xIwfbNg==}
     engines: {node: ^18.18.0 || >=20.0.0}
 
-  '@typescript-eslint/typescript-estree@7.8.0':
-    resolution: {integrity: sha512-5pfUCOwK5yjPaJQNy44prjCwtr981dO8Qo9J9PwYXZ0MosgAbfEMB008dJ5sNo3+/BN6ytBPuSvXUg9SAqB0dg==}
+  '@typescript-eslint/typescript-estree@7.10.0':
+    resolution: {integrity: sha512-LXFnQJjL9XIcxeVfqmNj60YhatpRLt6UhdlFwAkjNc6jSUlK8zQOl1oktAP8PlWFzPQC1jny/8Bai3/HPuvN5g==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
 
-  '@typescript-eslint/utils@7.8.0':
-    resolution: {integrity: sha512-L0yFqOCflVqXxiZyXrDr80lnahQfSOfc9ELAAZ75sqicqp2i36kEZZGuUymHNFoYOqxRT05up760b4iGsl02nQ==}
+  '@typescript-eslint/utils@7.10.0':
+    resolution: {integrity: sha512-olzif1Fuo8R8m/qKkzJqT7qwy16CzPRWBvERS0uvyc+DHd8AKbO4Jb7kpAvVzMmZm8TrHnI7hvjN4I05zow+tg==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       eslint: ^8.56.0
 
-  '@typescript-eslint/visitor-keys@7.8.0':
-    resolution: {integrity: sha512-q4/gibTNBQNA0lGyYQCmWRS5D15n8rXh4QjK3KV+MBPlTYHpfBUT3D3PaPR/HeNiI9W6R7FvlkcGhNyAoP+caA==}
+  '@typescript-eslint/visitor-keys@7.10.0':
+    resolution: {integrity: sha512-9ntIVgsi6gg6FIq9xjEO4VQJvwOqA3jaBFQJ/6TK5AvEup2+cECI6Fh7QiBxmfMHXU0V0J4RyPeOU1VDNzl9cg==}
     engines: {node: ^18.18.0 || >=20.0.0}
 
   '@ungap/structured-clone@1.2.0':
     resolution: {integrity: sha512-zuVdFrMJiuCDQUMCzQaD6KL28MjnqqN8XnAqiEq9PNm/hCPTSGfrXCOfwj1ow4LFb/tNymJPwsNbVePc1xFqrQ==}
 
-  '@vitejs/plugin-react@4.2.1':
-    resolution: {integrity: sha512-oojO9IDc4nCUUi8qIR11KoQm0XFFLIwsRBwHRR4d/88IWghn1y6ckz/bJ8GHDCsYEJee8mDzqtJxh15/cisJNQ==}
+  '@vitejs/plugin-react@4.3.0':
+    resolution: {integrity: sha512-KcEbMsn4Dpk+LIbHMj7gDPRKaTMStxxWRkRmxsg/jVdFdJCZWt1SchZcf0M4t8lIKdwwMsEyzhrcOXRrDPtOBw==}
     engines: {node: ^14.18.0 || >=16.0.0}
     peerDependencies:
       vite: ^4.2.0 || ^5.0.0
 
   '@vitest/expect@1.6.0':
     resolution: {integrity: sha512-ixEvFVQjycy/oNgHjqsL6AZCDduC+tflRluaHIzKIsdbzkLn2U/iBnVeJwB6HsIjQBdfMR8Z0tRxKUsvFJEeWQ==}
 
@@ -1261,14 +1258,15 @@
     engines: {node: '>=10.13.0'}
 
   glob-to-regexp@0.4.1:
     resolution: {integrity: sha512-lkX1HJXwyMcprw/5YUZc2s7DrpAiHB21/V+E1rHUrVNokkvB6bqMzT0VfV6/86ZNabt1k14YOIaT7nDvOX3Iiw==}
 
   glob@7.2.3:
     resolution: {integrity: sha512-nFR0zLpU2YCaRxwoCJvL6UvCH2JFyFVIvwTLsIf21AuHlMskA1hhTdk+LlYJtOlYt9v6dvszD2BGRqBL+iQK9Q==}
+    deprecated: Glob versions prior to v9 are no longer supported
 
   globals@11.12.0:
     resolution: {integrity: sha512-WOBp/EEGUiIsJSp7wcv/y6MO+lV9UoncWqxuFfm8eBwzWNgyfBd6Gz+IeKQ9jCmyhoH99g15M3T+QaVHFjizVA==}
     engines: {node: '>=4'}
 
   globals@13.24.0:
     resolution: {integrity: sha512-AhO5QUcj8llrbG09iWhPU2B204J1xnPeL8kQmVorSsy+Sjj1sk8gIyh6cUocGmH4L0UuhAJy+hJMRA4mgA4mFQ==}
@@ -1367,14 +1365,15 @@
 
   imurmurhash@0.1.4:
     resolution: {integrity: sha512-JmXMZ6wuvDmLiHEml9ykzqO6lwFbof0GG4IkcGaENdCRDDmMVnny7s5HsIgHCbaq0w2MyPhDqkhTUgS2LU2PHA==}
     engines: {node: '>=0.8.19'}
 
   inflight@1.0.6:
     resolution: {integrity: sha512-k92I/b08q4wvFscXCLvqfsHCrjrF7yiXsQuIVvVE7N82W3+aqpzuUdBbfhWcy/FZR3/4IgflMgKLOsvPDrGCJA==}
+    deprecated: This module is not supported, and leaks memory. Do not use it. Check out lru-cache if you want a good and tested way to coalesce async requests by a key value, which is much more comprehensive and powerful.
 
   inherits@2.0.4:
     resolution: {integrity: sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==}
 
   internal-slot@1.0.7:
     resolution: {integrity: sha512-NGnrKwXzSms2qUUih/ILZ5JBqNTSa1+ZmP6flaIp6KmSElgE9qdndzS3cqjrDovwFdmwsGsLdeFgB6suw+1e9g==}
     engines: {node: '>= 0.4'}
@@ -1533,16 +1532,16 @@
   js-tokens@9.0.0:
     resolution: {integrity: sha512-WriZw1luRMlmV3LGJaR6QOJjWwgLUTf89OwT2lUOyjX2dJGBwgmIkbcz+7WFZjrZM635JOIR517++e/67CP9dQ==}
 
   js-yaml@4.1.0:
     resolution: {integrity: sha512-wpxZs9NoxZaJESJGIZTyDEaYpl0FKSA+FB9aJiyemKhMwkxQg63h4T1KJgUGHpTqPDNRcmmYLugrRjJlBtWvRA==}
     hasBin: true
 
-  jsdom@24.0.0:
-    resolution: {integrity: sha512-UDS2NayCvmXSXVP6mpTj+73JnNQadZlr9N68189xib2tx5Mls7swlTNao26IoHv46BZJFvXygyRtyXd1feAk1A==}
+  jsdom@24.1.0:
+    resolution: {integrity: sha512-6gpM7pRXCwIOKxX47cgOyvyQDN/Eh0f1MeKySBV2xGdKtqJBLj8P25eY3EVCWo2mglDDzozR2r2MW4T+JiNUZA==}
     engines: {node: '>=18'}
     peerDependencies:
       canvas: ^2.11.2
     peerDependenciesMeta:
       canvas:
         optional: true
 
@@ -1667,16 +1666,16 @@
   node-releases@2.0.14:
     resolution: {integrity: sha512-y10wOWt8yZpqXmOgRo77WaHEmhYQYGNA6y421PKsKYWEK8aW+cqAphborZDhqfyKrbZEN92CN1X2KbafY2s7Yw==}
 
   npm-run-path@5.3.0:
     resolution: {integrity: sha512-ppwTtiJZq0O/ai0z7yfudtBpWIoxM8yE6nHi1X47eFR2EWORqfbu6CnPlNsjeN683eT0qG6H/Pyf9fCcvjnnnQ==}
     engines: {node: ^12.20.0 || ^14.13.1 || >=16.0.0}
 
-  nwsapi@2.2.9:
-    resolution: {integrity: sha512-2f3F0SEEer8bBu0dsNCFF50N0cTThV1nWFYcEYFZttdW0lDAoybv9cQoK7X7/68Z89S7FoRrVjP1LPX4XRf9vg==}
+  nwsapi@2.2.10:
+    resolution: {integrity: sha512-QK0sRs7MKv0tKe1+5uZIQk/C8XGza4DAnztJG8iD+TpJIORARrCxczA738awHrZoHeTjSSoHqao2teO0dC/gFQ==}
 
   object-assign@4.1.1:
     resolution: {integrity: sha512-rJgTQnkUnH1sFw8yT6VSU3zD3sWmu6sZhIseY8VX+GRu3P6F7Fu+JNDoXfklElbLJSnc3FUQHVe4cU5hj+BcUg==}
     engines: {node: '>=0.10.0'}
 
   object-inspect@1.13.1:
     resolution: {integrity: sha512-5qoj1RUiKOMsCCNLV1CBiPYE10sziTsnmNxkAI/rZhiD63CF7IqdFGC/XzjWjpSgLf0LxXX3bDFIh0E18f6UhQ==}
@@ -1861,23 +1860,23 @@
   react-lifecycles-compat@3.0.4:
     resolution: {integrity: sha512-fBASbA6LnOU9dOU2eW7aQ8xmYBSXUIWr+UmF9b1efZBazGNO+rcXT/icdKnYm2pTwcRylVUYwW7H1PHfLekVzA==}
 
   react-refresh@0.14.2:
     resolution: {integrity: sha512-jCvmsr+1IUSMUyzOkRcvnVbX3ZYC6g9TDrDbFuFmRDq7PD4yaGbLKNQL6k2jnArV8hjYxh7hVhAZB6s9HDGpZA==}
     engines: {node: '>=0.10.0'}
 
-  react-router-dom@6.23.0:
-    resolution: {integrity: sha512-Q9YaSYvubwgbal2c9DJKfx6hTNoBp3iJDsl+Duva/DwxoJH+OTXkxGpql4iUK2sla/8z4RpjAm6EWx1qUDuopQ==}
+  react-router-dom@6.23.1:
+    resolution: {integrity: sha512-utP+K+aSTtEdbWpC+4gxhdlPFwuEfDKq8ZrPFU65bbRJY+l706qjR7yaidBpo3MSeA/fzwbXWbKBI6ftOnP3OQ==}
     engines: {node: '>=14.0.0'}
     peerDependencies:
       react: '>=16.8'
       react-dom: '>=16.8'
 
-  react-router@6.23.0:
-    resolution: {integrity: sha512-wPMZ8S2TuPadH0sF5irFGjkNLIcRvOSaEe7v+JER8508dyJumm6XZB1u5kztlX0RVq6AzRVndzqcUh6sFIauzA==}
+  react-router@6.23.1:
+    resolution: {integrity: sha512-fzcOaRF69uvqbbM7OhvQyBTFDVrrGlsFdS3AL+1KfIBtGETibHzi3FkoTRyiDJnWNc2VxrfvR+657ROHjaNjqQ==}
     engines: {node: '>=14.0.0'}
     peerDependencies:
       react: '>=16.8'
 
   react-shallow-renderer@16.15.0:
     resolution: {integrity: sha512-oScf2FqQ9LFVQgA73vr86xl2NaOIX73rh+YFqcOp68CWj56tSfgtGKrEbyhCj0rSijyG9M1CYprTh39fBi5hzA==}
     peerDependencies:
@@ -1934,14 +1933,15 @@
 
   reusify@1.0.4:
     resolution: {integrity: sha512-U9nH88a3fc/ekCF1l0/UP1IosiuIjyTh7hBvXVMHYgVcfGvt897Xguj2UOLDeI5BG2m7/uwyaLVT6fbtCwTyzw==}
     engines: {iojs: '>=1.0.0', node: '>=0.10.0'}
 
   rimraf@3.0.2:
     resolution: {integrity: sha512-JZkJMZkAGFFPP2YqXZXPbMlMBgsxzE8ILs4lMIX/2o0L9UBw9O/Y3o6wFw/i9YLapcUJWwqbi3kdxIPdC62TIA==}
+    deprecated: Rimraf versions prior to v4 are no longer supported
     hasBin: true
 
   rollup-plugin-visualizer@5.12.0:
     resolution: {integrity: sha512-8/NU9jXcHRs7Nnj07PF2o4gjxmm9lXIrZ8r175bT9dK8qoLlvKTwRMArRCMgpMGlq8CTLugRvEmyMeMXIU2pNQ==}
     engines: {node: '>=14'}
     hasBin: true
     peerDependencies:
@@ -1954,14 +1954,17 @@
     resolution: {integrity: sha512-/9ClTJPByC0U4zNLowV1tMBe8yMEAxewtR3cUNX5BoEpGH3dQEWpJLr6CLp0fPdYRF/fzVOgvDb1zXuakwF5kQ==}
     engines: {node: '>=18.0.0', npm: '>=8.0.0'}
     hasBin: true
 
   rrweb-cssom@0.6.0:
     resolution: {integrity: sha512-APM0Gt1KoXBz0iIkkdB/kfvGOwC4UuJFeG/c+yV7wSc7q96cG/kJ0HiYCnzivD9SB53cLV1MlHFNfOuPaadYSw==}
 
+  rrweb-cssom@0.7.0:
+    resolution: {integrity: sha512-KlSv0pm9kgQSRxXEMgtivPJ4h826YHsuob8pSHcfSZsSXGtvpEAie8S0AnXuObEJ7nhikOb4ahwxDm0H2yW17g==}
+
   run-parallel@1.2.0:
     resolution: {integrity: sha512-5l4VyZR86LZ/lDxZTR6jqL8AFE2S0IFLMP26AbjsLVADxHdhB/c0GUsH+y39UfCi3dzz8OlQuPmnaJOMoDHQBA==}
 
   safe-array-concat@1.1.2:
     resolution: {integrity: sha512-vj6RsCsWBCf19jIeHEfkRMw8DPiBb+DMXklQ/1SGDHOMlHdPUkZXFQ2YdplS23zESTijAcurb1aSgJA3AgMu1Q==}
     engines: {node: '>=0.4'}
 
@@ -2265,16 +2268,16 @@
 
   url-parse@1.5.10:
     resolution: {integrity: sha512-WypcfiRhfeUP9vvF0j6rw0J3hrWrw6iZv3+22h6iRMJ/8z1Tj6XfLP4DsUix5MhMPnXpiHDoKyoZ/bdCkwBCiQ==}
 
   v8-compile-cache-lib@3.0.1:
     resolution: {integrity: sha512-wa7YjyUGfNZngI/vtK0UHAN+lgDCxBPCylVXGp0zu59Fz5aiGtNXaq3DhIov063MorB+VfufLh3JlF2KdTK3xg==}
 
-  vite-bundle-visualizer@1.1.0:
-    resolution: {integrity: sha512-cmi5OuS7Eta5keTJmCTEbBBA7gOsUQ4K44W5dbsP+n/X0GIilIIFbJeXF120MQpTxdiZ/GIx4A9zkPEcKpPAog==}
+  vite-bundle-visualizer@1.2.1:
+    resolution: {integrity: sha512-cwz/Pg6+95YbgIDp+RPwEToc4TKxfsFWSG/tsl2DSZd9YZicUag1tQXjJ5xcL7ydvEoaC2FOZeaXOU60t9BRXw==}
     engines: {node: ^18.19.0 || >=20.6.0}
     hasBin: true
 
   vite-node@1.6.0:
     resolution: {integrity: sha512-de6HJgzC+TFzOu0NTC4RAIsyf/DY/ibWDYQUcuEA84EMHhcefTUGkjFHKKEJhQN4A+6I0u++kr3l36ZF2d7XRw==}
     engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
@@ -2765,15 +2768,15 @@
   '@popperjs/core@2.11.8': {}
 
   '@react-aria/ssr@3.9.3(react@18.3.1)':
     dependencies:
       '@swc/helpers': 0.5.11
       react: 18.3.1
 
-  '@remix-run/router@1.16.0': {}
+  '@remix-run/router@1.16.1': {}
 
   '@restart/hooks@0.4.16(react@18.3.1)':
     dependencies:
       dequal: 2.0.3
       react: 18.3.1
 
   '@restart/ui@1.6.8(react-dom@18.3.1(react@18.3.1))(react@18.3.1)':
@@ -2895,130 +2898,123 @@
     dependencies:
       undici-types: 5.26.5
 
   '@types/prop-types@15.7.12': {}
 
   '@types/react-dom@18.3.0':
     dependencies:
-      '@types/react': 18.3.1
+      '@types/react': 18.3.3
 
   '@types/react-syntax-highlighter@15.5.13':
     dependencies:
-      '@types/react': 18.3.1
+      '@types/react': 18.3.3
 
   '@types/react-test-renderer@18.3.0':
     dependencies:
-      '@types/react': 18.3.1
+      '@types/react': 18.3.3
 
   '@types/react-transition-group@4.4.10':
     dependencies:
-      '@types/react': 18.3.1
+      '@types/react': 18.3.3
 
-  '@types/react@18.3.1':
+  '@types/react@18.3.3':
     dependencies:
       '@types/prop-types': 15.7.12
       csstype: 3.1.3
 
-  '@types/semver@7.5.8': {}
-
   '@types/unist@2.0.10': {}
 
   '@types/urijs@1.19.25': {}
 
   '@types/warning@3.0.3': {}
 
-  '@typescript-eslint/eslint-plugin@7.8.0(@typescript-eslint/parser@7.8.0(eslint@8.57.0)(typescript@5.4.5))(eslint@8.57.0)(typescript@5.4.5)':
+  '@typescript-eslint/eslint-plugin@7.10.0(@typescript-eslint/parser@7.10.0(eslint@8.57.0)(typescript@5.4.5))(eslint@8.57.0)(typescript@5.4.5)':
     dependencies:
       '@eslint-community/regexpp': 4.10.0
-      '@typescript-eslint/parser': 7.8.0(eslint@8.57.0)(typescript@5.4.5)
-      '@typescript-eslint/scope-manager': 7.8.0
-      '@typescript-eslint/type-utils': 7.8.0(eslint@8.57.0)(typescript@5.4.5)
-      '@typescript-eslint/utils': 7.8.0(eslint@8.57.0)(typescript@5.4.5)
-      '@typescript-eslint/visitor-keys': 7.8.0
-      debug: 4.3.4
+      '@typescript-eslint/parser': 7.10.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/scope-manager': 7.10.0
+      '@typescript-eslint/type-utils': 7.10.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/utils': 7.10.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/visitor-keys': 7.10.0
       eslint: 8.57.0
       graphemer: 1.4.0
       ignore: 5.3.1
       natural-compare: 1.4.0
-      semver: 7.6.0
       ts-api-utils: 1.3.0(typescript@5.4.5)
     optionalDependencies:
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
 
-  '@typescript-eslint/parser@7.8.0(eslint@8.57.0)(typescript@5.4.5)':
+  '@typescript-eslint/parser@7.10.0(eslint@8.57.0)(typescript@5.4.5)':
     dependencies:
-      '@typescript-eslint/scope-manager': 7.8.0
-      '@typescript-eslint/types': 7.8.0
-      '@typescript-eslint/typescript-estree': 7.8.0(typescript@5.4.5)
-      '@typescript-eslint/visitor-keys': 7.8.0
+      '@typescript-eslint/scope-manager': 7.10.0
+      '@typescript-eslint/types': 7.10.0
+      '@typescript-eslint/typescript-estree': 7.10.0(typescript@5.4.5)
+      '@typescript-eslint/visitor-keys': 7.10.0
       debug: 4.3.4
       eslint: 8.57.0
     optionalDependencies:
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
 
-  '@typescript-eslint/scope-manager@7.8.0':
+  '@typescript-eslint/scope-manager@7.10.0':
     dependencies:
-      '@typescript-eslint/types': 7.8.0
-      '@typescript-eslint/visitor-keys': 7.8.0
+      '@typescript-eslint/types': 7.10.0
+      '@typescript-eslint/visitor-keys': 7.10.0
 
-  '@typescript-eslint/type-utils@7.8.0(eslint@8.57.0)(typescript@5.4.5)':
+  '@typescript-eslint/type-utils@7.10.0(eslint@8.57.0)(typescript@5.4.5)':
     dependencies:
-      '@typescript-eslint/typescript-estree': 7.8.0(typescript@5.4.5)
-      '@typescript-eslint/utils': 7.8.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/typescript-estree': 7.10.0(typescript@5.4.5)
+      '@typescript-eslint/utils': 7.10.0(eslint@8.57.0)(typescript@5.4.5)
       debug: 4.3.4
       eslint: 8.57.0
       ts-api-utils: 1.3.0(typescript@5.4.5)
     optionalDependencies:
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
 
-  '@typescript-eslint/types@7.8.0': {}
+  '@typescript-eslint/types@7.10.0': {}
 
-  '@typescript-eslint/typescript-estree@7.8.0(typescript@5.4.5)':
+  '@typescript-eslint/typescript-estree@7.10.0(typescript@5.4.5)':
     dependencies:
-      '@typescript-eslint/types': 7.8.0
-      '@typescript-eslint/visitor-keys': 7.8.0
+      '@typescript-eslint/types': 7.10.0
+      '@typescript-eslint/visitor-keys': 7.10.0
       debug: 4.3.4
       globby: 11.1.0
       is-glob: 4.0.3
       minimatch: 9.0.4
       semver: 7.6.0
       ts-api-utils: 1.3.0(typescript@5.4.5)
     optionalDependencies:
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
 
-  '@typescript-eslint/utils@7.8.0(eslint@8.57.0)(typescript@5.4.5)':
+  '@typescript-eslint/utils@7.10.0(eslint@8.57.0)(typescript@5.4.5)':
     dependencies:
       '@eslint-community/eslint-utils': 4.4.0(eslint@8.57.0)
-      '@types/json-schema': 7.0.15
-      '@types/semver': 7.5.8
-      '@typescript-eslint/scope-manager': 7.8.0
-      '@typescript-eslint/types': 7.8.0
-      '@typescript-eslint/typescript-estree': 7.8.0(typescript@5.4.5)
+      '@typescript-eslint/scope-manager': 7.10.0
+      '@typescript-eslint/types': 7.10.0
+      '@typescript-eslint/typescript-estree': 7.10.0(typescript@5.4.5)
       eslint: 8.57.0
-      semver: 7.6.0
     transitivePeerDependencies:
       - supports-color
       - typescript
 
-  '@typescript-eslint/visitor-keys@7.8.0':
+  '@typescript-eslint/visitor-keys@7.10.0':
     dependencies:
-      '@typescript-eslint/types': 7.8.0
+      '@typescript-eslint/types': 7.10.0
       eslint-visitor-keys: 3.4.3
 
   '@ungap/structured-clone@1.2.0': {}
 
-  '@vitejs/plugin-react@4.2.1(vite@5.2.11(@types/node@20.11.5)(terser@5.27.0))':
+  '@vitejs/plugin-react@4.3.0(vite@5.2.11(@types/node@20.11.5)(terser@5.27.0))':
     dependencies:
       '@babel/core': 7.24.5
       '@babel/plugin-transform-react-jsx-self': 7.24.5(@babel/core@7.24.5)
       '@babel/plugin-transform-react-jsx-source': 7.24.1(@babel/core@7.24.5)
       '@types/babel__core': 7.20.5
       react-refresh: 0.14.2
       vite: 5.2.11(@types/node@20.11.5)(terser@5.27.0)
@@ -4077,27 +4073,27 @@
 
   js-tokens@9.0.0: {}
 
   js-yaml@4.1.0:
     dependencies:
       argparse: 2.0.1
 
-  jsdom@24.0.0:
+  jsdom@24.1.0:
     dependencies:
       cssstyle: 4.0.1
       data-urls: 5.0.0
       decimal.js: 10.4.3
       form-data: 4.0.0
       html-encoding-sniffer: 4.0.0
       http-proxy-agent: 7.0.2
       https-proxy-agent: 7.0.4
       is-potential-custom-element-name: 1.0.1
-      nwsapi: 2.2.9
+      nwsapi: 2.2.10
       parse5: 7.1.2
-      rrweb-cssom: 0.6.0
+      rrweb-cssom: 0.7.0
       saxes: 6.0.0
       symbol-tree: 3.2.4
       tough-cookie: 4.1.4
       w3c-xmlserializer: 5.0.0
       webidl-conversions: 7.0.0
       whatwg-encoding: 3.1.1
       whatwg-mimetype: 4.0.0
@@ -4219,15 +4215,15 @@
 
   node-releases@2.0.14: {}
 
   npm-run-path@5.3.0:
     dependencies:
       path-key: 4.0.0
 
-  nwsapi@2.2.9: {}
+  nwsapi@2.2.10: {}
 
   object-assign@4.1.1: {}
 
   object-inspect@1.13.1: {}
 
   object-keys@1.1.1: {}
 
@@ -4390,15 +4386,15 @@
       safe-buffer: 5.2.1
 
   react-bootstrap-icons@1.11.4(react@18.3.1):
     dependencies:
       prop-types: 15.8.1
       react: 18.3.1
 
-  react-bootstrap@2.10.2(@types/react@18.3.1)(react-dom@18.3.1(react@18.3.1))(react@18.3.1):
+  react-bootstrap@2.10.2(@types/react@18.3.3)(react-dom@18.3.1(react@18.3.1))(react@18.3.1):
     dependencies:
       '@babel/runtime': 7.24.5
       '@restart/hooks': 0.4.16(react@18.3.1)
       '@restart/ui': 1.6.8(react-dom@18.3.1(react@18.3.1))(react@18.3.1)
       '@types/react-transition-group': 4.4.10
       classnames: 2.5.1
       dom-helpers: 5.2.1
@@ -4407,15 +4403,15 @@
       prop-types-extra: 1.1.1(react@18.3.1)
       react: 18.3.1
       react-dom: 18.3.1(react@18.3.1)
       react-transition-group: 4.4.5(react-dom@18.3.1(react@18.3.1))(react@18.3.1)
       uncontrollable: 7.2.1(react@18.3.1)
       warning: 4.0.3
     optionalDependencies:
-      '@types/react': 18.3.1
+      '@types/react': 18.3.3
 
   react-dom@18.3.1(react@18.3.1):
     dependencies:
       loose-envify: 1.4.0
       react: 18.3.1
       scheduler: 0.23.2
 
@@ -4423,24 +4419,24 @@
 
   react-is@18.3.1: {}
 
   react-lifecycles-compat@3.0.4: {}
 
   react-refresh@0.14.2: {}
 
-  react-router-dom@6.23.0(react-dom@18.3.1(react@18.3.1))(react@18.3.1):
+  react-router-dom@6.23.1(react-dom@18.3.1(react@18.3.1))(react@18.3.1):
     dependencies:
-      '@remix-run/router': 1.16.0
+      '@remix-run/router': 1.16.1
       react: 18.3.1
       react-dom: 18.3.1(react@18.3.1)
-      react-router: 6.23.0(react@18.3.1)
+      react-router: 6.23.1(react@18.3.1)
 
-  react-router@6.23.0(react@18.3.1):
+  react-router@6.23.1(react@18.3.1):
     dependencies:
-      '@remix-run/router': 1.16.0
+      '@remix-run/router': 1.16.1
       react: 18.3.1
 
   react-shallow-renderer@16.15.0(react@18.3.1):
     dependencies:
       object-assign: 4.1.1
       react: 18.3.1
       react-is: 18.3.1
@@ -4546,14 +4542,16 @@
       '@rollup/rollup-win32-arm64-msvc': 4.17.2
       '@rollup/rollup-win32-ia32-msvc': 4.17.2
       '@rollup/rollup-win32-x64-msvc': 4.17.2
       fsevents: 2.3.3
 
   rrweb-cssom@0.6.0: {}
 
+  rrweb-cssom@0.7.0: {}
+
   run-parallel@1.2.0:
     dependencies:
       queue-microtask: 1.2.3
 
   safe-array-concat@1.1.2:
     dependencies:
       call-bind: 1.0.7
@@ -4844,15 +4842,15 @@
       has-bigints: 1.0.2
       has-symbols: 1.0.3
       which-boxed-primitive: 1.0.2
 
   uncontrollable@7.2.1(react@18.3.1):
     dependencies:
       '@babel/runtime': 7.24.5
-      '@types/react': 18.3.1
+      '@types/react': 18.3.3
       invariant: 2.2.4
       react: 18.3.1
       react-lifecycles-compat: 3.0.4
 
   uncontrollable@8.0.4(react@18.3.1):
     dependencies:
       react: 18.3.1
@@ -4876,15 +4874,15 @@
   url-parse@1.5.10:
     dependencies:
       querystringify: 2.2.0
       requires-port: 1.0.0
 
   v8-compile-cache-lib@3.0.1: {}
 
-  vite-bundle-visualizer@1.1.0(rollup@4.17.2):
+  vite-bundle-visualizer@1.2.1(rollup@4.17.2):
     dependencies:
       cac: 6.7.14
       import-from-esm: 1.3.4
       rollup-plugin-visualizer: 5.12.0(rollup@4.17.2)
       tmp: 0.2.3
     transitivePeerDependencies:
       - rollup
@@ -4913,15 +4911,15 @@
       postcss: 8.4.38
       rollup: 4.17.2
     optionalDependencies:
       '@types/node': 20.11.5
       fsevents: 2.3.3
       terser: 5.27.0
 
-  vitest@1.6.0(@types/node@20.11.5)(jsdom@24.0.0)(terser@5.27.0):
+  vitest@1.6.0(@types/node@20.11.5)(jsdom@24.1.0)(terser@5.27.0):
     dependencies:
       '@vitest/expect': 1.6.0
       '@vitest/runner': 1.6.0
       '@vitest/snapshot': 1.6.0
       '@vitest/spy': 1.6.0
       '@vitest/utils': 1.6.0
       acorn-walk: 8.3.2
@@ -4937,15 +4935,15 @@
       tinybench: 2.8.0
       tinypool: 0.8.4
       vite: 5.2.11(@types/node@20.11.5)(terser@5.27.0)
       vite-node: 1.6.0(@types/node@20.11.5)(terser@5.27.0)
       why-is-node-running: 2.2.2
     optionalDependencies:
       '@types/node': 20.11.5
-      jsdom: 24.0.0
+      jsdom: 24.1.0
     transitivePeerDependencies:
       - less
       - lightningcss
       - sass
       - stylus
       - sugarss
       - supports-color
```

### Comparing `bowtie_json_schema-2024.5.9/frontend/tsconfig.json` & `bowtie_json_schema-2024.6.1/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/public/favicon.svg` & `bowtie_json_schema-2024.6.1/frontend/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/DialectReportView.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/DialectReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/ReportDataHandler.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/ReportDataHandler.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/index.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/index.tsx`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import { implementationMetadataURI } from "./data/Site";
 import {
   ImplementationData,
   ReportData,
   implementationFromData,
   prepareImplementationReport,
 } from "./data/parseReportData";
+import EmbedBadges from "./components/ImplementationReportView/EmbedBadges";
 
 const fetchReportData = async (dialect: Dialect) => {
   document.title = `Bowtie - ${dialect.prettyName}`;
   return dialect.fetchReport();
 };
 
 const fetchAllReportsData = async (langImplementation: string) => {
@@ -29,20 +30,15 @@
   const promises = [];
   for (const dialect of Dialect.known()) {
     promises.push(
       dialect.fetchReport().then((data) => allReportsData.set(dialect, data)),
     );
   }
   await Promise.all(promises);
-
-  // FIXME: This magic prefix is duplicated from the backend side,
-  //        and probably we can separate handling this in Implementation
-  //        class (when we have it).
-  const implementationId = `ghcr.io/bowtie-json-schema/${langImplementation}`;
-  return prepareImplementationReport(allReportsData, implementationId);
+  return prepareImplementationReport(allReportsData, langImplementation);
 };
 
 const fetchImplementationMetadata = async () => {
   const response = await fetch(implementationMetadataURI);
   const implementations = (await response.json()) as Record<
     string,
     ImplementationData
@@ -85,14 +81,20 @@
         Component: DragAndDrop,
       },
       {
         path: "/implementations/:langImplementation",
         Component: ImplementationReportView,
         loader: async ({ params }) =>
           fetchAllReportsData(params.langImplementation!),
+        children: [
+          {
+            path: "badges",
+            Component: EmbedBadges,
+          },
+        ],
       },
     ],
   },
 ]);
 
 document.addEventListener("DOMContentLoaded", () => {
   const root = createRoot(document.getElementById("root")!);
```

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/assets/landscape-logo.svg` & `bowtie_json_schema-2024.6.1/frontend/src/assets/landscape-logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/CopyToClipboard.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/CopyToClipboard.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/FilterSection.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/FilterSection.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import "./FilterSection.css";
+import { Link } from "react-router-dom";
 import Badge from "react-bootstrap/Badge";
 import Card from "react-bootstrap/Card";
-import { Link } from "react-router-dom";
-import { useSearchParams } from "../hooks/useSearchParams.ts";
 import { X } from "react-bootstrap-icons";
+
+import { useSearchParams } from "../hooks/useSearchParams.ts";
 import { mapLanguage } from "../data/mapLanguage.ts";
+import styles from "./FilterSection.module.css";
 
 export const FilterSection = ({ languages }: { languages: string[] }) => {
   const params = useSearchParams();
 
   return (
     <Card className="mx-auto mb-3">
       <Card.Header>Filtering</Card.Header>
@@ -36,25 +37,25 @@
     const newParams = new URLSearchParams(searchParams);
     newParams.delete("language");
     languages
       .filter((lang) => lang !== current)
       .forEach((lang) => newParams.append("language", lang));
     return (
       <Link key={current} to={{ search: newParams.toString() }}>
-        <Badge pill bg="filter-active">
+        <Badge pill bg="" className={styles["bg-filter-active"]}>
           <div className="px-2">{mapLanguage(current)}</div>
           <X size="20px" className="mr-1" />
         </Badge>
       </Link>
     );
   } else {
     const newParams = new URLSearchParams(searchParams);
     newParams.append("language", current);
     return (
       <Link key={current} to={{ search: newParams.toString() }}>
-        <Badge pill bg="filter">
+        <Badge pill bg="" className={styles["bg-filter"]}>
           <div className="px-2">{mapLanguage(current)}</div>
         </Badge>
       </Link>
     );
   }
 };
```

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/NavBar.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/NavBar.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/OtherImplementations.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/OtherImplementations.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -45,22 +45,21 @@
         >
           {(props) => (
             <Popover id="popover-basic" {...props}>
               <Popover.Body>
                 <Container className="p-0">
                   <Row className="d-grid gap-2">
                     {otherImplementationsDataArray.map(([id, impl]) => {
-                      const implementationPath = getImplementationPath(id);
                       const latest = getLatestSupportedDialect(impl);
                       return (
                         <Col key={id}>
                           <div>
                             <NavLink
                               style={{ fontSize: "1rem", fontWeight: "bold" }}
-                              to={`/implementations/${implementationPath}`}
+                              to={`/implementations/${id}`}
                             >
                               {impl.name}
                             </NavLink>
                             <span className="ps-1 text-body-secondary fw-bold">
                               {mapLanguage(impl.language)}
                             </span>
                           </div>
@@ -88,17 +87,12 @@
         Other implementations are available which do not support the current
         dialect and filters.
       </div>
     </div>
   );
 };
 
-const getImplementationPath = (id: string): string => {
-  const pathSegment = id.split("/");
-  return pathSegment[pathSegment.length - 1];
-};
-
 const getLatestSupportedDialect = (impl: Implementation): Dialect => {
   return impl.dialects.reduce((acc, curr) =>
     curr.firstPublicationDate > acc.firstPublicationDate ? curr : acc,
   );
 };
```

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/Cases/CaseItem.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CaseItem.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/Cases/CaseResultSvg.test.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CaseResultSvg.test.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/Cases/CaseResultSvg.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CaseResultSvg.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/Cases/CasesSection.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/Cases/CasesSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/Cases/SchemaDisplay.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/Cases/SchemaDisplay.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/DragAndDrop/DragAndDrop.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/DragAndDrop/DragAndDrop.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import { ChangeEvent, DragEvent, useEffect, useRef, useState } from "react";
 import { CloudArrowUpFill } from "react-bootstrap-icons";
 import { useLocation } from "react-router-dom";
-import "./DragAndDrop.css";
+
 import { DialectReportView } from "../../DialectReportView";
 import { ReportData, parseReportData } from "../../data/parseReportData";
+import styles from "./DragAndDrop.module.css";
 
 export const DragAndDrop = () => {
   const location = useLocation();
 
   const [dragActive, setDragActive] = useState(false);
   const [invalidFile, setInvalidFile] = useState(false);
   const [lines, setLines] = useState<ReportData | null>(null);
@@ -85,15 +86,15 @@
 
   return (
     <div>
       <div aria-live="polite" aria-atomic="true"></div>
 
       <div className="card-body d-grid justify-content-center">
         <form
-          className="form-file-upload"
+          className={styles["form-file-upload"]}
           onDragEnter={handleDragEnter}
           onDragOver={handleDragEnter}
           onDragLeave={handleDragLeave}
           onDrop={handleDrop}
           onSubmit={(e) => e.preventDefault()}
         >
           <input
@@ -101,19 +102,19 @@
             type="file"
             id="input-file-upload"
             className="d-none"
             onChange={handleChange}
           />
 
           <div
-            id="label-file-upload"
-            className={dragActive ? "drag-active" : ""}
+            id={styles["label-file-upload"]}
+            className={dragActive ? styles["drag-active"] : ""}
             style={{ backgroundColor: `${invalidFile ? "#f00b0b39" : ""}` }}
           >
-            <div className="flex-div text-center">
+            <div className={`${styles["flex-div"]} text-center`}>
               <p>
                 You can generate a report by running{" "}
                 <a href="https://docs.bowtie.report/en/stable/cli/">
                   Bowtie&apos;s CLI
                 </a>{" "}
                 via e.g.:
               </p>
@@ -129,15 +130,15 @@
               <p>
                 which will run the <code>refRemote.json</code> test file from
                 the official suite against the specified implementation,
                 emitting a file called &apos;output&apos; which you can then
                 upload here!
               </p>
             </div>
-            <div className="flex-div text-center">
+            <div className={`${styles["flex-div"]} text-center`}>
               <CloudArrowUpFill size={80} />
               {invalidFile ? (
                 <h5 className={"pt-3 text-danger"}>
                   That doesn&apos;t look like a Bowtie report.
                 </h5>
               ) : (
                 <>
```

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/ImplementationReportView/DialectCompliance.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/ImplementationReportView/DialectCompliance.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/ImplementationReportView/EmbedBadges.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/ImplementationReportView/EmbedBadges.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -1,144 +1,142 @@
-import React, { useContext, useState } from "react";
+import { useContext, useState } from "react";
+import { useOutletContext, useNavigate } from "react-router-dom";
+import { Prism as SyntaxHighlighter } from "react-syntax-highlighter";
+import {
+  oneDark,
+  oneLight,
+} from "react-syntax-highlighter/dist/esm/styles/prism";
 import Container from "react-bootstrap/Container";
 import Image from "react-bootstrap/Image";
 import ListGroup from "react-bootstrap/ListGroup";
-import Button from "react-bootstrap/Button";
 import Modal from "react-bootstrap/Modal";
 import Row from "react-bootstrap/Row";
 import Col from "react-bootstrap/Col";
+
 import CopyToClipboard from "../CopyToClipboard";
-import { Implementation } from "../../data/parseReportData";
+import { EmbedBadgesContextType } from "./ImplementationReportView";
 import { Badge, badgesFor } from "../../data/Badge";
-import { Prism as SyntaxHighlighter } from "react-syntax-highlighter";
 import { ThemeContext } from "../../context/ThemeContext";
-import {
-  oneDark,
-  oneLight,
-} from "react-syntax-highlighter/dist/esm/styles/prism";
-import "./EmbedBadges.css";
+import styles from "./EmbedBadges.module.css";
 
-const EmbedBadges: React.FC<{
-  implementation: Implementation;
-}> = ({ implementation }) => {
+const EmbedBadges = () => {
+  const navigate = useNavigate();
+  const { implementationId, implementation } =
+    useOutletContext<EmbedBadgesContextType>();
   const allBadges = badgesFor(implementation);
   const { isDarkMode } = useContext(ThemeContext);
 
   const [activeFormat, setActiveFormat] = useState(supportedFormats[1]);
   const [activeBadge, setActiveBadge] = useState(allBadges.Metadata[0]);
-  const [show, setShow] = useState(false);
+  const [show, setShow] = useState(true);
   const badgeEmbed = activeFormat.generateEmbed(activeBadge);
 
   return (
-    <>
-      <Button variant="info" size="sm" onClick={() => setShow(true)}>
-        Badges
-      </Button>
-      <Modal
-        fullscreen="xl-down"
-        contentClassName="px-4"
-        dialogClassName="modal-width"
-        show={show}
-        onHide={() => setShow(false)}
-      >
-        <Modal.Header closeButton className="border-0 mt-4">
-          <Modal.Title className="fs-5 ms-3">Badges</Modal.Title>
-        </Modal.Header>
-        <Modal.Body>
-          <Container className="px-5">
-            <Row className="pb-3 gap-5 align-items-center">
-              <Col sm={5} md={3} lg={2} className="order-2 order-md-1">
-                <div>
-                  {Object.entries(allBadges).map(([category, badges]) => (
-                    <div key={category}>
-                      <h6>{category}</h6>
-                      <ListGroup variant="flush" className="pb-2">
-                        {badges.map((badge) => (
-                          <ListGroup.Item
-                            key={badge.name}
-                            action
-                            active={badge.name === activeBadge.name}
-                            onClick={() => setActiveBadge(badge)}
-                          >
-                            {badge.name}
-                          </ListGroup.Item>
-                        ))}
-                      </ListGroup>
-                    </div>
-                  ))}
-                </div>
-              </Col>
-
-              <Col
-                sm={12}
-                md={8}
-                lg={6}
-                xl
-                className="overflow-auto order-1 order-md-2"
-              >
-                <div className="pb-3">
-                  <p>
-                    Bowtie regularly rebuilds a number of badges for
-                    <code> {implementation.name}</code>.
-                  </p>
-                  <p>
-                    If you are a maintainer, you may be interested in embedding
-                    one or more of them in your documentation to show off! Here
-                    are embeddable snippets for whatever documentation language
-                    you are likely to be using. The badge will automatically
-                    update as Bowtie re-runs its report, so no manual updating
-                    should be necessary.
-                  </p>
-                </div>
-
-                <hr className="mx-5 py-3" />
-                <div className="font-monospace d-flex position-relative rounded mx-5">
-                  <span className="m-2 position-absolute top-0 end-0">
-                    <CopyToClipboard textToCopy={badgeEmbed} />
-                  </span>
-                  <SyntaxHighlighter
-                    language={activeFormat.name.toLowerCase()}
-                    style={isDarkMode ? oneDark : oneLight}
-                    className="code-block"
-                    wrapLongLines
+    <Modal
+      fullscreen="xl-down"
+      contentClassName="px-4"
+      dialogClassName={styles["modal-width"]}
+      show={show}
+      onHide={() => setShow(false)}
+      onExited={() => navigate(`/implementations/${implementationId}`)}
+    >
+      <Modal.Header closeButton className="border-0 mt-4">
+        <Modal.Title className="fs-5 ms-3">Badges</Modal.Title>
+      </Modal.Header>
+      <Modal.Body>
+        <Container className="px-5">
+          <Row className="pb-3 gap-5 align-items-center">
+            <Col sm={5} md={3} lg={2} className="order-2 order-md-1">
+              <div>
+                {Object.entries(allBadges).map(([category, badges]) => (
+                  <div key={category}>
+                    <h6>{category}</h6>
+                    <ListGroup variant="flush" className="pb-2">
+                      {badges.map((badge) => (
+                        <ListGroup.Item
+                          key={badge.name}
+                          action
+                          active={badge.name === activeBadge.name}
+                          onClick={() => setActiveBadge(badge)}
+                        >
+                          {badge.name}
+                        </ListGroup.Item>
+                      ))}
+                    </ListGroup>
+                  </div>
+                ))}
+              </div>
+            </Col>
+
+            <Col
+              sm={12}
+              md={8}
+              lg={6}
+              xl
+              className="overflow-auto order-1 order-md-2"
+            >
+              <div className="pb-3">
+                <p>
+                  Bowtie regularly rebuilds a number of badges for
+                  <code> {implementation.name}</code>.
+                </p>
+                <p>
+                  If you are a maintainer, you may be interested in embedding
+                  one or more of them in your documentation to show off! Here
+                  are embeddable snippets for whatever documentation language
+                  you are likely to be using. The badge will automatically
+                  update as Bowtie re-runs its report, so no manual updating
+                  should be necessary.
+                </p>
+              </div>
+
+              <hr className="mx-5 py-3" />
+              <div className="font-monospace d-flex position-relative rounded mx-5">
+                <span className="m-2 position-absolute top-0 end-0">
+                  <CopyToClipboard textToCopy={badgeEmbed} />
+                </span>
+                <SyntaxHighlighter
+                  language={activeFormat.name.toLowerCase()}
+                  style={isDarkMode ? oneDark : oneLight}
+                  className={styles["code-block"]}
+                  wrapLongLines
+                >
+                  {badgeEmbed}
+                </SyntaxHighlighter>
+              </div>
+
+              <Image
+                alt={activeBadge.name}
+                src={activeBadge.uri.href()}
+                className="d-block mx-auto my-5"
+              />
+              <hr className="mx-5 d-lg-none" />
+            </Col>
+
+            <div className="vr my-lg-5 px-0 order-3 d-none d-sm-block d-md-none d-lg-block"></div>
+            <Col sm={4} md={5} lg xl={2} className="order-4 px-lg-0 pb-1">
+              <hr className="hr d-block d-sm-none order-3 m-5 mt-0"></hr>
+              <h5 className="ps-1">Format</h5>
+              <ListGroup variant="flush">
+                {supportedFormats.map((format) => (
+                  <ListGroup.Item
+                    action
+                    active={activeFormat === format}
+                    onClick={() => setActiveFormat(format)}
+                    key={format.name}
                   >
-                    {badgeEmbed}
-                  </SyntaxHighlighter>
-                </div>
-
-                <Image
-                  alt={activeBadge.name}
-                  src={activeBadge.uri.href()}
-                  className="d-block mx-auto my-5"
-                />
-                <hr className="mx-5 d-lg-none" />
-              </Col>
-
-              <div className="vr my-lg-5 px-0 order-3 d-none d-sm-block d-md-none d-lg-block"></div>
-              <Col sm={4} md={5} lg xl={2} className="order-4 px-lg-0 pb-1">
-                <hr className="hr d-block d-sm-none order-3 m-5 mt-0"></hr>
-                <h5 className="ps-1">Format</h5>
-                <ListGroup variant="flush">
-                  {supportedFormats.map((format) => (
-                    <ListGroup.Item
-                      action
-                      active={activeFormat === format}
-                      onClick={() => setActiveFormat(format)}
-                      key={format.name}
-                    >
-                      {format.name}
-                    </ListGroup.Item>
-                  ))}
-                </ListGroup>
-              </Col>
-            </Row>
-          </Container>
-        </Modal.Body>
-      </Modal>
-    </>
+                    {format.name}
+                  </ListGroup.Item>
+                ))}
+              </ListGroup>
+            </Col>
+          </Row>
+        </Container>
+      </Modal.Body>
+    </Modal>
   );
 };
 
 interface BadgeFormat {
   name: string;
   generateEmbed: (badge: Badge) => string;
 }
```

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,30 @@
+import {
+  useLoaderData,
+  Link,
+  Navigate,
+  Outlet,
+  useNavigate,
+} from "react-router-dom";
 import Container from "react-bootstrap/Container";
 import Card from "react-bootstrap/Card";
 import Table from "react-bootstrap/Table";
-import { useLoaderData, Link, Navigate } from "react-router-dom";
+import Button from "react-bootstrap/Button";
 
 import DialectCompliance from "./DialectCompliance";
-import EmbedBadges from "./EmbedBadges";
 import LoadingAnimation from "../LoadingAnimation";
 import { ImplementationReport } from "../../data/parseReportData";
 import { mapLanguage } from "../../data/mapLanguage";
 import { versionsBadgeFor } from "../../data/Badge";
 
+export type EmbedBadgesContextType = Pick<
+  ImplementationReport,
+  "implementationId" | "implementation"
+>;
+
 export const ImplementationReportView = () => {
   const implementationReport = useLoaderData() as ImplementationReport | null;
 
   return implementationReport === null ? (
     // FIXME: Probably redirect to /implementations if/when that's a thing.
     <Navigate to="/" />
   ) : !implementationReport ? (
@@ -22,27 +33,38 @@
     <ReportComponent implementationReport={implementationReport} />
   );
 };
 
 const ReportComponent: React.FC<{
   implementationReport: ImplementationReport;
 }> = ({ implementationReport }) => {
-  const { implementation } = implementationReport;
+  const navigate = useNavigate();
+  const { implementationId, implementation } = implementationReport;
 
   return (
     <Container className="p-4">
       <Card className="mx-auto mb-3 col-md-9">
         <Card.Header className="d-flex align-items-center justify-content-between">
           <span className="d-flex">
             <span className="pe-2 text-muted">
               {mapLanguage(implementation.language)}
             </span>
             <span>{implementation.name}</span>
           </span>
-          <EmbedBadges implementation={implementation} />
+          <Button variant="info" size="sm" onClick={() => navigate("badges")}>
+            Badges
+          </Button>
+          <Outlet
+            context={
+              {
+                implementation,
+                implementationId,
+              } satisfies EmbedBadgesContextType
+            }
+          />
         </Card.Header>
 
         <Card.Body className="overflow-x-auto">
           <Table>
             <tbody>
               <tr>
                 <th>Homepage</th>
```

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/Modals/DetailsButtonModal.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/Modals/DetailsButtonModal.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/RunInfo/RunInfoSection.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/RunInfo/RunInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2024.6.1/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/Summary/ImplementationRow.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/Summary/ImplementationRow.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -22,21 +22,20 @@
   implementationResults: ImplementationResults;
   key: number;
   index: number;
 }) => {
   const { isDarkMode } = useContext(ThemeContext);
   const [showDetails, setShowDetails] = useState(false);
   const navigate = useNavigate();
-  const implementationPath = getImplementationPath(id);
 
   return (
     <tr>
       <th
         className="table-implementation-name align-middle p-0"
-        onClick={() => navigate(`/implementations/${implementationPath}`)}
+        onClick={() => navigate(`/implementations/${id}`)}
         scope="row"
       >
         <span
           className={`text-decoration-underline ${
             isDarkMode ? "text-primary-emphasis" : "text-primary"
           }`}
         >
@@ -92,13 +91,8 @@
         implementationResults={implementationResults}
         implementation={implementation}
       />
     </tr>
   );
 };
 
-const getImplementationPath = (id: string) => {
-  const pathSegment = id.split("/");
-  return pathSegment[pathSegment.length - 1];
-};
-
 export default ImplementationRow;
```

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/Summary/SummarySection.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/Summary/SummarySection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/components/Summary/SummaryTable.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/components/Summary/SummaryTable.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/context/BowtieVersionContext.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/context/BowtieVersionContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/context/ThemeContext.tsx` & `bowtie_json_schema-2024.6.1/frontend/src/context/ThemeContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/data/Badge.test.ts` & `bowtie_json_schema-2024.6.1/frontend/src/data/Badge.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/data/Badge.ts` & `bowtie_json_schema-2024.6.1/frontend/src/data/Badge.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/data/Dialect.ts` & `bowtie_json_schema-2024.6.1/frontend/src/data/Dialect.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/data/Site.test.ts` & `bowtie_json_schema-2024.6.1/frontend/src/data/Site.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/data/parseReportData.test.ts` & `bowtie_json_schema-2024.6.1/frontend/src/data/parseReportData.test.ts`

 * *Files 2% similar despite different names*

```diff
@@ -290,32 +290,34 @@
       didFailFast: false,
     });
   });
 
   test("prepares a summarized implementation report using all the dialect reports", () => {
     const cases = Object.values(testCases).map((each) => JSON.stringify(each));
     const allReportsData = new Map<Dialect, ReportData>();
+    const fakeImplementationId = tag("envsonschema");
 
     for (const dialect of Dialect.known()) {
       const lines = bowtie(
-        ["run", "-i", tag("envsonschema"), "-D", dialect.shortName],
+        ["run", "-i", fakeImplementationId, "-D", dialect.shortName],
         cases.join("\n") + "\n",
       );
       const report = fromSerialized(lines);
       allReportsData.set(dialect, report);
     }
 
     const implementationReport = prepareImplementationReport(
       allReportsData,
-      tag("envsonschema"),
+      fakeImplementationId,
     );
 
     const metadata = implementationReport!.implementation;
 
     expect(implementationReport).toStrictEqual({
+      implementationId: fakeImplementationId,
       implementation: {
         name: "envsonschema",
         language: "python",
         homepage: metadata.homepage,
         issues: metadata.issues,
         source: metadata.source,
         dialects: metadata.dialects,
```

### Comparing `bowtie_json_schema-2024.5.9/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2024.6.1/frontend/src/data/parseReportData.ts`

 * *Files 1% similar despite different names*

```diff
@@ -200,19 +200,21 @@
         failedTests: implementationResults.totals.failedTests,
       });
 
       const implementation = runMetadata.implementations.get(implementationId)!;
 
       if (!implementationReport) {
         implementationReport = {
+          implementationId,
           implementation,
           dialectCompliance,
         };
       } else {
         implementationReport = {
+          implementationId,
           implementation: Object.assign(
             {},
             implementationReport.implementation,
             implementation,
           ),
           dialectCompliance: new Map([
             ...implementationReport.dialectCompliance,
@@ -305,14 +307,15 @@
   os_version?: string;
   language_version?: string;
 
   [k: string]: unknown;
 }
 
 export interface ImplementationReport {
+  implementationId: string;
   implementation: Implementation;
   dialectCompliance: Map<Dialect, Partial<Totals>>;
 }
 
 export interface Case {
   description: string;
   comment?: string;
```

### Comparing `bowtie_json_schema-2024.5.9/implementations/.java-implementations-pmd-ruleset.xml` & `bowtie_json_schema-2024.6.1/implementations/.java-implementations-pmd-ruleset.xml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/clojure-json-schema/Dockerfile` & `bowtie_json_schema-2024.6.1/implementations/clojure-json-schema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj` & `bowtie_json_schema-2024.6.1/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/cpp-valijson/bowtie_valijson.cpp` & `bowtie_json_schema-2024.6.1/implementations/cpp-valijson/bowtie_valijson.cpp`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/dotnet-jsonschema-net/.gitignore` & `bowtie_json_schema-2024.6.1/implementations/dotnet-corvus-jsonschema/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/dotnet-jsonschema-net/Program.cs` & `bowtie_json_schema-2024.6.1/implementations/dotnet-jsonschema-net/Program.cs`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 using System;
 using System.Collections.Generic;
 using System.IO;
+using System.Linq;
 using System.Text.Json;
 using System.Text.Json.Nodes;
 using System.Reflection;
 using System.Text.RegularExpressions;
 
 using Json.Schema;
 
@@ -85,18 +86,21 @@
             }
 
             var testCase = root["case"];
             var seq = root["seq"].DeepClone();
             var testCaseDescription = testCase["description"].GetValue<string>();
             string? testDescription = null;
             var schemaText = testCase["schema"];
-            var registry = testCase["registry"];
 
-            options.SchemaRegistry.Fetch = uri =>
-            { return registry[uri.ToString()].Deserialize<JsonSchema>(); };
+            JsonNode? nullableRegistry = testCase["registry"];
+            if (nullableRegistry is not null)
+            {
+                var registry = nullableRegistry.AsObject().ToDictionary(x => new Uri(x.Key), x => x.Value);
+                options.SchemaRegistry.Fetch = uri => registry[uri].Deserialize<JsonSchema>();
+            }
 
             var schema = schemaText.Deserialize<JsonSchema>();
             var tests = testCase["tests"].AsArray();
 
             try
             {
                 var results = new JsonArray();
```

### Comparing `bowtie_json_schema-2024.5.9/implementations/go-gojsonschema/bowtie_gojsonschema.go` & `bowtie_json_schema-2024.6.1/implementations/go-gojsonschema/bowtie_gojsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/go-gojsonschema/go.sum` & `bowtie_json_schema-2024.6.1/implementations/go-gojsonschema/go.sum`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/go-jsonschema/bowtie_jsonschema.go` & `bowtie_json_schema-2024.6.1/implementations/go-jsonschema/bowtie_jsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-json-schema/BowtieJsonSchema.java` & `bowtie_json_schema-2024.6.1/implementations/java-json-schema/BowtieJsonSchema.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-json-schema/build.gradle` & `bowtie_json_schema-2024.6.1/implementations/java-json-schema/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.6.1/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-json-tools-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.6.1/implementations/java-json-tools-json-schema-validator/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java` & `bowtie_json_schema-2024.6.1/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-jsonschemafriend/build.gradle` & `bowtie_json_schema-2024.6.1/implementations/java-jsonschemafriend/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.6.1/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-networknt-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.6.1/implementations/java-networknt-json-schema-validator/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/build.gradle.kts` & `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/justfile` & `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/justfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/gradle/libs.versions.toml` & `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/gradle/libs.versions.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [versions]
 validator = "2024.3"
 
-kotlin = "1.9.24"
+kotlin = "2.0.0"
 build-jdk = "11"
 
 [libraries]
 jsv-bom = { module = "io.openapiprocessor:json-schema-validator-bom", version.ref = "validator" }
 jsv-validator = { module = "io.openapiprocessor:json-schema-validator" }
 io-interfaces = { module = "io.openapiprocessor:io-interfaces" }
 io-jackson = { module = "io.openapiprocessor:io-jackson" }
```

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt` & `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/src/main/kotlin/Support.kt` & `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/Support.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt` & `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt` & `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt` & `bowtie_json_schema-2024.6.1/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/js-ajv/bowtie_ajv.js` & `bowtie_json_schema-2024.6.1/implementations/js-ajv/bowtie_ajv.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/js-ajv/package-lock.json` & `bowtie_json_schema-2024.6.1/implementations/js-ajv/package-lock.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9959883432539683%*

 * *Differences: {"'dependencies'": "{'ajv': {'version': '8.14.0', 'resolved': "*

 * *                   "'https://registry.npmjs.org/ajv/-/ajv-8.14.0.tgz', 'integrity': "*

 * *                   "'sha512-oYs1UUtO97ZO2lJ4bwnWeQW8/zvOIQLGKcvPTsWmvc2SYgBb+upuNS5NxoLaMU4h8Ju3Nbj6Cq8mD2LQoqVKFA=='}}",*

 * * "'packages'": "{'': {'dependencies': {'ajv': '^8.14.0'}}, 'node_modules/ajv': {'version': "*

 * *               "'8.14.0', 'resolved': 'https://registry.npmjs.org/ajv/-/ajv-8.14.0.tgz', "*

 * *               "'integrity': "*

 * *               "'sha512-o […]*

```diff
@@ -1,19 +1,19 @@
 {
     "dependencies": {
         "ajv": {
-            "integrity": "sha512-PRA911Blj99jR5RMeTunVbNXMF6Lp4vZXnk5GQjcnUWUTsrXtekg/pnmFFI2u/I36Y/2bITGS30GZCXei6uNkA==",
+            "integrity": "sha512-oYs1UUtO97ZO2lJ4bwnWeQW8/zvOIQLGKcvPTsWmvc2SYgBb+upuNS5NxoLaMU4h8Ju3Nbj6Cq8mD2LQoqVKFA==",
             "requires": {
                 "fast-deep-equal": "^3.1.3",
                 "json-schema-traverse": "^1.0.0",
                 "require-from-string": "^2.0.2",
                 "uri-js": "^4.4.1"
             },
-            "resolved": "https://registry.npmjs.org/ajv/-/ajv-8.13.0.tgz",
-            "version": "8.13.0"
+            "resolved": "https://registry.npmjs.org/ajv/-/ajv-8.14.0.tgz",
+            "version": "8.14.0"
         },
         "ajv-draft-04": {
             "integrity": "sha512-mv00Te6nmYbRp5DCwclxtt7yV/joXJPGS7nM+97GdxvuttCOfgI3K4U25zboyeX0O+myI8ERluxQe5wljMmVIw==",
             "requires": {},
             "resolved": "https://registry.npmjs.org/ajv-draft-04/-/ajv-draft-04-1.0.0.tgz",
             "version": "1.0.0"
         },
@@ -47,15 +47,15 @@
         }
     },
     "lockfileVersion": 2,
     "name": "bowtie-ajv",
     "packages": {
         "": {
             "dependencies": {
-                "ajv": "^8.13.0",
+                "ajv": "^8.14.0",
                 "ajv-draft-04": "^1.0.0"
             },
             "name": "bowtie-ajv",
             "version": "1.0.0"
         },
         "node_modules/ajv": {
             "dependencies": {
@@ -64,17 +64,17 @@
                 "require-from-string": "^2.0.2",
                 "uri-js": "^4.4.1"
             },
             "funding": {
                 "type": "github",
                 "url": "https://github.com/sponsors/epoberezkin"
             },
-            "integrity": "sha512-PRA911Blj99jR5RMeTunVbNXMF6Lp4vZXnk5GQjcnUWUTsrXtekg/pnmFFI2u/I36Y/2bITGS30GZCXei6uNkA==",
-            "resolved": "https://registry.npmjs.org/ajv/-/ajv-8.13.0.tgz",
-            "version": "8.13.0"
+            "integrity": "sha512-oYs1UUtO97ZO2lJ4bwnWeQW8/zvOIQLGKcvPTsWmvc2SYgBb+upuNS5NxoLaMU4h8Ju3Nbj6Cq8mD2LQoqVKFA==",
+            "resolved": "https://registry.npmjs.org/ajv/-/ajv-8.14.0.tgz",
+            "version": "8.14.0"
         },
         "node_modules/ajv-draft-04": {
             "integrity": "sha512-mv00Te6nmYbRp5DCwclxtt7yV/joXJPGS7nM+97GdxvuttCOfgI3K4U25zboyeX0O+myI8ERluxQe5wljMmVIw==",
             "peerDependencies": {
                 "ajv": "^8.5.0"
             },
             "peerDependenciesMeta": {
```

### Comparing `bowtie_json_schema-2024.5.9/implementations/js-hyperjump/bowtie_hyperjump.js` & `bowtie_json_schema-2024.6.1/implementations/js-hyperjump/bowtie_hyperjump.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/js-json-schema/bowtie_json_schema.js` & `bowtie_json_schema-2024.6.1/implementations/js-json-schema/bowtie_json_schema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/js-jsonschema/bowtie_jsonschema.js` & `bowtie_json_schema-2024.6.1/implementations/js-jsonschema/bowtie_jsonschema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts` & `bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt` & `bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt` & `bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt` & `bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt` & `bowtie_json_schema-2024.6.1/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/lua-jsonschema/Dockerfile` & `bowtie_json_schema-2024.6.1/implementations/lua-jsonschema/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM alpine:3.19
+FROM alpine:3.20
 RUN apk add --no-cache luajit luajit-dev pcre-dev gcc libc-dev curl make cmake && \
     wget 'https://luarocks.org/releases/luarocks-3.9.2.tar.gz' && \
     tar -xf luarocks-3.9.2.tar.gz && rm luarocks-3.9.2.tar.gz && \
     cd luarocks-3.9.2 && ./configure && make && make install && \
     cd .. && rm -r luarocks-3.9.2 && \
     sed -i '/WGET/d' /usr/local/share/lua/5.1/luarocks/fs/tools.lua && \
     luarocks install jsonschema && \
```

### Comparing `bowtie_json_schema-2024.5.9/implementations/lua-jsonschema/bowtie_jsonschema.lua` & `bowtie_json_schema-2024.6.1/implementations/lua-jsonschema/bowtie_jsonschema.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/lua-jsonschema/json.lua` & `bowtie_json_schema-2024.6.1/implementations/lua-jsonschema/json.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/php-opis-json-schema/bowtieJsonSchema.php` & `bowtie_json_schema-2024.6.1/implementations/php-opis-json-schema/bowtieJsonSchema.php`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/python-fastjsonschema/bowtie_fastjsonschema.py` & `bowtie_json_schema-2024.6.1/implementations/python-fastjsonschema/bowtie_fastjsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/python-jschon/bowtie_jschon.py` & `bowtie_json_schema-2024.6.1/implementations/python-jschon/bowtie_jschon.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/python-jsonschema/bowtie_jsonschema.py` & `bowtie_json_schema-2024.6.1/implementations/python-jsonschema/bowtie_jsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/ruby-json_schemer/bowtie_json_schemer.rb` & `bowtie_json_schema-2024.6.1/implementations/ruby-json_schemer/bowtie_json_schemer.rb`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/rust-boon/Cargo.lock` & `bowtie_json_schema-2024.6.1/implementations/rust-boon/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "appendlist"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e149dc73cd30538307e7ffa2acd3d2221148eaeed4871f246657b1c3eaa1cbd2"
+
+[[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "base64"
@@ -39,19 +45,20 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "boon"
-version = "0.5.3"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "35b8a1c0fea99bf5301d3851e261168de966419c1d02a705a7ca11da64e54827"
+checksum = "9672cb0edeadf721484e298c0ed4dd70b0eaa3acaed5b4fd0bd73ca32e51d814"
 dependencies = [
  "ahash",
+ "appendlist",
  "base64",
  "fluent-uri",
  "idna 0.5.0",
  "once_cell",
  "percent-encoding",
  "regex",
  "regex-syntax",
```

### Comparing `bowtie_json_schema-2024.5.9/implementations/rust-boon/Dockerfile` & `bowtie_json_schema-2024.6.1/implementations/rust-boon/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/rust-boon/src/main.rs` & `bowtie_json_schema-2024.6.1/implementations/rust-boon/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/rust-jsonschema/Cargo.lock` & `bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "addr2line"
-version = "0.21.0"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a30b2e23b9e17a9f90641c7ab1549cd9b44f296d3ccbf309d2863cfe398a0cb"
+checksum = "6e4503c46a5c0c7844e948c9a4d6acd9f50cccb4de1c48eb9e291ea17470c678"
 dependencies = [
  "gimli",
 ]
 
 [[package]]
 name = "adler"
 version = "1.0.2"
@@ -99,17 +99,17 @@
 name = "autocfg"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
-version = "0.3.71"
+version = "0.3.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
+checksum = "17c6a35df3749d2e8bb1b7b21a976d82b15548788d2735b9d82f329268f71a11"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -357,17 +357,17 @@
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.28.1"
+version = "0.29.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
+checksum = "40ecd4077b5ae9fd2e9e169b102c6c330d0605168eb0e8bf79952b256dbefffd"
 
 [[package]]
 name = "hashbrown"
 version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
@@ -717,17 +717,17 @@
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "object"
-version = "0.32.2"
+version = "0.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
+checksum = "b8ec7ab813848ba4522158d5517a6093db1ded27575b070f4177b8d12b41db5e"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
@@ -948,26 +948,26 @@
 checksum = "61697e0a1c7e512e84a621326239844a24d8207b4669b41bc18b32ea5cbf988b"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.201"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
+checksum = "7253ab4de971e72fb7be983802300c30b5a7f0c2e56fab8abfc6a214307c0094"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.201"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
+checksum = "500cbc0ebeb6f46627f50f3f5811ccf6bf00643be300b4c3eabc0ef55dc5b5ba"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
```

### Comparing `bowtie_json_schema-2024.5.9/implementations/rust-jsonschema/Dockerfile` & `bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/rust-jsonschema/src/main.rs` & `bowtie_json_schema-2024.6.1/implementations/rust-jsonschema/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/scala-mjs-validator/Harness.scala` & `bowtie_json_schema-2024.6.1/implementations/scala-mjs-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/scala-mjs-validator/build.sbt` & `bowtie_json_schema-2024.6.1/implementations/scala-mjs-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/scala-rc-circe-json-validator/Harness.scala` & `bowtie_json_schema-2024.6.1/implementations/scala-rc-circe-json-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/scala-rc-circe-json-validator/build.sbt` & `bowtie_json_schema-2024.6.1/implementations/scala-rc-circe-json-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts` & `bowtie_json_schema-2024.6.1/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/tests/test_connectables.py` & `bowtie_json_schema-2024.6.1/tests/test_connectables.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import pytest
 
 from bowtie._connectables import Connectable, UnknownConnector
-from bowtie._containers import IMAGE_REPOSITORY, ConnectableImage
+from bowtie._containers import (
+    IMAGE_REPOSITORY,
+    ConnectableContainer,
+    ConnectableImage,
+)
 from bowtie._core import validator_registry
+from bowtie._direct_connectable import Direct
 
 validator = validator_registry().for_uri(
     "tag:bowtie.report,2024:connectables",
 )
 
 
 def test_explicit_image_with_repository():
@@ -106,7 +111,34 @@
     assert Connectable.from_str(id).to_terse() == "bar"
 
 
 def test_terse_implicit_image_no_repository():
     id = "bar"
     validator.validate(id)
     assert Connectable.from_str(id).to_terse() == "bar"
+
+
+def test_container_connectable():
+    id = "container:c7895a98f49d"
+    validator.validate(id)
+    connectable = Connectable.from_str(id)
+    assert connectable == Connectable(
+        id=id,
+        connector=ConnectableContainer(id="c7895a98f49d"),
+    )
+
+
+def test_direct_connectable_jsonschema():
+    id = "direct:jsonschema"
+    validator.validate(id)
+    connectable = Connectable.from_str(id)
+    assert connectable == Connectable(
+        id=id,
+        connector=Direct(id="jsonschema"),
+    )
+
+
+def test_direct_connectable_unknown():
+    id = "direct:foobar"
+    validator.validate(id)
+    with pytest.raises(ValueError, match="'jsonschema'"):
+        Connectable.from_str(id)
```

### Comparing `bowtie_json_schema-2024.5.9/tests/test_github.py` & `bowtie_json_schema-2024.6.1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/tests/test_hypothesis.py` & `bowtie_json_schema-2024.6.1/tests/test_hypothesis.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,16 +89,16 @@
 
 
 @given(strategies.report_data())
 @settings(suppress_health_check=[HealthCheck.too_slow], deadline=None)
 def test_report_data_generates_implementations_which_support_the_dialect(data):
     report = Report.from_input(data)
     assert all(
-        report.metadata.dialect in each.dialects
-        for each in report.implementations
+        report.metadata.dialect in implementation.dialects
+        for implementation in report.implementations.values()
     )
 
 
 @given(strategies.report_data())
 @settings(suppress_health_check=[HealthCheck.too_slow], deadline=None)
 def test_report_data_generates_boolean_schemas_only_when_supported(data):
     report = Report.from_input(data)
```

### Comparing `bowtie_json_schema-2024.5.9/tests/test_integration.py` & `bowtie_json_schema-2024.6.1/tests/test_integration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-from contextlib import asynccontextmanager
+from contextlib import asynccontextmanager, suppress
+from datetime import datetime, timedelta
 from io import BytesIO
 from pathlib import Path
 from pprint import pformat
-from textwrap import dedent, indent
+from textwrap import dedent
 import asyncio
 import json as _json
 import os
 import sys
 import tarfile
 
 from aiodocker.exceptions import DockerError
+from dateutil.parser import isoparse, parse as parse_datetime
+from dateutil.tz import tzlocal
+from dateutil.utils import default_tzinfo, within_delta
 from markdown_it import MarkdownIt
 from markdown_it.tree import SyntaxTreeNode
 import pexpect
 import pytest
 import pytest_asyncio
 
 from bowtie._cli import EX
@@ -331,17 +335,44 @@
     contents=r"""
     read -r request
     printf '{"implementation": {"name": "fake-js", "language": "javascript", "homepage": "urn:example", "issues": "urn:example", "source": "urn:example", "dialects": ["http://json-schema.org/draft-07/schema#"]}, "version": 1}\n'
     """,  # noqa: E501
 )
 
 
-def _failed(message, stderr):
-    indented = indent(stderr.decode(), prefix=" " * 2)
-    pytest.fail(f"{message}. stderr contained:\n\n{indented}")
+@pytest_asyncio.fixture
+async def envsonschema_container(docker, envsonschema):
+    config = dict(
+        Image=envsonschema,
+        OpenStdin=True,
+        HostConfig=dict(NetworkMode="none"),
+    )
+    container = await docker.containers.create(config=config)
+    await container.start()
+    yield f"container:{container.id}"
+
+    # FIXME: When this happens, it's likely due to #1187.
+    with suppress(DockerError):
+        await container.delete()
+
+
+@pytest_asyncio.fixture
+async def lintsonschema_container(docker, lintsonschema):
+    config = dict(
+        Image=lintsonschema,
+        OpenStdin=True,
+        HostConfig=dict(NetworkMode="none"),
+    )
+    container = await docker.containers.create(config=config)
+    await container.start()
+    yield f"container:{container.id}"
+
+    # FIXME: When this happens, it's likely due to #1187.
+    with suppress(DockerError):
+        await container.delete()
 
 
 @asynccontextmanager
 async def run(*args, **kwargs):
     async def _send(stdin=""):
         input = dedent(stdin).lstrip("\n")
         stdout, stderr = await bowtie("run", *args, stdin=input, **kwargs)
@@ -1504,14 +1535,41 @@
         "javascript",
         stdin=stdin + "\n",
     )
     assert (stdout, stderr) == (f"{tag('fake_js')}\n", "")
 
 
 @pytest.mark.asyncio
+async def test_filter_implementations_json(
+    envsonschema,
+    lintsonschema,
+    fake_js,
+):
+    jsonout, stderr = await bowtie(
+        "filter-implementations",
+        "-i",
+        envsonschema,
+        "-i",
+        lintsonschema,
+        "-i",
+        fake_js,
+        "-l",
+        "javascript",
+        "-d",
+        "7",
+        "--format",
+        "json",
+        json=True,
+    )
+    (await command_validator("filter-implementations")).validate(jsonout)
+    assert jsonout == [tag("fake_js")]
+    assert stderr == ""
+
+
+@pytest.mark.asyncio
 async def test_filter_dialects():
     stdout, stderr = await bowtie("filter-dialects")
     dialects_supported = "\n".join(
         [
             str(dialect.uri)
             for dialect in sorted(Dialect.known(), reverse=True)
         ],
@@ -1521,15 +1579,15 @@
 
 @pytest.mark.asyncio
 async def test_filter_dialects_latest_dialect():
     stdout, stderr = await bowtie(
         "filter-dialects",
         "-l",
     )
-    assert (stdout, stderr) == (f"{max(Dialect.known()).uri}\n", "")
+    assert (stdout, stderr) == (f"{Dialect.latest().uri}\n", "")
 
 
 @pytest.mark.asyncio
 async def test_filter_dialects_supporting_implementation(only_draft3):
     stdout, stderr = await bowtie("filter-dialects", "-i", only_draft3)
     assert (stdout, stderr) == (
         "http://json-schema.org/draft-03/schema#\n",
@@ -1658,19 +1716,18 @@
     )
     assert stderr == ""
     assert stdout == dedent(
         """\
         # Bowtie Failures Summary
 
         | Implementation | Skips | Errors | Failures |
-        |:-:|:-:|:-:|:-:|
+        |:---------------------:|:-:|:-:|:-:|
         | envsonschema (python) | 0 | 0 | 2 |
 
         **2 tests ran**
-
         """,
     )
 
 
 @pytest.mark.asyncio
 async def test_summary_failures_valid_markdown(envsonschema, tmp_path):
     tmp_path.joinpath("schema.json").write_text("{}")
@@ -2168,7 +2225,218 @@
         "-D",
         "2019",
         tmp_path / "schema.json",
         tmp_path / "instance.json",
     )
     report = Report.from_serialized(stdout.splitlines())
     assert report.metadata.dialect == Dialect.by_short_name()["draft2019-09"]
+
+
+@pytest.mark.asyncio
+async def test_statistics_pretty(envsonschema, always_valid):
+    raw = """
+        {"description":"one","schema":{"type": "integer"},"tests":[{"description":"valid:1","instance":12},{"description":"valid:0","instance":12.5}]}
+        {"description":"two","schema":{"type": "string"},"tests":[{"description":"crash:1","instance":"{}"}]}
+        {"description":"crash:1","schema":{"type": "number"},"tests":[{"description":"three","instance":"{}"}, {"description": "another", "instance": 37}]}
+        {"description":"four","schema":{"type": "array"},"tests":[{"description":"skip:message=foo","instance":""}]}
+        {"description":"skip:message=bar","schema":{"type": "boolean"},"tests":[{"description":"five","instance":""}]}
+        {"description":"six","schema":{"type": "array"},"tests":[{"description":"error:message=boom","instance":""}, {"description":"valid:0", "instance":12}]}
+        {"description":"error:message=boom","schema":{"type": "array"},"tests":[{"description":"seven","instance":""}]}
+    """  # noqa: E501
+    run_stdout, run_stderr = await bowtie(
+        "run",
+        "-i",
+        envsonschema,
+        "-i",
+        always_valid,
+        "-V",
+        stdin=dedent(raw.strip("\n")),
+    )
+
+    stdout, stderr = await bowtie(
+        "statistics",
+        "--format",
+        "pretty",
+        stdin=run_stdout,
+    )
+
+    prefix = "Ran on: "
+    ran_on_lines = [
+        line.removeprefix(prefix)
+        for line in stdout.splitlines()
+        if line.startswith(prefix)
+    ]
+    assert len(ran_on_lines) == 1, ("Couldn't find run date", stdout, stderr)
+    ran_on = default_tzinfo(parse_datetime(ran_on_lines[0]), tzlocal())
+
+    now, delta = datetime.now(tzlocal()), timedelta(minutes=1)
+    assert within_delta(ran_on, now, delta), f"{ran_on} is too far from {now}."
+
+    assert stdout == dedent(
+        f"""\
+        Dialect: Draft 2020-12
+        {prefix}{ran_on_lines[0]}
+
+        median: 0.65
+        mean: 0.65
+        """,
+    )
+    assert stderr == "", stderr
+
+
+@pytest.mark.asyncio
+@pytest.mark.json
+async def test_statistics_json(envsonschema, always_valid):
+    raw = """
+        {"description":"one","schema":{"type": "integer"},"tests":[{"description":"valid:1","instance":12},{"description":"valid:0","instance":12.5}]}
+        {"description":"two","schema":{"type": "string"},"tests":[{"description":"crash:1","instance":"{}"}]}
+        {"description":"crash:1","schema":{"type": "number"},"tests":[{"description":"three","instance":"{}"}, {"description": "another", "instance": 37}]}
+        {"description":"four","schema":{"type": "array"},"tests":[{"description":"skip:message=foo","instance":""}]}
+        {"description":"skip:message=bar","schema":{"type": "boolean"},"tests":[{"description":"five","instance":""}]}
+        {"description":"six","schema":{"type": "array"},"tests":[{"description":"error:message=boom","instance":""}, {"description":"valid:0", "instance":12}]}
+        {"description":"error:message=boom","schema":{"type": "array"},"tests":[{"description":"seven","instance":""}]}
+    """  # noqa: E501
+    run_stdout, run_stderr = await bowtie(
+        "run",
+        "-i",
+        envsonschema,
+        "-i",
+        always_valid,
+        "-V",
+        stdin=dedent(raw.strip("\n")),
+    )
+
+    jsonout, stderr = await bowtie(
+        "statistics",
+        "--format",
+        "json",
+        stdin=run_stdout,
+        json=True,
+    )
+
+    ran_on = isoparse(jsonout["ran_on"])
+    now, delta = datetime.now(tzlocal()), timedelta(minutes=1)
+    assert within_delta(ran_on, now, delta), f"{ran_on} is too far from {now}."
+
+    (await command_validator("statistics")).validate(jsonout)
+    assert jsonout == dict(
+        dialect="https://json-schema.org/draft/2020-12/schema",
+        ran_on=jsonout["ran_on"],
+        median=0.65,
+        mean=0.65,
+    )
+    assert stderr == "", stderr
+
+
+@pytest.mark.asyncio
+async def test_statistics_markdown(envsonschema, always_valid):
+    raw = """
+        {"description":"one","schema":{"type": "integer"},"tests":[{"description":"valid:1","instance":12},{"description":"valid:0","instance":12.5}]}
+        {"description":"two","schema":{"type": "string"},"tests":[{"description":"crash:1","instance":"{}"}]}
+        {"description":"crash:1","schema":{"type": "number"},"tests":[{"description":"three","instance":"{}"}, {"description": "another", "instance": 37}]}
+        {"description":"four","schema":{"type": "array"},"tests":[{"description":"skip:message=foo","instance":""}]}
+        {"description":"skip:message=bar","schema":{"type": "boolean"},"tests":[{"description":"five","instance":""}]}
+        {"description":"six","schema":{"type": "array"},"tests":[{"description":"error:message=boom","instance":""}, {"description":"valid:0", "instance":12}]}
+        {"description":"error:message=boom","schema":{"type": "array"},"tests":[{"description":"seven","instance":""}]}
+    """  # noqa: E501
+    run_stdout, run_stderr = await bowtie(
+        "run",
+        "-i",
+        envsonschema,
+        "-i",
+        always_valid,
+        "-V",
+        stdin=dedent(raw.strip("\n")),
+    )
+
+    stdout, stderr = await bowtie(
+        "statistics",
+        "--format",
+        "markdown",
+        stdin=run_stdout,
+    )
+
+    prefix = "### Ran on:"
+
+    ran_on_lines = [
+        line.removeprefix(prefix)
+        for line in stdout.splitlines()
+        if line.startswith(prefix)
+    ]
+    assert len(ran_on_lines) == 1, ("Couldn't find run date", stdout, stderr)
+    ran_on = default_tzinfo(parse_datetime(ran_on_lines[0]), tzlocal())
+
+    now, delta = datetime.now(tzlocal()), timedelta(minutes=1)
+    assert within_delta(ran_on, now, delta), f"{ran_on} is too far from {now}."
+
+    assert stdout == dedent(
+        f"""\
+        ## Dialect: Draft 2020-12
+
+        {prefix}{ran_on_lines[0]}
+
+        | Metric | Value |
+        |:------:|:----:|
+        | median | 0.65 |
+        |  mean  | 0.65 |
+        """,
+    )
+    assert stderr == "", stderr
+
+
+@pytest.mark.asyncio
+async def test_container_connectables(
+    lintsonschema_container,
+    envsonschema_container,
+    tmp_path,
+):
+    tmp_path.joinpath("schema.json").write_text("{}")
+    tmp_path.joinpath("instance.json").write_text("12")
+
+    stdout, stderr = await bowtie(
+        "validate",
+        "-i",
+        lintsonschema_container,
+        "-i",
+        envsonschema_container,
+        tmp_path / "schema.json",
+        tmp_path / "instance.json",
+        exit_code=0,
+    )
+    assert stderr == ""
+
+    report = Report.from_serialized(stdout.splitlines())
+    assert [
+        [test_results for _, test_results in results]
+        for _, results in report.cases_with_results()
+    ] == [
+        [
+            {
+                envsonschema_container: TestResult.INVALID,
+                lintsonschema_container: TestResult.VALID,
+            },
+        ],
+    ], stderr
+
+
+@pytest.mark.asyncio
+async def test_direct_connectable_python_jsonschema(tmp_path):
+    tmp_path.joinpath("schema.json").write_text("{}")
+    tmp_path.joinpath("instance.json").write_text("12")
+
+    stdout, stderr = await bowtie(
+        "validate",
+        "-i",
+        "direct:jsonschema",
+        tmp_path / "schema.json",
+        tmp_path / "instance.json",
+        exit_code=0,
+    )
+    assert stderr == ""
+
+    report = Report.from_serialized(stdout.splitlines())
+    assert [
+        [test_results for _, test_results in results]
+        for _, results in report.cases_with_results()
+    ] == [
+        [{"direct:jsonschema": TestResult.VALID}],
+    ], stderr
```

### Comparing `bowtie_json_schema-2024.5.9/tests/test_registry.py` & `bowtie_json_schema-2024.6.1/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/tests/test_report.py` & `bowtie_json_schema-2024.6.1/tests/test_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,28 @@
 TestCase.__test__ = False  # frigging py.test
 
 
 DIALECT = Dialect.by_alias()["2020"]
 FOO = ImplementationInfo(
     name="foo",
     language="blub",
-    image="foo",
     homepage=HOMEPAGE,
     issues=REPO / "issues",
     source=REPO,
     dialects=frozenset([DIALECT]),
 )
 BAR = ImplementationInfo(
     name="bar",
     language="crust",
-    image="x/baz",
     homepage=HOMEPAGE,
     issues=REPO / "issues",
     source=REPO,
     dialects=frozenset([DIALECT]),
 )
-FOO_RUN = RunMetadata(dialect=DIALECT, implementations=[FOO])
+FOO_RUN = RunMetadata(dialect=DIALECT, implementations={"foo": FOO})
 NO_FAIL_FAST = dict(did_fail_fast=False)
 
 
 def test_eq():
     data = (
         FOO_RUN.serializable(),
         SeqCase(
@@ -287,22 +285,23 @@
         NO_FAIL_FAST,
     ]
 
     assert Report.from_input(data) != Report.from_input(different_result)
 
 
 @given(dialect=known_dialects)
+@settings(suppress_health_check=[HealthCheck.too_slow])
 def test_ne_different_implementations(dialect):
     foo = RunMetadata(
         dialect=dialect,
-        implementations=[FOO],
+        implementations={"foo": FOO},
     )
     foo_and_bar = RunMetadata(
         dialect=dialect,
-        implementations=[FOO, BAR],
+        implementations={"foo": FOO, "x/baz": BAR},
     )
     data = [
         SeqCase(
             seq=1,
             case=TestCase(
                 description="foo",
                 schema={},
```

### Comparing `bowtie_json_schema-2024.5.9/tests/test_schemas.py` & `bowtie_json_schema-2024.6.1/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2024.6.1/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files 14% similar despite different names*

```diff
@@ -5,32 +5,24 @@
 from dataclasses import dataclass
 from pathlib import Path
 import io
 import json
 import os
 import sys
 
-from referencing.jsonschema import EMPTY_REGISTRY, specification_with
+from referencing.jsonschema import EMPTY_REGISTRY
 import jsonschema.validators
 import referencing_loaders as loaders
 
 SCHEMA_PATH = Path(os.environ.get("BOWTIE_SCHEMAS", "/schemas"))
 
 _schemas = loaders.from_path(SCHEMA_PATH)
-_REGISTRY = EMPTY_REGISTRY.with_resources(_schemas).crawl()
+REGISTRY = EMPTY_REGISTRY.with_resources(_schemas).crawl()
 ROOT_URI = "tag:bowtie.report,2023:ihop"
-METASCHEMA_ID = _REGISTRY.contents(ROOT_URI)["$schema"]
-SPECIFICATION = specification_with(METASCHEMA_ID)
-CURRENT_DIALECT = SPECIFICATION.create_resource(  # FIXME: wrong spec...
-    {
-        "$id": "tag:bowtie.report,2023:ihop:__dialect__",
-        "$ref": METASCHEMA_ID,
-    },
-)
-REGISTRY = CURRENT_DIALECT @ _REGISTRY
+METASCHEMA_ID = REGISTRY.contents(ROOT_URI)["$schema"]
 
 Validator = jsonschema.validators.validator_for(METASCHEMA_ID)
 
 
 @dataclass
 class Runner:
     _started: bool = False
```

### Comparing `bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/connectables.json` & `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/connectables.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9503968253968254%*

 * *Differences: {"'$defs'": "{'container': OrderedDict([('title', 'External Container'), ('description', 'An "*

 * *            "already running OCI container which Bowtie will connect to'), ('$anchor', "*

 * *            "'container'), ('pattern', '^container:*')]), 'direct': OrderedDict([('title', 'Direct "*

 * *            "Python Connection'), ('description', 'A directly importable (from Python) "*

 * *            "implementation which Bowtie will speak to'), ('$anchor', 'direct'), ('pattern', "*

 * *            "'^direct:[^.]*')])}",*

 * * "'oneOf […]*

```diff
@@ -1,9 +1,21 @@
 {
     "$defs": {
+        "container": {
+            "$anchor": "container",
+            "description": "An already running OCI container which Bowtie will connect to",
+            "pattern": "^container:*",
+            "title": "External Container"
+        },
+        "direct": {
+            "$anchor": "direct",
+            "description": "A directly importable (from Python) implementation which Bowtie will speak to",
+            "pattern": "^direct:[^.]*",
+            "title": "Direct Python Connection"
+        },
         "image": {
             "$anchor": "image",
             "description": "An OCI container image which Bowtie will spin up and manage",
             "pattern": "^image:*",
             "title": "Container Image"
         }
     },
@@ -20,14 +32,20 @@
             "title": "Implicit Image With Repository & Tag"
         },
         {
             "description": "A connectable with explicit connector.",
             "oneOf": [
                 {
                     "$ref": "#image"
+                },
+                {
+                    "$ref": "#container"
+                },
+                {
+                    "$ref": "#direct"
                 }
             ],
             "pattern": "^[^:]+:[^:]+(:[^:]+)?$",
             "title": "Fully Qualified Connectable"
         }
     ],
     "title": "Connectables",
```

### Comparing `bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/report.json` & `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/report.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/cli/info.json` & `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/info.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json` & `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json` & `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/io/v1.json` & `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/v1.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999479166666667%*

 * *Differences: {"'$defs'": '{\'case\': {\'properties\': {\'schema\': {\'$comment\': "We do no current validation '*

 * *            "here, as we may want to send schemas which truly aren't valid, but some day we likely "*

 * *            'will again.", delete: [\'$ref\']}}}}'}*

```diff
@@ -17,17 +17,16 @@
                     "description": "A collection of schemas (with URIs) which tests may reference (via $ref) and expect to be retrievable. They should be registered in whatever mechanism is expected by the implementation.",
                     "propertyNames": {
                         "format": "uri"
                     },
                     "type": "object"
                 },
                 "schema": {
-                    "$comment": "the URI used here is a sort of 'magic' URI set by Bowtie during runs, which will resolve to (effectively) the meta-schema for the current dialect being run by Bowtie. E.g. when running tests using the Draft 2020-12 dialect, the URI will resolve to the schema `{\"$ref\": \"https://json-schema.org/draft/2020-12/schema\"}`. This sort of dynamically set value is necessary, as schemas are supposed to be valid under the current dialect being spoken by Bowtie, but that's not known until runtime.",
+                    "$comment": "We do no current validation here, as we may want to send schemas which truly aren't valid, but some day we likely will again.",
                     "$id": "tag:bowtie.report,2024:ihop:schemaInCurrentDialect",
-                    "$ref": "tag:bowtie.report,2023:ihop:__dialect__",
                     "description": "A valid JSON Schema."
                 },
                 "tests": {
                     "description": "A set of related tests all using the same schema",
                     "items": {
                         "$ref": "tag:bowtie.report,2023:models:test"
                     },
```

### Comparing `bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json` & `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json` & `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json` & `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/models/group.json` & `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json` & `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/tests/fauxmplementations/lintsonschema/schemas/models/test.json` & `bowtie_json_schema-2024.6.1/tests/fauxmplementations/lintsonschema/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/.gitignore` & `bowtie_json_schema-2024.6.1/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -153,7 +153,8 @@
 
 # Cython debug symbols
 cython_debug/
 
 # Editor vomit
 .idea/
 .vscode/
+.vs/
```

### Comparing `bowtie_json_schema-2024.5.9/LICENSE` & `bowtie_json_schema-2024.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/README.rst` & `bowtie_json_schema-2024.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/hatch_build.py` & `bowtie_json_schema-2024.6.1/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.5.9/pyproject.toml` & `bowtie_json_schema-2024.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 ]
 dynamic = ["version"]
 dependencies = [
   "aiodocker",
   "attrs>=22.2.0",
   "diagnostic",
   "github3.py",
+  "httpx",
   "jsonschema>=4.19.0",
   "jsonschema_lexer",
   "referencing>=0.31.0",
   "referencing-loaders>=2024.5.2",
   "rich",
   "rich-click>=1.8.0",
   "rpds.py>=0.18.0",
```

### Comparing `bowtie_json_schema-2024.5.9/PKG-INFO` & `bowtie_json_schema-2024.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bowtie-json-schema
-Version: 2024.5.9
+Version: 2024.6.1
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://docs.bowtie.report/
 Project-URL: Homepage, https://bowtie.report/
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author-email: Julian Berman <Julian+bowtie@GrayVines.com>
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: File Formats :: JSON :: JSON Schema
 Requires-Python: >=3.10
 Requires-Dist: aiodocker
 Requires-Dist: attrs>=22.2.0
 Requires-Dist: diagnostic
 Requires-Dist: github3-py
+Requires-Dist: httpx
 Requires-Dist: jsonschema-lexer
 Requires-Dist: jsonschema>=4.19.0
 Requires-Dist: referencing-loaders>=2024.5.2
 Requires-Dist: referencing>=0.31.0
 Requires-Dist: rich
 Requires-Dist: rich-click>=1.8.0
 Requires-Dist: rpds-py>=0.18.0
```

