# Comparing `tmp/ape-solidity-0.7.3.tar.gz` & `tmp/ape-solidity-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-solidity-0.7.3.tar", last modified: Tue Apr 30 22:38:47 2024, max compression
+gzip compressed data, was "ape-solidity-0.8.0.tar", last modified: Sat Jun  1 03:52:19 2024, max compression
```

## Comparing `ape-solidity-0.7.3.tar` & `ape-solidity-0.8.0.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.825332 ape-solidity-0.7.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.813332 ape-solidity-0.7.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.813332 ape-solidity-0.7.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.813332 ape-solidity-0.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-30 22:38:47.829332 ape-solidity-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.813332 ape-solidity-0.7.3/ape_solidity/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/ape_solidity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/ape_solidity/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    46268 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/ape_solidity/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/ape_solidity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/ape_solidity/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 22:38:47.000000 ape-solidity-0.7.3/ape_solidity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.813332 ape-solidity-0.7.3/ape_solidity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-30 22:38:47.000000 ape-solidity-0.7.3/ape_solidity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-30 22:38:47.000000 ape-solidity-0.7.3/ape_solidity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 22:38:47.000000 ape-solidity-0.7.3/ape_solidity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 22:38:47.000000 ape-solidity-0.7.3/ape_solidity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-30 22:38:47.000000 ape-solidity-0.7.3/ape_solidity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 22:38:47.000000 ape-solidity-0.7.3/ape_solidity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-30 22:38:47.829332 ape-solidity-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/BrownieProject/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/BrownieProject/brownie-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/BrownieProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/BrownieProject/contracts/BrownieContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/BrownieStyleDependency/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/BrownieStyleDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/BrownieStyleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/BrownieStyleDependency/contracts/FailingContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/Dependency/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/Dependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/Dependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/Dependency/contracts/Dependency.sol
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/Dependency/contracts/OlderDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/Dependency/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/Dependency/contracts/subfolder_with_imports/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/DependencyOfDependency/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/DependencyOfDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/DependencyOfDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/ProjectWithinProject/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/ProjectWithinProject/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/ProjectWithinProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/ProjectWithinProject/contracts/Contract.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/VersionSpecifiedInConfig/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/VersionSpecifiedInConfig/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/VersionSpecifiedInConfig/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.821332 ape-solidity-0.7.3/tests/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/BuiltinErrorChecker.sol
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/CircularImport1.sol
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/CircularImport2.sol
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/CompilesOnce.sol
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/DifferentNameThanFile.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.821332 ape-solidity-0.7.3/tests/contracts/DirectoryWithExtension.sol/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/DirectoryWithExtension.sol/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/ExperimentalABIEncoderV2.sol
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/ImportOlderDependency.sol
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/ImportSourceWithEqualSignVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/ImportSourceWithNoPrefixVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/ImportingLessConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/Imports.sol
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/JustAStruct.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/LibraryFun.sol
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/MissingPragma.sol
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/MultipleDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/NumerousDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/OlderVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/RandomVyperFile.vy
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/RangedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/SpacesInPragma.sol
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/SpecificVersionNoPrefix.sol
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/SpecificVersionNoPrefix2.sol
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/SpecificVersionRange.sol
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/SpecificVersionWithEqualSign.sol
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/UseYearn.sol
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/VagueVersion.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.821332 ape-solidity-0.7.3/tests/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/subfolder/Relativecontract.sol
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.825332 ape-solidity-0.7.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/data/ImportingLessConstrainedVersionFlat.sol
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/data/ImportsFlattened.sol.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.809332 ape-solidity-0.7.3/tests/data/packages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.809332 ape-solidity-0.7.3/tests/data/packages/OpenZeppelin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.825332 ape-solidity-0.7.3/tests/data/packages/OpenZeppelin/v4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)   698486 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.825332 ape-solidity-0.7.3/tests/data/packages/OpenZeppelin/v4.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)   879002 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.809332 ape-solidity-0.7.3/tests/data/packages/vault/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.825332 ape-solidity-0.7.3/tests/data/packages/vault/master/
--rw-r--r--   0 runner    (1001) docker     (127)   167518 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/data/packages/vault/master/vault_main.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.825332 ape-solidity-0.7.3/tests/data/packages/vault/v0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)   167551 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/data/packages/vault/v0.4.5/vault.json
--rw-r--r--   0 runner    (1001) docker     (127)    32767 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.825332 ape-solidity-0.7.3/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/scripts/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)    25148 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.919383 ape-solidity-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.903383 ape-solidity-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.903383 ape-solidity-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.903383 ape-solidity-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-06-01 03:52:19.919383 ape-solidity-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.903383 ape-solidity-0.8.0/ape_solidity/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/ape_solidity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/ape_solidity/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48626 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/ape_solidity/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/ape_solidity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/ape_solidity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-01 03:52:19.000000 ape-solidity-0.8.0/ape_solidity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.907383 ape-solidity-0.8.0/ape_solidity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-06-01 03:52:19.000000 ape-solidity-0.8.0/ape_solidity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-06-01 03:52:19.000000 ape-solidity-0.8.0/ape_solidity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 03:52:19.000000 ape-solidity-0.8.0/ape_solidity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 03:52:19.000000 ape-solidity-0.8.0/ape_solidity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-06-01 03:52:19.000000 ape-solidity-0.8.0/ape_solidity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-01 03:52:19.000000 ape-solidity-0.8.0/ape_solidity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-01 03:52:19.919383 ape-solidity-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.907383 ape-solidity-0.8.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.907383 ape-solidity-0.8.0/tests/BrownieProject/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/BrownieProject/brownie-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.907383 ape-solidity-0.8.0/tests/BrownieProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/BrownieProject/contracts/BrownieContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.907383 ape-solidity-0.8.0/tests/Dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/Dependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.907383 ape-solidity-0.8.0/tests/Dependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/Dependency/contracts/Dependency.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/Dependency/contracts/OlderDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.907383 ape-solidity-0.8.0/tests/Dependency/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.907383 ape-solidity-0.8.0/tests/Dependency/contracts/subfolder_with_imports/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.907383 ape-solidity-0.8.0/tests/DependencyOfDependency/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/DependencyOfDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.907383 ape-solidity-0.8.0/tests/DependencyOfDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.907383 ape-solidity-0.8.0/tests/NonCompilingDependency/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/NonCompilingDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.907383 ape-solidity-0.8.0/tests/NonCompilingDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/NonCompilingDependency/contracts/CompilingContract.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/NonCompilingDependency/contracts/NonCompilingContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.907383 ape-solidity-0.8.0/tests/ProjectWithinProject/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/ProjectWithinProject/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.911383 ape-solidity-0.8.0/tests/ProjectWithinProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/ProjectWithinProject/contracts/Contract.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.911383 ape-solidity-0.8.0/tests/VersionSpecifiedInConfig/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/VersionSpecifiedInConfig/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.911383 ape-solidity-0.8.0/tests/VersionSpecifiedInConfig/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.915383 ape-solidity-0.8.0/tests/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/BuiltinErrorChecker.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/CircularImport1.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/CircularImport2.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/CompilesOnce.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/ContractUsingLibraryNotInSameSource.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/DifferentNameThanFile.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.915383 ape-solidity-0.8.0/tests/contracts/DirectoryWithExtension.sol/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/DirectoryWithExtension.sol/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/ExperimentalABIEncoderV2.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/ImportOlderDependency.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/ImportSourceWithEqualSignVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/ImportSourceWithNoPrefixVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/ImportingLessConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/Imports.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/JustAStruct.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/LibraryFun.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/MissingPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/MultipleDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/NumerousDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/OlderVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/RandomVyperFile.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/RangedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/SpacesInPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/SpecificVersionNoPrefix.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/SpecificVersionNoPrefix2.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/SpecificVersionRange.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/SpecificVersionWithEqualSign.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/UseYearn.sol
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/VagueVersion.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.915383 ape-solidity-0.8.0/tests/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/subfolder/Relativecontract.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.915383 ape-solidity-0.8.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/data/ImportingLessConstrainedVersionFlat.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/data/ImportsFlattened.sol.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.899383 ape-solidity-0.8.0/tests/data/packages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.899383 ape-solidity-0.8.0/tests/data/packages/OpenZeppelin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.915383 ape-solidity-0.8.0/tests/data/packages/OpenZeppelin/v4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)   698486 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.915383 ape-solidity-0.8.0/tests/data/packages/OpenZeppelin/v4.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)   879002 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.899383 ape-solidity-0.8.0/tests/data/packages/vault/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.919383 ape-solidity-0.8.0/tests/data/packages/vault/master/
+-rw-r--r--   0 runner    (1001) docker     (127)   167518 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/data/packages/vault/master/vault_main.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.919383 ape-solidity-0.8.0/tests/data/packages/vault/v0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)   167551 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/data/packages/vault/v0.4.5/vault.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32767 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:52:19.919383 ape-solidity-0.8.0/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/scripts/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27054 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-06-01 03:51:30.000000 ape-solidity-0.8.0/tests/test_integration.py
```

### Comparing `ape-solidity-0.7.3/.github/ISSUE_TEMPLATE/bug.md` & `ape-solidity-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/.github/ISSUE_TEMPLATE/feature.md` & `ape-solidity-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/.github/ISSUE_TEMPLATE/work-item.md` & `ape-solidity-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/.github/release-drafter.yml` & `ape-solidity-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/.github/workflows/codeql.yml` & `ape-solidity-0.8.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/.github/workflows/prtitle.yaml` & `ape-solidity-0.8.0/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/.github/workflows/publish.yaml` & `ape-solidity-0.8.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/.github/workflows/stale-prs.yml` & `ape-solidity-0.8.0/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/.github/workflows/test.yaml` & `ape-solidity-0.8.0/.github/workflows/test.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 # TODO: Replace with macos-latest when works again.
                 #   https://github.com/actions/setup-python/issues/808
                 os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, '3.10', '3.11', '3.12']
+                python-version: [3.9, '3.10', '3.11', '3.12']
 
         env:
           GITHUB_ACCESS_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
         steps:
         - uses: actions/checkout@v4
```

### Comparing `ape-solidity-0.7.3/.gitignore` & `ape-solidity-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/.pre-commit-config.yaml` & `ape-solidity-0.8.0/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -26,12 +26,12 @@
     -   id: mypy
         additional_dependencies: [types-requests, types-setuptools, pydantic, types-pkg-resources]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
     -   id: mdformat
-        additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
+        additional_dependencies: [mdformat-gfm, mdformat-frontmatter, mdformat-pyproject]
 
 
 default_language_version:
     python: python3
```

### Comparing `ape-solidity-0.7.3/CONTRIBUTING.md` & `ape-solidity-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/LICENSE` & `ape-solidity-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/PKG-INFO` & `ape-solidity-0.8.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,14 @@
-Metadata-Version: 2.1
-Name: ape-solidity
-Version: 0.7.3
-Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
-Home-page: https://github.com/ApeWorX/ape-solidity
-Author: ApeWorX Ltd.
-Author-email: admin@apeworx.io
-License: Apache-2.0
-Keywords: ethereum
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8,<4
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: doc
-Provides-Extra: release
-Provides-Extra: dev
-License-File: LICENSE
-
 # Quick Start
 
 Compile Solidity contracts.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
 
