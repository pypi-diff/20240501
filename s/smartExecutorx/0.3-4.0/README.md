# Comparing `tmp/smartExecutorx-0.3.tar.gz` & `tmp/smartExecutorx-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartExecutorx-0.3.tar", last modified: Fri Dec  1 20:24:22 2023, max compression
+gzip compressed data, was "smartExecutorx-4.0.tar", last modified: Wed May  1 11:53:41 2024, max compression
```

## Comparing `smartExecutorx-0.3.tar` & `smartExecutorx-4.0.tar`

### file list

```diff
@@ -1,261 +1,257 @@
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.323691 smartExecutorx-0.3/
--rw-rw-rw-   0        0        0     1112 2023-10-09 01:29:55.000000 smartExecutorx-0.3/LICENSE
--rw-rw-rw-   0        0        0      112 2023-10-09 05:58:34.000000 smartExecutorx-0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6003 2023-12-01 20:24:22.322691 smartExecutorx-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5183 2023-10-09 06:09:20.000000 smartExecutorx-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.074247 smartExecutorx-0.3/fdg/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/fdg/__init__.py
--rw-rw-rw-   0        0        0       21 2023-12-01 20:15:34.000000 smartExecutorx-0.3/fdg/__version__.py
--rw-rw-rw-   0        0        0     1251 2023-11-05 23:18:36.000000 smartExecutorx-0.3/fdg/constraint_check.py
--rw-rw-rw-   0        0        0      981 2023-10-09 01:29:55.000000 smartExecutorx-0.3/fdg/constraint_check_time.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.081416 smartExecutorx-0.3/fdg/control/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/fdg/control/__init__.py
--rw-rw-rw-   0        0        0    13317 2023-11-03 21:52:34.000000 smartExecutorx-0.3/fdg/control/ftn_search_strategy.py
--rw-rw-rw-   0        0        0    12289 2023-11-07 20:50:26.000000 smartExecutorx-0.3/fdg/control/function_assignment.py
--rw-rw-rw-   0        0        0     9741 2023-12-01 18:42:42.000000 smartExecutorx-0.3/fdg/control/guider.py
--rw-rw-rw-   0        0        0    52761 2023-12-01 18:42:42.000000 smartExecutorx-0.3/fdg/control/mine.py
--rw-rw-rw-   0        0        0     2219 2023-10-30 22:15:11.000000 smartExecutorx-0.3/fdg/control/weight_computation.py
--rw-rw-rw-   0        0        0     6635 2023-12-01 18:42:42.000000 smartExecutorx-0.3/fdg/expression_slot.py
--rw-rw-rw-   0        0        0    15860 2023-12-01 18:43:09.000000 smartExecutorx-0.3/fdg/fdg_pruner.py
--rw-rw-rw-   0        0        0     5622 2023-12-01 18:42:42.000000 smartExecutorx-0.3/fdg/function_coverage.py
--rw-rw-rw-   0        0        0    13515 2023-12-01 18:42:42.000000 smartExecutorx-0.3/fdg/fwrg_manager.py
--rw-rw-rw-   0        0        0     3113 2023-10-15 04:56:48.000000 smartExecutorx-0.3/fdg/global_config.py
--rw-rw-rw-   0        0        0    15937 2023-10-09 02:44:48.000000 smartExecutorx-0.3/fdg/instruction_modification.py
--rw-rw-rw-   0        0        0     9534 2023-11-05 22:48:36.000000 smartExecutorx-0.3/fdg/output_data.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.088563 smartExecutorx-0.3/fdg/preprocessing/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/fdg/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2028 2023-10-16 02:38:03.000000 smartExecutorx-0.3/fdg/preprocessing/address_collection.py
--rw-rw-rw-   0        0        0     4959 2023-10-09 01:29:55.000000 smartExecutorx-0.3/fdg/preprocessing/instruction_coverage.py
--rw-rw-rw-   0        0        0     4456 2023-11-02 02:56:40.000000 smartExecutorx-0.3/fdg/preprocessing/preprocess.py
--rw-rw-rw-   0        0        0     3064 2023-10-30 20:39:54.000000 smartExecutorx-0.3/fdg/preprocessing/read_in_conditions.py
--rw-rw-rw-   0        0        0     7734 2023-11-03 20:33:22.000000 smartExecutorx-0.3/fdg/preprocessing/slot_location.py
--rw-rw-rw-   0        0        0     4215 2023-11-01 01:55:38.000000 smartExecutorx-0.3/fdg/preprocessing/write_read_info.py
--rw-rw-rw-   0        0        0     4988 2023-10-25 02:39:36.000000 smartExecutorx-0.3/fdg/utils.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.089563 smartExecutorx-0.3/images/
--rw-rw-rw-   0        0        0   352017 2023-10-09 05:36:28.000000 smartExecutorx-0.3/images/exampleUsingDockerImage.png
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.092565 smartExecutorx-0.3/mythril/
--rw-rw-rw-   0        0        0      371 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/__init__.py
--rw-rw-rw-   0        0        0      145 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/__main__.py
--rw-rw-rw-   0        0        0      185 2023-10-09 03:49:50.000000 smartExecutorx-0.3/mythril/__version__.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.108127 smartExecutorx-0.3/mythril/analysis/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/analysis_args.py
--rw-rw-rw-   0        0        0     1847 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/call_helpers.py
--rw-rw-rw-   0        0        0     7045 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/callgraph.py
--rw-rw-rw-   0        0        0     1067 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/issue_annotation.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.115628 smartExecutorx-0.3/mythril/analysis/module/
--rw-rw-rw-   0        0        0      236 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/__init__.py
--rw-rw-rw-   0        0        0     4358 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/base.py
--rw-rw-rw-   0        0        0     4187 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/loader.py
--rw-rw-rw-   0        0        0      407 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/module_helpers.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.136202 smartExecutorx-0.3/mythril/analysis/module/modules/
--rw-rw-rw-   0        0        0        2 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/modules/__init__.py
--rw-rw-rw-   0        0        0     3738 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/modules/arbitrary_jump.py
--rw-rw-rw-   0        0        0     2594 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/modules/arbitrary_write.py
--rw-rw-rw-   0        0        0     3761 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/modules/delegatecall.py
--rw-rw-rw-   0        0        0     4068 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/modules/dependence_on_origin.py
--rw-rw-rw-   0        0        0     7652 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/modules/dependence_on_predictable_vars.py
--rw-rw-rw-   0        0        0     3601 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/modules/ether_thief.py
--rw-rw-rw-   0        0        0     5319 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/modules/exceptions.py
--rw-rw-rw-   0        0        0     4033 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/modules/external_calls.py
--rw-rw-rw-   0        0        0    11819 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/modules/integer.py
--rw-rw-rw-   0        0        0     4353 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/modules/multiple_sends.py
--rw-rw-rw-   0        0        0     7843 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/modules/state_change_external_calls.py
--rw-rw-rw-   0        0        0     4793 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/modules/suicide.py
--rw-rw-rw-   0        0        0     5791 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/modules/unchecked_retval.py
--rw-rw-rw-   0        0        0     4303 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/modules/user_assertions.py
--rw-rw-rw-   0        0        0     2006 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/module/util.py
--rw-rw-rw-   0        0        0     1915 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/ops.py
--rw-rw-rw-   0        0        0     4506 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/potential_issues.py
--rw-rw-rw-   0        0        0    12882 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/report.py
--rw-rw-rw-   0        0        0     1535 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/security.py
--rw-rw-rw-   0        0        0     9558 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/solver.py
--rw-rw-rw-   0        0        0     2452 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/swc_data.py
--rw-rw-rw-   0        0        0    12997 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/symbolic.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.140183 smartExecutorx-0.3/mythril/analysis/templates/
--rw-rw-rw-   0        0        0     2262 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/templates/callgraph.html
--rw-rw-rw-   0        0        0     2075 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/templates/report_as_markdown.jinja2
--rw-rw-rw-   0        0        0     1954 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/templates/report_as_text.jinja2
--rw-rw-rw-   0        0        0     4902 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/analysis/traceexplore.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.145184 smartExecutorx-0.3/mythril/concolic/
--rw-rw-rw-   0        0        0      128 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/concolic/__init__.py
--rw-rw-rw-   0        0        0     2959 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/concolic/concolic_execution.py
--rw-rw-rw-   0        0        0      645 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/concolic/concrete_data.py
--rw-rw-rw-   0        0        0     3469 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/concolic/find_trace.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.149303 smartExecutorx-0.3/mythril/disassembler/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/disassembler/__init__.py
--rw-rw-rw-   0        0        0     4523 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/disassembler/asm.py
--rw-rw-rw-   0        0        0     4770 2023-12-01 18:42:42.000000 smartExecutorx-0.3/mythril/disassembler/disassembly.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.152302 smartExecutorx-0.3/mythril/ethereum/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/ethereum/__init__.py
--rw-rw-rw-   0        0        0     3282 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/ethereum/evmcontract.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.153303 smartExecutorx-0.3/mythril/ethereum/interface/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/ethereum/interface/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.160483 smartExecutorx-0.3/mythril/ethereum/interface/rpc/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/ethereum/interface/rpc/__init__.py
--rw-rw-rw-   0        0        0     2896 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/ethereum/interface/rpc/base_client.py
--rw-rw-rw-   0        0        0     2500 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/ethereum/interface/rpc/client.py
--rw-rw-rw-   0        0        0      248 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/ethereum/interface/rpc/constants.py
--rw-rw-rw-   0        0        0      765 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/ethereum/interface/rpc/exceptions.py
--rw-rw-rw-   0        0        0      991 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/ethereum/interface/rpc/utils.py
--rw-rw-rw-   0        0        0     6534 2023-11-01 14:54:19.000000 smartExecutorx-0.3/mythril/ethereum/util.py
--rw-rw-rw-   0        0        0     1175 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.165884 smartExecutorx-0.3/mythril/interfaces/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/interfaces/__init__.py
--rw-rw-rw-   0        0        0    34137 2023-12-01 18:43:09.000000 smartExecutorx-0.3/mythril/interfaces/cli.py
--rw-rw-rw-   0        0        0     7462 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/interfaces/epic.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.167883 smartExecutorx-0.3/mythril/laser/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.180483 smartExecutorx-0.3/mythril/laser/ethereum/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/__init__.py
--rw-rw-rw-   0        0        0     8985 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/call.py
--rw-rw-rw-   0        0        0     2825 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/cfg.py
--rw-rw-rw-   0        0        0     1924 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/cheat_code.py
--rw-rw-rw-   0        0        0      936 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/evm_exceptions.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.183760 smartExecutorx-0.3/mythril/laser/ethereum/function_managers/
--rw-rw-rw-   0        0        0      151 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/function_managers/__init__.py
--rw-rw-rw-   0        0        0     2291 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/function_managers/exponent_function_manager.py
--rw-rw-rw-   0        0        0     7644 2023-10-30 20:54:42.000000 smartExecutorx-0.3/mythril/laser/ethereum/function_managers/keccak_function_manager.py
--rw-rw-rw-   0        0        0     1447 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/instruction_data.py
--rw-rw-rw-   0        0        0    87355 2023-10-30 20:54:42.000000 smartExecutorx-0.3/mythril/laser/ethereum/instructions.py
--rw-rw-rw-   0        0        0     8063 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/natives.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.197178 smartExecutorx-0.3/mythril/laser/ethereum/state/
--rw-rw-rw-   0        0        0       10 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/state/__init__.py
--rw-rw-rw-   0        0        0     7426 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/state/account.py
--rw-rw-rw-   0        0        0     2200 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/state/annotation.py
--rw-rw-rw-   0        0        0    10018 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/state/calldata.py
--rw-rw-rw-   0        0        0     4489 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/state/constraints.py
--rw-rw-rw-   0        0        0     2152 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/state/environment.py
--rw-rw-rw-   0        0        0     5814 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/state/global_state.py
--rw-rw-rw-   0        0        0     8218 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/state/machine_state.py
--rw-rw-rw-   0        0        0     8877 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/state/memory.py
--rw-rw-rw-   0        0        0      742 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/state/return_data.py
--rw-rw-rw-   0        0        0     9119 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/state/world_state.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.202667 smartExecutorx-0.3/mythril/laser/ethereum/strategy/
--rw-rw-rw-   0        0        0     1583 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/strategy/__init__.py
--rw-rw-rw-   0        0        0     3639 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/strategy/basic.py
--rw-rw-rw-   0        0        0     1266 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/strategy/beam.py
--rw-rw-rw-   0        0        0     5023 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/strategy/concolic.py
--rw-rw-rw-   0        0        0     1799 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/strategy/constraint_strategy.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.204670 smartExecutorx-0.3/mythril/laser/ethereum/strategy/extensions/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/strategy/extensions/__init__.py
--rw-rw-rw-   0        0        0     4546 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/strategy/extensions/bounded_loops.py
--rw-rw-rw-   0        0        0    40658 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/svm.py
--rw-rw-rw-   0        0        0      521 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/time_handler.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.207865 smartExecutorx-0.3/mythril/laser/ethereum/transaction/
--rw-rw-rw-   0        0        0      190 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/transaction/__init__.py
--rw-rw-rw-   0        0        0     5546 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/transaction/concolic.py
--rw-rw-rw-   0        0        0    10799 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/transaction/symbolic.py
--rw-rw-rw-   0        0        0    10038 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/transaction/transaction_models.py
--rw-rw-rw-   0        0        0     5023 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/ethereum/util.py
--rw-rw-rw-   0        0        0      284 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/execution_info.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.212818 smartExecutorx-0.3/mythril/laser/plugin/
--rw-rw-rw-   0        0        0      754 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/__init__.py
--rw-rw-rw-   0        0        0      454 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/builder.py
--rw-rw-rw-   0        0        0      939 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/interface.py
--rw-rw-rw-   0        0        0     3826 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/loader.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.218061 smartExecutorx-0.3/mythril/laser/plugin/plugins/
--rw-rw-rw-   0        0        0      623 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/plugins/__init__.py
--rw-rw-rw-   0        0        0     2867 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/plugins/benchmark.py
--rw-rw-rw-   0        0        0     1036 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/plugins/call_depth_limiter.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.221066 smartExecutorx-0.3/mythril/laser/plugin/plugins/coverage/
--rw-rw-rw-   0        0        0      104 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/plugins/coverage/__init__.py
--rw-rw-rw-   0        0        0     4401 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/plugins/coverage/coverage_plugin.py
--rw-rw-rw-   0        0        0     1869 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/plugins/coverage/coverage_strategy.py
--rw-rw-rw-   0        0        0    13351 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/plugins/dependency_pruner.py
--rw-rw-rw-   0        0        0     3745 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/plugins/instruction_profiler.py
--rw-rw-rw-   0        0        0     3574 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/plugins/mutation_pruner.py
--rw-rw-rw-   0        0        0     4960 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/plugins/plugin_annotations.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.222065 smartExecutorx-0.3/mythril/laser/plugin/plugins/summary_backup/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/plugins/summary_backup/__init__.py
--rw-rw-rw-   0        0        0      677 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/plugin/signals.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.233209 smartExecutorx-0.3/mythril/laser/smt/
--rw-rw-rw-   0        0        0     5236 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/smt/__init__.py
--rw-rw-rw-   0        0        0     2695 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/smt/array.py
--rw-rw-rw-   0        0        0     8808 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/smt/bitvec.py
--rw-rw-rw-   0        0        0     6161 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/smt/bitvec_helper.py
--rw-rw-rw-   0        0        0     4130 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/smt/bool.py
--rw-rw-rw-   0        0        0     2386 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/smt/expression.py
--rw-rw-rw-   0        0        0     1133 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/smt/function.py
--rw-rw-rw-   0        0        0     2213 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/smt/model.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.236380 smartExecutorx-0.3/mythril/laser/smt/solver/
--rw-rw-rw-   0        0        0      356 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/smt/solver/__init__.py
--rw-rw-rw-   0        0        0     5157 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/smt/solver/independence_solver.py
--rw-rw-rw-   0        0        0     3626 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/smt/solver/solver.py
--rw-rw-rw-   0        0        0     1041 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/laser/smt/solver/solver_statistics.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.241166 smartExecutorx-0.3/mythril/mythril/
--rw-rw-rw-   0        0        0      145 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/mythril/__init__.py
--rw-rw-rw-   0        0        0     8241 2023-10-09 02:14:28.000000 smartExecutorx-0.3/mythril/mythril/mythril_analyzer.py
--rw-rw-rw-   0        0        0     8198 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/mythril/mythril_config.py
--rw-rw-rw-   0        0        0    15253 2023-10-14 18:03:08.000000 smartExecutorx-0.3/mythril/mythril/mythril_disassembler.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.244542 smartExecutorx-0.3/mythril/plugin/
--rw-rw-rw-   0        0        0      125 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/plugin/__init__.py
--rw-rw-rw-   0        0        0     2235 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/plugin/discovery.py
--rw-rw-rw-   0        0        0     1441 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/plugin/interface.py
--rw-rw-rw-   0        0        0     2849 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/plugin/loader.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.247655 smartExecutorx-0.3/mythril/solidity/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/solidity/__init__.py
--rw-rw-rw-   0        0        0    12703 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/solidity/soliditycontract.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.258958 smartExecutorx-0.3/mythril/support/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/support/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.259956 smartExecutorx-0.3/mythril/support/assets/
--rw-rw-rw-   0        0        0 12406784 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/support/assets/signatures.db
--rw-rw-rw-   0        0        0     3069 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/support/loader.py
--rw-rw-rw-   0        0        0     2094 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/support/lock.py
--rw-rw-rw-   0        0        0     3923 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/support/model.py
--rw-rw-rw-   0        0        0     7543 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/support/opcodes.py
--rw-rw-rw-   0        0        0     9223 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/support/signatures.py
--rw-rw-rw-   0        0        0     2613 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/support/source_support.py
--rw-rw-rw-   0        0        0      260 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/support/start_time.py
--rw-rw-rw-   0        0        0      734 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/support/support_args.py
--rw-rw-rw-   0        0        0     3255 2023-10-09 01:29:55.000000 smartExecutorx-0.3/mythril/support/support_utils.py
--rw-rw-rw-   0        0        0      735 2023-10-09 01:29:55.000000 smartExecutorx-0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-12-01 20:24:22.323691 smartExecutorx-0.3/setup.cfg
--rw-rw-rw-   0        0        0     4264 2023-12-01 20:15:46.000000 smartExecutorx-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.286667 smartExecutorx-0.3/smartExecutorx.egg-info/
--rw-rw-rw-   0        0        0     6003 2023-12-01 20:24:21.000000 smartExecutorx-0.3/smartExecutorx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7779 2023-12-01 20:24:21.000000 smartExecutorx-0.3/smartExecutorx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-01 20:24:21.000000 smartExecutorx-0.3/smartExecutorx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-12-01 20:24:21.000000 smartExecutorx-0.3/smartExecutorx.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      694 2023-12-01 20:24:21.000000 smartExecutorx-0.3/smartExecutorx.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-12-01 20:24:21.000000 smartExecutorx-0.3/smartExecutorx.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.057392 smartExecutorx-0.3/tests/
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.288667 smartExecutorx-0.3/tests/disassembler/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/disassembler/__init__.py
--rw-rw-rw-   0        0        0     3152 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/disassembler/asm.py
--rw-rw-rw-   0        0        0     1728 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/disassembler/disassembly.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.302338 smartExecutorx-0.3/tests/instructions/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/instructions/__init__.py
--rw-rw-rw-   0        0        0     2747 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/instructions/berlin_fork_opcodes_test.py
--rw-rw-rw-   0        0        0     1319 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/instructions/codecopy_test.py
--rw-rw-rw-   0        0        0     2579 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/instructions/create2_test.py
--rw-rw-rw-   0        0        0     1947 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/instructions/create_test.py
--rw-rw-rw-   0        0        0     2295 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/instructions/extcodecopy_test.py
--rw-rw-rw-   0        0        0     2015 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/instructions/extcodehash_test.py
--rw-rw-rw-   0        0        0     5835 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/instructions/sar_test.py
--rw-rw-rw-   0        0        0     4698 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/instructions/shl_test.py
--rw-rw-rw-   0        0        0     4763 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/instructions/shr_test.py
--rw-rw-rw-   0        0        0     4067 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/instructions/static_call_test.py
--rw-rw-rw-   0        0        0     1393 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/instructions/test_basefee.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.304337 smartExecutorx-0.3/tests/laser/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-0.3/tests/laser/__init__.py
--rw-rw-rw-   0        0        0     4300 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/laser/keccak_tests.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.307552 smartExecutorx-0.3/tests/laser/smt/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/laser/smt/__init__.py
--rw-rw-rw-   0        0        0     3570 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/laser/smt/independece_solver_test.py
--rw-rw-rw-   0        0        0     1189 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/laser/smt/model_test.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.314689 smartExecutorx-0.3/tests/laser/state/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/laser/state/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/laser/state/calldata_test.py
--rw-rw-rw-   0        0        0     1327 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/laser/state/mstack_test.py
--rw-rw-rw-   0        0        0     3673 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/laser/state/mstate_test.py
--rw-rw-rw-   0        0        0     1584 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/laser/state/storage_test.py
--rw-rw-rw-   0        0        0     1909 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/laser/state/world_state_account_exist_load_test.py
--rw-rw-rw-   0        0        0     2546 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/laser/test_transaction.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.320690 smartExecutorx-0.3/tests/laser/transaction/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/laser/transaction/__init__.py
--rw-rw-rw-   0        0        0     1732 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/laser/transaction/create_transaction_test.py
--rw-rw-rw-   0        0        0     2143 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/laser/transaction/symbolic_test.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:24:22.321691 smartExecutorx-0.3/tests/testdata/
--rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/testdata/__init__.py
--rw-rw-rw-   0        0        0      446 2023-10-09 01:29:56.000000 smartExecutorx-0.3/tests/testdata/compile.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:41.009657 smartExecutorx-4.0/
+-rw-rw-rw-   0        0        0     1112 2023-10-09 01:29:55.000000 smartExecutorx-4.0/LICENSE
+-rw-rw-rw-   0        0        0      112 2023-10-09 05:58:34.000000 smartExecutorx-4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5876 2024-05-01 11:53:41.009657 smartExecutorx-4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5091 2024-05-01 11:40:16.000000 smartExecutorx-4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.828003 smartExecutorx-4.0/fdg/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/fdg/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-05-01 04:56:29.000000 smartExecutorx-4.0/fdg/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.834517 smartExecutorx-4.0/fdg/control/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/fdg/control/__init__.py
+-rw-rw-rw-   0        0        0    13717 2024-04-30 03:03:58.000000 smartExecutorx-4.0/fdg/control/ftn_search_strategy.py
+-rw-rw-rw-   0        0        0    12289 2023-11-07 20:50:26.000000 smartExecutorx-4.0/fdg/control/function_assignment.py
+-rw-rw-rw-   0        0        0     9908 2024-04-30 03:03:58.000000 smartExecutorx-4.0/fdg/control/guider.py
+-rw-rw-rw-   0        0        0    23756 2024-04-30 11:17:07.000000 smartExecutorx-4.0/fdg/control/mine.py
+-rw-rw-rw-   0        0        0     2219 2023-10-30 22:15:11.000000 smartExecutorx-4.0/fdg/control/weight_computation.py
+-rw-rw-rw-   0        0        0     6308 2024-04-30 11:09:14.000000 smartExecutorx-4.0/fdg/expression_slot.py
+-rw-rw-rw-   0        0        0    14495 2024-05-01 04:56:29.000000 smartExecutorx-4.0/fdg/fdg_pruner.py
+-rw-rw-rw-   0        0        0     5658 2024-04-30 03:03:58.000000 smartExecutorx-4.0/fdg/function_coverage.py
+-rw-rw-rw-   0        0        0    13147 2024-05-01 04:27:00.000000 smartExecutorx-4.0/fdg/fwrg_manager.py
+-rw-rw-rw-   0        0        0     3263 2024-04-30 03:03:58.000000 smartExecutorx-4.0/fdg/global_config.py
+-rw-rw-rw-   0        0        0    16303 2024-04-17 02:45:47.000000 smartExecutorx-4.0/fdg/instruction_modification.py
+-rw-rw-rw-   0        0        0     9534 2023-11-05 22:48:36.000000 smartExecutorx-4.0/fdg/output_data.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.838033 smartExecutorx-4.0/fdg/preprocessing/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/fdg/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2028 2023-10-16 02:38:03.000000 smartExecutorx-4.0/fdg/preprocessing/address_collection.py
+-rw-rw-rw-   0        0        0     4959 2023-10-09 01:29:55.000000 smartExecutorx-4.0/fdg/preprocessing/instruction_coverage.py
+-rw-rw-rw-   0        0        0     4583 2024-04-17 02:45:47.000000 smartExecutorx-4.0/fdg/preprocessing/preprocess.py
+-rw-rw-rw-   0        0        0     3149 2024-04-17 02:45:47.000000 smartExecutorx-4.0/fdg/preprocessing/read_in_conditions.py
+-rw-rw-rw-   0        0        0     7945 2024-04-17 02:45:47.000000 smartExecutorx-4.0/fdg/preprocessing/slot_location.py
+-rw-rw-rw-   0        0        0     4215 2023-11-01 01:55:38.000000 smartExecutorx-4.0/fdg/preprocessing/write_read_info.py
+-rw-rw-rw-   0        0        0     4182 2024-05-01 04:56:29.000000 smartExecutorx-4.0/fdg/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.842316 smartExecutorx-4.0/mythril/
+-rw-rw-rw-   0        0        0      371 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/__init__.py
+-rw-rw-rw-   0        0        0      145 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/__main__.py
+-rw-rw-rw-   0        0        0      265 2024-05-01 03:09:12.000000 smartExecutorx-4.0/mythril/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.842316 smartExecutorx-4.0/mythril/analysis/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/analysis_args.py
+-rw-rw-rw-   0        0        0     1847 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/call_helpers.py
+-rw-rw-rw-   0        0        0     7045 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/callgraph.py
+-rw-rw-rw-   0        0        0     1067 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/issue_annotation.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.858466 smartExecutorx-4.0/mythril/analysis/module/
+-rw-rw-rw-   0        0        0      236 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/__init__.py
+-rw-rw-rw-   0        0        0     4358 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/base.py
+-rw-rw-rw-   0        0        0     4187 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/loader.py
+-rw-rw-rw-   0        0        0      407 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/module_helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.875490 smartExecutorx-4.0/mythril/analysis/module/modules/
+-rw-rw-rw-   0        0        0        2 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/modules/__init__.py
+-rw-rw-rw-   0        0        0     3738 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/modules/arbitrary_jump.py
+-rw-rw-rw-   0        0        0     2594 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/modules/arbitrary_write.py
+-rw-rw-rw-   0        0        0     3761 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/modules/delegatecall.py
+-rw-rw-rw-   0        0        0     4068 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/modules/dependence_on_origin.py
+-rw-rw-rw-   0        0        0     7652 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/modules/dependence_on_predictable_vars.py
+-rw-rw-rw-   0        0        0     3601 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/modules/ether_thief.py
+-rw-rw-rw-   0        0        0     5319 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/modules/exceptions.py
+-rw-rw-rw-   0        0        0     4033 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/modules/external_calls.py
+-rw-rw-rw-   0        0        0    11819 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/modules/integer.py
+-rw-rw-rw-   0        0        0     4353 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/modules/multiple_sends.py
+-rw-rw-rw-   0        0        0     7843 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/modules/state_change_external_calls.py
+-rw-rw-rw-   0        0        0     4793 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/modules/suicide.py
+-rw-rw-rw-   0        0        0     5791 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/modules/unchecked_retval.py
+-rw-rw-rw-   0        0        0     4303 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/modules/user_assertions.py
+-rw-rw-rw-   0        0        0     2006 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/module/util.py
+-rw-rw-rw-   0        0        0     1915 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/ops.py
+-rw-rw-rw-   0        0        0     4506 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/potential_issues.py
+-rw-rw-rw-   0        0        0    12882 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/report.py
+-rw-rw-rw-   0        0        0     1535 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/security.py
+-rw-rw-rw-   0        0        0     9558 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/solver.py
+-rw-rw-rw-   0        0        0     2452 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/swc_data.py
+-rw-rw-rw-   0        0        0    12997 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/symbolic.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.875490 smartExecutorx-4.0/mythril/analysis/templates/
+-rw-rw-rw-   0        0        0     2262 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/templates/callgraph.html
+-rw-rw-rw-   0        0        0     2075 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/templates/report_as_markdown.jinja2
+-rw-rw-rw-   0        0        0     1954 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/templates/report_as_text.jinja2
+-rw-rw-rw-   0        0        0     4902 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/analysis/traceexplore.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.875490 smartExecutorx-4.0/mythril/concolic/
+-rw-rw-rw-   0        0        0      128 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/concolic/__init__.py
+-rw-rw-rw-   0        0        0     2959 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/concolic/concolic_execution.py
+-rw-rw-rw-   0        0        0      645 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/concolic/concrete_data.py
+-rw-rw-rw-   0        0        0     3469 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/concolic/find_trace.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.875490 smartExecutorx-4.0/mythril/disassembler/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/disassembler/__init__.py
+-rw-rw-rw-   0        0        0     4523 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/disassembler/asm.py
+-rw-rw-rw-   0        0        0     4770 2023-12-01 18:42:42.000000 smartExecutorx-4.0/mythril/disassembler/disassembly.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.875490 smartExecutorx-4.0/mythril/ethereum/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/ethereum/__init__.py
+-rw-rw-rw-   0        0        0     3282 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/ethereum/evmcontract.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.888498 smartExecutorx-4.0/mythril/ethereum/interface/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/ethereum/interface/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.891638 smartExecutorx-4.0/mythril/ethereum/interface/rpc/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/ethereum/interface/rpc/__init__.py
+-rw-rw-rw-   0        0        0     2896 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/ethereum/interface/rpc/base_client.py
+-rw-rw-rw-   0        0        0     2500 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/ethereum/interface/rpc/client.py
+-rw-rw-rw-   0        0        0      248 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/ethereum/interface/rpc/constants.py
+-rw-rw-rw-   0        0        0      765 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/ethereum/interface/rpc/exceptions.py
+-rw-rw-rw-   0        0        0      991 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/ethereum/interface/rpc/utils.py
+-rw-rw-rw-   0        0        0     6534 2023-11-01 14:54:19.000000 smartExecutorx-4.0/mythril/ethereum/util.py
+-rw-rw-rw-   0        0        0     1175 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.891638 smartExecutorx-4.0/mythril/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/interfaces/__init__.py
+-rw-rw-rw-   0        0        0    34731 2024-05-01 03:08:10.000000 smartExecutorx-4.0/mythril/interfaces/cli.py
+-rw-rw-rw-   0        0        0     7462 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/interfaces/epic.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.891638 smartExecutorx-4.0/mythril/laser/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.908387 smartExecutorx-4.0/mythril/laser/ethereum/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/__init__.py
+-rw-rw-rw-   0        0        0     8985 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/call.py
+-rw-rw-rw-   0        0        0     2825 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/cfg.py
+-rw-rw-rw-   0        0        0     1924 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/cheat_code.py
+-rw-rw-rw-   0        0        0      936 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/evm_exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.908895 smartExecutorx-4.0/mythril/laser/ethereum/function_managers/
+-rw-rw-rw-   0        0        0      151 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/function_managers/__init__.py
+-rw-rw-rw-   0        0        0     2291 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/function_managers/exponent_function_manager.py
+-rw-rw-rw-   0        0        0     7644 2023-10-30 20:54:42.000000 smartExecutorx-4.0/mythril/laser/ethereum/function_managers/keccak_function_manager.py
+-rw-rw-rw-   0        0        0     1447 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/instruction_data.py
+-rw-rw-rw-   0        0        0    87355 2023-10-30 20:54:42.000000 smartExecutorx-4.0/mythril/laser/ethereum/instructions.py
+-rw-rw-rw-   0        0        0     8063 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/natives.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.918905 smartExecutorx-4.0/mythril/laser/ethereum/state/
+-rw-rw-rw-   0        0        0       10 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/state/__init__.py
+-rw-rw-rw-   0        0        0     7426 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/state/account.py
+-rw-rw-rw-   0        0        0     2200 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/state/annotation.py
+-rw-rw-rw-   0        0        0    10018 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/state/calldata.py
+-rw-rw-rw-   0        0        0     4489 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/state/constraints.py
+-rw-rw-rw-   0        0        0     2152 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/state/environment.py
+-rw-rw-rw-   0        0        0     5814 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/state/global_state.py
+-rw-rw-rw-   0        0        0     8218 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/state/machine_state.py
+-rw-rw-rw-   0        0        0     8877 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/state/memory.py
+-rw-rw-rw-   0        0        0      742 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/state/return_data.py
+-rw-rw-rw-   0        0        0     9119 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/state/world_state.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.918905 smartExecutorx-4.0/mythril/laser/ethereum/strategy/
+-rw-rw-rw-   0        0        0     1583 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/strategy/__init__.py
+-rw-rw-rw-   0        0        0     3639 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/strategy/basic.py
+-rw-rw-rw-   0        0        0     1266 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/strategy/beam.py
+-rw-rw-rw-   0        0        0     5023 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/strategy/concolic.py
+-rw-rw-rw-   0        0        0     1799 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/strategy/constraint_strategy.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.925223 smartExecutorx-4.0/mythril/laser/ethereum/strategy/extensions/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/strategy/extensions/__init__.py
+-rw-rw-rw-   0        0        0     4546 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/strategy/extensions/bounded_loops.py
+-rw-rw-rw-   0        0        0    40658 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/svm.py
+-rw-rw-rw-   0        0        0      521 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/time_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.925223 smartExecutorx-4.0/mythril/laser/ethereum/transaction/
+-rw-rw-rw-   0        0        0      190 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/transaction/__init__.py
+-rw-rw-rw-   0        0        0     5546 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/transaction/concolic.py
+-rw-rw-rw-   0        0        0    10799 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/transaction/symbolic.py
+-rw-rw-rw-   0        0        0    10038 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/transaction/transaction_models.py
+-rw-rw-rw-   0        0        0     5023 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/ethereum/util.py
+-rw-rw-rw-   0        0        0      284 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/execution_info.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.925223 smartExecutorx-4.0/mythril/laser/plugin/
+-rw-rw-rw-   0        0        0      754 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/plugin/__init__.py
+-rw-rw-rw-   0        0        0      454 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/plugin/builder.py
+-rw-rw-rw-   0        0        0      939 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/plugin/interface.py
+-rw-rw-rw-   0        0        0     3826 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/plugin/loader.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.938239 smartExecutorx-4.0/mythril/laser/plugin/plugins/
+-rw-rw-rw-   0        0        0      623 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/plugin/plugins/__init__.py
+-rw-rw-rw-   0        0        0     2867 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/plugin/plugins/benchmark.py
+-rw-rw-rw-   0        0        0     1036 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/plugin/plugins/call_depth_limiter.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.941477 smartExecutorx-4.0/mythril/laser/plugin/plugins/coverage/
+-rw-rw-rw-   0        0        0      104 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/plugin/plugins/coverage/__init__.py
+-rw-rw-rw-   0        0        0     4401 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/plugin/plugins/coverage/coverage_plugin.py
+-rw-rw-rw-   0        0        0     1869 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/plugin/plugins/coverage/coverage_strategy.py
+-rw-rw-rw-   0        0        0    12968 2024-02-04 06:04:24.000000 smartExecutorx-4.0/mythril/laser/plugin/plugins/dependency_pruner.py
+-rw-rw-rw-   0        0        0     3745 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/plugin/plugins/instruction_profiler.py
+-rw-rw-rw-   0        0        0     3574 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/plugin/plugins/mutation_pruner.py
+-rw-rw-rw-   0        0        0     4960 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/plugin/plugins/plugin_annotations.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.941477 smartExecutorx-4.0/mythril/laser/plugin/plugins/summary_backup/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/plugin/plugins/summary_backup/__init__.py
+-rw-rw-rw-   0        0        0      677 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/plugin/signals.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.948987 smartExecutorx-4.0/mythril/laser/smt/
+-rw-rw-rw-   0        0        0     5236 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/smt/__init__.py
+-rw-rw-rw-   0        0        0     2695 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/smt/array.py
+-rw-rw-rw-   0        0        0     8808 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/smt/bitvec.py
+-rw-rw-rw-   0        0        0     6161 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/smt/bitvec_helper.py
+-rw-rw-rw-   0        0        0     4130 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/smt/bool.py
+-rw-rw-rw-   0        0        0     2386 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/smt/expression.py
+-rw-rw-rw-   0        0        0     1133 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/smt/function.py
+-rw-rw-rw-   0        0        0     2213 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/smt/model.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.948987 smartExecutorx-4.0/mythril/laser/smt/solver/
+-rw-rw-rw-   0        0        0      356 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/smt/solver/__init__.py
+-rw-rw-rw-   0        0        0     5157 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/smt/solver/independence_solver.py
+-rw-rw-rw-   0        0        0     3626 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/smt/solver/solver.py
+-rw-rw-rw-   0        0        0     1041 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/laser/smt/solver/solver_statistics.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.948987 smartExecutorx-4.0/mythril/mythril/
+-rw-rw-rw-   0        0        0      145 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/mythril/__init__.py
+-rw-rw-rw-   0        0        0     8065 2024-05-01 04:56:29.000000 smartExecutorx-4.0/mythril/mythril/mythril_analyzer.py
+-rw-rw-rw-   0        0        0     8198 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/mythril/mythril_config.py
+-rw-rw-rw-   0        0        0    15253 2023-10-14 18:03:08.000000 smartExecutorx-4.0/mythril/mythril/mythril_disassembler.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.958740 smartExecutorx-4.0/mythril/plugin/
+-rw-rw-rw-   0        0        0      125 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/plugin/__init__.py
+-rw-rw-rw-   0        0        0     2235 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/plugin/discovery.py
+-rw-rw-rw-   0        0        0     1441 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/plugin/interface.py
+-rw-rw-rw-   0        0        0     2849 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/plugin/loader.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.958740 smartExecutorx-4.0/mythril/solidity/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/solidity/__init__.py
+-rw-rw-rw-   0        0        0    12703 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/solidity/soliditycontract.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.958740 smartExecutorx-4.0/mythril/support/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/support/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.958740 smartExecutorx-4.0/mythril/support/assets/
+-rw-rw-rw-   0        0        0 12406784 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/support/assets/signatures.db
+-rw-rw-rw-   0        0        0     3069 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/support/loader.py
+-rw-rw-rw-   0        0        0     2094 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/support/lock.py
+-rw-rw-rw-   0        0        0     3923 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/support/model.py
+-rw-rw-rw-   0        0        0     7543 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/support/opcodes.py
+-rw-rw-rw-   0        0        0     9223 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/support/signatures.py
+-rw-rw-rw-   0        0        0     2613 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/support/source_support.py
+-rw-rw-rw-   0        0        0      260 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/support/start_time.py
+-rw-rw-rw-   0        0        0      734 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/support/support_args.py
+-rw-rw-rw-   0        0        0     3255 2023-10-09 01:29:55.000000 smartExecutorx-4.0/mythril/support/support_utils.py
+-rw-rw-rw-   0        0        0      735 2023-10-09 01:29:55.000000 smartExecutorx-4.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 11:53:41.009657 smartExecutorx-4.0/setup.cfg
+-rw-rw-rw-   0        0        0     4264 2024-05-01 11:53:31.000000 smartExecutorx-4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.979254 smartExecutorx-4.0/smartExecutorx.egg-info/
+-rw-rw-rw-   0        0        0     5876 2024-05-01 11:53:40.000000 smartExecutorx-4.0/smartExecutorx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7691 2024-05-01 11:53:40.000000 smartExecutorx-4.0/smartExecutorx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 11:53:40.000000 smartExecutorx-4.0/smartExecutorx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-01 11:53:40.000000 smartExecutorx-4.0/smartExecutorx.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      694 2024-05-01 11:53:40.000000 smartExecutorx-4.0/smartExecutorx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-01 11:53:40.000000 smartExecutorx-4.0/smartExecutorx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.807978 smartExecutorx-4.0/tests/
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.979254 smartExecutorx-4.0/tests/disassembler/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/disassembler/__init__.py
+-rw-rw-rw-   0        0        0     3152 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/disassembler/asm.py
+-rw-rw-rw-   0        0        0     1728 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/disassembler/disassembly.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.991514 smartExecutorx-4.0/tests/instructions/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/instructions/__init__.py
+-rw-rw-rw-   0        0        0     2747 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/instructions/berlin_fork_opcodes_test.py
+-rw-rw-rw-   0        0        0     1319 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/instructions/codecopy_test.py
+-rw-rw-rw-   0        0        0     2579 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/instructions/create2_test.py
+-rw-rw-rw-   0        0        0     1947 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/instructions/create_test.py
+-rw-rw-rw-   0        0        0     2295 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/instructions/extcodecopy_test.py
+-rw-rw-rw-   0        0        0     2015 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/instructions/extcodehash_test.py
+-rw-rw-rw-   0        0        0     5835 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/instructions/sar_test.py
+-rw-rw-rw-   0        0        0     4698 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/instructions/shl_test.py
+-rw-rw-rw-   0        0        0     4763 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/instructions/shr_test.py
+-rw-rw-rw-   0        0        0     4067 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/instructions/static_call_test.py
+-rw-rw-rw-   0        0        0     1393 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/instructions/test_basefee.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.991514 smartExecutorx-4.0/tests/laser/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:55.000000 smartExecutorx-4.0/tests/laser/__init__.py
+-rw-rw-rw-   0        0        0     4300 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/laser/keccak_tests.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:40.991514 smartExecutorx-4.0/tests/laser/smt/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/laser/smt/__init__.py
+-rw-rw-rw-   0        0        0     3570 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/laser/smt/independece_solver_test.py
+-rw-rw-rw-   0        0        0     1189 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/laser/smt/model_test.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:41.007603 smartExecutorx-4.0/tests/laser/state/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/laser/state/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/laser/state/calldata_test.py
+-rw-rw-rw-   0        0        0     1327 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/laser/state/mstack_test.py
+-rw-rw-rw-   0        0        0     3673 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/laser/state/mstate_test.py
+-rw-rw-rw-   0        0        0     1584 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/laser/state/storage_test.py
+-rw-rw-rw-   0        0        0     1909 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/laser/state/world_state_account_exist_load_test.py
+-rw-rw-rw-   0        0        0     2546 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/laser/test_transaction.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:41.009657 smartExecutorx-4.0/tests/laser/transaction/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/laser/transaction/__init__.py
+-rw-rw-rw-   0        0        0     1732 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/laser/transaction/create_transaction_test.py
+-rw-rw-rw-   0        0        0     2143 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/laser/transaction/symbolic_test.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:53:41.009657 smartExecutorx-4.0/tests/testdata/
+-rw-rw-rw-   0        0        0        0 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/testdata/__init__.py
+-rw-rw-rw-   0        0        0      446 2023-10-09 01:29:56.000000 smartExecutorx-4.0/tests/testdata/compile.py
```

### Comparing `smartExecutorx-0.3/LICENSE` & `smartExecutorx-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/fdg/constraint_check_time.py` & `smartExecutorx-4.0/mythril/laser/smt/solver/solver_statistics.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 from time import time
+
 from mythril.support.support_utils import Singleton
