# Comparing `tmp/ape-hardhat-0.7.3.tar.gz` & `tmp/ape-hardhat-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-hardhat-0.7.3.tar", last modified: Fri May 10 14:48:46 2024, max compression
+gzip compressed data, was "ape-hardhat-0.8.0.tar", last modified: Sat Jun  1 01:40:28 2024, max compression
```

## Comparing `ape-hardhat-0.7.3.tar` & `ape-hardhat-0.8.0.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.213968 ape-hardhat-0.7.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.197968 ape-hardhat-0.7.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.201968 ape-hardhat-0.7.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.201968 ape-hardhat-0.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-10 14:48:46.213968 ape-hardhat-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.201968 ape-hardhat-0.7.3/ape_hardhat/
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/ape_hardhat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/ape_hardhat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    42370 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/ape_hardhat/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/ape_hardhat/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 14:48:45.000000 ape-hardhat-0.7.3/ape_hardhat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.201968 ape-hardhat-0.7.3/ape_hardhat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-10 14:48:46.000000 ape-hardhat-0.7.3/ape_hardhat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-05-10 14:48:46.000000 ape-hardhat-0.7.3/ape_hardhat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:48:46.000000 ape-hardhat-0.7.3/ape_hardhat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:48:46.000000 ape-hardhat-0.7.3/ape_hardhat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-10 14:48:46.000000 ape-hardhat-0.7.3/ape_hardhat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 14:48:46.000000 ape-hardhat-0.7.3/ape_hardhat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-10 14:48:46.213968 ape-hardhat-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.201968 ape-hardhat-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.197968 ape-hardhat-0.7.3/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.197968 ape-hardhat-0.7.3/tests/data/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.197968 ape-hardhat-0.7.3/tests/data/contracts/ethereum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.205968 ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/
--rw-r--r--   0 runner    (1001) docker     (127)    28685 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/contract_a.json
--rw-r--r--   0 runner    (1001) docker     (127)    27534 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/contract_b.json
--rw-r--r--   0 runner    (1001) docker     (127)    14844 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/contract_c.json
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/has_error.json
--rw-r--r--   0 runner    (1001) docker     (127)    33356 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/solidity_contract.json
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/token_a.json
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/token_b.json
--rw-r--r--   0 runner    (1001) docker     (127)    28197 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/vyper_contract.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.197968 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.213968 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
--rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
--rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
--rw-r--r--   0 runner    (1001) docker     (127)    16120 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
--rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
--rw-r--r--   0 runner    (1001) docker     (127)    19792 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
--rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
--rw-r--r--   0 runner    (1001) docker     (127)    44429 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
--rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
--rw-r--r--   0 runner    (1001) docker     (127)    23253 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
--rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
--rw-r--r--   0 runner    (1001) docker     (127)    15942 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
--rw-r--r--   0 runner    (1001) docker     (127)    14160 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
--rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
--rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.213968 ape-hardhat-0.7.3/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/python/pytest_test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/python/pytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.213968 ape-hardhat-0.7.3/tests/data/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/sources/TokenA.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/sources/TokenB.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:48:46.213968 ape-hardhat-0.7.3/tests/data/sources/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/data/sources/interfaces/ISubRevertsVy.vy
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/expected_traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     9470 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/test_fork_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/test_gas_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    11385 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-10 14:47:49.000000 ape-hardhat-0.7.3/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.328464 ape-hardhat-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.312464 ape-hardhat-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.312464 ape-hardhat-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.312464 ape-hardhat-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-06-01 01:40:28.328464 ape-hardhat-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.312464 ape-hardhat-0.8.0/ape_hardhat/
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/ape_hardhat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/ape_hardhat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37382 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/ape_hardhat/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/ape_hardhat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-01 01:40:27.000000 ape-hardhat-0.8.0/ape_hardhat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.312464 ape-hardhat-0.8.0/ape_hardhat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-06-01 01:40:28.000000 ape-hardhat-0.8.0/ape_hardhat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-06-01 01:40:28.000000 ape-hardhat-0.8.0/ape_hardhat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:40:28.000000 ape-hardhat-0.8.0/ape_hardhat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:40:28.000000 ape-hardhat-0.8.0/ape_hardhat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-06-01 01:40:28.000000 ape-hardhat-0.8.0/ape_hardhat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-01 01:40:28.000000 ape-hardhat-0.8.0/ape_hardhat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-01 01:40:28.328464 ape-hardhat-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.316464 ape-hardhat-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.308464 ape-hardhat-0.8.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.308464 ape-hardhat-0.8.0/tests/data/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.308464 ape-hardhat-0.8.0/tests/data/contracts/ethereum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.316464 ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/
+-rw-r--r--   0 runner    (1001) docker     (127)    28685 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/contract_a.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27534 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/contract_b.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14844 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/contract_c.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/has_error.json
+-rw-r--r--   0 runner    (1001) docker     (127)    33356 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/solidity_contract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/token_a.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/token_b.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28197 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/vyper_contract.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.308464 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.328464 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16120 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19792 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44429 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23253 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15942 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14160 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.328464 ape-hardhat-0.8.0/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/python/pytest_test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/python/pytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.328464 ape-hardhat-0.8.0/tests/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/sources/TokenA.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/sources/TokenB.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:40:28.328464 ape-hardhat-0.8.0/tests/data/sources/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/data/sources/interfaces/ISubRevertsVy.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/expected_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/test_fork_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/test_gas_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-06-01 01:39:34.000000 ape-hardhat-0.8.0/tests/test_trace.py
```

### Comparing `ape-hardhat-0.7.3/.github/ISSUE_TEMPLATE/bug.md` & `ape-hardhat-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/.github/ISSUE_TEMPLATE/feature.md` & `ape-hardhat-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/.github/ISSUE_TEMPLATE/work-item.md` & `ape-hardhat-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/.github/release-drafter.yml` & `ape-hardhat-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/.github/workflows/codeql.yml` & `ape-hardhat-0.8.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/.github/workflows/commit.yaml` & `ape-hardhat-0.8.0/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/.github/workflows/prtitle.yaml` & `ape-hardhat-0.8.0/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/.github/workflows/publish.yaml` & `ape-hardhat-0.8.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/.github/workflows/stale-prs.yml` & `ape-hardhat-0.8.0/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/.github/workflows/test.yaml` & `ape-hardhat-0.8.0/.github/workflows/test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 # TODO: Replace with macos-latest when works again.
                 #   https://github.com/actions/setup-python/issues/808
-                python-version: [3.8, 3.9, "3.10", "3.11", "3.12"]
+                python-version: [3.9, "3.10", "3.11", "3.12"]
                 os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
 
         steps:
         - uses: actions/checkout@v4
 
         - name: Setup Python
           uses: actions/setup-python@v5
@@ -76,15 +76,15 @@
 
         - name: Setup Node
           uses: actions/setup-node@v3
           with:
               node-version: '18'
 
         - name: Install Node Dependencies