@@ -88,40 +58,40 @@
 ```yaml
 solidity:
   evm_version: paris
 ```
 
 ### Dependency Mapping
 
-To configure import remapping, use your project's `ape-config.yaml` file:
-
-```yaml
-solidity:
-  import_remapping:
-    - "@openzeppelin=path/to/open_zeppelin/contracts"
-```
-
-If you are using the `dependencies:` key in your `ape-config.yaml`, `ape` can automatically
-search those dependencies for the path.
+By default, `ape-solidity` knows to look at installed dependencies for potential remapping-values and will use those when it notices you are importing them.
+For example, if you are using dependencies like:
 
 ```yaml
 dependencies:
-  - name: OpenZeppelin
+  - name: openzeppelin
     github: OpenZeppelin/openzeppelin-contracts
     version: 4.4.2
-
-solidity:
-  import_remapping:
-    - "@openzeppelin=OpenZeppelin/4.4.2"
 ```
 
-Once you have your dependencies configured, you can import packages using your import keys:
+And your source files import from `openzeppelin` this way:
 
 ```solidity
-import "@openzeppelin/token/ERC721/ERC721.sol";
+import "@openzeppelin/contracts/token/ERC721/ERC721.sol";
+```
+
+Ape knows how to resolve the `@openzeppelin` value and find the correct source.
+
+If you want to override this behavior or add new remappings that are not dependencies, you can add them to your `ape-config.yaml` under the `solidity:` key.
+For example, let's say you have downloaded `openzeppelin` somewhere and do not have it installed in Ape.
+You can map to your local install of `openzeppelin` this way:
+
+```yaml
+solidity:
+  import_remapping:
+    - "@openzeppelin=path/to/openzeppelin"
 ```
 
 ### Library Linking
 
 To compile contracts that use libraries, you need to add the libraries first.
 Use the `add_library()` method from the `ape-solidity` compiler class to add the library.
 A typical flow is:
```

### Comparing `ape-solidity-0.7.3/ape_solidity/compiler.py` & `ape-solidity-0.8.0/ape_solidity/compiler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 import os
 import re
+from collections.abc import Iterable, Iterator
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Sequence, Set, Tuple, Type, Union, cast
+from typing import Any, Optional, Union
 
 from ape.api import CompilerAPI, PluginConfig
 from ape.contracts import ContractInstance
-from ape.exceptions import CompilerError, ConfigError, ContractLogicError
+from ape.exceptions import CompilerError, ConfigError, ContractLogicError, ProjectError
 from ape.logging import logger
+from ape.managers.project import ProjectManager
 from ape.types import AddressType, ContractType
-from ape.utils import cached_property, get_package_version, get_relative_path
+from ape.utils import cached_property, get_full_extension, get_relative_path
+from ape.version import version
 from eth_pydantic_types import HexBytes
 from eth_utils import add_0x_prefix, is_0x_prefixed
-from ethpm_types import PackageManifest
 from ethpm_types.source import Compiler, Content
 from packaging.specifiers import SpecifierSet
 from packaging.version import Version
+from pydantic import model_validator
 from requests.exceptions import ConnectionError
 from solcx import (
     compile_source,
     compile_standard,
     get_installable_solc_versions,
     get_installed_solc_versions,
     install_solc,
 )
 from solcx.exceptions import SolcError
 from solcx.install import get_executable
 
 from ape_solidity._utils import (
     OUTPUT_SELECTION,
     Extension,
-    ImportRemapping,
-    ImportRemappingBuilder,
     add_commit_hash,
     get_import_lines,
     get_pragma_spec_from_path,
     get_pragma_spec_from_str,
+    get_versions_can_use,
     load_dict,
     select_version,
     strip_commit_hash,
-    verify_contract_filepaths,
 )
 from ape_solidity.exceptions import (
     RUNTIME_ERROR_CODE_PREFIX,
     RUNTIME_ERROR_MAP,
-    IncorrectMappingFormatError,
     RuntimeErrorType,
     RuntimeErrorUnion,
     SolcCompileError,
     SolcInstallError,
 )
 
 # Define a regex pattern that matches import statements
@@ -56,81 +56,121 @@
     r"import\s+((.*?)(?=;)|[\s\S]*?from\s+(.*?)(?=;));\s", flags=re.MULTILINE
 )
 LICENSES_PATTERN = re.compile(r"(// SPDX-License-Identifier:\s*([^\n]*)\s)")
 VERSION_PRAGMA_PATTERN = re.compile(r"pragma solidity[^;]*;")
 DEFAULT_OPTIMIZATION_RUNS = 200
 
 
+class ImportRemapping(PluginConfig):
+    """
+    A remapped import set in the config.
+    """
+
+    @model_validator(mode="before")
+    def validate_str(cls, value):
+        if isinstance(value, str):
+            parts = value.split("=")
+            return {"key": parts[0], "value": parts[1]}
+
+        return value
+
+    """
+    The key of the remapping, such as ``@openzeppelin``.
+    """
+    key: str
+
+    """
+    The value to use in place of the key,
+    such as ``path/somewhere/else``.
+    """
+    value: str
+
+    def __str__(self) -> str:
+        return f"{self.key}={self.value}"
+
+    def __eq__(self, other):
+        if isinstance(other, str):
+            return str(self) == other
+
+        return super().__eq__(other)
+
+
 class SolidityConfig(PluginConfig):
     """
-    Configure the Solidity plugin.
+    Configure the ape-solidity plugin.
     """
 
-    import_remapping: List[str] = []
+    import_remapping: list[ImportRemapping] = []
     """
-    Configure re-mappings using a ``=`` separated-str,
-    e.g. ``"@import_name=path/to/dependency"``.
+    Custom remappings as a key value map..
+    Note: You do not need to specify dependencies here.
     """
 
     optimize: bool = True
     """
-    Set to ``False`` to disable compiler-optimizations.
+    Compile with optimization. Defaults to ``True``.
     """
 
     version: Optional[str] = None
     """
-    The compiler version to use. Defaults to selecting
-    the best version(s) it can for each file-set.
+    Hardcode a Solidity version to use. When not set,
+    ape-solidity attempts to use the best version(s)
+    available.
     """
 
     evm_version: Optional[str] = None
     """
-    The EVM version (fork) to use. Defaults to letting
-    the compiler decide.
+    Compile targeting this EVM version.
     """
 
     via_ir: Optional[bool] = None
     """
     Set to ``True`` to turn on compilation mode via the IR.
     Defaults to ``None`` which does not pass the flag to
     the compiler (same as ``False``).
     """
 
 
+def _get_flattened_source(path: Path, name: Optional[str] = None) -> str:
+    name = name or path.name
+    result = f"// File: {name}\n"
+    result += path.read_text() + "\n"
+    return result
+
+
 class SolidityCompiler(CompilerAPI):
-    _import_remapping_hash: Optional[int] = None
-    _cached_project_path: Optional[Path] = None
-    _cached_import_map: Dict[str, str] = {}
-    _libraries: Dict[str, Dict[str, AddressType]] = {}
-    _contracts_needing_libraries: Set[Path] = set()
+    """
+    The implementation of the ape-solidity Compiler class.
+    Implements all methods in :class:`~ape.api.compilers.CompilerAPI`.
+    Compiles ``.sol`` files into ``ContractTypes`` for usage in the
+    Ape framework.
+    """
+
+    # Libraries adding for linking. See `add_library` method.
+    _libraries: dict[str, dict[str, AddressType]] = {}
 
     @property
     def name(self) -> str:
         return "solidity"
 
     @property
-    def config(self) -> SolidityConfig:
-        return cast(SolidityConfig, self.config_manager.get_config(self.name))
-
-    @property
-    def libraries(self) -> Dict[str, Dict[str, AddressType]]:
+    def libraries(self) -> dict[str, dict[str, AddressType]]:
         return self._libraries
 
     @cached_property
-    def available_versions(self) -> List[Version]:
-        # NOTE: Package version should already be included in available versions
+    def available_versions(self) -> list[Version]:
         try:
             return get_installable_solc_versions()
         except ConnectionError:
             # Compiling offline
             logger.warning("Internet connection required to fetch installable Solidity versions.")
             return []
 
     @property
-    def installed_versions(self) -> List[Version]:
+    def installed_versions(self) -> list[Version]:
         """
         Returns a lis of installed version WITHOUT their
         commit hashes.
         """
         return get_installed_solc_versions()
 
     @property
@@ -146,422 +186,429 @@
     def latest_installed_version(self) -> Optional[Version]:
         """
         Returns the highest version of all the installed versions.
         If ``solc`` is not installed at all, returns ``None``.
         """
         return _try_max(self.installed_versions)
 
-    @property
-    def _settings_version(self) -> Optional[Version]:
+    def _get_configured_version(
+        self, project: Optional[ProjectManager] = None
+    ) -> Optional[Version]:
         """
         A helper property that gets, verifies, and installs (if needed)
-        the version specified in the settings.
+        the version specified in the config.
         """
-        if not (version := self.settings.version):
+        pm = project or self.local_project
+        config = self.get_config(project=pm)
+        if not (version := config.version):
             return None
 
         installed_versions = self.installed_versions
         specified_commit_hash = "+" in version
         base_version = strip_commit_hash(version)
         if base_version not in installed_versions:
             install_solc(base_version, show_progress=True)
 
         settings_version = add_commit_hash(base_version)
-        if specified_commit_hash:
-            if settings_version != version:
-                raise ConfigError(
-                    f"Commit hash from settings version {version} "
-                    f"differs from installed: {settings_version}"
-                )
+        if specified_commit_hash and settings_version != version:
+            raise ConfigError(
+                f"Commit hash from settings version {version} "
+                f"differs from installed: {settings_version}"
+            )
 
         return settings_version
 
     @cached_property
     def _ape_version(self) -> Version:
-        version_str = get_package_version("eth-ape").split(".dev")[0].strip()
-        return Version(version_str)
+        return Version(version.split(".dev")[0].strip())
 
-    def add_library(self, *contracts: ContractInstance):
+    def add_library(self, *contracts: ContractInstance, project: Optional[ProjectManager] = None):
         """
         Set a library contract type address. This is useful when deploying a library
         in a local network and then adding the address afterward. Now, when
         compiling again, it will use the new address.
 
         Args:
-            contracts (``ContractInstance``): The deployed library contract(s).
+            *contracts (``ContractInstance``): The deployed library contract(s).
+            project (Optional[ProjectManager]): The project using the library.
         """
-
+        pm = project or self.local_project
         for contract in contracts:
-            source_id = contract.contract_type.source_id
-            if not source_id:
+            if not (source_id := contract.contract_type.source_id):
                 raise CompilerError("Missing source ID.")
-
-            name = contract.contract_type.name
-            if not name:
+            elif not (name := contract.contract_type.name):
                 raise CompilerError("Missing contract type name.")
 
             self._libraries[source_id] = {name: contract.address}
+            path = pm.path / source_id
+            if not path.is_file():
+                return
+
+            # Recompile the same source, in case contracts were in there
+            # that required the libraries.
+            contract_types = {
+                ct.name: ct for ct in self.compile((path,), project=project) if ct.name
+            }
+            if contract_types:
+                all_types = {**pm.manifest.contract_types, **contract_types}
+                pm.update_manifest(contract_types=all_types)
 
