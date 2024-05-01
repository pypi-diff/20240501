# Comparing `tmp/rlgym_tools-1.8.2.tar.gz` & `tmp/rlgym_tools-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rlgym_tools-1.8.2.tar", last modified: Tue Feb 14 08:47:22 2023, max compression
+gzip compressed data, was "dist/rlgym_tools-1.8.3.tar", last modified: Wed May  1 09:51:35 2024, max compression
```

## Comparing `rlgym_tools-1.8.2.tar` & `rlgym_tools-1.8.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:22.000000 rlgym_tools-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-02-14 08:47:22.000000 rlgym_tools-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:22.000000 rlgym_tools-1.8.2/rlgym_tools/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:22.000000 rlgym_tools-1.8.2/rlgym_tools/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/examples/rllib_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/examples/sb3_multi_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/examples/sb3_multiple_models_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:22.000000 rlgym_tools-1.8.2/rlgym_tools/extra_action_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_action_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_action_parsers/kbm_act.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_action_parsers/lookup_act.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:22.000000 rlgym_tools-1.8.2/rlgym_tools/extra_obs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_obs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_obs/advanced_padder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_obs/advanced_stacker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_obs/general_stacking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:22.000000 rlgym_tools-1.8.2/rlgym_tools/extra_rewards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_rewards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_rewards/anneal_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_rewards/diff_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_rewards/distribute_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_rewards/jump_touch_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_rewards/kickoff_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_rewards/multi_model_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_rewards/multiply_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_rewards/sequential_rewards.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:22.000000 rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/augment_setter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/goalie_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/hoops_setter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/replay_setter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/symmetric_setter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/wall_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/weighted_sample_setter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:22.000000 rlgym_tools-1.8.2/rlgym_tools/extra_terminals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_terminals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/extra_terminals/game_condition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:22.000000 rlgym_tools-1.8.2/rlgym_tools/pettingzoo_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/pettingzoo_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/pettingzoo_utils/pettingzoo_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/replay_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:22.000000 rlgym_tools-1.8.2/rlgym_tools/rllib_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/rllib_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/rllib_utils/rllib_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:22.000000 rlgym_tools-1.8.2/rlgym_tools/sb3_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/sb3_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/sb3_utils/sb3_distribute_rewards_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/sb3_utils/sb3_instantaneous_fps_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/sb3_utils/sb3_log_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)    13231 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/sb3_utils/sb3_multi_agent_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/sb3_utils/sb3_multiple_instance_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/sb3_utils/sb3_single_instance_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/rlgym_tools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 08:47:22.000000 rlgym_tools-1.8.2/rlgym_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-02-14 08:47:21.000000 rlgym_tools-1.8.2/rlgym_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-02-14 08:47:22.000000 rlgym_tools-1.8.2/rlgym_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 08:47:21.000000 rlgym_tools-1.8.2/rlgym_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-14 08:47:21.000000 rlgym_tools-1.8.2/rlgym_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-14 08:47:21.000000 rlgym_tools-1.8.2/rlgym_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 08:47:22.000000 rlgym_tools-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-02-14 08:47:14.000000 rlgym_tools-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/examples/rllib_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/examples/sb3_multi_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/examples/sb3_multiple_models_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools/extra_action_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_action_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_action_parsers/kbm_act.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_action_parsers/lookup_act.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools/extra_obs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_obs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_obs/advanced_padder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_obs/advanced_stacker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_obs/general_stacking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools/extra_rewards/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_rewards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_rewards/anneal_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_rewards/diff_reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_rewards/distribute_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_rewards/jump_touch_reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_rewards/kickoff_reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_rewards/multi_model_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_rewards/multiply_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_rewards/sequential_rewards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/augment_setter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/goalie_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/hoops_setter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/replay_setter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/symmetric_setter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/wall_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/weighted_sample_setter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools/extra_terminals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_terminals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/extra_terminals/game_condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools/pettingzoo_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/pettingzoo_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/pettingzoo_utils/pettingzoo_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/replay_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools/rllib_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/rllib_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/rllib_utils/rllib_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools/sb3_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/sb3_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/sb3_utils/sb3_distribute_rewards_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/sb3_utils/sb3_instantaneous_fps_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/sb3_utils/sb3_log_reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/sb3_utils/sb3_multi_agent_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/sb3_utils/sb3_multiple_instance_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/sb3_utils/sb3_single_instance_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/rlgym_tools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/rlgym_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 09:51:35.000000 rlgym_tools-1.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-01 09:51:30.000000 rlgym_tools-1.8.3/setup.py
```

### Comparing `rlgym_tools-1.8.2/PKG-INFO` & `rlgym_tools-1.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlgym_tools
-Version: 1.8.2
+Version: 1.8.3
 Summary: Extra tools for RLGym, like SB3 compatibility
 Home-page: https://rlgym.github.io
 Author: Rolv-Arild Braaten, Lucas Emery and Matthew Allen
 License: Apache 2.0
 Description: # rlgym-tools
         Extra tools for RLGym.
