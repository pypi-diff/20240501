# Comparing `tmp/ape-solidity-0.7.2.tar.gz` & `tmp/ape-solidity-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-solidity-0.7.2.tar", last modified: Tue Apr 16 17:47:10 2024, max compression
+gzip compressed data, was "ape-solidity-0.7.3.tar", last modified: Tue Apr 30 22:38:47 2024, max compression
```

## Comparing `ape-solidity-0.7.2.tar` & `ape-solidity-0.7.3.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.375099 ape-solidity-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.359098 ape-solidity-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.359098 ape-solidity-0.7.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.359098 ape-solidity-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-04-16 17:47:10.375099 ape-solidity-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.359098 ape-solidity-0.7.2/ape_solidity/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/ape_solidity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/ape_solidity/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    45726 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/ape_solidity/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/ape_solidity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/ape_solidity/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-16 17:47:09.000000 ape-solidity-0.7.2/ape_solidity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/ape_solidity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-04-16 17:47:10.000000 ape-solidity-0.7.2/ape_solidity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-16 17:47:10.000000 ape-solidity-0.7.2/ape_solidity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:47:10.000000 ape-solidity-0.7.2/ape_solidity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:47:10.000000 ape-solidity-0.7.2/ape_solidity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-16 17:47:10.000000 ape-solidity-0.7.2/ape_solidity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 17:47:10.000000 ape-solidity-0.7.2/ape_solidity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 17:47:10.375099 ape-solidity-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/BrownieProject/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/BrownieProject/brownie-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/BrownieProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/BrownieProject/contracts/BrownieContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/BrownieStyleDependency/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/BrownieStyleDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/BrownieStyleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/BrownieStyleDependency/contracts/FailingContract.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/Dependency/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/Dependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/Dependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/Dependency/contracts/Dependency.sol
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/Dependency/contracts/OlderDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/Dependency/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/Dependency/contracts/subfolder_with_imports/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/DependencyOfDependency/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/DependencyOfDependency/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/DependencyOfDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/ProjectWithinProject/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/ProjectWithinProject/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/ProjectWithinProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/ProjectWithinProject/contracts/Contract.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.363098 ape-solidity-0.7.2/tests/VersionSpecifiedInConfig/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/VersionSpecifiedInConfig/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.367098 ape-solidity-0.7.2/tests/VersionSpecifiedInConfig/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.371098 ape-solidity-0.7.2/tests/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/BuiltinErrorChecker.sol
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/CircularImport1.sol
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/CircularImport2.sol
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/CompilesOnce.sol
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/DifferentNameThanFile.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.371098 ape-solidity-0.7.2/tests/contracts/DirectoryWithExtension.sol/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/DirectoryWithExtension.sol/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/ExperimentalABIEncoderV2.sol
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/ImportOlderDependency.sol
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/ImportSourceWithEqualSignVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/ImportSourceWithNoPrefixVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/ImportingLessConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/Imports.sol
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/JustAStruct.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/LibraryFun.sol
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/MissingPragma.sol
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/MultipleDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/NumerousDefinitions.sol
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/OlderVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/RandomVyperFile.vy
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/RangedVersion.sol
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/SpacesInPragma.sol
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/SpecificVersionNoPrefix.sol
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/SpecificVersionNoPrefix2.sol
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/SpecificVersionRange.sol
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/SpecificVersionWithEqualSign.sol
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/UseYearn.sol
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/VagueVersion.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.371098 ape-solidity-0.7.2/tests/contracts/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/subfolder/Relativecontract.sol
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.371098 ape-solidity-0.7.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/data/ImportingLessConstrainedVersionFlat.sol
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/data/ImportsFlattened.sol.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.355098 ape-solidity-0.7.2/tests/data/packages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.355098 ape-solidity-0.7.2/tests/data/packages/OpenZeppelin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.371098 ape-solidity-0.7.2/tests/data/packages/OpenZeppelin/v4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)   698486 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.371098 ape-solidity-0.7.2/tests/data/packages/OpenZeppelin/v4.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)   879002 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.355098 ape-solidity-0.7.2/tests/data/packages/vault/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.375099 ape-solidity-0.7.2/tests/data/packages/vault/master/
--rw-r--r--   0 runner    (1001) docker     (127)   167518 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/data/packages/vault/master/vault_main.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.375099 ape-solidity-0.7.2/tests/data/packages/vault/v0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)   167551 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/data/packages/vault/v0.4.5/vault.json
--rw-r--r--   0 runner    (1001) docker     (127)    32767 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:47:10.375099 ape-solidity-0.7.2/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/scripts/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)    25275 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-16 17:46:12.000000 ape-solidity-0.7.2/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.825332 ape-solidity-0.7.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.813332 ape-solidity-0.7.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.813332 ape-solidity-0.7.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.813332 ape-solidity-0.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-30 22:38:47.829332 ape-solidity-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.813332 ape-solidity-0.7.3/ape_solidity/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/ape_solidity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/ape_solidity/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46268 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/ape_solidity/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/ape_solidity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/ape_solidity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-30 22:38:47.000000 ape-solidity-0.7.3/ape_solidity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.813332 ape-solidity-0.7.3/ape_solidity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-30 22:38:47.000000 ape-solidity-0.7.3/ape_solidity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-30 22:38:47.000000 ape-solidity-0.7.3/ape_solidity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 22:38:47.000000 ape-solidity-0.7.3/ape_solidity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 22:38:47.000000 ape-solidity-0.7.3/ape_solidity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-30 22:38:47.000000 ape-solidity-0.7.3/ape_solidity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-30 22:38:47.000000 ape-solidity-0.7.3/ape_solidity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-30 22:38:47.829332 ape-solidity-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/BrownieProject/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/BrownieProject/brownie-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/BrownieProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/BrownieProject/contracts/BrownieContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/BrownieStyleDependency/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/BrownieStyleDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/BrownieStyleDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/BrownieStyleDependency/contracts/BrownieStyleDependency.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/BrownieStyleDependency/contracts/FailingContract.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/Dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/Dependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/Dependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/Dependency/contracts/Dependency.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/Dependency/contracts/OlderDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/Dependency/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/Dependency/contracts/subfolder/InDependencySubfolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/Dependency/contracts/subfolder_with_imports/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/Dependency/contracts/subfolder_with_imports/InDependencySubfolderWithImports.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/DependencyOfDependency/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/DependencyOfDependency/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/DependencyOfDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/DependencyOfDependency/contracts/DependencyOfDependency.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/ProjectWithinProject/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/ProjectWithinProject/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/ProjectWithinProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/ProjectWithinProject/contracts/Contract.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/VersionSpecifiedInConfig/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/VersionSpecifiedInConfig/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.817332 ape-solidity-0.7.3/tests/VersionSpecifiedInConfig/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/VersionSpecifiedInConfig/contracts/VersionSpecifiedInConfig.sol
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.821332 ape-solidity-0.7.3/tests/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/BuiltinErrorChecker.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/CircularImport1.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/CircularImport2.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/CompilesOnce.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/DifferentNameThanFile.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.821332 ape-solidity-0.7.3/tests/contracts/DirectoryWithExtension.sol/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/DirectoryWithExtension.sol/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/ExperimentalABIEncoderV2.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/ImportOlderDependency.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/ImportSourceWithEqualSignVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/ImportSourceWithNoPrefixVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/ImportingLessConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/Imports.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/IndirectlyImportingMoreConstrainedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/IndirectlyImportingMoreConstrainedVersionCompanionImport.sol
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/JustAStruct.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/LibraryFun.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/MissingPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/MultipleDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/NumerousDefinitions.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/OlderVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/RandomVyperFile.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/RangedVersion.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/SpacesInPragma.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/SpecificVersionNoPrefix.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/SpecificVersionNoPrefix2.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/SpecificVersionRange.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/SpecificVersionWithEqualSign.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/UseYearn.sol
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/VagueVersion.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.821332 ape-solidity-0.7.3/tests/contracts/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/subfolder/Relativecontract.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/contracts/subfolder/UsingDependencyWithinSubFolder.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.825332 ape-solidity-0.7.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/data/ImportingLessConstrainedVersionFlat.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/data/ImportsFlattened.sol.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.809332 ape-solidity-0.7.3/tests/data/packages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.809332 ape-solidity-0.7.3/tests/data/packages/OpenZeppelin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.825332 ape-solidity-0.7.3/tests/data/packages/OpenZeppelin/v4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)   698486 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.825332 ape-solidity-0.7.3/tests/data/packages/OpenZeppelin/v4.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)   879002 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.809332 ape-solidity-0.7.3/tests/data/packages/vault/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.825332 ape-solidity-0.7.3/tests/data/packages/vault/master/
+-rw-r--r--   0 runner    (1001) docker     (127)   167518 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/data/packages/vault/master/vault_main.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.825332 ape-solidity-0.7.3/tests/data/packages/vault/v0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)   167551 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/data/packages/vault/v0.4.5/vault.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32767 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:38:47.825332 ape-solidity-0.7.3/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/scripts/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25148 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-30 22:37:41.000000 ape-solidity-0.7.3/tests/test_integration.py
```

### Comparing `ape-solidity-0.7.2/.github/ISSUE_TEMPLATE/bug.md` & `ape-solidity-0.7.3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/.github/ISSUE_TEMPLATE/feature.md` & `ape-solidity-0.7.3/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/.github/ISSUE_TEMPLATE/work-item.md` & `ape-solidity-0.7.3/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/.github/release-drafter.yml` & `ape-solidity-0.7.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/.github/workflows/codeql.yml` & `ape-solidity-0.7.3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/.github/workflows/prtitle.yaml` & `ape-solidity-0.7.3/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/.github/workflows/publish.yaml` & `ape-solidity-0.7.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/.github/workflows/stale-prs.yml` & `ape-solidity-0.7.3/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/.github/workflows/test.yaml` & `ape-solidity-0.7.3/.github/workflows/test.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -58,16 +58,18 @@
           run: mypy .
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
-                os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, '3.10', '3.11']
+                # TODO: Replace with macos-latest when works again.
+                #   https://github.com/actions/setup-python/issues/808
+                os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
+                python-version: [3.8, 3.9, '3.10', '3.11', '3.12']
 
         env:
           GITHUB_ACCESS_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
         steps:
         - uses: actions/checkout@v4