-        if self._contracts_needing_libraries:
-            # TODO: Only attempt to re-compile contacts that use the given libraries.
-            # Attempt to re-compile contracts that needed libraries.
-            try:
-                self.project_manager.load_contracts(
-                    [
-                        self.config_manager.contracts_folder / s
-                        for s in self._contracts_needing_libraries
-                    ],
-                    use_cache=False,
-                )
-            except CompilerError as err:
-                logger.error(
-                    f"Failed when trying to re-compile contracts requiring libraries.\n{err}"
-                )
-
-            self._contracts_needing_libraries = set()
-
-    def get_versions(self, all_paths: Sequence[Path]) -> Set[str]:
+    def get_versions(self, all_paths: Iterable[Path]) -> set[str]:
+        _validate_can_compile(all_paths)
         versions = set()
         for path in all_paths:
             # Make sure we have the compiler available to compile this
             if version_spec := get_pragma_spec_from_path(path):
                 if selected_version := select_version(version_spec, self.available_versions):
                     versions.add(selected_version.base_version)
 
         return versions
 
-    def get_import_remapping(self, base_path: Optional[Path] = None) -> Dict[str, str]:
+    def get_import_remapping(self, project: Optional[ProjectManager] = None) -> dict[str, str]:
         """
         Config remappings like ``'@import_name=path/to/dependency'`` parsed here
         as ``{'@import_name': 'path/to/dependency'}``.
 
         Returns:
-            Dict[str, str]: Where the key is the import name, e.g. ``"@openzeppelin/contracts"`
+            Dict[str, str]: Where the key is the import name, e.g. ``"@openzeppelin"`
             and the value is a stringified relative path (source ID) of the cached contract,
-            e.g. `".cache/OpenZeppelin/v4.4.2".
+            e.g. `".cache/openzeppelin/4.4.2".
         """
-        base_path = base_path or self.project_manager.contracts_folder
-        if not (remappings := self.settings.import_remapping):
-            return {}
-
-        elif not isinstance(remappings, (list, tuple)) or not isinstance(remappings[0], str):
-            raise IncorrectMappingFormatError()
-
-        # We use these helpers to transform the values configured
-        # to values matching files in the compiler cache folder.
-        builder = ImportRemappingBuilder(
-            get_relative_path(self.project_manager.compiler_cache_folder, base_path)
-        )
-        packages_cache = self.config_manager.packages_folder
-
-        # Here we hash and validate if there were changes to remappings.
-        # If there were, we continue, else return the cached value for
-        # performance reasons.
-        remappings_tuple = tuple(remappings)
-        if (
-            self._import_remapping_hash
-            and self._import_remapping_hash == hash(remappings_tuple)
-            and self.project_manager.compiler_cache_folder.is_dir()
-        ):
-            return self._cached_import_map
+        pm = project or self.local_project
+        prefix = f"{get_relative_path(pm.contracts_folder, pm.path)}"
 
-        # NOTE: Dependencies are only extracted if calling for the first.
-        # Likely, this was done already before this point, unless
-        # calling python methods manually. However, dependencies MUST be
-        # fully loaded to properly evaluate remapping paths.
-        dependencies = self.project_manager.load_dependencies()
-
-        for item in remappings:
-            remapping_obj = ImportRemapping(entry=item, packages_cache=packages_cache)
-            builder.add_entry(remapping_obj)
-            package_id = remapping_obj.package_id
-
-            # Handle missing version ID
-            if len(package_id.parts) == 1:
-                if package_id.name not in dependencies or len(dependencies[package_id.name]) == 0:
-                    logger.warning(f"Missing dependency '{package_id.name}'.")
-                    continue
-
-                elif len(dependencies[package_id.name]) != 1:
-                    logger.warning("version ID missing and unable to evaluate version.")
-                    continue
+        specified = pm.dependencies.install()
 
-                version_id = next(iter(dependencies[package_id.name]))
-                logger.debug(f"for {package_id.name} version ID missing, using {version_id}")
-                package_id = package_id / version_id
-
-            data_folder_cache = packages_cache / package_id
-
-            # Re-build a downloaded dependency manifest into the .cache directory for imports.
-            sub_contracts_cache = self.project_manager.compiler_cache_folder / package_id
-            if not sub_contracts_cache.is_dir() or not list(sub_contracts_cache.iterdir()):
-                cached_manifest_file = data_folder_cache / f"{remapping_obj.name}.json"
-                if not cached_manifest_file.is_file():
-                    logger.debug(f"Unable to find dependency '{package_id}'.")
-
-                else:
-                    manifest = PackageManifest.model_validate_json(cached_manifest_file.read_text())
-                    self._add_dependencies(manifest, sub_contracts_cache, builder)
-
-        # Update cache and hash
-        self._cached_project_path = self.project_manager.path
-        self._cached_import_map = builder.import_map
-        self._import_remapping_hash = hash(remappings_tuple)
-        return builder.import_map
-
-    def _add_dependencies(
-        self, manifest: PackageManifest, cache_dir: Path, builder: ImportRemappingBuilder
-    ):
-        if not cache_dir.is_dir():
-            cache_dir.mkdir(parents=True)
-
-        sources = manifest.sources or {}
+        # Ensure .cache folder is ready-to-go.
+        cache_folder = pm.contracts_folder / ".cache"
+        cache_folder.mkdir(exist_ok=True, parents=True)
+
+        # Start with explicitly configured remappings.
+        cfg_remappings: dict[str, str] = {
+            m.key: m.value for m in pm.config.solidity.import_remapping
+        }
+        key_map: dict[str, str] = {}
 
-        for source_name, src in sources.items():
-            cached_source = cache_dir / source_name
+        def get_cache_id(dep) -> str:
+            return os.path.sep.join((prefix, ".cache", dep.name, dep.version))
 
-            if cached_source.is_file():
-                # Source already present
+        def unpack(dep):
+            # Ensure the dependency is installed.
+            try:
+                dep.project
+            except ProjectError:
+                # Try to compile anyway.
+                # Let the compiler fail on its own.
+                return
+
+            for unpacked_dep in dep.unpack(pm.contracts_folder / ".cache"):
+                _key = key_map.get(unpacked_dep.name, f"@{unpacked_dep.name}")
+                if _key not in remapping:
+                    remapping[_key] = get_cache_id(unpacked_dep)
+                # else, was specified or configured more appropriately.
+
+        remapping: dict[str, str] = {}
+        for key, value in cfg_remappings.items():
+            # Check if legacy-style and still accept it.
+            parts = value.split(os.path.sep)
+            name = parts[0]
+            _version = None
+            if len(parts) > 2:
+                # Clearly, not pointing at a dependency.
+                remapping[key] = value
                 continue
 
-            # NOTE: Cached source may included sub-directories.
-            cached_source.parent.mkdir(parents=True, exist_ok=True)
-            if src.content:
-                cached_source.touch()
-                cached_source.write_text(str(src.content))
-
-        # Add dependency remapping that may be needed.
-        for compiler in manifest.compilers or []:
-            settings = compiler.settings or {}
-            settings_map = settings.get("remappings") or []
-            remapping_list = [
-                ImportRemapping(entry=x, packages_cache=self.config_manager.packages_folder)
-                for x in settings_map
-            ]
-            for remapping in remapping_list:
-                builder.add_entry(remapping)
-
-        # Locate the dependency in the .ape packages cache
-        dependencies = manifest.dependencies or {}
-        packages_dir = self.config_manager.packages_folder
-        for dependency_package_name, uri in dependencies.items():
-            uri_str = str(uri)
-            if "://" in uri_str:
-                uri_str = "://".join(uri_str.split("://")[1:])  # strip off scheme
-
-            dependency_name = str(dependency_package_name)
-            if str(self.config_manager.packages_folder) in uri_str:
-                # Using a local dependency
-                version = "local"
-            else:
-                # Check for GitHub-style dependency
-                match_checks = (r".*/releases/tag/(v?[\d|.]+)", r".*/tree/(v?[\w|.|\d]+)")
-                version = None
-                for check in match_checks:
-                    version_match = re.match(check, str(uri_str))
-                    if version_match:
-                        version = version_match.groups()[0]
-                        if not version.startswith("v") and version[0].isnumeric():
-                            version = f"v{version}"
-
-                        break
+            elif len(parts) == 2:
+                _version = parts[1]
 
-            # Find matching package
-            for package in packages_dir.iterdir():
-                if package.name.replace("_", "-").lower() == dependency_name:
-                    dependency_name = str(package.name)
-                    break
+            if _version is None:
+                matching_deps = [d for d in pm.dependencies.installed if d.name == name]
+                if len(matching_deps) == 1:
+                    _version = matching_deps[0].version
+                else:
+                    # Not obvious if it is pointing at one of these dependencies.
+                    remapping[key] = value
+                    continue
 
-            dependency_root_path = self.config_manager.packages_folder / Path(dependency_name)
+            # Dependency found. Map to it using the provider key.
+            dependency = pm.dependencies.get_dependency(name, _version)
+            key_map[dependency.name] = key
+            unpack(dependency)
+
+        # Add auto-remapped dependencies.
+        # (Meaning, the dependencies are specified but their remappings
+        # are not, so we auto-generate default ones).
+        for dependency in specified:
+            unpack(dependency)
 
-            if version is None:
-                version_dirs = [
-                    d
-                    for d in list(dependency_root_path.iterdir())
-                    if d.is_dir() and not d.name.startswith(".")
-                ]
-                if len(version_dirs) == 1:
-                    # Use the only existing version.
-                    version = version_dirs[0].name
-
-                elif (dependency_root_path / "local").is_dir():
-                    # If not specified, and local exists, use local by default.
-                    version = "local"
+        return remapping
 
-                else:
-                    options = ", ".join([x.name for x in dependency_root_path.iterdir()])
-                    raise CompilerError(
-                        f"Ambiguous dependency version. "
-                        f"Please specify. Available versions: '{options}'."
-                    )
+    def get_compiler_settings(
+        self, contract_filepaths: Iterable[Path], project: Optional[ProjectManager] = None, **kwargs
+    ) -> dict[Version, dict]:
+        pm = project or self.local_project
+        _validate_can_compile(contract_filepaths)
+        remapping = self.get_import_remapping(project=pm)
+        imports = self.get_imports_from_remapping(contract_filepaths, remapping, project=pm)
+        return self._get_settings_from_imports(contract_filepaths, imports, remapping, project=pm)
 
-            dependency_path = dependency_root_path / version / f"{dependency_name}.json"
-            if dependency_path.is_file():
-                sub_manifest = PackageManifest.model_validate_json(dependency_path.read_text())
-                dep_id = Path(dependency_name) / version
-                if dep_id not in builder.dependencies_added:
-                    builder.dependencies_added.add(dep_id)
-                    self._add_dependencies(
-                        sub_manifest,
-                        builder.contracts_cache / dep_id,
-                        builder,
-                    )
+    def _get_settings_from_imports(
+        self,
+        contract_filepaths: Iterable[Path],
+        import_map: dict[str, list[str]],
+        remappings: dict[str, str],
+        project: Optional[ProjectManager] = None,
+    ):
+        pm = project or self.local_project
+        files_by_solc_version = self.get_version_map_from_imports(
+            contract_filepaths, import_map, project=pm
+        )
+        return self._get_settings_from_version_map(files_by_solc_version, remappings, project=pm)
 