```

### Comparing `rlgym_tools-1.8.2/rlgym_tools/examples/rllib_example.py` & `rlgym_tools-1.8.3/rlgym_tools/examples/rllib_example.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/examples/sb3_multi_example.py` & `rlgym_tools-1.8.3/rlgym_tools/examples/sb3_multi_example.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/examples/sb3_multiple_models_example.py` & `rlgym_tools-1.8.3/rlgym_tools/examples/sb3_multiple_models_example.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_action_parsers/kbm_act.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_action_parsers/kbm_act.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_action_parsers/lookup_act.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_action_parsers/lookup_act.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,8 +46,10 @@
         actions = np.array(actions)
         return actions
 
     def get_action_space(self) -> gym.spaces.Space:
         return Discrete(len(self._lookup_table))
 
     def parse_actions(self, actions: Any, state: GameState) -> np.ndarray:
-        return self._lookup_table[actions]
+        indexes = np.array(actions, dtype=np.int32)
+        indexes = np.squeeze(indexes)
+        return self._lookup_table[indexes]
```

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_obs/advanced_padder.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_obs/advanced_padder.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_obs/advanced_stacker.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_obs/advanced_stacker.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_obs/general_stacking.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_obs/general_stacking.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_rewards/anneal_rewards.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_rewards/anneal_rewards.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_rewards/diff_reward.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_rewards/diff_reward.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_rewards/distribute_rewards.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_rewards/distribute_rewards.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_rewards/jump_touch_reward.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_rewards/jump_touch_reward.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_rewards/kickoff_reward.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_rewards/kickoff_reward.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_rewards/multi_model_rewards.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_rewards/multi_model_rewards.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_rewards/multiply_rewards.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_rewards/multiply_rewards.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_rewards/sequential_rewards.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_rewards/sequential_rewards.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/augment_setter.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/augment_setter.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/goalie_state.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/goalie_state.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/hoops_setter.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/hoops_setter.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/replay_setter.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/replay_setter.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/symmetric_setter.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/symmetric_setter.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/wall_state.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/wall_state.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_state_setters/weighted_sample_setter.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_state_setters/weighted_sample_setter.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/extra_terminals/game_condition.py` & `rlgym_tools-1.8.3/rlgym_tools/extra_terminals/game_condition.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/pettingzoo_utils/pettingzoo_env.py` & `rlgym_tools-1.8.3/rlgym_tools/pettingzoo_utils/pettingzoo_env.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/replay_converter.py` & `rlgym_tools-1.8.3/rlgym_tools/replay_converter.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/rllib_utils/rllib_env.py` & `rlgym_tools-1.8.3/rlgym_tools/rllib_utils/rllib_env.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/sb3_utils/sb3_distribute_rewards_wrapper.py` & `rlgym_tools-1.8.3/rlgym_tools/sb3_utils/sb3_distribute_rewards_wrapper.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/sb3_utils/sb3_instantaneous_fps_callback.py` & `rlgym_tools-1.8.3/rlgym_tools/sb3_utils/sb3_instantaneous_fps_callback.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/sb3_utils/sb3_log_reward.py` & `rlgym_tools-1.8.3/rlgym_tools/sb3_utils/sb3_log_reward.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/sb3_utils/sb3_multi_agent_tools.py` & `rlgym_tools-1.8.3/rlgym_tools/sb3_utils/sb3_multi_agent_tools.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/sb3_utils/sb3_multiple_instance_env.py` & `rlgym_tools-1.8.3/rlgym_tools/sb3_utils/sb3_multiple_instance_env.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/sb3_utils/sb3_single_instance_env.py` & `rlgym_tools-1.8.3/rlgym_tools/sb3_utils/sb3_single_instance_env.py`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/rlgym_tools/version.py` & `rlgym_tools-1.8.3/rlgym_tools/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # From https://github.com/RLBot/RLBot/blob/master/src/main/python/rlbot/version.py
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
 # https://stackoverflow.com/questions/458550/standard-way-to-embed-version-into-python-package
 
-__version__ = '1.8.2'
+__version__ = '1.8.3'
 
 release_notes = {
+    '1.8.3': """
+       - Update parse_actions in lookup_act.py (Jeff)
+    """,
     '1.8.2': """
        - Fix no touch timer in GameCondition (Rolv)
        - Update RLLib example (Aech)
     """,
     '1.8.1': """
         - Refactor GameCondition (Rolv, Impossibum)
         - Fix a small mistake in LookupAction (Rolv)
```

### Comparing `rlgym_tools-1.8.2/rlgym_tools.egg-info/PKG-INFO` & `rlgym_tools-1.8.3/rlgym_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlgym-tools
-Version: 1.8.2
+Version: 1.8.3
 Summary: Extra tools for RLGym, like SB3 compatibility
 Home-page: https://rlgym.github.io
 Author: Rolv-Arild Braaten, Lucas Emery and Matthew Allen
 License: Apache 2.0
 Description: # rlgym-tools
         Extra tools for RLGym.
```

### Comparing `rlgym_tools-1.8.2/rlgym_tools.egg-info/SOURCES.txt` & `rlgym_tools-1.8.3/rlgym_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rlgym_tools-1.8.2/setup.py` & `rlgym_tools-1.8.3/setup.py`

 * *Files identical despite different names*

