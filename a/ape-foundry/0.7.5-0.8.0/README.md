# Comparing `tmp/ape-foundry-0.7.5.tar.gz` & `tmp/ape-foundry-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-foundry-0.7.5.tar", last modified: Thu May  9 18:48:52 2024, max compression
+gzip compressed data, was "ape-foundry-0.8.0.tar", last modified: Sat Jun  1 01:15:18 2024, max compression
```

## Comparing `ape-foundry-0.7.5.tar` & `ape-foundry-0.8.0.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.074081 ape-foundry-0.7.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.058081 ape-foundry-0.7.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.058081 ape-foundry-0.7.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.058081 ape-foundry-0.7.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-09 18:48:52.074081 ape-foundry-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.058081 ape-foundry-0.7.5/ape_foundry/
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/ape_foundry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/ape_foundry/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/ape_foundry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    37942 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/ape_foundry/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/ape_foundry/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 18:48:51.000000 ape-foundry-0.7.5/ape_foundry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.058081 ape-foundry-0.7.5/ape_foundry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-09 18:48:51.000000 ape-foundry-0.7.5/ape_foundry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-09 18:48:52.000000 ape-foundry-0.7.5/ape_foundry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:48:51.000000 ape-foundry-0.7.5/ape_foundry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:48:51.000000 ape-foundry-0.7.5/ape_foundry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-09 18:48:51.000000 ape-foundry-0.7.5/ape_foundry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 18:48:51.000000 ape-foundry-0.7.5/ape_foundry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 18:48:52.074081 ape-foundry-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.062081 ape-foundry-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.054081 ape-foundry-0.7.5/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.054081 ape-foundry-0.7.5/tests/data/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.054081 ape-foundry-0.7.5/tests/data/contracts/ethereum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.062081 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/
--rw-r--r--   0 runner    (1001) docker     (127)    77599 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/contract_a.json
--rw-r--r--   0 runner    (1001) docker     (127)    75147 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/contract_b.json
--rw-r--r--   0 runner    (1001) docker     (127)    32313 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/contract_c.json
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/has_error.json
--rw-r--r--   0 runner    (1001) docker     (127)    33356 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/solidity_contract.json
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/token_a.json
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/token_b.json
--rw-r--r--   0 runner    (1001) docker     (127)    28197 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/vyper_contract.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.054081 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.074081 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
--rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
--rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
--rw-r--r--   0 runner    (1001) docker     (127)    16120 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
--rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
--rw-r--r--   0 runner    (1001) docker     (127)    19792 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
--rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
--rw-r--r--   0 runner    (1001) docker     (127)    44429 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
--rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
--rw-r--r--   0 runner    (1001) docker     (127)    23253 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
--rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
--rw-r--r--   0 runner    (1001) docker     (127)    15942 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
--rw-r--r--   0 runner    (1001) docker     (127)    14160 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
--rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
--rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.074081 ape-foundry-0.7.5/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/python/pytest_test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/python/pytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.074081 ape-foundry-0.7.5/tests/data/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/sources/RevertsContractVy.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/sources/TokenA.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/sources/TokenB.vy
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/expected_traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/test_fork_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17730 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/test_pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:18.392109 ape-foundry-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:18.376109 ape-foundry-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:18.376109 ape-foundry-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:18.376109 ape-foundry-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-06-01 01:15:18.392109 ape-foundry-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:18.376109 ape-foundry-0.8.0/ape_foundry/
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/ape_foundry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/ape_foundry/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/ape_foundry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31523 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/ape_foundry/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/ape_foundry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-01 01:15:18.000000 ape-foundry-0.8.0/ape_foundry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:18.376109 ape-foundry-0.8.0/ape_foundry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-06-01 01:15:18.000000 ape-foundry-0.8.0/ape_foundry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-06-01 01:15:18.000000 ape-foundry-0.8.0/ape_foundry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:15:18.000000 ape-foundry-0.8.0/ape_foundry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:15:18.000000 ape-foundry-0.8.0/ape_foundry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-01 01:15:18.000000 ape-foundry-0.8.0/ape_foundry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-01 01:15:18.000000 ape-foundry-0.8.0/ape_foundry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-06-01 01:15:18.392109 ape-foundry-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:18.380109 ape-foundry-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:18.372109 ape-foundry-0.8.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:18.372109 ape-foundry-0.8.0/tests/data/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:18.372109 ape-foundry-0.8.0/tests/data/contracts/ethereum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:18.380109 ape-foundry-0.8.0/tests/data/contracts/ethereum/local/
+-rw-r--r--   0 runner    (1001) docker     (127)    77599 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/local/contract_a.json
+-rw-r--r--   0 runner    (1001) docker     (127)    75147 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/local/contract_b.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32313 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/local/contract_c.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/local/has_error.json
+-rw-r--r--   0 runner    (1001) docker     (127)    33356 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/local/solidity_contract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/local/token_a.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/local/token_b.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28197 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/local/vyper_contract.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:18.372109 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:18.392109 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16120 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19792 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44429 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23253 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15942 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14160 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:18.392109 ape-foundry-0.8.0/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/python/pytest_test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/python/pytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:15:18.392109 ape-foundry-0.8.0/tests/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/sources/RevertsContractVy.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/sources/TokenA.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/data/sources/TokenB.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/expected_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/test_fork_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16181 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/test_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-06-01 01:14:15.000000 ape-foundry-0.8.0/tests/test_trace.py
```

### Comparing `ape-foundry-0.7.5/.github/ISSUE_TEMPLATE/bug.md` & `ape-foundry-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/.github/ISSUE_TEMPLATE/feature.md` & `ape-foundry-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/.github/ISSUE_TEMPLATE/work-item.md` & `ape-foundry-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/.github/release-drafter.yml` & `ape-foundry-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/.github/workflows/codeql.yml` & `ape-foundry-0.8.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/.github/workflows/commitlint.yaml` & `ape-foundry-0.8.0/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/.github/workflows/prtitle.yaml` & `ape-foundry-0.8.0/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/.github/workflows/publish.yaml` & `ape-foundry-0.8.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/.github/workflows/stale-prs.yml` & `ape-foundry-0.8.0/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/.github/workflows/test.yaml` & `ape-foundry-0.8.0/.github/workflows/test.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 # TODO: Replace with macos-latest when works again.
                 #   https://github.com/actions/setup-python/issues/808
                 os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10", "3.11", "3.12"]
+                python-version: [3.9, "3.10", "3.11", "3.12"]
 
         steps:
         - uses: actions/checkout@v4
 
         - name: Install Foundry
           uses: foundry-rs/foundry-toolchain@v1
           with:
```

### Comparing `ape-foundry-0.7.5/.gitignore` & `ape-foundry-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/.pre-commit-config.yaml` & `ape-foundry-0.8.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -26,11 +26,11 @@
     -   id: mypy
         additional_dependencies: [types-PyYAML, types-requests, types-setuptools, pydantic]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
     -   id: mdformat
-        additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
+        additional_dependencies: [mdformat-gfm, mdformat-frontmatter, mdformat-pyproject]
 
 default_language_version:
     python: python3
```

### Comparing `ape-foundry-0.7.5/CONTRIBUTING.md` & `ape-foundry-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/LICENSE` & `ape-foundry-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/PKG-INFO` & `ape-foundry-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: ape-foundry
-Version: 0.7.5
+Version: 0.8.0
 Summary: ape-foundry: Ape network provider for Foundry
 Home-page: https://github.com/ApeWorX/ape-foundry
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
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -31,15 +30,15 @@
 # Quick Start
 
 Foundry network provider plugin for Ape.
 Foundry is a development framework written in Rust for Ethereum that includes a local network implementation.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 - Foundry. See Foundry's [Installation](https://github.com/foundry-rs/foundry#installation) documentation for steps.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-foundry-0.7.5/README.md` & `ape-foundry-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Quick Start
 
 Foundry network provider plugin for Ape.
 Foundry is a development framework written in Rust for Ethereum that includes a local network implementation.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 - Foundry. See Foundry's [Installation](https://github.com/foundry-rs/foundry#installation) documentation for steps.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-foundry-0.7.5/ape_foundry/__init__.py` & `ape-foundry-0.8.0/ape_foundry/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/ape_foundry/constants.py` & `ape-foundry-0.8.0/ape_foundry/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,17 @@
             9200000: "muirglacier",
             12244000: "berlin",
             12965000: "london",
         },
         "sepolia": {
             0: "london",
         },