-    def get_compiler_settings(
-        self, contract_filepaths: Sequence[Path], base_path: Optional[Path] = None
-    ) -> Dict[Version, Dict]:
-        base_path = base_path or self.config_manager.contracts_folder
-        files_by_solc_version = self.get_version_map(contract_filepaths, base_path=base_path)
-        if not files_by_solc_version:
+    def _get_settings_from_version_map(
+        self,
+        version_map: dict,
+        import_remappings: dict[str, str],
+        project: Optional[ProjectManager] = None,
+        **kwargs,
+    ) -> dict[Version, dict]:
+        pm = project or self.local_project
+        if not version_map:
             return {}
 
-        import_remappings = self.get_import_remapping(base_path=base_path)
-        settings: Dict = {}
-        for solc_version, sources in files_by_solc_version.items():
-            version_settings: Dict[str, Union[Any, List[Any]]] = {
-                "optimizer": {"enabled": self.settings.optimize, "runs": DEFAULT_OPTIMIZATION_RUNS},
+        config = self.get_config(project=pm)
+        settings: dict = {}
+        for solc_version, sources in version_map.items():
+            version_settings: dict[str, Union[Any, list[Any]]] = {
+                "optimizer": {"enabled": config.optimize, "runs": DEFAULT_OPTIMIZATION_RUNS},
                 "outputSelection": {
-                    str(get_relative_path(p, base_path)): {"*": OUTPUT_SELECTION, "": ["ast"]}
-                    for p in sources
+                    str(get_relative_path(p, pm.path)): {"*": OUTPUT_SELECTION, "": ["ast"]}
+                    for p in sorted(sources)
                 },
+                **kwargs,
             }
-            if remappings_used := self._get_used_remappings(
-                sources, remappings=import_remappings, base_path=base_path
-            ):
+            if remappings_used := self._get_used_remappings(sources, import_remappings, project=pm):
                 remappings_str = [f"{k}={v}" for k, v in remappings_used.items()]
 
                 # Standard JSON input requires remappings to be sorted.
                 version_settings["remappings"] = sorted(remappings_str)
 
-            if evm_version := self.settings.evm_version:
+            if evm_version := config.evm_version:
                 version_settings["evmVersion"] = evm_version
 
-            if solc_version >= Version("0.7.5") and self.settings.via_ir is not None:
-                version_settings["viaIR"] = self.settings.via_ir
+            if solc_version >= Version("0.7.5") and config.via_ir is not None:
+                version_settings["viaIR"] = config.via_ir
 
             settings[solc_version] = version_settings
 
             # TODO: Filter out libraries that are not used for this version.
             if libs := self.libraries:
                 version_settings["libraries"] = libs
 
         return settings
 
     def _get_used_remappings(
-        self, sources, remappings: Dict[str, str], base_path: Optional[Path] = None
-    ) -> Dict[str, str]:
-        base_path = base_path or self.project_manager.contracts_folder
-        remappings = remappings or self.get_import_remapping(base_path=base_path)
+        self,
+        sources: Iterable[Path],
+        remappings: dict[str, str],
+        project: Optional[ProjectManager] = None,
+    ) -> dict[str, str]:
+        pm = project or self.local_project
         if not remappings:
             # No remappings used at all.
             return {}
 
-        relative_cache = get_relative_path(self.project_manager.compiler_cache_folder, base_path)
+        cache_path = (
+            f"{get_relative_path(pm.contracts_folder.absolute(), pm.path)}{os.path.sep}.cache"
+        )
 
         # Filter out unused import remapping.
-        return {
-            k: v
-            for source in (
-                x
-                for sourceset in self.get_imports(list(sources), base_path=base_path).values()
-                for x in sourceset
-                if str(relative_cache) in x
-            )
-            for parent_key in (
-                os.path.sep.join(source.split(os.path.sep)[:3]) for source in [source]
-            )
-            for k, v in [(k, v) for k, v in remappings.items() if parent_key in v]
-        }
+        result = {}
+        sources = list(sources)
+        imports = self.get_imports(sources, project=pm).values()
+
+        for source_list in imports:
+            for src in source_list:
+                if not src.startswith(cache_path):
+                    continue
+
+                parent_key = os.path.sep.join(src.split(os.path.sep)[:3])
+                for k, v in remappings.items():
+                    if parent_key in v:
+                        result[k] = v
+
+        return result
 
     def get_standard_input_json(
-        self, contract_filepaths: Sequence[Path], base_path: Optional[Path] = None
-    ) -> Dict[Version, Dict]:
-        base_path = base_path or self.config_manager.contracts_folder
-        files_by_solc_version = self.get_version_map(contract_filepaths, base_path=base_path)
-        settings = self.get_compiler_settings(contract_filepaths, base_path)
-        input_jsons = {}
+        self,
+        contract_filepaths: Iterable[Path],
+        project: Optional[ProjectManager] = None,
+        **overrides,
+    ) -> dict[Version, dict]:
+        pm = project or self.local_project
+        paths = list(contract_filepaths)  # Handle if given generator=
+        remapping = self.get_import_remapping(project=pm)
+        import_map = self.get_imports_from_remapping(paths, remapping, project=pm)
+        version_map = self.get_version_map_from_imports(paths, import_map, project=pm)
+        return self.get_standard_input_json_from_version_map(
+            version_map, remapping, project=pm, **overrides
+        )
+
+    def get_standard_input_json_from(
+        self,
+        version_map: dict[Version, set[Path]],
+        import_remappings: dict[str, str],
+        project: Optional[ProjectManager] = None,
+        **overrides,
+    ):
+        pm = project or self.local_project
+        settings = self._get_settings_from_version_map(
+            version_map, import_remappings, project=pm, **overrides
+        )
+        return self.get_standard_input_json_from_settings(settings, version_map, project=pm)
+
+    def get_standard_input_json_from_version_map(
+        self,
+        version_map: dict[Version, set[Path]],
+        import_remapping: dict[str, str],
+        project: Optional[ProjectManager] = None,
+        **overrides,
+    ):
+        pm = project or self.local_project
+        settings = self._get_settings_from_version_map(
+            version_map, import_remapping, project=pm, **overrides
+        )
+        return self.get_standard_input_json_from_settings(settings, version_map, project=pm)
+
+    def get_standard_input_json_from_settings(
+        self,
+        settings: dict[Version, dict],
+        version_map: dict[Version, set[Path]],
+        project: Optional[ProjectManager] = None,
+    ):
+        pm = project or self.local_project
+        input_jsons: dict[Version, dict] = {}
+
         for solc_version, vers_settings in settings.items():
-            if not list(files_by_solc_version[solc_version]):
+            if not list(version_map[solc_version]):
                 continue
 
             cleaned_version = Version(solc_version.base_version)
             solc_binary = get_executable(version=cleaned_version)
             arguments = {"solc_binary": solc_binary, "solc_version": cleaned_version}
 
             if solc_version >= Version("0.6.9"):
-                arguments["base_path"] = base_path
+                arguments["base_path"] = pm.path
 
             if missing_sources := [
-                x for x in vers_settings["outputSelection"] if not (base_path / x).is_file()
+                x for x in vers_settings["outputSelection"] if not (pm.path / x).is_file()
             ]:
+                # See if the missing sources are from dependencies (they likely are)
+                # and cater the error message accordingly.
+                if dependencies_needed := [x for x in missing_sources if str(x).startswith("@")]:
+                    # Missing dependencies. Should only get here if dependencies are found
+                    # in import-strs but are not installed anywhere (not in project or globally).
+                    missing_str = ", ".join(dependencies_needed)
+                    raise CompilerError(
+                        f"Missing required dependencies '{missing_str}'. "
+                        "Install them using `dependencies:` "
+                        "in an ape-config.yaml or using the `ape pm install` command."
+                    )
+
+                # Otherwise, we are missing project-level source files for some reason.
+                # This would only happen if the user passes in unexpected files outside
+                # of core.
                 missing_src_str = ", ".join(missing_sources)
-                raise CompilerError(f"Missing sources: '{missing_src_str}'.")
+                raise CompilerError(f"Sources '{missing_src_str}' not found in '{pm.name}'.")
 
             sources = {
-                x: {"content": (base_path / x).read_text()}
-                for x in vers_settings["outputSelection"]
+                x: {"content": (pm.path / x).read_text()}
+                for x in sorted(vers_settings["outputSelection"])
             }
 
             input_jsons[solc_version] = {
                 "sources": sources,
                 "settings": vers_settings,
                 "language": "Solidity",
             }
 
-        return input_jsons
+        return {v: input_jsons[v] for v in sorted(input_jsons)}
 
     def compile(
-        self, contract_filepaths: Sequence[Path], base_path: Optional[Path] = None
-    ) -> List[ContractType]:
-        base_path = base_path or self.config_manager.contracts_folder
-        contract_versions: Dict[str, Version] = {}
-        contract_types: List[ContractType] = []
-        input_jsons = self.get_standard_input_json(contract_filepaths, base_path=base_path)
+        self,
+        contract_filepaths: Iterable[Path],
+        project: Optional[ProjectManager] = None,
+        settings: Optional[dict] = None,
+    ) -> Iterator[ContractType]:
+        pm = project or self.local_project
+        settings = settings or {}
+        paths = [p for p in contract_filepaths]  # Handles generator.
+        source_ids = [f"{get_relative_path(p.absolute(), pm.path)}" for p in paths]
+        _validate_can_compile(paths)
+
+        # Compile in an isolated env so the .cache folder does not interfere with anything.
+        with pm.isolate_in_tempdir() as isolated_project:
+            filepaths = [isolated_project.path / src_id for src_id in source_ids]
+            yield from self._compile(filepaths, project=isolated_project, settings=settings)
+            compilers = isolated_project.manifest.compilers
+
+        pm.update_manifest(compilers=compilers)
 
+    def _compile(
+        self,
+        contract_filepaths: Iterable[Path],
+        project: Optional[ProjectManager] = None,
+        settings: Optional[dict] = None,
+    ):
+        pm = project or self.local_project
+        input_jsons = self.get_standard_input_json(
+            contract_filepaths, project=pm, **(settings or {})
+        )
+        contract_versions: dict[str, Version] = {}
+        contract_types: list[ContractType] = []
         for solc_version, input_json in input_jsons.items():
-            logger.info(f"Compiling using Solidity compiler '{solc_version}'.")
+            keys = (
+                "\n\t".join(sorted([x for x in input_json.get("sources", {}).keys()]))
+                or "No input."
+            )
+            log_str = f"Compiling using Solidity compiler '{solc_version}'.\nInput:\n\t{keys}"
+            logger.info(log_str)
             cleaned_version = Version(solc_version.base_version)
             solc_binary = get_executable(version=cleaned_version)
-            arguments: Dict = {"solc_binary": solc_binary, "solc_version": cleaned_version}
+            arguments: dict = {"solc_binary": solc_binary, "solc_version": cleaned_version}
 
             if solc_version >= Version("0.6.9"):