```

### Comparing `ape-solidity-0.7.2/.gitignore` & `ape-solidity-0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/.pre-commit-config.yaml` & `ape-solidity-0.7.3/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.6.0
     hooks:
     -   id: check-yaml
 
--   repo: https://github.com/pre-commit/mirrors-isort
-    rev: v5.10.1
+-   repo: https://github.com/PyCQA/isort
+    rev: 5.13.2
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 24.3.0
+    rev: 24.4.2
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
     rev: 7.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
     -   id: mypy
         additional_dependencies: [types-requests, types-setuptools, pydantic, types-pkg-resources]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
```

### Comparing `ape-solidity-0.7.2/CONTRIBUTING.md` & `ape-solidity-0.7.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/LICENSE` & `ape-solidity-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/PKG-INFO` & `ape-solidity-0.7.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-solidity
-Version: 0.7.2
+Version: 0.7.3
 Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
 Home-page: https://github.com/ApeWorX/ape-solidity
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
@@ -29,15 +30,15 @@
 
 # Quick Start
 
 Compile Solidity contracts.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-solidity-0.7.2/README.md` & `ape-solidity-0.7.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Compile Solidity contracts.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-solidity-0.7.2/ape_solidity/_utils.py` & `ape-solidity-0.7.3/ape_solidity/_utils.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/ape_solidity/compiler.py` & `ape-solidity-0.7.3/ape_solidity/compiler.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 from typing import Any, Dict, List, Optional, Sequence, Set, Tuple, Type, Union, cast
 
 from ape.api import CompilerAPI, PluginConfig
 from ape.contracts import ContractInstance
 from ape.exceptions import CompilerError, ConfigError, ContractLogicError
 from ape.logging import logger
 from ape.types import AddressType, ContractType