+        "holesky": {
+            0: "london",
+        },
     },
     "polygon": {
         "mainnet": {
             0: "petersburg",
             3395000: "muirglacier",
             14750000: "berlin",
             23850000: "london",
```

### Comparing `ape-foundry-0.7.5/ape_foundry/exceptions.py` & `ape-foundry-0.8.0/ape_foundry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/ape_foundry/provider.py` & `ape-foundry-0.8.0/ape_foundry/provider.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,41 @@
 import os
 import random
 import shutil
 from bisect import bisect_right
 from copy import copy
-from itertools import tee
-from pathlib import Path
 from subprocess import PIPE, call
-from typing import Any, Dict, Iterator, List, Literal, Optional, Tuple, Union, cast
+from typing import Literal, Optional, Union, cast
 
 from ape.api import (
     BlockAPI,
     ForkedNetworkAPI,
     PluginConfig,
     ReceiptAPI,
     SubprocessProvider,
     TestProviderAPI,
+    TraceAPI,
     TransactionAPI,
 )
 from ape.exceptions import (
     ContractLogicError,
     OutOfGasError,
     SubprocessError,
     TransactionError,
     VirtualMachineError,
 )
 from ape.logging import logger
-from ape.types import (
-    AddressType,
-    BlockID,
-    CallTreeNode,
-    ContractCode,
-    SnapshotID,
-    SourceTraceback,
-    TraceFrame,
-)
+from ape.types import AddressType, BlockID, ContractCode, SnapshotID
 from ape.utils import cached_property
 from ape_ethereum.provider import Web3Provider
+from ape_ethereum.trace import TraceApproach, TransactionTrace
 from ape_test import ApeTestConfig
 from eth_pydantic_types import HashBytes32, HexBytes
 from eth_typing import HexStr
 from eth_utils import add_0x_prefix, is_0x_prefixed, is_hex, to_hex
-from evm_trace import CallType, ParityTraceList
-from evm_trace import TraceFrame as EvmTraceFrame
-from evm_trace import get_calltree_from_geth_trace, get_calltree_from_parity_trace
 from pydantic import field_validator, model_validator
 from pydantic_settings import SettingsConfigDict
 from web3 import HTTPProvider, Web3
 from web3.exceptions import ContractCustomError
 from web3.exceptions import ContractLogicError as Web3ContractLogicError
 from web3.exceptions import ExtraDataLengthError
 from web3.gas_strategies.rpc import rpc_gas_price_strategy
@@ -90,15 +79,15 @@
     base_fee: int = 0
     priority_fee: int = 0
     gas_price: int = 0
 
     # For setting the values in --fork and --fork-block-number command arguments.
     # Used only in FoundryForkProvider.
     # Mapping of ecosystem_name => network_name => FoundryForkConfig
-    fork: Dict[str, Dict[str, FoundryForkConfig]] = {}
+    fork: dict[str, dict[str, FoundryForkConfig]] = {}
 
     disable_block_gas_limit: bool = False
     """
     Disable the ``call.gas_limit <= block.gas_limit`` constraint.
     """
 
     auto_mine: bool = True
@@ -122,20 +111,20 @@
 
 def _call(*args):
     return call([*args], stderr=PIPE, stdout=PIPE, stdin=PIPE)
 
 
 class FoundryProvider(SubprocessProvider, Web3Provider, TestProviderAPI):
     _host: Optional[str] = None
-    attempted_ports: List[int] = []
+    attempted_ports: list[int] = []
     cached_chain_id: Optional[int] = None
     _did_warn_wrong_node = False
 
     @property
-    def unlocked_accounts(self) -> List[AddressType]:
+    def unlocked_accounts(self) -> list[AddressType]:
         return list(self.account_manager.test_accounts._impersonated_accounts)
 
     @property
     def mnemonic(self) -> str:
         return self._test_config.mnemonic
 
     @property
@@ -188,18 +177,14 @@
             raise FoundrySubprocessError(
                 "Anvil executable returned error code. See ape-foundry README for install steps."
             )
 
         return anvil
 
     @property
-    def project_folder(self) -> Path:
-        return self.config_manager.PROJECT_FOLDER
-
-    @property
     def uri(self) -> str:
         if self._host is not None:
             return self._host
 
         elif config_host := self.settings.host:
             if config_host == "auto":
                 self._host = "auto"
@@ -252,28 +237,24 @@
 
     @cached_property
     def _test_config(self) -> ApeTestConfig:
         return cast(ApeTestConfig, self.config_manager.get_config("test"))
 
     @property
     def auto_mine(self) -> bool:
-        return self._make_request("anvil_getAutomine", [])
+        return self.make_request("anvil_getAutomine", [])
+
+    @auto_mine.setter
+    def auto_mine(self, value) -> None:
+        self.make_request("anvil_setAutomine", [value])
 
     @property
     def settings(self) -> FoundryNetworkConfig:
         return cast(FoundryNetworkConfig, super().settings)
 
-    def __setattr__(self, attr: str, value: Any) -> None:
-        # NOTE: Need to do this until https://github.com/pydantic/pydantic/pull/2625 is figured out
-        if attr == "auto_mine":
-            self._make_request("anvil_setAutomine", [value])
-
-        else:
-            super().__setattr__(attr, value)
-
     def connect(self):
         """
         Start the foundry process and verify it's up and accepting connections.
         **NOTE**: Must set port before calling 'super().connect()'.
         """
 
         if "APE_FOUNDRY_HOST" in os.environ:
@@ -425,15 +406,15 @@
             raise FoundryProviderError(f"Failed to connect to Anvil node at '{self._clean_uri}'.")
 
     def disconnect(self):
         self._web3 = None
         self._host = None
         super().disconnect()
 
-    def build_command(self) -> List[str]:
+    def build_command(self) -> list[str]:
         cmd = [
             self.anvil_bin,
             "--port",
             f"{self._port or DEFAULT_PORT}",
             "--mnemonic",
             self.mnemonic,
             "--accounts",
@@ -471,40 +452,40 @@
 
         # Convert to hex str
         if is_str and not _is_hex:
             amount_hex_str = to_hex(int(amount))
         elif isinstance(amount, int) or isinstance(amount, bytes):
             amount_hex_str = to_hex(amount)
 
-        self._make_request("anvil_setBalance", [account, amount_hex_str])
+        self.make_request("anvil_setBalance", [account, amount_hex_str])
 
     def set_timestamp(self, new_timestamp: int):
-        self._make_request("evm_setNextBlockTimestamp", [new_timestamp])
+        self.make_request("evm_setNextBlockTimestamp", [new_timestamp])
 
     def mine(self, num_blocks: int = 1):
         # NOTE: Request fails when given numbers with any left padded 0s.
         num_blocks_arg = f"0x{HexBytes(num_blocks).hex().replace('0x', '').lstrip('0')}"
-        self._make_request("anvil_mine", [num_blocks_arg])
+        self.make_request("anvil_mine", [num_blocks_arg])
 
     def snapshot(self) -> str:
-        return self._make_request("evm_snapshot", [])
+        return self.make_request("evm_snapshot", [])
 
-    def revert(self, snapshot_id: SnapshotID) -> bool:
+    def restore(self, snapshot_id: SnapshotID) -> bool:
         if isinstance(snapshot_id, int):
             snapshot_id = HexBytes(snapshot_id).hex()
 
-        result = self._make_request("evm_revert", [snapshot_id])
+        result = self.make_request("evm_revert", [snapshot_id])
         return result is True
 
     def unlock_account(self, address: AddressType) -> bool:
-        self._make_request("anvil_impersonateAccount", [address])
+        self.make_request("anvil_impersonateAccount", [address])
         return True
 
     def relock_account(self, address: AddressType):
-        self._make_request("anvil_stopImpersonatingAccount", [address])
+        self.make_request("anvil_stopImpersonatingAccount", [address])
         if address in self.account_manager.test_accounts._impersonated_accounts:
             del self.account_manager.test_accounts._impersonated_accounts[address]
 
     def send_transaction(self, txn: TransactionAPI) -> ReceiptAPI:
         """
         Creates a new message call transaction or a contract creation
         for signed transactions.
@@ -577,145 +558,34 @@
             # If we get here, for some reason the tx-replay did not produce
             # a VM error.
             receipt.raise_for_status()
 
         self.chain_manager.history.append(receipt)
         return receipt
 
-    def send_call(
-        self,
-        txn: TransactionAPI,
-        block_id: Optional[BlockID] = None,
-        state: Optional[Dict] = None,
-        **kwargs,
-    ) -> HexBytes:
-        if block_id is not None:
-            kwargs["block_identifier"] = block_id
-        if state is not None:
-            kwargs["state_override"] = state
-        skip_trace = kwargs.pop("skip_trace", False)
-        arguments = self._prepare_call(txn, **kwargs)
-
-        if skip_trace:
-            return self._eth_call(arguments)
-
-        show_gas = kwargs.pop("show_gas_report", False)
-        show_trace = kwargs.pop("show_trace", False)
-
-        if self._test_runner is not None:
-            track_gas = self._test_runner.gas_tracker.enabled
-            track_coverage = self._test_runner.coverage_tracker.enabled
-        else:
-            track_gas = False
-            track_coverage = False
-
-        needs_trace = track_gas or track_coverage or show_gas or show_trace
-        if not needs_trace:
-            return self._eth_call(arguments)
-
-        # The user is requesting information related to a call's trace,
-        # such as gas usage data.
-
-        if "type" in arguments[0] and isinstance(arguments[0]["type"], int):
-            arguments[0]["type"] = to_hex(arguments[0]["type"])
-
-        result, trace_frames = self._trace_call(arguments)
-        trace_frames, frames_copy = tee(trace_frames)
-        return_value = HexBytes(result["returnValue"])
-        root_node_kwargs = {
-            "gas_cost": result.get("gas", 0),
-            "address": txn.receiver,
-            "calldata": txn.data,
-            "value": txn.value,
-            "call_type": CallType.CALL,
-            "failed": False,
-            "returndata": return_value,
-        }
-
-        evm_call_tree = get_calltree_from_geth_trace(trace_frames, **root_node_kwargs)
-
-        # NOTE: Don't pass txn_hash here, as it will fail (this is not a real txn).
-        call_tree = self._create_call_tree_node(evm_call_tree)
-
-        receiver = txn.receiver
-        if track_gas and show_gas and not show_trace:
-            # Optimization to enrich early and in_place=True.
-            call_tree.enrich()
-
-        if track_gas and call_tree and receiver is not None and self._test_runner is not None:
-            # Gas report being collected, likely for showing a report
-            # at the end of a test run.
-            # Use `in_place=False` in case also `show_trace=True`
-            enriched_call_tree = call_tree.enrich(in_place=False)
-            self._test_runner.gas_tracker.append_gas(enriched_call_tree, receiver)
-
-        if track_coverage and self._test_runner is not None and receiver:
-            contract_type = self.chain_manager.contracts.get(receiver)
-            if contract_type:
-                traceframes = (self._create_trace_frame(x) for x in frames_copy)
-                method_id = HexBytes(txn.data)
-                selector = (
-                    contract_type.methods[method_id].selector
-                    if method_id in contract_type.methods
-                    else None
-                )
-                source_traceback = SourceTraceback.create(contract_type, traceframes, method_id)
-                self._test_runner.coverage_tracker.cover(
-                    source_traceback, function=selector, contract=contract_type.name
-                )
-
-        if show_gas:
-            enriched_call_tree = call_tree.enrich(in_place=False)
-            self.chain_manager._reports.show_gas(enriched_call_tree)
-
-        if show_trace:
-            call_tree = call_tree.enrich(use_symbol_for_tokens=True)
-            self.chain_manager._reports.show_trace(call_tree)
-
-        return return_value
-
-    def _trace_call(self, arguments: List[Any]) -> Tuple[Dict, Iterator[EvmTraceFrame]]:
-        result = self._make_request("debug_traceCall", arguments)
-        trace_data = result.get("structLogs", [])
-        return result, (EvmTraceFrame(**f) for f in trace_data)
-
     def get_balance(self, address: AddressType, block_id: Optional[BlockID] = None) -> int:
         if hasattr(address, "address"):
             address = address.address
 
-        result = self._make_request("eth_getBalance", [address, "latest"])
+        result = self.make_request("eth_getBalance", [address, block_id])
         if not result:
             raise FoundryProviderError(f"Failed to get balance for account '{address}'.")
 
         return int(result, 16) if isinstance(result, str) else result
 
-    def get_transaction_trace(self, txn_hash: str) -> Iterator[TraceFrame]:
-        for trace in self._get_transaction_trace(txn_hash):
-            yield self._create_trace_frame(trace)
-
-    def _get_transaction_trace(
-        self, txn_hash: str, steps_tracing: bool = True, enable_memory: bool = True
-    ) -> Iterator[EvmTraceFrame]:
-        result = self._make_request(
-            "debug_traceTransaction",
-            [txn_hash, {"stepsTracing": steps_tracing, "enableMemory": enable_memory}],
-        )
-        frames = result.get("structLogs", [])
-        for frame in frames:
-            yield EvmTraceFrame(**frame)
-
-    def get_call_tree(self, txn_hash: str) -> CallTreeNode:
-        raw_trace_list = self._make_request("trace_transaction", [txn_hash])
-        trace_list = ParityTraceList.model_validate(raw_trace_list)
+    def get_transaction_trace(self, transaction_hash: str, **kwargs) -> TraceAPI:
+        if "debug_trace_transaction_parameters" not in kwargs:
+            kwargs["debug_trace_transaction_parameters"] = {
+                "stepsTracing": True,
+                "enableMemory": True,
+            }
+        if "call_trace_approach" not in kwargs:
+            kwargs["call_trace_approach"] = TraceApproach.PARITY
 
-        if not trace_list:
-            raise FoundryProviderError(f"No trace found for transaction '{txn_hash}'")
-
-        evm_call = get_calltree_from_parity_trace(trace_list)
-        return self._create_call_tree_node(evm_call, txn_hash=txn_hash)
+        return _get_transaction_trace(transaction_hash, **kwargs)
 
     def get_virtual_machine_error(self, exception: Exception, **kwargs) -> VirtualMachineError:
         if not len(exception.args):
             return VirtualMachineError(base_err=exception, **kwargs)
 
         err_data = exception.args[0]
         message = str(err_data.get("message")) if isinstance(err_data, dict) else err_data
@@ -756,18 +626,18 @@
 
         elif "Transaction reverted without a reason string" in message:
             return _handle_execution_reverted(exception, **kwargs)
 
         elif message.lower() == "execution reverted":
             message = TransactionError.DEFAULT_MESSAGE
             if isinstance(exception, Web3ContractLogicError) and (
-                msg := _extract_custom_error(self, **kwargs)
+                msg := self._extract_custom_error(**kwargs)
             ):
-                if msg not in ("", "0x", None):
-                    message = msg
+                exception.message = msg
+
             return _handle_execution_reverted(exception, revert_message=message, **kwargs)
 
         elif message == "Transaction ran out of gas" or "OutOfGas" in message:
             return OutOfGasError(base_err=exception, **kwargs)
 
         elif message.startswith("execution reverted: "):
             message = (
@@ -779,79 +649,69 @@
         elif isinstance(exception, ContractCustomError):
             # Is raw hex (custom exception)
             message = TransactionError.DEFAULT_MESSAGE if message in ("", None, "0x") else message
             return _handle_execution_reverted(exception, revert_message=message, **kwargs)
 
         return VirtualMachineError(message, **kwargs)
 
+    # Abstracted for easier testing conditions.
+    def _extract_custom_error(self, **kwargs) -> str:
+        # Check for custom error.
+        trace = None
+        if "trace" in kwargs:
+            trace = kwargs["trace"]
+
+        elif "txn" in kwargs:
+            txn = kwargs["txn"]
+            try:
+                txn_hash = txn.txn_hash if isinstance(txn.txn_hash, str) else txn.txn_hash.hex()
+                trace = self.get_transaction_trace(txn_hash)
+            except Exception:
+                pass
+
+        if trace is not None and (revert_msg := trace.revert_message):
+            return revert_msg
+
+        return ""
+
     def set_block_gas_limit(self, gas_limit: int) -> bool:
-        return self._make_request("evm_setBlockGasLimit", [hex(gas_limit)]) is True
+        return self.make_request("evm_setBlockGasLimit", [hex(gas_limit)]) is True
 
     def set_code(self, address: AddressType, code: ContractCode) -> bool:
         if isinstance(code, bytes):
             code = code.hex()
 
         elif isinstance(code, str) and not is_0x_prefixed(code):
             code = add_0x_prefix(HexStr(code))
 
         elif not is_hex(code):
             raise ValueError(f"Value {code} is not convertible to hex")
 
-        self._make_request("anvil_setCode", [address, code])
+        self.make_request("anvil_setCode", [address, code])
         return True
 
     def set_storage(self, address: AddressType, slot: int, value: HexBytes):
-        self._make_request(
+        self.make_request(
             "anvil_setStorageAt",
             [
                 address,
                 HashBytes32.__eth_pydantic_validate__(slot).hex(),
                 HashBytes32.__eth_pydantic_validate__(value).hex(),
             ],
         )
 
-    def _eth_call(self, arguments: List) -> HexBytes:
-        # Override from Web3Provider because foundry is pickier.
-
+    def _eth_call(self, arguments: list) -> HexBytes:
+        # Overridden to handle unique Foundry pickiness.
         txn_dict = copy(arguments[0])
         if isinstance(txn_dict.get("type"), int):
             txn_dict["type"] = HexBytes(txn_dict["type"]).hex()
 
         txn_dict.pop("chainId", None)
         arguments[0] = txn_dict
-        trace = None
-
-        try:
-            result = self._make_request("eth_call", arguments)
-        except Exception as err:
-            contract_address = arguments[0].get("to") if len(arguments) > 0 else None
-            tb = None
-            if contract_address:
-                try:
-                    trace, trace2 = tee(
-                        self._create_trace_frame(x) for x in self._trace_call(arguments)[1]
-                    )
-                    contract_type = self.chain_manager.contracts.get(contract_address)
-                    method_id = arguments[0].get("data", "")[:10] or None
-                    tb = (
-                        SourceTraceback.create(contract_type, trace2, method_id)
-                        if method_id and contract_type
-                        else None
-                    )
-                except Exception as sub_err:
-                    logger.error(f"Error getting source traceback: {sub_err}")
-
-            if trace is None:
-                trace = (self._create_trace_frame(x) for x in self._trace_call(arguments)[1])
-
-            raise self.get_virtual_machine_error(
-                err, trace=trace, contract_address=contract_address, source_traceback=tb
-            ) from err
-
-        return HexBytes(result)
+        return super()._eth_call(arguments)
 
 
 class FoundryForkProvider(FoundryProvider):
     """
     A Foundry provider that uses ``--fork``, like:
     ``npx foundry node --fork <upstream-provider-url>``.
 
@@ -865,15 +725,15 @@
     def set_upstream_provider(cls, value):
         network = value["network"]
         adhoc_settings = value.get("provider_settings", {}).get("fork", {})
         ecosystem_name = network.ecosystem.name
         plugin_config = cls.config_manager.get_config(value["name"])
         config_settings = plugin_config.get("fork", {})
 
-        def _get_upstream(data: Dict) -> Optional[str]:
+        def _get_upstream(data: dict) -> Optional[str]:
             return (
                 data.get(ecosystem_name, {})
                 .get(network.name.replace("-fork", ""), {})
                 .get("upstream_provider")
             )
 
         # If upstream provider set anywhere in provider settings, ignore.
@@ -964,15 +824,15 @@
 
         if self.get_block(0).hash != upstream_genesis_block_hash:
             logger.warning(
                 "Upstream network has mismatching genesis block. "
                 "This could be an issue with foundry."
             )
 
-    def build_command(self) -> List[str]:
+    def build_command(self) -> list[str]:
         if not self.fork_url:
             raise FoundryProviderError("Upstream provider does not have a ``connection_str``.")
 
         if self.fork_url.replace("localhost", "127.0.0.1").replace("http://", "") == self.uri:
             raise FoundryProviderError(
                 "Invalid upstream-fork URL. Can't be same as local anvil node."
             )
@@ -987,41 +847,20 @@
 
         if self._fork_config.evm_version is not None:
             cmd.extend(("--hardfork", self._fork_config.evm_version))
 
         return cmd
 
     def reset_fork(self, block_number: Optional[int] = None):
-        forking_params: Dict[str, Union[str, int]] = {"jsonRpcUrl": self.fork_url}
+        forking_params: dict[str, Union[str, int]] = {"jsonRpcUrl": self.fork_url}
         block_number = block_number if block_number is not None else self.fork_block_number
         if block_number is not None:
             forking_params["blockNumber"] = block_number
 
         # # Rest the fork
-        result = self._make_request("anvil_reset", [{"forking": forking_params}])
+        result = self.make_request("anvil_reset", [{"forking": forking_params}])
         return result
 
 
-# Abstracted for easier testing conditions.
-def _extract_custom_error(provider: FoundryProvider, **kwargs) -> str:
-    data = {}
-    if "trace" in kwargs:
-        kwargs["trace"], new_trace = tee(kwargs["trace"])
-        data = list(new_trace)[-1].raw
-
-    elif "txn" in kwargs:
-        txn = kwargs["txn"]
-        txn_hash = txn.txn_hash if isinstance(txn.txn_hash, str) else txn.txn_hash.hex()
-        try:
-            trace = list(provider._get_transaction_trace(txn_hash))[-1]
-        except Exception:
-            return ""
-
-        data = trace.model_dump(by_alias=True, mode="json") if trace else {}
-
-    if data and data.get("op") == "REVERT":
-        memory = data.get("memory", [])
-        custom_err = "".join([x[2:] for x in memory[4:]])
-        if custom_err:
-            return f"0x{custom_err}"
-
-    return ""
+def _get_transaction_trace(transaction_hash: str, **kwargs) -> TraceAPI:
+    # Abstracted for testing purposes.
+    return TransactionTrace(transaction_hash=transaction_hash, **kwargs)
```

### Comparing `ape-foundry-0.7.5/ape_foundry.egg-info/PKG-INFO` & `ape-foundry-0.8.0/ape_foundry.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: ape-foundry
-Version: 0.7.5
+Version: 0.8.0
 Summary: ape-foundry: Ape network provider for Foundry
 Home-page: https://github.com/ApeWorX/ape-foundry
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
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -31,15 +30,15 @@
 # Quick Start
 
 Foundry network provider plugin for Ape.
 Foundry is a development framework written in Rust for Ethereum that includes a local network implementation.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 - Foundry. See Foundry's [Installation](https://github.com/foundry-rs/foundry#installation) documentation for steps.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-foundry-0.7.5/ape_foundry.egg-info/SOURCES.txt` & `ape-foundry-0.8.0/ape_foundry.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 .pre-commit-config.yaml
 CONTRIBUTING.md
 LICENSE
 README.md
+ape-config.yaml
 pyproject.toml
 setup.cfg
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
 .github/release-drafter.yml
 .github/ISSUE_TEMPLATE/bug.md
 .github/ISSUE_TEMPLATE/feature.md
@@ -27,15 +28,14 @@
 ape_foundry.egg-info/PKG-INFO
 ape_foundry.egg-info/SOURCES.txt
 ape_foundry.egg-info/dependency_links.txt
 ape_foundry.egg-info/not-zip-safe
 ape_foundry.egg-info/requires.txt
 ape_foundry.egg-info/top_level.txt
 tests/__init__.py
-tests/ape-config.yaml
 tests/conftest.py
 tests/expected_traces.py
 tests/test_fork_provider.py
 tests/test_provider.py
 tests/test_pytest.py
 tests/test_trace.py
 tests/data/contracts/ethereum/local/contract_a.json
```

### Comparing `ape-foundry-0.7.5/ape_foundry.egg-info/requires.txt` & `ape-foundry-0.8.0/ape_foundry.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-eth-ape<0.8,>=0.7.4
+eth-ape<0.9,>=0.8.1
 ethpm-types
 eth-pydantic-types
 evm-trace
 web3
 yarl
 hexbytes
```

### Comparing `ape-foundry-0.7.5/pyproject.toml` & `ape-foundry-0.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
+target-version = ['py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ape-foundry-0.7.5/setup.py` & `ape-foundry-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-foundry",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.4,<0.8",
+        "eth-ape>=0.8.1,<0.9",
         "ethpm-types",  # Use same version as eth-ape
         "eth-pydantic-types",  # Use same version as eth-ape
         "evm-trace",  # Use same version as ape
         "web3",  # Use same version as ape
         "yarl",  # Use same version as ape
         "hexbytes",  # Use same version as ape
     ],
@@ -92,14 +92,13 @@
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

### Comparing `ape-foundry-0.7.5/tests/ape-config.yaml` & `ape-foundry-0.8.0/ape-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-contracts_folder: data/contracts/ethereum/local
+contracts_folder: tests/data/contracts/ethereum/local
 
 ethereum:
   mainnet:
     default_provider: alchemy
   local:
     default_provider: foundry
 
@@ -24,14 +24,17 @@
     ethereum:
       mainnet:
         upstream_provider: alchemy
         block_number: 15776634
       sepolia:
         upstream_provider: alchemy
         block_number: 3091950
+      holesky:
+        upstream_provider: alchemy
+        block_number: 100
 
 test:
   # `false` because running pytest within pytest.
   disconnect_providers_after: false
 
   gas:
     exclude:
```

### Comparing `ape-foundry-0.7.5/tests/conftest.py` & `ape-foundry-0.8.0/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-import json
 import os
-import tempfile
+import shutil
 from contextlib import contextmanager
 from pathlib import Path
 from tempfile import mkdtemp
-from typing import Dict, Optional
 
 import ape
 import pytest
-import yaml
 from _pytest.runner import pytest_runtest_makereport as orig_pytest_runtest_makereport
 from ape.contracts import ContractContainer
 from ape.exceptions import APINotImplementedError, UnknownSnapshotError
-from ape.managers.config import CONFIG_FILE_NAME
 from ethpm_types import ContractType
 
 from ape_foundry import FoundryProvider
 
 # NOTE: Ensure that we don't use local paths for the DATA FOLDER
-ape.config.DATA_FOLDER = Path(mkdtemp()).resolve()
+DATA_FOLDER = Path(mkdtemp()).resolve()
+ape.config.DATA_FOLDER = DATA_FOLDER
 
 BASE_CONTRACTS_PATH = Path(__file__).parent / "data" / "contracts"
 LOCAL_CONTRACTS_PATH = BASE_CONTRACTS_PATH / "ethereum" / "local"
 NAME = "foundry"
 
 # Needed to test tracing support in core `ape test` command.
 pytest_plugins = ["pytester"]
@@ -41,17 +38,17 @@
 
 @pytest.fixture(scope="session")
 def name():
     return NAME
 
 
 @pytest.fixture(scope="session", autouse=True)
-def in_tests_dir(config):
-    with config.using_project(Path(__file__).parent):
-        yield
+def clean_datafodler(config):
+    yield  # Run all collected tests.
+    shutil.rmtree(DATA_FOLDER, ignore_errors=True)
 
 
 @contextmanager
 def _isolate():
     if ape.networks.active_provider is None:
         raise AssertionError("Isolation should only be used with a connected provider.")
 
@@ -238,41 +235,14 @@
 def sepolia_fork_provider(name, ethereum, sepolia_fork_port):
     with ethereum.sepolia_fork.use_provider(
         name, provider_settings={"host": f"http://127.0.0.1:{sepolia_fork_port}"}
     ) as provider:
         yield provider
 
 
-@pytest.fixture(scope="session")
-def temp_config(config):
-    @contextmanager
-    def func(data: Dict, package_json: Optional[Dict] = None):
-        # TODO: Use `ape.utils.use_tempdir()` (once released)
-        with tempfile.TemporaryDirectory() as temp_dir_str:
-            temp_dir = Path(temp_dir_str).resolve()
-
-            config._cached_configs = {}
-            config_file = temp_dir / CONFIG_FILE_NAME
-            config_file.touch()
-            config_file.write_text(yaml.dump(data))
-            config.load(force_reload=True)
-
-            if package_json:
-                package_json_file = temp_dir / "package.json"
-                package_json_file.write_text(json.dumps(package_json))
-
-            with config.using_project(temp_dir):
-                yield temp_dir
-
-            config_file.unlink()
-            config._cached_configs = {}
-
-    return func
-
-
 @pytest.fixture
 def contract_a(owner, connected_provider, get_contract_type):
     contract_c = owner.deploy(ContractContainer(get_contract_type("contract_c")))
     contract_b = owner.deploy(
         ContractContainer(get_contract_type("contract_b")), contract_c.address
     )
     contract_a = owner.deploy(
```

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/contract_a.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/local/contract_a.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/contract_b.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/local/contract_b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/contract_c.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/local/contract_c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/has_error.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/local/has_error.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/solidity_contract.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/local/solidity_contract.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/token_a.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/local/token_a.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/token_b.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/local/token_b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/vyper_contract.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/local/vyper_contract.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json` & `ape-foundry-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/python/pytest_tests.py` & `ape-foundry-0.8.0/tests/data/python/pytest_tests.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/sources/RevertsContractVy.vy` & `ape-foundry-0.8.0/tests/data/sources/RevertsContractVy.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/sources/TokenA.vy` & `ape-foundry-0.8.0/tests/data/sources/TokenA.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/data/sources/TokenB.vy` & `ape-foundry-0.8.0/tests/data/sources/TokenB.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.5/tests/expected_traces.py` & `ape-foundry-0.8.0/tests/expected_traces.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 │       \],
 │       \[234444, 92222229999998888882, 3454\],
 │       \[
 │         111145345347789999991,
 │         333399998888882,
 │         234545457847457457458457457457
 │       \]
-│     \] \[\d+ gas\]
+│   \] \[\d+ gas\]
 ├── SYMBOL\.methodB1\(lolol="ice-cream", dynamo=345457847457457458457457457\) \[\d+ gas\]
 │   ├── ContractC\.getSomeList\(\) -> \[
 │   │     3425311345134513461345134534531452345,
 │   │     111344445534535353,
 │   │     993453434534534534534977788884443333
 │   │   \] \[\d+ gas\]
 │   └── ContractC\.methodC1\(
```

### Comparing `ape-foundry-0.7.5/tests/test_fork_provider.py` & `ape-foundry-0.8.0/tests/test_fork_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import tempfile
 from pathlib import Path
 
 import pytest
 from ape.api.networks import LOCAL_NETWORK_NAME
 from ape.contracts import ContractInstance
 from ape.exceptions import ContractLogicError
 from ape_ethereum.ecosystem import NETWORKS
@@ -44,16 +43,15 @@
         assert networks.active_provider.uri == mainnet_fork_host
 
     assert networks.active_provider.name == name
     assert networks.active_provider.network.name == LOCAL_NETWORK_NAME
     assert networks.active_provider.uri == default_host
 
 
-# TODO: Remove `in` check once goerli removed from core.
-@pytest.mark.parametrize("network", [k for k in NETWORKS.keys() if k not in ("goerli",)])
+@pytest.mark.parametrize("network", NETWORKS)
 def test_fork_config(name, config, network):
     plugin_config = config.get_config(name)
     network_config = plugin_config["fork"].get("ethereum", {}).get(network, {})
     message = f"Config not registered for network '{network}'."
     assert network_config.get("upstream_provider") == "alchemy", message
 
 
@@ -74,25 +72,22 @@
     impersonated_account.balance += 1_000_000_000_000_000_000
     receipt = impersonated_account.transfer(other_account, "1 wei")
     assert receipt.receiver == other_account
     assert receipt.sender == impersonated_account
 
 
 @pytest.mark.fork
-def test_request_timeout(networks, config, mainnet_fork_provider):
+def test_request_timeout(networks, project, mainnet_fork_provider):
     actual = mainnet_fork_provider.web3.provider._request_kwargs["timeout"]
     expected = 360  # Value set in `ape-config.yaml`
     assert actual == expected
 
     # Test default behavior
-    # TODO: Use `ape.utils.use_tempdir()` (once released)
-    with tempfile.TemporaryDirectory() as temp_dir_str:
-        temp_dir = Path(temp_dir_str).resolve()
-        with config.using_project(temp_dir):
-            assert networks.active_provider.timeout == 300
+    with project.temp_config(foundry={"fork_request_timeout": 300}):
+        assert networks.active_provider.timeout == 300
 
 
 @pytest.mark.fork
 def test_reset_fork_no_fork_block_number(sepolia_fork_provider):
     sepolia_fork_provider.mine(5)
     prev_block_num = sepolia_fork_provider.get_block("latest").number
     sepolia_fork_provider.reset_fork()
```

### Comparing `ape-foundry-0.7.5/tests/test_provider.py` & `ape-foundry-0.8.0/tests/test_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import os
-import tempfile
-from pathlib import Path
 
 import pytest
+from ape.api import TraceAPI
 from ape.api.accounts import ImpersonatedAccount
 from ape.contracts import ContractContainer
 from ape.exceptions import ContractLogicError, TransactionError
-from ape.types import CallTreeNode, TraceFrame
+from ape_ethereum.trace import Trace
 from ape_ethereum.transactions import TransactionStatusEnum, TransactionType
 from eth_pydantic_types import HashBytes32
-from eth_utils import encode_hex, to_int
+from eth_utils import to_int
 from evm_trace import CallType
 from hexbytes import HexBytes
 
 from ape_foundry import FoundryProviderError
-from ape_foundry.provider import FOUNDRY_CHAIN_ID, FoundryNetworkConfig, _extract_custom_error
+from ape_foundry.provider import FOUNDRY_CHAIN_ID, FoundryNetworkConfig
 
 TEST_WALLET_ADDRESS = "0xD9b7fdb3FC0A0Aa3A507dCf0976bc23D49a9C7A3"
 
 
 def test_instantiation(disconnected_provider, name):
     assert disconnected_provider.name == name
 
@@ -69,46 +68,45 @@
 def test_mine(connected_provider):
     block_num = connected_provider.get_block("latest").number
     connected_provider.mine(100)
     next_block_num = connected_provider.get_block("latest").number
     assert next_block_num > block_num
 
 
-def test_revert_failure(connected_provider):
-    assert connected_provider.revert(0xFFFF) is False
+def test_restore_failure(connected_provider):
+    assert connected_provider.restore(0xFFFF) is False
 
 
 def test_get_balance(connected_provider, owner):
     assert connected_provider.get_balance(owner.address)
 
 
-def test_snapshot_and_revert(connected_provider):
+def test_snapshot_and_restore(connected_provider):
     snap = connected_provider.snapshot()
 
     block_1 = connected_provider.get_block("latest")
     connected_provider.mine()
     block_2 = connected_provider.get_block("latest")
     assert block_2.number > block_1.number
     assert block_1.hash != block_2.hash
 
-    connected_provider.revert(snap)
+    connected_provider.restore(snap)
     block_3 = connected_provider.get_block("latest")
     assert block_1.number == block_3.number
     assert block_1.hash == block_3.hash
 
 
 @pytest.mark.parametrize(
     "tx_kwargs",
     [
         {},  # NO KWARGS CASE: Should default to type 2
         {"type": 0},
         {"type": 0, "gas_price": 0},
-        # TODO: Uncomment after ape 0.7.5 is released
-        # {"type": 1},
-        # {"type": 1, "gas_price": 0},
+        {"type": 1},
+        {"type": 1, "gas_price": 0},
         {"type": 2},
         {"type": 2, "max_priority_fee": 0},
         {"type": 2, "base_fee": 0, "max_priority_fee": 0},
     ],
 )
 def test_unlock_account(connected_provider, contract_a, accounts, tx_kwargs):
     actual = connected_provider.unlock_account(TEST_WALLET_ADDRESS)
@@ -133,41 +131,40 @@
 
     assert not receipt_0.failed
 
 
 def test_get_transaction_trace(connected_provider, contract_instance, owner):
     receipt = contract_instance.setNumber(10, sender=owner)
 
+    actual = connected_provider.get_transaction_trace(receipt.txn_hash)
+    assert isinstance(actual, TraceAPI), f"{type(actual)}"
+    assert actual == receipt.trace
+
     # Indirectly calls `connected_provider.get_transaction_trace()`
-    frame_data = list(receipt.trace)
-    assert frame_data
-    for frame in frame_data:
-        assert isinstance(frame, TraceFrame)
+    assert isinstance(receipt.trace, TraceAPI)
 
 
-def test_get_call_tree(connected_provider, sender, receiver):
+def test_get_transaction_trace_call_tree(connected_provider, sender, receiver):
     transfer = sender.transfer(receiver, 1)
-    call_tree = connected_provider.get_call_tree(transfer.txn_hash)
-    assert isinstance(call_tree, CallTreeNode)
-    assert call_tree.call_type == CallType.CALL.value
-    assert repr(call_tree) == "0x70997970C51812dc3A010C7d01b50e0d17dc79C8.0x()"
+    trace = connected_provider.get_transaction_trace(transfer.txn_hash)
+    assert isinstance(trace, Trace)
+    call_tree = trace.get_calltree()
+    assert call_tree.call_type == CallType.CALL
+    assert repr(trace) == "__ETH_transfer__.0x() 1"
 
 
-def test_request_timeout(connected_provider, config):
+def test_request_timeout(connected_provider, project):
     # Test value set in `ape-config.yaml`
     expected = 29
     actual = connected_provider.web3.provider._request_kwargs["timeout"]
     assert actual == expected
 
     # Test default behavior
-    # TODO: Use `ape.utils.use_tempdir()` (once released)
-    with tempfile.TemporaryDirectory() as temp_dir_str:
-        temp_dir = Path(temp_dir_str).resolve()
-        with config.using_project(temp_dir):
-            assert connected_provider.timeout == 30
+    with project.temp_config(foundry={"timeout": 30}):
+        assert connected_provider.timeout == 30
 
 
 def test_contract_interaction(connected_provider, owner, contract_instance, mocker):
     # Spy on the estimate_gas RPC method.
     estimate_gas_spy = mocker.spy(connected_provider.web3.eth, "estimate_gas")
 
     # Check what max gas is before transacting.
@@ -268,31 +265,30 @@
     acct = accounts[TEST_WALLET_ADDRESS]
     acct.balance = "1000 ETH"
     with pytest.raises(error_contract.Unauthorized):
         error_contract.withdraw(sender=acct)
 
 
 @pytest.mark.parametrize("host", ("https://example.com", "example.com"))
-def test_host(temp_config, local_network, host):
-    data = {"foundry": {"host": host}}
-    with temp_config(data):
+def test_host(project, local_network, host):
+    with project.temp_config(foundry={"host": host}):
         provider = local_network.get_provider("foundry")
         assert provider.uri == "https://example.com"
 
 
-def test_base_fee(connected_provider, temp_config, networks, accounts):
+def test_base_fee(connected_provider, project, networks, accounts):
     assert connected_provider.base_fee == 0
 
     acct1 = accounts[-1]
     acct2 = accounts[-2]
 
     # Show we can se the base-fee.
     new_base_fee = 1_000_000
-    data = {"foundry": {"base_fee": new_base_fee, "host": "http://127.0.0.1:8555"}}
-    with temp_config(data):
+    data = {"base_fee": new_base_fee, "host": "http://127.0.0.1:8555"}
+    with project.temp_config(foundry=data):
         with networks.ethereum.local.use_provider("foundry") as provider:
             # Verify the block has the right base fee
             block_one = provider.get_block("latest")
             assert block_one.base_fee == new_base_fee
 
             # Make sure the command has the right base fee
             cmd = provider.build_command()
@@ -332,45 +328,42 @@
 ):
     exception = Exception(message)
     actual = connected_provider.get_virtual_machine_error(exception)
     assert isinstance(actual, ContractLogicError)
     assert actual.base_err == exception
 
 
-def test_no_mining(temp_config, local_network, connected_provider):
+def test_no_mining(project, local_network, connected_provider):
     assert "--no-mining" not in connected_provider.build_command()
-    data = {"foundry": {"auto_mine": "false"}}
-    with temp_config(data):
+    with project.temp_config(foundry={"auto_mine": "false"}):
         provider = local_network.get_provider("foundry")
         cmd = provider.build_command()
         assert "--no-mining" in cmd
 
 
-def test_block_time(temp_config, local_network, connected_provider):
+def test_block_time(project, local_network, connected_provider):
     assert "--block-time" not in connected_provider.build_command()
-    data = {"foundry": {"block_time": 10}}
-    with temp_config(data):
+    with project.temp_config(foundry={"block_time": 10}):
         provider = local_network.get_provider("foundry")
         cmd = provider.build_command()
         assert "--block-time" in cmd
         assert "10" in cmd
 
 
-def test_remote_host(temp_config, local_network, no_anvil_bin):
-    data = {"foundry": {"host": "https://example.com"}}
-    with temp_config(data):
+def test_remote_host(project, local_network, no_anvil_bin):
+    with project.temp_config(foundry={"host": "https://example.com"}):
         with pytest.raises(
             FoundryProviderError,
             match=r"Failed to connect to remote Anvil node at 'https://example.com'\.",
         ):
             with local_network.use_provider("foundry"):
                 assert True
 
 
-def test_remote_host_using_env_var(temp_config, local_network, no_anvil_bin):
+def test_remote_host_using_env_var(local_network, no_anvil_bin):
     original = os.environ.get("APE_FOUNDRY_HOST")
     os.environ["APE_FOUNDRY_HOST"] = "https://example2.com"
 
     try:
         with pytest.raises(
             FoundryProviderError,
             match=r"Failed to connect to remote Anvil node at 'https://example2.com'\.",
@@ -437,61 +430,21 @@
     assert tx.gas_limit is None, "Test setup failed - couldn't clear tx gas limit."
 
     # NOTE: The local network by default uses max_gas.
     actual = connected_provider.prepare_transaction(tx)
     assert actual.gas_limit == connected_provider.max_gas
 
 
-def test_disable_block_gas_limit(temp_config, disconnected_provider):
+def test_disable_block_gas_limit(project, disconnected_provider):
     # Ensure it is disabled by default.
     cmd = disconnected_provider.build_command()
     assert "--disable-block-gas-limit" not in cmd
 
     # Show we can enable it.
-    data = {"foundry": {"disable_block_gas_limit": True}}
-    with temp_config(data):
+    with project.temp_config(foundry={"disable_block_gas_limit": True}):
         cmd = disconnected_provider.build_command()
         assert "--disable-block-gas-limit" in cmd
 
 
-def test_extract_custom_error_trace_given(mocker):
-    provider = mocker.MagicMock()
-    trace = mocker.MagicMock()
-    trace.raw = {"op": "REVERT", "memory": [None, None, None, None, encode_hex("CustomError")]}
-    trace = iter([trace])
-    actual = _extract_custom_error(provider, trace=trace)
-    assert actual.startswith("0x")
-
-
-def test_extract_custom_error_transaction_given(
-    connected_provider, vyper_contract_instance, not_owner
-):
-    with pytest.raises(ContractLogicError) as err:
-        vyper_contract_instance.setNumber(546, sender=not_owner, allow_fail=True)
-
-    actual = _extract_custom_error(connected_provider, txn=err.value.txn)
-    assert actual == ""
-
-
-@pytest.mark.parametrize("tx_hash", ("0x0123", HexBytes("0x0123")))
-def test_extract_custom_error_transaction_given_trace_fails(mocker, tx_hash):
-    provider = mocker.MagicMock()
-    tx = mocker.MagicMock()
-    tx.txn_hash = tx_hash
-    tracker = []
-
-    def trace(txn_hash: str, *args, **kwargs):
-        tracker.append(txn_hash)
-        raise ValueError("Connection failed.")
-
-    provider._get_transaction_trace.side_effect = trace
-
-    actual = _extract_custom_error(provider, txn=tx)
-    assert actual == ""
-
-    # Show failure was tracked
-    assert tracker[0] == HexBytes(tx.txn_hash).hex()
-
-
 def test_fork_config_none():
     cfg = FoundryNetworkConfig.model_validate({"fork": None})
     assert isinstance(cfg["fork"], dict)
```

### Comparing `ape-foundry-0.7.5/tests/test_pytest.py` & `ape-foundry-0.8.0/tests/test_pytest.py`

 * *Files identical despite different names*