-                arguments["base_path"] = base_path
-
-            if self.project_manager.compiler_cache_folder.is_dir():
-                arguments["allow_paths"] = self.project_manager.compiler_cache_folder
+                arguments["base_path"] = pm.path
 
             # Allow empty contracts, like Vyper does.
             arguments["allow_empty"] = True
 
             try:
                 output = compile_standard(input_json, **arguments)
             except SolcError as err:
                 raise SolcCompileError(err) from err
 
             contracts = output.get("contracts", {})
-
             # Perf back-out.
             if not contracts:
                 continue
 
-            input_contract_names: List[str] = []
+            input_contract_names: list[str] = []
             for source_id, contracts_out in contracts.items():
                 for name, _ in contracts_out.items():
                     # Filter source files that the user did not ask for, such as
                     # imported relative files that are not part of the input.
                     for input_file_path in contract_filepaths:
                         if source_id in str(input_file_path):
                             input_contract_names.append(name)
 
             for source_id, contracts_out in contracts.items():
                 # ast_data = output["sources"][source_id]["ast"]
 
                 for contract_name, ct_data in contracts_out.items():
-                    contract_path = base_path / source_id
-
                     if contract_name not in input_contract_names:
                         # Only return ContractTypes explicitly asked for.
                         continue
 
                     evm_data = ct_data["evm"]
 
                     # NOTE: This sounds backwards, but it isn't...
@@ -572,45 +619,37 @@
 
                     # Skip library linking.
                     if "__$" in deployment_bytecode or "__$" in runtime_bytecode:
                         logger.warning(
                             f"Unable to compile {contract_name} - missing libraries. "
                             f"Call `{self.add_library.__name__}` with the necessary libraries"
                         )
-                        self._contracts_needing_libraries.add(contract_path)
                         continue
 
-                    if previous_version := contract_versions.get(contract_name, None):
-                        if previous_version < solc_version:
-                            # Keep the smallest version for max compat.
-                            continue
-
-                        else:
-                            # Remove the previously compiled contract types and re-compile.
-                            contract_types = [
-                                ct for ct in contract_types if ct.name != contract_name
-                            ]
-                            if contract_name in contract_versions:
-                                del contract_versions[contract_name]
+                    if contract_name in contract_versions:
+                        # Already yield in smaller version. Must not yield again
+                        # or else we will have a contract-type collision.
+                        # (Sources that are required in multiple version-sets will
+                        # hit this).
+                        continue
 
                     ct_data["contractName"] = contract_name
-                    ct_data["sourceId"] = str(
-                        get_relative_path(base_path / contract_path, base_path)
-                    )
+                    ct_data["sourceId"] = source_id
                     ct_data["deploymentBytecode"] = {"bytecode": deployment_bytecode}
                     ct_data["runtimeBytecode"] = {"bytecode": runtime_bytecode}
                     ct_data["userdoc"] = load_dict(ct_data["userdoc"])
                     ct_data["devdoc"] = load_dict(ct_data["devdoc"])
                     ct_data["sourcemap"] = evm_data["bytecode"]["sourceMap"]
                     contract_type = ContractType.model_validate(ct_data)
+                    yield contract_type
                     contract_types.append(contract_type)
                     contract_versions[contract_name] = solc_version
 
         # Output compiler data used.
-        compilers_used: Dict[Version, Compiler] = {}
+        compilers_used: dict[Version, Compiler] = {}
         for ct in contract_types:
             if not ct.name:
                 # Won't happen, but just for mypy.
                 continue
 
             vers = contract_versions[ct.name]
             settings = input_jsons[vers]["settings"]
@@ -624,27 +663,27 @@
                 compilers_used[vers] = Compiler(
                     name=self.name.lower(),
                     version=f"{vers}",
                     contractTypes=[ct.name],
                     settings=settings,
                 )
 
+        # Update compilers used in project manifest.
         # First, output compiler information to manifest.
         compilers_ls = list(compilers_used.values())
-        self.project_manager.local_project.add_compiler_data(compilers_ls)
-
-        return contract_types
+        pm.add_compiler_data(compilers_ls)
 
     def compile_code(
         self,
         code: str,
-        base_path: Optional[Path] = None,
+        project: Optional[ProjectManager] = None,
         **kwargs,
     ) -> ContractType:
-        if settings_version := self._settings_version:
+        pm = project or self.local_project
+        if settings_version := self._get_configured_version(project=pm):
             version = settings_version
 
         elif pragma := self._get_pramga_spec_from_str(code):
             if selected_version := select_version(pragma, self.installed_versions):
                 version = selected_version
             else:
                 if selected_version := select_version(pragma, self.available_versions):
@@ -665,155 +704,191 @@
 
         version = add_commit_hash(version)
         cleaned_version = Version(version.base_version)
         executable = get_executable(cleaned_version)
         try:
             result = compile_source(
                 code,
-                import_remappings=self.get_import_remapping(base_path=base_path),
-                base_path=base_path,
+                import_remappings=self.get_import_remapping(project=pm),
+                base_path=pm.path,
                 solc_binary=executable,
                 solc_version=cleaned_version,
                 allow_empty=True,
             )
         except SolcError as err:
             raise SolcCompileError(err) from err
 
         output = result[next(iter(result.keys()))]
-        return ContractType(
-            abi=output["abi"],
-            ast=output["ast"],
-            deploymentBytecode={"bytecode": HexBytes(output["bin"])},
-            devdoc=load_dict(output["devdoc"]),
-            runtimeBytecode={"bytecode": HexBytes(output["bin-runtime"])},
-            sourcemap=output["srcmap"],
-            userdoc=load_dict(output["userdoc"]),
-            **kwargs,
+        return ContractType.model_validate(
+            {
+                "abi": output["abi"],
+                "ast": output["ast"],
+                "deploymentBytecode": {"bytecode": HexBytes(output["bin"])},
+                "devdoc": load_dict(output["devdoc"]),
+                "runtimeBytecode": {"bytecode": HexBytes(output["bin-runtime"])},
+                "sourcemap": output["srcmap"],
+                "userdoc": load_dict(output["userdoc"]),
+                **kwargs,
+            }
         )
 
-    def _get_unmapped_imports(
+    def get_imports(
         self,
-        contract_filepaths: Sequence[Path],
-        base_path: Optional[Path] = None,
-    ) -> Dict[str, List[Tuple[str, str]]]:
-        contracts_path = base_path or self.config_manager.contracts_folder
-        import_remapping = self.get_import_remapping(base_path=contracts_path)
-        contract_filepaths_set = verify_contract_filepaths(contract_filepaths)
-
-        imports_dict: Dict[str, List[Tuple[str, str]]] = {}
-        for src_path, import_strs in get_import_lines(contract_filepaths_set).items():
-            import_list = []
-            for import_str in import_strs:
-                raw_import_item_search = re.search(r'"(.*?)"', import_str)
-                if raw_import_item_search is None:
-                    raise CompilerError(f"No target filename found in import {import_str}")
-                raw_import_item = raw_import_item_search.group(1)
-                import_item = _import_str_to_source_id(
-                    import_str, src_path, contracts_path, import_remapping
-                )
+        contract_filepaths: Iterable[Path],
+        project: Optional[ProjectManager] = None,
+    ) -> dict[str, list[str]]:
+        pm = project or self.local_project
+        remapping = self.get_import_remapping(project=pm)
+        _validate_can_compile(contract_filepaths)
+        paths = [x for x in contract_filepaths]  # Handle if given generator.
+        return self.get_imports_from_remapping(paths, remapping, project=pm)
 
-                # Only add to the list if it's not already there, to mimic set behavior
-                if (import_item, raw_import_item) not in import_list:
-                    import_list.append((import_item, raw_import_item))
+    def get_imports_from_remapping(
+        self,
+        paths: Iterable[Path],
+        remapping: dict[str, str],
+        project: Optional[ProjectManager] = None,
+    ) -> dict[str, list[str]]:
+        pm = project or self.local_project
+        return self._get_imports(paths, remapping, pm, tracked=set())  # type: ignore
 
-            source_id = str(get_relative_path(src_path, contracts_path))
-            imports_dict[str(source_id)] = import_list
+    def _get_imports(
+        self,
+        paths: Iterable[Path],
+        remapping: dict[str, str],
+        pm: "ProjectManager",
+        tracked: set[str],
+        include_raw: bool = False,
+    ) -> dict[str, Union[dict[str, str], list[str]]]:
+        result: dict = {}
+
+        for src_path, import_strs in get_import_lines(paths).items():
+            source_id = str(get_relative_path(src_path, pm.path))
+            if source_id in tracked:
+                # We have already accumulated imports from this source.
+                continue
 
-        return imports_dict
+            tracked.add(source_id)
 
-    def get_imports(
-        self,
-        contract_filepaths: Sequence[Path],
-        base_path: Optional[Path] = None,
-    ) -> Dict[str, List[str]]:
-        contracts_path = base_path or self.config_manager.contracts_folder
-
-        def build_map(paths: Set[Path], prev: Optional[Dict] = None) -> Dict[str, List[str]]:
-            result: Dict[str, List[str]] = prev or {}
-
-            for src_path, import_strs in get_import_lines(paths).items():
-                source_id = str(get_relative_path(src_path, contracts_path))
-                if source_id in result:
-                    continue
+            # Init with all top-level imports.
+            import_map = {
+                x: self._import_str_to_source_id(x, src_path, remapping, project=pm)
+                for x in import_strs
+            }
+            import_source_ids = list(set(list(import_map.values())))
 
-                import_set = {
-                    _import_str_to_source_id(import_str, src_path, contracts_path, import_remapping)
-                    for import_str in import_strs
-                }
-                result[source_id] = list(import_set)
-
-                # Add imports of imports.
-                import_paths = {contracts_path / p for p in import_set if p not in result}
-                result = {**result, **build_map(import_paths, prev=result)}
-
-            return result
-
-        # NOTE: Process import remapping list _before_ getting the full contract set.
-        import_remapping = self.get_import_remapping(base_path=contracts_path)
-        contract_filepaths_set = verify_contract_filepaths(contract_filepaths)
-        return build_map(contract_filepaths_set)
+            # NOTE: Add entry even if empty here.
+            result[source_id] = import_map if include_raw else import_source_ids
+
+            # Add imports of imports.
+            if not result[source_id]:
+                # Nothing else imported.
+                continue
+
+            # Add known imports.
+            known_imports = {p: result[p] for p in import_source_ids if p in result}
+            imp_paths = [pm.path / p for p in import_source_ids if p not in result]
+            unknown_imports = self._get_imports(
+                imp_paths,
+                remapping,
+                pm,
+                tracked=tracked,
+                include_raw=include_raw,
+            )
+            sub_imports = {**known_imports, **unknown_imports}
+
+            # All imported sources from imported sources are imported sources.
+            for sub_set in sub_imports.values():
+                if isinstance(sub_set, dict):
+                    for import_str, sub_import in sub_set.items():
+                        result[source_id][import_str] = sub_import
+
+                else:
+                    for sub_import in sub_set:
+                        if sub_import not in result[source_id]:
+                            result[source_id].append(sub_import)
+
+                    # Keep sorted.
+                    result[source_id] = sorted((result[source_id]))
+
+            # Combine results. This ends up like a tree-structure.
+            result = {**result, **sub_imports}
+
+        # Sort final keys and import lists for more predictable compiler behavior.
+        return {k: result[k] for k in sorted(result.keys())}
 
     def get_version_map(
         self,
-        contract_filepaths: Union[Path, Sequence[Path]],
-        base_path: Optional[Path] = None,
-    ) -> Dict[Version, Set[Path]]:
-        #  Ensure `.cache` folder is built before getting version map.
-        self.get_import_remapping(base_path=base_path)
-
-        if not isinstance(contract_filepaths, Sequence):
-            contract_filepaths = [contract_filepaths]
-
-        base_path = base_path or self.project_manager.contracts_folder
-        contract_filepaths_set = verify_contract_filepaths(contract_filepaths)
-        sources = [
-            p
-            for p in self.project_manager.source_paths
-            if p.is_file() and p.suffix == Extension.SOL.value
-        ]
-        imports = self.get_imports(sources, base_path)
+        contract_filepaths: Union[Path, Iterable[Path]],
+        project: Optional[ProjectManager] = None,
+    ) -> dict[Version, set[Path]]:
+        pm = project or self.local_project
+        paths = (
+            [contract_filepaths]
+            if isinstance(contract_filepaths, Path)
+            else [p for p in contract_filepaths]
+        )
+        _validate_can_compile(paths)
+        imports = self.get_imports(paths, project=pm)
+        return self.get_version_map_from_imports(paths, imports, project=pm)
+
+    def get_version_map_from_imports(
+        self,
+        contract_filepaths: Union[Path, Iterable[Path]],
+        import_map: dict[str, list[str]],
+        project: Optional[ProjectManager] = None,
+    ):
+        pm = project or self.local_project
+        paths = (
+            [contract_filepaths]
+            if isinstance(contract_filepaths, Path)
+            else [p for p in contract_filepaths]
+        )
+        path_set: set[Path] = {p for p in paths}
 
         # Add imported source files to list of contracts to compile.