+
 from typing import Callable
 
-def constraint_check_time_flags(func: Callable):
+
+def stat_smt_query(func: Callable):
     """Measures statistics for annotated smt query check function"""
-    cons_chk_flags = StateConstraintCheckIndicator()
+    stat_store = SolverStatistics()
 
     def function_wrapper(*args, **kwargs):
-        # if not cons_chk_flags.enabled:
-        #     return func(*args, **kwargs)
+        if not stat_store.enabled:
+            return func(*args, **kwargs)
+
+        stat_store.query_count += 1
         begin = time()
 
         result = func(*args, **kwargs)
 
         end = time()
-        cons_chk_flags.accumated_time += end - begin
-        # print(f'constraint checking accumulated time:{cons_chk_flags.accumated_time}')
+        stat_store.solver_time += end - begin
 
         return result
 
     return function_wrapper
 
 
-class StateConstraintCheckIndicator(object, metaclass=Singleton):
+class SolverStatistics(object, metaclass=Singleton):
+    """Solver Statistics Class
+
+    Keeps track of the important statistics around smt queries
+    """
+
     def __init__(self):
-        self.accumated_time = 0
         self.enabled = False
-
+        self.query_count = 0
+        self.solver_time = 0
 
     def __repr__(self):
-        return "checking time: {}".format(
-            self.accumated_time
+        return "Query count: {} \nSolver time: {}".format(
+            self.query_count, self.solver_time
         )
-
```

### Comparing `smartExecutorx-0.3/fdg/control/ftn_search_strategy.py` & `smartExecutorx-4.0/fdg/control/ftn_search_strategy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,368 +1,368 @@
-import ast
-
-from copy import deepcopy
-
-
-import fdg.global_config
-from fdg.control.function_assignment import FunctionAssignment
-
-from fdg.fwrg_manager import FWRG_manager
-from fdg.output_data import print_data_for_bfs_strategy, print_data_for_dfs_strategy
-
-from fdg.utils import get_ftn_seq_from_key_1
-
-
-
-
-class FunctionSearchStrategy():
-    def __init__(self,strategy_name:str):
-        self.name=strategy_name
-        self.world_states={}
-        self.search_history={}
-        self.current_state_key=''
-        # print(f'search strategy: {self.name}')
-
-    def save_states(self,key:str,states:list):
-        if key in self.world_states.keys():
-            self.world_states[key]+=states
-        else:
-            self.world_states[key]=states
-    def get_states(self,key:str):
-        if key in self.world_states.keys():
-            return self.world_states[key]
-        else:
-            return []
-    def delete_state(self,key:str):
-        if key in self.world_states.keys():
-            self.world_states.pop(key)
-
-    def assign_states(self, deep_functions: list=None, current_state_key: str = None, fdfg: FWRG_manager = None,
-                      states_dict: dict = {},iteration:int=0) -> list:
-        pass
-
-
-
-    def termination(self,states_num:int=0,current_seq_length:int=0,sequence_depth_limit:int=0,iteration:int=0)->bool:
-        ...
-
-
-
-class Seq(FunctionSearchStrategy):
-    def __init__(self):
-        self.queue = []
-
-        # # 0x00c0443f42932d9efe27e64409b21d2e48928d66.sol	0.5.8	JarvisExchange
-        # self.sequences = [
-        #     ['setController(address)', 'withdrawToken(address,uint256,uint256)']
-        # ]
-
-        # 0x9afb9d7ed0f6c054ec76ea61d5cabc384d4dcb25.sol	0.4.26	ConverterFactory
-        self.sequences = [
-            ['transferOwnership(address)', 'acceptOwnership()']
-        ]
-        #0x2caf5a42ec2d6747ec696714bf913b174d94fdf0.sol	0.5.17	LexLocker
-        # contain GT, and function signature with 3 bytes
-        self.sequences = [
-            ['updateJudgmentReward(uint256)']
-        ]
-
-        if len(fdg.global_config.sequences)>0:
-            # assume that the sequenes are presented as string
-            self.sequences=ast.literal_eval(fdg.global_config.sequences)
-        else:self.sequences=[]
-
-        super().__init__('seq')
-
-    def initialize(self, main_path_sf: dict, main_path_df: dict, fdfg_manager: FWRG_manager):
-        ...
-
-
-
-
-
-    def termination(self, states_num: int = 0, current_seq_length: int = 0, sequence_depth_limit: int = 0,
-                    iteration: int = 0) -> bool:
-        # need to test
-        if states_num == 0: return True
-        if iteration>2:
-            if len(self.queue) == 0:
-                return True
-        return False
-
-    def assign_states(self, deep_functions: list = None, current_state_key: str = None, fdfg: FWRG_manager = None,
-                      states_dict: dict = {},iteration:int=0) -> list:
-        """
-
-        :param deep_functions:
-        :param current_state_key:
-        :param fdfg:
-        :param states_dict:
-        :return:
-        """
-        if len(states_dict)>0:
-            for key, states in states_dict.items():
-
-                if key not in self.world_states.keys():
-                    self.world_states[key]=deepcopy(states)
-                else:
-                    self.world_states[key]+=deepcopy(states)
-                self.queue.append(key)
-
-        while True:
-            if len(self.queue)==0: return {},False
-            state_key=self.queue.pop(0)
-            if state_key=='constructor':
-                if len(self.sequences)==0:
-                    return {},True
-                return {'constructor':[seq[0] for seq in self.sequences]},True
-
-            seq=get_ftn_seq_from_key_1(state_key)
-            functions=[]
-            for seq_ in self.sequences:
-                if len(seq)==len(seq_):continue
-                if len(seq)<len(seq_):
-                    for i in range(len(seq)):
-                        if seq[i]!=seq_[i]:break
-                    functions.append(seq_[len(seq)])
-            if len(functions)>0:
-                return {state_key:functions},True
-
-
-class DFS(FunctionSearchStrategy):
-    def __init__(self):
-        self.stack=[]
-        self.preprocess_timeout = False
-        self.preprocess_coverage = 0
-        self.flag_one_state_at_depth1=False
-        super().__init__('dfs')
-
-    def initialize(self,flag_one_state_depth1:bool,preprocess_timeout:bool, preprocess_coverage:float,all_functions:list,fwrg_manager:FWRG_manager):
-        self.flag_one_state_at_depth1=flag_one_state_depth1
-        self.preprocess_timeout = preprocess_timeout
-        self.preprocess_coverage = preprocess_coverage
-        self.functionAssignment=FunctionAssignment(all_functions,fwrg_manager)
-
-
-    def termination(self,states_num:int=0, current_seq_length: int = 0, sequence_depth_limit: int = 0,iteration:int=0)->bool:
-        if iteration<=2:
-            if states_num==0:return True
-        return False
-
-
-
-
-
-    def assign_states(self, deep_functions: list=None, states_dict: dict = {},iteration:int=0) -> list:
-
-        """
-            save states, push state keys to the stack
-            select a state by poping an item from the stack
-            assign functions to be executed on the selected state
-        :param deep_functions:
-        :param current_state_key:
-        :param fdfg:
-        :param states_dict:
-        :return:
-        """
-        if len(states_dict)>0:
-            for key, states in states_dict.items():
-                ftn_seq=get_ftn_seq_from_key_1(key)
-                if len(ftn_seq)>=fdg.global_config.seq_len_limit:
-                    continue # do not save these states as they will not be explored
-                # save states
-                self.world_states[key]=deepcopy(states)
-                self.stack.append(key)
-
-        print_data_for_dfs_strategy(self.stack)
-
-        if self.flag_one_state_at_depth1:
-            self.flag_one_state_at_depth1=False
-            state_key = self.stack.pop()
-            assign_functions = self.functionAssignment.assign_all_functions()
-
-            return {state_key : assign_functions},True
-
-        while True:
-            if len(self.stack)==0:
-                return {},None
-
-            state_key=self.stack.pop()
-
-            if self.preprocess_timeout or fdg.global_config.preprocessing_exception:
-                if self.preprocess_coverage<50:
-                    assigned_functions=self.functionAssignment.assign_functions_timeout(state_key,deep_functions, 7)
-                    if len(assigned_functions) > 0:
-                        return {state_key: assigned_functions},True
-                    continue
-                elif self.preprocess_coverage < 80:
-                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,deep_functions, 5)
-                    if len(assigned_functions) > 0:
-                        return {state_key: assigned_functions},True
-                    continue
-                else:
-                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,deep_functions, 3)
-                    if len(assigned_functions) > 0:
-                        return {state_key: assigned_functions},True
-                    continue
-            assigned_functions = self.functionAssignment.assign_functions(state_key,deep_functions)
-            if len(assigned_functions) > 0:
-                return {state_key: assigned_functions},True
-
-
-
-class BFS(FunctionSearchStrategy):
-    """
-    no need to save states
-    """
-    def __init__(self):
-        self.flag_one_state_at_depth1=False
-        self.preprocess_timeout = False
-        self.preprocess_coverage = 0
-        self.queue=[]
-        super().__init__('bfs')
-        pass
-
-    def initialize(self,flag_one_state_depth1:bool,preprocess_timeout:bool, preprocess_coverage:float,all_functions:list,fwrg_manager:FWRG_manager):
-        self.flag_one_state_at_depth1=flag_one_state_depth1
-        self.preprocess_timeout = preprocess_timeout
-        self.preprocess_coverage = preprocess_coverage
-        self.functionAssignment=FunctionAssignment(all_functions,fwrg_manager)
-
-    def termination(self,states_num:int=0, current_seq_length: int = 0, sequence_depth_limit: int = 0,iteration:int=0)->bool:
-        if iteration <= 2:
-            if states_num == 0: return True
-        return False
-
-
-    def assign_states(self, dk_functions: list=None, current_state_key: str = None, fwrg: FWRG_manager = None,
-                      states_dict: dict = {},iteration:int=0) -> list:
-        """
-        assign functions for multiple states at the same time.
-        :param deep_functions:
-        :param current_state_key:
-        :param fwrg:
-        :param states_dict:
-        :return:
-        """
-
-        if len(states_dict) > 0:
-            for key, states in states_dict.items():
-                ftn_seq = get_ftn_seq_from_key_1(key)
-                if len(ftn_seq) >= fdg.global_config.seq_len_limit:
-                    continue  # do not save these states as they will not be explored
-                # save states
-                self.world_states[key] = deepcopy(states)
-                self.queue.append(key)
-
-            # # put key containing fallback at the end of the queue
-            # if len(ftn_seq)==1:
-            #     temp=[]
-            #     for item in self.queue:
-            #         if 'fallback' in item:
-            #             temp.append(item)
-            #         else:
-            #             temp=[item]+temp
-            #     self.queue=temp
-
-
-        print_data_for_bfs_strategy(self.queue)
-
-        if self.flag_one_state_at_depth1:
-            self.flag_one_state_at_depth1 = False
-            state_key = self.queue.pop(0)
-            assign_functions = self.functionAssignment.assign_all_functions()
-
-            return {state_key: assign_functions},True
-
-
-        while True:
-            if len(self.queue) == 0:
-                return {},None
-
-            state_key = self.queue.pop(0)
-            if self.preprocess_timeout or  fdg.global_config.preprocessing_exception:
-                if self.preprocess_coverage < 50:
-                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,dk_functions, 7)
-                    if len(assigned_functions) > 0:
-                        return {state_key: assigned_functions},True
-                    continue
-                elif self.preprocess_coverage < 80:
-                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,dk_functions, 5)
-                    if len(assigned_functions) > 0:
-                        return {state_key: assigned_functions},True
-                    continue
-                else:
-                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,dk_functions, 3)
-                    if len(assigned_functions) > 0:
-                        return {state_key: assigned_functions},True
-                    continue
-            assigned_functions = self.functionAssignment.assign_functions(state_key, dk_functions)
-            if len(assigned_functions) > 0:
-                return {state_key: assigned_functions},True
-
-
-
-class RandomBaseline(FunctionSearchStrategy):
-    """
-    no need to save states
-    """
-    def __init__(self,percent_of_functions:int,functions:list):
-        self.functionAssignment=FunctionAssignment(functions,None,select_percent=percent_of_functions)
-        self.flag_one_state_at_depth1=False
-        self.queue=[]
-        super().__init__('baseline')
-
-    def initialize(self, flag_one_state_depth1: bool):
-        self.flag_one_state_at_depth1 = flag_one_state_depth1
-
-    def assign_states(self, dk_functions: list=None, states_dict: dict = {}) -> list:
-        """
-        apply BFS
-        :param dk_functions:
-        :param current_state_key:
-        :param fwrg:
-        :param states_dict:
-        :return:
-        """
-        if len(states_dict) > 0:
-            for key, states in states_dict.items():
-                ftn_seq = get_ftn_seq_from_key_1(key)
-                if len(ftn_seq) >= fdg.global_config.seq_len_limit:
-                    continue  # do not save these states as they will not be explored
-                # save states
-                self.world_states[key] = deepcopy(states)
-                self.queue.append(key)
-
-        print_data_for_bfs_strategy(self.queue)
-
-        if self.flag_one_state_at_depth1:
-            self.flag_one_state_at_depth1 = False
-            state_key = self.queue.pop(0)
-            assign_functions = self.functionAssignment.assign_all_functions()
-
-            return {state_key: assign_functions}, True
-
-        while True:
-            if len(self.queue) == 0:
-                return {}, None
-
-            state_key = self.queue.pop(0)
-
-            assigned_functions =self.functionAssignment.assign_functions_for_baseline()
-            if len(assigned_functions) > 0:
-                return {state_key: assigned_functions}, True
-
-
-
-
-    def termination(self, states_num: int = None, current_seq_length: int = 0,
-                    sequence_depth_limit: int = 0,iteration:int=0) -> bool:
-
-        if iteration <= 1:
-            if states_num == 0: return True
-
-        return False
-
-
-
-
+import ast
+
+from copy import deepcopy
+
+
+import fdg.global_config
+from fdg.control.function_assignment import FunctionAssignment
+
+from fdg.fwrg_manager import FWRG_manager
+from fdg.output_data import print_data_for_bfs_strategy, print_data_for_dfs_strategy
+
+from fdg.utils import get_ftn_seq_from_key_1
+
+
+
+
+class FunctionSearchStrategy():
+    def __init__(self,strategy_name:str):
+        self.name=strategy_name
+        self.world_states={}
+        self.search_history={}
+        self.current_state_key=''
+        # print(f'search strategy: {self.name}')
+
+    def save_states(self,key:str,states:list):
+        if key in self.world_states.keys():
+            self.world_states[key]+=states
+        else:
+            self.world_states[key]=states
+    def get_states(self,key:str):
+        if key in self.world_states.keys():
+            return self.world_states[key]
+        else:
+            return []
+    def delete_state(self,key:str):
+        if key in self.world_states.keys():
+            self.world_states.pop(key)
+
+    def assign_states(self, deep_functions: list=None, current_state_key: str = None, fdfg: FWRG_manager = None,
+                      states_dict: dict = {},iteration:int=0) -> list:
+        pass
+
+
+
+    def termination(self,states_num:int=0,current_seq_length:int=0,sequence_depth_limit:int=0,iteration:int=0)->bool:
+        ...
+
+
+
+class Seq(FunctionSearchStrategy):
+    def __init__(self):
+        self.queue = []
+
+        # # 0x00c0443f42932d9efe27e64409b21d2e48928d66.sol	0.5.8	JarvisExchange
+        # self.sequences = [
+        #     ['setController(address)', 'withdrawToken(address,uint256,uint256)']
+        # ]
+
+        # 0x9afb9d7ed0f6c054ec76ea61d5cabc384d4dcb25.sol	0.4.26	ConverterFactory
+        self.sequences = [
+            ['transferOwnership(address)', 'acceptOwnership()']
+        ]
+        #0x2caf5a42ec2d6747ec696714bf913b174d94fdf0.sol	0.5.17	LexLocker
+        # contain GT, and function signature with 3 bytes
+        self.sequences = [
+            ['updateJudgmentReward(uint256)']
+        ]
+
+        if len(fdg.global_config.sequences)>0:
+            # assume that the sequenes are presented as string
+            self.sequences=ast.literal_eval(fdg.global_config.sequences)
+        else:self.sequences=[]
+
+        super().__init__('seq')
+
+    def initialize(self, main_path_sf: dict, main_path_df: dict, fdfg_manager: FWRG_manager):
+        ...
+
+
+
+
+
+    def termination(self, states_num: int = 0, current_seq_length: int = 0, sequence_depth_limit: int = 0,
+                    iteration: int = 0) -> bool:
+        # need to test
+        if states_num == 0: return True
+        if iteration>2:
+            if len(self.queue) == 0:
+                return True
+        return False
+
+    def assign_states(self, deep_functions: list = None, current_state_key: str = None, fdfg: FWRG_manager = None,
+                      states_dict: dict = {},iteration:int=0) -> list:
+        """
+
+        :param deep_functions:
+        :param current_state_key:
+        :param fdfg:
+        :param states_dict:
+        :return:
+        """
+        if len(states_dict)>0:
+            for key, states in states_dict.items():
+
+                if key not in self.world_states.keys():
+                    self.world_states[key]=deepcopy(states)
+                else:
+                    self.world_states[key]+=deepcopy(states)
+                self.queue.append(key)
+
+        while True:
+            if len(self.queue)==0: return {},False
+            state_key=self.queue.pop(0)
+            if state_key=='constructor':
+                if len(self.sequences)==0:
+                    return {},True
+                return {'constructor':[seq[0] for seq in self.sequences]},True
+
+            seq=get_ftn_seq_from_key_1(state_key)
+            functions=[]
+            for seq_ in self.sequences:
+                if len(seq)==len(seq_):continue
+                if len(seq)<len(seq_):
+                    for i in range(len(seq)):
+                        if seq[i]!=seq_[i]:break
+                    functions.append(seq_[len(seq)])
+            if len(functions)>0:
+                return {state_key:functions},True
+
+
+class DFS(FunctionSearchStrategy):
+    def __init__(self):
+        self.stack=[]
+        self.preprocess_timeout = False
+        self.preprocess_coverage = 0
+        self.flag_one_start_function=False
+        super().__init__('dfs')
+
+    def initialize(self, flag_one_start_function:bool, preprocess_timeout:bool, preprocess_coverage:float, all_functions:list, fwrg_manager:FWRG_manager):
+        self.flag_one_start_function=flag_one_start_function
+        self.preprocess_timeout = preprocess_timeout
+        self.preprocess_coverage = preprocess_coverage
+        self.functionAssignment=FunctionAssignment(all_functions,fwrg_manager)
+
+
+    def termination(self,states_num:int=0, current_seq_length: int = 0, sequence_depth_limit: int = 0,iteration:int=0)->bool:
+        if iteration<=2:
+            if states_num==0:return True
+        return False
+
+
+
+
+
+    def assign_states(self, deep_functions: list=None, states_dict: dict = {},iteration:int=0) -> list:
+
+        """
+            save states, push state keys to the stack
+            select a state by poping an item from the stack
+            assign functions to be executed on the selected state
+        :param deep_functions:
+        :param current_state_key:
+        :param fdfg:
+        :param states_dict:
+        :return:
+        """
+        if len(states_dict)>0:
+            for key, states in states_dict.items():
+                ftn_seq=get_ftn_seq_from_key_1(key)
+                if len(ftn_seq)>=fdg.global_config.seq_len_limit:
+                    continue # do not save these states as they will not be explored
+                # save states
+                self.world_states[key]=deepcopy(states)
+                self.stack.append(key)
+
+        print_data_for_dfs_strategy(self.stack)
+
+        if self.flag_one_start_function:
+            self.flag_one_start_function=False
+            state_key = self.stack.pop()
+            assign_functions = self.functionAssignment.assign_all_functions()
+
+            return {state_key : assign_functions},True
+
+        while True:
+            if len(self.stack)==0:
+                return {},None
+
+            state_key=self.stack.pop()
+
+            if self.preprocess_timeout or fdg.global_config.preprocessing_exception:
+                if self.preprocess_coverage<50:
+                    assigned_functions=self.functionAssignment.assign_functions_timeout(state_key,deep_functions, 7)
+                    if len(assigned_functions) > 0:
+                        return {state_key: assigned_functions},True
+                    continue
+                elif self.preprocess_coverage < 80:
+                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,deep_functions, 5)
+                    if len(assigned_functions) > 0:
+                        return {state_key: assigned_functions},True
+                    continue
+                else:
+                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,deep_functions, 3)
+                    if len(assigned_functions) > 0:
+                        return {state_key: assigned_functions},True
+                    continue
+            assigned_functions = self.functionAssignment.assign_functions(state_key,deep_functions)
+            if len(assigned_functions) > 0:
+                return {state_key: assigned_functions},True
+
+
+
+class BFS(FunctionSearchStrategy):
+    """
+    no need to save states
+    """
+    def __init__(self):
+        self.flag_one_start_function=False
+        self.preprocess_timeout = False
+        self.preprocess_coverage = 0
+        self.queue=[]
+        super().__init__('bfs')
+        pass
+
+    def initialize(self, flag_one_start_function:bool, preprocess_timeout:bool, preprocess_coverage:float, all_functions:list, fwrg_manager:FWRG_manager):
+        self.flag_one_start_function=flag_one_start_function
+        self.preprocess_timeout = preprocess_timeout
+        self.preprocess_coverage = preprocess_coverage
+        self.functionAssignment=FunctionAssignment(all_functions,fwrg_manager)
+
+    def termination(self,states_num:int=0, current_seq_length: int = 0, sequence_depth_limit: int = 0,iteration:int=0)->bool:
+        if iteration <= fdg.global_config.p1_dl+1:
+            if states_num == 0: return True
+        return False
+
+
+    def assign_states(self, dk_functions: list=None, current_state_key: str = None, fwrg: FWRG_manager = None,
+                      states_dict: dict = {},iteration:int=0) -> list:
+        """
+        assign functions for multiple states at the same time.
+        :param deep_functions:
+        :param current_state_key:
+        :param fwrg:
+        :param states_dict:
+        :return:
+        """
+
+        if len(states_dict) > 0:
+            for key, states in states_dict.items():
+                ftn_seq = get_ftn_seq_from_key_1(key)
+                if len(ftn_seq) >= fdg.global_config.seq_len_limit:
+                    continue  # do not save these states as they will not be explored
+                # save states
+                self.world_states[key] = deepcopy(states)
+                self.queue.append(key)
+
+            # # put key containing fallback at the end of the queue
+            # if len(ftn_seq)==1:
+            #     temp=[]
+            #     for item in self.queue:
+            #         if 'fallback' in item:
+            #             temp.append(item)
+            #         else:
+            #             temp=[item]+temp
+            #     self.queue=temp
+
+
+        print_data_for_bfs_strategy(self.queue)
+
+        if self.flag_one_start_function:
+            self.flag_one_start_function = False
+            state_key = self.queue.pop(0)
+            assign_functions = self.functionAssignment.assign_all_functions()
+
+            return {state_key: assign_functions},True
+
+
+        while True:
+            if len(self.queue) == 0:
+                return {},None
+
+            state_key = self.queue.pop(0)
+            if self.preprocess_timeout or  fdg.global_config.preprocessing_exception:
+                if self.preprocess_coverage < 50:
+                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,dk_functions, 7)
+                    if len(assigned_functions) > 0:
+                        return {state_key: assigned_functions},True
+                    continue
+                elif self.preprocess_coverage < 80:
+                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,dk_functions, 5)
+                    if len(assigned_functions) > 0:
+                        return {state_key: assigned_functions},True
+                    continue
+                else:
+                    assigned_functions = self.functionAssignment.assign_functions_timeout(state_key,dk_functions, 3)
+                    if len(assigned_functions) > 0:
+                        return {state_key: assigned_functions},True
+                    continue
+            assigned_functions = self.functionAssignment.assign_functions(state_key, dk_functions)
+            if len(assigned_functions) > 0:
+                return {state_key: assigned_functions},True
+
+
+
+class RandomBaseline(FunctionSearchStrategy):
+    """
+    no need to save states
+    """
+    def __init__(self,percent_of_functions:int,functions:list):
+        self.functionAssignment=FunctionAssignment(functions,None,select_percent=percent_of_functions)
+        self.flag_one_start_function=False
+        self.queue=[]
+        super().__init__('baseline')
+
+    def initialize(self, flag_one_start_function: bool):
+        self.flag_one_start_function = flag_one_start_function
+
+    def assign_states(self, dk_functions: list=None, states_dict: dict = {}) -> list:
+        """
+        apply BFS
+        :param dk_functions:
+        :param current_state_key:
+        :param fwrg:
+        :param states_dict:
+        :return:
+        """
+        if len(states_dict) > 0:
+            for key, states in states_dict.items():
+                ftn_seq = get_ftn_seq_from_key_1(key)
+                if len(ftn_seq) >= fdg.global_config.seq_len_limit:
+                    continue  # do not save these states as they will not be explored
+                # save states
+                self.world_states[key] = deepcopy(states)
+                self.queue.append(key)
+
+        print_data_for_bfs_strategy(self.queue)
+
+        if self.flag_one_start_function:
+            self.flag_one_start_function = False
+            state_key = self.queue.pop(0)
+            assign_functions = self.functionAssignment.assign_all_functions()
+
+            return {state_key: assign_functions}, True
+
+        while True:
+            if len(self.queue) == 0:
+                return {}, None
+
+            state_key = self.queue.pop(0)
+
+            assigned_functions =self.functionAssignment.assign_functions_for_baseline()
+            if len(assigned_functions) > 0:
+                return {state_key: assigned_functions}, True
+
+
+
+
+    def termination(self, states_num: int = None, current_seq_length: int = 0,
+                    sequence_depth_limit: int = 0,iteration:int=0) -> bool:
+
+        if iteration <= 1:
+            if states_num == 0: return True
+
+        return False
+
+
+
+
```

### Comparing `smartExecutorx-0.3/fdg/control/function_assignment.py` & `smartExecutorx-4.0/fdg/control/function_assignment.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/fdg/control/guider.py` & `smartExecutorx-4.0/fdg/control/guider.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,19 @@
         self.state_index=0 # used to form state keys
 
 
     def init(self, start_functions:list, depth_k_functions:list, preprocess:Preprocessing):
         fwrg_manager=FWRG_manager(start_functions, depth_k_functions, preprocess)
         if self.ftn_search_strategy.name in ['seq']:
             self.ftn_search_strategy.initialize(fwrg_manager.acyclicPaths.main_paths_sf, fwrg_manager.updateFWRG.main_paths_df, fwrg_manager)