-from ape.utils import cached_property, get_relative_path
+from ape.utils import cached_property, get_package_version, get_relative_path
 from eth_pydantic_types import HexBytes
 from eth_utils import add_0x_prefix, is_0x_prefixed
 from ethpm_types import PackageManifest
 from ethpm_types.source import Compiler, Content
 from packaging.specifiers import SpecifierSet
 from packaging.version import Version
-from pkg_resources import get_distribution
 from requests.exceptions import ConnectionError
 from solcx import (
     compile_source,
     compile_standard,
     get_installable_solc_versions,
     get_installed_solc_versions,
     install_solc,
@@ -58,21 +57,47 @@
 )
 LICENSES_PATTERN = re.compile(r"(// SPDX-License-Identifier:\s*([^\n]*)\s)")
 VERSION_PRAGMA_PATTERN = re.compile(r"pragma solidity[^;]*;")
 DEFAULT_OPTIMIZATION_RUNS = 200
 
 
 class SolidityConfig(PluginConfig):
-    # Configure re-mappings using a `=` separated-str,
-    # e.g. '@import_name=path/to/dependency'
+    """
+    Configure the Solidity plugin.
+    """
+
     import_remapping: List[str] = []
+    """
+    Configure re-mappings using a ``=`` separated-str,
+    e.g. ``"@import_name=path/to/dependency"``.
+    """
+
     optimize: bool = True
