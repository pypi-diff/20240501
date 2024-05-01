# Comparing `tmp/UniswapPy-1.3.0.tar.gz` & `tmp/uniswappy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UniswapPy-1.3.0.tar", last modified: Thu Apr 25 15:01:13 2024, max compression
+gzip compressed data, was "uniswappy-1.4.0.tar", last modified: Wed May  1 19:05:50 2024, max compression
```

## Comparing `UniswapPy-1.3.0.tar` & `uniswappy-1.4.0.tar`

### file list

```diff
@@ -1,130 +1,133 @@
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.911008 UniswapPy-1.3.0/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1065 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/LICENSE.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)     4544 2024-04-25 15:01:13.911077 UniswapPy-1.3.0/PKG-INFO
--rw-r--r--   0 ian_moore   (501) staff       (20)     4248 2024-04-25 14:42:37.000000 UniswapPy-1.3.0/README.md
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.891244 UniswapPy-1.3.0/UniswapPy.egg-info/
--rw-r--r--   0 ian_moore   (501) staff       (20)     4544 2024-04-25 15:01:13.000000 UniswapPy-1.3.0/UniswapPy.egg-info/PKG-INFO
--rw-r--r--   0 ian_moore   (501) staff       (20)     3565 2024-04-25 15:01:13.000000 UniswapPy-1.3.0/UniswapPy.egg-info/SOURCES.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-04-25 15:01:13.000000 UniswapPy-1.3.0/UniswapPy.egg-info/dependency_links.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-02-11 00:15:12.000000 UniswapPy-1.3.0/UniswapPy.egg-info/not-zip-safe
--rw-r--r--   0 ian_moore   (501) staff       (20)       13 2024-04-25 15:01:13.000000 UniswapPy-1.3.0/UniswapPy.egg-info/requires.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)       10 2024-04-25 15:01:13.000000 UniswapPy-1.3.0/UniswapPy.egg-info/top_level.txt
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.888201 UniswapPy-1.3.0/python/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.891373 UniswapPy-1.3.0/python/prod/
--rw-r--r--   0 ian_moore   (501) staff       (20)      880 2024-04-25 02:25:34.000000 UniswapPy-1.3.0/python/prod/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.888577 UniswapPy-1.3.0/python/prod/cpt/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.892746 UniswapPy-1.3.0/python/prod/cpt/exchg/
--rw-r--r--   0 ian_moore   (501) staff       (20)     7376 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/cpt/exchg/ChildUniswapExchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)    21642 2024-04-25 02:25:34.000000 UniswapPy-1.3.0/python/prod/cpt/exchg/UniswapExchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)    40686 2024-04-25 02:33:33.000000 UniswapPy-1.3.0/python/prod/cpt/exchg/UniswapV3Exchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      148 2024-04-23 22:24:39.000000 UniswapPy-1.3.0/python/prod/cpt/exchg/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.893263 UniswapPy-1.3.0/python/prod/cpt/factory/
--rw-r--r--   0 ian_moore   (501) staff       (20)     4228 2024-04-25 02:27:11.000000 UniswapPy-1.3.0/python/prod/cpt/factory/UniswapFactory.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       44 2024-02-07 00:37:49.000000 UniswapPy-1.3.0/python/prod/cpt/factory/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.894048 UniswapPy-1.3.0/python/prod/cpt/index/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1719 2024-02-13 21:41:28.000000 UniswapPy-1.3.0/python/prod/cpt/index/RebaseIndexToken.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1712 2024-02-13 21:41:15.000000 UniswapPy-1.3.0/python/prod/cpt/index/SettlementLPToken.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/cpt/index/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.895102 UniswapPy-1.3.0/python/prod/cpt/quote/
--rw-r--r--   0 ian_moore   (501) staff       (20)     6938 2024-02-13 21:15:34.000000 UniswapPy-1.3.0/python/prod/cpt/quote/IndexTokenQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     6990 2024-02-13 21:32:43.000000 UniswapPy-1.3.0/python/prod/cpt/quote/LPQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1752 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/cpt/quote/LPTokenQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/cpt/quote/TreeAmountQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/cpt/quote/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.895558 UniswapPy-1.3.0/python/prod/cpt/vault/
--rw-r--r--   0 ian_moore   (501) staff       (20)    15329 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/cpt/vault/IndexVault.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      651 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/cpt/vault/Vault.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       59 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/cpt/vault/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.895912 UniswapPy-1.3.0/python/prod/cpt/wallet/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2646 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/cpt/wallet/Wallets.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/cpt/wallet/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.897031 UniswapPy-1.3.0/python/prod/erc/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1684 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/erc/DOAERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1456 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/erc/ERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1103 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/erc/IndexERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1720 2024-02-13 20:20:33.000000 UniswapPy-1.3.0/python/prod/erc/LPERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      119 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/erc/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.889014 UniswapPy-1.3.0/python/prod/math/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.897495 UniswapPy-1.3.0/python/prod/math/basic/
--rw-r--r--   0 ian_moore   (501) staff       (20)      500 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/basic/IDGenerator.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      485 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/basic/RoundFloat.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       52 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/basic/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.897883 UniswapPy-1.3.0/python/prod/math/interest/
--rw-r--r--   0 ian_moore   (501) staff       (20)      410 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/interest/CompoundReturn.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      519 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/interest/Yield.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       50 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/interest/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.898270 UniswapPy-1.3.0/python/prod/math/interest/ips/
--rw-r--r--   0 ian_moore   (501) staff       (20)      766 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/interest/ips/ConstantIPS.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      390 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/interest/ips/IPS.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       45 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/interest/ips/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.898525 UniswapPy-1.3.0/python/prod/math/interest/ips/aggregate/
--rw-r--r--   0 ian_moore   (501) staff       (20)      496 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/interest/ips/aggregate/AggregateIPS.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       27 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/interest/ips/aggregate/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.899289 UniswapPy-1.3.0/python/prod/math/model/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2069 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/model/BrownianModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      504 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/model/EventSelectionModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      591 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/model/ModelQueue.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      762 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/model/TimeDeltaModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1262 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/model/TokenDeltaModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      151 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/model/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.899660 UniswapPy-1.3.0/python/prod/math/risk/
--rw-r--r--   0 ian_moore   (501) staff       (20)     5556 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/risk/MaxDrop.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       22 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/risk/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.899942 UniswapPy-1.3.0/python/prod/process/
--rw-r--r--   0 ian_moore   (501) staff       (20)      300 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/Process.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/process/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.900315 UniswapPy-1.3.0/python/prod/process/burn/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2470 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/burn/IndexTokenBurn.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       43 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/process/burn/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.900577 UniswapPy-1.3.0/python/prod/process/deposit/
--rw-r--r--   0 ian_moore   (501) staff       (20)     3690 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/deposit/SwapDeposit.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/process/deposit/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.901070 UniswapPy-1.3.0/python/prod/process/liquidity/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2434 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/liquidity/AddLiquidity.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     2393 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/liquidity/RemoveLiquidity.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       83 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/process/liquidity/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.901427 UniswapPy-1.3.0/python/prod/process/mint/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2747 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/mint/SwapIndexMint.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       40 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/process/mint/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.903885 UniswapPy-1.3.0/python/prod/process/swap/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2329 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/process/swap/RandomSwap.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1805 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/swap/Swap.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     3996 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/swap/WithdrawSwap.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/process/swap/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.906994 UniswapPy-1.3.0/python/prod/simulate/
--rw-r--r--   0 ian_moore   (501) staff       (20)     3383 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/simulate/Arbitrage.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     4185 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/simulate/CorrectReserves.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     3648 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/simulate/MarkovState.py
--rw-r--r--   0 ian_moore   (501) staff       (20)    15429 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/simulate/QuantTerminal.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     2712 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/simulate/SimpleLPSimulation.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1850 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/simulate/SolveDeltas.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      244 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/simulate/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.889730 UniswapPy-1.3.0/python/prod/utils/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.907597 UniswapPy-1.3.0/python/prod/utils/client/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2164 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/utils/client/API0x.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       24 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/utils/client/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.908484 UniswapPy-1.3.0/python/prod/utils/data/
--rw-r--r--   0 ian_moore   (501) staff       (20)    10464 2024-04-25 01:17:59.000000 UniswapPy-1.3.0/python/prod/utils/data/Chain0x.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      261 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/utils/data/ExchangeData.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      324 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/utils/data/FactoryData.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      628 2024-04-23 22:24:39.000000 UniswapPy-1.3.0/python/prod/utils/data/UniswapExchangeData.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/utils/data/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.908920 UniswapPy-1.3.0/python/prod/utils/interfaces/
--rw-r--r--   0 ian_moore   (501) staff       (20)      439 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/utils/interfaces/IExchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      506 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/utils/interfaces/IExchangeFactory.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-02-07 00:37:49.000000 UniswapPy-1.3.0/python/prod/utils/interfaces/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.889767 UniswapPy-1.3.0/python/prod/utils/tools/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.910856 UniswapPy-1.3.0/python/prod/utils/tools/v3/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1331 2024-04-25 02:27:11.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/FullMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      844 2024-04-25 02:27:11.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/LiquidityMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     4659 2024-04-24 18:20:10.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/Position.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1928 2024-04-24 18:20:10.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/SafeMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     6201 2024-04-24 18:20:10.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/Shared.py
--rw-r--r--   0 ian_moore   (501) staff       (20)    10440 2024-04-24 18:20:10.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/SqrtPriceMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     4961 2024-04-24 18:20:10.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/SwapMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     7724 2024-04-24 18:20:10.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/Tick.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     6407 2024-04-24 18:20:10.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/TickMath.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     7573 2024-04-25 02:27:11.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/UniV3Utils.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      266 2024-04-25 02:27:11.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/__init__.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-04-25 15:01:13.911280 UniswapPy-1.3.0/setup.cfg
--rw-r--r--   0 ian_moore   (501) staff       (20)     1478 2024-04-23 22:24:39.000000 UniswapPy-1.3.0/setup.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.539687 uniswappy-1.4.0/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1065 2024-02-07 00:37:32.000000 uniswappy-1.4.0/LICENSE.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-05-01 19:05:50.539627 uniswappy-1.4.0/PKG-INFO
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4341 2024-05-01 19:05:23.000000 uniswappy-1.4.0/README.md
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.539382 uniswappy-1.4.0/UniswapPy.egg-info/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-05-01 19:05:50.000000 uniswappy-1.4.0/UniswapPy.egg-info/PKG-INFO
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3635 2024-05-01 19:05:50.000000 uniswappy-1.4.0/UniswapPy.egg-info/SOURCES.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-05-01 19:05:50.000000 uniswappy-1.4.0/UniswapPy.egg-info/dependency_links.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-02-11 00:15:12.000000 uniswappy-1.4.0/UniswapPy.egg-info/not-zip-safe
+-rw-r--r--   0 ian_moore   (501) staff       (20)       30 2024-05-01 19:05:50.000000 uniswappy-1.4.0/UniswapPy.egg-info/requires.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)       10 2024-05-01 19:05:50.000000 uniswappy-1.4.0/UniswapPy.egg-info/top_level.txt
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.518165 uniswappy-1.4.0/python/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.524136 uniswappy-1.4.0/python/prod/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      917 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.518593 uniswappy-1.4.0/python/prod/cpt/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.525171 uniswappy-1.4.0/python/prod/cpt/exchg/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7376 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/cpt/exchg/ChildUniswapExchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    21859 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/exchg/UniswapExchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    42515 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/exchg/UniswapV3Exchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      148 2024-04-23 22:24:39.000000 uniswappy-1.4.0/python/prod/cpt/exchg/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.525613 uniswappy-1.4.0/python/prod/cpt/factory/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4208 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/factory/UniswapFactory.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       44 2024-02-07 00:37:49.000000 uniswappy-1.4.0/python/prod/cpt/factory/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.526215 uniswappy-1.4.0/python/prod/cpt/index/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2508 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/index/RebaseIndexToken.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2485 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/index/SettlementLPToken.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/cpt/index/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.527111 uniswappy-1.4.0/python/prod/cpt/quote/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6933 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/quote/IndexTokenQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6973 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/quote/LPQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1752 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/cpt/quote/LPTokenQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/cpt/quote/TreeAmountQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/cpt/quote/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.527574 uniswappy-1.4.0/python/prod/cpt/vault/
+-rw-r--r--   0 ian_moore   (501) staff       (20)    15304 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/cpt/vault/IndexVault.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      651 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/cpt/vault/Vault.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       59 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/cpt/vault/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.527918 uniswappy-1.4.0/python/prod/cpt/wallet/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2646 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/cpt/wallet/Wallets.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/cpt/wallet/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.528874 uniswappy-1.4.0/python/prod/erc/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1664 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/erc/DOAERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1441 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/erc/ERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1088 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/erc/IndexERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1700 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/erc/LPERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      119 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/erc/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.519066 uniswappy-1.4.0/python/prod/math/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.529368 uniswappy-1.4.0/python/prod/math/basic/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      500 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/basic/IDGenerator.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      485 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/basic/RoundFloat.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       52 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/basic/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.529835 uniswappy-1.4.0/python/prod/math/interest/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      410 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/interest/CompoundReturn.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      519 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/interest/Yield.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       50 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/interest/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.530272 uniswappy-1.4.0/python/prod/math/interest/ips/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      766 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/interest/ips/ConstantIPS.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      390 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/interest/ips/IPS.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       45 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/interest/ips/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.530584 uniswappy-1.4.0/python/prod/math/interest/ips/aggregate/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      496 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/interest/ips/aggregate/AggregateIPS.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       27 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/interest/ips/aggregate/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.531421 uniswappy-1.4.0/python/prod/math/model/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2069 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/model/BrownianModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      504 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/model/EventSelectionModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      591 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/model/ModelQueue.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      762 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/model/TimeDeltaModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1262 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/model/TokenDeltaModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      151 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/math/model/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.531751 uniswappy-1.4.0/python/prod/math/risk/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     5551 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/math/risk/MaxDrop.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       22 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/math/risk/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.532020 uniswappy-1.4.0/python/prod/process/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      301 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/Process.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/process/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.532446 uniswappy-1.4.0/python/prod/process/burn/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2465 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/burn/IndexTokenBurn.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       43 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/process/burn/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.532745 uniswappy-1.4.0/python/prod/process/deposit/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     5363 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/deposit/SwapDeposit.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/process/deposit/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.533020 uniswappy-1.4.0/python/prod/process/join/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1650 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/join/Join.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       22 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/join/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.533427 uniswappy-1.4.0/python/prod/process/liquidity/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3527 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/liquidity/AddLiquidity.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3200 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/liquidity/RemoveLiquidity.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       83 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/process/liquidity/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.533688 uniswappy-1.4.0/python/prod/process/mint/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2737 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/mint/SwapIndexMint.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       40 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/process/mint/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.534270 uniswappy-1.4.0/python/prod/process/swap/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2319 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/swap/RandomSwap.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2566 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/swap/Swap.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     5632 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/process/swap/WithdrawSwap.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 uniswappy-1.4.0/python/prod/process/swap/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.535795 uniswappy-1.4.0/python/prod/simulate/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3383 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/simulate/Arbitrage.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4185 2024-04-10 18:17:44.000000 uniswappy-1.4.0/python/prod/simulate/CorrectReserves.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3648 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/simulate/MarkovState.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    15429 2024-04-10 18:17:44.000000 uniswappy-1.4.0/python/prod/simulate/QuantTerminal.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2712 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/simulate/SimpleLPSimulation.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1850 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/simulate/SolveDeltas.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      244 2024-04-10 18:17:44.000000 uniswappy-1.4.0/python/prod/simulate/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.519920 uniswappy-1.4.0/python/prod/utils/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.536202 uniswappy-1.4.0/python/prod/utils/client/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2164 2024-04-10 18:17:44.000000 uniswappy-1.4.0/python/prod/utils/client/API0x.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       24 2024-04-10 18:17:44.000000 uniswappy-1.4.0/python/prod/utils/client/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.537019 uniswappy-1.4.0/python/prod/utils/data/
+-rw-r--r--   0 ian_moore   (501) staff       (20)    10464 2024-04-25 01:17:59.000000 uniswappy-1.4.0/python/prod/utils/data/Chain0x.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      261 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/utils/data/ExchangeData.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      324 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/utils/data/FactoryData.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      628 2024-04-23 22:24:39.000000 uniswappy-1.4.0/python/prod/utils/data/UniswapExchangeData.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-04-10 18:17:44.000000 uniswappy-1.4.0/python/prod/utils/data/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.537411 uniswappy-1.4.0/python/prod/utils/interfaces/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      439 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/utils/interfaces/IExchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      506 2024-02-11 00:47:28.000000 uniswappy-1.4.0/python/prod/utils/interfaces/IExchangeFactory.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-02-07 00:37:49.000000 uniswappy-1.4.0/python/prod/utils/interfaces/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.519965 uniswappy-1.4.0/python/prod/utils/tools/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-05-01 19:05:50.539202 uniswappy-1.4.0/python/prod/utils/tools/v3/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1331 2024-04-25 02:27:11.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/FullMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      844 2024-04-25 02:27:11.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/LiquidityMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4659 2024-04-24 18:20:10.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/Position.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1928 2024-04-24 18:20:10.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/SafeMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6201 2024-04-24 18:20:10.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/Shared.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    10496 2024-05-01 19:05:23.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/SqrtPriceMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4961 2024-04-24 18:20:10.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/SwapMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7724 2024-04-24 18:20:10.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/Tick.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6407 2024-04-24 18:20:10.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/TickMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7573 2024-04-25 02:27:11.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/UniV3Utils.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      266 2024-04-25 02:27:11.000000 uniswappy-1.4.0/python/prod/utils/tools/v3/__init__.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-05-01 19:05:50.539978 uniswappy-1.4.0/setup.cfg
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1537 2024-05-01 19:05:23.000000 uniswappy-1.4.0/setup.py
```

### Comparing `UniswapPy-1.3.0/LICENSE.txt` & `uniswappy-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/PKG-INFO` & `uniswappy-1.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: UniswapPy
-Version: 1.3.0
+Version: 1.4.0
 Summary: Uniswap Analytics with Python
 Home-page: https://github.com/defipy-devs/uniswappy
 Author: icmoore
 Author-email: defipy.devs@gmail.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: scipy>=1.7.3