-          run: pushd tests && npm install --save-dev hardhat && popd
+          run: npm install --save-dev hardhat
 
         - name: Run Async Tests
           run: pytest -m "not fork and not manual and not fuzzing"
 
         - name: Run Sync Tests
           # Only run forked-network tests if not from a forked repo (Else it always fails)
           if: github.event.pull_request.head.repo.full_name == github.repository
```

### Comparing `ape-hardhat-0.7.3/.gitignore` & `ape-hardhat-0.8.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -115,20 +115,21 @@
 .dmypy.json
 dmypy.json
 
 # setuptools-scm
 version.py
 
 # Ape stuff
-tests/hardhat.config.js
+hardhat.config.js
+hardhat.config.ts
 
 # NPM
 package.json
 package-lock.json
 node_modules/
 
 # Hardhat
-tests/**/cache
+**/cache
 
 **/.DS_Store
 *.swp
 *.swo
```

### Comparing `ape-hardhat-0.7.3/.pre-commit-config.yaml` & `ape-hardhat-0.8.0/.pre-commit-config.yaml`

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

### Comparing `ape-hardhat-0.7.3/CONTRIBUTING.md` & `ape-hardhat-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/LICENSE` & `ape-hardhat-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/PKG-INFO` & `ape-hardhat-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: ape-hardhat
-Version: 0.7.3
+Version: 0.8.0
 Summary: ape-hardhat: Ape network provider for Hardhat
 Home-page: https://github.com/ApeWorX/ape-hardhat
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
@@ -32,15 +31,15 @@
 
 This is a Hardhat network provider plugin for Ape.
 Hardhat is a development framework written in Node.js for Ethereum that includes a local network implementation.
 Use this plugin to manage a Hardhat node process or connect to an existing one.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 - Node.js, NPM, and Hardhat 2.12.0 or greater. See Hardhat's [Installation](https://hardhat.org/getting-started/#installation%3E) documentation for steps.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-hardhat-0.7.3/README.md` & `ape-hardhat-0.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This is a Hardhat network provider plugin for Ape.
 Hardhat is a development framework written in Node.js for Ethereum that includes a local network implementation.
 Use this plugin to manage a Hardhat node process or connect to an existing one.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 - Node.js, NPM, and Hardhat 2.12.0 or greater. See Hardhat's [Installation](https://hardhat.org/getting-started/#installation%3E) documentation for steps.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-hardhat-0.7.3/ape_hardhat/__init__.py` & `ape-hardhat-0.8.0/ape_hardhat/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/ape_hardhat/exceptions.py` & `ape-hardhat-0.8.0/ape_hardhat/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/ape_hardhat/provider.py` & `ape-hardhat-0.8.0/ape_hardhat/provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,43 @@
 import json
 import random
 import re
 import shutil
-from itertools import tee
 from pathlib import Path
 from subprocess import PIPE, CalledProcessError, call, check_output