-        elif self.ftn_search_strategy.name in ['mine','bfs','dfs','mine1']:
-            flag_one_state_depth1=True if len(start_functions)==1 else False
+        elif self.ftn_search_strategy.name in ['mine','bfs','dfs']:
+            flag_one_start_function=True if len(start_functions)==1 else False  #to-do: how to update flag_one_state_dpeht1
             if preprocess.coverage is None:
                 preprocess.coverage=0
-            self.ftn_search_strategy.initialize(flag_one_state_depth1,preprocess.timeout,preprocess.coverage,preprocess.write_read_info.all_functions,fwrg_manager)
+            self.ftn_search_strategy.initialize(flag_one_start_function,preprocess.timeout,preprocess.coverage,preprocess.write_read_info.all_functions,fwrg_manager)
 
 
 
     def organize_states(self, states:[WorldState]):
         all_states = {}
         for state in states:
             ftn_seq = get_ftn_seq_annotation_from_ws(state)
@@ -184,29 +184,32 @@
         self.termination=self.ftn_search_strategy.termination(
             states_num=len(laserEVM.open_states),
             current_seq_length=len_seq,
             sequence_depth_limit=fdg.global_config.seq_len_limit,
             iteration=iteration)
 
     def get_start_sequence(self,laserEVM:LaserEVM):
+        """
+        get the sequences used to annotate the states (world states) at the end of Phase 1
+        """
         state_chaning_seq = []
         for state in laserEVM.open_states:
             seq = get_ftn_seq_annotation_from_ws(state)
             if seq not in state_chaning_seq:
                 state_chaning_seq.append(seq)
         return state_chaning_seq
 
 
     def should_terminate(self):
         return self.termination
 