+Requires-Dist: termcolor>=2.4.0
 
 # UniswapPy: Uniswap V2 / V3 Analytics with Python
 This package contains python re-factors of both original Uniswap [V2](https://github.com/Uniswap/v2-core/blob/master/contracts/UniswapV2Pair.sol) and [V3](https://github.com/Uniswap/v3-core/blob/main/contracts/UniswapV3Pool.sol)
 pairing codes, and can be utilized for the purpose of analysing and modelling its behavior for DeFi
 
 ## Docs
 Visit [docs](https://defipy.org) for full documentation with walk-through 
@@ -26,73 +27,92 @@
 or
 ```
 > pip install UniswapPy
 ```
 
 ## Uniswap V2
 
-* See [test notebook](https://github.com/icmoore/uniswappy/blob/main/notebooks/tutorials/pairingcode.ipynb) 
+* See [test notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/uniswap_v2.ipynb) 
 for basic usage
 
 ```
 from uniswappy import *
 
-user_nm = 'user_intro'
-eth_amount = 3162.277660168379
-dai_amount = 316227.7660168379
+user_nm = 'user'
+eth_amount = 1000
+tkn_amount = 100000
 
-dai = ERC20("DAI", "0x111")
+tkn = ERC20("TKN", "0x111")
 eth = ERC20("ETH", "0x09")
-exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", 
-address="0x011")
+exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = tkn, symbol="LP", address="0x011")
 
 factory = UniswapFactory("ETH pool factory", "0x2")
 lp = factory.deploy(exchg_data)
-lp.add_liquidity("user0", eth_amount, dai_amount, eth_amount, dai_amount)
+
+Join().apply(lp, user_nm, eth_amount, tkn_amount)
+lp.summary()
+```
+
+#### OUTPUT:
+Exchange ETH-TKN (LP) <br/>
+Reserves: ETH = 1000, TKN = 100000 <br/>
+Liquidity: 10000.0 <br/><br/> 
+
+```
+out = Swap().apply(lp, tkn, user_nm, 1000)
 lp.summary()
 ```
 
 #### OUTPUT:
-Exchange ETH-DAI (LP) <br/>
-Reserves: ETH = 3162.277660168379, DAI = 316227.7660168379  <br/>
-Liquidity: 31622.776601683792 <br/><br/> 
+Exchange ETH-TKN (LP) <br/>
+Reserves: 990.1284196560293, TKN = 101000 <br/>
+Liquidity: 10000.0 <br/><br/> 
 
 
 ## Uniswap V3
 
 * See [test notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/uniswap_v3.ipynb) 
 for basic usage
 
 ```
-user = 'user_intro'
-fee = UniV3Utils.FeeAmount.MEDIUM
-tick_spacing = UniV3Utils.TICK_SPACINGS[fee]
-lwr_tick = UniV3Utils.getMinTick(tick_spacing)
-upr_tick = UniV3Utils.getMaxTick(tick_spacing)
-init_price = UniV3Utils.encodePriceSqrt(100, 1)
+from uniswappy import *
 
-dai = ERC20("DAI", "0x09")
-eth = ERC20("ETH", "0x111")
+user_nm = 'user'
+eth_amount = 1000
+tkn_amount = 100000
+
+eth = ERC20("ETH", "0x09")
+tkn = ERC20("TKN", "0x111")
 
-exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", 
+exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = tkn, symbol="LP", 
                                    address="0x011", version = 'V3', 
                                    tick_spacing = tick_spacing, 
                                    fee = fee)
 
 factory = UniswapFactory("ETH pool factory", "0x2")
 lp = factory.deploy(exchg_data)
-lp.initialize(init_price)
-out = lp.mint(user, lwr_tick, upr_tick, 31622.776601683792)
+
+out_v3 = Join().apply(lp, user_nm, eth_amount, tkn_amount, lwr_tick, upr_tick)
 lp.summary()
 ```
 
 #### OUTPUT:
-Exchange ETH-DAI (LP) <br/>
-Reserves: ETH = 3162.277660168379, DAI = 316227.7660168379 <br/>
-Liquidity: 31622.776601683792 <br/><br/>  
+Exchange ETH-TKN (LP) <br/>
+Reserves: ETH = 1000, TKN = 100000 <br/>
+Liquidity: 10000.0 <br/><br/> 
+
+```
+out = Swap().apply(lp, tkn, user_nm, 1000)
+lp.summary()
+```
+
+#### OUTPUT:
+Exchange ETH-TKN (LP) <br/>
+Real Reserves: ETH = 990.1284196560293, TKN = 101000 <br/>
+Liquidity: 10000.0 <br/><br/> 
 
 
 ## 0x Quant Terminal
 
 This application utilizes the 0x API to produce a mock Uniswap pool which allows end-users to stress test
 the limitations of a Uniswap pool setup using live price feeds from [0x API](https://0x.org); for backend setup, see 
 [notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/quant_terminal.ipynb) 
@@ -125,9 +145,7 @@
  * **Randomized Events**: Token amount and time delta models to simulate 
 possible trading behavior
  * **Analytical Tools**: Basic yeild calculators and risk tools to assist 
 in analyzing outcomes
  
  
 
-
-
```

### Comparing `UniswapPy-1.3.0/README.md` & `uniswappy-1.4.0/UniswapPy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: UniswapPy
+Version: 1.4.0
+Summary: Uniswap Analytics with Python
+Home-page: https://github.com/defipy-devs/uniswappy
+Author: icmoore
+Author-email: defipy.devs@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: scipy>=1.7.3
+Requires-Dist: termcolor>=2.4.0
+
 # UniswapPy: Uniswap V2 / V3 Analytics with Python
 This package contains python re-factors of both original Uniswap [V2](https://github.com/Uniswap/v2-core/blob/master/contracts/UniswapV2Pair.sol) and [V3](https://github.com/Uniswap/v3-core/blob/main/contracts/UniswapV3Pool.sol)
 pairing codes, and can be utilized for the purpose of analysing and modelling its behavior for DeFi
 
 ## Docs
 Visit [docs](https://defipy.org) for full documentation with walk-through 
 tutorials
@@ -14,73 +27,92 @@
 or
 ```
 > pip install UniswapPy
 ```
 
 ## Uniswap V2
 
-* See [test notebook](https://github.com/icmoore/uniswappy/blob/main/notebooks/tutorials/pairingcode.ipynb) 
+* See [test notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/uniswap_v2.ipynb) 
 for basic usage
 
 ```
 from uniswappy import *
 
-user_nm = 'user_intro'
-eth_amount = 3162.277660168379
-dai_amount = 316227.7660168379
+user_nm = 'user'
+eth_amount = 1000
+tkn_amount = 100000
 
-dai = ERC20("DAI", "0x111")
+tkn = ERC20("TKN", "0x111")
 eth = ERC20("ETH", "0x09")
-exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", 
-address="0x011")
+exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = tkn, symbol="LP", address="0x011")
 
 factory = UniswapFactory("ETH pool factory", "0x2")
 lp = factory.deploy(exchg_data)
-lp.add_liquidity("user0", eth_amount, dai_amount, eth_amount, dai_amount)
+
+Join().apply(lp, user_nm, eth_amount, tkn_amount)
 lp.summary()
 ```
 
 #### OUTPUT:
-Exchange ETH-DAI (LP) <br/>
-Reserves: ETH = 3162.277660168379, DAI = 316227.7660168379  <br/>
-Liquidity: 31622.776601683792 <br/><br/> 
+Exchange ETH-TKN (LP) <br/>
+Reserves: ETH = 1000, TKN = 100000 <br/>
+Liquidity: 10000.0 <br/><br/> 
+
+```
+out = Swap().apply(lp, tkn, user_nm, 1000)
+lp.summary()
+```
+
+#### OUTPUT:
+Exchange ETH-TKN (LP) <br/>
+Reserves: 990.1284196560293, TKN = 101000 <br/>
+Liquidity: 10000.0 <br/><br/> 
 
 
 ## Uniswap V3
 
 * See [test notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/uniswap_v3.ipynb) 
 for basic usage
 
 ```
-user = 'user_intro'
-fee = UniV3Utils.FeeAmount.MEDIUM
-tick_spacing = UniV3Utils.TICK_SPACINGS[fee]
-lwr_tick = UniV3Utils.getMinTick(tick_spacing)
-upr_tick = UniV3Utils.getMaxTick(tick_spacing)
-init_price = UniV3Utils.encodePriceSqrt(100, 1)
+from uniswappy import *
 
-dai = ERC20("DAI", "0x09")
-eth = ERC20("ETH", "0x111")
+user_nm = 'user'
+eth_amount = 1000
+tkn_amount = 100000
 
-exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", 
+eth = ERC20("ETH", "0x09")
+tkn = ERC20("TKN", "0x111")
+
+exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = tkn, symbol="LP", 
                                    address="0x011", version = 'V3', 
                                    tick_spacing = tick_spacing, 
                                    fee = fee)
 
 factory = UniswapFactory("ETH pool factory", "0x2")
 lp = factory.deploy(exchg_data)
-lp.initialize(init_price)
-out = lp.mint(user, lwr_tick, upr_tick, 31622.776601683792)
+
+out_v3 = Join().apply(lp, user_nm, eth_amount, tkn_amount, lwr_tick, upr_tick)
+lp.summary()
+```
+
+#### OUTPUT:
+Exchange ETH-TKN (LP) <br/>
+Reserves: ETH = 1000, TKN = 100000 <br/>
+Liquidity: 10000.0 <br/><br/> 
+
+```
+out = Swap().apply(lp, tkn, user_nm, 1000)
 lp.summary()
 ```
 
 #### OUTPUT:
-Exchange ETH-DAI (LP) <br/>
-Reserves: ETH = 3162.277660168379, DAI = 316227.7660168379 <br/>
-Liquidity: 31622.776601683792 <br/><br/>  
+Exchange ETH-TKN (LP) <br/>
+Real Reserves: ETH = 990.1284196560293, TKN = 101000 <br/>
+Liquidity: 10000.0 <br/><br/> 
 
 
 ## 0x Quant Terminal
 
 This application utilizes the 0x API to produce a mock Uniswap pool which allows end-users to stress test
 the limitations of a Uniswap pool setup using live price feeds from [0x API](https://0x.org); for backend setup, see 
 [notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/quant_terminal.ipynb)
```

### Comparing `UniswapPy-1.3.0/UniswapPy.egg-info/PKG-INFO` & `uniswappy-1.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: UniswapPy
-Version: 1.3.0
-Summary: Uniswap Analytics with Python
-Home-page: https://github.com/defipy-devs/uniswappy
-Author: icmoore
-Author-email: defipy.devs@gmail.com
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # UniswapPy: Uniswap V2 / V3 Analytics with Python
 This package contains python re-factors of both original Uniswap [V2](https://github.com/Uniswap/v2-core/blob/master/contracts/UniswapV2Pair.sol) and [V3](https://github.com/Uniswap/v3-core/blob/main/contracts/UniswapV3Pool.sol)
 pairing codes, and can be utilized for the purpose of analysing and modelling its behavior for DeFi
 
 ## Docs
 Visit [docs](https://defipy.org) for full documentation with walk-through 
 tutorials
@@ -26,73 +14,92 @@
 or
 ```
 > pip install UniswapPy
 ```
 
 ## Uniswap V2
 
-* See [test notebook](https://github.com/icmoore/uniswappy/blob/main/notebooks/tutorials/pairingcode.ipynb) 
+* See [test notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/uniswap_v2.ipynb) 
 for basic usage
 
 ```
 from uniswappy import *
 
-user_nm = 'user_intro'
-eth_amount = 3162.277660168379
-dai_amount = 316227.7660168379
+user_nm = 'user'
+eth_amount = 1000
+tkn_amount = 100000
 
-dai = ERC20("DAI", "0x111")
+tkn = ERC20("TKN", "0x111")
 eth = ERC20("ETH", "0x09")
-exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", 
-address="0x011")
+exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = tkn, symbol="LP", address="0x011")
 
 factory = UniswapFactory("ETH pool factory", "0x2")
 lp = factory.deploy(exchg_data)
-lp.add_liquidity("user0", eth_amount, dai_amount, eth_amount, dai_amount)
+
+Join().apply(lp, user_nm, eth_amount, tkn_amount)
+lp.summary()
+```
+
+#### OUTPUT:
+Exchange ETH-TKN (LP) <br/>
+Reserves: ETH = 1000, TKN = 100000 <br/>
+Liquidity: 10000.0 <br/><br/> 
+
+```
+out = Swap().apply(lp, tkn, user_nm, 1000)
 lp.summary()
 ```
 
 #### OUTPUT:
-Exchange ETH-DAI (LP) <br/>
-Reserves: ETH = 3162.277660168379, DAI = 316227.7660168379  <br/>
-Liquidity: 31622.776601683792 <br/><br/> 
+Exchange ETH-TKN (LP) <br/>
+Reserves: 990.1284196560293, TKN = 101000 <br/>
+Liquidity: 10000.0 <br/><br/> 
 
 
 ## Uniswap V3
 
 * See [test notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/uniswap_v3.ipynb) 
 for basic usage
 
 ```
-user = 'user_intro'
-fee = UniV3Utils.FeeAmount.MEDIUM
-tick_spacing = UniV3Utils.TICK_SPACINGS[fee]
-lwr_tick = UniV3Utils.getMinTick(tick_spacing)
-upr_tick = UniV3Utils.getMaxTick(tick_spacing)
-init_price = UniV3Utils.encodePriceSqrt(100, 1)
+from uniswappy import *
+
+user_nm = 'user'
+eth_amount = 1000
+tkn_amount = 100000
 
-dai = ERC20("DAI", "0x09")
-eth = ERC20("ETH", "0x111")
+eth = ERC20("ETH", "0x09")
+tkn = ERC20("TKN", "0x111")
 
-exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", 
+exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = tkn, symbol="LP", 
                                    address="0x011", version = 'V3', 
                                    tick_spacing = tick_spacing, 
                                    fee = fee)
 
 factory = UniswapFactory("ETH pool factory", "0x2")
 lp = factory.deploy(exchg_data)
-lp.initialize(init_price)
-out = lp.mint(user, lwr_tick, upr_tick, 31622.776601683792)
+
+out_v3 = Join().apply(lp, user_nm, eth_amount, tkn_amount, lwr_tick, upr_tick)
+lp.summary()
+```
+
+#### OUTPUT:
+Exchange ETH-TKN (LP) <br/>
+Reserves: ETH = 1000, TKN = 100000 <br/>
+Liquidity: 10000.0 <br/><br/> 
+
+```
+out = Swap().apply(lp, tkn, user_nm, 1000)
 lp.summary()
 ```
 
 #### OUTPUT:
-Exchange ETH-DAI (LP) <br/>
-Reserves: ETH = 3162.277660168379, DAI = 316227.7660168379 <br/>
-Liquidity: 31622.776601683792 <br/><br/>  
+Exchange ETH-TKN (LP) <br/>
+Real Reserves: ETH = 990.1284196560293, TKN = 101000 <br/>
+Liquidity: 10000.0 <br/><br/> 
 
 
 ## 0x Quant Terminal
 
 This application utilizes the 0x API to produce a mock Uniswap pool which allows end-users to stress test
 the limitations of a Uniswap pool setup using live price feeds from [0x API](https://0x.org); for backend setup, see 
 [notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/quant_terminal.ipynb) 
@@ -125,9 +132,7 @@
  * **Randomized Events**: Token amount and time delta models to simulate 
 possible trading behavior
  * **Analytical Tools**: Basic yeild calculators and risk tools to assist 
 in analyzing outcomes
  
  
 
-
-
```

### Comparing `UniswapPy-1.3.0/UniswapPy.egg-info/SOURCES.txt` & `uniswappy-1.4.0/UniswapPy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,16 @@
 python/prod/math/risk/__init__.py
 python/prod/process/Process.py
 python/prod/process/__init__.py
 python/prod/process/burn/IndexTokenBurn.py
 python/prod/process/burn/__init__.py
 python/prod/process/deposit/SwapDeposit.py
 python/prod/process/deposit/__init__.py
+python/prod/process/join/Join.py
+python/prod/process/join/__init__.py
 python/prod/process/liquidity/AddLiquidity.py
 python/prod/process/liquidity/RemoveLiquidity.py
 python/prod/process/liquidity/__init__.py
 python/prod/process/mint/SwapIndexMint.py
 python/prod/process/mint/__init__.py
 python/prod/process/swap/RandomSwap.py
 python/prod/process/swap/Swap.py
```

### Comparing `UniswapPy-1.3.0/python/prod/__init__.py` & `uniswappy-1.4.0/python/prod/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,12 +13,13 @@
 from uniswappy.math.risk import *
 from uniswappy.process import *
 from uniswappy.process.burn import *
 from uniswappy.process.deposit import *
 from uniswappy.process.liquidity import *
 from uniswappy.process.mint import *
 from uniswappy.process.swap import *
+from uniswappy.process.join import *
 from uniswappy.simulate import *
 from uniswappy.utils.interfaces import *
 from uniswappy.utils.data import *
 from uniswappy.utils.client import *
 from uniswappy.utils.tools.v3 import *
```

### Comparing `UniswapPy-1.3.0/python/prod/cpt/exchg/ChildUniswapExchange.py` & `uniswappy-1.4.0/python/prod/cpt/exchg/ChildUniswapExchange.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/cpt/exchg/UniswapExchange.py` & `uniswappy-1.4.0/python/prod/cpt/exchg/UniswapExchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,21 +14,22 @@
 class UniswapExchange(IExchange, LPERC20):
     
     """ 
         Uniswap V2 Exchange  
 
         Parameters
         -----------------
-        self.factory_struct : FactoryInit
+        factory_struct : FactoryInit
             Factory initialization data
-        self.exchg_struct : UniswapExchangeInit
+        exchg_struct : UniswapExchangeInit
             Exchange initialization data           
     """          
     def __init__(self, factory_struct: FactoryData, exchg_struct: UniswapExchangeData):
         super().__init__(exchg_struct.tkn0.token_name+exchg_struct.tkn1.token_name, exchg_struct.address)
+        self.version = exchg_struct.version
         self.factory = factory_struct
         self.token0 = exchg_struct.tkn0.token_name     
         self.token1 = exchg_struct.tkn1.token_name       
         self.reserve0 = 0             
         self.reserve1 = 0       
         self.fee0_arr = []
         self.fee1_arr = []
@@ -578,14 +579,23 @@
         elif(token.token_name == self.token1):
             if(self.reserve1 == 0):
                 return None
             else:
                 return self.reserve0/self.reserve1
         else:
             assert False, 'UniswapV2: WRONG_INPUT_TOKEN'      
+
+    def get_liquidity(self):  
+        
+        """ get_liquidity
+
+            Get liquidity of exchange pool         
+        """          
+
+        return self.total_supply       
             
     def get_reserve(self, token):  
         
         """ get_reserve
 
             Get reserve amount of select token in the exchange pair
```

### Comparing `UniswapPy-1.3.0/python/prod/cpt/exchg/UniswapV3Exchange.py` & `uniswappy-1.4.0/python/prod/cpt/exchg/UniswapV3Exchange.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,43 +42,14 @@
 @dataclass
 class SwapCache:
     ## the protocol fee for the input token
     feeProtocol: int
     ## liquidity at the beginning of the swap
     liquidityStart: int
 
-MINIMUM_LIQUIDITY = 1e-15
-
-@dataclass
-class Slot0:
-    ## the current price
-    sqrtPriceX96: int
-    ## the current tick
-    tick: int
-    ## the current protocol fee as a percentage of the swap fee taken on withdrawal
-    ## represented as an integer denominator (1#x)%
-    feeProtocol: int
-    
-@dataclass
-class ModifyPositionParams:
-    ## the address that owns the position
-    owner: str
-    ## the lower and upper tick of the position
-    tickLower: int
-    tickUpper: int
-    ## any change in liquidity
-    liquidityDelta: int  
-
-@dataclass
-class SwapCache:
-    ## the protocol fee for the input token
-    feeProtocol: int
-    ## liquidity at the beginning of the swap
-    liquidityStart: int
-
 @dataclass
 class SwapState:
     ## the amount remaining to be swapped in#out of the input#output asset
     amountSpecifiedRemaining: int
     ## the amount already swapped out#in of the output#input asset
     amountCalculated: int
     ## current sqrt(price)
@@ -120,22 +91,23 @@
 class UniswapV3Exchange(IExchange, LPERC20):
 
     """ 
         Uniswap V3 Exchange  
 
         Parameters
         -----------------
-        self.factory_struct : FactoryInit
+        factory_struct : FactoryInit
             Factory initialization data
-        self.exchg_struct : UniswapExchangeInit
+        exchg_struct : UniswapExchangeInit
             Exchange initialization data           
     """       
                        
     def __init__(self, factory_struct: FactoryData, exchg_struct: UniswapExchangeData):
         super().__init__(exchg_struct.tkn0.token_name+exchg_struct.tkn1.token_name, exchg_struct.address)
+        self.version = exchg_struct.version
         self.factory = factory_struct
         self.token0 = exchg_struct.tkn0.token_name     
         self.token1 = exchg_struct.tkn1.token_name       
         self.reserve0 = 0             
         self.reserve1 = 0 
         self.fee = exchg_struct.fee
         self.fee0_arr = []
@@ -160,22 +132,26 @@
         self.maxLiquidityPerTick = Tick.tickSpacingToMaxLiquidityPerTick(self.tickSpacing)      
 
     def summary(self):
 
         """ summary
             Summary print-out of exchange, reserves and liquidity              
         """         
-
+        
+        tokens = self.factory.token_from_exchange[self.name] 
+        
         print(f"Exchange {self.name} ({self.symbol})")
 
         if (self.precision == UniswapExchangeData.TYPE_GWEI):
-            print(f"Reserves: {self.token0} = {self.reserve0}, {self.token1} = {self.reserve1}")
+            print(f"Real Reserves:   {self.token0} = {self.reserve0}, {self.token1} = {self.reserve1}")
+            print(f"Virual Reserves: {self.token0} = {self.get_virtual_reserve(tokens[self.token0])}, {self.token1} = {self.get_virtual_reserve(tokens[self.token1])}")
             print(f"Liquidity: {self.total_supply} \n")
         else:  
-            print(f"Reserves: {self.token0} = {self.gwei2dec(self.reserve0)}, {self.token1} = {self.gwei2dec(self.reserve1)}")
+            print(f"Real Reserves:   {self.token0} = {self.gwei2dec(self.reserve0)}, {self.token1} = {self.gwei2dec(self.reserve1)}")
+            #print(f"Virual Reserves: {self.token0} = {self.get_virtual_reserve(tokens[self.token0])}, {self.token1} = {self.get_virtual_reserve(tokens[self.token1])}")
             print(f"Liquidity: {self.gwei2dec(self.total_supply)} \n")            
 
     def initialize(self, sqrtPriceX96):
 
         """ initialize
 
             Sets the initial price for the pool
@@ -205,28 +181,28 @@
             calculated are automatically transferred from the swapper to the pool and vice verse. 
             The amount of token0/token1 due depends on tickLower, tickUpper, the amount of liquidity, 
             and the current price.
                 
             Parameters
             -----------------    
             recipient : str
-                address for which the liquidity will be created      
+                Address for which the liquidity will be created      
             tickLower : int
-                lower tick of the position in which to add liquidity  
+                Lower tick of the position in which to add liquidity  
             tickUpper : int
-                upper tick of the position in which to add liquidity 
+                Upper tick of the position in which to add liquidity 
             amount : int
-                amount of liquidity to mint  
+                Amount of liquidity to mint  
                 
             Returns
             -------
             amount0 : float
-                amount of token0 that was paid to mint the given amount of liquidity.   
+                Amount of token0 that was paid to mint the given amount of liquidity.   
             amount1 : float
-                amount of token1 that was paid to mint the given amount of liquidity.                   
+                Amount of token1 that was paid to mint the given amount of liquidity.                   
         """          
 
         amount = amount if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount)
         
         checkInputTypes(
             accounts=(recipient), int24=(tickLower, tickUpper), uint128=(amount)
         )
@@ -271,31 +247,37 @@
             To withdraw only token0 or only token1, amount0Requested or amount1Requested may be set to zero. 
             To withdraw all tokens owed, caller may pass any value greater than the actual tokens owed, e.g. 
             type(uint128).max. Tokens owed may be from accumulated swap fees or burned liquidity.
                 
             Parameters
             -----------------    
             recipient : str
-                address for which the liquidity will be created      
+                Address for which the liquidity will be created      
             tickLower : int
-                lower tick of the position in which to add liquidity  
+                Lower tick of the position in which to add liquidity  
             tickUpper : int
-                lower tick of the position in which to add liquidity                 
+                Lower tick of the position in which to add liquidity                 
             amount0Requested : int
-                how much token0 should be withdrawn from the fees owed
+                How much token0 should be withdrawn from the fees owed
             amount1Requested : int
-                how much token1 should be withdrawn from the fees owed  
+                How much token1 should be withdrawn from the fees owed  
                 
             Returns
             -------
             amount0 : float
-                amount of token0 that was paid to mint the given amount of liquidity.   
+                Amount of token0 that was paid to mint the given amount of liquidity.   
             amount1 : float
-                amount of token1 that was paid to mint the given amount of liquidity.                   
-        """  
+                Amount of token1 that was paid to mint the given amount of liquidity.                   
+        """ 
+
+        amount0Requested = amount0Requested if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount0Requested)
+        amount1Requested = amount1Requested if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount1Requested)
+
+        print(f'amount0Requested {amount0Requested}')
+        print(f'amount1Requested {amount1Requested}')
         
         checkInputTypes(
             accounts=(recipient),
             int24=(tickLower, tickUpper),
             uint128=(amount0Requested, amount1Requested),
         )
         # Add this check to prevent creating a new position if the position doesn't exist or it's empty
@@ -310,19 +292,24 @@
         )
         amount1 = (
             position.tokensOwed1
             if (amount1Requested > position.tokensOwed1)
             else amount1Requested
         )
 
+        tokens = self.factory.token_from_exchange[self.name]
+        assert tokens.get(self.token0) and tokens.get(self.token1), 'UniswapV3: TOKEN_UNAVAILABLE' 
+        
         if amount0 > 0:
             position.tokensOwed0 -= amount0
+            tokens.get(self.token0).deposit(recipient, amount0)
             #self.ledger.transferToken(self, recipient, self.token0, amount0)
         if amount1 > 0:
             position.tokensOwed1 -= amount1
+            tokens.get(self.token1).deposit(recipient, amount1) 
             #self.ledger.transferToken(self, recipient, self.token1, amount1)
   
         amount0 = self.convert(amount0)
         amount1 = self.convert(amount1)        
 
         return (recipient, tickLower, tickUpper, amount0, amount1)   
         
@@ -334,32 +321,32 @@
             Burn liquidity from the sender and account tokens owed for the liquidity to the position. Can 
             be used to trigger a recalculation of fees owed to a position by calling with an amount of 0. 
             Fees must be collected separately via a call to collect
                 
             Parameters
             -----------------    
             recipient : str
-                address for which the liquidity will be created      
+                Address for which the liquidity will be created      
             tickLower : int
-                lower tick of the position in which to add liquidity  
+                Lower tick of the position in which to add liquidity  
             tickUpper : int
-                lower tick of the position in which to add liquidity                 
+                Lower tick of the position in which to add liquidity                 
             amount : int
-                how much liquidity to burn
+                How much liquidity to burn
                 
             Returns
             -------
             recipient : str
-                address for which the liquidity will be created 
+                Address for which the liquidity will be created 
             amount0 : int
-                delta of the balance of token0 of the pool, exact when negative, minimum when positive
+                Delta of the balance of token0 of the pool, exact when negative, minimum when positive
             amount1 : int
-                delta of the balance of token1 of the pool, exact when negative, minimum when positive               
+                Delta of the balance of token1 of the pool, exact when negative, minimum when positive               
             amount : int
-                how much liquidity to burn                  
+                How much liquidity to burn                  
         """  
         
         amount = amount if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount)
         
         checkInputTypes(
             accounts=(recipient), int24=(tickLower, tickUpper), uint128=(amount)
         )
@@ -403,29 +390,29 @@
         """ swapExact0For1
 
             Swap exact value of token0 for token1
                 
             Parameters
             -----------------    
             recipient : str
-                address for which the liquidity will be created      
+                Address for which the liquidity will be created      
             amount : int
-                how much token to swap
+                How much token to swap
             sqrtPriceLimit : int
-                used to determine the highest price in the swap, and needs to be set when swapping on 
+                Used to determine the highest price in the swap, and needs to be set when swapping on 
                 the pool directly.       
                 
             Returns
             -------
             recipient : str
-                address for which the liquidity will be created 
+                Address for which the liquidity will be created 
             amount0 : int
-                delta of the balance of token0 of the pool, exact when negative, minimum when positive
+                Delta of the balance of token0 of the pool, exact when negative, minimum when positive
             amount1 : int
-                delta of the balance of token1 of the pool, exact when negative, minimum when positive                             
+                Delta of the balance of token1 of the pool, exact when negative, minimum when positive                             
         """         
 
         amount = amount if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount)
         sqrtPriceLimitX96 = (
             sqrtPriceLimit
             if sqrtPriceLimit != None
             else UniV3Utils.getSqrtPriceLimitX96('Token0')
@@ -438,29 +425,29 @@
         """ swapExact0For1
 
             Swap token0 for exact value of token1
                 
             Parameters
             -----------------    
             recipient : str
-                address for which the liquidity will be created      
+                Address for which the liquidity will be created      
             amount : int
-                how much token to swap
+                How much token to swap
             sqrtPriceLimit : int
-                used to determine the highest price in the swap, and needs to be set when swapping 
+                Used to determine the highest price in the swap, and needs to be set when swapping 
                 on the pool directly.       
                 
             Returns
             -------
             recipient : str
-                address for which the liquidity will be created 
+                Address for which the liquidity will be created 
             amount0 : int
-                delta of the balance of token0 of the pool, exact when negative, minimum when positive
+                Delta of the balance of token0 of the pool, exact when negative, minimum when positive
             amount1 : int
-                delta of the balance of token1 of the pool, exact when negative, minimum when positive                             
+                Delta of the balance of token1 of the pool, exact when negative, minimum when positive                             
         """           
         
         amount = amount if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount)
         sqrtPriceLimitX96 = (
             sqrtPriceLimit
             if sqrtPriceLimit != None
             else UniV3Utils.getSqrtPriceLimitX96(UniV3Utils.TEST_TOKENS[0])
@@ -473,29 +460,29 @@
         """ swapExact0For1
 
             Swap exact value of token1 for token0
                 
             Parameters
             -----------------    
             recipient : str
-                address for which the liquidity will be created      
+                Address for which the liquidity will be created      
             amount : int
-                how much token to swap
+                How much token to swap
             sqrtPriceLimit : int
-                used to determine the highest price in the swap, and needs to be set when swapping 
+                Used to determine the highest price in the swap, and needs to be set when swapping 
                 on the pool directly.       
                 
             Returns
             -------
             recipient : str
-                address for which the liquidity will be created 
+                Address for which the liquidity will be created 
             amount0 : int
-                delta of the balance of token0 of the pool, exact when negative, minimum when positive
+                Delta of the balance of token0 of the pool, exact when negative, minimum when positive
             amount1 : int
-                delta of the balance of token1 of the pool, exact when negative, minimum when positive                             
+                Delta of the balance of token1 of the pool, exact when negative, minimum when positive                             
         """          
         
         amount = amount if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount)
         sqrtPriceLimitX96 = (
             sqrtPriceLimit
             if sqrtPriceLimit != None
             else UniV3Utils.getSqrtPriceLimitX96(UniV3Utils.TEST_TOKENS[1])
@@ -507,29 +494,29 @@
         """ swapExact0For1
 
             Swap token1 for exact value of token0
                 
             Parameters
             -----------------    
             recipient : str
-                address for which the liquidity will be created      
+                Address for which the liquidity will be created      
             amount : int
-                how much token to swap
+                How much token to swap
             sqrtPriceLimit : int
-                used to determine the highest price in the swap, and needs to be set when swapping 
+                Used to determine the highest price in the swap, and needs to be set when swapping 
                 on the pool directly.       
                 
             Returns
             -------
             recipient : str
-                address for which the liquidity will be created 
+                Address for which the liquidity will be created 
             amount0 : int
-                delta of the balance of token0 of the pool, exact when negative, minimum when positive
+                Delta of the balance of token0 of the pool, exact when negative, minimum when positive
             amount1 : int
-                delta of the balance of token1 of the pool, exact when negative, minimum when positive                             
+                Delta of the balance of token1 of the pool, exact when negative, minimum when positive                             
         """         
 
         amount = amount if self.precision == UniswapExchangeData.TYPE_GWEI else self.dec2gwei(amount)
         sqrtPriceLimitX96 = (
             sqrtPriceLimit
             if sqrtPriceLimit != None
             else UniV3Utils.getSqrtPriceLimitX96(UniV3Utils.TEST_TOKENS[1])
@@ -542,33 +529,33 @@
 
             Swap token0 for token1, or token1 for token0. The tokens are automatically transferred 
             at the end of the swapping function.
                 
             Parameters
             -----------------    
             recipient : str
-                address for which the liquidity will be created      
+                Address for which the liquidity will be created      
             zeroForOne : int
                 the direction of the swap, true for token0 to token1, false for token1 to token0 
             amountSpecified : int
-                the amount of the swap, which implicitly configures the swap as exact input 
+                The amount of the swap, which implicitly configures the swap as exact input 
                 (positive), or exact output (negative)        
             sqrtPriceLimitX96 : int
-                the Q64.96 sqrt price limit. If zero for one, the price cannot be less than this 
+                The Q64.96 sqrt price limit. If zero for one, the price cannot be less than this 
                 value after the swap. If one for zero, the price cannot be greater than this 
                 value after the swap
                 
             Returns
             -------
             recipient : str
-                address for which the liquidity will be created 
+                Address for which the liquidity will be created 
             amount0 : int
-                delta of the balance of token0 of the pool, exact when negative, minimum when positive
+                Delta of the balance of token0 of the pool, exact when negative, minimum when positive
             amount1 : int
-                delta of the balance of token1 of the pool, exact when negative, minimum when positive                             
+                Delta of the balance of token1 of the pool, exact when negative, minimum when positive                             
         """ 
         
         checkInputTypes(
             accounts=(recipient),
             bool=(zeroForOne),
             int256=(amountSpecified),
             uint160=(sqrtPriceLimitX96),
@@ -761,17 +748,17 @@
         """ setFeeProtocol
 
             Set the denominator of the protocol's % share of the fees
             
             Parameters
             -----------------    
             feeProtocol0 : int
-                new protocol fee for token0 of the pool      
+                New protocol fee for token0 of the pool      
             feeProtocol1 : int
-                new protocol fee for token1 of the pool                        
+                New protocol fee for token1 of the pool                        
         """ 
         
         checkInputTypes(uint8=(feeProtocol0, feeProtocol1))
         assert (feeProtocol0 == 0 or (feeProtocol0 >= 4 and feeProtocol0 <= 10)) and (
             feeProtocol1 == 0 or (feeProtocol1 >= 4 and feeProtocol1 <= 10)
         )
 
@@ -787,17 +774,17 @@
         """ checkTicks
 
             Common checks for valid tick inputs
             
             Parameters
             -----------------    
             tickLower : int
-                lower tick of the position in which to add liquidity  
+                Lower tick of the position in which to add liquidity  
             tickUpper : int
-                lower tick of the position in which to add liquidity                    
+                Lower tick of the position in which to add liquidity                    
         """ 
         
         checkInputTypes(int24=(tickLower, tickUpper))
         assert tickLower < tickUpper, "UniswapV3: TLU"
         assert tickLower >= TickMath.MIN_TICK, "UniswapV3: TLM"
         assert tickUpper <= TickMath.MAX_TICK, "UniswapV3: TUM"        
 
@@ -810,22 +797,22 @@
             (keys) have been initialized within the boundaries. However, if there is no initialized 
             tick to the left or right we will return the next boundary. Then we need to return the 
             initialized bool to indicate that we are at the boundary and it is not an initalized tick.
             
             Parameters
             -----------------    
             tick : int
-                the starting tick    
+                The starting tick    
             lte : int
-                whether to search for the next initialized tick to the left (less than or equal to the starting tick)
+                Whether to search for the next initialized tick to the left (less than or equal to the starting tick)
                 
             Returns
             -------
             nextTick : int
-                next tick with liquidity to be used in the swap function                      
+                Next tick with liquidity to be used in the swap function                      
         """ 
         
         checkInputTypes(int24=(tick), bool=(lte))
 
         keyList = list(self.ticks.keys())
 
         # If tick doesn't exist in the mapping we fake it (easier than searching for nearest value). This is probably not the
@@ -853,29 +840,76 @@
 
         # Return tick within the boundaries
         return nextTick, True  
 
     def get_price(self, token): 
         pass
             
-    def get_reserve(self, token): 
-        pass 
+    def get_liquidity(self):  
+        
+        """ get_liquidity
+
+            Get liquidity of exchange pool         
+        """          
+
+        return self.gwei2dec(self.total_supply)        
+            
+    def get_reserve(self, token):  
+        
+        """ get_reserve
+
+            Get reserve amount of select token in the exchange pair
+                
+            Parameters
+            -----------------
+            token : ERC20
+                ERC20 token                
+        """         
+        
+        if(token.token_name == self.token0):
+            return self.gwei2dec(self.reserve0) 
+        elif(token.token_name == self.token1):
+            return self.gwei2dec(self.reserve1)
+        else:
+            assert False, 'UniswapV2: WRONG_INPUT_TOKEN'      
+
+    def get_virtual_reserve(self, token):  
+        
+        """ get_virtual_reserve
+
+            Get virtual reserve amount of select token in the exchange pair
+                
+            Parameters
+            -----------------
+            token : ERC20
+                ERC20 token                
+        """         
+        
+        sqrt_P = self.slot0.sqrtPriceX96/2**96
+        liq = self.get_liquidity()
+        
+        if(token.token_name == self.token0):
+            return liq/sqrt_P
+        elif(token.token_name == self.token1):
+            return liq*sqrt_P
+        else:
+            assert False, 'UniswapV2: WRONG_INPUT_TOKEN'           
 
     def convert(self, val): 
         val = val if self.precision == UniswapExchangeData.TYPE_GWEI else self.gwei2dec(val)
         return val
     
 
     def dec2gwei(self, tkn_amt, precision=None):
         precision = GWEI_PRECISION if precision == None else precision
         return int(Decimal(str(tkn_amt))*Decimal(str(10**precision)))
     
-    def gwei2dec(self, dec_amt, precision=None):   
+    def gwei2dec(self, tkn_amt, precision=None):   
         precision = GWEI_PRECISION if precision == None else precision
-        return float(Decimal(str(dec_amt))/Decimal(str(10**precision)))  
+        return float(Decimal(str(tkn_amt))/Decimal(str(10**precision)))  
     
 
     def _swap(self, inputToken, amounts, recipient, sqrtPriceLimitX96):
         [amountIn, amountOut] = amounts
         exactInput = amountOut == 0
         amount = amountIn if exactInput else amountOut
 
@@ -899,19 +933,19 @@
         """ _swap_tokens
 
             Remove liquidity from both coins in the pair based on lp amount
                 
             Parameters
             -----------------
             amountA_out : float
-                swap amountA out
+                Swap amountA out
             amountB_out : float
-                swap amountB out               
+                Swap amountB out               
             to_addr : str
-               receiving user address                   
+                Receiving user address                   
         """         
         
         assert amountA_out > 0 or amountB_out > 0, 'UniswapV3: INSUFFICIENT_OUTPUT_AMOUNT'
         assert amountA_out < self.reserve0 and amountB_out < self.reserve1, 'UniswapV3: INSUFFICIENT_LIQUIDITY'
 
         tokens = self.factory.token_from_exchange[self.name]
         assert tokens.get(self.token0).token_addr != to_addr, 'UniswapV3: INVALID_TO_ADDRESS'
@@ -937,17 +971,17 @@
         """ _update
 
             Update reserve amounts for both coins in the pair
                 
             Parameters
             -----------------   
             balanceA : float
-                new reserve amount of A      
+                New reserve amount of A      
             balance1 : float
-                new reserve amount of B                   
+                New reserve amount of B                   
         """         
         
         self.reserve0 = balanceA
         self.reserve1 = balanceB    
     
     def _modifyPosition(self, params):
```

### Comparing `UniswapPy-1.3.0/python/prod/cpt/factory/UniswapFactory.py` & `uniswappy-1.4.0/python/prod/cpt/factory/UniswapFactory.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 class UniswapFactory(IExchangeFactory):
 
     """ 
         Create Uniswap liquidity pools for given token pairs
         
         Parameters
         -----------------
-        self.name : str
+        name : str
             Token name 
-        self.address : str
+        address : str
             Token 0 name  
-        self.exchange_from_token : dictionary
+        exchange_from_token : dictionary
             Map of tokens to exchanges
-        self.tokens_from_exchange : dictionary
+        tokens_from_exchange : dictionary
             Map of exchanges to pair tokens          
     """     
     
     def __init__(self, name: str, address: str) -> None:
         self.name = name
         self.address = address
         self.exchange_from_token = {}
```

### Comparing `UniswapPy-1.3.0/python/prod/cpt/index/SettlementLPToken.py` & `uniswappy-1.4.0/python/prod/cpt/index/SettlementLPToken.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright [2023] [Ian Moore]
 # Distributed under the MIT License (license terms are at http://opensource.org/licenses/MIT).
 # Email: defipy.devs@gmail.com
 
-import math
+import numpy as np
+from ...utils.data import UniswapExchangeData
 
 class SettlementLPToken():
     
     """ Determine settlement amount of LP token given a certain amount of token    
     """  
     
     def __init__(self):
@@ -34,29 +35,41 @@
                    
         """          
         
         return self.calc_lp_settlement(lp, tkn, itkn_amt)
     
     def calc_lp_settlement(self, lp, token_in, itkn_amt):
 
-        if(token_in.token_name == lp.token1):
-            x = lp.reserve0
-            y = lp.reserve1
-        else: 
-            x = lp.reserve1
-            y = lp.reserve0
-
-        L = lp.total_supply
+        (x, y) = self.get_reserves(lp, token_in)
+        L = lp.get_liquidity()
         if(L == 0): 
             return 0
         else:
             gamma = 997
 
             a1 = x*y/L
             a2 = L
             a = a1/a2
             b = (1000*itkn_amt*x - itkn_amt*gamma*x + 1000*x*y + x*y*gamma)/(1000*L);
             c = itkn_amt*x;
 
-            dL = (b*a2 - a2*math.sqrt(b*b - 4*a1*c/a2)) / (2*a1);
-            return dL      
+            dL = (b*a2 - a2*np.sqrt(b*b - 4*a1*c/a2)) / (2*a1);
+            return dL  
+
+    def get_reserves(self, lp, token_in):
+        tokens = lp.factory.token_from_exchange[lp.name]
+        if(lp.version == UniswapExchangeData.VERSION_V2):
+            if(token_in.token_name == lp.token1):
+                x = lp.get_reserve(tokens[lp.token0])
+                y = lp.get_reserve(tokens[lp.token1])
+            else: 
+                x = lp.get_reserve(tokens[lp.token1])
+                y = lp.get_reserve(tokens[lp.token0])
+        elif(lp.version == UniswapExchangeData.VERSION_V3):   
+            if(token_in.token_name == lp.token1):
+                x = lp.get_virtual_reserve(tokens[lp.token0])
+                y = lp.get_virtual_reserve(tokens[lp.token1])
+            else: 
+                x = lp.get_virtual_reserve(tokens[lp.token1])
+                y = lp.get_virtual_reserve(tokens[lp.token0]) 
+        return (x, y)
```

### Comparing `UniswapPy-1.3.0/python/prod/cpt/quote/IndexTokenQuote.py` & `uniswappy-1.4.0/python/prod/cpt/quote/IndexTokenQuote.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class IndexTokenQuote():
     
     """ 
         Index token quotes
         
         Parameters
         -----------------
-        self.quote_native_tokens : boolean
+        quote_native_tokens : boolean
             Quote LP amount of base pool, otherwise quote indexed pool      
     """        
     
     def __init__(self, quote_native_tokens = True):
         self.quote_native_tokens = quote_native_tokens    
 
     def get_x(self, lp, amt_lp):
```

### Comparing `UniswapPy-1.3.0/python/prod/cpt/quote/LPQuote.py` & `uniswappy-1.4.0/python/prod/cpt/quote/LPQuote.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # Copyright [2023] [Ian Moore]
 # Distributed under the MIT License (license terms are at http://opensource.org/licenses/MIT).
 # Email: defipy.devs@gmail.com
 
 from ..index import RebaseIndexToken
 from ..index import SettlementLPToken
-import math
 
 class LPQuote():
     
     """ 
         Liquidity pool token quotes (ie, price, reserve and liquidity)
         
         Parameters
         -----------------
-        self.quote_opposing : boolean
+        quote_opposing : boolean
             Quote the opposing token amount by default, given LP and a token    
     """      
     
     def __init__(self, quote_opposing = True):
         self.quote_opposing = quote_opposing
         
     def get_opposing_token(self, lp, tkn):
```

### Comparing `UniswapPy-1.3.0/python/prod/cpt/quote/LPTokenQuote.py` & `uniswappy-1.4.0/python/prod/cpt/quote/LPTokenQuote.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/cpt/quote/TreeAmountQuote.py` & `uniswappy-1.4.0/python/prod/cpt/quote/TreeAmountQuote.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/cpt/vault/IndexVault.py` & `uniswappy-1.4.0/python/prod/cpt/vault/IndexVault.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 
 class IndexVault(Vault):
     
     """ Vault of index tokens
 
         Parameters
         ----------
-        self.token_name : str
+        token_name : str
             Token name 
-        self.token_addr : str
+        token_addr : str
             Token address  
-        self.lp_providers : dictionary
+        lp_providers : dictionary
             Map of LP providers to their respective holdings
-        self.lp_tokens : dictionary
+        lp_tokens : dictionary
             Map of LPs to their ERC20 tokens and total amounts
-        self.index_tokens : dictionary
+        index_tokens : dictionary
             Map of index tokens to their ERC20 tokens and total amounts            
     """  
     
     
     def __init__(self, name: str, addr: str) -> None:
         self.token_name = name
         self.token_addr = addr
```

### Comparing `UniswapPy-1.3.0/python/prod/cpt/vault/Vault.py` & `uniswappy-1.4.0/python/prod/cpt/vault/Vault.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/cpt/wallet/Wallets.py` & `uniswappy-1.4.0/python/prod/cpt/wallet/Wallets.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/erc/DOAERC20.py` & `uniswappy-1.4.0/python/prod/erc/DOAERC20.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 class DOAERC20(ERC20):
     
     """ DAOSYS ERC20 token
 
         Parameters
         ----------
-        self.token_name : str
+        token_name : str
             Token name 
-        self.token_addr : str
+        token_addr : str
             Token address  
-        self.token_total : float
+        token_total : float
             Token holdings 
-        self.type : float
+        type : float
             Token type 
     """      
 
     def __init__(self, name: str, addr: str) -> None:
         self.token_name = name+'-LP'
         self.token_addr = addr
         self.token_supply = 1_000_000_000
```

### Comparing `UniswapPy-1.3.0/python/prod/erc/ERC20.py` & `uniswappy-1.4.0/python/prod/erc/ERC20.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 class ERC20:
     
     """ ERC20 token
 
         Parameters
         -----------------
-        self.token_name : str
+        token_name : str
             Token name 
-        self.token_addr : str
+        token_addr : str
             Token address  
-        self.token_total : float
+        token_total : float
             Token holdings 
     """   
     
     def __init__(self, name: str, addr: str, decimal: int = None):
         self.token_name = name
         self.token_addr = addr
         self.token_total = 0
```

### Comparing `UniswapPy-1.3.0/python/prod/erc/IndexERC20.py` & `uniswappy-1.4.0/python/prod/erc/IndexERC20.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 class IndexERC20(ERC20):
     
     """ Index ERC20 token
 
         Parameters
         ----------
-        self.token_name : str
+        token_name : str
             Token name 
-        self.token_addr : str
+        token_addr : str
             Token address  
-        self.token_total : float
+        token_total : float
             Token holdings 
     """  
 
     def __init__(self, name, addr, parent_tkn, parent_lp):
         self.token_name = name
         self.token_addr = addr
         self.parent_lp = parent_lp
```

### Comparing `UniswapPy-1.3.0/python/prod/erc/LPERC20.py` & `uniswappy-1.4.0/python/prod/erc/LPERC20.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 class LPERC20(ERC20):
     
     """ DAOSYS ERC20 token
 
         Parameters
         -----------------
-        self.token_name : str
+        token_name : str
             Token name 
-        self.token_addr : str
+        token_addr : str
             Token address  
-        self.token_total : float
+        token_total : float
             Token holdings 
-        self.type : float
+        type : float
             Token type 
     """      
 
     def __init__(self, name: str, addr: str) -> None:
         self.token_name = name+'-LP'
         self.token_addr = addr
         self.token_supply = 1_000_000_000
```

### Comparing `UniswapPy-1.3.0/python/prod/math/interest/Yield.py` & `uniswappy-1.4.0/python/prod/math/interest/Yield.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/math/interest/ips/ConstantIPS.py` & `uniswappy-1.4.0/python/prod/math/interest/ips/ConstantIPS.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/math/model/BrownianModel.py` & `uniswappy-1.4.0/python/prod/math/model/BrownianModel.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/math/model/ModelQueue.py` & `uniswappy-1.4.0/python/prod/math/model/ModelQueue.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/math/model/TimeDeltaModel.py` & `uniswappy-1.4.0/python/prod/math/model/TimeDeltaModel.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/math/model/TokenDeltaModel.py` & `uniswappy-1.4.0/python/prod/math/model/TokenDeltaModel.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/math/risk/MaxDrop.py` & `uniswappy-1.4.0/python/prod/math/risk/MaxDrop.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         
         """ get_pnt1
 
             Get end point (x,y) of max percentage drop
 
             Returns
             -------
-            self.__pnt1 : tuple
+            __pnt1 : tuple
                 End point (x, y)            
         """         
         
         return self.__pnt2      
         
     def n_diff(self, arr, N):
```

### Comparing `UniswapPy-1.3.0/python/prod/process/burn/IndexTokenBurn.py` & `uniswappy-1.4.0/python/prod/process/burn/IndexTokenBurn.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class IndexTokenBurn(Process):
 
     """ Index token burn process
 
         Parameters
         ----------
-        self.ivault : IndexVault
+        ivault : IndexVault
             Index vault
     """       
     
     def __init__(self, ivault):
         self.ivault = IndexVault('iVault', "0x7") if ivault  == None else ivault
             
     def apply(self, lp_tkn, token, user_nm, lp_burn_amt):
```

### Comparing `UniswapPy-1.3.0/python/prod/process/deposit/SwapDeposit.py` & `uniswappy-1.4.0/python/prod/process/deposit/SwapDeposit.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,35 +3,36 @@
 # Email: defipy.devs@gmail.com
 
 from ..Process import Process
 from ..liquidity import AddLiquidity
 from ..swap import Swap
 from ...math.model import TokenDeltaModel
 from ...math.model import EventSelectionModel
+from ...utils.data import UniswapExchangeData
 import math
 
 
 class SwapDeposit(Process):
     
     """ Process to swap approx. half of single token X for token Y (and vice verse) and deposit proceeds
         plus remaining other approximated half
 
         Parameters
         ----------
-        self.ev : EventSelectionModel
+        ev : EventSelectionModel
             EventSelectionModel object to randomly generate buy vs sell events
-        self.tDel : TokenDeltaModel
+        tDel : TokenDeltaModel
             TokenDeltaModel to randomly generate token amounts        
     """       
 
     def __init__(self, ev = None, tDel = None):
         self.ev = EventSelectionModel() if ev  == None else ev
         self.tDel = TokenDeltaModel(50) if tDel == None else tDel
             
-    def apply(self, lp, token_in, user_nm, amount_in):   
+    def apply(self, lp, token_in, user_nm, amount_in, lwr_tick = None, upr_tick = None):   
         
         """ apply
 
             Swap approx. half of single token X for token Y (and vice verse) and deposit proceeds
             plus remaining other approximated half
                 
             Parameters
@@ -39,57 +40,64 @@
             lp : Exchange
                 LP exchange
             token_in : ERC20
                 specified ERC20 token               
             user_nm : str
                 account name
             amount_in : float
-               token amount to be swap 
+                token amount to be swap 
+            lwr_tick : int
+                lower tick of the position in which to add liquidity   
+            upr_tick : int
+                upper tick of the position in which to add liquidity   
                 
             Returns
             -------
             (amount_in, amount_out) : float, float
                 token swap amounts                
         """          
         
-        amount_in = tDel.delta() if amount_in == None else amount_in
-        
-        # Step 1: swap
-        p_in = self.calc_deposit_portion(lp, token_in, amount_in)
+        amount_in = tDel.delta() if amount_in == None else amount_in    
+
+        # Step 1: swap        
+        p_in = self._calc_deposit_portion(lp, token_in, amount_in)
         amount_out = Swap().apply(lp, token_in, user_nm, p_in*amount_in)
         trading_token = self.get_trading_token(lp, token_in)
-        
+
         # Step 2: deposit   
-        if(token_in.token_name == lp.token1):
-            balance0 = amount_out 
-            balance1 = lp.quote(balance0, lp.reserve0, lp.reserve1)
-            deposited = balance1 + p_in*amount_in
-        elif(token_in.token_name == lp.token0):
-            balance1 = amount_out
-            balance0 = lp.quote(balance1, lp.reserve1, lp.reserve0) 
-            deposited = balance0 + p_in*amount_in
-        lp.add_liquidity(user_nm, balance0, balance1, balance0, balance1) 
+        if(lp.version == UniswapExchangeData.VERSION_V2):
+            if(token_in.token_name == lp.token1):
+                balance0 = amount_out 
+                balance1 = lp.quote(balance0, lp.reserve0, lp.reserve1)
+                deposited = balance1 + p_in*amount_in
+            elif(token_in.token_name == lp.token0):
+                balance1 = amount_out
+                balance0 = lp.quote(balance1, lp.reserve1, lp.reserve0)
+                deposited = balance0 + p_in*amount_in
+            lp.add_liquidity(user_nm, balance0, balance1, balance0, balance1) 
+            
+        elif(lp.version == UniswapExchangeData.VERSION_V3):  
+            tot_liq = lp.get_liquidity()
+            sqrt_P = lp.slot0.sqrtPriceX96/2**96
+            tokens = lp.factory.token_from_exchange[lp.name] 
+
+            if(token_in.token_name == lp.token0):
+                balance1 = abs(amount_out[2]) 
+                liq = balance1/sqrt_P 
+                deposited = liq/sqrt_P + p_in*amount_in
+                                
+            elif(token_in.token_name == lp.token1): 
+                balance0 = abs(amount_out[1]) 
+                liq = balance0*sqrt_P 
+                deposited = liq*sqrt_P + p_in*amount_in
+                
+            lp.mint(user_nm, lwr_tick, upr_tick, liq)  
                             
         return deposited  
 
-    
-    def calc_deposit_portion(self, lp, token_in, dx):
-
-        if(token_in.token_name == lp.token0):
-            tkn_supply = lp.reserve0
-        else:    
-            tkn_supply = lp.reserve1
-
-        a = 997*(dx**2)/(1000*tkn_supply)
-        b = dx*(1997/1000)
-        c = -dx
-
-        alpha = -(b - math.sqrt(b*b - 4*a*c)) / (2*a)
-        return alpha 
-        
     def get_trading_token(self, lp, token):
         
         """ get_trading_token
 
             Get opposing token from specified token
                 
             Parameters
@@ -104,8 +112,34 @@
             trading_token : ERC20 
                 opposing ERC20 token                   
         """         
         
         tokens = lp.factory.token_from_exchange[lp.name]
         trading_token = tokens[lp.token1] if token.token_name == lp.token0 else tokens[lp.token0]
         return trading_token       
+            
+    
+    def _calc_deposit_portion(self, lp, token_in, dx):
+
+        tkn_supply = self._get_tkn_supply(lp, token_in)
+        a = 997*(dx**2)/(1000*tkn_supply)
+        b = dx*(1997/1000)
+        c = -dx
+
+        alpha = -(b - math.sqrt(b*b - 4*a*c)) / (2*a)
+        return alpha 
+
+    def _get_tkn_supply(self, lp, token_in):
+        tokens = lp.factory.token_from_exchange[lp.name]
+        if(lp.version == UniswapExchangeData.VERSION_V2):
+            if(token_in.token_name == lp.token0):
+                tkn_supply = lp.get_reserve(tokens[lp.token0])
+            else:    
+                tkn_supply = lp.get_reserve(tokens[lp.token1])
+        elif(lp.version == UniswapExchangeData.VERSION_V3):   
+            if(token_in.token_name == lp.token0):
+                tkn_supply = lp.get_virtual_reserve(tokens[lp.token0])
+            else:    
+                tkn_supply = lp.get_virtual_reserve(tokens[lp.token1])
+        return tkn_supply        
         
+
```

### Comparing `UniswapPy-1.3.0/python/prod/process/liquidity/AddLiquidity.py` & `uniswappy-1.4.0/python/prod/process/mint/SwapIndexMint.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,80 @@
 # Copyright [2023] [Ian Moore]
 # Distributed under the MIT License (license terms are at http://opensource.org/licenses/MIT).
 # Email: defipy.devs@gmail.com
 
 from ..Process import Process
+from ..deposit import SwapDeposit
 from ...math.model import TokenDeltaModel
 from ...math.model import EventSelectionModel
 
-class AddLiquidity(Process):
-     
-    """ Add liquidity process
+class SwapIndexMint(Process):
+    
+    """ Process to swap-deposit single token into LP and mint its respective indexing token
 
         Parameters
         ----------
-        self.ev : EventSelectionModel
-            EventSelectionModel object to randomly generate buy vs sell events
-        self.tDel : TokenDeltaModel
-            TokenDeltaModel to randomly generate token amounts        
+        ivault : IndexVault
+            Index vault     
+        opposing : boolean
+            Boolean variable to determine whether to mint token opposing the one that was deposited                
     """     
 
-    def __init__(self, init_price = None, ev = None, tDel = None):
-        self.ev = EventSelectionModel() if ev  == None else ev
-        self.tDel = TokenDeltaModel(50) if tDel == None else tDel
-        self.init_price = 1 if init_price == None else init_price
+    def __init__(self, ivault, opposing = None):
+        self.ivault = IndexVault('iVault', "0x7") if ivault  == None else ivault
+        self.opposing = False if opposing  == None else opposing
+        self.mint_amt = 0
             
-    def apply(self, lp, token_in, user_nm, amount_in):    
+    def apply(self, lp_tkn, token, user_nm, amt):    
         
         """ apply
 
-            Adds liquidity using only X or Y amounts
+            Swap-deposit single token into LP and mint its respective indexing token
                 
             Parameters
             -------
-            lp : Exchange
+            lp_tkn : Exchange
                 LP exchange
-            token_in : ERC20
+            token : ERC20
                 specified ERC20 token               
             user_nm : str
                 account name
-            amount_in : float
-               token amount to be add to liquidity 
+            amt : float
+               token amount to be swapped and minted 
                 
             Returns
             -------
             (amount_in, amount_out) : float, float
                 token swap amounts                
-        """          
+        """           
         
-        amount_in = tDel.delta() if amount_in == None else amount_in
-        if(token_in.token_name == lp.token0):
-            balance0 = amount_in         
-            if(lp.reserve1 > 0):
-                balance1 = lp.quote(amount_in, lp.reserve0, lp.reserve1)
-            else:
-                balance1 = self.init_price*balance0               
-            
-            lp.add_liquidity(user_nm, balance0, balance1, balance0, balance1)
-        elif(token_in.token_name == lp.token1):
-            balance1 = amount_in
-            if(lp.reserve0 > 0):
-                balance0 = lp.quote(amount_in, lp.reserve1, lp.reserve0)
-            else:
-                balance0 = self.init_price*balance1            
-            
-            lp.add_liquidity(user_nm, balance0, balance1, balance0, balance1) 
+        lp_amt0 = lp_tkn.liquidity_providers[user_nm]
+        out = SwapDeposit().apply(lp_tkn, token, user_nm, amt)
+        lp_amt1 = lp_tkn.liquidity_providers[user_nm]
+        lp_amt = lp_amt1 - lp_amt0
+        mint_token = token if not self.opposing else self.get_trading_token(lp_tkn, token)
+        self.ivault.deposit_lp_tkn(user_nm, lp_tkn, lp_amt)
+        self.ivault.rebase_index_tkn(lp_tkn, mint_token) 
+     
+    def get_trading_token(self, lp, token):
+        
+        """ get_trading_token
 
-        return {lp.token0:balance0, lp.token1:balance1}    
-    
- 
+            Get opposing token from specified token
+                
+            Parameters
+            -------
+            lp : Exchange
+                LP exchange
+            token : ERC20
+                specified ERC20 token      
+                
+            Returns
+            -------
+            trading_token : ERC20 
+                opposing ERC20 token                   
+        """           
+        
+        tokens = lp.factory.exchange_to_tokens[lp.name]
+        trading_token = tokens[lp.token1] if token.token_name == lp.token0 else tokens[lp.token0]
+        return trading_token
```

### Comparing `UniswapPy-1.3.0/python/prod/process/liquidity/RemoveLiquidity.py` & `uniswappy-1.4.0/python/prod/process/liquidity/RemoveLiquidity.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,88 @@
 # Copyright [2023] [Ian Moore]
 # Distributed under the MIT License (license terms are at http://opensource.org/licenses/MIT).
 # Email: defipy.devs@gmail.com
 
 from ..Process import Process
 from ...math.model import TokenDeltaModel
 from ...math.model import EventSelectionModel
+from ...utils.data import UniswapExchangeData
+
 
 class RemoveLiquidity(Process):
     
     """ Remove liquidity process
 
         Parameters
         ----------
-        self.ev : EventSelectionModel
+        ev : EventSelectionModel
             EventSelectionModel object to randomly generate buy vs sell events
-        self.tDel : TokenDeltaModel
+        tDel : TokenDeltaModel
             TokenDeltaModel to randomly generate token amounts        
     """       
 
     def __init__(self, ev = None, tDel = None):
         self.ev = EventSelectionModel() if ev  == None else ev
         self.tDel = TokenDeltaModel(50) if tDel == None else tDel
             
-    def apply(self, lp, token_in, user_nm, amount_in):    
+    def apply(self, lp, token_in, user_nm, amount_in, lwr_tick = None, upr_tick = None):    
         
         """ apply
 
             Removes liquidity using only X or Y amounts
                 
             Parameters
             -------
             lp : Exchange
                 LP exchange
             token_in : ERC20
                 specified ERC20 token               
             user_nm : str
                 account name
             amount_in : float
-               token amount to be add to liquidity 
+                token amount to be add to liquidity 
+            lwr_tick : int
+                lower tick of the position in which to add liquidity   
+            upr_tick : int
+                upper tick of the position in which to add liquidity                
                 
             Returns
             -------
             reserve amounts : dictionary
                 dictionary of reserve amounts                
         """          
         
         amount_in = self.tDel.delta() if amount_in == None else amount_in
-        if(token_in.token_name == lp.token0):
-            liq = amount_in*lp.total_supply/lp.reserve0
-            amount1 = liq*lp.reserve1/lp.total_supply
-            #liq = LPQuote().get_liquidity(lp, token_in, amount_in)
-            #amount1 = LPQuote().get_amount(lp, token_in, amount_in)
-            amount0, amount1 = lp.remove_liquidity(user_nm, liq, amount_in, amount1)
-        elif(token_in.token_name == lp.token1): 
-            liq = amount_in*lp.total_supply/lp.reserve1
-            amount0 = liq*lp.reserve0/lp.total_supply
-            #liq = LPQuote().get_liquidity(lp, token_in, amount_in)
-            #amount0 = LPQuote().get_amount(lp, token_in, amount_in)
-            amount0, amount1 = lp.remove_liquidity(user_nm, liq, amount0, amount_in)  
+        tokens = lp.factory.token_from_exchange[lp.name]  
+
+        if(lp.version == UniswapExchangeData.VERSION_V2):
 
+            res0 = lp.get_reserve(tokens[lp.token0])
+            res1 = lp.get_reserve(tokens[lp.token1])
+            tot_liq = lp.get_liquidity()
+            
+            if(token_in.token_name == lp.token0):
+                liq = amount_in*tot_liq/res0
+                amount1 = liq*res1/tot_liq
+                amount0, amount1 = lp.remove_liquidity(user_nm, liq, amount_in, amount1) 
+            elif(token_in.token_name == lp.token1): 
+                liq = amount_in*tot_liq/res1
+                amount0 = liq*res0/tot_liq
+                amount0, amount1 = lp.remove_liquidity(user_nm, liq, amount0, amount_in) 
+
+        elif(lp.version == UniswapExchangeData.VERSION_V3):  
+
+            tot_liq = lp.get_liquidity()
+            sqrt_P = lp.slot0.sqrtPriceX96/2**96
+
+            if(token_in.token_name == lp.token0):
+                liq = amount_in*sqrt_P
+                (_, _, _, _, amount0, amount1) = lp.burn(user_nm, lwr_tick, upr_tick, liq)
+            elif(token_in.token_name == lp.token1): 
+                liq = amount_in/sqrt_P
+                (_, _, _, _, amount0, amount1) = lp.burn(user_nm, lwr_tick, upr_tick, liq)        
+        
+            
         return {lp.token0:amount0, lp.token1:amount1}
```

### Comparing `UniswapPy-1.3.0/python/prod/process/swap/RandomSwap.py` & `uniswappy-1.4.0/python/prod/process/swap/RandomSwap.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 class RandomSwap(Process):
     
     """ Process to randomly swap token X for token Y (and vice verse) 
 
         Parameters
         ----------
-        self.ev : EventSelectionModel
+        ev : EventSelectionModel
             EventSelectionModel object to randomly generate buy vs sell events
-        self.tDel : TokenDeltaModel
+        tDel : TokenDeltaModel
             TokenDeltaModel to randomly generate token amounts                 
     """           
 
     def __init__(self, p = None, ev = None, tDel = None):
         self.ev = EventSelectionModel() if ev  == None else ev
         self.tDel = TokenDeltaModel(50) if tDel == None else tDel
         self.buy_sell_prob = 0.5 if p == None else p
```

### Comparing `UniswapPy-1.3.0/python/prod/process/swap/Swap.py` & `uniswappy-1.4.0/python/prod/process/join/Join.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,52 @@
-# Copyright [2023] [Ian Moore]
+# Copyright [2024] [Ian Moore]
 # Distributed under the MIT License (license terms are at http://opensource.org/licenses/MIT).
 # Email: defipy.devs@gmail.com
 
-from ..Process import Process
-from ...math.model import TokenDeltaModel
-from ...math.model import EventSelectionModel
+from ...utils.data import UniswapExchangeData
+from ...utils.tools.v3 import UniV3Utils
 import math
 
-class Swap(Process):
+class Join():
     
-    """ Process to swap token X for token Y (and vice verse) 
-
-        Parameters
-        ----------
-        self.ev : EventSelectionModel
-            EventSelectionModel object to randomly generate buy vs sell events
-        self.tDel : TokenDeltaModel
-            TokenDeltaModel to randomly generate token amounts                 
+    """ Process to join x and y amounts to pool              
     """       
 
-    def __init__(self, ev = None, tDel = None):
-        self.ev = EventSelectionModel() if ev  == None else ev
-        self.tDel = TokenDeltaModel(50) if tDel == None else tDel
-            
-    def apply(self, lp, token_in, user_nm, amount_in):    
-        
+    def __init__(self):
+        pass
+
+    def apply(self, lp, user_nm, amount0, amount1, lwr_tick = None, upr_tick = None):
         """ apply
 
-            Swap token X for token Y (and vice verse) 
+            Join x and y amounts to pool
                 
             Parameters
             -------
             lp : Exchange
-                LP exchange
-            token_in : ERC20
-                specified ERC20 token               
+                LP exchange            
             user_nm : str
                 account name
-            amount_in : float
-               token amount to be swap 
-                
+            amount0 : float
+               x token amount 
+            amount1 : float
+               y token amount       
+            lwr_tick : int
+               Lower tick of the position in which to add liquidity   
+            upr_tick : int
+               Upper tick of the position in which to add liquidity   
+                     
             Returns
             -------
-            amount_out_expected : float
-                exchanged token amount               
-        """          
-        
-        amount_in = tDel.delta() if amount_in == None else amount_in
-        amount_out = math.floor(lp.get_amount_out(amount_in, token_in))
-        amount_out_expected = lp.swap_exact_tokens_for_tokens(amount_in, amount_out, token_in, to_addr=user_nm)
-        return amount_out_expected        
-        
+            out : dictionary
+                join output               
+        """ 
+
+        if(lp.version == UniswapExchangeData.VERSION_V2):
+            out = lp.add_liquidity(user_nm, amount0, amount1, amount0, amount1)
+            
+        elif(lp.version == UniswapExchangeData.VERSION_V3):
+            k = math.sqrt(amount0*amount1)
+            init_liquidity = UniV3Utils.encodePriceSqrt(amount1, amount0)
+            lp.initialize(init_liquidity)
+            out = lp.mint(user_nm, lwr_tick, upr_tick, k)
+             
+        return out
```

### Comparing `UniswapPy-1.3.0/python/prod/process/swap/WithdrawSwap.py` & `uniswappy-1.4.0/python/prod/process/liquidity/AddLiquidity.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,128 +1,96 @@
 # Copyright [2023] [Ian Moore]
 # Distributed under the MIT License (license terms are at http://opensource.org/licenses/MIT).
 # Email: defipy.devs@gmail.com
 
 from ..Process import Process
-from .Swap import Swap
-from ..liquidity import RemoveLiquidity
 from ...math.model import TokenDeltaModel
 from ...math.model import EventSelectionModel
-import math
+from ...utils.data import UniswapExchangeData
 
-class WithdrawSwap(Process):
-    
-    """ Process to withdraw liquidity from LP and swap opposing token which is added to specifed token to receive         
-        a single amount of specified token
+class AddLiquidity(Process):
+     
+    """ Add liquidity process
 
         Parameters
         ----------
-        self.ev : EventSelectionModel
+        ev : EventSelectionModel
             EventSelectionModel object to randomly generate buy vs sell events
-        self.tDel : TokenDeltaModel
+        tDel : TokenDeltaModel
             TokenDeltaModel to randomly generate token amounts        
-    """       
+    """     
 
-    def __init__(self, ev = None, tDel = None):
+    def __init__(self, init_price = None, ev = None, tDel = None):
         self.ev = EventSelectionModel() if ev  == None else ev
         self.tDel = TokenDeltaModel(50) if tDel == None else tDel
+        self.init_price = 1 if init_price == None else init_price
             
-    def apply(self, lp, token_out, user_nm, amount_out):    
+    def apply(self, lp, token_in, user_nm, amount_in, lwr_tick = None, upr_tick = None):    
         
         """ apply
 
-            Withdraw liquidity from LP and swap opposing token which is added to specifed token to receive                 
-            a single amount of specified token
+            Adds liquidity using only X or Y amounts
                 
             Parameters
             -------
             lp : Exchange
                 LP exchange
-            token_out : ERC20
+            token_in : ERC20
                 specified ERC20 token               
             user_nm : str
                 account name
-            amount_out : float
-               token amount to be swap 
+            amount_in : float
+                token amount to be add to liquidity 
+            lwr_tick : int
+                lower tick of the position in which to add liquidity   
+            upr_tick : int
+                upper tick of the position in which to add liquidity                  
                 
             Returns
             -------
-            amount_out : float
-                amount of withdrawn token               
+            (amount_in, amount_out) : float, float
+                token swap amounts                
         """          
         
-        amount_out = tDel.delta() if amount_out == None else amount_out
-    
-        # Step 1: withdrawal
-        p_out = self.calc_withdraw_portion(lp, token_out, amount_out)
-        removeLiq = RemoveLiquidity()
-        res = removeLiq.apply(lp, token_out, user_nm, p_out*amount_out)
-
-        # Step 2: swap
-        trading_token = self.get_trading_token(lp, token_out)
-        out = Swap().apply(lp, trading_token, user_nm, res[trading_token.token_name])  
-        withdrawn = out + p_out*amount_out 
-        return withdrawn 
- 
-    def calc_lp_settlement(self, lp, token_in, itkn_amt):
+        amount_in = tDel.delta() if amount_in == None else amount_in
+        tokens = lp.factory.token_from_exchange[lp.name]  
 
-        if(token_in.token_name == lp.token1):
-            x = lp.reserve0
-            y = lp.reserve1
-        else: 
-            x = lp.reserve1
-            y = lp.reserve0
-
-        L = lp.total_supply
-        gamma = 997
-
-        a1 = x*y/L
-        a2 = L
-        a = a1/a2
-        b = (1000*itkn_amt*x - itkn_amt*gamma*x + 1000*x*y + x*y*gamma)/(1000*L);
-        c = itkn_amt*x;
-
-        dL = (b*a2 - a2*math.sqrt(b*b - 4*a1*c/a2)) / (2*a1);
-        return dL
-
-    def calc_withdraw_portion(self, lp, token_in, amt):
-
-        if(token_in.token_name == lp.token1):
-            x = lp.reserve0
-            y = lp.reserve1
-        else: 
-            x = lp.reserve1
-            y = lp.reserve0
-
-        L = lp.total_supply
-        gamma = 997/1000
-
-        dL = self.calc_lp_settlement(lp, token_in, amt) 
-        dx = dL*x/L
-        dy = dL*y/L
-        aswap = (gamma*dx)*(y-dy)/(x-dx+gamma*dx)
-
-        return dy/amt      
-
-    def get_trading_token(self, lp, token):
-        
-        """ get_trading_token
+        if(lp.version == UniswapExchangeData.VERSION_V2):
 
-            Get opposing token from specified token
+            res0 = lp.get_reserve(tokens[lp.token0])
+            res1 = lp.get_reserve(tokens[lp.token1])
+            tot_liq = lp.get_liquidity()
+            
+            if(token_in.token_name == lp.token0):
+                balance0 = amount_in         
+                if(res1 > 0):
+                    balance1 = lp.quote(amount_in, res0, res1)
+                else:
+                    balance1 = self.init_price*balance0  
+                    
+                lp.add_liquidity(user_nm, balance0, balance1, balance0, balance1)
                 
-            Parameters
-            -------
-            lp : Exchange
-                LP exchange
-            token : ERC20
-                specified ERC20 token      
+            elif(token_in.token_name == lp.token1):
+                balance1 = amount_in
+                if(res0 > 0):
+                    balance0 = lp.quote(amount_in, res1, res0)
+                else:
+                    balance0 = self.init_price*balance1            
                 
-            Returns
-            -------
-            trading_token : ERC20 
-                opposing ERC20 token                   
-        """          
-        
-        tokens = lp.factory.token_from_exchange[lp.name]
-        trading_token = tokens[lp.token1] if token.token_name == lp.token0 else tokens[lp.token0]
-        return trading_token        
+                lp.add_liquidity(user_nm, balance0, balance1, balance0, balance1) 
+
+        elif(lp.version == UniswapExchangeData.VERSION_V3): 
+
+            tot_liq = lp.get_liquidity()
+            sqrt_P = lp.slot0.sqrtPriceX96/2**96
+
+            if(token_in.token_name == lp.token0):
+                liq = amount_in*sqrt_P
+                (balance0, balance1)  = lp.mint(user_nm, lwr_tick, upr_tick, liq)
+            elif(token_in.token_name == lp.token1): 
+                liq = amount_in/sqrt_P
+                (balance0, balance1) = lp.mint(user_nm, lwr_tick, upr_tick, liq)  
+
+        return {lp.token0:balance0, lp.token1:balance1}    
+    
+
```

### Comparing `UniswapPy-1.3.0/python/prod/simulate/Arbitrage.py` & `uniswappy-1.4.0/python/prod/simulate/Arbitrage.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/simulate/CorrectReserves.py` & `uniswappy-1.4.0/python/prod/simulate/CorrectReserves.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/simulate/MarkovState.py` & `uniswappy-1.4.0/python/prod/simulate/MarkovState.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/simulate/QuantTerminal.py` & `uniswappy-1.4.0/python/prod/simulate/QuantTerminal.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/simulate/SimpleLPSimulation.py` & `uniswappy-1.4.0/python/prod/simulate/SimpleLPSimulation.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/simulate/SolveDeltas.py` & `uniswappy-1.4.0/python/prod/simulate/SolveDeltas.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/utils/client/API0x.py` & `uniswappy-1.4.0/python/prod/utils/client/API0x.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/utils/data/Chain0x.py` & `uniswappy-1.4.0/python/prod/utils/data/Chain0x.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/utils/data/UniswapExchangeData.py` & `uniswappy-1.4.0/python/prod/utils/data/UniswapExchangeData.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/utils/tools/v3/FullMath.py` & `uniswappy-1.4.0/python/prod/utils/tools/v3/FullMath.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/utils/tools/v3/LiquidityMath.py` & `uniswappy-1.4.0/python/prod/utils/tools/v3/LiquidityMath.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/utils/tools/v3/Position.py` & `uniswappy-1.4.0/python/prod/utils/tools/v3/Position.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/utils/tools/v3/SafeMath.py` & `uniswappy-1.4.0/python/prod/utils/tools/v3/SafeMath.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/utils/tools/v3/Shared.py` & `uniswappy-1.4.0/python/prod/utils/tools/v3/Shared.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/utils/tools/v3/SqrtPriceMath.py` & `uniswappy-1.4.0/python/prod/utils/tools/v3/SqrtPriceMath.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,14 +152,17 @@
 ### @dev Calculates liquidity / sqrt(lower) - liquidity / sqrt(upper),
 ### i.e. liquidity * (sqrt(upper) - sqrt(lower)) / (sqrt(upper) * sqrt(lower))
 ### @param sqrtRatioAX96 A sqrt price
 ### @param sqrtRatioBX96 Another sqrt price
 ### @param liquidity The amount of usable liquidity
 ### @return amount0 Amount of token0 required to cover a position of size liquidity between the two passed prices
 def getAmount0Delta(sqrtRatioAX96, sqrtRatioBX96, liquidity, roundUp):
+
+    #print('Delta X')
+    
     checkInputTypes(
         uint160=(sqrtRatioAX96, sqrtRatioBX96), uint128=liquidity, bool=roundUp
     )
     if sqrtRatioAX96 > sqrtRatioBX96:
         (sqrtRatioAX96, sqrtRatioBX96) = (sqrtRatioBX96, sqrtRatioAX96)
 
     numerator1 = liquidity << FixedPoint96_RESOLUTION
@@ -179,14 +182,17 @@
 ### @notice Gets the amount1 delta between two prices
 ### @dev Calculates liquidity * (sqrt(upper) - sqrt(lower))
 ### @param sqrtRatioAX96 A sqrt price
 ### @param sqrtRatioBX96 Another sqrt price
 ### @param liquidity The amount of usable liquidity
 ### @return amount1 Amount of token1 required to cover a position of size liquidity between the two passed prices
 def getAmount1Delta(sqrtRatioAX96, sqrtRatioBX96, liquidity, roundUp):
+
+    #print('Delta Y')
+    
     checkInputTypes(
         uint160=(sqrtRatioAX96, sqrtRatioBX96), uint128=liquidity, bool=roundUp
     )
     if sqrtRatioAX96 > sqrtRatioBX96:
         (sqrtRatioAX96, sqrtRatioBX96) = (sqrtRatioBX96, sqrtRatioAX96)
 
     if roundUp:
```

### Comparing `UniswapPy-1.3.0/python/prod/utils/tools/v3/SwapMath.py` & `uniswappy-1.4.0/python/prod/utils/tools/v3/SwapMath.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/utils/tools/v3/Tick.py` & `uniswappy-1.4.0/python/prod/utils/tools/v3/Tick.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/utils/tools/v3/TickMath.py` & `uniswappy-1.4.0/python/prod/utils/tools/v3/TickMath.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/python/prod/utils/tools/v3/UniV3Utils.py` & `uniswappy-1.4.0/python/prod/utils/tools/v3/UniV3Utils.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.3.0/setup.py` & `uniswappy-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='UniswapPy',
-      version='1.3.0',
+      version='1.4.0',
       description='Uniswap Analytics with Python',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/defipy-devs/uniswappy',
       author = "icmoore",
       author_email = "defipy.devs@gmail.com",
       license='MIT',
@@ -30,17 +30,19 @@
           'uniswappy.math.risk',
           'uniswappy.process',
           'uniswappy.process.burn',
           'uniswappy.process.deposit',
           'uniswappy.process.liquidity',
           'uniswappy.process.mint',
           'uniswappy.process.swap',
+          'uniswappy.process.join',
           'uniswappy.simulate',
           'uniswappy.utils.interfaces',
           'uniswappy.utils.data',
           'uniswappy.utils.client',
           'uniswappy.utils.tools.v3'
       ],
       install_requires=[
-          'scipy >= 1.7.3'         
+          'scipy >= 1.7.3',
+          'termcolor >= 2.4.0'
       ],
       zip_safe=False)
```