-        source_paths_to_get = contract_filepaths_set.copy()
-        for source_path in contract_filepaths_set:
-            imported_source_paths = self._get_imported_source_paths(source_path, base_path, imports)
-            for imported_source in imported_source_paths:
-                source_paths_to_get.add(imported_source)
+        for source_path in paths:
+            source_id = f"{get_relative_path(source_path, pm.path)}"
+            if source_id not in import_map or len(import_map[source_id]) == 0:
+                continue
 
-        # Use specified version if given one
-        if version := self._settings_version:
-            return {version: source_paths_to_get}
+            import_set = {pm.path / src_id for src_id in import_map[source_id]}
+            path_set = path_set.union(import_set)
 
+        # Use specified version if given one
+        if _version := self._get_configured_version(project=pm):
+            return {_version: path_set}
         # else: find best version per source file
 
         # Build map of pragma-specs.
-        source_by_pragma_spec = {p: get_pragma_spec_from_path(p) for p in source_paths_to_get}
+        pragma_map = {p: get_pragma_spec_from_path(p) for p in path_set}
 
         # If no Solidity version has been installed previously while fetching the
         # contract version pragma, we must install a compiler, so choose the latest
         if (
             not self.installed_versions
-            and not any(source_by_pragma_spec.values())
+            and not any(pragma_map.values())
             and (latest := self.latest_version)
         ):
             install_solc(latest, show_progress=True)
 
         # Adjust best-versions based on imports.
-        files_by_solc_version: Dict[Version, Set[Path]] = {}
-        for source_file_path in source_paths_to_get:
-            solc_version = self._get_best_version(source_file_path, source_by_pragma_spec)
+        files_by_solc_version: dict[Version, set[Path]] = {}
+        for source_file_path in path_set:
+            solc_version = self._get_best_version(source_file_path, pragma_map)
             imported_source_paths = self._get_imported_source_paths(
-                source_file_path, base_path, imports
+                source_file_path, pm.path, import_map
             )
 
             for imported_source_path in imported_source_paths:
-                imported_pragma_spec = source_by_pragma_spec[imported_source_path]
-                imported_version = self._get_best_version(
-                    imported_source_path, source_by_pragma_spec
-                )
+                if imported_source_path not in pragma_map:
+                    continue
+
+                imported_pragma_spec = pragma_map[imported_source_path]
+                imported_version = self._get_best_version(imported_source_path, pragma_map)
 
                 if imported_pragma_spec is not None and (
                     str(imported_pragma_spec)[0].startswith("=")
                     or str(imported_pragma_spec)[0].isdigit()
                 ):
                     # Have to use this version.
                     solc_version = imported_version
@@ -838,34 +913,38 @@
                 )
                 if not used_in_other_version:
                     continue
 
                 other_files = [f for f in files_by_solc_version[solc_version] if f != file]
                 used_in_imports = False
                 for other_file in other_files:
-                    source_id = str(get_relative_path(other_file, base_path))
-                    import_paths = [base_path / i for i in imports.get(source_id, []) if i]
+                    source_id = str(get_relative_path(other_file, pm.path))
+                    import_paths = [pm.path / i for i in import_map.get(source_id, []) if i]
                     if file in import_paths:
                         used_in_imports = True
                         break
 
                 if not used_in_imports:
                     files_by_solc_version[solc_version].remove(file)
                     if not files_by_solc_version[solc_version]:
                         del files_by_solc_version[solc_version]
 
-        return {add_commit_hash(v): ls for v, ls in files_by_solc_version.items()}
+        result = {add_commit_hash(v): ls for v, ls in files_by_solc_version.items()}
+
+        # Sort, so it is a nicer version map and the rest of the compilation flow
+        # is more predictable.
+        return {k: result[k] for k in sorted(result)}
 
     def _get_imported_source_paths(
         self,
         path: Path,
         base_path: Path,
-        imports: Dict,
-        source_ids_checked: Optional[List[str]] = None,
-    ) -> Set[Path]:
+        imports: dict,
+        source_ids_checked: Optional[list[str]] = None,
+    ) -> set[Path]:
         source_ids_checked = source_ids_checked or []
         source_identifier = str(get_relative_path(path, base_path))
         if source_identifier in source_ids_checked:
             # Already got this source's imports
             return set()
 
         source_ids_checked.append(source_identifier)
@@ -889,16 +968,16 @@
             return pragma_spec
 
         elif compiler_version := select_version(pragma_spec, self.available_versions):
             install_solc(compiler_version, show_progress=True)
 
         else:
             # Attempt to use the best-installed version.
-            for version in self.installed_versions:
-                if version not in pragma_spec:
+            for _version in self.installed_versions:
+                if _version not in pragma_spec:
                     continue
 
                 logger.warning(
                     "Ape is unable to determine if additional versions are needed "
                     f"in order to meet spec {pragma_spec}. Resorting to the best matching "
                     "already-installed version. Alternatively, specify a Solidity "
                     "compiler version in your ape-config.yaml."
@@ -906,15 +985,28 @@
                 return pragma_spec
 
             # None of the installed versions match, and we are unable to install.
             raise CompilerError(f"Solidity version specification '{pragma_spec}' could not be met.")
 
         return pragma_spec
 
-    def _get_best_version(self, path: Path, source_by_pragma_spec: Dict) -> Version:
+    def _get_best_versions(self, path: Path, options, source_by_pragma_spec: dict) -> list[Version]:
+        # NOTE: Doesn't install.
+        if pragma_spec := source_by_pragma_spec.get(path):
+            res = get_versions_can_use(pragma_spec, list(options))
+        elif latest_installed := self.latest_installed_version:
+            res = [latest_installed]
+        elif latest := self.latest_version:
+            res = [latest]
+        else:
+            raise SolcInstallError()
+
+        return [add_commit_hash(v) for v in res]
+
+    def _get_best_version(self, path: Path, source_by_pragma_spec: dict) -> Version:
         compiler_version: Optional[Version] = None
         if pragma_spec := source_by_pragma_spec.get(path):
             if selected := select_version(pragma_spec, self.installed_versions):
                 compiler_version = selected
 
             elif selected := select_version(pragma_spec, self.available_versions):
                 # Install missing version.
@@ -937,42 +1029,37 @@
         return add_commit_hash(compiler_version)
 
     def enrich_error(self, err: ContractLogicError) -> ContractLogicError:
         if not is_0x_prefixed(err.revert_message):
             # Nothing to do.
             return err
 
-        if panic_cls := _get_sol_panic(err.revert_message):
+        elif panic_cls := _get_sol_panic(err.revert_message):
             return panic_cls(
                 base_err=err.base_err,
                 contract_address=err.contract_address,
                 source_traceback=err.source_traceback,
                 trace=err.trace,
                 txn=err.txn,
             )
 
         # Check for ErrorABI.
         bytes_message = HexBytes(err.revert_message)
         selector = bytes_message[:4]
         input_data = bytes_message[4:]
 
-        # TODO: Any version after Ape 0.6.11 we can replace this with `err.address`.
-        if not (
-            address := err.contract_address
-            or getattr(err.txn, "receiver", None)
-            or getattr(err.txn, "contract_address", None)
-        ):
+        if not err.address:
             return err
 
         if not self.network_manager.active_provider:
             # Connection required.
             return err
 
         if (
-            not (contract := self.chain_manager.contracts.instance_at(address))
+            not (contract := self.chain_manager.contracts.instance_at(err.address))
             or selector not in contract.contract_type.errors
         ):
             return err
 
         ecosystem = self.provider.network.ecosystem
         abi = contract.contract_type.errors[selector]
         inputs = ecosystem.decode_calldata(abi, input_data)
@@ -984,44 +1071,116 @@
             contract_address=err.contract_address,
             source_traceback=err.source_traceback,
             trace=err.trace,
             txn=err.txn,
         )
 
     def _flatten_source(
-        self, path: Path, base_path: Optional[Path] = None, raw_import_name: Optional[str] = None
+        self,
+        path: Path,
+        project: Optional[ProjectManager] = None,
+        raw_import_name: Optional[str] = None,
+        handled: Optional[set[str]] = None,
     ) -> str:
-        base_path = base_path or self.config_manager.contracts_folder
-        imports = self._get_unmapped_imports([path])
-        source = ""
-        for import_list in imports.values():
-            for import_path, raw_import_path in sorted(import_list):
-                source += self._flatten_source(
-                    base_path / import_path, base_path=base_path, raw_import_name=raw_import_path
-                )
-        if raw_import_name:
-            source += f"// File: {raw_import_name}\n"
-        else:
-            source += f"// File: {path.name}\n"
-        source += path.read_text() + "\n"
-        return source
+        pm = project or self.local_project
+        handled = handled or set()
+        source_id = f"{get_relative_path(path, pm.path)}"
+        handled.add(source_id)
+        remapping = self.get_import_remapping(project=project)
+        imports = self._get_imports((path,), remapping, pm, tracked=set(), include_raw=True)
+        relevant_imports = imports.get(source_id, {})
+
+        final_source = ""
+
+        for import_str, source_id in relevant_imports.items():  # type: ignore
+            if source_id in handled:
+                continue
+
+            sub_import_name = import_str.replace("import ", "").strip(" \n\t;\"'")
+            final_source += self._flatten_source(
+                pm.path / source_id,
+                project=pm,
+                raw_import_name=sub_import_name,
+                handled=handled,
+            )
 