+    """
+    Set to ``False`` to disable compiler-optimizations.
+    """
+
     version: Optional[str] = None
+    """
+    The compiler version to use. Defaults to selecting
+    the best version(s) it can for each file-set.
+    """
+
     evm_version: Optional[str] = None
+    """
+    The EVM version (fork) to use. Defaults to letting
+    the compiler decide.
+    """
+
     via_ir: Optional[bool] = None
+    """
+    Set to ``True`` to turn on compilation mode via the IR.
+    Defaults to ``None`` which does not pass the flag to
+    the compiler (same as ``False``).
+    """
 
 
 class SolidityCompiler(CompilerAPI):
     _import_remapping_hash: Optional[int] = None
     _cached_project_path: Optional[Path] = None
     _cached_import_map: Dict[str, str] = {}
     _libraries: Dict[str, Dict[str, AddressType]] = {}
@@ -148,15 +173,16 @@
                     f"differs from installed: {settings_version}"
                 )
 
         return settings_version
 
     @cached_property
     def _ape_version(self) -> Version:
-        return Version(get_distribution("eth-ape").version.split(".dev")[0].strip())
+        version_str = get_package_version("eth-ape").split(".dev")[0].strip()
+        return Version(version_str)
 
     def add_library(self, *contracts: ContractInstance):
         """
         Set a library contract type address. This is useful when deploying a library
         in a local network and then adding the address afterward. Now, when
         compiling again, it will use the new address.
```

### Comparing `ape-solidity-0.7.2/ape_solidity/exceptions.py` & `ape-solidity-0.7.3/ape_solidity/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/ape_solidity.egg-info/PKG-INFO` & `ape-solidity-0.7.3/ape_solidity.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-solidity
-Version: 0.7.2
+Version: 0.7.3
 Summary: Plugin for Ape Ethereum Framework for compiling Solidity contracts
 Home-page: https://github.com/ApeWorX/ape-solidity
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
@@ -29,15 +30,15 @@
 
 # Quick Start
 
 Compile Solidity contracts.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-solidity-0.7.2/ape_solidity.egg-info/SOURCES.txt` & `ape-solidity-0.7.3/ape_solidity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/ape_solidity.egg-info/requires.txt` & `ape-solidity-0.7.3/ape_solidity.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 pytest-mock
 hypothesis<7.0,>=6.2.0
 pytest-benchmark
-black<25,>=24.3.0
-mypy<2,>=1.9.0
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-requests
 types-setuptools
 types-pkg-resources
 flake8<8,>=7.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
@@ -37,21 +37,21 @@
 
 [doc]
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
 
 [lint]
-black<25,>=24.3.0
-mypy<2,>=1.9.0
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-requests
 types-setuptools
 types-pkg-resources
 flake8<8,>=7.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 
 [release]
 setuptools
```

### Comparing `ape-solidity-0.7.2/pyproject.toml` & `ape-solidity-0.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/setup.py` & `ape-solidity-0.7.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,21 @@
         "pytest-xdist",  # Multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "pytest-mock",  # For creating and using mocks
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
         "pytest-benchmark",  # For performance tests
     ],
     "lint": [
-        "black>=24.3.0,<25",  # Auto-formatter and linter
-        "mypy>=1.9.0,<2",  # Static type analyzer
+        "black>=24.4.2,<25",  # Auto-formatter and linter
+        "mypy>=1.10.0,<2",  # Static type analyzer
         "types-requests",  # Needed for mypy type shed
         "types-setuptools",  # Needed for mypy type shed
         "types-pkg-resources",  # Needed for type checking tests
         "flake8>=7.0.0,<8",  # Style linter
-        "isort>=5.10.1,<6",  # Import sorting linter
+        "isort>=5.13.2,<6",  # Import sorting linter
         "mdformat>=0.7.17",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
         "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
     ],
     "doc": [
         "Sphinx>=6.1.3,<7",  # Documentation generator
@@ -91,9 +91,10 @@
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `ape-solidity-0.7.2/tests/ape-config.yaml` & `ape-solidity-0.7.3/tests/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/tests/conftest.py` & `ape-solidity-0.7.3/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import shutil
 from contextlib import contextmanager
-from distutils.dir_util import copy_tree
 from pathlib import Path
+from shutil import copytree
 from tempfile import mkdtemp
 from unittest import mock
 
 import ape
 import pytest
 import solcx
 
@@ -53,15 +53,15 @@
     with _tmp_solcx_path(monkeypatch) as path:
         yield path
 
 
 @pytest.fixture(autouse=True)
 def data_folder():
     base_path = Path(__file__).parent / "data"
-    copy_tree(base_path.as_posix(), DATA_FOLDER.as_posix())
+    copytree(base_path, DATA_FOLDER, dirs_exist_ok=True)
     return DATA_FOLDER
 
 
 @pytest.fixture
 def config():
     return ape.config
 
@@ -83,15 +83,15 @@
         project_path / "ProjectWithinProject",
         project_path / "VersionSpecifiedInConfig",
     ):
         for cache in (path / ".build", path / "contracts" / ".cache"):
             if cache.is_dir():
                 shutil.rmtree(cache)
 
-    copy_tree(project_source_dir.as_posix(), project_dest_dir.as_posix())
+    copytree(project_source_dir, project_dest_dir, dirs_exist_ok=True)
     with config.using_project(project_dest_dir) as project:
         yield project
         if project.local_project._cache_folder.is_dir():
             shutil.rmtree(project.local_project._cache_folder)
 
 
 @pytest.fixture
@@ -143,9 +143,9 @@
 @pytest.fixture
 def not_owner():
     return ape.accounts.test_accounts[2]
 
 
 @pytest.fixture
 def connection():
-    with ape.networks.ethereum.local.use_provider("test"):
-        yield
+    with ape.networks.ethereum.local.use_provider("test") as provider:
+        yield provider
```

### Comparing `ape-solidity-0.7.2/tests/contracts/Imports.sol` & `ape-solidity-0.7.3/tests/contracts/Imports.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/tests/contracts/LibraryFun.sol` & `ape-solidity-0.7.3/tests/contracts/LibraryFun.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/tests/data/ImportingLessConstrainedVersionFlat.sol` & `ape-solidity-0.7.3/tests/data/ImportingLessConstrainedVersionFlat.sol`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/tests/data/ImportsFlattened.sol.txt` & `ape-solidity-0.7.3/tests/data/ImportsFlattened.sol.txt`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json` & `ape-solidity-0.7.3/tests/data/packages/OpenZeppelin/v4.5.0/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json` & `ape-solidity-0.7.3/tests/data/packages/OpenZeppelin/v4.7.1/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/tests/data/packages/vault/master/vault_main.json` & `ape-solidity-0.7.3/tests/data/packages/vault/master/vault_main.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/tests/data/packages/vault/v0.4.5/vault.json` & `ape-solidity-0.7.3/tests/data/packages/vault/v0.4.5/vault.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/tests/package-lock.json` & `ape-solidity-0.7.3/tests/package-lock.json`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/tests/scripts/clean.py` & `ape-solidity-0.7.3/tests/scripts/clean.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/tests/test_compiler.py` & `ape-solidity-0.7.3/tests/test_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import pytest
 import solcx
 from ape import reverts
 from ape.contracts import ContractContainer
 from ape.exceptions import CompilerError
 from ape.logging import LogLevel
 from packaging.version import Version
-from pkg_resources import get_distribution
 from requests.exceptions import ConnectionError
 
 from ape_solidity import Extension
 from ape_solidity._utils import OUTPUT_SELECTION
 from ape_solidity.exceptions import IndexOutOfBoundsError
 
 BASE_PATH = Path(__file__).parent / "contracts"
@@ -33,15 +32,14 @@
     "MultipleDefinitions",
     "RandomVyperFile",
     "LibraryFun",
     "JustAStruct",
 )
 raises_because_not_sol = pytest.raises(CompilerError, match=EXPECTED_NON_SOLIDITY_ERR_MSG)
 DEFAULT_OPTIMIZER = {"enabled": True, "runs": 200}
-APE_VERSION = Version(get_distribution("eth-ape").version.split(".dev")[0].strip())
 
 
 @pytest.mark.parametrize(
     "contract",
     [c for c in TEST_CONTRACTS if all(n not in str(c) for n in normal_test_skips)],
 )
 def test_compile(project, contract):
```

### Comparing `ape-solidity-0.7.2/tests/test_exceptions.py` & `ape-solidity-0.7.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-solidity-0.7.2/tests/test_integration.py` & `ape-solidity-0.7.3/tests/test_integration.py`

 * *Files identical despite different names*