-    def save_genesis_states(self,states:list):
-        self.genesis_states=deepcopy(states)
-        if self.ftn_search_strategy.name in ['mine','mine1']:
-            states_dict=self.organize_states(states)
-            # if len(states_dict)>=2:
-            #     print('Check when two or more genesis states are generated (guider.py)')
-            self.ftn_search_strategy.update_states(states_dict)
-            self.ftn_search_strategy.state_key_assigned_at_last =list(states_dict.keys())[0]
+    # def save_genesis_states(self,states:list):
+    #     self.genesis_states=deepcopy(states)
+    #     if self.ftn_search_strategy.name in ['mine']:
+    #         states_dict=self.organize_states(states)
+    #         # if len(states_dict)>=2:
+    #         #     print('Check when two or more genesis states are generated (guider.py)')
+    #         self.ftn_search_strategy.update_states(states_dict)
+    #         self.ftn_search_strategy.state_key_assigned_at_last =list(states_dict.keys())[0]
```

### Comparing `smartExecutorx-0.3/fdg/control/weight_computation.py` & `smartExecutorx-4.0/fdg/control/weight_computation.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/fdg/expression_slot.py` & `smartExecutorx-4.0/fdg/expression_slot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,187 +1,183 @@
-import re
-
-from fdg.output_data import my_print
-from fdg.utils import str_without_space_line
-from mythril.laser.smt import BitVec
-from z3 import  Z3Exception
-
-"""
-extract the storage locations from Concat() expressions, condition expressions, and (not know yet)
-
-observation: the expression can be extracted multiple times, so, saving the extracted results
-On HoloToken.sol: before saving the results: 28 times
-after saving the results: 6
-
-
-"""
-
-
-max_length=10000
-expression_str_to_slot_normal={} # used in the normal execution process
-
-def map_concrete_hash_key_to_slot_normal(expression:BitVec, data:BitVec):
-    """
-    pplied in create_keccak(self, data: BitVec) n keccak_function_manager.py module
-    """
-    if not expression.symbolic:
-        expr_str = str_without_space_line(expression)
-        data_str=str_without_space_line(data)
-        if expr_str not in expression_str_to_slot_normal.keys():
-            if data_str in expression_str_to_slot_normal.keys():
-                final_data_str=expression_str_to_slot_normal[data_str]
-                expression_str_to_slot_normal[expr_str] = final_data_str
-                # print(f'map: {expr_str}')
-                # print(f'to: {final_data_str}')
-            else:
-                expression_str_to_slot_normal[expr_str] = data_str
-                # print(f'map: {expr_str}')
-                # print(f'to: {data_str}')
-
-
-def identify_slot_from_symbolic_slot_expression(concat_expr: BitVec) -> str:
-    """
-    get the locations of storage from expressions:
-        Concat(0,x,location)
-        keccak256_512(Concat(0,x,location))
-        need to think about the case of array
-
-    also consider the case of concrete hash, the location info is collected in a place where it is created.
-    """
-
-    def map_expr_str_to_slot(expr_str:str)->str:
-        matched_expr = find_matched_expr(expr_str,
-                                         expression_str_to_slot_normal.keys())
-        if matched_expr is not None:
-            temp = expression_str_to_slot_normal[matched_expr]
-            if temp in expression_str_to_slot_normal.keys():
-                return expression_str_to_slot_normal[temp]
-            else:
-                return temp
-
-        slot = expr_str
-        # save the result
-        if expr_str not in expression_str_to_slot_normal.keys():
-            expression_str_to_slot_normal[expr_str] = slot
-        return slot
-
-    def find_matched_expr(expr:str, expr_list:list)->str:
-        if len(expr)>=10:
-            expr_prefix=expr[0:len(expr)-2]
-            for e in expr_list:
-                if str(e[0:len(e)-2]).__eq__(expr_prefix):
-                    return e
-            return None
-        else:
-            if expr in expr_list:
-                return expr
-            else:
-                return None
-
-    if isinstance(concat_expr,BitVec):
-        if not concat_expr.symbolic:
-            expr_str = str_without_space_line(concat_expr)
-            # check if it is already considered once
-            return map_expr_str_to_slot(expr_str)
-
-    if isinstance(concat_expr, str):
-        if concat_expr.isdigit():
-            return map_expr_str_to_slot(concat_expr)
-
-    str_data = str_without_space_line(concat_expr)
-    if len(str_data)>=max_length:
-        # print(f'reach max length')
-        return ""
-
-    # handle the case: 62514009886607029107290561805838585334079798074568712924583230797734656856475 +
-    # Concat(If(1_calldatasize <= 4, 0, 1_calldata[4]),
-    if str_data.count('+')==1:
-        items=str_data.split('+')
-        if items[0].isdigit() and len(items[0])>=10:
-            return map_expr_str_to_slot(items[0])
-        else:
-            str_data=items[1]
-
-
-    last_parameter = ""
-    try:
-
-        # handle the case below:
-        # 1+keccak256_512(Concat(If(1_calldatasize<=4...)
-        # 2+keccak256_512(Concat(If(1_calldatasize<=4...)
-        pattern = r"^(\d+\+)\w+"
-        results = re.search(pattern, str_data)
-        if results:
-            # get the str that
-            str_data = str_data.split(results.group(1))[-1]
-
-        # check if it is already considered once
-        if str_data in expression_str_to_slot_normal.keys():
-            last_parameter = expression_str_to_slot_normal[str_data]
-        else:
-            if str_data.startswith('keccak256_512'):
-                # Use regular expressions to find the last parameter within the keccak256_512 function
-                last_parameter = re.search(r'keccak256_512\(.*?,(\d+)\)',
-                                           str_data)
-            else:
-                # Use regular expressions to find the last parameter within the Concat function
-                last_parameter = re.search(r'Concat\(.*?,(\d+)\)', str_data)
-
-            if last_parameter is not None:
-                last_parameter = last_parameter.group(1)
-                # print(f'(new) exp:{str_data}')
-                # print(f'(new) slot:{last_parameter}')
-                # save the result
-                expression_str_to_slot_normal[str_data] = str(last_parameter)
-            else:
-                # print(f'Failed to identify a slot from {concat_expr}')
-                last_parameter=""
-
-    except Z3Exception as ze:
-        print(f'Have Z3Exception: {concat_expr}')
-    finally:
-        return last_parameter
-
-
-
-def is_slot_in_a_list(slot, slot_list: list) -> bool:
-    """
-    pay special attention to slot that is symbolic. need to find the original slot, i.e., where the dynamic state variable is declared
-    """
-    if slot.symbolic:
-        slot_str = identify_slot_from_symbolic_slot_expression(slot)
-
-        if len(slot_str) == 0:
-            my_print(f'slot_str:{slot_str}')
-            my_print(
-                f'Check why original slot can not be identified for {slot}.')
-            return False
-    else:
-        slot_str = str(slot)
-
-    slot_str_list = [identify_slot_from_symbolic_slot_expression(s) for s in slot_list]
-
-    my_print(f'is slot {slot_str} in slots {slot_str_list}?')
-    if slot_str in slot_str_list:
-        my_print(f'\t yes')
-        return True
-    else:
-        my_print(f'\t no')
-        return False
-
-
-def common_elements(lst_1:list,lst_2_str:list)->list:
-    lst_1_str = [identify_slot_from_symbolic_slot_expression(s) for s in
-                     lst_1]
-
-    my_print(f'\tread slots:{lst_1_str}')
-
-    common_ele=[]
-    for ele in lst_1_str:
-        if ele in lst_2_str:
-            common_ele.append(ele)
-    return common_ele
-
-
-
-
-
+import re
+
+from fdg.output_data import my_print
+from fdg.utils import str_without_space_line
+from mythril.laser.smt import BitVec
+from z3 import  Z3Exception
+
+"""
+extract the storage locations from Concat() expressions, condition expressions, and (not know yet)
+
+observation: the expression can be extracted multiple times, so, saving the extracted results
+On HoloToken.sol: before saving the results: 28 times
+after saving the results: 6
+
+
+"""
+
+
+max_length=10000
+expression_str_to_slot_normal={} # used in the normal execution process
+
+def map_concrete_hash_key_to_slot_normal(expression:BitVec, data:BitVec):
+    """
+    pplied in create_keccak(self, data: BitVec) n keccak_function_manager.py module
+    """
+    if not expression.symbolic:
+        expr_str = str_without_space_line(expression)
+        data_str=str_without_space_line(data)
+        if expr_str not in expression_str_to_slot_normal.keys():
+            if data_str in expression_str_to_slot_normal.keys():
+                final_data_str=expression_str_to_slot_normal[data_str]
+                expression_str_to_slot_normal[expr_str] = final_data_str
+                # print(f'map: {expr_str}')
+                # print(f'to: {final_data_str}')
+            else:
+                expression_str_to_slot_normal[expr_str] = data_str
+                # print(f'map: {expr_str}')
+                # print(f'to: {data_str}')
+
+
+def identify_slot_from_symbolic_slot_expression(concat_expr: BitVec) -> str:
+    """
+    get the locations of storage from expressions:
+        Concat(0,x,location)
+        keccak256_512(Concat(0,x,location))
+        need to think about the case of array
+
+    also consider the case of concrete hash, the location info is collected in a place where it is created.
+    """
+
+    def map_expr_str_to_slot(expr_str:str)->str:
+        matched_expr = find_matched_expr(expr_str,
+                                         expression_str_to_slot_normal.keys())
+        if matched_expr is not None:
+            temp = expression_str_to_slot_normal[matched_expr]
+            if temp in expression_str_to_slot_normal.keys():
+                return expression_str_to_slot_normal[temp]
+            else:
+                return temp
+
+        slot = expr_str
+        # save the result
+        if expr_str not in expression_str_to_slot_normal.keys():
+            expression_str_to_slot_normal[expr_str] = slot
+        return slot
+
+    def find_matched_expr(expr:str, expr_list:list)->str:
+        if len(expr)>=10:
+            expr_prefix=expr[0:len(expr)-2]
+            for e in expr_list:
+                if str(e[0:len(e)-2]).__eq__(expr_prefix):
+                    return e
+            return None
+        else:
+            if expr in expr_list:
+                return expr
+            else:
+                return None
+
+    if isinstance(concat_expr,BitVec):
+        if not concat_expr.symbolic:
+            expr_str = str_without_space_line(concat_expr)
+            # check if it is already considered once
+            return map_expr_str_to_slot(expr_str)
+
+    if isinstance(concat_expr, str):
+        if concat_expr.isdigit():
+            return map_expr_str_to_slot(concat_expr)
+
+    str_data = str_without_space_line(concat_expr)
+    if len(str_data)>=max_length:
+        # print(f'reach max length')
+        return ""
+
+    # handle the case: 62514009886607029107290561805838585334079798074568712924583230797734656856475 +
+    # Concat(If(1_calldatasize <= 4, 0, 1_calldata[4]),
+    if str_data.count('+')==1:
+        items=str_data.split('+')
+        if items[0].isdigit() and len(items[0])>=10:
+            return map_expr_str_to_slot(items[0])
+        else:
+            str_data=items[1]
+
+
+    last_parameter = ""
+    try:
+
+        # handle the case below:
+        # 1+keccak256_512(Concat(If(1_calldatasize<=4...)
+        # 2+keccak256_512(Concat(If(1_calldatasize<=4...)
+        pattern = r"^(\d+\+)\w+"
+        results = re.search(pattern, str_data)
+        if results:
+            # get the str that
+            str_data = str_data.split(results.group(1))[-1]
+
+        # check if it is already considered once
+        if str_data in expression_str_to_slot_normal.keys():
+            last_parameter = expression_str_to_slot_normal[str_data]
+        else:
+            if str_data.startswith('keccak256_512'):
+                # Use regular expressions to find the last parameter within the keccak256_512 function
+                last_parameter = re.search(r'keccak256_512\(.*?,(\d+)\)',
+                                           str_data)
+            else:
+                # Use regular expressions to find the last parameter within the Concat function
+                last_parameter = re.search(r'Concat\(.*?,(\d+)\)', str_data)
+
+            if last_parameter is not None:
+                last_parameter = last_parameter.group(1)
+                # print(f'(new) exp:{str_data}')
+                # print(f'(new) slot:{last_parameter}')
+                # save the result
+                expression_str_to_slot_normal[str_data] = str(last_parameter)
+            else:
+                # print(f'Failed to identify a slot from {concat_expr}')
+                last_parameter=""
+
+    except Z3Exception as ze:
+        print(f'Have Z3Exception: {concat_expr}')
+    finally:
+        return last_parameter
+
+
+
+def is_slot_in_a_list(slot, slot_list: list) -> bool:
+    """
+    pay special attention to slot that is symbolic. need to find the original slot, i.e., where the dynamic state variable is declared
+    """
+    if slot.symbolic:
+        slot_str = identify_slot_from_symbolic_slot_expression(slot)
+
+        if len(slot_str) == 0:
+            my_print(f'slot_str:{slot_str}')
+            my_print(
+                f'Check why original slot can not be identified for {slot}.')
+            return False
+    else:
+        slot_str = str(slot)
+
+    slot_str_list = [identify_slot_from_symbolic_slot_expression(s) for s in slot_list]
+
+    my_print(f'is slot {slot_str} in slots {slot_str_list}?')
+    if slot_str in slot_str_list:
+        my_print(f'\t yes')
+        return True
+    else:
+        my_print(f'\t no')
+        return False
+
+
+def common_elements(lst_1_str:list,lst_2_str:list)->list:
+
+    common_ele=[]
+    for ele in lst_1_str:
+        if ele in lst_2_str:
+            common_ele.append(ele)
+    return common_ele
+
+
+
+
+
```

### Comparing `smartExecutorx-0.3/fdg/fdg_pruner.py` & `smartExecutorx-4.0/fdg/fdg_pruner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 # support FDG-guided execution and sequence execution
-from fdg.control.mine import Mine, Mine1
+from fdg.control.mine import Mine
 from fdg.preprocessing.address_collection import collect_addresses_in_constructor
 
 from fdg.control.ftn_search_strategy import BFS, RandomBaseline, DFS, Seq
 from fdg.control.guider import Guider
 
 from fdg.function_coverage import FunctionCoverage
 
 from fdg.preprocessing.preprocess import Preprocessing
-from fdg.constraint_check import state_constraints_hash_check
+
 
 from mythril.laser.ethereum.state.world_state import WorldState
 from mythril.laser.ethereum.svm import LaserEVM
 from mythril.laser.plugin.interface import LaserPlugin
 from mythril.laser.plugin.builder import PluginBuilder
 from mythril.laser.plugin.plugins.coverage import InstructionCoveragePlugin
 from mythril.laser.ethereum.state.global_state import GlobalState
@@ -39,15 +39,15 @@
 
 
 class FDG_pruner(LaserPlugin):
     """ """
     def __init__(self,instructionCoveragePlugin:InstructionCoveragePlugin):
         """Creates FDG pruner"""
         self._reset()
-        self.functionCoverage=FunctionCoverage(instructionCoveragePlugin )
+        self.functionCoverage=FunctionCoverage(instructionCoveragePlugin)
 
     def _reset(self):
         self._iteration_ = 0
 
         self.state_hash_check=None
         self.preprocess=None
         self.condi_cov=None
@@ -56,16 +56,14 @@
         if fdg.global_config.random_baseline>0:
             self.search_stragety = RandomBaseline(fdg.global_config.random_baseline,
                                                   fdg.global_config.method_identifiers)
         elif fdg.global_config.function_search_strategy=='dfs':
             self.search_stragety=DFS()
         elif fdg.global_config.function_search_strategy=='mine':
             self.search_stragety=Mine()
-        elif fdg.global_config.function_search_strategy=='mine1':
-            self.search_stragety=Mine1()
         elif fdg.global_config.function_search_strategy=='seq':
             self.search_stragety=Seq()
         else:
             self.search_stragety = Mine()
 
         self.guider=Guider(self.search_stragety,list(fdg.global_config.method_identifiers.keys()))
 