-from typing import Any, Dict, Iterator, List, Literal, Optional, Tuple, Union, cast
+from typing import Literal, Optional, Union, cast
 
 from ape.api import (
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
     RPCTimeoutError,
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
+from ape.types import AddressType, ContractCode, SnapshotID
 from ape.utils import DEFAULT_TEST_HD_PATH, cached_property
 from ape_ethereum.provider import Web3Provider
+from ape_ethereum.trace import TraceApproach, TransactionTrace
 from ape_test import ApeTestConfig
 from chompjs import parse_js_object  # type: ignore
 from eth_pydantic_types import HexBytes
-from eth_typing import HexStr
 from eth_utils import is_0x_prefixed, is_hex, to_hex
-from evm_trace import CallType
-from evm_trace import TraceFrame as EvmTraceFrame
-from evm_trace import create_trace_frames, get_calltree_from_geth_trace
 from packaging.version import Version
-from pydantic import BaseModel, Field, model_validator
+from pydantic import BaseModel, Field, field_validator, model_validator
 from pydantic_settings import SettingsConfigDict
 from web3 import HTTPProvider, Web3
 from web3.exceptions import ExtraDataLengthError
 from web3.gas_strategies.rpc import rpc_gas_price_strategy
 from web3.middleware import geth_poa_middleware
 from web3.middleware.validation import MAX_EXTRADATA_LENGTH
 from web3.types import TxParams
@@ -171,16 +160,16 @@
     return path
 
 
 class PackageJson(BaseModel):
     name: Optional[str] = None
     version: Optional[str] = None
     description: Optional[str] = None
-    dependencies: Optional[Dict[str, str]] = None
-    dev_dependencies: Optional[Dict[str, str]] = Field(None, alias="devDependencies")
+    dependencies: Optional[dict[str, str]] = None
+    dev_dependencies: Optional[dict[str, str]] = Field(None, alias="devDependencies")
 
 
 class HardhatForkConfig(PluginConfig):
     host: Optional[Union[str, Literal["auto"]]] = None
     """
     The host address or ``"auto"`` to use localhost with a random port (with attempts).
     If ``host`` is specified in the root config, this will take precendence for this
@@ -235,18 +224,28 @@
     Note: If you do this, you may need to ensure its settings
     matches Ape's.
     """
 
     # For setting the values in --fork and --fork-block-number command arguments.
     # Used only in HardhatForkProvider.
     # Mapping of ecosystem_name => network_name => HardhatForkConfig
-    fork: Dict[str, Dict[str, HardhatForkConfig]] = {}
+    fork: dict[str, dict[str, HardhatForkConfig]] = {}
 
     model_config = SettingsConfigDict(extra="allow")
 
+    @field_validator("bin_path", mode="before")
+    @classmethod
+    def resolve_bin_path(cls, value):
+        if not value:
+            return None
+
+        # NOTE: Don't resolve symlinks because CLI bin will turn
+        # into a .js file otherwise.
+        return Path(value).expanduser().absolute()
+
 
 class ForkedNetworkMetadata(BaseModel):
     """
     Metadata from the RPC ``hardhat_metadata``.
     """
 
     chain_id: int = Field(alias="chainId")
@@ -294,25 +293,28 @@
 
 def _call(*args):
     return call([*args], stderr=PIPE, stdout=PIPE, stdin=PIPE)
 
 
 class HardhatProvider(SubprocessProvider, Web3Provider, TestProviderAPI):
     _host: Optional[str] = None
-    attempted_ports: List[int] = []
+    attempted_ports: list[int] = []
     _did_warn_wrong_node = False
 
     # Will get set to False if notices not installed correctly.
     # However, will still attempt to connect and only raise
     # if failed to connect. This is because sometimes Hardhat may still work,
     # such when running via `pytester`.
     _detected_correct_install: bool = True
 
+    # Hardhat supports `debug_trceCall`.
+    _supports_debug_trace_call: Optional[bool] = True
+
     @property
-    def unlocked_accounts(self) -> List[AddressType]:
+    def unlocked_accounts(self) -> list[AddressType]:
         return list(self.account_manager.test_accounts._impersonated_accounts)
 
     @property
     def mnemonic(self) -> str:
         return self._test_config.mnemonic
 
     @property
@@ -387,18 +389,14 @@
         node = shutil.which("node")
         if not node:
             raise HardhatSubprocessError(f"Could not locate `node` executable. {suffix}")
 
         return node
 
     @property
-    def project_folder(self) -> Path:
-        return self.config_manager.PROJECT_FOLDER
-
-    @property
     def config_host(self) -> Optional[str]:
         # NOTE: Overriden in Forked networks.
         return self.settings.host
 
     @property
     def uri(self) -> str:
         if self._host is not None:
@@ -438,20 +436,19 @@
             return False
 
         self._set_web3()
         return self._web3 is not None
 
     @property
     def bin_path(self) -> Path:
-        if self.settings.bin_path:
-            # NOTE: Don't resolve symlinks
-            return Path(self.settings.bin_path).expanduser().absolute()
+        if path := self.settings.bin_path:
+            return path
 
         suffix = Path("node_modules") / ".bin" / "hardhat"
-        options = (self.project_folder, Path.home())
+        options = (self.local_project.path, Path.home())
         for base in options:
             path = base / suffix
             if path.exists():
                 return path
 
         # Default to the expected path suffx (relative).
         return suffix
@@ -475,33 +472,42 @@
     def metadata(self) -> NetworkMetadata:
         """
         Get network metadata, including an object about forked-metadata.
         If the network is not a fork, it will be ``None``.
         This is a helpful way of determing if a Hardhat node is a fork or not
         when connecting to a remote Hardhat network.
         """
-        metadata = self._make_request("hardhat_metadata", [])
+        metadata = self.make_request("hardhat_metadata", [])
         return NetworkMetadata.model_validate(metadata)
 
     @cached_property
     def _test_config(self) -> ApeTestConfig:
         return cast(ApeTestConfig, self.config_manager.get_config("test"))
 
+    @property
+    def auto_mine(self) -> bool:
+        return self.make_request("hardhat_getAutomine", [])
+
+    @auto_mine.setter
+    def auto_mine(self, value) -> None:
+        # NOTE: The prefix is for `evm_` instead of `hardhat_` for some reason!
+        return self.make_request("evm_setAutomine", [value])
+
     @cached_property
     def _package_json(self) -> PackageJson:
-        json_path = self.project_folder / "package.json"
+        json_path = self.local_project.path / "package.json"
 
         if not json_path.is_file():
             return PackageJson()
 
         return PackageJson.model_validate_json(json_path.read_text())
 
     @cached_property
-    def _hardhat_plugins(self) -> List[str]:
-        plugins: List[str] = []
+    def _hardhat_plugins(self) -> list[str]:
+        plugins: list[str] = []
 
         def package_is_plugin(package: str) -> bool:
             return re.search(HARDHAT_PLUGIN_PATTERN, package) is not None
 
         if self._package_json.dependencies:
             plugins.extend(filter(package_is_plugin, self._package_json.dependencies.keys()))
 
@@ -646,25 +652,25 @@
             raise  # RPCTimeoutError
 
     def disconnect(self):
         self._web3 = None
         self._host = None
         super().disconnect()
 
-    def build_command(self) -> List[str]:
+    def build_command(self) -> list[str]:
         # Run `node` on the actual binary.
         # This allows the process mgmt to function and prevents dangling nodes.
         if not self.bin_path.is_file():
             raise HardhatSubprocessError("Unable to find Hardhat binary. Is it installed?")
 
         return self._get_command()
 
-    def _get_command(self) -> List[str]:
+    def _get_command(self) -> list[str]:
         if self.hardhat_config_file == self._ape_managed_hardhat_config_file:
-            # If we are using the Ape managed file. regenerated before launch.
+            # If we are using the Ape managed file, regenerate before launch.
             self._ape_managed_hardhat_config_file.unlink(missing_ok=True)
 
         # Validate (and create if needed) the user-given path.
         hh_config_path = _validate_hardhat_config_file(
             self.hardhat_config_file,
             self.mnemonic,
             self.number_of_accounts,
@@ -682,150 +688,44 @@
             "--port",
             f"{self._port or DEFAULT_PORT}",
             "--config",
             str(hh_config_path),
         ]
 
     def set_block_gas_limit(self, gas_limit: int) -> bool:
-        return self._make_request("evm_setBlockGasLimit", [hex(gas_limit)]) is True
+        return self.make_request("evm_setBlockGasLimit", [hex(gas_limit)]) is True
 
     def set_code(self, address: AddressType, code: ContractCode) -> bool:
         if isinstance(code, bytes):
             code = code.hex()
 
         elif not is_hex(code):
             raise ValueError(f"Value {code} is not convertible to hex")
 
-        return self._make_request("hardhat_setCode", [address, code])
+        return self.make_request("hardhat_setCode", [address, code])
 
     def set_timestamp(self, new_timestamp: int):
-        self._make_request("evm_setNextBlockTimestamp", [new_timestamp])
+        self.make_request("evm_setNextBlockTimestamp", [new_timestamp])
 
     def mine(self, num_blocks: int = 1):
         # NOTE: Request fails when given numbers with any left padded 0s.
         num_blocks_arg = f"0x{HexBytes(num_blocks).hex().replace('0x', '').lstrip('0')}"
-        self._make_request("hardhat_mine", [num_blocks_arg])
+        self.make_request("hardhat_mine", [num_blocks_arg])
 
     def snapshot(self) -> str:
-        return self._make_request("evm_snapshot", [])
+        return self.make_request("evm_snapshot", [])
 
-    def revert(self, snapshot_id: SnapshotID) -> bool:
+    def restore(self, snapshot_id: SnapshotID) -> bool:
         if isinstance(snapshot_id, int):
             snapshot_id = HexBytes(snapshot_id).hex()
 
-        return self._make_request("evm_revert", [snapshot_id]) is True
+        return self.make_request("evm_revert", [snapshot_id]) is True
 
     def unlock_account(self, address: AddressType) -> bool:
-        return self._make_request("hardhat_impersonateAccount", [address])
-
-    def send_call(
-        self,
-        txn: TransactionAPI,
-        block_id: Optional[BlockID] = None,
-        state: Optional[Dict] = None,
-        **kwargs,
-    ) -> HexBytes:
-        skip_trace = kwargs.pop("skip_trace", False)
-        if block_id is not None:
-            kwargs["block_identifier"] = block_id
-        if state is not None:
-            kwargs["state_override"] = state
-
-        arguments = self._prepare_call(txn, **kwargs)
-        if skip_trace:
-            return self._send_call_legacy(txn, **kwargs)
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
-            return self._send_call_legacy(txn, **kwargs)
-
-        # The user is requesting information related to a call's trace,
-        # such as gas usage data.
-        try:
-            result, trace_frames = self._trace_call(arguments)
-        except Exception as err:
-            logger.error(f"Error when tracing call: {err}")
-            return self._send_call_legacy(txn, **kwargs)
-
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
-        if track_gas and show_gas and not show_trace and call_tree:
-            # Optimization to enrich early and in_place=True.
-            call_tree.enrich()
-
-        if track_gas and call_tree and self._test_runner is not None and txn.receiver:
-            # Gas report being collected, likely for showing a report
-            # at the end of a test run.
-            # Use `in_place=False` in case also `show_trace=True`
-            enriched_call_tree = call_tree.enrich(in_place=False)
-            self._test_runner.gas_tracker.append_gas(enriched_call_tree, txn.receiver)
-
-        if track_coverage and self._test_runner is not None and txn.receiver:
-            contract_type = self.chain_manager.contracts.get(txn.receiver)
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
-        return result, create_trace_frames(trace_data)
-
-    def _send_call_legacy(self, txn, **kwargs) -> HexBytes:
-        result = super().send_call(txn, **kwargs)
-
-        # Older versions of Hardhat do not support call tracing.
-        # But we are still able to incremenet func hits.
-        self._increment_call_func_coverage_hit_count(txn)
-
-        return result
+        return self.make_request("hardhat_impersonateAccount", [address])
 
     def _increment_call_func_coverage_hit_count(self, txn: TransactionAPI):
         """
         A helper method for increment a method call function hit count in a
         non-orthodox way. This is because Hardhat does support call traces yet.
         """
         if (
@@ -839,15 +739,15 @@
         if not cov_data:
             return
 
         contract_type = self.chain_manager.contracts.get(txn.receiver)
         if not contract_type:
             return
 
-        contract_src = self.project_manager._create_contract_source(contract_type)
+        contract_src = self.local_project._create_contract_source(contract_type)
         if not contract_src:
             return
 
         method_id = txn.data[:4]
         if method_id in contract_type.view_methods:
             method = contract_type.methods[method_id]
             self._test_runner.coverage_tracker.hit_function(contract_src, method)
@@ -899,79 +799,47 @@
             receipt.raise_for_status()
 
         else:
             receipt = super().send_transaction(txn)
 
         return receipt
 
-    def get_receipt(
-        self,
-        txn_hash: str,
-        required_confirmations: int = 0,
-        timeout: Optional[int] = None,
-        **kwargs,
-    ) -> ReceiptAPI:
-        try:
-            # Try once without waiting first.
-            # NOTE: This is required for txn sent with an impersonated account.
-            receipt_data = dict(self.web3.eth.get_transaction_receipt(HexStr(txn_hash)))
-        except Exception:
-            return super().get_receipt(
-                txn_hash, required_confirmations=required_confirmations, timeout=timeout
-            )
-
-        txn = kwargs.get("txn", dict(self.web3.eth.get_transaction(HexStr(txn_hash))))
-        data: Dict = {"txn_hash": txn_hash, **receipt_data, **txn}
-        if "gas_price" not in data:
-            data["gas_price"] = self.gas_price
+    # def get_receipt(
+    #     self,
+    #     txn_hash: str,
+    #     required_confirmations: int = 0,
+    #     timeout: Optional[int] = None,
+    #     **kwargs,
+    # ) -> ReceiptAPI:
+    #     try:
+    #         # Try once without waiting first.
+    #         # NOTE: This is required for txn sent with an impersonated account.
+    #         receipt_data = dict(self.web3.eth.get_transaction_receipt(HexStr(txn_hash)))
+    #     except Exception:
+    #         return super().get_receipt(
+    #             txn_hash, required_confirmations=required_confirmations, timeout=timeout
+    #         )
+    #
+    #     txn = kwargs.get("txn", dict(self.web3.eth.get_transaction(HexStr(txn_hash))))
+    #     data: dict = {"txn_hash": txn_hash, **receipt_data, **txn}
+    #     if "gas_price" not in data:
+    #         data["gas_price"] = self.gas_price
+    #
+    #     receipt = self.network.ecosystem.decode_receipt(data)
+    #     self.chain_manager.history.append(receipt)
+    #     return receipt
+
+    def get_transaction_trace(self, transaction_hash: str, **kwargs) -> TraceAPI:
+        if "debug_trace_transaction_parameters" not in kwargs:
+            kwargs["debug_trace_transaction_parameters"] = {}
 
-        receipt = self.network.ecosystem.decode_receipt(data)
-        self.chain_manager.history.append(receipt)
-        return receipt
+        if "call_trace_approach" not in kwargs:
+            kwargs["call_trace_approach"] = TraceApproach.GETH_STRUCT_LOG_PARSE
 
-    def get_transaction_trace(self, txn_hash: str) -> Iterator[TraceFrame]:
-        for trace in self._get_transaction_trace(txn_hash):
-            yield self._create_trace_frame(trace)
-
-    def _get_transaction_trace(self, txn_hash: str) -> Iterator[EvmTraceFrame]:
-        result = self._make_request("debug_traceTransaction", [txn_hash])
-        frames = result.get("structLogs", [])
-        yield from create_trace_frames(frames)
-
-    def get_call_tree(self, txn_hash: str) -> CallTreeNode:
-        receipt = self.chain_manager.get_receipt(txn_hash)
-
-        # Subtract base gas costs.
-        # (21_000 + 4 gas per 0-byte and 16 gas per non-zero byte).
-        data_gas = sum([4 if x == 0 else 16 for x in receipt.data])
-        method_gas_cost = receipt.gas_used - 21_000 - data_gas
-
-        if receipt.receiver:
-            address = receipt.receiver
-            call_type = CallType.CALL
-        elif receipt.contract_address:
-            address = receipt.contract_address
-            call_type = CallType.CREATE
-        else:
-            # Not sure if this is possible.
-            address = None
-            call_type = None
-
-        address = receipt.receiver or receipt.contract_address
-        evm_call = get_calltree_from_geth_trace(
-            self._get_transaction_trace(txn_hash),
-            gas_cost=method_gas_cost,
-            gas_limit=receipt.gas_limit,
-            address=address,
-            calldata=receipt.data,
-            value=receipt.value,
-            call_type=call_type,
-            failed=receipt.failed,
-        )
-        return self._create_call_tree_node(evm_call, txn_hash=txn_hash)
+        return _get_transaction_trace(transaction_hash, **kwargs)
 
     def set_balance(self, account: AddressType, amount: Union[int, float, str, bytes]):
         is_str = isinstance(amount, str)
         _is_hex = False if not is_str else is_0x_prefixed(str(amount))
         is_key_word = is_str and len(str(amount).split(" ")) > 1
         if is_key_word:
             # This allows values such as "1000 ETH".
@@ -982,15 +850,15 @@
 
         # Convert to hex str
         if is_str and not _is_hex:
             amount_hex_str = to_hex(int(amount))
         elif isinstance(amount, int) or isinstance(amount, bytes):
             amount_hex_str = to_hex(amount)
 
-        self._make_request("hardhat_setBalance", [account, amount_hex_str])
+        self.make_request("hardhat_setBalance", [account, amount_hex_str])
 
     def get_virtual_machine_error(self, exception: Exception, **kwargs) -> VirtualMachineError:
         if not len(exception.args):
             return VirtualMachineError(base_err=exception, **kwargs)
 
         err_data = exception.args[0]
 
@@ -1066,15 +934,15 @@
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
@@ -1132,22 +1000,22 @@
     def connect(self):
         super().connect()
 
         if not self.metadata.forked_network:
             # This will fail when trying to connect hardhat-fork to
             # a non-forked network.
             raise HardhatProviderError(
-                "Network is no a fork. "
+                "Network is not a fork. "
                 "Hardhat is likely already running on the local network. "
                 "Try using config:\n\n(ape-config.yaml)\n```\nhardhat:\n  "
                 "host: auto\n```\n\nso that multiple processes can automatically "
                 "use different ports."
             )
 
-    def build_command(self) -> List[str]:
+    def build_command(self) -> list[str]:
         if not self.fork_url:
             raise HardhatProviderError("Upstream provider does not have a ``connection_str``.")
 
         if self.fork_url.replace("localhost", "127.0.0.1").replace("http://", "") == self.uri:
             raise HardhatProviderError(
                 "Invalid upstream-fork URL. Can't be same as local Hardhat node."
             )
@@ -1160,18 +1028,23 @@
             cmd.append("--no-deploy")
         if self.fork_block_number is not None:
             cmd.extend(("--fork-block-number", str(self.fork_block_number)))
 
         return cmd
 
     def reset_fork(self, block_number: Optional[int] = None):
-        forking_params: Dict[str, Union[str, int]] = {"jsonRpcUrl": self.fork_url}
+        forking_params: dict[str, Union[str, int]] = {"jsonRpcUrl": self.fork_url}
         block_number = block_number if block_number is not None else self.fork_block_number
         if block_number is not None:
             forking_params["blockNumber"] = block_number
 
-        return self._make_request("hardhat_reset", [{"forking": forking_params}])
+        return self.make_request("hardhat_reset", [{"forking": forking_params}])
 
 
 def _create_web3(uri: str, timeout: int) -> Web3:
     # NOTE: This method exists so can be mocked in testing.
     return Web3(HTTPProvider(uri, request_kwargs={"timeout": timeout}))
+
+
+def _get_transaction_trace(transaction_hash: str, **kwargs) -> TraceAPI:
+    # Abstracted for testing purposes.
+    return TransactionTrace(transaction_hash=transaction_hash, **kwargs)
```

### Comparing `ape-hardhat-0.7.3/ape_hardhat.egg-info/PKG-INFO` & `ape-hardhat-0.8.0/ape_hardhat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: ape-hardhat
-Version: 0.7.3
+Version: 0.8.0
 Summary: ape-hardhat: Ape network provider for Hardhat
 Home-page: https://github.com/ApeWorX/ape-hardhat
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
@@ -32,15 +31,15 @@
 
 This is a Hardhat network provider plugin for Ape.
 Hardhat is a development framework written in Node.js for Ethereum that includes a local network implementation.
 Use this plugin to manage a Hardhat node process or connect to an existing one.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 - Node.js, NPM, and Hardhat 2.12.0 or greater. See Hardhat's [Installation](https://hardhat.org/getting-started/#installation%3E) documentation for steps.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-hardhat-0.7.3/ape_hardhat.egg-info/SOURCES.txt` & `ape-hardhat-0.8.0/ape_hardhat.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

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
@@ -26,15 +27,14 @@
 ape_hardhat.egg-info/PKG-INFO
 ape_hardhat.egg-info/SOURCES.txt
 ape_hardhat.egg-info/dependency_links.txt
 ape_hardhat.egg-info/not-zip-safe
 ape_hardhat.egg-info/requires.txt
 ape_hardhat.egg-info/top_level.txt
 tests/__init__.py
-tests/ape-config.yaml
 tests/conftest.py
 tests/expected_traces.py
 tests/test_fork_provider.py
 tests/test_gas_report.py
 tests/test_provider.py
 tests/test_trace.py
 tests/data/contracts/ethereum/local/contract_a.json
```

### Comparing `ape-hardhat-0.7.3/ape_hardhat.egg-info/requires.txt` & `ape-hardhat-0.8.0/ape_hardhat.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-eth-ape<0.8,>=0.7.0
+eth-ape<0.9,>=0.8.1
 ethpm-types
 evm-trace
 web3
 chompjs<2,>=1.1.9
 requests
 hexbytes
 packaging
```

### Comparing `ape-hardhat-0.7.3/pyproject.toml` & `ape-hardhat-0.8.0/pyproject.toml`

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
 norecursedirs = "projects"
 addopts = """
     -p no:ape_test
     --cov-branch
```

### Comparing `ape-hardhat-0.7.3/setup.py` & `ape-hardhat-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 from setuptools import find_packages, setup
 
 extras_require = {
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-mock",  # For patching and mocking
@@ -73,15 +72,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-hardhat",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.0,<0.8",
+        "eth-ape>=0.8.1,<0.9",
         "ethpm-types",  # Use same version as eth-ape
         "evm-trace",  # Use same version as eth-ape
         "web3",  # Use same version as eth-ape
         "chompjs>=1.1.9,<2",  # To help parse hardhat files
         "requests",  # Use same version as eth-ape
         "hexbytes",  # Use same version as eth-ape
         "packaging",  # Use same version as eth-ape
@@ -99,14 +98,13 @@
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

### Comparing `ape-hardhat-0.7.3/tests/conftest.py` & `ape-hardhat-0.8.0/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-import json
 import shutil
 import subprocess
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
-from ape.utils import create_tempdir
 from ethpm_types import ContractType
 
 from ape_hardhat import HardhatProvider
 
 # NOTE: Ensure that we don't use local paths for the DATA FOLDER
 DATA_FOLDER = Path(mkdtemp()).resolve()
 ape.config.DATA_FOLDER = DATA_FOLDER
@@ -37,30 +32,35 @@
     if call.excinfo is not None and "too many requests" in str(call.excinfo).lower():
         tr.outcome = "skipped"
         tr.wasxfail = "reason: Alchemy requests overloaded (likely in CI)"
 
     return tr
 
 
+@pytest.fixture(autouse=True, scope="session")
+def project():
+    return ape.project
+
+
+@pytest.fixture(autouse=True, scope="session")
+def clean_datafolder():
+    yield  # Run all collected tests.
+    shutil.rmtree(DATA_FOLDER, ignore_errors=True)
+
+
 @pytest.fixture(scope="session")
 def name():
     return NAME
 
 
 @pytest.fixture(scope="session")
 def data_folder():
     return DATA_FOLDER
 
 
-@pytest.fixture(scope="session", autouse=True)
-def in_tests_dir(config):
-    with config.using_project(Path(__file__).parent):
-        yield
-
-
 @contextmanager
 def _isolation():
     if ape.networks.active_provider is None:
         raise AssertionError("Isolation should only be used with a connected provider.")
 
     init_network_name = ape.chain.provider.network.name
     init_provider_name = ape.chain.provider.name
@@ -97,19 +97,14 @@
 
 @pytest.fixture(scope="session")
 def config():
     return ape.config
 
 
 @pytest.fixture(scope="session")
-def project():
-    return ape.project
-
-
-@pytest.fixture(scope="session")
 def accounts():
     return ape.accounts.test_accounts
 
 
 @pytest.fixture(scope="session")
 def convert():
     return ape.convert
@@ -178,14 +173,17 @@
 @pytest.fixture(scope="session")
 def local_network_api(networks):
     return networks.ethereum.local
 
 
 @pytest.fixture
 def connected_provider(name, networks, local_network_api):
+    """
+    The main HH local-network (non-fork) instance.
+    """
     with networks.ethereum.local.use_provider(name) as provider:
         yield provider
 
 
 @pytest.fixture(scope="session")
 def disconnected_provider(name, local_network_api):
     return HardhatProvider(
@@ -219,44 +217,14 @@
 def sepolia_fork_provider(name, networks, sepolia_fork_port):
     with networks.ethereum.sepolia_fork.use_provider(
         name, provider_settings={"host": f"http://127.0.0.1:{sepolia_fork_port}"}
     ) as provider:
         yield provider
 
 
-@pytest.fixture(scope="session")
-def temp_config(config):
-    @contextmanager
-    def func(data: Dict, package_json: Optional[Dict] = None):
-        with create_tempdir() as temp_dir:
-            config._cached_configs = {}
-            config_file = temp_dir / CONFIG_FILE_NAME
-            config_file.touch()
-
-            # Default to using the normal bin to avoid a temp installation.
-            data["bin_path"] = data.get(
-                "bin_path", (Path(__file__).parent / "node_modules" / ".bin" / "hardhat").as_posix()
-            )
-
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

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/contract_a.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/contract_a.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/contract_b.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/contract_b.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/contract_c.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/contract_c.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/has_error.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/has_error.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/solidity_contract.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/solidity_contract.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/token_a.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/token_a.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/token_b.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/token_b.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/local/vyper_contract.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/local/vyper_contract.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json` & `ape-hardhat-0.8.0/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/python/pytest_tests.py` & `ape-hardhat-0.8.0/tests/data/python/pytest_tests.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/sources/TokenA.vy` & `ape-hardhat-0.8.0/tests/data/sources/TokenA.vy`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/data/sources/TokenB.vy` & `ape-hardhat-0.8.0/tests/data/sources/TokenB.vy`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.7.3/tests/expected_traces.py` & `ape-hardhat-0.8.0/tests/expected_traces.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LOCAL_TRACE = r"""
 Call trace for '0x([A-Fa-f0-9]{64})'
 tx\.origin=0x[a-fA-F0-9]{40}
-ContractA\.methodWithoutArguments\(\) -> 0x00..5174 \[\d+ gas\]
+ContractA\.methodWithoutArguments\(\) -> 0x00..93bc \[\d+ gas\]
 ├── SYMBOL\.methodB1\(lolol="ice-cream", dynamo=36\)
 │   ├── ContractC\.getSomeList\(\) -> \[
 │   │     3425311345134513461345134534531452345,
 │   │     111344445534535353,
 │   │     993453434534534534534977788884443333
 │   │   \]
 │   └── ContractC\.methodC1\(windows95="simpler", jamaica=36, cardinal=ContractA\)
@@ -54,15 +54,15 @@
     │   ├── UniswapV3Pool\.fee\(\) -> 500
     │   └── WETH\.transfer\(dst=UniswapV3Pool, wad=2098831888913057968\) -> True
     └── WETH\.balanceOf\(UniswapV3Pool\) -> 68359883632315875514968
 """
 MAINNET_TRACE_FIRST_10_LINES = r"""
 Call trace for '0xb7d7f1d5ce7743e821d3026647df486f517946ef1342a1ae93c96e4a8016eab7'
 tx\.origin=0x5668EAd1eDB8E2a4d724C8fb9cB5fFEabEB422dc
-DSProxy\.execute\(_target=LoanShifterTaker, _data=0x35\.\.0000\) -> "" \[1249147 gas\]
+DSProxy\.execute\(_target=LoanShifterTaker, _data=0x35\.\.0000\) -> 0 \[\d+ gas\]
 └── \(delegate\) LoanShifterTaker\.moveLoan\(
       _exchangeData=\[
         0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE,
         ZERO_ADDRESS,
         0,
         0,
 """
```

### Comparing `ape-hardhat-0.7.3/tests/test_fork_provider.py` & `ape-hardhat-0.8.0/tests/test_fork_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import json
 from pathlib import Path
 
 import pytest
 from ape.api.networks import LOCAL_NETWORK_NAME
 from ape.contracts import ContractInstance
 from ape.exceptions import ContractLogicError
-from ape.utils import create_tempdir
 from ape_ethereum.ecosystem import NETWORKS
 
 from ape_hardhat.provider import HardhatForkProvider
 
 TESTS_DIRECTORY = Path(__file__).parent
 TEST_ADDRESS = "0xd8da6bf26964af9d7eed9e03e53415d37aa96045"
 
@@ -48,15 +48,15 @@
         assert networks.active_provider.uri == mainnet_fork_host
 
     assert networks.active_provider.name == name
     assert networks.active_provider.network.name == LOCAL_NETWORK_NAME
     assert networks.active_provider.uri == default_host
 
 
-@pytest.mark.parametrize("network", [k for k in NETWORKS.keys() if k != "goerli"])
+@pytest.mark.parametrize("network", NETWORKS)
 def test_fork_config(name, config, network):
     plugin_config = config.get_config(name)
     network_config = plugin_config["fork"].get("ethereum", {}).get(network, {})
     assert network_config.get("upstream_provider") == "alchemy", "config not registered"
 
 
 @pytest.mark.fork
@@ -74,23 +74,25 @@
     other_account = accounts[0]
     receipt = impersonated_account.transfer(other_account, "1 wei")
     assert receipt.receiver == other_account
     assert receipt.sender == impersonated_account
 
 
 @pytest.mark.fork
-def test_request_timeout(networks, config, mainnet_fork_provider):
+def test_request_timeout(networks, project, mainnet_fork_provider):
+    # Is set in ape-config.yaml
+    expected = 360
+    assert networks.active_provider.timeout == expected
     actual = mainnet_fork_provider.web3.provider._request_kwargs["timeout"]
-    expected = 360  # Value set in `ape-config.yaml`
     assert actual == expected
 
-    # Test default behavior
-    with create_tempdir() as temp_dir:
-        with config.using_project(temp_dir):
-            assert networks.active_provider.timeout == 300
+    # Test default behavior.
+    with project.temp_config(hardhat={}):
+        actual = mainnet_fork_provider.timeout
+        assert actual == 300
 
 
 @pytest.mark.fork
 def test_reset_fork_no_fork_block_number(networks, sepolia_fork_provider):
     sepolia_fork_provider.mine(5)
     prev_block_num = sepolia_fork_provider.get_block("latest").number
     sepolia_fork_provider.reset_fork()
@@ -178,49 +180,50 @@
         ("mainnet", 8996, True, 15_900_000, False),
         ("sepolia", 8997, False, 7_948_861, False),
         ("sepolia", 8998, False, 7_424_430, True),
         ("sepolia", 8999, True, 7_900_000, False),
     ],
 )
 def test_hardhat_command(
-    temp_config,
+    project,
     networks,
     port,
     upstream_network,
     enable_hardhat_deployments,
     fork_block_number,
     has_hardhat_deploy,
     name,
     data_folder,
 ):
-    eth_config = {
-        name: {
-            "fork": {
-                "ethereum": {
-                    upstream_network: {
-                        "enable_hardhat_deployments": enable_hardhat_deployments,
-                        "block_number": fork_block_number,
-                    }
+    hh_ape_config = {
+        "fork": {
+            "ethereum": {
+                upstream_network: {
+                    "enable_hardhat_deployments": enable_hardhat_deployments,
+                    "block_number": fork_block_number,
                 }
-            },
+            }
         },
     }
     package_json = {
         "name": "contracts",
         "version": "0.1.0",
         "dependencies": {
             "hardhat": "^2.13.1",
             "hardhat-ethers": "^2.0.2",
         },
     }
 
     if has_hardhat_deploy:
         package_json["devDependencies"] = {"hardhat-deploy": "^0.8.10"}
 
-    with temp_config(eth_config, package_json):
+    with project.temp_config(hardhat=hh_ape_config):
+        package_json_path = project.path / "package.json"
+        package_json_path.unlink(missing_ok=True)
+        package_json_path.write_text(json.dumps(package_json, indent=2))
         network_api = networks.ethereum[f"{upstream_network}-fork"]
         provider = HardhatForkProvider(
             name=name,
             network=network_api,
             request_header={},
             data_folder=Path("."),
             provider_settings={},
@@ -239,21 +242,21 @@
             provider.fork_url,
         ]
         if not enable_hardhat_deployments and has_hardhat_deploy:
             expected.append("--no-deploy")
         if fork_block_number:
             expected.extend(("--fork-block-number", str(fork_block_number)))
 
-        assert actual[0].endswith("npx")
+        assert actual[0].endswith("npx") or actual[0].endswith("node")  # depends on node version
         assert actual[1].endswith("hardhat")
         assert actual[2:] == expected
 
 
 @pytest.mark.fork
 def test_connect_to_polygon(networks, owner, contract_container):
     """
     Ensures we don't get PoA middleware issue.
     Also, ensure that we using a different host (via config).
     """
-    with networks.polygon.mumbai_fork.use_provider("hardhat"):
+    with networks.polygon.amoy_fork.use_provider("hardhat"):
         contract = owner.deploy(contract_container)
         assert isinstance(contract, ContractInstance)  # Didn't fail
```

### Comparing `ape-hardhat-0.7.3/tests/test_gas_report.py` & `ape-hardhat-0.8.0/tests/test_gas_report.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,21 +81,27 @@
 
     for actual_line, expected_line in zip(actual, expected):
         message = f"'{actual_line}' does not match pattern '{expected_line}'."
         assert re.match(expected_line, actual_line), message
 
 
 def test_gas_flag_in_tests(ape_pytester):
-    result = ape_pytester.runpytest("--gas")
+    result = ape_pytester.runpytest("--gas", "--network", "ethereum:local:hardhat")
     run_gas_test(result)
 
     # Verify can happen more than once.
     run_gas_test(result)
 
 
 def test_gas_flag_exclude_method_using_cli_option(ape_pytester):
     # NOTE: Includes both a mutable and a view method.
     expected = filter_expected_methods("fooAndBar", "myNumber")
     # Also ensure can filter out whole class
     expected = expected.replace(TOKEN_B_GAS_REPORT, "")
-    result = ape_pytester.runpytest("--gas", "--gas-exclude", "*:fooAndBar,*:myNumber,tokenB:*")
+    result = ape_pytester.runpytest(
+        "--gas",
+        "--gas-exclude",
+        "*:fooAndBar,*:myNumber,tokenB:*",
+        "--network",
+        "ethereum:local:hardhat",
+    )
     run_gas_test(result, expected_report=expected)
```

### Comparing `ape-hardhat-0.7.3/tests/test_provider.py` & `ape-hardhat-0.8.0/tests/test_provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import shutil
 
 import pytest
 import requests
-from ape.api import ReceiptAPI
+from ape.api import ReceiptAPI, TraceAPI
 from ape.api.accounts import ImpersonatedAccount
 from ape.contracts import ContractContainer
 from ape.exceptions import ContractLogicError
-from ape.types import CallTreeNode, TraceFrame
-from ape.utils import create_tempdir
-from evm_trace import CallType
 from hexbytes import HexBytes
 
 from ape_hardhat.exceptions import HardhatNotInstalledError, HardhatProviderError
 from ape_hardhat.provider import HARDHAT_CHAIN_ID
 
 TEST_WALLET_ADDRESS = "0xD9b7fdb3FC0A0Aa3A507dCf0976bc23D49a9C7A3"
 
@@ -84,32 +81,32 @@
     connected_provider.mine(12)
     next_block_num = connected_provider.get_block("latest").number
 
     # NOTE: Uses >= due to x-dist
     assert next_block_num >= block_num + 12
 
 
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
 
 
 def test_unlock_account(connected_provider, owner, contract_a, accounts):
     # This first statement is not needed but testing individually anyway.
@@ -121,37 +118,27 @@
     # Ensure can transact.
     receipt = contract_a.methodWithoutArguments(sender=impersonated_account)
     assert not receipt.failed
 
 
 def test_get_transaction_trace(connected_provider, sender, receiver):
     transfer = sender.transfer(receiver, 1)
-    frame_data = connected_provider.get_transaction_trace(transfer.txn_hash)
-    for frame in frame_data:
-        assert isinstance(frame, TraceFrame)
+    trace = connected_provider.get_transaction_trace(transfer.txn_hash)
+    assert isinstance(trace, TraceAPI)
 
 
-def test_get_call_tree(connected_provider, sender, receiver):
-    transfer = sender.transfer(receiver, 1)
-    call_tree = connected_provider.get_call_tree(transfer.txn_hash)
-    assert isinstance(call_tree, CallTreeNode)
-    assert call_tree.call_type == CallType.CALL.value
-    assert repr(call_tree) == "0x70997970C51812dc3A010C7d01b50e0d17dc79C8.0x()"
-
-
-def test_request_timeout(connected_provider, config):
-    # Test value set in `ape-config.yaml`
-    expected = 29
+def test_request_timeout(connected_provider, project):
+    # Value set from config.
+    assert connected_provider.timeout == 29
     actual = connected_provider.web3.provider._request_kwargs["timeout"]
-    assert actual == expected
+    assert actual == 29
 
-    # Test default behavior
-    with create_tempdir() as temp_dir:
-        with config.using_project(temp_dir):
-            assert connected_provider.timeout == 30
+    with project.temp_config(hardhat={}):
+        actual = connected_provider.timeout
+        assert actual == 30  # default
 
 
 def test_send_transaction_and_send_call(contract_instance, owner):
     number = 10
     contract_instance.setNumber(number, sender=owner)  # send tx
     actual = contract_instance.myNumber(show_trace=True)  # send call
     assert actual == number
@@ -231,30 +218,28 @@
 
     # Before, this would fail because there would not be an associated txn
     # because the account is impersonated.
     assert err.value.txn.txn_hash.startswith("0x")
 
 
 @pytest.mark.parametrize("host", ("https://example.com", "example.com"))
-def test_host(temp_config, networks, host):
-    data = {"hardhat": {"host": host}}
-    with temp_config(data):
+def test_host(project, networks, host):
+    with project.temp_config(hardhat={"host": host}):
         provider = networks.ethereum.local.get_provider("hardhat")
         assert provider.uri == "https://example.com"
 
 
-def test_use_different_config(temp_config, networks, project):
-    data = {"hardhat": {"hardhat_config_file": "./hardhat.config.ts"}}
-    with temp_config(data):
+def test_use_different_config(project, networks):
+    with project.temp_config(hardhat={"hardhat_config_file": "./hardhat.config.ts"}):
         provider = networks.ethereum.local.get_provider("hardhat")
         assert provider.hardhat_config_file.name == "hardhat.config.ts"
         assert "--config" in provider._get_command()
 
         actual = provider._get_command()
-        assert "npx" in actual[0]
+        assert "npx" in actual[0] or "node" in actual[0]  # depends on node version.
         # Will either be home dir hardhat if installed there
         # or just the relative suffix (like in CI).
         assert actual[1].endswith("node_modules/.bin/hardhat")
 
 
 def test_connect_when_hardhat_not_installed(networks, mock_web3, install_detection_fail):
     """
@@ -271,14 +256,22 @@
         r"Note: global installation of Hardhat will not work and "
         r"you must be in your project's directory\."
     )
     with pytest.raises(HardhatNotInstalledError, match=expected):
         provider.connect()
 
 
+def test_auto_mine(connected_provider):
+    assert connected_provider.auto_mine is True
+    connected_provider.auto_mine = False
+    assert connected_provider.auto_mine is False
+    connected_provider.auto_mine = True
+    assert connected_provider.auto_mine is True
+
+
 def test_get_virtual_machine_error_when_sol_panic(connected_provider):
     msg = "Error: VM Exception while processing transaction: reverted with panic code 0x1"
     err = ValueError(msg)
     actual = connected_provider.get_virtual_machine_error(err)
     expected = "0x1"
     assert actual.revert_message == expected
 
@@ -295,23 +288,21 @@
         actual = connected_provider.bin_path
         assert actual.as_posix().endswith("node_modules/.bin/hardhat")
 
     finally:
         shutil.move(bin_cp, expected)
 
 
-def test_remote_host(temp_config, networks, no_hardhat_bin, project):
-    data = {"hardhat": {"host": "https://example.com"}}
-    with temp_config(data):
+def test_remote_host(networks, no_hardhat_bin, project):
+    with project.temp_config(hardhat={"host": "https://example.com"}):
         with pytest.raises(
             HardhatProviderError,
             match=r"Failed to connect to remote Hardhat node at 'https://example.com'\.",
         ):
             with networks.ethereum.local.use_provider("hardhat"):
                 pass
 
 
-def test_hardfork(temp_config, networks):
-    data = {"hardhat": {"evm_version": "london"}}
-    with temp_config(data):
+def test_hardfork(project, networks):
+    with project.temp_config(hardhat={"evm_version": "london"}):
         with networks.ethereum.local.use_provider("hardhat") as provider:
             assert provider.config.evm_version == "london"
```

### Comparing `ape-hardhat-0.7.3/tests/test_trace.py` & `ape-hardhat-0.8.0/tests/test_trace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 import shutil
-import tempfile
 from pathlib import Path
 from typing import List
 
 import pytest
+from ape.utils import create_tempdir
 
 from .expected_traces import (
     LOCAL_GAS_REPORT,
     LOCAL_TRACE,
     MAINNET_FAIL_TRACE_FIRST_10_LINES,
     MAINNET_FAIL_TRACE_LAST_10_LINES,
     MAINNET_TRACE_FIRST_10_LINES,
@@ -59,16 +59,16 @@
 
 
 @pytest.mark.fork
 def test_local_transaction_traces(local_receipt, captrace):
     # NOTE: Strange bug in Rich where we can't use sys.stdout for testing tree output.
     # And we have to write to a file, close it, and then re-open it to see output.
     def run_test():
-        with tempfile.TemporaryDirectory() as temp_dir:
-            temp_file = Path(temp_dir) / "temp"
+        with create_tempdir() as temp_dir:
+            temp_file = temp_dir / "temp"
 
             with open(temp_file, "w") as file:
                 local_receipt.show_trace(file=file)
 
             with open(temp_file, "r") as file:
                 lines = captrace.read_trace("Call trace for", file=file)
 
@@ -79,16 +79,16 @@
     # Verify can happen more than once.
     run_test()
 
 
 @pytest.mark.fork
 def test_local_transaction_gas_report(local_receipt, captrace):
     def run_test():
-        with tempfile.TemporaryDirectory() as temp_dir:
-            temp_file = Path(temp_dir) / "temp"
+        with create_tempdir() as temp_dir:
+            temp_file = temp_dir / "temp"
 
             with open(temp_file, "w") as file:
                 local_receipt.show_gas_report(file=file)
 
             with open(temp_file, "r") as file:
                 lines = captrace.read_trace("ContractA Gas", file=file)
 
@@ -98,16 +98,16 @@
 
     # Verify can happen more than once.
     run_test()
 
 
 @pytest.mark.manual
 def test_mainnet_transaction_traces(mainnet_receipt, captrace):
-    with tempfile.TemporaryDirectory() as temp_dir:
-        temp_file = Path(temp_dir) / "temp"
+    with create_tempdir() as temp_dir:
+        temp_file = temp_dir / "temp"
 
         with open(temp_file, "w") as file:
             mainnet_receipt.show_trace(file=file)
 
         with open(temp_file, "r") as file:
             lines = captrace.read_trace("Call trace for", file=file)
 
@@ -122,15 +122,15 @@
     expected_lines = [x.rstrip() for x in expected.splitlines() if x.rstrip()]
     actual_lines = [x.rstrip() for x in rich_capture if x.rstrip()]
     assert actual_lines, "No output."
     output = "\n".join(actual_lines)
 
     for actual, expected in zip(actual_lines, expected_lines):
         fail_message = f"""\n
-        \tPattern: {expected},\n
+        \tPattern: {expected}\n
         \tLine   : {actual}\n
         \n
         Complete output:
         \n{output}
         """
 
         try:
@@ -140,8 +140,8 @@
         except Exception as err:
             pytest.fail(f"{fail_message}\n{err}")
 
     actual_len = len(actual_lines)
     expected_len = len(expected_lines)
     if expected_len > actual_len:
         rest = "\n".join(expected_lines[actual_len:])
-        pytest.fail(f"Missing expected lines: {rest}")
+        pytest.fail(f"Missing expected lines: {rest}\nfull output:\n{output}")
```