-    def flatten_contract(self, path: Path, **kwargs) -> Content:
+        final_source += _get_flattened_source(path, name=raw_import_name)
+        return final_source
+
+    def flatten_contract(
+        self, path: Path, project: Optional[ProjectManager] = None, **kwargs
+    ) -> Content:
         # try compiling in order to validate it works
-        self.compile([path], base_path=self.config_manager.contracts_folder)
-        source = self._flatten_source(path)
-        source = remove_imports(source)
-        source = process_licenses(source)
-        source = remove_version_pragmas(source)
+        res = self._flatten_source(path, project=project)
+        res = remove_imports(res)
+        res = process_licenses(res)
+        res = remove_version_pragmas(res)
         pragma = get_first_version_pragma(path.read_text())
-        source = "\n".join([pragma, source])
-        lines = source.splitlines()
+        res = "\n".join([pragma, res])
+        lines = res.splitlines()
         line_dict = {i + 1: line for i, line in enumerate(lines)}
         return Content(root=line_dict)
 
+    def _import_str_to_source_id(
+        self,
+        _import_str: str,
+        source_path: Path,
+        import_remapping: dict[str, str],
+        project: Optional[ProjectManager] = None,
+    ) -> str:
+        pm = project or self.local_project
+        quote = '"' if '"' in _import_str else "'"
+
+        try:
+            end_index = _import_str.index(quote) + 1
+        except ValueError as err:
+            raise CompilerError(
+                f"Error parsing import statement '{_import_str}' in '{source_path.name}'."
+            ) from err
+
+        import_str_prefix = _import_str[end_index:]
+        import_str_value = import_str_prefix[: import_str_prefix.index(quote)]
+
+        # Get all matches.
+        valid_matches: list[tuple[str, str]] = []
+        key = None
+        base_path = None
+        for key, value in import_remapping.items():
+            if key not in import_str_value:
+                continue
+
+            valid_matches.append((key, value))
+
+        if valid_matches:
+            key, value = max(valid_matches, key=lambda x: len(x[0]))
+            import_str_value = import_str_value.replace(key, value)
+
+        if import_str_value.startswith("."):
+            base_path = source_path.parent
+        elif (pm.path / import_str_value).is_file():
+            base_path = pm.path
+        elif (pm.contracts_folder / import_str_value).is_file():
+            base_path = pm.contracts_folder
+        elif key is not None and key.startswith("@"):
+            nm = key[1:]
+            for cfg_dep in pm.config.dependencies:
+                if (
+                    cfg_dep.get("name") == nm
+                    and "project" in cfg_dep
+                    and (Path(cfg_dep["project"]) / import_str_value).is_file()
+                ):
+                    base_path = Path(cfg_dep["project"])
+
+        if base_path is None:
+            # No base_path, do as-is.
+            return import_str_value
+
+        path = (base_path / import_str_value).resolve()
+        return f"{get_relative_path(path.absolute(), pm.path)}"
+
 
 def remove_imports(flattened_contract: str) -> str:
     # Use regex.sub() to remove matched import statements
     no_imports_contract = IMPORTS_PATTERN.sub("", flattened_contract)
 
     return no_imports_contract
 
@@ -1033,15 +1192,15 @@
 def get_first_version_pragma(source: str) -> str:
     match = VERSION_PRAGMA_PATTERN.search(source)
     if match:
         return match.group(0)
     return ""
 
 
-def get_licenses(src: str) -> List[Tuple[str, str]]:
+def get_licenses(src: str) -> list[tuple[str, str]]:
     return LICENSES_PATTERN.findall(src)
 
 
 def process_licenses(contract: str) -> str:
     """
     Process the licenses in a contract.
     Ensure that all licenses are identical, and if not, raise an error.
@@ -1080,15 +1239,15 @@
 
     # Prepend the contract with only the root license line.
     contract_with_single_license = f"{license_line}\n{contract_without_licenses}"
 
     return contract_with_single_license
 
 
-def _get_sol_panic(revert_message: str) -> Optional[Type[RuntimeErrorUnion]]:
+def _get_sol_panic(revert_message: str) -> Optional[type[RuntimeErrorUnion]]:
     if revert_message.startswith(RUNTIME_ERROR_CODE_PREFIX):
         # ape-geth (style) plugins show the hex with the Panic ABI prefix.
         error_type_val = int(
             f"0x{revert_message.replace(RUNTIME_ERROR_CODE_PREFIX, '').lstrip('0')}", 16
         )
     else:
         # Some plugins, like ape-hardhat, will deliver panic codes directly (no Panic ABI prefix)
@@ -1096,56 +1255,17 @@
 
     if error_type_val in [x.value for x in RuntimeErrorType]:
         return RUNTIME_ERROR_MAP[RuntimeErrorType(error_type_val)]
 
     return None
 
 
-def _import_str_to_source_id(
-    _import_str: str, source_path: Path, base_path: Path, import_remapping: Dict[str, str]
-) -> str:
-    quote = '"' if '"' in _import_str else "'"
-
-    try:
-        end_index = _import_str.index(quote) + 1
-    except ValueError as err:
-        raise CompilerError(
-            f"Error parsing import statement '{_import_str}' in '{source_path.name}'."
-        ) from err
-
-    import_str_prefix = _import_str[end_index:]
-    import_str_value = import_str_prefix[: import_str_prefix.index(quote)]
-    path = (source_path.parent / import_str_value).resolve()
-    source_id_value = str(get_relative_path(path, base_path))
-
-    # Get all matches.
-    matches: List[Tuple[str, str]] = []
-    for key, value in import_remapping.items():
-        if key not in source_id_value:
-            continue
-
-        matches.append((key, value))
-
-    if not matches:
-        return source_id_value
-
-    # Convert remapping list back to source using longest match (most exact).
-    key, value = max(matches, key=lambda x: len(x[0]))
-    sections = [s for s in source_id_value.split(key) if s]
-    depth = len(sections) - 1
-    source_id_value = ""
-
-    index = 0
-    for section in sections:
-        if index == depth:
-            source_id_value += value
-            source_id_value += section
-        elif index >= depth:
-            source_id_value += section
-
-        index += 1
+def _try_max(ls: list[Any]):
+    return max(ls) if ls else None
 
-    return source_id_value
 
+def _validate_can_compile(paths: Iterable[Path]):
+    extensions = {get_full_extension(p): p for p in paths if p}
 
-def _try_max(ls: List[Any]):
-    return max(ls) if ls else None
+    for ext, file in extensions.items():
+        if ext not in [e.value for e in Extension]:
+            raise CompilerError(f"Unable to compile '{file.name}' using Solidity compiler.")
```

### Comparing `ape-solidity-0.7.3/ape_solidity/exceptions.py` & `ape-solidity-0.8.0/ape_solidity/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import IntEnum
-from typing import Dict, Type, Union
+from typing import Union
 
 from ape.exceptions import CompilerError, ConfigError, ContractLogicError
 from ape.logging import LogLevel, logger
 from solcx.exceptions import SolcError
 
 
 class SolcInstallError(CompilerError):
@@ -165,15 +165,15 @@
     EnumConversionError,
     EncodeStorageError,
     IndexOutOfBoundsError,
     MemoryOverflowError,
     PopOnEmptyArrayError,
     ZeroInitializedVariableError,
 ]
-RUNTIME_ERROR_MAP: Dict[RuntimeErrorType, Type[RuntimeErrorUnion]] = {
+RUNTIME_ERROR_MAP: dict[RuntimeErrorType, type[RuntimeErrorUnion]] = {
     RuntimeErrorType.ASSERTION_ERROR: SolidityAssertionError,
     RuntimeErrorType.ARITHMETIC_UNDER_OR_OVERFLOW: SolidityArithmeticError,
     RuntimeErrorType.DIVISION_BY_ZERO_ERROR: DivisionByZeroError,
     RuntimeErrorType.ENUM_CONVERSION_OUT_OF_BOUNDS: EnumConversionError,
     RuntimeErrorType.INCORRECTLY_ENCODED_STORAGE_BYTE_ARRAY: EncodeStorageError,
     RuntimeErrorType.INDEX_OUT_OF_BOUNDS_ERROR: IndexOutOfBoundsError,
     RuntimeErrorType.MEMORY_OVERFLOW_ERROR: MemoryOverflowError,
```

### Comparing `ape-solidity-0.7.3/ape_solidity.egg-info/PKG-INFO` & `ape-solidity-0.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 Metadata-Version: 2.1
 Name: ape-solidity
-Version: 0.7.3
+Version: 0.8.0
 Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
 Home-page: https://github.com/ApeWorX/ape-solidity
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 Compile Solidity contracts.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
 
@@ -88,40 +87,40 @@
 ```yaml
 solidity:
   evm_version: paris
 ```
 
 ### Dependency Mapping
 
-To configure import remapping, use your project's `ape-config.yaml` file:
-
-```yaml
-solidity:
-  import_remapping:
-    - "@openzeppelin=path/to/open_zeppelin/contracts"
-```
-
-If you are using the `dependencies:` key in your `ape-config.yaml`, `ape` can automatically
-search those dependencies for the path.
+By default, `ape-solidity` knows to look at installed dependencies for potential remapping-values and will use those when it notices you are importing them.
+For example, if you are using dependencies like:
 
 ```yaml
 dependencies:
-  - name: OpenZeppelin
+  - name: openzeppelin
     github: OpenZeppelin/openzeppelin-contracts
     version: 4.4.2
-
-solidity:
-  import_remapping:
-    - "@openzeppelin=OpenZeppelin/4.4.2"
 ```
 
-Once you have your dependencies configured, you can import packages using your import keys:
+And your source files import from `openzeppelin` this way:
 
 ```solidity
-import "@openzeppelin/token/ERC721/ERC721.sol";
+import "@openzeppelin/contracts/token/ERC721/ERC721.sol";
+```
+
+Ape knows how to resolve the `@openzeppelin` value and find the correct source.
+
+If you want to override this behavior or add new remappings that are not dependencies, you can add them to your `ape-config.yaml` under the `solidity:` key.
+For example, let's say you have downloaded `openzeppelin` somewhere and do not have it installed in Ape.
+You can map to your local install of `openzeppelin` this way:
+
+```yaml
+solidity:
+  import_remapping:
+    - "@openzeppelin=path/to/openzeppelin"
 ```
 
 ### Library Linking
 
 To compile contracts that use libraries, you need to add the libraries first.
 Use the `add_library()` method from the `ape-solidity` compiler class to add the library.
 A typical flow is:
```

### Comparing `ape-solidity-0.7.3/ape_solidity.egg-info/SOURCES.txt` & `ape-solidity-0.8.0/ape_solidity.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,32 +35,33 @@
 tests/package-lock.json
 tests/package.json
 tests/test_compiler.py
 tests/test_exceptions.py
 tests/test_integration.py
 tests/BrownieProject/brownie-config.yaml
 tests/BrownieProject/contracts/BrownieContract.sol
-tests/BrownieStyleDependency/ape-config.yaml
-tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
-tests/BrownieStyleDependency/contracts/FailingContract.sol
 tests/Dependency/ape-config.yaml
 tests/Dependency/contracts/Dependency.sol
 tests/Dependency/contracts/OlderDependency.sol
 tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
 tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
 tests/DependencyOfDependency/ape-config.yaml
 tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
+tests/NonCompilingDependency/ape-config.yaml
+tests/NonCompilingDependency/contracts/CompilingContract.sol
+tests/NonCompilingDependency/contracts/NonCompilingContract.sol
 tests/ProjectWithinProject/ape-config.yaml
 tests/ProjectWithinProject/contracts/Contract.sol
 tests/VersionSpecifiedInConfig/ape-config.yaml
 tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
 tests/contracts/BuiltinErrorChecker.sol
 tests/contracts/CircularImport1.sol
 tests/contracts/CircularImport2.sol
 tests/contracts/CompilesOnce.sol
+tests/contracts/ContractUsingLibraryNotInSameSource.sol
 tests/contracts/DifferentNameThanFile.sol
 tests/contracts/ExperimentalABIEncoderV2.sol
 tests/contracts/HasError.sol
 tests/contracts/ImportOlderDependency.sol
 tests/contracts/ImportSourceWithEqualSignVersion.sol
 tests/contracts/ImportSourceWithNoPrefixVersion.sol
 tests/contracts/ImportingLessConstrainedVersion.sol
```

### Comparing `ape-solidity-0.7.3/ape_solidity.egg-info/requires.txt` & `ape-solidity-0.8.0/ape_solidity.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 py-solc-x<3,>=2.0.2
-eth-ape<0.8,>=0.7.10
+eth-ape<0.9,>=0.8.1
 ethpm-types
 eth-pydantic-types
 packaging
 requests
 
 [dev]
 pytest>=6.0
```

### Comparing `ape-solidity-0.7.3/pyproject.toml` & `ape-solidity-0.8.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -12,29 +12,32 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311']
+target-version = ['py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
     --cov-report html
     --cov-report xml
     --cov=ape_solidity
 """
 python_files = "test_*.py"
 testpaths = "tests"