@@ -78,16 +76,17 @@
         :param symbolic_vm
         """
         self._reset()
 
         @symbolic_vm.laser_hook("start_sym_exec")
         def start_sym_exec_hook():
 
-            # for saving the generated states and executed sequences
-            self.state_hash_check=state_constraints_hash_check()
+            # # for saving the generated states and executed sequences
+            # self.state_hash_check=state_constraints_hash_check()
+            pass
 
 
         @symbolic_vm.laser_hook("stop_sym_exec")
         def stop_sym_exec_hook():
             if fdg.global_config.random_baseline>0:return
             # if not fdg.global_config.flag_preprocess_timeout:
             #     if not fdg.global_config.preprocessing_exception:
@@ -135,160 +134,134 @@
 
                 # it means no contract is deployed as no valid contracts are given
                 if isinstance(fdg.global_config.contract_address,str): return
 
                 self.guider.instructionModification.feed_instructions(
                     laserEVM.open_states[0], fdg.global_config.contract_address)
 
-                self.guider.save_genesis_states(laserEVM.open_states)
+                # self.guider.save_genesis_states(laserEVM.open_states) # to-do: think about removing it
                 self.get_runtime_bytecode(laserEVM.open_states[0],fdg.global_config.contract_address)
 
 
-            if fdg.global_config.random_baseline>0 :
-                self.guider.start_iteration(
-                    laserEVM=laserEVM, deep_functions=None, iteration=self._iteration_)
-
-                return
 
             if self._iteration_==1:
-                # do preprocessing
+                # create a Preprocessing instance
                 self.preprocess = Preprocessing(fdg.global_config.method_identifiers,
                                                 laserEVM.open_states[0],
                                                 fdg.global_config.contract_address)
 
+                # do preprocessing
                 self.preprocess.main_preprocessing_start(self._iteration_, laserEVM)
                 return
 
             else:
-
-                if self._iteration_==2:
-                    # prepare for the execution in depth 1
-                    self.guider.start_iteration(laserEVM=laserEVM,iteration=self._iteration_)
-                    # self.condi_cov=ConditionCoverage(self.preprocess)
+                if self._iteration_<=fdg.global_config.p1_dl+1:
+                    # Phase 1
+                    ...
                 else:
+                    # Phase 2
                     self.get_depth_k_functions()
-                    self.guider.start_iteration(laserEVM, self.depth_k, self._iteration_)
-                    flag_terminate=self.guider.should_terminate()
+                    self.guider.start_iteration(laserEVM, self.depth_k,
+                                                self._iteration_)
+                    flag_terminate = self.guider.should_terminate()
                     if flag_terminate:
-                        fdg.global_config.transaction_count=self._iteration_
-                        laserEVM.open_states=[]
-
+                        fdg.global_config.transaction_count = self._iteration_
+                        laserEVM.open_states = []
 
         @symbolic_vm.laser_hook("stop_sym_trans_laserEVM")
         def stop_sym_trans_hook_laserEVM(laserEVM: LaserEVM):
             """
             - save states
             - some saved states are used as initial states in sequence execution
 
             :param laserEVM:
             :return:
             """
             log.info(f'\n----------------------------------------')
             log.info(f'end: self._iteration_={self._iteration_}')
 
-            if fdg.global_config.random_baseline>0 :
-                # prune unfeasible states
-                old_states_count = len(laserEVM.open_states)
-                laserEVM.open_states = [
-                    state for state in laserEVM.open_states if state.constraints.is_possible
-                ]
-                prune_count = old_states_count - len(laserEVM.open_states)
-                if prune_count: log.info("Pruned {} unreachable states".format(prune_count))
-
-                # compute coverage
-                self.functionCoverage.compute_contract_coverage(fdg.global_config.target_runtime_bytecode)
-                self.functionCoverage.print_coverage()
-
-
-                # check at the end of iteration
-                self.guider.end_iteration(laserEVM,self._iteration_)
-                flag_terminate=self.guider.should_terminate()
-                if flag_terminate:
-                    fdg.global_config.transaction_count=self._iteration_
-
-                if self._iteration_==1 and len(laserEVM.open_states) == 1:
-                    # in case that there are one state
-                    self.search_stragety.initialize(True)
-
-                # termination based on the coverage of the contract
-                if self.functionCoverage.coverage >= fdg.global_config.function_coverage_threshold:
-                    if not self.search_stragety.flag_one_state_at_depth1:
-                        fdg.global_config.transaction_count = self._iteration_
-
-                return
-
-
             #++++++++++++++++++++++++++++++++++++++++++++++++++
             if self.preprocess is None: return
 
             # collect results at the end of preprocessing
             if self._iteration_==1:
                 self.preprocess.main_preprocessing_end(self._iteration_)
-                self.functionCoverage.feed_function_indices(
+                self.functionCoverage.feed_function_intruction_indices(
                     self.preprocess.instruction_cov.function_instruction_indices)
                 self.functionCoverage.set_runtime_bytecode(fdg.global_config.target_runtime_bytecode)
                 return
 
 
             #----------------------------------------
-            # end of normal symbolic execution
+            # at the end of each iteration in the normal symbolic execution
             # prune unfeasible states
             old_states_count = len(laserEVM.open_states)
             laserEVM.open_states = [
                 state for state in laserEVM.open_states if state.constraints.is_possible
             ]
             prune_count = old_states_count - len(laserEVM.open_states)
             if prune_count: log.info("Pruned {} unreachable states".format(prune_count))
 
 
             # compute coverage
             self.functionCoverage.compute_coverage()
             self.functionCoverage.print_coverage()
 
-            if self._iteration_==2:
+            if self._iteration_ == 2:
+                # at iteration 2 (i.e., at the end of depth 1)
                 if len(laserEVM.open_states) == 0:
                     print('No states are generated at depth 1.')
-                # initialize fdfg manager
+                    # terminate
+                    fdg.global_config.transaction_count = self._iteration_
+                    return
+
+            if self._iteration_<=fdg.global_config.p1_dl:
+                # the basic symbolic execution
+                ...
+
+            elif self._iteration_==fdg.global_config.p1_dl+1:
+                # call init() of self.guider so that it can prepare to guide
                 self.guider.end_iteration(laserEVM,self._iteration_)
                 sequences=self.guider.get_start_sequence(laserEVM)
+
                 flag_termination=self.guider.should_terminate()
                 if flag_termination:
                     fdg.global_config.transaction_count=self._iteration_
                     return
-                if self.search_stragety.name in ['bfs','dfs','mine','mine1']:
+                if self.search_stragety.name in ['bfs','dfs','mine']:
                     self.get_depth_k_functions()
                     start_functions = [seq[-1] for seq in sequences if len(seq)>0 ]
                     start_functions = list(set(start_functions))
                     self.guider.init(start_functions,self.depth_k,self.preprocess)
 
 
             else:
-
+                # belong to Phase 2
                 self.guider.end_iteration(laserEVM,self._iteration_)
 
             flag_termination=self.guider.should_terminate()
             if flag_termination:
                 fdg.global_config.transaction_count = self._iteration_
 
 
             # # termination based on deep functions(not appropriate when timeout can happen in preprocessing as the instructions of functions can not be correctly obtained)
             # self.get_depth_k_functions()            #
             # if len(self.depth_k) ==0:
             #     fdg.global_config.transaction_count = self._iteration_
 
             # termination based on the coverage of the contract
             if self.functionCoverage.coverage>=fdg.global_config.function_coverage_threshold:
-                if self.search_stragety.name in ['mine', 'mine1']:
+                if self.search_stragety.name in ['mine']:
                     if self.functionCoverage.coverage>=fdg.global_config.function_coverage_threshold+1:
-                        if not self.search_stragety.flag_one_state_at_depth1:
+                        if not self.search_stragety.flag_one_start_function:
                             # make sure that when there is only one state generated at depth1,
                             # the execution does not terminate
                             fdg.global_config.transaction_count = self._iteration_
                 else:
-                    if not self.search_stragety.flag_one_state_at_depth1:
+                    if not self.search_stragety.flag_one_start_function:
                         # make sure that when there is only one state generated at depth1,
                         # the execution does not terminate
                         fdg.global_config.transaction_count = self._iteration_
 
         # record the instructions visited
         @symbolic_vm.laser_hook("preprocessing_execute_state")
         def execute_state_hook(global_state: GlobalState,opcode:str):
```

### Comparing `smartExecutorx-0.3/fdg/function_coverage.py` & `smartExecutorx-4.0/fdg/function_coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
         self.contract_bytecode='' # the bytecode of the contract that is used to retrieve the instruction coverage status from the coverage plugin
 
         self.function_coverage={}
         self.coverage=0
         self.deep_functions=[]
         self.deep_functions_1st_time = []  # record how many deep functions are there
 
-    def feed_function_indices(self,function_indices:dict):
-        self.function_instruction_indices=function_indices
+    def feed_function_intruction_indices(self, function_instruction_indices:dict):
+        self.function_instruction_indices=function_instruction_indices
         # initialize coverage for each function except constructor
         for ftn, ftn_instr_list in self.function_instruction_indices.items():
             # if ftn=='constructor' or ftn=='fallback':continue
             if ftn == 'constructor': continue
             if len(ftn_instr_list)==0:continue
             self.function_coverage[ftn] = 0 / len(ftn_instr_list)
```

### Comparing `smartExecutorx-0.3/fdg/fwrg_manager.py` & `smartExecutorx-4.0/fdg/fwrg_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,372 +1,372 @@
-from copy import copy, deepcopy
-
-import fdg.global_config
-
-from fdg.output_data import output_fwrg_data
-from fdg.preprocessing.preprocess import Preprocessing
-
-class FWRG():
-    def __init__(self,ftn_reads_in_condition:dict,ftn_writes:dict):
-        self.ftn_reads_in_condition = ftn_reads_in_condition
-        self.ftn_writes = ftn_writes
-        self.fwrg_dict={}
-        self.frwg_dict={}
-
-        self._generate_fwrg()
-        self._generate_frwg()
-
-    def _generate_fwrg(self):
-        for ftn,writes in self.ftn_writes.items():
-            if len(writes)==0:
-                self.fwrg_dict[ftn]={}
-                continue
-
-            children={}
-            for ftn_read,reads in self.ftn_reads_in_condition.items():
-                for write in writes:
-                    if write in reads:
-                        if ftn_read not in children.keys():
-                            children[ftn_read]=[write]
-                        else:
-                            children[ftn_read]+=[write]
-            self.fwrg_dict[ftn]=children
-
-    def _generate_frwg(self):
-        for ftn, reads in self.ftn_reads_in_condition.items():
-            if len(reads)==0:
-                self.frwg_dict[ftn]={}
-                continue
-            for ftn_write,writes in self.ftn_writes.items():
-                for read in reads:
-                    if read in writes:
-                        if ftn not in self.frwg_dict.keys():
-                            self.frwg_dict[ftn]=[ftn_write]
-                        else:
-                            if ftn_write not in self.frwg_dict[ftn]:
-                                self.frwg_dict[ftn]+=[ftn_write]
-                        break
-
-    def get_reads_in_conditions(self,ftn_name:str):
-        if ftn_name in self.ftn_reads_in_condition.keys():
-            return self.ftn_reads_in_condition[ftn_name]
-        else:return []
-
-class AcyclicPath():
-    def __init__(self, start_functions:list, dk_functions:list, fwrg:FWRG):
-        self.path_len_limit = fdg.global_config.seq_len_limit
-        self.fwrg=fwrg
-        self.start_functions=start_functions
-        self.dk_functions=[ftn for ftn,_ in dk_functions]
-
-        self.paths = {}
-        self._get_path()
-        self.paths_df={}
-        self.organize_paths()
-
-    def _get_path(self):
-        """
-        get all acyclic paths from starting functions (bounded by sequence length)
-        :return:
-        """
-        def get_children(ftn:str):
-            if ftn in self.fwrg.fwrg_dict.keys():
-                children=self.fwrg.fwrg_dict[ftn]
-                if len(children)>0:
-                    return list(children.keys())
-            return []
-        def derive_paths(start_ftn:str):
-            all_paths=[]
-            paths=[[start_ftn]]
-            for i in range(self.path_len_limit-1):
-                derived_paths=[]
-                for path in paths:
-                    children=get_children(path[-1])
-                    if len(children)==0:
-                        if path not in all_paths:
-                            all_paths.append(path)
-                    else:
-                        for child in children:
-                            if child in path:
-                                # think of the case [A(),A()](self dependency)
-                                if child==path[0] and len(path)==1:
-                                    path.append(child)
-                                if path not in all_paths:
-                                    all_paths.append(path)
-                            else:
-                                derived_paths.append(path+[child])
-                paths=derived_paths
-
-            all_paths+=paths
-            return all_paths
-
-
-        for sf in self.start_functions:
-            sf_path=derive_paths(sf)
-            self.paths[sf]=sf_path
-
-    def organize_paths(self):
-        for paths in self.paths.values():
-            for path in paths:
-                for idx,ftn in enumerate(path):
-                    if ftn in self.dk_functions and idx>0:# deep function can not be the frist function in a sequence
-                        t_path=path[0:idx+1]
-                        # add t_path
-                        if ftn not in self.paths_df.keys():
-                            self.paths_df[ftn]={}
-                        if len(t_path)-1 not in self.paths_df[ftn].keys():
-                            self.paths_df[ftn][len(t_path)-1]=[t_path]
-                        else:
-                            if t_path not in self.paths_df[ftn][len(t_path)-1]:
-                                self.paths_df[ftn][len(t_path)-1] += [t_path]
-
-class UpdateFWRG():
-    def __init__(self, fdg:FWRG, paths:AcyclicPath):
-        self.fwrg=fdg
-        self.acyclicPaths=paths
-
-        self.fwrg_targets={}
-
-        self.construct_fwrg_targets()
-
-        self.print_graphs(self.fwrg_targets,'fwrg_targets_data.txt')
-
-        self.fwrg_targets_augmented=deepcopy(self.fwrg_targets)
-        self.add_edges_1()
-        self.print_graphs(self.fwrg_targets_augmented,'fwrg_targets_augmented_data_update.txt')
-
-        self.dk_not_reachable=[]
-        self.identity_dk_function_not_reachable()
-
-    def print_graphs(self,data:dict,file_name:str):
-        output_fwrg_data(data, file_name, 'funtion write-read graph data')
-
-
-    def add_edge_to_graph(self,from_:str,to_:str):
-        if from_ in self.fwrg_targets_augmented.keys():
-            if to_ not in self.fwrg_targets_augmented[from_]:
-                self.fwrg_targets_augmented[from_].append(to_)
-        else:
-            self.fwrg_targets_augmented[from_]=[to_]
-
-
-    def construct_fwrg_targets(self):
-        # reconstruct edges from given acyclic paths
-        for value in self.acyclicPaths.paths_df.values():
-            if not isinstance(value,dict):continue
-            for paths in value.values():
-                for path in paths:
-                    # add edges
-                    for i in range(len(path) - 1):
-                        if path[i] not in self.fwrg_targets.keys():
-                            self.fwrg_targets[path[i]] = [path[i + 1]]
-                        else:
-                            if path[i+1] not in self.fwrg_targets[path[i]]:
-                                self.fwrg_targets[path[i]] += [path[i + 1]]
-
-
-
-    def add_edges_1(self):
-        """
-        for each deep function, add edges to connect some of its paths
-
-        for each deep function, try to find a combined path
-        :return:
-        """
-        def belong_relation(seq1:list,seq2:list):
-            s1=seq1
-            s2=seq2
-            if len(seq1)>len(seq2):
-                s1=seq2
-                s2=seq1
-            if [True for e in s1 if e not in s2].count(True)>0:
-                return False
-            else:
-                return True
-
-        def common_elements(seq1: list, seq2: list):
-            common=[]
-            s1 = seq1
-            s2 = seq2
-            if len(seq1) > len(seq2):
-                s1 = seq2
-                s2 = seq1
-            for e in s1:
-                if e in s2:
-                    common.append(e)
-            return common
-
-        def find_edges(seq1: list, seq2: list, common: list):
-            edges = []
-            s1 = seq1
-            s2 = seq2
-            if len(seq1) > len(seq2):
-                s1 = seq2
-                s2 = seq1
-
-            f1 = -1
-            t1 = -1
-            f2 = -1
-            t2 = -1
-            idx2 = 0
-            for idx, e in enumerate(s1):
-                if e not in common:
-                    if t1 == -1:
-                        t1 = idx
-                    f1 = idx
-                else:
-
-                    # check s2 if there are elements before e
-                    for i in range(idx2, len(s2)):
-                        if not s2[i] == e:
-                            if t2 == -1:
-                                t2 = i
-                            f2 = i
-                        else:
-
-                            break
-
-                    if f2 >= 0 and t2 >= 0 and t1 >= 0 and f1 >= 0:
-                        edges.append((s2[f2], s1[t1]))
-                        edges.append((s1[f1], s2[t2]))
-
-                    idx2 = i + 1
-                    f1 = f2 = t1 = t2 = -1
-                    continue
-
-            if t1 >= 0 and f1 >= 0:
-                if idx2 > len(s2) - 1:
-                    return edges
-                for i in range(idx2, len(s2)):
-                    if not s2[i] == e:
-                        if t2 == -1:
-                            t2 = i
-                        f2 = i
-                    else:
-                        break
-                if f2 >= 0 and t2 >= 0:
-                    edges.append((s2[f2], s1[t1]))
-                    edges.append((s1[f1], s2[t2]))
-
-            return edges
-        for df,value in self.acyclicPaths.paths_df.items():
-
-            if isinstance(value,dict):
-                sequences=[]
-                for seq_list in value.values():
-                    for seq in seq_list:
-                        sequences.append(seq[0:-1])
-
-                all_pairs=[(a,b) for idx,a in enumerate(sequences) for b in sequences[idx+1:]]
-
-                for seq1,seq2 in all_pairs:
-                    if belong_relation(seq1, seq2):
-                        # do not add edges
-                        continue
-                    common = common_elements(seq1, seq2)
-                    if len(common) == 0:
-                        # add edges
-                        self.add_edge_to_graph(seq1[-1], seq2[0])
-                        self.add_edge_to_graph(seq2[-1], seq1[0])
-
-                    else:
-                        edges=find_edges(seq1, seq2, common)
-                        for f,t in edges:
-                            self.add_edge_to_graph(f, t)
-
-    def identity_dk_function_not_reachable(self):
-        for dk in self.acyclicPaths.dk_functions:
-            if dk not in self.acyclicPaths.paths_df.keys():
-                self.dk_not_reachable.append(dk)
-                print(f'{dk} is not reachable')
-            else:
-                if len(self.acyclicPaths.paths_df[dk])==0:
-                    self.dk_not_reachable.append(dk)
-                    print(f'{dk} is not reachable')
-
-class FWRG_manager():
-    def __init__(self, start_functions:list, dk_functions:list, preprocess:Preprocessing):
-        self.fwrg=FWRG(preprocess.read_in_conditions.read_slots_in_conditions,
-                       preprocess.write_read_info.write_slots)
-        self.fwrg_all_reads={}
-        self.generate_graph_all_reads(preprocess.write_read_info.write_slots,preprocess.write_read_info.read_slots)
-
-        self.acyclicPaths=AcyclicPath(start_functions, dk_functions, self.fwrg)
-        self.updateFWRG=UpdateFWRG(self.fwrg, self.acyclicPaths)
-
-    def generate_graph_all_reads(self,writes:dict,all_reads:dict):
-        for ftn,writes in writes.items():
-            if len(writes)==0:
-                self.fwrg_all_reads[ftn]={}
-                continue
-            children={}
-            for ftn_read,reads in all_reads.items():
-                for write in writes:
-                     if write in reads:
-                         if ftn_read not in children.keys():
-                             children[ftn_read]=[write]
-                         else:
-                             children[ftn_read]+=[write]
-            self.fwrg_all_reads[ftn]=children
-                
-    def get_children_all_reads(self,ftn:str):
-        if ftn in self.fwrg_all_reads.keys():
-            return list(self.fwrg_all_reads[ftn].keys())
-        else:
-            return []
-    def get_children_fwrg(self,ftn:str):
-        if ftn in self.fwrg.fwrg_dict.keys():
-            return list(self.fwrg.fwrg_dict[ftn])
-        else:
-            return []
-
-    def get_children_fwrg_T_A(self, ftn:str)->list:
-        if ftn in self.updateFWRG.fwrg_targets_augmented.keys():
-            return self.updateFWRG.fwrg_targets_augmented[ftn]
-        else: return []
-
-    def get_parents_frwg(self, ftn:str)->list:
-        if ftn in self.fwrg.frwg_dict.keys():
-            return self.fwrg.frwg_dict[ftn]
-        else:
-            return []
-
-    def get_children_bf_update(self, ftn:str)->list:
-        if ftn in self.updateFWRG.fwrg_targets.keys():
-            return self.updateFWRG.fwrg_targets[ftn]
-        else: return []
-
-
-
-
-
-
-
-
-def test_1():
-    ftn_r_in_condi = {'f2': ['a'], 'f3': ['b'], 'f4': ['c'], 'f5': ['c']}
-    ftn_w = {'f2': ['b'], 'f3': ['a', 'c'], 'f4': [], 'f5': []}
-    fdg = FWRG(ftn_r_in_condi, ftn_w)
-
-    starts = ['f1', 'f2', 'f3']
-    df = ['f4', 'f5']
-    paths = AcyclicPath(starts, df, fdg)
-    print(f'{paths.paths}')
-
-def test_2():
-    ftn_r_in_condi = {'f1': ['a'], 'f2': [], 'f3': ['b'], 'f4': ['c','a']}
-    ftn_w = {'f1': ['a'], 'f2': ['b'], 'f3': ['c'], 'f4': []}
-    fdg = FWRG(ftn_r_in_condi, ftn_w)
-
-    starts = ['f1', 'f2' ]
-    df = ['f3', 'f4']
-    paths = AcyclicPath(starts, df, fdg)
-    print(f'{paths.paths}')
-    print(f'{paths.paths_df}')
-
-    updateFDG=UpdateFWRG(fdg, paths)
-    updateFDG.construct_fwrg_targets()
-    updateFDG.add_edges()
-    print(f'{updateFDG.fwrg_targets}')
-if __name__=='__main__':
-    test_2()
-
+from copy import copy, deepcopy
+
+import fdg.global_config
+
+from fdg.output_data import output_fwrg_data
+from fdg.preprocessing.preprocess import Preprocessing
+
+class FWRG():
+    def __init__(self,ftn_reads_in_condition:dict,ftn_writes:dict):
+        self.ftn_reads_in_condition = ftn_reads_in_condition
+        self.ftn_writes = ftn_writes
+        self.fwrg_dict={}
+        self.frwg_dict={}
+
+        self._generate_fwrg()
+        self._generate_frwg()
+
+    def _generate_fwrg(self):
+        for ftn,writes in self.ftn_writes.items():
+            if len(writes)==0:
+                self.fwrg_dict[ftn]={}
+                continue
+
+            children={}
+            for ftn_read,reads in self.ftn_reads_in_condition.items():
+                for write in writes:
+                    if write in reads:
+                        if ftn_read not in children.keys():
+                            children[ftn_read]=[write]
+                        else:
+                            children[ftn_read]+=[write]
+            self.fwrg_dict[ftn]=children
+
+    def _generate_frwg(self):
+        for ftn, reads in self.ftn_reads_in_condition.items():
+            if len(reads)==0:
+                self.frwg_dict[ftn]={}
+                continue
+            for ftn_write,writes in self.ftn_writes.items():
+                for read in reads:
+                    if read in writes:
+                        if ftn not in self.frwg_dict.keys():
+                            self.frwg_dict[ftn]=[ftn_write]
+                        else:
+                            if ftn_write not in self.frwg_dict[ftn]:
+                                self.frwg_dict[ftn]+=[ftn_write]
+                        break
+
+    def get_reads_in_conditions(self,ftn_name:str):
+        if ftn_name in self.ftn_reads_in_condition.keys():
+            return self.ftn_reads_in_condition[ftn_name]
+        else:return []
+
+class AcyclicPath():
+    def __init__(self, start_functions:list, dk_functions:list, fwrg:FWRG):
+        self.path_len_limit = fdg.global_config.seq_len_limit
+        self.fwrg=fwrg
+        self.start_functions=start_functions
+        self.dk_functions=[ftn for ftn,_ in dk_functions]
+
+        self.paths = {}
+        self._get_path()
+        self.paths_df={}
+        self.organize_paths()
+
+    def _get_path(self):
+        """
+        get all acyclic paths from starting functions (bounded by sequence length)
+        :return:
+        """
+        def get_children(ftn:str):
+            if ftn in self.fwrg.fwrg_dict.keys():
+                children=self.fwrg.fwrg_dict[ftn]
+                if len(children)>0:
+                    return list(children.keys())
+            return []
+        def derive_paths(start_ftn:str):
+            all_paths=[]
+            paths=[[start_ftn]]
+            for i in range(self.path_len_limit-1):
+                derived_paths=[]
+                for path in paths:
+                    children=get_children(path[-1])
+                    if len(children)==0:
+                        if path not in all_paths:
+                            all_paths.append(path)
+                    else:
+                        for child in children:
+                            if child in path:
+                                # think of the case [A(),A()](self dependency)
+                                if child==path[0] and len(path)==1:
+                                    path.append(child)
+                                if path not in all_paths:
+                                    all_paths.append(path)
+                            else:
+                                derived_paths.append(path+[child])
+                paths=derived_paths
+
+            all_paths+=paths
+            return all_paths
+
+
+        for sf in self.start_functions:
+            sf_path=derive_paths(sf)
+            self.paths[sf]=sf_path
+
+    def organize_paths(self):
+        for paths in self.paths.values():
+            for path in paths:
+                for idx,ftn in enumerate(path):
+                    if ftn in self.dk_functions and idx>0:# deep function can not be the frist function in a sequence
+                        t_path=path[0:idx+1]
+                        # add t_path
+                        if ftn not in self.paths_df.keys():
+                            self.paths_df[ftn]={}
+                        if len(t_path)-1 not in self.paths_df[ftn].keys():
+                            self.paths_df[ftn][len(t_path)-1]=[t_path]
+                        else:
+                            if t_path not in self.paths_df[ftn][len(t_path)-1]:
+                                self.paths_df[ftn][len(t_path)-1] += [t_path]
+
+class UpdateFWRG():
+    def __init__(self, fdg:FWRG, paths:AcyclicPath):
+        self.fwrg=fdg
+        self.acyclicPaths=paths
+
+        self.fwrg_targets={}
+
+        self.construct_fwrg_targets()
+
+        self.print_graphs(self.fwrg_targets,'fwrg_targets_data.txt')
+
+        self.fwrg_targets_augmented=deepcopy(self.fwrg_targets)
+        self.add_edges_1()
+        self.print_graphs(self.fwrg_targets_augmented,'fwrg_targets_augmented_data_update.txt')
+
+        self.dk_not_reachable=[]
+        self.identity_dk_function_not_reachable()
+
+    def print_graphs(self,data:dict,file_name:str):
+        output_fwrg_data(data, file_name, 'funtion write-read graph data')
+
+
+    def add_edge_to_graph(self,from_:str,to_:str):
+        if from_ in self.fwrg_targets_augmented.keys():
+            if to_ not in self.fwrg_targets_augmented[from_]:
+                self.fwrg_targets_augmented[from_].append(to_)
+        else:
+            self.fwrg_targets_augmented[from_]=[to_]
+
+
+    def construct_fwrg_targets(self):
+        # reconstruct edges from given acyclic paths
+        for value in self.acyclicPaths.paths_df.values():
+            if not isinstance(value,dict):continue
+            for paths in value.values():
+                for path in paths:
+                    # add edges
+                    for i in range(len(path) - 1):
+                        if path[i] not in self.fwrg_targets.keys():
+                            self.fwrg_targets[path[i]] = [path[i + 1]]
+                        else:
+                            if path[i+1] not in self.fwrg_targets[path[i]]:
+                                self.fwrg_targets[path[i]] += [path[i + 1]]
+
+
+
+    def add_edges_1(self):
+        """
+        for each deep function, add edges to connect some of its paths
+
+        for each deep function, try to find a combined path
+        :return:
+        """
+        def belong_relation(seq1:list,seq2:list):
+            s1=seq1
+            s2=seq2
+            if len(seq1)>len(seq2):
+                s1=seq2
+                s2=seq1
+            if [True for e in s1 if e not in s2].count(True)>0:
+                return False
+            else:
+                return True
+
+        def common_elements(seq1: list, seq2: list):
+            common=[]
+            s1 = seq1
+            s2 = seq2
+            if len(seq1) > len(seq2):
+                s1 = seq2
+                s2 = seq1
+            for e in s1:
+                if e in s2:
+                    common.append(e)
+            return common
+
+        def find_edges(seq1: list, seq2: list, common: list):
+            edges = []
+            s1 = seq1
+            s2 = seq2
+            if len(seq1) > len(seq2):
+                s1 = seq2
+                s2 = seq1
+
+            f1 = -1
+            t1 = -1
+            f2 = -1
+            t2 = -1
+            idx2 = 0
+            for idx, e in enumerate(s1):
+                if e not in common:
+                    if t1 == -1:
+                        t1 = idx
+                    f1 = idx
+                else:
+
+                    # check s2 if there are elements before e
+                    for i in range(idx2, len(s2)):
+                        if not s2[i] == e:
+                            if t2 == -1:
+                                t2 = i
+                            f2 = i
+                        else:
+
+                            break
+
+                    if f2 >= 0 and t2 >= 0 and t1 >= 0 and f1 >= 0:
+                        edges.append((s2[f2], s1[t1]))
+                        edges.append((s1[f1], s2[t2]))
+
+                    idx2 = i + 1
+                    f1 = f2 = t1 = t2 = -1
+                    continue
+
+            if t1 >= 0 and f1 >= 0:
+                if idx2 > len(s2) - 1:
+                    return edges
+                for i in range(idx2, len(s2)):
+                    if not s2[i] == e:
+                        if t2 == -1:
+                            t2 = i
+                        f2 = i
+                    else:
+                        break
+                if f2 >= 0 and t2 >= 0:
+                    edges.append((s2[f2], s1[t1]))
+                    edges.append((s1[f1], s2[t2]))
+
+            return edges
+        for df,value in self.acyclicPaths.paths_df.items():
+
+            if isinstance(value,dict):
+                sequences=[]
+                for seq_list in value.values():
+                    for seq in seq_list:
+                        sequences.append(seq[0:-1])
+
+                all_pairs=[(a,b) for idx,a in enumerate(sequences) for b in sequences[idx+1:]]
+
+                for seq1,seq2 in all_pairs:
+                    if belong_relation(seq1, seq2):
+                        # do not add edges
+                        continue
+                    common = common_elements(seq1, seq2)
+                    if len(common) == 0:
+                        # add edges
+                        self.add_edge_to_graph(seq1[-1], seq2[0])
+                        self.add_edge_to_graph(seq2[-1], seq1[0])
+
+                    else:
+                        edges=find_edges(seq1, seq2, common)
+                        for f,t in edges:
+                            self.add_edge_to_graph(f, t)
+
+    def identity_dk_function_not_reachable(self):
+        for dk in self.acyclicPaths.dk_functions:
+            if dk not in self.acyclicPaths.paths_df.keys():
+                self.dk_not_reachable.append(dk)
+                # print(f'{dk} is not reachable')
+            else:
+                if len(self.acyclicPaths.paths_df[dk])==0:
+                    self.dk_not_reachable.append(dk)
+                    # print(f'{dk} is not reachable')
+
+class FWRG_manager():
+    def __init__(self, start_functions:list, dk_functions:list, preprocess:Preprocessing):
+        self.fwrg=FWRG(preprocess.read_in_conditions.read_slots_in_conditions,
+                       preprocess.write_read_info.write_slots)
+        self.fwrg_all_reads={}
+        self.generate_graph_all_reads(preprocess.write_read_info.write_slots,preprocess.write_read_info.read_slots)
+
+        self.acyclicPaths=AcyclicPath(start_functions, dk_functions, self.fwrg)
+        self.updateFWRG=UpdateFWRG(self.fwrg, self.acyclicPaths)
+
+    def generate_graph_all_reads(self,writes:dict,all_reads:dict):
+        for ftn,writes in writes.items():
+            if len(writes)==0:
+                self.fwrg_all_reads[ftn]={}
+                continue
+            children={}
+            for ftn_read,reads in all_reads.items():
+                for write in writes:
+                     if write in reads:
+                         if ftn_read not in children.keys():
+                             children[ftn_read]=[write]
+                         else:
+                             children[ftn_read]+=[write]
+            self.fwrg_all_reads[ftn]=children
+                
+    def get_children_all_reads(self,ftn:str):
+        if ftn in self.fwrg_all_reads.keys():
+            return list(self.fwrg_all_reads[ftn].keys())
+        else:
+            return []
+    def get_children_fwrg(self,ftn:str):
+        if ftn in self.fwrg.fwrg_dict.keys():
+            return list(self.fwrg.fwrg_dict[ftn])
+        else:
+            return []
+
+    def get_children_fwrg_T_A(self, ftn:str)->list:
+        if ftn in self.updateFWRG.fwrg_targets_augmented.keys():
+            return self.updateFWRG.fwrg_targets_augmented[ftn]
+        else: return []
+
+    def get_parents_frwg(self, ftn:str)->list:
+        if ftn in self.fwrg.frwg_dict.keys():
+            return self.fwrg.frwg_dict[ftn]
+        else:
+            return []
+
+    def get_children_bf_update(self, ftn:str)->list:
+        if ftn in self.updateFWRG.fwrg_targets.keys():
+            return self.updateFWRG.fwrg_targets[ftn]
+        else: return []
+
+
+
+
+
+
+
+
+def test_1():
+    ftn_r_in_condi = {'f2': ['a'], 'f3': ['b'], 'f4': ['c'], 'f5': ['c']}
+    ftn_w = {'f2': ['b'], 'f3': ['a', 'c'], 'f4': [], 'f5': []}
+    fdg = FWRG(ftn_r_in_condi, ftn_w)
+
+    starts = ['f1', 'f2', 'f3']
+    df = ['f4', 'f5']
+    paths = AcyclicPath(starts, df, fdg)
+    print(f'{paths.paths}')
+
+def test_2():
+    ftn_r_in_condi = {'f1': ['a'], 'f2': [], 'f3': ['b'], 'f4': ['c','a']}
+    ftn_w = {'f1': ['a'], 'f2': ['b'], 'f3': ['c'], 'f4': []}
+    fdg = FWRG(ftn_r_in_condi, ftn_w)
+
+    starts = ['f1', 'f2' ]
+    df = ['f3', 'f4']
+    paths = AcyclicPath(starts, df, fdg)
+    print(f'{paths.paths}')
+    print(f'{paths.paths_df}')
+
+    updateFDG=UpdateFWRG(fdg, paths)
+    updateFDG.construct_fwrg_targets()
+    updateFDG.add_edges()
+    print(f'{updateFDG.fwrg_targets}')
+if __name__=='__main__':
+    test_2()
+
```

### Comparing `smartExecutorx-0.3/fdg/global_config.py` & `smartExecutorx-4.0/fdg/global_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,125 +1,128 @@
-
-"""
-Important parameters 
-"""
-#===============================================
-# parameters that can be set by users
-#--------------------------------------------
-
-# indicate if a graph strategy is used to direct the symbolic execution
-global flag_fwrg
-fdg_fwrg=False
-
-
-# set the search strategy when guiding the symolic execution using a graph structure
-global function_search_strategy
-function_search_strategy='bfs'
-
-
-# having value larger than 0 means brandom baseline is active
-# the value indicates the percentage of functions to be selected
-# 1: 10%, 5:50%,...
-global random_baseline
-random_baseline=0
-
-
-# indicate the code coverage that a function should reach
-global function_coverage_threshold
-function_coverage_threshold=98
-
-
-# set the timeout for the preprocessing
-global preprocess_timeout
-preprocess_timeout=300
-
-
-# indicate if functions' coverage will be printed.1:yes, 0:no
-global print_function_coverage
-print_function_coverage=1
-
-# set to 1 if optimization is considered or not
-# optimizations:
-#    collect concrete addresses and treat them as the possible address msg.sender can take
-#    add initial ether for the contract
-global optimization
-optimization=1
-
-
-# indicate if all the state variables read in functions should be considered.
-# by default, only the state varibles read in conditions are considered.
-global flag_consider_all_reads
-flag_consider_all_read=1
-
-
-# set the limit on the times a function can be executed
-global execution_times_limit
-execution_times_limit=5
-
-
-# provide the sequences to  be executed
-global sequences
-sequences=[]
-
-#===============================================
-# currently, does not support to change them through command line
-#----------------------------------------------
-global output_path
-output_path='C:\\Users\\18178\\Desktop\\temp\\'
-
-# set maximum number of iterations of the symbolic execution engine
-global transaction_count
-transaction_count=100
-
-# the max length of a sequence
-global seq_len_limit
-seq_len_limit=4
-
-
-#===============================================
-# their values are set based on the execution
-#----------------------------------------------
-# save the contract address
-global contract_address
-contract_address=''
-
-# save the function signatures from the disassembler
-global method_identifiers
-method_identifiers={}
-
-# set True if there is an exception in the preprocessing
-global preprocessing_exception
-preprocessing_exception=False
-
-# indicate if the execution is in the preprocessing
-global flag_preprocessing
-flag_preprocessing=False
-
-# set True if there is timeout in the preprocessing
-global flag_preprocess_timeout
-flag_preprocess_timeout=False
-
-# save the runtime bytecode of the target function
-global target_runtime_bytecode
-target_runtime_bytecode= ''
-
-# there are used by the modules (no need to set their values)
-global flag_query_solver
-flag_query_solver=[]
-
-# indicate the length of the transaction sequence
-global tx_len
-tx_len=0
-
-global flag_fallback
-flag_fallback=False
-
-#===============================================
-
-global temp_count
-temp_count=0
-
-global time_temp
-time_temp=0
-
-global count
-count=0
+
+"""
+Important parameters 
+"""
+#===============================================
+# parameters that can be set by users
+#--------------------------------------------
+
+# indicate if a graph strategy is used to direct the symbolic execution
+global flag_fwrg
+fdg_fwrg=False
+
+
+# set the search strategy when guiding the symolic execution using a graph structure
+global function_search_strategy
+function_search_strategy='bfs'
+
+
+# having value larger than 0 means brandom baseline is active
+# the value indicates the percentage of functions to be selected
+# 1: 10%, 5:50%,...
+global random_baseline
+random_baseline=0
+
+
+# indicate the code coverage that a function should reach
+global function_coverage_threshold
+function_coverage_threshold=98
+
+
+# set the timeout for the preprocessing
+global preprocess_timeout
+preprocess_timeout=300
+
+
+# indicate if functions' coverage will be printed.1:yes, 0:no
+global print_function_coverage
+print_function_coverage=1
+
+# set to 1 if optimization is considered or not
+# optimizations:
+#    collect concrete addresses and treat them as the possible address msg.sender can take
+#    add initial ether for the contract
+global optimization
+optimization=1
+
+
+# indicate if all the state variables read in functions should be considered.
+# by default, only the state varibles read in conditions are considered.
+global flag_consider_all_reads
+flag_consider_all_read=1
+
+
+# set the limit on the times a function can be executed
+global execution_times_limit
+execution_times_limit=5
+
+
+# provide the sequences to  be executed
+global sequences
+sequences=[]
+
+#===============================================
+# currently, does not support to change them through command line
+#----------------------------------------------
+global output_path
+output_path='C:\\Users\\18178\\Desktop\\temp\\'
+
+# set maximum number of iterations of the symbolic execution engine
+global transaction_count
+transaction_count=100
+
+# the max length of a sequence
+global seq_len_limit
+seq_len_limit=4
+
+
+#===============================================
+# their values are set based on the execution
+#----------------------------------------------
+# save the contract address
+global contract_address
+contract_address=''
+
+# save the function signatures from the disassembler
+global method_identifiers
+method_identifiers={}
+
+# set True if there is an exception in the preprocessing
+global preprocessing_exception
+preprocessing_exception=False
+
+# indicate if the execution is in the preprocessing
+global flag_preprocessing
+flag_preprocessing=False
+
+# set True if there is timeout in the preprocessing
+global flag_preprocess_timeout
+flag_preprocess_timeout=False
+
+# save the runtime bytecode of the target function
+global target_runtime_bytecode
+target_runtime_bytecode= ''
+
+# there are used by the modules (no need to set their values)
+global flag_query_solver
+flag_query_solver=[]
+
+# indicate the length of the transaction sequence
+global tx_len
+tx_len=0
+
+global flag_fallback
+flag_fallback=False
+
+global p1_dl
+p1_dl=1
+
+#===============================================
+
+global temp_count
+temp_count=0
+
+global time_temp
+time_temp=0
+
+global count
+count=0
```

### Comparing `smartExecutorx-0.3/fdg/instruction_modification.py` & `smartExecutorx-4.0/fdg/instruction_modification.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,366 +1,366 @@
-from copy import copy
-
-from fdg.output_data import print_list, print_dict
-from mythril.laser.ethereum.state.world_state import WorldState
-
-
-
-class InstructionModification():
-    """
-    change the function dispatcher at the beginning part of the instruction list
-    """
-
-    def __init__(self,ftn_identifier:dict):
-        self.function_identifier=ftn_identifier
-        self.contract_address=None # used to identity the instructions of the contract
-
-        self.instruction_list = []
-
-        self.functions_to_positions = {}
-        self.positions_to_instructions = {} # divide instructions into groups and use the positions to indicate the order
-        self.all_positions_related_function=[]
-        self.jumpdest_in_dispatcher=[]# record the number of jumpdest in the function dispatcher
-        self.address_jumpdest_revert_block=0
-        self.positions_contain_GT = [] # the positions are kept in this case as they involve in branches in dispatcher
-
-    def feed_instructions(self, state:WorldState, contract_address):
-        """
-        new way to group instructions.
-        :argument
-        """
-        self.contract_address = contract_address
-        key = contract_address.value
-        code = state.accounts[key].code
-        self.instruction_list=code.instruction_list
-
-        # print_list(self.instruction_list, "instruction list")
-
-        if len(self.function_identifier)>0:
-            self._feed_instructions_update()
-
-        print(f'total instructions: {len(self.instruction_list)}')
-
-    def _feed_instructions(self):
-        """
-        new way to group instructions.
-        :argument
-        """
-
-        def record_position(position:int,instruction:dict):
-
-            self.positions_to_instructions[position] = []
-
-            # get the function's signature as a key
-            function_key = instruction['argument']
-            if len(function_key) == 8:
-                function_key = '0x00' + function_key[2:]
-                print(f'convert {instruction["argument"]} to {function_key}')
-
-            if function_key not in self.functions_to_positions.keys():
-                self.functions_to_positions[function_key] = [position]
-            else:
-                self.functions_to_positions[function_key] += [position]
-
-
-        # ============================================
-        # through PHSH4 and JUMPDEST to sperate instructions
-        offset_instr = 0
-        flag_status = 0  # change its value when "CALLDATASIZE" is met and the first PUSH after "CALLDATASIZE" is met
-
-        position = 0
-        self.positions_to_instructions[0] = []
-        self.address_jumpdest_revert_block = 0  # signal the end of function dispatcher
-        self.positions_contain_GT=[]
-
-        for instruction in self.instruction_list:
-            print(f'instruction:{instruction}')
-            opcode = instruction['opcode']
-            if str(opcode).__eq__('CALLDATASIZE'):
-                flag_status = 1  # ready to get address of JUMPDEST for the block of revert
-
-            elif str(opcode).startswith('PUSH'):
-                if flag_status==1:
-                    print(f'flag_status==1:{instruction}')
-                    jumpdest_address = int(instruction["argument"], 0)
-                    if jumpdest_address > 0:
-                        self.address_jumpdest_revert_block = jumpdest_address
-                if flag_status == 2:
-                    if not str(instruction['argument']).__eq__('0xffffffff'):
-                        if str(opcode).__eq__('PUSH4') or str(opcode).__eq__('PUSH3'):
-                            if len(self.positions_to_instructions[position]) > 0:
-                                if self.positions_to_instructions[position][-1]['opcode'] == 'DUP1':
-                                    # get a new key-value pair to hold instructions for the function whose signature specified by this PUSH instruction
-                                    position += 1
-                                    record_position(position, instruction)
-
-
-            elif str(opcode).__eq__('JUMPDEST'):  # the entry to the revert block when call data size is less than 4(before the code of functions)
-                if flag_status == 2:
-                    if self.address_jumpdest_revert_block == instruction["address"]:
-                        # stop when reaching the end of function dispatcher
-                        break
-                    else:
-                        position += 1
-                        self.jumpdest_in_dispatcher.append((position,offset_instr))
-                        self.positions_to_instructions[position] = []
-            elif str(opcode).__eq__(
-                'CALLDATALOAD'): # assume that CALLDATALOAD appears before funcion matching
-
-                flag_status=2 # ready to get matching instructions
-
-            elif str(opcode)in ['GT']:
-                if flag_status == 2:
-                    self.positions_contain_GT.append(position)# get the positions that contain GT
-
-            # save the current instruction
-            self.positions_to_instructions[position] += [instruction]
-
-            offset_instr += 1
-
-        print_dict(self.positions_to_instructions,'instruction grouping in instruction modification')
-
-
-        # end of instruction iteration at the beginning section
-        last_position=position+1
-
-        # keep the last portion of instructions
-        self.positions_to_instructions[last_position] = self.instruction_list[offset_instr:]
-
-
-
-
-        # find all positions that are corresponding to functions
-        positions=[]
-        for p in self.functions_to_positions.values():
-            positions+=p
-        self.all_positions_related_function=positions
-    def _feed_instructions_update(self):
-        """
-        new way to group instructions.
-        :argument
-        """
-
-        def record_position(position:int,instruction:dict):
-
-            self.positions_to_instructions[position] = []
-
-            # get the function's signature as a key
-            function_key = get_back_functin_signature(instruction['argument'])
-
-            # if len(function_key) == 8:
-            #     function_key = '0x00' + function_key[2:]
-            #     print(f'convert {instruction["argument"]} to {function_key}')
-
-            if function_key not in self.functions_to_positions.keys():
-                self.functions_to_positions[function_key] = [position]
-            else:
-                self.functions_to_positions[function_key] += [position]
-
-        def get_back_functin_signature(byte_tuple)->str:
-            key='0x'
-            if len(byte_tuple)==3:
-                key+='00'
-            for item in byte_tuple:
-                v=hex(item)[2:]
-                key+=v if len(v)==2 else '0'+v
-            # print(f'{byte_tuple}=>{key}')
-            return key
-
-        def get_address_from_argument(int_tuple) -> int:
-            value = 0
-            exp = 0
-            for item in reversed(int_tuple):
-                value += item * 256 ** exp
-                exp += 1
-            return value
-
-        # ============================================
-        # through PHSH4 and JUMPDEST to sperate instructions
-        offset_instr = 0
-        flag_status = 0  # change its value when "CALLDATASIZE" is met and the first PUSH after "CALLDATASIZE" is met
-
-        position = 0
-        self.positions_to_instructions[0] = []
-        self.address_jumpdest_revert_block = 0  # signal the end of function dispatcher
-        self.positions_contain_GT=[]
-
-        for instruction in self.instruction_list:
-            # print(f'instruction:{instruction}')
-            opcode = instruction['opcode']
-            if str(opcode).__eq__('CALLDATASIZE'):
-                flag_status = 1  # ready to get address of JUMPDEST for the block of revert
-
-            elif str(opcode).startswith('PUSH'):
-                if flag_status==1:
-                    jumpdest_address=get_address_from_argument( instruction["argument"])
-                    if jumpdest_address> 0:
-                        self.address_jumpdest_revert_block = jumpdest_address
-                if flag_status == 2:
-                    if not get_back_functin_signature(instruction['argument']).__eq__('0xffffffff'):
-                        if str(opcode).__eq__('PUSH4') or str(opcode).__eq__('PUSH3'):
-                            if len(self.positions_to_instructions[position]) > 0:
-                                if self.positions_to_instructions[position][-1]['opcode'] == 'DUP1':
-                                    # get a new key-value pair to hold instructions for the function whose signature specified by this PUSH instruction
-                                    position += 1
-                                    record_position(position, instruction)
-
-
-            elif str(opcode).__eq__('JUMPDEST'):  # the entry to the revert block when call data size is less than 4(before the code of functions)
-                if flag_status == 2:
-                    if self.address_jumpdest_revert_block == instruction["address"]:
-                        # stop when reaching the end of function dispatcher
-                        break
-                    else:
-                        position += 1
-                        self.jumpdest_in_dispatcher.append((position,offset_instr))
-                        self.positions_to_instructions[position] = []
-            elif str(opcode).__eq__(
-                'CALLDATALOAD'): # assume that CALLDATALOAD appears before funcion matching
-
-                flag_status=2 # ready to get matching instructions
-
-            elif str(opcode)in ['GT']:
-                if flag_status == 2:
-                    self.positions_contain_GT.append(position)# get the positions that contain GT
-
-            # save the current instruction
-            self.positions_to_instructions[position] += [instruction]
-
-            offset_instr += 1
-
-        # print_dict(self.positions_to_instructions,'instruction grouping in instruction modification')
-
-
-        # end of instruction iteration at the beginning section
-        last_position=position+1
-
-        # keep the last portion of instructions
-        self.positions_to_instructions[last_position] = self.instruction_list[offset_instr:]
-
-
-
-
-        # find all positions that are corresponding to functions
-        positions=[]
-        for p in self.functions_to_positions.values():
-            positions+=p
-        self.all_positions_related_function=positions
-    def modify_on_a_state__str(self, state: WorldState, functions: list):
-        """
-            update the instructions on multiple states
-        """
-        if len(functions)>=len(self.function_identifier.keys()):
-            final_instructions=self.instruction_list
-            state.accounts[self.contract_address.value].code.instruction_list = final_instructions
-
-        else:
-            fct_selectors=[]
-            for ftn in functions:
-                if ftn in ['fallback']:continue
-                if ftn not in self.function_identifier.keys():continue # can  not do anything
-                fct_selectors.append(self.function_identifier[ftn])
-            final_instructions=self._get_modified_instructions_1(fct_selectors)
-
-            # update instructions for states
-            state.accounts[self.contract_address.value].code.instruction_list = final_instructions
-            state.accounts[self.contract_address.value].code.func_hashes = fct_selectors
-
-    def modity_on_multiple_states(self,states:[WorldState],functions:list):
-        if 'original_instruction_list' in functions:
-            final_instructions = self.instruction_list
-            print(f'keep the original instruction list in instruction_modification.py')
-            for state in states:
-                state.accounts[self.contract_address.value].code.instruction_list = final_instructions
-            return
-
-
-        if len(functions) >= len(self.function_identifier.keys()):
-            final_instructions = self.instruction_list
-            for state in states:
-                state.accounts[self.contract_address.value].code.instruction_list = final_instructions
-            return
-
-
-        fct_selectors = []
-        for ftn in functions:
-            if ftn in ['fallback']: continue
-            if ftn not in self.function_identifier.keys(): continue  # can  not do anything
-            fct_selectors.append(self.function_identifier[ftn])
-
-        final_instructions = self._get_modified_instructions_1(fct_selectors)
-
-        for state in states:
-           # update instructions for states
-            state.accounts[self.contract_address.value].code.instruction_list = final_instructions
-            state.accounts[self.contract_address.value].code.func_hashes = fct_selectors
-
-    def _get_modified_instructions_1(self, fct_selectors: list) -> list:
-        """
-            replace the matching instructions of other functions with EMPTY instruction
-            keep the matching instructions of the specified functions
-            * handle fallback() which has no selector
-            * make sure that the last "DUP1" is replaced when the max position of the kept functions is not the last function
-        """
-
-        ftn_selectors_valid = [selector for selector in fct_selectors if selector in self.functions_to_positions.keys()]
-
-
-        # find positions not kept
-        # keep the functions having two positions(there are branches in the function dispatcher)
-        keep = copy(self.positions_contain_GT)
-        for ftn_selector in ftn_selectors_valid:
-            keep += self.functions_to_positions[ftn_selector]
-
-        not_kept = [p for p in self.all_positions_related_function if p not in keep]
-
-         # combine instruction groups
-        combined_instructions = []
-        for p in range(0,len(self.positions_to_instructions) - 1):
-            if p not in not_kept:
-                combined_instructions += self.positions_to_instructions[p]
-            else:
-                # replace with EMPTY instructions
-                empty_instructions = []  # do not remove them, it will cause inconsistency in terms of the total number of instructions
-                for instruction in self.positions_to_instructions[p]:
-                    empty_instructions.append({"address": instruction["address"], "opcode": "EMPTY"})
-
-                combined_instructions += empty_instructions
-
-        # before combining the last instruction group (the instructions of regular functions)
-        # If the last non-EMPTY opcode is DUP,remove it in the already combined instructions
-        for index in range(len(combined_instructions) - 1, 0, -1):
-            if str(combined_instructions[index]['opcode']).__eq__('EMPTY'):
-                continue
-            else:
-                if str(combined_instructions[index]['opcode']).__eq__('DUP1'):
-                    instruction = combined_instructions[index]
-                    combined_instructions[index] = {"address": instruction["address"], "opcode": "EMPTY"}
-
-                break
-
-
-        #
-        for p,idx in self.jumpdest_in_dispatcher:
-            idx=idx-1
-            while True:
-                instruction=combined_instructions[idx]
-                opcode=instruction['opcode']
-                if str(opcode).__eq__('EMPTY'):
-                    idx = idx - 1
-                    continue
-                else:
-                    if str(opcode) in ['JUMPDEST','PUSH4']:
-                        break
-                    if str(opcode).__eq__('DUP1'):
-                        combined_instructions[idx] = {"address": instruction["address"], "opcode": "EMPTY"}
-                    break
-
-        # print_list(combined_instructions)
-        combined_instructions += self.positions_to_instructions[len(self.positions_to_instructions) - 1]
-
-
-        return combined_instructions
-
-    def modify_no_modification(self,state:WorldState):
-        state.accounts[self.contract_address.value].code.instruction_list = self.instruction_list
-
+from copy import copy
+
+from fdg.output_data import print_list, print_dict
+from mythril.laser.ethereum.state.world_state import WorldState
+
+
+
+class InstructionModification():
+    """
+    change the function dispatcher at the beginning part of the instruction list
+    """
+
+    def __init__(self,ftn_identifier:dict):
+        self.function_identifier=ftn_identifier
+        self.contract_address=None # used to identity the instructions of the contract
+
+        self.instruction_list = []
+
+        self.functions_to_positions = {}
+        self.positions_to_instructions = {} # divide instructions into groups and use the positions to indicate the order
+        self.all_positions_related_function=[]
+        self.jumpdest_in_dispatcher=[]# record the number of jumpdest in the function dispatcher
+        self.address_jumpdest_revert_block=0
+        self.positions_contain_GT = [] # the positions are kept in this case as they involve in branches in dispatcher
+
+    def feed_instructions(self, state:WorldState, contract_address):
+        """
+        new way to group instructions.
+        :argument
+        """
+        self.contract_address = contract_address
+        key = contract_address.value
+        code = state.accounts[key].code
+        self.instruction_list=code.instruction_list
+
+        # print_list(self.instruction_list, "instruction list")
+
+        if len(self.function_identifier)>0:
+            self._feed_instructions_update()
+
+        print(f'total instructions: {len(self.instruction_list)}')
+
+    def _feed_instructions(self):
+        """
+        new way to group instructions.
+        :argument
+        """
+
+        def record_position(position:int,instruction:dict):
+
+            self.positions_to_instructions[position] = []
+
+            # get the function's signature as a key
+            function_key = instruction['argument']
+            if len(function_key) == 8:
+                function_key = '0x00' + function_key[2:]
+                print(f'convert {instruction["argument"]} to {function_key}')
+
+            if function_key not in self.functions_to_positions.keys():
+                self.functions_to_positions[function_key] = [position]
+            else:
+                self.functions_to_positions[function_key] += [position]
+
+
+        # ============================================
+        # through PHSH4 and JUMPDEST to sperate instructions
+        offset_instr = 0
+        flag_status = 0  # change its value when "CALLDATASIZE" is met and the first PUSH after "CALLDATASIZE" is met
+
+        position = 0
+        self.positions_to_instructions[0] = []
+        self.address_jumpdest_revert_block = 0  # signal the end of function dispatcher
+        self.positions_contain_GT=[]
+
+        for instruction in self.instruction_list:
+            print(f'instruction:{instruction}')
+            opcode = instruction['opcode']
+            if str(opcode).__eq__('CALLDATASIZE'):
+                flag_status = 1  # ready to get address of JUMPDEST for the block of revert
+
+            elif str(opcode).startswith('PUSH'):
+                if flag_status==1:
+                    print(f'flag_status==1:{instruction}')
+                    jumpdest_address = int(instruction["argument"], 0)
+                    if jumpdest_address > 0:
+                        self.address_jumpdest_revert_block = jumpdest_address
+                if flag_status == 2:
+                    if not str(instruction['argument']).__eq__('0xffffffff'):
+                        if str(opcode).__eq__('PUSH4') or str(opcode).__eq__('PUSH3'):
+                            if len(self.positions_to_instructions[position]) > 0:
+                                if self.positions_to_instructions[position][-1]['opcode'] == 'DUP1':
+                                    # get a new key-value pair to hold instructions for the function whose signature specified by this PUSH instruction
+                                    position += 1
+                                    record_position(position, instruction)
+
+
+            elif str(opcode).__eq__('JUMPDEST'):  # the entry to the revert block when call data size is less than 4(before the code of functions)
+                if flag_status == 2:
+                    if self.address_jumpdest_revert_block == instruction["address"]:
+                        # stop when reaching the end of function dispatcher
+                        break
+                    else:
+                        position += 1
+                        self.jumpdest_in_dispatcher.append((position,offset_instr))
+                        self.positions_to_instructions[position] = []
+            elif str(opcode).__eq__(
+                'CALLDATALOAD'): # assume that CALLDATALOAD appears before funcion matching
+
+                flag_status=2 # ready to get matching instructions
+
+            elif str(opcode)in ['GT']:
+                if flag_status == 2:
+                    self.positions_contain_GT.append(position)# get the positions that contain GT
+
+            # save the current instruction
+            self.positions_to_instructions[position] += [instruction]
+
+            offset_instr += 1
+
+        print_dict(self.positions_to_instructions,'instruction grouping in instruction modification')
+
+
+        # end of instruction iteration at the beginning section
+        last_position=position+1
+
+        # keep the last portion of instructions
+        self.positions_to_instructions[last_position] = self.instruction_list[offset_instr:]
+
+
+
+
+        # find all positions that are corresponding to functions
+        positions=[]
+        for p in self.functions_to_positions.values():
+            positions+=p
+        self.all_positions_related_function=positions
+    def _feed_instructions_update(self):
+        """
+        new way to group instructions.
+        :argument
+        """
+
+        def record_position(position:int,instruction:dict):
+
+            self.positions_to_instructions[position] = []
+
+            # get the function's signature as a key
+            function_key = get_back_functin_signature(instruction['argument'])
+
+            # if len(function_key) == 8:
+            #     function_key = '0x00' + function_key[2:]
+            #     print(f'convert {instruction["argument"]} to {function_key}')
+
+            if function_key not in self.functions_to_positions.keys():
+                self.functions_to_positions[function_key] = [position]
+            else:
+                self.functions_to_positions[function_key] += [position]
+
+        def get_back_functin_signature(byte_tuple)->str:
+            key='0x'
+            if len(byte_tuple)==3:
+                key+='00'
+            for item in byte_tuple:
+                v=hex(item)[2:]
+                key+=v if len(v)==2 else '0'+v
+            # print(f'{byte_tuple}=>{key}')
+            return key
+
+        def get_address_from_argument(int_tuple) -> int:
+            value = 0
+            exp = 0
+            for item in reversed(int_tuple):
+                value += item * 256 ** exp
+                exp += 1
+            return value
+
+        # ============================================
+        # through PHSH4 and JUMPDEST to sperate instructions
+        offset_instr = 0
+        flag_status = 0  # change its value when "CALLDATASIZE" is met and the first PUSH after "CALLDATASIZE" is met
+
+        position = 0
+        self.positions_to_instructions[0] = []
+        self.address_jumpdest_revert_block = 0  # signal the end of function dispatcher
+        self.positions_contain_GT=[]
+
+        for instruction in self.instruction_list:
+            # print(f'instruction:{instruction}')
+            opcode = instruction['opcode']
+            if str(opcode).__eq__('CALLDATASIZE'):
+                flag_status = 1  # ready to get address of JUMPDEST for the block of revert
+
+            elif str(opcode).startswith('PUSH'):
+                if flag_status==1:
+                    jumpdest_address=get_address_from_argument( instruction["argument"])
+                    if jumpdest_address> 0:
+                        self.address_jumpdest_revert_block = jumpdest_address
+                if flag_status == 2:
+                    if not get_back_functin_signature(instruction['argument']).__eq__('0xffffffff'):
+                        if str(opcode).__eq__('PUSH4') or str(opcode).__eq__('PUSH3'):
+                            if len(self.positions_to_instructions[position]) > 0:
+                                if self.positions_to_instructions[position][-1]['opcode'] == 'DUP1':
+                                    # get a new key-value pair to hold instructions for the function whose signature specified by this PUSH instruction
+                                    position += 1
+                                    record_position(position, instruction)
+
+
+            elif str(opcode).__eq__('JUMPDEST'):  # the entry to the revert block when call data size is less than 4(before the code of functions)
+                if flag_status == 2:
+                    if self.address_jumpdest_revert_block == instruction["address"]:
+                        # stop when reaching the end of function dispatcher
+                        break
+                    else:
+                        position += 1
+                        self.jumpdest_in_dispatcher.append((position,offset_instr))
+                        self.positions_to_instructions[position] = []
+            elif str(opcode).__eq__(
+                'CALLDATALOAD'): # assume that CALLDATALOAD appears before funcion matching
+
+                flag_status=2 # ready to get matching instructions
+
+            elif str(opcode)in ['GT']:
+                if flag_status == 2:
+                    self.positions_contain_GT.append(position)# get the positions that contain GT
+
+            # save the current instruction
+            self.positions_to_instructions[position] += [instruction]
+
+            offset_instr += 1
+
+        # print_dict(self.positions_to_instructions,'instruction grouping in instruction modification')
+
+
+        # end of instruction iteration at the beginning section
+        last_position=position+1
+
+        # keep the last portion of instructions
+        self.positions_to_instructions[last_position] = self.instruction_list[offset_instr:]
+
+
+
+
+        # find all positions that are corresponding to functions
+        positions=[]
+        for p in self.functions_to_positions.values():
+            positions+=p
+        self.all_positions_related_function=positions
+    def modify_on_a_state__str(self, state: WorldState, functions: list):
+        """
+            update the instructions on multiple states
+        """
+        if len(functions)>=len(self.function_identifier.keys()):
+            final_instructions=self.instruction_list
+            state.accounts[self.contract_address.value].code.instruction_list = final_instructions
+
+        else:
+            fct_selectors=[]
+            for ftn in functions:
+                if ftn in ['fallback']:continue
+                if ftn not in self.function_identifier.keys():continue # can  not do anything
+                fct_selectors.append(self.function_identifier[ftn])
+            final_instructions=self._get_modified_instructions_1(fct_selectors)
+
+            # update instructions for states
+            state.accounts[self.contract_address.value].code.instruction_list = final_instructions
+            state.accounts[self.contract_address.value].code.func_hashes = fct_selectors
+
+    def modity_on_multiple_states(self,states:[WorldState],functions:list):
+        if 'original_instruction_list' in functions:
+            final_instructions = self.instruction_list
+            print(f'keep the original instruction list in instruction_modification.py')
+            for state in states:
+                state.accounts[self.contract_address.value].code.instruction_list = final_instructions
+            return
+
+
+        if len(functions) >= len(self.function_identifier.keys()):
+            final_instructions = self.instruction_list
+            for state in states:
+                state.accounts[self.contract_address.value].code.instruction_list = final_instructions
+            return
+
+
+        fct_selectors = []
+        for ftn in functions:
+            if ftn in ['fallback']: continue
+            if ftn not in self.function_identifier.keys(): continue  # can  not do anything
+            fct_selectors.append(self.function_identifier[ftn])
+
+        final_instructions = self._get_modified_instructions_1(fct_selectors)
+
+        for state in states:
+           # update instructions for states
+            state.accounts[self.contract_address.value].code.instruction_list = final_instructions
+            state.accounts[self.contract_address.value].code.func_hashes = fct_selectors
+
+    def _get_modified_instructions_1(self, fct_selectors: list) -> list:
+        """
+            replace the matching instructions of other functions with EMPTY instruction
+            keep the matching instructions of the specified functions
+            * handle fallback() which has no selector
+            * make sure that the last "DUP1" is replaced when the max position of the kept functions is not the last function
+        """
+
+        ftn_selectors_valid = [selector for selector in fct_selectors if selector in self.functions_to_positions.keys()]
+
+
+        # find positions not kept
+        # keep the functions having two positions(there are branches in the function dispatcher)
+        keep = copy(self.positions_contain_GT)
+        for ftn_selector in ftn_selectors_valid:
+            keep += self.functions_to_positions[ftn_selector]
+
+        not_kept = [p for p in self.all_positions_related_function if p not in keep]
+
+         # combine instruction groups
+        combined_instructions = []
+        for p in range(0,len(self.positions_to_instructions) - 1):
+            if p not in not_kept:
+                combined_instructions += self.positions_to_instructions[p]
+            else:
+                # replace with EMPTY instructions
+                empty_instructions = []  # do not remove them, it will cause inconsistency in terms of the total number of instructions
+                for instruction in self.positions_to_instructions[p]:
+                    empty_instructions.append({"address": instruction["address"], "opcode": "EMPTY"})
+
+                combined_instructions += empty_instructions
+
+        # before combining the last instruction group (the instructions of regular functions)
+        # If the last non-EMPTY opcode is DUP,remove it in the already combined instructions
+        for index in range(len(combined_instructions) - 1, 0, -1):
+            if str(combined_instructions[index]['opcode']).__eq__('EMPTY'):
+                continue
+            else:
+                if str(combined_instructions[index]['opcode']).__eq__('DUP1'):
+                    instruction = combined_instructions[index]
+                    combined_instructions[index] = {"address": instruction["address"], "opcode": "EMPTY"}
+
+                break
+
+
+        #
+        for p,idx in self.jumpdest_in_dispatcher:
+            idx=idx-1
+            while True:
+                instruction=combined_instructions[idx]
+                opcode=instruction['opcode']
+                if str(opcode).__eq__('EMPTY'):
+                    idx = idx - 1
+                    continue
+                else:
+                    if str(opcode) in ['JUMPDEST','PUSH4']:
+                        break
+                    if str(opcode).__eq__('DUP1'):
+                        combined_instructions[idx] = {"address": instruction["address"], "opcode": "EMPTY"}
+                    break
+
+        # print_list(combined_instructions)
+        combined_instructions += self.positions_to_instructions[len(self.positions_to_instructions) - 1]
+
+
+        return combined_instructions
+
+    def modify_no_modification(self,state:WorldState):
+        state.accounts[self.contract_address.value].code.instruction_list = self.instruction_list
+
```

### Comparing `smartExecutorx-0.3/fdg/output_data.py` & `smartExecutorx-4.0/fdg/output_data.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/fdg/preprocessing/address_collection.py` & `smartExecutorx-4.0/fdg/preprocessing/address_collection.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/fdg/preprocessing/instruction_coverage.py` & `smartExecutorx-4.0/fdg/preprocessing/instruction_coverage.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/fdg/preprocessing/preprocess.py` & `smartExecutorx-4.0/fdg/preprocessing/preprocess.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-import time
-from copy import deepcopy, copy
-
-import fdg.global_config
-from fdg.output_data import output_key_to_slot
-
-from fdg.preprocessing.instruction_coverage import InstructionCoverage
-
-from fdg.preprocessing.read_in_conditions import ReadInCondition
-from fdg.preprocessing.slot_location import expression_str_to_slot
-
-from fdg.preprocessing.write_read_info import Function_Write_Read_Info
-from mythril.laser.ethereum.function_managers.keccak_function_manager import keccak_function_manager
-from mythril.laser.ethereum.strategy.basic import DepthFirstSearchStrategy, BreadthFirstSearchStrategy
-from mythril.laser.ethereum.strategy.extensions.bounded_loops import BoundedLoopsStrategy
-
-
-import logging
-
-from mythril.laser.ethereum.transaction.symbolic import execute_message_call_preprocessing
-
-log = logging.getLogger(__name__)
-"""
-For each function:
-    need to collect conditions
-    instruction indices
-    read/write slots
-
-expression to slot map (can not simplify expression, because the slot information can be lost if the expression can simplified to a concrete value.
-
-concrete addresses used in the contract, which may be used to check against msg.sender which is implemented an array of three concrete addresses by default
-
-"""
-class Preprocessing():
-    def __init__(self,method_identifiers:dict,state,contract_address):
-        self.function_to_signature=method_identifiers
-
-        self.read_in_conditions=ReadInCondition(list(method_identifiers.keys()))
-        # print_dict(method_identifiers,"function and signature")
-
-        self.write_read_info=Function_Write_Read_Info(list(method_identifiers.keys()))
-
-        self.instruction_cov=InstructionCoverage(list(method_identifiers.keys()))
-
-
-        self.timeout=False
-        self.coverage=0
-
-        self.save_keccak_function_manager=None
-
-    def main_preprocessing_start(self,iteration:int,laserEVM):
-        fdg.global_config.tx_len = 1  # temporarily used as a flag
-        log.info(f'start_iteration preprocessing.')
-
-        # save keccak_function_manager
-        self.save_keccak_function_manager=deepcopy(keccak_function_manager)
-
-        laserEVM.open_states = laserEVM.open_states[0:1]
-
-        # laserEVM.strategy=DepthFirstSearchStrategy(laserEVM.work_list,laserEVM.max_depth)
-        laserEVM.strategy = BreadthFirstSearchStrategy(laserEVM.work_list, laserEVM.max_depth)
-
-        laserEVM.extend_strategy(BoundedLoopsStrategy, loop_bound=2)
-        return
-
-
-    def main_preprocessing_end(self, iteration:int):
-        # set back the save data
-        keccak_function_manager.set_data(self.save_keccak_function_manager)
-
-        self.timeout = fdg.global_config.flag_preprocess_timeout
-        self.coverage=self.instruction_cov.call_at_end_of_preprocessing()
-
-        seconds_start = time.time()
-
-        output_key_to_slot(expression_str_to_slot,'key_to_slot.txt','hash values to the corresponding slots')
-
-        self.write_read_info.refine_read_write_slots()
-        self.write_read_info.print_write_read_info()  #output
-
-        seconds_end = time.time()
-        # print(f'self.write_read_info time(s):{seconds_end - seconds_start}')
-
-        seconds_start = time.time()
-
-        self.read_in_conditions.extract_read_slots_in_conditions()
-        self.read_in_conditions.print_read_slot_info()
-
-        seconds_end = time.time()
-        # print(f'self.read_in_conditions time(s):{seconds_end - seconds_start}')
-
-        # print(f'\n==== expression_str_to_slot ====')
-        # for key,value in expression_str_to_slot.items():
-        #     print(f'\texpression: {key}')
-        #     print(f'\tslot: {value}')
-
-        log.info(f'end preprocessing.')
-        return
-
-
-
-
-def execute_preprocessing(address, laserEVM):
-
-    begin = time.time()
-    print("Starting preprocessing.")
-    fdg.global_config.flag_preprocessing = True
-
-    # doing preprocesing on a copy of laserEVM.
-    # the problem of doing preprocessing on the original laserEVM is that
-    # it is hard to set the current state of laserEVM to the previous laserEVM state (generated after contract creation transaction)
-
-
-    for hook in laserEVM._start_sym_trans_hooks_laserEVM:
-        hook(laserEVM)
-
-    execute_message_call_preprocessing(laserEVM, address)
-
-    for hook in laserEVM._stop_sym_trans_hooks_laserEVM:
-        hook(laserEVM)
-
-    fdg.global_config.flag_preprocessing = False
-
-    print("Ending preprocessing.")#
-    end = time.time()
-    print(f"preprocessing time(s): {end - begin}")
-
+import time
+from copy import deepcopy, copy
+
+import fdg.global_config
+from fdg.output_data import output_key_to_slot
+
+from fdg.preprocessing.instruction_coverage import InstructionCoverage
+
+from fdg.preprocessing.read_in_conditions import ReadInCondition
+from fdg.preprocessing.slot_location import expression_str_to_slot
+
+from fdg.preprocessing.write_read_info import Function_Write_Read_Info
+from mythril.laser.ethereum.function_managers.keccak_function_manager import keccak_function_manager
+from mythril.laser.ethereum.strategy.basic import DepthFirstSearchStrategy, BreadthFirstSearchStrategy
+from mythril.laser.ethereum.strategy.extensions.bounded_loops import BoundedLoopsStrategy
+
+
+import logging
+
+from mythril.laser.ethereum.transaction.symbolic import execute_message_call_preprocessing
+
+log = logging.getLogger(__name__)
+"""
+For each function:
+    need to collect conditions
+    instruction indices
+    read/write slots
+
+expression to slot map (can not simplify expression, because the slot information can be lost if the expression can simplified to a concrete value.
+
+concrete addresses used in the contract, which may be used to check against msg.sender which is implemented an array of three concrete addresses by default
+
+"""
+class Preprocessing():
+    def __init__(self,method_identifiers:dict,state,contract_address):
+        self.function_to_signature=method_identifiers
+
+        self.read_in_conditions=ReadInCondition(list(method_identifiers.keys()))
+        # print_dict(method_identifiers,"function and signature")
+
+        self.write_read_info=Function_Write_Read_Info(list(method_identifiers.keys()))
+
+        self.instruction_cov=InstructionCoverage(list(method_identifiers.keys()))
+
+
+        self.timeout=False
+        self.coverage=0
+
+        self.save_keccak_function_manager=None
+
+    def main_preprocessing_start(self,iteration:int,laserEVM):
+        fdg.global_config.tx_len = 1  # temporarily used as a flag
+        log.info(f'start_iteration preprocessing.')
+
+        # save keccak_function_manager
+        self.save_keccak_function_manager=deepcopy(keccak_function_manager)
+
+        laserEVM.open_states = laserEVM.open_states[0:1]
+
+        # laserEVM.strategy=DepthFirstSearchStrategy(laserEVM.work_list,laserEVM.max_depth)
+        laserEVM.strategy = BreadthFirstSearchStrategy(laserEVM.work_list, laserEVM.max_depth)
+
+        laserEVM.extend_strategy(BoundedLoopsStrategy, loop_bound=2)
+        return
+
+
+    def main_preprocessing_end(self, iteration:int):
+        # set back the save data
+        keccak_function_manager.set_data(self.save_keccak_function_manager)
+
+        self.timeout = fdg.global_config.flag_preprocess_timeout
+        self.coverage=self.instruction_cov.call_at_end_of_preprocessing()
+
+        seconds_start = time.time()
+
+        output_key_to_slot(expression_str_to_slot,'key_to_slot.txt','hash values to the corresponding slots')
+
+        self.write_read_info.refine_read_write_slots()
+        self.write_read_info.print_write_read_info()  #output
+
+        seconds_end = time.time()
+        # print(f'self.write_read_info time(s):{seconds_end - seconds_start}')
+
+        seconds_start = time.time()
+
+        self.read_in_conditions.extract_read_slots_in_conditions()
+        self.read_in_conditions.print_read_slot_info()
+
+        seconds_end = time.time()
+        # print(f'self.read_in_conditions time(s):{seconds_end - seconds_start}')
+
+        # print(f'\n==== expression_str_to_slot ====')
+        # for key,value in expression_str_to_slot.items():
+        #     print(f'\texpression: {key}')
+        #     print(f'\tslot: {value}')
+
+        log.info(f'end preprocessing.')
+        return
+
+
+
+
+def execute_preprocessing(address, laserEVM):
+
+    begin = time.time()
+    print("Starting preprocessing.")
+    fdg.global_config.flag_preprocessing = True
+
+    # doing preprocesing on a copy of laserEVM.
+    # the problem of doing preprocessing on the original laserEVM is that
+    # it is hard to set the current state of laserEVM to the previous laserEVM state (generated after contract creation transaction)
+
+
+    for hook in laserEVM._start_sym_trans_hooks_laserEVM:
+        hook(laserEVM)
+
+    execute_message_call_preprocessing(laserEVM, address)
+
+    for hook in laserEVM._stop_sym_trans_hooks_laserEVM:
+        hook(laserEVM)
+
+    fdg.global_config.flag_preprocessing = False
+
+    print("Ending preprocessing.")#
+    end = time.time()
+    print(f"preprocessing time(s): {end - begin}")
+
```

### Comparing `smartExecutorx-0.3/fdg/preprocessing/slot_location.py` & `smartExecutorx-4.0/fdg/preprocessing/slot_location.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-import re
-from copy import copy
-
-import fdg
-from fdg.preprocessing.address_collection import collect_value_for_sender
-from fdg.utils import str_without_space_line
-
-
-from mythril.laser.smt import (
-    BitVec,
-)
-from z3 import BitVecRef, BitVecNumRef, Z3Exception
-from mythril.laser.smt.expression import simplify_yes
-"""
-extract the storage locations from Concat() expressions, condition expressions, and (not know yet)
-
-observation: the expression can be extracted multiple times, so, saving the extracted results
-On HoloToken.sol: before saving the results: 28 times
-after saving the results: 6
-
-"""
-
-#----------------------------------------------
-# key refers to the location in the storage, it is created through hash function
-# the value of get_empty_keccak_hash
-# 89477152217924674838424037953991966239322087453347756267410168184682657981552
-
-
-# used to keep symbolic expressions and their mapped slots
-# saved when identify slots from given expressions
-expression_str_to_slot={}
-
-max_length=10000 # refers the length of the str version of a symbolic expression
-
-
-def map_concrete_hash_key_to_slot(expression:BitVec, data:BitVec):
-    """
-    pplied in create_keccak(self, data: BitVec) n keccak_function_manager.py module
-    """
-    sim_exp=simplify_yes(expression)
-    if not sim_exp.symbolic:
-        expr_str = str_without_space_line(expression)
-        data_str = str_without_space_line(data)
-        if expr_str not in expression_str_to_slot.keys():
-            if data_str in expression_str_to_slot.keys():
-                final_data_str =expression_str_to_slot[data_str]
-                expression_str_to_slot[expr_str] = final_data_str
-            else:
-                expression_str_to_slot[expr_str] = data_str
-
-
-def get_slot_from_location_expression(concat_expr:BitVec)->str:
-    """
-
-    get the locations of storage from expressions:
-        Concat(0,x,location)
-        keccak256_512(Concat(0,x,location))
-        need to think about the case of array
-
-    also consider the case of concrete hash, the location info is collected in a place where it is created.
-    used in preprocessing
-    """
-    def map_expr_str_to_slot(expr_str:str)->str:
-        matched_expr = find_matched_expr(expr_str,
-                                         expression_str_to_slot.keys())
-        if matched_expr is not None:
-            temp = expression_str_to_slot[matched_expr]
-            if temp in expression_str_to_slot.keys():
-                return expression_str_to_slot[temp]
-            else:
-                return temp
-
-        slot = expr_str
-        # save the result
-        if expr_str not in expression_str_to_slot.keys():
-            expression_str_to_slot[expr_str] = slot
-        return slot
-
-    def find_matched_expr(expr:str, expr_list:list)->str:
-        if len(expr)>=10:
-            expr_prefix=expr[0:len(expr)-2]
-            for e in expr_list:
-                if str(e[0:len(e)-2]).__eq__(expr_prefix):
-                    return e
-            return None
-        else:
-            if expr in expr_list:
-                return expr
-            else:
-                return None
-    if isinstance(concat_expr,BitVec):
-        if not concat_expr.symbolic:
-            # in case of a concrete hash, find it corresponding slot from a map
-            expr_str= str_without_space_line(concat_expr)
-            # check if it is already considered once
-            return map_expr_str_to_slot(expr_str)
-
-
-    if isinstance(concat_expr, str):
-        if concat_expr.isdigit():
-            return map_expr_str_to_slot(concat_expr)
-
-    str_data = str_without_space_line(concat_expr)
-    # handle the case: 62514009886607029107290561805838585334079798074568712924583230797734656856475 +
-    # Concat(If(1_calldatasize <= 4, 0, 1_calldata[4]),
-    if str_data.count('+')==1:
-        items=str_data.split('+')
-        if items[0].isdigit() and len(items[0]) >= 10:
-            return map_expr_str_to_slot(items[0])
-        else:
-            str_data = items[1]
-
-    last_parameter = ""
-    try:
-        # handle the case below:
-        # 1+keccak256_512(Concat(If(1_calldatasize<=4...)
-        # 2+keccak256_512(Concat(If(1_calldatasize<=4...)
-        pattern = r"^(\d+\+)\w+"
-        results=re.search(pattern, str_data)
-        if results:
-            # get the str that
-            str_data=str_data.split(results.group(1))[-1]
-
-        # check if it is already considered once
-        if str_data in expression_str_to_slot.keys():
-            last_parameter= expression_str_to_slot[str_data]
-        else:
-            if str_data.startswith('keccak256_512'):
-                # Use regular expressions to find the last parameter within the keccak256_512 function
-                last_parameter = re.search(r'keccak256_512\(.*?,(\d+)\)',
-                                           str_data)
-            else:
-                # Use regular expressions to find the last parameter within the Concat function
-                last_parameter = re.search(r'Concat\(.*?,(\d+)\)', str_data)
-
-            if last_parameter is not None:
-                last_parameter=last_parameter.group(1)
-                # print(f'(new) exp:{str_data}')
-                # print(f'(new) slot:{last_parameter}')
-
-                # save the result
-                expression_str_to_slot[str_data] = str(last_parameter)
-            else:
-                # print(f'Failed to identify a slot from {concat_expr}')
-                last_parameter=""
-
-    except Z3Exception as ze:
-        print(f'Have Z3Exception: {concat_expr}')
-    finally:
-        return  last_parameter
-
-def extract_locations_read_in_storage_in_a_condition(condition: BitVec)->list:
-    """
-        collect the storage locations read in a conditions:'If(If(255&UDiv(Store(Store(K(BitVec(256),0),4,0),0,1004753105490295263244812946565948198177742958590)[4],1)==0,1,0)==0,1,0)'
-        collect the addresses that are compared with msg.sender
-    """
-    # get the str versions of condition and its simplified expression.
-
-    condi_str = str_without_space_line(str(condition))
-
-    simplified_condition = simplify_yes(copy(condition))
-    simplified_condi_str = str_without_space_line(str(simplified_condition))
-
-
-    # select which condition to consider
-    # not simplified condition may contain ",...,...)[...],...))"
-    # simplified condition may lose the storage read information
-
-    if 'Store(K' in simplified_condi_str:
-        temp_condi = simplified_condition
-
-    elif 'Store(K' in condi_str:
-        temp_condi = condition
-
-    else:
-        return []
-
-    # collect the value that is compared with msg.sender
-    if fdg.global_config.optimization == 1:
-        collect_value_for_sender(simplified_condi_str)
-
-    # collect the locations of the storage that are read.
-    locations = []
-    try:
-        if isinstance(temp_condi, BitVec):
-            def go_deep(item: BitVecRef):
-                if isinstance(item, BitVecNumRef):
-                    return
-                elif str(item.decl()) == 'Select':
-                    children = item.children()
-                    if str(children[0].decl()) == 'Store':
-                        if children[1] not in locations:
-                            # the second child is the position of the storage
-                            # raw = z3.BitVecVal(value, size)
-                            # return BitVec(raw, annotations)
-                            locations.append(BitVec(children[1]))
-                    return
-                else:
-                    for child in item.children():
-                        go_deep(child)
-
-            condi_raw = temp_condi.raw
-            for item in condi_raw.children():
-                go_deep(item)
-    except:
-        pass
-    finally:
-        return locations
-
-
-
+import re
+from copy import copy
+
+import fdg
+from fdg.preprocessing.address_collection import collect_value_for_sender
+from fdg.utils import str_without_space_line
+
+
+from mythril.laser.smt import (
+    BitVec,
+)
+from z3 import BitVecRef, BitVecNumRef, Z3Exception
+from mythril.laser.smt.expression import simplify_yes
+"""
+extract the storage locations from Concat() expressions, condition expressions, and (not know yet)
+
+observation: the expression can be extracted multiple times, so, saving the extracted results
+On HoloToken.sol: before saving the results: 28 times
+after saving the results: 6
+
+"""
+
+#----------------------------------------------
+# key refers to the location in the storage, it is created through hash function
+# the value of get_empty_keccak_hash
+# 89477152217924674838424037953991966239322087453347756267410168184682657981552
+
+
+# used to keep symbolic expressions and their mapped slots
+# saved when identify slots from given expressions
+expression_str_to_slot={}
+
+max_length=10000 # refers the length of the str version of a symbolic expression
+
+
+def map_concrete_hash_key_to_slot(expression:BitVec, data:BitVec):
+    """
+    pplied in create_keccak(self, data: BitVec) n keccak_function_manager.py module
+    """
+    sim_exp=simplify_yes(expression)
+    if not sim_exp.symbolic:
+        expr_str = str_without_space_line(expression)
+        data_str = str_without_space_line(data)
+        if expr_str not in expression_str_to_slot.keys():
+            if data_str in expression_str_to_slot.keys():
+                final_data_str =expression_str_to_slot[data_str]
+                expression_str_to_slot[expr_str] = final_data_str
+            else:
+                expression_str_to_slot[expr_str] = data_str
+
+
+def get_slot_from_location_expression(concat_expr:BitVec)->str:
+    """
+
+    get the locations of storage from expressions:
+        Concat(0,x,location)
+        keccak256_512(Concat(0,x,location))
+        need to think about the case of array
+
+    also consider the case of concrete hash, the location info is collected in a place where it is created.
+    used in preprocessing
+    """
+    def map_expr_str_to_slot(expr_str:str)->str:
+        matched_expr = find_matched_expr(expr_str,
+                                         expression_str_to_slot.keys())
+        if matched_expr is not None:
+            temp = expression_str_to_slot[matched_expr]
+            if temp in expression_str_to_slot.keys():
+                return expression_str_to_slot[temp]
+            else:
+                return temp
+
+        slot = expr_str
+        # save the result
+        if expr_str not in expression_str_to_slot.keys():
+            expression_str_to_slot[expr_str] = slot
+        return slot
+
+    def find_matched_expr(expr:str, expr_list:list)->str:
+        if len(expr)>=10:
+            expr_prefix=expr[0:len(expr)-2]
+            for e in expr_list:
+                if str(e[0:len(e)-2]).__eq__(expr_prefix):
+                    return e
+            return None
+        else:
+            if expr in expr_list:
+                return expr
+            else:
+                return None
+    if isinstance(concat_expr,BitVec):
+        if not concat_expr.symbolic:
+            # in case of a concrete hash, find it corresponding slot from a map
+            expr_str= str_without_space_line(concat_expr)
+            # check if it is already considered once
+            return map_expr_str_to_slot(expr_str)
+
+
+    if isinstance(concat_expr, str):
+        if concat_expr.isdigit():
+            return map_expr_str_to_slot(concat_expr)
+
+    str_data = str_without_space_line(concat_expr)
+    # handle the case: 62514009886607029107290561805838585334079798074568712924583230797734656856475 +
+    # Concat(If(1_calldatasize <= 4, 0, 1_calldata[4]),
+    if str_data.count('+')==1:
+        items=str_data.split('+')
+        if items[0].isdigit() and len(items[0]) >= 10:
+            return map_expr_str_to_slot(items[0])
+        else:
+            str_data = items[1]
+
+    last_parameter = ""
+    try:
+        # handle the case below:
+        # 1+keccak256_512(Concat(If(1_calldatasize<=4...)
+        # 2+keccak256_512(Concat(If(1_calldatasize<=4...)
+        pattern = r"^(\d+\+)\w+"
+        results=re.search(pattern, str_data)
+        if results:
+            # get the str that
+            str_data=str_data.split(results.group(1))[-1]
+
+        # check if it is already considered once
+        if str_data in expression_str_to_slot.keys():
+            last_parameter= expression_str_to_slot[str_data]
+        else:
+            if str_data.startswith('keccak256_512'):
+                # Use regular expressions to find the last parameter within the keccak256_512 function
+                last_parameter = re.search(r'keccak256_512\(.*?,(\d+)\)',
+                                           str_data)
+            else:
+                # Use regular expressions to find the last parameter within the Concat function
+                last_parameter = re.search(r'Concat\(.*?,(\d+)\)', str_data)
+
+            if last_parameter is not None:
+                last_parameter=last_parameter.group(1)
+                # print(f'(new) exp:{str_data}')
+                # print(f'(new) slot:{last_parameter}')
+
+                # save the result
+                expression_str_to_slot[str_data] = str(last_parameter)
+            else:
+                # print(f'Failed to identify a slot from {concat_expr}')
+                last_parameter=""
+
+    except Z3Exception as ze:
+        print(f'Have Z3Exception: {concat_expr}')
+    finally:
+        return  last_parameter
+
+def extract_locations_read_in_storage_in_a_condition(condition: BitVec)->list:
+    """
+        collect the storage locations read in a conditions:'If(If(255&UDiv(Store(Store(K(BitVec(256),0),4,0),0,1004753105490295263244812946565948198177742958590)[4],1)==0,1,0)==0,1,0)'
+        collect the addresses that are compared with msg.sender
+    """
+    # get the str versions of condition and its simplified expression.
+
+    condi_str = str_without_space_line(str(condition))
+
+    simplified_condition = simplify_yes(copy(condition))
+    simplified_condi_str = str_without_space_line(str(simplified_condition))
+
+
+    # select which condition to consider
+    # not simplified condition may contain ",...,...)[...],...))"
+    # simplified condition may lose the storage read information
+
+    if 'Store(K' in simplified_condi_str:
+        temp_condi = simplified_condition
+
+    elif 'Store(K' in condi_str:
+        temp_condi = condition
+
+    else:
+        return []
+
+    # collect the value that is compared with msg.sender
+    if fdg.global_config.optimization == 1:
+        collect_value_for_sender(simplified_condi_str)
+
+    # collect the locations of the storage that are read.
+    locations = []
+    try:
+        if isinstance(temp_condi, BitVec):
+            def go_deep(item: BitVecRef):
+                if isinstance(item, BitVecNumRef):
+                    return
+                elif str(item.decl()) == 'Select':
+                    children = item.children()
+                    if str(children[0].decl()) == 'Store':
+                        if children[1] not in locations:
+                            # the second child is the position of the storage
+                            # raw = z3.BitVecVal(value, size)
+                            # return BitVec(raw, annotations)
+                            locations.append(BitVec(children[1]))
+                    return
+                else:
+                    for child in item.children():
+                        go_deep(child)
+
+            condi_raw = temp_condi.raw
+            for item in condi_raw.children():
+                go_deep(item)
+    except:
+        pass
+    finally:
+        return locations
+
+
+
```

### Comparing `smartExecutorx-0.3/fdg/preprocessing/write_read_info.py` & `smartExecutorx-4.0/fdg/preprocessing/write_read_info.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/fdg/utils.py` & `smartExecutorx-4.0/fdg/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -148,35 +148,8 @@
     if '#' in key:
         return key.split('#')[0:-1]
     else:
         return [key]
 
 
 
-if __name__ == '__main__':
-    # import numpy as np
-    # print(get_binary(7,16))
-    # print(get_binary(6,16))
-    # print(np.random.choice(range(10), size=2, replace=False))
-    # print(get_combination_for_a_list([1,2,3],3))
-    # print(get_combination([["1","2"], ["b"]], 2))
-    #
-    # sv1_seq_indices = range(2)
-    # sv2_seq_indices = range(1)
-    # sv3_seq_indices = range(2)
-    # comb_indices = get_combination([sv1_seq_indices, sv2_seq_indices,sv3_seq_indices], 3)
-    # print(comb_indices)
-
-    a=[1,2,3]
-    b=[1,2,3]
-    print(f'a={hash_for_list(a)}\nb={hash_for_list(b)}')
-    a=[0,1,2,3]
-    select=random_indices(0,3,2)
-    b=[item for idx,item in enumerate(a) if idx in select]
-    print(f'a={a}')
-    print(f'select={select}')
-    print(f'b={b}')
-
-    print(get_key_1_prefix("2#2#4"))
-
-
```

### Comparing `smartExecutorx-0.3/mythril/analysis/call_helpers.py` & `smartExecutorx-4.0/mythril/analysis/call_helpers.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/callgraph.py` & `smartExecutorx-4.0/mythril/analysis/callgraph.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/issue_annotation.py` & `smartExecutorx-4.0/mythril/analysis/issue_annotation.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/base.py` & `smartExecutorx-4.0/mythril/analysis/module/base.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/loader.py` & `smartExecutorx-4.0/mythril/analysis/module/loader.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/modules/arbitrary_jump.py` & `smartExecutorx-4.0/mythril/analysis/module/modules/arbitrary_jump.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/modules/arbitrary_write.py` & `smartExecutorx-4.0/mythril/analysis/module/modules/arbitrary_write.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/modules/delegatecall.py` & `smartExecutorx-4.0/mythril/analysis/module/modules/delegatecall.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/modules/dependence_on_origin.py` & `smartExecutorx-4.0/mythril/analysis/module/modules/dependence_on_origin.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/modules/dependence_on_predictable_vars.py` & `smartExecutorx-4.0/mythril/analysis/module/modules/dependence_on_predictable_vars.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/modules/ether_thief.py` & `smartExecutorx-4.0/mythril/analysis/module/modules/ether_thief.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/modules/exceptions.py` & `smartExecutorx-4.0/mythril/analysis/module/modules/exceptions.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/modules/external_calls.py` & `smartExecutorx-4.0/mythril/analysis/module/modules/external_calls.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/modules/integer.py` & `smartExecutorx-4.0/mythril/analysis/module/modules/integer.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/modules/multiple_sends.py` & `smartExecutorx-4.0/mythril/analysis/module/modules/multiple_sends.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/modules/state_change_external_calls.py` & `smartExecutorx-4.0/mythril/analysis/module/modules/state_change_external_calls.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/modules/suicide.py` & `smartExecutorx-4.0/mythril/analysis/module/modules/suicide.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/modules/unchecked_retval.py` & `smartExecutorx-4.0/mythril/analysis/module/modules/unchecked_retval.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/modules/user_assertions.py` & `smartExecutorx-4.0/mythril/analysis/module/modules/user_assertions.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/module/util.py` & `smartExecutorx-4.0/mythril/analysis/module/util.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/ops.py` & `smartExecutorx-4.0/mythril/analysis/ops.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/potential_issues.py` & `smartExecutorx-4.0/mythril/analysis/potential_issues.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/report.py` & `smartExecutorx-4.0/mythril/analysis/report.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/security.py` & `smartExecutorx-4.0/mythril/analysis/security.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/solver.py` & `smartExecutorx-4.0/mythril/analysis/solver.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/swc_data.py` & `smartExecutorx-4.0/mythril/analysis/swc_data.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/symbolic.py` & `smartExecutorx-4.0/mythril/analysis/symbolic.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/templates/callgraph.html` & `smartExecutorx-4.0/mythril/analysis/templates/callgraph.html`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/templates/report_as_markdown.jinja2` & `smartExecutorx-4.0/mythril/analysis/templates/report_as_markdown.jinja2`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/templates/report_as_text.jinja2` & `smartExecutorx-4.0/mythril/analysis/templates/report_as_text.jinja2`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/analysis/traceexplore.py` & `smartExecutorx-4.0/mythril/analysis/traceexplore.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/concolic/concolic_execution.py` & `smartExecutorx-4.0/mythril/concolic/concolic_execution.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/concolic/concrete_data.py` & `smartExecutorx-4.0/mythril/concolic/concrete_data.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/concolic/find_trace.py` & `smartExecutorx-4.0/mythril/concolic/find_trace.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/disassembler/asm.py` & `smartExecutorx-4.0/mythril/disassembler/asm.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/disassembler/disassembly.py` & `smartExecutorx-4.0/mythril/disassembler/disassembly.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/ethereum/evmcontract.py` & `smartExecutorx-4.0/mythril/ethereum/evmcontract.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/ethereum/interface/rpc/base_client.py` & `smartExecutorx-4.0/mythril/ethereum/interface/rpc/base_client.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/ethereum/interface/rpc/client.py` & `smartExecutorx-4.0/mythril/ethereum/interface/rpc/client.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/ethereum/interface/rpc/exceptions.py` & `smartExecutorx-4.0/mythril/ethereum/interface/rpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/ethereum/interface/rpc/utils.py` & `smartExecutorx-4.0/mythril/ethereum/interface/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/ethereum/util.py` & `smartExecutorx-4.0/mythril/ethereum/util.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/exceptions.py` & `smartExecutorx-4.0/mythril/exceptions.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/interfaces/cli.py` & `smartExecutorx-4.0/mythril/interfaces/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -463,16 +463,17 @@
         help="specify the code coverage threshold that is used to determine deep functions",
     )
 
     # @wei
     options.add_argument(
         "-fss",
         "--function-search-strategy",
-        choices=["dfs", "bfs", "mine", 'seq','mine1'],
-        default="bfs",
+        choices=["dfs", "bfs", "mine", 'seq'],
+        default="mine",
+
         help="Function data flow graph search strategy",
     )
 
     # @wei
     options.add_argument(
         "-seq",
         "--sequences",
@@ -486,14 +487,22 @@
         "--print-function-coverage",
         type=int,
         default=1,
         help="0: no; 1:print function coverage",
     )
 
     options.add_argument(
+        "-p1dl",
+        "--phase1-depth-limit",
+        type=int,
+        default=1,
+        help="determine the depth limit of the sequences in Phase 1"
+    )
+
+    options.add_argument(
         "--preprocess-timeout",
         type=int,
         default=100,
         help="The amount of seconds to spend on the preprocess",
     )
 
     options.add_argument(
@@ -507,41 +516,52 @@
         "--random-baseline",
         type=int,
         default=0,  # 0 means the baseline is inactive
         help=" with values from  0 to 10. indicate the percent of functions to be considered",
     )
 
 def add_fwrg_arguments(args: Namespace):
-    # @wei
+    """
+    collect the values for the global parameters defined in fdg.global_config.py.
+    """
     fdg.global_config.function_coverage_threshold = args.function_coverage_threshold
     fdg.global_config.function_search_strategy = args.function_search_strategy
     fdg.global_config.sequences = args.sequences
     fdg.global_config.random_baseline = args.random_baseline
 
     fdg.global_config.print_function_coverage = args.print_function_coverage
-
+    fdg.global_config.p1_dl=args.phase1_depth_limit
     fdg.global_config.preprocess_timeout = args.preprocess_timeout
     fdg.global_config.optimization = args.optimization
     fdg.global_config.flag_consider_all_reads = args.consider_all_reads
     fdg.global_config.execution_times_limit = args.execution_times_limit
-
-    fdg.global_config.flag_fwrg=args.function_wr_graph
-
+    if args.no_guidance:
+        fdg.global_config.flag_fwrg=False
+    else:
+        fdg.global_config.flag_fwrg=True
+    # fdg.global_config.flag_fwrg=args.function_wr_graph
     if args.v>=3:
         fdg.output_data.flag_basic=True
 
 def add_analysis_args(options):
     """
     Adds arguments for analysis
 
     :param options: Analysis Options
     """
     options.add_argument(
         "-fdg",
         "--function-wr-graph",
+        default=True,
+        action="store_true", #
+        help="use guided exploration",
+    )
+    options.add_argument(
+
+        "--no-guidance",
         default=False,
         action="store_true",
         help="use guided exploration",
     )
 
     options.add_argument(
         "-m",
@@ -1024,15 +1044,15 @@
         parser.print_help()
         sys.exit()
 
     if args.command == VERSION_COMMAND:
         if args.outform == "json":
             print(json.dumps({"version_str": VERSION}))
         else:
-            print("Mythril version {}".format(VERSION))
+            print("SmartExecutor version {}".format(VERSION))
         sys.exit()
 
     if args.command == LIST_DETECTORS_COMMAND:
         modules = []
         for module in ModuleLoader().get_detection_modules():
             modules.append({"classname": type(module).__name__, "title": module.name})
         if args.outform == "json":
```

### Comparing `smartExecutorx-0.3/mythril/interfaces/epic.py` & `smartExecutorx-4.0/mythril/interfaces/epic.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/call.py` & `smartExecutorx-4.0/mythril/laser/ethereum/call.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/cfg.py` & `smartExecutorx-4.0/mythril/laser/ethereum/cfg.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/cheat_code.py` & `smartExecutorx-4.0/mythril/laser/ethereum/cheat_code.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/evm_exceptions.py` & `smartExecutorx-4.0/mythril/laser/ethereum/evm_exceptions.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/function_managers/exponent_function_manager.py` & `smartExecutorx-4.0/mythril/laser/ethereum/function_managers/exponent_function_manager.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/function_managers/keccak_function_manager.py` & `smartExecutorx-4.0/mythril/laser/ethereum/function_managers/keccak_function_manager.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/instruction_data.py` & `smartExecutorx-4.0/mythril/laser/ethereum/instruction_data.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/instructions.py` & `smartExecutorx-4.0/mythril/laser/ethereum/instructions.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/natives.py` & `smartExecutorx-4.0/mythril/laser/ethereum/natives.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/state/account.py` & `smartExecutorx-4.0/mythril/laser/ethereum/state/account.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/state/annotation.py` & `smartExecutorx-4.0/mythril/laser/ethereum/state/annotation.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/state/calldata.py` & `smartExecutorx-4.0/mythril/laser/ethereum/state/calldata.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/state/constraints.py` & `smartExecutorx-4.0/mythril/laser/ethereum/state/constraints.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/state/environment.py` & `smartExecutorx-4.0/mythril/laser/ethereum/state/environment.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/state/global_state.py` & `smartExecutorx-4.0/mythril/laser/ethereum/state/global_state.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/state/machine_state.py` & `smartExecutorx-4.0/mythril/laser/ethereum/state/machine_state.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/state/memory.py` & `smartExecutorx-4.0/mythril/laser/ethereum/state/memory.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/state/return_data.py` & `smartExecutorx-4.0/mythril/laser/ethereum/state/return_data.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/state/world_state.py` & `smartExecutorx-4.0/mythril/laser/ethereum/state/world_state.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/strategy/__init__.py` & `smartExecutorx-4.0/mythril/laser/ethereum/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/strategy/basic.py` & `smartExecutorx-4.0/mythril/laser/ethereum/strategy/basic.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/strategy/beam.py` & `smartExecutorx-4.0/mythril/laser/ethereum/strategy/beam.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/strategy/concolic.py` & `smartExecutorx-4.0/mythril/laser/ethereum/strategy/concolic.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/strategy/constraint_strategy.py` & `smartExecutorx-4.0/mythril/laser/ethereum/strategy/constraint_strategy.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/strategy/extensions/bounded_loops.py` & `smartExecutorx-4.0/mythril/laser/ethereum/strategy/extensions/bounded_loops.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/svm.py` & `smartExecutorx-4.0/mythril/laser/ethereum/svm.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/time_handler.py` & `smartExecutorx-4.0/mythril/laser/ethereum/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/transaction/concolic.py` & `smartExecutorx-4.0/mythril/laser/ethereum/transaction/concolic.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/transaction/symbolic.py` & `smartExecutorx-4.0/mythril/laser/ethereum/transaction/symbolic.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/transaction/transaction_models.py` & `smartExecutorx-4.0/mythril/laser/ethereum/transaction/transaction_models.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/ethereum/util.py` & `smartExecutorx-4.0/mythril/laser/ethereum/util.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/plugin/__init__.py` & `smartExecutorx-4.0/mythril/laser/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/plugin/interface.py` & `smartExecutorx-4.0/mythril/laser/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/plugin/loader.py` & `smartExecutorx-4.0/mythril/laser/plugin/loader.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/plugin/plugins/__init__.py` & `smartExecutorx-4.0/mythril/laser/plugin/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/plugin/plugins/benchmark.py` & `smartExecutorx-4.0/mythril/laser/plugin/plugins/benchmark.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/plugin/plugins/call_depth_limiter.py` & `smartExecutorx-4.0/mythril/laser/plugin/plugins/call_depth_limiter.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/plugin/plugins/coverage/coverage_plugin.py` & `smartExecutorx-4.0/mythril/laser/plugin/plugins/coverage/coverage_plugin.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/plugin/plugins/coverage/coverage_strategy.py` & `smartExecutorx-4.0/mythril/laser/plugin/plugins/coverage/coverage_strategy.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/plugin/plugins/instruction_profiler.py` & `smartExecutorx-4.0/mythril/laser/plugin/plugins/instruction_profiler.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/plugin/plugins/mutation_pruner.py` & `smartExecutorx-4.0/mythril/laser/plugin/plugins/mutation_pruner.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/plugin/plugins/plugin_annotations.py` & `smartExecutorx-4.0/mythril/laser/plugin/plugins/plugin_annotations.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/plugin/signals.py` & `smartExecutorx-4.0/mythril/laser/plugin/signals.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/smt/__init__.py` & `smartExecutorx-4.0/mythril/laser/smt/__init__.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/smt/array.py` & `smartExecutorx-4.0/mythril/laser/smt/array.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/smt/bitvec.py` & `smartExecutorx-4.0/mythril/laser/smt/bitvec.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/smt/bitvec_helper.py` & `smartExecutorx-4.0/mythril/laser/smt/bitvec_helper.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/smt/bool.py` & `smartExecutorx-4.0/mythril/laser/smt/bool.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/smt/expression.py` & `smartExecutorx-4.0/mythril/laser/smt/expression.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/smt/function.py` & `smartExecutorx-4.0/mythril/laser/smt/function.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/smt/model.py` & `smartExecutorx-4.0/mythril/laser/smt/model.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/smt/solver/independence_solver.py` & `smartExecutorx-4.0/mythril/laser/smt/solver/independence_solver.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/laser/smt/solver/solver.py` & `smartExecutorx-4.0/mythril/laser/smt/solver/solver.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/mythril/mythril_analyzer.py` & `smartExecutorx-4.0/mythril/mythril/mythril_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 import logging
 import traceback
 from typing import Optional, List
 from argparse import Namespace
 
-from fdg.constraint_check_time import StateConstraintCheckIndicator
+
 from . import MythrilDisassembler
 from mythril.support.source_support import Source
 from mythril.support.loader import DynLoader
 from mythril.support.support_args import args
 from mythril.analysis.symbolic import SymExecWrapper
 from mythril.analysis.callgraph import generate_graph
 from mythril.analysis.traceexplore import get_serializable_statespace
@@ -138,15 +138,14 @@
         """
         :param modules: The analysis modules which should be executed
         :param transaction_count: The amount of transactions to be executed
         :return: The Report class which contains the all the issues/vulnerabilities
         """
         all_issues = []  # type: List[Issue]
         SolverStatistics().enabled = True
-        StateConstraintCheckIndicator().enabled = True  # @wei to record the time to check state constraints
 
         exceptions = []
         execution_info = None  # type: Optional[List[ExecutionInfo]]
         for contract in self.contracts:
             StartTime()  # Reinitialize start time for new contracts
             try:
                 sym = SymExecWrapper(
```

### Comparing `smartExecutorx-0.3/mythril/mythril/mythril_config.py` & `smartExecutorx-4.0/mythril/mythril/mythril_config.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/mythril/mythril_disassembler.py` & `smartExecutorx-4.0/mythril/mythril/mythril_disassembler.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/plugin/discovery.py` & `smartExecutorx-4.0/mythril/plugin/discovery.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/plugin/interface.py` & `smartExecutorx-4.0/mythril/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/plugin/loader.py` & `smartExecutorx-4.0/mythril/plugin/loader.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/solidity/soliditycontract.py` & `smartExecutorx-4.0/mythril/solidity/soliditycontract.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/support/assets/signatures.db` & `smartExecutorx-4.0/mythril/support/assets/signatures.db`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/support/loader.py` & `smartExecutorx-4.0/mythril/support/loader.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/support/lock.py` & `smartExecutorx-4.0/mythril/support/lock.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/support/model.py` & `smartExecutorx-4.0/mythril/support/model.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/support/opcodes.py` & `smartExecutorx-4.0/mythril/support/opcodes.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/support/signatures.py` & `smartExecutorx-4.0/mythril/support/signatures.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/support/source_support.py` & `smartExecutorx-4.0/mythril/support/source_support.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/support/support_args.py` & `smartExecutorx-4.0/mythril/support/support_args.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/mythril/support/support_utils.py` & `smartExecutorx-4.0/mythril/support/support_utils.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/requirements.txt` & `smartExecutorx-4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/setup.py` & `smartExecutorx-4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 TESTS_REQUIRE = ["mypy==0.782", "pytest>=3.6.0", "pytest_mock", "pytest-cov"]
 
 # What packages are optional?
 EXTRAS = {}
 
 # If version is set to None then it will be fetched from __version__.py
-VERSION = "v0.3"
+VERSION = "v4.0"
 
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
 try:
     with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
         long_description = "\n" + f.read()
```

### Comparing `smartExecutorx-0.3/smartExecutorx.egg-info/SOURCES.txt` & `smartExecutorx-4.0/smartExecutorx.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 fdg/__init__.py
 fdg/__version__.py
-fdg/constraint_check.py
-fdg/constraint_check_time.py
 fdg/expression_slot.py
 fdg/fdg_pruner.py
 fdg/function_coverage.py
 fdg/fwrg_manager.py
 fdg/global_config.py
 fdg/instruction_modification.py
 fdg/output_data.py
@@ -24,15 +22,14 @@
 fdg/preprocessing/__init__.py
 fdg/preprocessing/address_collection.py
 fdg/preprocessing/instruction_coverage.py
 fdg/preprocessing/preprocess.py
 fdg/preprocessing/read_in_conditions.py
 fdg/preprocessing/slot_location.py
 fdg/preprocessing/write_read_info.py
-images/exampleUsingDockerImage.png
 mythril/__init__.py
 mythril/__main__.py
 mythril/__version__.py
 mythril/exceptions.py
 mythril/analysis/__init__.py
 mythril/analysis/analysis_args.py
 mythril/analysis/call_helpers.py
```

### Comparing `smartExecutorx-0.3/smartExecutorx.egg-info/requires.txt` & `smartExecutorx-4.0/smartExecutorx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/disassembler/asm.py` & `smartExecutorx-4.0/tests/disassembler/asm.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/disassembler/disassembly.py` & `smartExecutorx-4.0/tests/disassembler/disassembly.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/instructions/berlin_fork_opcodes_test.py` & `smartExecutorx-4.0/tests/instructions/berlin_fork_opcodes_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/instructions/codecopy_test.py` & `smartExecutorx-4.0/tests/instructions/codecopy_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/instructions/create2_test.py` & `smartExecutorx-4.0/tests/instructions/create2_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/instructions/create_test.py` & `smartExecutorx-4.0/tests/instructions/create_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/instructions/extcodecopy_test.py` & `smartExecutorx-4.0/tests/instructions/extcodecopy_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/instructions/extcodehash_test.py` & `smartExecutorx-4.0/tests/instructions/extcodehash_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/instructions/sar_test.py` & `smartExecutorx-4.0/tests/instructions/sar_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/instructions/shl_test.py` & `smartExecutorx-4.0/tests/instructions/shl_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/instructions/shr_test.py` & `smartExecutorx-4.0/tests/instructions/shr_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/instructions/static_call_test.py` & `smartExecutorx-4.0/tests/instructions/static_call_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/instructions/test_basefee.py` & `smartExecutorx-4.0/tests/instructions/test_basefee.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/laser/keccak_tests.py` & `smartExecutorx-4.0/tests/laser/keccak_tests.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/laser/smt/independece_solver_test.py` & `smartExecutorx-4.0/tests/laser/smt/independece_solver_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/laser/smt/model_test.py` & `smartExecutorx-4.0/tests/laser/smt/model_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/laser/state/calldata_test.py` & `smartExecutorx-4.0/tests/laser/state/calldata_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/laser/state/mstack_test.py` & `smartExecutorx-4.0/tests/laser/state/mstack_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/laser/state/mstate_test.py` & `smartExecutorx-4.0/tests/laser/state/mstate_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/laser/state/storage_test.py` & `smartExecutorx-4.0/tests/laser/state/storage_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/laser/state/world_state_account_exist_load_test.py` & `smartExecutorx-4.0/tests/laser/state/world_state_account_exist_load_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/laser/test_transaction.py` & `smartExecutorx-4.0/tests/laser/test_transaction.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/laser/transaction/create_transaction_test.py` & `smartExecutorx-4.0/tests/laser/transaction/create_transaction_test.py`

 * *Files identical despite different names*

### Comparing `smartExecutorx-0.3/tests/laser/transaction/symbolic_test.py` & `smartExecutorx-4.0/tests/laser/transaction/symbolic_test.py`

 * *Files identical despite different names*