-markers = "fuzzing: Run Hypothesis fuzz test suite"
+markers = """
+fuzzing: Run Hypothesis fuzz test suite
+install: Tests that will install a solc version (slow)
+"""
 
 [tool.isort]
 line_length = 100
 force_grid_wrap = 0
 include_trailing_comma = true
 multi_line_output = 3
 use_parentheses = true
```

### Comparing `ape-solidity-0.7.3/setup.py` & `ape-solidity-0.8.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,21 +65,21 @@
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-solidity",
     include_package_data=True,
     install_requires=[
         "py-solc-x>=2.0.2,<3",
-        "eth-ape>=0.7.10,<0.8",
+        "eth-ape>=0.8.1,<0.9",
         "ethpm-types",  # Use the version ape requires
         "eth-pydantic-types",  # Use the version ape requires
         "packaging",  # Use the version ape requires
         "requests",
     ],
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["ape_solidity"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_solidity": ["py.typed"]},
@@ -87,14 +87,13 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `ape-solidity-0.7.3/tests/conftest.py` & `ape-solidity-0.8.0/tests/conftest.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 import shutil
 from contextlib import contextmanager
 from pathlib import Path
-from shutil import copytree
 from tempfile import mkdtemp
 from unittest import mock
 
 import ape
 import pytest
 import solcx
+from ape.utils.os import create_tempdir
 
-from ape_solidity.compiler import Extension
-
-# NOTE: Ensure that we don't use local paths for these
-DATA_FOLDER = Path(mkdtemp()).resolve()
-PROJECT_FOLDER = Path(mkdtemp()).resolve()
-ape.config.DATA_FOLDER = DATA_FOLDER
-ape.config.PROJECT_FOLDER = PROJECT_FOLDER
+from ape_solidity._utils import Extension
 
 
 @contextmanager
 def _tmp_solcx_path(monkeypatch):
     solcx_install_path = mkdtemp()
 
     monkeypatch.setenv(
@@ -50,52 +44,59 @@
     """
     Creates a new, temporary installation path for solcx for a given test.
     """
     with _tmp_solcx_path(monkeypatch) as path:
         yield path
 
 
-@pytest.fixture(autouse=True)
-def data_folder():
-    base_path = Path(__file__).parent / "data"
-    copytree(base_path, DATA_FOLDER, dirs_exist_ok=True)
-    return DATA_FOLDER
-
-
-@pytest.fixture
-def config():
-    return ape.config
-
-
-@pytest.fixture(autouse=True)
-def project(data_folder, config):
-    _ = data_folder  # Ensure happens first.
-    project_source_dir = Path(__file__).parent
-    project_dest_dir = PROJECT_FOLDER / project_source_dir.name
+@pytest.fixture(scope="session")
+def project(config):
+    _ = config  # Ensure temp data folder gets set first.
+    root = Path(__file__).parent
 
-    # Delete build / .cache that may exist pre-copy
-    project_path = Path(__file__).parent
+    # Delete .build / .cache that may exist pre-copy
     for path in (
-        project_path,
-        project_path / "BrownieProject",
-        project_path / "BrownieStyleDependency",
-        project_path / "Dependency",
-        project_path / "DependencyOfDependency",
-        project_path / "ProjectWithinProject",
-        project_path / "VersionSpecifiedInConfig",
+        root,
+        root / "BrownieProject",
+        root / "BrownieStyleDependency",
+        root / "Dependency",
+        root / "DependencyOfDependency",
+        root / "ProjectWithinProject",
+        root / "VersionSpecifiedInConfig",
     ):
         for cache in (path / ".build", path / "contracts" / ".cache"):
             if cache.is_dir():
                 shutil.rmtree(cache)
 
-    copytree(project_source_dir, project_dest_dir, dirs_exist_ok=True)
-    with config.using_project(project_dest_dir) as project:
-        yield project
-        if project.local_project._cache_folder.is_dir():
-            shutil.rmtree(project.local_project._cache_folder)
+    root_project = ape.Project(root)
+    with root_project.isolate_in_tempdir() as tmp_project:
+        yield tmp_project
+
+
+@pytest.fixture(scope="session", autouse=True)
+def config():
+    cfg = ape.config
+
+    # Uncomment to install dependencies in actual data folder.
+    # This will save time running tests.
+    # project = ape.Project(Path(__file__).parent)
+    # project.dependencies.install()
+
+    # Ensure we don't persist any .ape data.
+    real_data_folder = cfg.DATA_FOLDER
+    with create_tempdir() as path:
+        cfg.DATA_FOLDER = path
+
+        # Copy in existing packages to save test time
+        # when running locally.
+        packages = real_data_folder / "packages"
+        packages.mkdir(parents=True, exist_ok=True)
+        shutil.copytree(packages, path / "packages", dirs_exist_ok=True)
+
+        yield cfg
 
 
 @pytest.fixture
 def compiler_manager():
     return ape.compilers
 
 
@@ -122,19 +123,14 @@
     mock_registered_compilers = mocker.patch(path, new_callable=mock.PropertyMock)
 
     # Only ethpm (.json) and Solidity extensions allowed.
     mock_registered_compilers.return_value = {".json": ape_pm, **valid_compilers}
 
 
 @pytest.fixture
-def vyper_source_path(project):
-    return project.contracts_folder / "RandomVyperFile.vy"
-
-
-@pytest.fixture
 def account():
     return ape.accounts.test_accounts[0]
 
 
 @pytest.fixture
 def owner():
     return ape.accounts.test_accounts[1]
```

### Comparing `ape-solidity-0.7.3/tests/contracts/LibraryFun.sol` & `ape-solidity-0.8.0/tests/contracts/LibraryFun.sol`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 // We define a new struct datatype that will be used to
 // hold its data in the calling contract.
 struct Data {
     mapping(uint => bool) flags;
 }
 
-library Set {
+library ExampleLibrary {
     // Note that the first parameter is of type "storage
     // reference" and thus only its storage address and not
     // its contents is passed as part of the call.  This is a
     // special feature of library functions.  It is idiomatic
     // to call the first parameter `self`, if the function can
     // be seen as a method of that object.
     function insert(Data storage self, uint value)
@@ -42,18 +42,18 @@
         returns (bool)
     {
         return self.flags[value];
     }
 }
 
 
-contract C {
+contract ContractUsingLibraryInSameSource {
     Data knownValues;
 
     function register(uint value) public {
         // The library functions can be called without a
         // specific instance of the library, since the
         // "instance" will be the current contract.
-        require(Set.insert(knownValues, value));
+        require(ExampleLibrary.insert(knownValues, value));
     }
     // In this contract, we can also directly access knownValues.flags, if we want.
 }
```

### Comparing `ape-solidity-0.7.3/tests/data/ImportingLessConstrainedVersionFlat.sol` & `ape-solidity-0.8.0/tests/data/ImportingLessConstrainedVersionFlat.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/tests/data/ImportsFlattened.sol.txt` & `ape-solidity-0.8.0/tests/data/ImportsFlattened.sol.txt`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json` & `ape-solidity-0.8.0/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json` & `ape-solidity-0.8.0/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/tests/data/packages/vault/master/vault_main.json` & `ape-solidity-0.8.0/tests/data/packages/vault/master/vault_main.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/tests/data/packages/vault/v0.4.5/vault.json` & `ape-solidity-0.8.0/tests/data/packages/vault/v0.4.5/vault.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/tests/package-lock.json` & `ape-solidity-0.8.0/tests/package-lock.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/tests/scripts/clean.py` & `ape-solidity-0.8.0/tests/scripts/clean.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/tests/test_exceptions.py` & `ape-solidity-0.8.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.3/tests/test_integration.py` & `ape-solidity-0.8.0/tests/test_integration.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,35 +9,32 @@
 
 
 @pytest.fixture
 def runner():
     return CliRunner()
 
 
-def test_compile_using_cli(ape_cli, runner):
-    result = runner.invoke(ape_cli, ["compile"], catch_exceptions=False)
+def test_compile_using_cli(ape_cli, runner, project):
+    arguments = ["compile", "--project", f"{project.path}"]
+    result = runner.invoke(ape_cli, [*arguments, "--force"], catch_exceptions=False)
     assert result.exit_code == 0
     assert "CompilesOnce" in result.output
-    result = runner.invoke(ape_cli, ["compile"], catch_exceptions=False)
+    result = runner.invoke(ape_cli, arguments, catch_exceptions=False)
 
     # Already compiled so does not compile again.
     assert "CompilesOnce" not in result.output
 
 
 @pytest.mark.parametrize(
     "contract_path",
     (
         "CompilesOnce",
         "CompilesOnce.sol",
         "contracts/CompilesOnce",
         "contracts/CompilesOnce.sol",
     ),
 )
-def test_compile_specified_contracts(ape_cli, runner, contract_path):
-    result = runner.invoke(ape_cli, ["compile", contract_path, "--force"], catch_exceptions=False)
+def test_compile_specified_contracts(ape_cli, runner, contract_path, project):
+    arguments = ("compile", "--project", f"{project.path}", contract_path, "--force")
+    result = runner.invoke(ape_cli, arguments, catch_exceptions=False)
     assert result.exit_code == 0, result.output
-    assert "Compiling 'CompilesOnce.sol'" in result.output, f"Failed to compile {contract_path}."
-
-
-def test_force_recompile(ape_cli, runner):
-    result = runner.invoke(ape_cli, ["compile", "--force"], catch_exceptions=False)
-    assert result.exit_code == 0
+    assert "contracts/CompilesOnce.sol" in result.output, f"Failed to compile {contract_path}."
```

