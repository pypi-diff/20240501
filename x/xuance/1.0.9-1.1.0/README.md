# Comparing `tmp/xuance-1.0.9.tar.gz` & `tmp/xuance-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xuance-1.0.9.tar", last modified: Fri Jan  5 13:22:05 2024, max compression
+gzip compressed data, was "xuance-1.1.0.tar", last modified: Wed May  1 15:42:23 2024, max compression
```

## Comparing `xuance-1.0.9.tar` & `xuance-1.1.0.tar`

### file list

```diff
@@ -1,809 +1,833 @@
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.763570 xuance-1.0.9/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2023-12-25 08:46:35.000000 xuance-1.0.9/LICENSE.txt
--rw-r--r--   0 wzliu     (1000) wzliu     (1000)     1732 2024-01-05 13:22:05.763570 xuance-1.0.9/PKG-INFO
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    18523 2024-01-02 09:13:39.000000 xuance-1.0.9/README.md
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       38 2024-01-05 13:22:05.763570 xuance-1.0.9/setup.cfg
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2715 2024-01-05 13:21:02.000000 xuance-1.0.9/setup.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      184 2024-01-05 13:21:02.000000 xuance-1.0.9/xuance/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/common/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      213 2023-12-18 07:52:17.000000 xuance-1.0.9/xuance/common/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12369 2023-12-23 15:23:59.000000 xuance-1.0.9/xuance/common/common_tools.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    25239 2023-12-21 05:26:17.000000 xuance-1.0.9/xuance/common/memory_tools.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    36360 2024-01-02 02:35:29.000000 xuance-1.0.9/xuance/common/memory_tools_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2879 2023-12-19 13:13:16.000000 xuance-1.0.9/xuance/common/segtree_tool.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4606 2023-12-19 11:27:23.000000 xuance-1.0.9/xuance/common/statistic_tools.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1426 2023-12-18 07:52:53.000000 xuance-1.0.9/xuance/configs/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/a2c/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1132 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/a2c/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/a2c/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      722 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/a2c/box2d/BipedalWalker-v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      725 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/a2c/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/a2c/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      746 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/a2c/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      749 2023-11-02 13:42:30.000000 xuance-1.0.9/xuance/configs/a2c/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      750 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/a2c/classic_control/MountainCar-v0.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      743 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/a2c/classic_control/Pendulum-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      737 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/a2c/mujoco.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      483 2023-12-20 03:35:42.000000 xuance-1.0.9/xuance/configs/basic.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/c51/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1110 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/c51/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/c51/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      811 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/c51/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      667 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/c51/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/c51/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      673 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/c51/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      674 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/c51/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      677 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/c51/classic_control/MountainCar-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.727571 xuance-1.0.9/xuance/configs/coma/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/coma/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1095 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/coma/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/coma/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1156 2023-11-04 11:59:31.000000 xuance-1.0.9/xuance/configs/coma/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1153 2023-11-04 12:02:30.000000 xuance-1.0.9/xuance/configs/coma/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1158 2023-11-04 11:59:31.000000 xuance-1.0.9/xuance/configs/coma/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1154 2023-11-04 11:59:31.000000 xuance-1.0.9/xuance/configs/coma/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1151 2023-11-04 12:04:32.000000 xuance-1.0.9/xuance/configs/coma/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1160 2023-11-04 11:59:31.000000 xuance-1.0.9/xuance/configs/coma/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1152 2023-11-04 11:59:31.000000 xuance-1.0.9/xuance/configs/coma/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1160 2023-11-04 11:59:31.000000 xuance-1.0.9/xuance/configs/coma/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1156 2023-11-04 12:02:30.000000 xuance-1.0.9/xuance/configs/coma/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1160 2023-11-04 12:02:30.000000 xuance-1.0.9/xuance/configs/coma/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.727571 xuance-1.0.9/xuance/configs/dcg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/dcg/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1549 2023-12-10 08:32:15.000000 xuance-1.0.9/xuance/configs/dcg/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/dcg/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1679 2023-12-10 08:33:10.000000 xuance-1.0.9/xuance/configs/dcg/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1676 2023-12-10 08:33:10.000000 xuance-1.0.9/xuance/configs/dcg/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1681 2023-12-10 08:33:10.000000 xuance-1.0.9/xuance/configs/dcg/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1677 2023-12-10 08:33:10.000000 xuance-1.0.9/xuance/configs/dcg/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1675 2023-12-10 08:33:10.000000 xuance-1.0.9/xuance/configs/dcg/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1684 2023-12-10 08:33:10.000000 xuance-1.0.9/xuance/configs/dcg/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1675 2023-12-10 08:33:10.000000 xuance-1.0.9/xuance/configs/dcg/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1684 2023-12-10 08:33:10.000000 xuance-1.0.9/xuance/configs/dcg/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1680 2023-12-10 08:33:10.000000 xuance-1.0.9/xuance/configs/dcg/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1684 2023-12-10 08:33:10.000000 xuance-1.0.9/xuance/configs/dcg/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/ddpg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/ddpg/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      657 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ddpg/box2d/BipedalWalker-v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/ddpg/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      662 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ddpg/classic_control/Pendulum-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      797 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ddpg/mujoco.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/ddqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ddqn/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/ddqn/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      784 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ddqn/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      637 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ddqn/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/ddqn/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      645 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ddqn/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      646 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ddqn/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      649 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ddqn/classic_control/MountainCar-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/dqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1078 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/dqn/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/dqn/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      781 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/dqn/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      634 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/dqn/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/dqn/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      648 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/dqn/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      649 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/dqn/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      632 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/dqn/classic_control/MountainCar-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/drqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1145 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/drqn/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/drqn/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      870 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/drqn/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      793 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/drqn/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/drqn/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      793 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/drqn/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      794 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/drqn/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      789 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/drqn/classic_control/MountainCar-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/dueldqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1097 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/dueldqn/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/dueldqn/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      793 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/dueldqn/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      648 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/dueldqn/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/dueldqn/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      654 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/dueldqn/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      655 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/dueldqn/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      659 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/dueldqn/classic_control/MountainCar-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.727571 xuance-1.0.9/xuance/configs/iddpg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/iddpg/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1043 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/iddpg/mpe/simple_adversary_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1038 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/iddpg/mpe/simple_push_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1036 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/iddpg/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.727571 xuance-1.0.9/xuance/configs/ippo/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/ippo/football/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2014 2023-11-17 07:24:08.000000 xuance-1.0.9/xuance/configs/ippo/football/3v1.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/ippo/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1449 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/ippo/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/ippo/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1532 2023-11-02 12:41:07.000000 xuance-1.0.9/xuance/configs/ippo/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1551 2023-11-02 12:41:07.000000 xuance-1.0.9/xuance/configs/ippo/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1590 2023-11-02 12:41:07.000000 xuance-1.0.9/xuance/configs/ippo/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1530 2023-11-02 12:41:07.000000 xuance-1.0.9/xuance/configs/ippo/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1528 2023-11-02 12:41:07.000000 xuance-1.0.9/xuance/configs/ippo/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1561 2023-11-02 12:41:07.000000 xuance-1.0.9/xuance/configs/ippo/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1550 2023-11-02 12:41:07.000000 xuance-1.0.9/xuance/configs/ippo/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1561 2023-11-02 12:41:07.000000 xuance-1.0.9/xuance/configs/ippo/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1553 2023-11-02 12:41:07.000000 xuance-1.0.9/xuance/configs/ippo/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1558 2023-11-02 12:41:07.000000 xuance-1.0.9/xuance/configs/ippo/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.727571 xuance-1.0.9/xuance/configs/iql/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/iql/football/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1549 2023-11-09 06:10:59.000000 xuance-1.0.9/xuance/configs/iql/football/3v1.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/iql/magent2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1066 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/iql/magent2/adversarial_pursuit_v4.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/iql/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      927 2023-12-14 03:46:31.000000 xuance-1.0.9/xuance/configs/iql/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/iql/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1079 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/iql/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1076 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/iql/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1101 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/iql/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1077 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/iql/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/iql/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1084 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/iql/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/iql/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1084 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/iql/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1080 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/iql/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1084 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/iql/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.727571 xuance-1.0.9/xuance/configs/isac/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/isac/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1049 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/isac/mpe/simple_adversary_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1044 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/isac/mpe/simple_push_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1046 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/isac/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.727571 xuance-1.0.9/xuance/configs/maddpg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/maddpg/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1006 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/maddpg/mpe/simple_adversary_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1028 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/maddpg/mpe/simple_push_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      992 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/maddpg/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/mappo/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/mappo/football/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2002 2023-11-22 10:19:27.000000 xuance-1.0.9/xuance/configs/mappo/football/1v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2017 2023-11-20 14:34:50.000000 xuance-1.0.9/xuance/configs/mappo/football/3v1.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/mappo/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1501 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/mappo/mpe/simple_adversary_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1496 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/mappo/mpe/simple_push_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1506 2023-12-13 04:10:01.000000 xuance-1.0.9/xuance/configs/mappo/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/mappo/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1524 2023-11-04 08:33:19.000000 xuance-1.0.9/xuance/configs/mappo/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1543 2023-11-04 08:33:19.000000 xuance-1.0.9/xuance/configs/mappo/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1592 2023-11-04 08:33:19.000000 xuance-1.0.9/xuance/configs/mappo/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1522 2023-11-04 08:33:19.000000 xuance-1.0.9/xuance/configs/mappo/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1520 2023-11-04 10:24:42.000000 xuance-1.0.9/xuance/configs/mappo/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1557 2023-11-13 12:18:52.000000 xuance-1.0.9/xuance/configs/mappo/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1542 2023-11-04 08:33:19.000000 xuance-1.0.9/xuance/configs/mappo/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1558 2023-11-14 02:11:28.000000 xuance-1.0.9/xuance/configs/mappo/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1545 2023-11-04 08:33:19.000000 xuance-1.0.9/xuance/configs/mappo/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1550 2023-11-04 08:33:19.000000 xuance-1.0.9/xuance/configs/mappo/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/masac/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/masac/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1053 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/masac/mpe/simple_adversary_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1048 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/masac/mpe/simple_push_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1051 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/masac/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/matd3/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/matd3/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      993 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/matd3/mpe/simple_adversary_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      988 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/matd3/mpe/simple_push_v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      990 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/matd3/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/mfac/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/mfac/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1641 2023-12-13 08:44:49.000000 xuance-1.0.9/xuance/configs/mfac/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/mfq/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/mfq/magent2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1133 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/mfq/magent2/adversarial_pursuit_v4.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/mfq/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      993 2023-12-14 03:46:31.000000 xuance-1.0.9/xuance/configs/mfq/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/mpdqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      699 2023-12-14 08:41:27.000000 xuance-1.0.9/xuance/configs/mpdqn/Platform.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/noisydqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1093 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/noisydqn/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/noisydqn/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      796 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/noisydqn/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      649 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/noisydqn/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/noisydqn/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      655 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/noisydqn/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      656 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/noisydqn/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      659 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/noisydqn/classic_control/MountainCar-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/pdqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      694 2023-12-14 08:40:00.000000 xuance-1.0.9/xuance/configs/pdqn/Platform.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/perdqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1118 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/perdqn/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/perdqn/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      821 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/perdqn/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      684 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/perdqn/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/perdqn/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      680 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/perdqn/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      681 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/perdqn/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      684 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/perdqn/classic_control/MountainCar-v1.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/pg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.735570 xuance-1.0.9/xuance/configs/pg/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      695 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/pg/box2d/BipedalWalker-v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      692 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/pg/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/pg/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      701 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/pg/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      702 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/pg/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      706 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/pg/classic_control/MountainCar-v0.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      704 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/pg/classic_control/Pendulum-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      703 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/pg/mujoco.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/ppg/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/ppg/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      695 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppg/box2d/BipedalWalker-v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      691 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppg/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/ppg/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      702 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppg/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      698 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppg/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      706 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppg/classic_control/MountainCar-v0.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      700 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppg/classic_control/Pendulum-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      707 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppg/mujoco.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/ppo/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1199 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppo/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/ppo/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      780 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppo/box2d/BipedalWalker-v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      983 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppo/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      781 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppo/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/ppo/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      788 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppo/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      789 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppo/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      792 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppo/classic_control/MountainCar-v0.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      786 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppo/classic_control/Pendulum-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1028 2023-12-28 07:51:31.000000 xuance-1.0.9/xuance/configs/ppo/drones.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      942 2023-12-26 04:13:30.000000 xuance-1.0.9/xuance/configs/ppo/minigrid.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      860 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/ppo/mujoco.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/qmix/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/qmix/football/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1667 2023-11-09 06:10:59.000000 xuance-1.0.9/xuance/configs/qmix/football/3v1.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/qmix/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1046 2023-12-14 12:55:47.000000 xuance-1.0.9/xuance/configs/qmix/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/qmix/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1216 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/qmix/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1215 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/qmix/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1218 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/qmix/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1214 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/qmix/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1212 2023-11-02 12:41:07.000000 xuance-1.0.9/xuance/configs/qmix/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1223 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/qmix/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1213 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/qmix/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1223 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/qmix/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1219 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/qmix/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1223 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/qmix/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/qrdqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1098 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/qrdqn/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/qrdqn/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      801 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/qrdqn/box2d/CarRacing-v2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      654 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/qrdqn/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/qrdqn/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      662 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/qrdqn/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      663 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/qrdqn/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      666 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/qrdqn/classic_control/MountainCar-v0.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/qtran/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/qtran/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1121 2023-12-14 12:56:04.000000 xuance-1.0.9/xuance/configs/qtran/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/random/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/random/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      121 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/random/mpe/simple_adversary.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      116 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/random/mpe/simple_push.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      118 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/random/mpe/simple_spread.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/sac/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1033 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/sac/atari.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/sac/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      664 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/sac/box2d/BipedalWalker-v3.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      696 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/sac/box2d/LunarLander-v2.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/sac/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      702 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/sac/classic_control/Acrobot-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      703 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/sac/classic_control/CartPole-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      706 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/sac/classic_control/MountainCar-v0.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      669 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/sac/classic_control/Pendulum-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      701 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/sac/mujoco.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/spdqn/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      630 2023-12-14 08:41:27.000000 xuance-1.0.9/xuance/configs/spdqn/Platform.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/td3/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/td3/box2d/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      662 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/td3/box2d/BipedalWalker-v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/td3/classic_control/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      667 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/td3/classic_control/Pendulum-v1.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      786 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/configs/td3/mujoco.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/vdac/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/vdac/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1676 2023-12-14 14:33:00.000000 xuance-1.0.9/xuance/configs/vdac/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/vdac/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1664 2023-11-04 16:18:22.000000 xuance-1.0.9/xuance/configs/vdac/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1721 2023-11-04 16:18:24.000000 xuance-1.0.9/xuance/configs/vdac/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1665 2023-11-04 16:18:24.000000 xuance-1.0.9/xuance/configs/vdac/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1662 2023-11-04 16:18:48.000000 xuance-1.0.9/xuance/configs/vdac/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1464 2023-11-04 16:18:24.000000 xuance-1.0.9/xuance/configs/vdac/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1730 2023-11-04 16:18:24.000000 xuance-1.0.9/xuance/configs/vdac/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1719 2023-11-04 16:18:24.000000 xuance-1.0.9/xuance/configs/vdac/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1730 2023-11-04 16:18:24.000000 xuance-1.0.9/xuance/configs/vdac/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1723 2023-11-04 16:18:24.000000 xuance-1.0.9/xuance/configs/vdac/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1728 2023-11-04 16:18:24.000000 xuance-1.0.9/xuance/configs/vdac/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/vdn/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/vdn/football/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1560 2023-11-07 11:40:38.000000 xuance-1.0.9/xuance/configs/vdn/football/3v1.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/vdn/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      940 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/vdn/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/vdn/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1095 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/vdn/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1092 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/vdn/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1097 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/vdn/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1093 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/vdn/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1091 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/vdn/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1100 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/vdn/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1091 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/vdn/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1100 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/vdn/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1095 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/vdn/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1100 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/vdn/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance/configs/wqmix/
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/wqmix/mpe/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1287 2023-11-04 15:49:09.000000 xuance-1.0.9/xuance/configs/wqmix/mpe/simple_spread_v3.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/configs/wqmix/sc2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1277 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/wqmix/sc2/1c3s5z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1276 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/wqmix/sc2/25m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1279 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/wqmix/sc2/2m_vs_1z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1275 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/wqmix/sc2/2s3z.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1273 2023-11-02 12:41:07.000000 xuance-1.0.9/xuance/configs/wqmix/sc2/3m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1284 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/wqmix/sc2/5m_vs_6m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1273 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/wqmix/sc2/8m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1284 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/wqmix/sc2/8m_vs_9m.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1278 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/wqmix/sc2/MMM2.yaml
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1284 2023-11-02 12:40:47.000000 xuance-1.0.9/xuance/configs/wqmix/sc2/corridor.yaml
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/environment/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5081 2023-12-28 06:20:18.000000 xuance-1.0.9/xuance/environment/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/environment/drones/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      134 2023-12-28 08:02:52.000000 xuance-1.0.9/xuance/environment/drones/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2289 2023-12-28 07:54:37.000000 xuance-1.0.9/xuance/environment/drones/drones_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2441 2023-12-28 06:44:10.000000 xuance-1.0.9/xuance/environment/drones/drones_vec_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/environment/football/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3014 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/football/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3508 2023-12-19 13:20:43.000000 xuance-1.0.9/xuance/environment/football/gfootball_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11368 2023-11-07 11:06:45.000000 xuance-1.0.9/xuance/environment/football/gfootball_vec_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4176 2023-12-15 02:19:06.000000 xuance-1.0.9/xuance/environment/football/raw_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/environment/gym/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/gym/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10151 2023-12-14 05:19:51.000000 xuance-1.0.9/xuance/environment/gym/gym_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10276 2023-12-28 06:43:02.000000 xuance-1.0.9/xuance/environment/gym/gym_vec_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/environment/gym_platform/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      239 2019-05-17 10:11:51.000000 xuance-1.0.9/xuance/environment/gym_platform/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.739570 xuance-1.0.9/xuance/environment/gym_platform/envs/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       74 2023-12-14 06:11:08.000000 xuance-1.0.9/xuance/environment/gym_platform/envs/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21868 2023-12-14 05:45:17.000000 xuance-1.0.9/xuance/environment/gym_platform/envs/platform_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/environment/magent2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      646 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/environment/magent2/builtin/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/builtin/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/environment/magent2/builtin/config/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/builtin/config/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1066 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/builtin/config/battle.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1372 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/builtin/config/double_attack.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1150 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/builtin/config/forest.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1015 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/builtin/config/pursuit.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1229 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/c_lib.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      702 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/environment.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/environment/magent2/environments/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      155 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/environments/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/environment/magent2/environments/adversarial_pursuit/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       60 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/environments/adversarial_pursuit/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7541 2023-10-20 05:41:16.000000 xuance-1.0.9/xuance/environment/magent2/environments/adversarial_pursuit/adversarial_pursuit.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       91 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/environments/adversarial_pursuit_v4.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/environment/magent2/environments/battle/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       47 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/environments/battle/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8888 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/environment/magent2/environments/battle/battle.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       61 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/environments/battle_v4.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/environment/magent2/environments/battlefield/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       52 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/environments/battlefield/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8882 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/environment/magent2/environments/battlefield/battlefield.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       66 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/environments/battlefield_v5.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/environment/magent2/environments/combined_arms/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       54 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/environments/combined_arms/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12397 2023-10-20 05:41:15.000000 xuance-1.0.9/xuance/environment/magent2/environments/combined_arms/combined_arms.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       68 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/environments/combined_arms_v6.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/environment/magent2/environments/gather/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       47 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/environments/gather/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9543 2023-10-20 05:41:16.000000 xuance-1.0.9/xuance/environment/magent2/environments/gather/gather.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       61 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/environments/gather_v5.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10576 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/environments/magent_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/environment/magent2/environments/tiger_deer/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       51 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/environments/tiger_deer/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7817 2023-10-20 05:41:18.000000 xuance-1.0.9/xuance/environment/magent2/environments/tiger_deer/tiger_deer.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       65 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/environments/tiger_deer_v4.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    31405 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/gridworld.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)   166808 2023-12-12 04:50:11.000000 xuance-1.0.9/xuance/environment/magent2/libmagent.dylib
--rwxrwxr-x   0 wzliu     (1000) wzliu     (1000)  2945728 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/libmagent.so
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)   126464 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/magent.dll
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2980 2023-12-27 09:21:43.000000 xuance-1.0.9/xuance/environment/magent2/magent_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7700 2023-12-27 09:50:01.000000 xuance-1.0.9/xuance/environment/magent2/magent_vec_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11270 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/render.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3233 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/magent2/utility.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/environment/minigrid/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-12-26 02:33:54.000000 xuance-1.0.9/xuance/environment/minigrid/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2712 2023-12-27 02:21:08.000000 xuance-1.0.9/xuance/environment/minigrid/minigrid_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1250 2023-12-26 03:09:11.000000 xuance-1.0.9/xuance/environment/minigrid/minigrid_vec_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/environment/new_env/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-12-11 05:44:33.000000 xuance-1.0.9/xuance/environment/new_env/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1525 2023-12-02 05:16:36.000000 xuance-1.0.9/xuance/environment/new_env/new_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1230 2023-12-02 04:54:59.000000 xuance-1.0.9/xuance/environment/new_env/new_vec_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/environment/pettingzoo/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1564 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/pettingzoo/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4238 2023-11-04 15:56:22.000000 xuance-1.0.9/xuance/environment/pettingzoo/pettingzoo_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    18321 2023-11-03 09:07:41.000000 xuance-1.0.9/xuance/environment/pettingzoo/pettingzoo_vec_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/environment/starcraft2/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/starcraft2/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2078 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/starcraft2/sc2_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12554 2023-11-07 10:59:22.000000 xuance-1.0.9/xuance/environment/starcraft2/sc2_vec_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/environment/vector_envs/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/vector_envs/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3981 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/vector_envs/env_utils.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6147 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/vector_envs/subproc_vec_env.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3019 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/environment/vector_envs/vector_env.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/mindspore/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/mindspore/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.743570 xuance-1.0.9/xuance/mindspore/agents/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4007 2023-12-12 07:20:21.000000 xuance-1.0.9/xuance/mindspore/agents/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5222 2023-12-09 11:40:00.000000 xuance-1.0.9/xuance/mindspore/agents/agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2640 2023-12-11 07:21:42.000000 xuance-1.0.9/xuance/mindspore/agents/agents_marl.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.747570 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7347 2023-12-10 06:30:07.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/coma_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5758 2023-12-27 08:59:15.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/dcg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2795 2023-12-12 04:30:33.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/iddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6168 2023-12-12 05:44:12.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/ippo_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4743 2023-12-27 09:00:15.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/iql_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2740 2023-12-13 04:20:55.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/isac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2798 2023-12-12 12:00:49.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/maddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6454 2023-12-13 03:46:25.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/mappo_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2788 2023-12-13 05:38:02.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/masac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3064 2023-12-13 05:46:54.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/matd3_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4672 2023-12-13 09:57:55.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/mfac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5074 2023-12-14 04:58:00.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/mfq_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4910 2023-12-27 09:00:48.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/qmix_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5237 2023-12-27 09:01:17.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/qtran_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5479 2023-12-14 15:09:07.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/vdac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4777 2023-12-27 09:01:49.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/vdn_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5068 2023-12-27 08:49:17.000000 xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/wqmix_agents.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.747570 xuance-1.0.9/xuance/mindspore/agents/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/mindspore/agents/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7501 2023-12-08 14:21:13.000000 xuance-1.0.9/xuance/mindspore/agents/policy_gradient/a2c_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6421 2023-12-11 08:45:21.000000 xuance-1.0.9/xuance/mindspore/agents/policy_gradient/ddpg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8389 2023-12-14 08:59:31.000000 xuance-1.0.9/xuance/mindspore/agents/policy_gradient/mpdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7622 2023-12-14 08:59:31.000000 xuance-1.0.9/xuance/mindspore/agents/policy_gradient/pdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6780 2023-12-14 10:58:45.000000 xuance-1.0.9/xuance/mindspore/agents/policy_gradient/pg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8511 2023-12-14 11:32:26.000000 xuance-1.0.9/xuance/mindspore/agents/policy_gradient/ppg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7425 2023-12-14 11:44:02.000000 xuance-1.0.9/xuance/mindspore/agents/policy_gradient/ppoclip_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6552 2023-12-25 08:01:55.000000 xuance-1.0.9/xuance/mindspore/agents/policy_gradient/ppokl_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5826 2023-12-14 14:01:49.000000 xuance-1.0.9/xuance/mindspore/agents/policy_gradient/sac_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6161 2023-12-14 13:53:57.000000 xuance-1.0.9/xuance/mindspore/agents/policy_gradient/sacdis_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8054 2023-12-14 08:59:32.000000 xuance-1.0.9/xuance/mindspore/agents/policy_gradient/spdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6255 2023-12-14 14:12:38.000000 xuance-1.0.9/xuance/mindspore/agents/policy_gradient/td3_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.747570 xuance-1.0.9/xuance/mindspore/agents/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6338 2023-12-10 02:45:30.000000 xuance-1.0.9/xuance/mindspore/agents/qlearning_family/C51_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/mindspore/agents/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6345 2023-12-11 14:37:19.000000 xuance-1.0.9/xuance/mindspore/agents/qlearning_family/ddqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6338 2023-12-12 07:19:44.000000 xuance-1.0.9/xuance/mindspore/agents/qlearning_family/dqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7563 2023-12-11 16:27:28.000000 xuance-1.0.9/xuance/mindspore/agents/qlearning_family/drqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6370 2023-12-12 02:47:52.000000 xuance-1.0.9/xuance/mindspore/agents/qlearning_family/dueldqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6376 2023-12-14 07:33:46.000000 xuance-1.0.9/xuance/mindspore/agents/qlearning_family/noisydqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6769 2023-12-14 10:39:02.000000 xuance-1.0.9/xuance/mindspore/agents/qlearning_family/perdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6354 2023-12-14 12:42:12.000000 xuance-1.0.9/xuance/mindspore/agents/qlearning_family/qrdqn_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.747570 xuance-1.0.9/xuance/mindspore/learners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2445 2023-12-14 07:33:46.000000 xuance-1.0.9/xuance/mindspore/learners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3773 2023-12-12 05:18:55.000000 xuance-1.0.9/xuance/mindspore/learners/learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.747570 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5469 2023-12-10 07:25:06.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/coma_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9850 2023-12-11 05:36:13.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/dcg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3696 2023-12-12 04:28:24.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/iddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6130 2023-12-13 03:59:31.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/ippo_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2847 2023-12-12 07:23:31.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/iql_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4341 2023-12-13 04:22:33.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/isac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4010 2023-12-12 12:04:11.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/maddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6260 2023-12-13 04:02:46.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/mappo_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4346 2023-12-13 05:38:16.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/masac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5292 2023-12-13 05:53:16.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/matd3_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3566 2023-12-13 09:58:44.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/mfac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3448 2023-12-14 04:59:30.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/mfq_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3294 2023-12-14 12:28:36.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/qmix_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6262 2023-12-14 13:33:25.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/qtran_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3483 2023-12-14 15:09:41.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/vdac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3184 2023-12-14 15:17:55.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/vdn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4808 2023-12-14 15:23:28.000000 xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/wqmix_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.747570 xuance-1.0.9/xuance/mindspore/learners/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/mindspore/learners/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2422 2023-12-09 11:20:09.000000 xuance-1.0.9/xuance/mindspore/learners/policy_gradient/a2c_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2707 2023-12-11 08:46:06.000000 xuance-1.0.9/xuance/mindspore/learners/policy_gradient/ddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4558 2023-12-14 06:37:27.000000 xuance-1.0.9/xuance/mindspore/learners/policy_gradient/mpdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3227 2023-12-14 08:11:30.000000 xuance-1.0.9/xuance/mindspore/learners/policy_gradient/pdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2101 2023-12-14 11:00:21.000000 xuance-1.0.9/xuance/mindspore/learners/policy_gradient/pg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4400 2023-12-14 11:29:33.000000 xuance-1.0.9/xuance/mindspore/learners/policy_gradient/ppg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2747 2023-12-14 11:47:36.000000 xuance-1.0.9/xuance/mindspore/learners/policy_gradient/ppoclip_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2798 2023-12-15 02:16:25.000000 xuance-1.0.9/xuance/mindspore/learners/policy_gradient/ppokl_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2738 2023-12-14 14:03:37.000000 xuance-1.0.9/xuance/mindspore/learners/policy_gradient/sac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3166 2023-12-14 13:57:10.000000 xuance-1.0.9/xuance/mindspore/learners/policy_gradient/sacdis_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4570 2023-12-14 08:16:36.000000 xuance-1.0.9/xuance/mindspore/learners/policy_gradient/spdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3100 2023-12-14 14:11:09.000000 xuance-1.0.9/xuance/mindspore/learners/policy_gradient/td3_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.747570 xuance-1.0.9/xuance/mindspore/learners/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/mindspore/learners/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3599 2023-12-10 02:53:02.000000 xuance-1.0.9/xuance/mindspore/learners/qlearning_family/c51_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2380 2023-12-11 14:44:06.000000 xuance-1.0.9/xuance/mindspore/learners/qlearning_family/ddqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2367 2023-12-11 14:52:23.000000 xuance-1.0.9/xuance/mindspore/learners/qlearning_family/dqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2750 2023-12-11 16:09:42.000000 xuance-1.0.9/xuance/mindspore/learners/qlearning_family/drqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2239 2023-12-12 02:46:31.000000 xuance-1.0.9/xuance/mindspore/learners/qlearning_family/dueldqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2440 2023-12-14 07:36:25.000000 xuance-1.0.9/xuance/mindspore/learners/qlearning_family/noisydqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2624 2023-12-14 10:42:40.000000 xuance-1.0.9/xuance/mindspore/learners/qlearning_family/perdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2988 2023-12-14 12:42:12.000000 xuance-1.0.9/xuance/mindspore/learners/qlearning_family/qrdqn_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.747570 xuance-1.0.9/xuance/mindspore/policies/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8887 2023-12-13 02:58:26.000000 xuance-1.0.9/xuance/mindspore/policies/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    14094 2023-12-14 13:56:24.000000 xuance-1.0.9/xuance/mindspore/policies/categorical.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16181 2023-12-27 08:44:15.000000 xuance-1.0.9/xuance/mindspore/policies/categorical_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4460 2023-12-23 08:58:45.000000 xuance-1.0.9/xuance/mindspore/policies/coordination_graph.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    40243 2023-12-22 09:37:01.000000 xuance-1.0.9/xuance/mindspore/policies/deterministic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    29574 2023-12-27 08:39:23.000000 xuance-1.0.9/xuance/mindspore/policies/deterministic_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10536 2023-12-23 04:26:37.000000 xuance-1.0.9/xuance/mindspore/policies/gaussian.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16781 2023-12-27 08:43:51.000000 xuance-1.0.9/xuance/mindspore/policies/gaussian_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6926 2023-12-23 08:58:45.000000 xuance-1.0.9/xuance/mindspore/policies/mixers.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.747570 xuance-1.0.9/xuance/mindspore/representations/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      939 2023-12-15 05:03:25.000000 xuance-1.0.9/xuance/mindspore/representations/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3706 2023-12-15 04:57:29.000000 xuance-1.0.9/xuance/mindspore/representations/cnn.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1570 2023-12-15 04:57:29.000000 xuance-1.0.9/xuance/mindspore/representations/mlp.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3600 2023-12-15 05:05:10.000000 xuance-1.0.9/xuance/mindspore/representations/rnn.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.747570 xuance-1.0.9/xuance/mindspore/runners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      198 2023-12-10 03:30:31.000000 xuance-1.0.9/xuance/mindspore/runners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      376 2023-12-08 14:07:56.000000 xuance-1.0.9/xuance/mindspore/runners/runner_basic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7274 2023-12-09 11:58:58.000000 xuance-1.0.9/xuance/mindspore/runners/runner_drl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21367 2023-12-14 15:06:56.000000 xuance-1.0.9/xuance/mindspore/runners/runner_pettingzoo.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.747570 xuance-1.0.9/xuance/mindspore/utils/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      555 2023-12-10 05:41:45.000000 xuance-1.0.9/xuance/mindspore/utils/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1726 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/mindspore/utils/distributions.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4934 2023-12-15 06:04:32.000000 xuance-1.0.9/xuance/mindspore/utils/input_reformat.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3930 2023-12-15 05:03:25.000000 xuance-1.0.9/xuance/mindspore/utils/layers.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2421 2023-12-08 14:09:42.000000 xuance-1.0.9/xuance/mindspore/utils/operations.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1536 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/mindspore/utils/set_trainer.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.747570 xuance-1.0.9/xuance/tensorflow/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/tensorflow/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.747570 xuance-1.0.9/xuance/tensorflow/agents/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4028 2023-12-18 09:17:36.000000 xuance-1.0.9/xuance/tensorflow/agents/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5312 2023-12-20 08:10:48.000000 xuance-1.0.9/xuance/tensorflow/agents/agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2688 2023-12-15 14:37:25.000000 xuance-1.0.9/xuance/tensorflow/agents/agents_marl.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.747570 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7409 2023-12-15 14:01:47.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/coma_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5903 2023-12-27 11:01:48.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/dcg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2988 2023-12-15 15:45:06.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/iddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4844 2023-12-18 09:48:22.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/ippo_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5143 2023-12-15 15:11:06.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/iql_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2828 2023-12-15 15:51:42.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/isac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2993 2023-12-15 15:54:30.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/maddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5487 2023-12-18 10:42:02.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/mappo_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2832 2023-12-15 15:58:24.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/masac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2988 2023-12-15 16:01:34.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/matd3_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4808 2023-12-18 08:40:15.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/mfac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4342 2023-12-18 06:18:31.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/mfq_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5133 2023-12-15 15:32:48.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/qmix_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5415 2023-12-15 16:17:48.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/qtran_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5602 2023-12-18 11:20:47.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/vdac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4991 2023-12-15 15:22:26.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/vdn_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5291 2023-12-15 16:12:55.000000 xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/wqmix_agents.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.751570 xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7245 2023-12-15 03:25:38.000000 xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/a2c_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6206 2023-12-15 08:36:20.000000 xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/ddpg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7961 2023-12-18 08:14:46.000000 xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/mpdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7930 2023-12-15 09:02:49.000000 xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/pdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6774 2023-12-15 05:39:32.000000 xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/pg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8842 2023-12-15 11:40:23.000000 xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/ppg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7495 2023-12-15 11:57:03.000000 xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/ppoclip_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7558 2023-12-15 05:41:10.000000 xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/ppokl_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5887 2023-12-15 05:41:37.000000 xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/sac_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6188 2023-12-15 12:16:32.000000 xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/sacdis_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7557 2023-12-15 09:13:28.000000 xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/spdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6261 2023-12-15 12:23:25.000000 xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/td3_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.751570 xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6215 2023-12-15 02:21:05.000000 xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/c51_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6367 2023-12-15 05:31:41.000000 xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/ddqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6360 2023-12-15 05:52:10.000000 xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/dqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7527 2023-12-15 06:59:53.000000 xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/drqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6392 2023-12-15 05:33:29.000000 xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/dueldqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6347 2023-12-15 05:34:28.000000 xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/noisydqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6791 2023-12-15 05:35:00.000000 xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/perdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6377 2023-12-15 05:35:38.000000 xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/qrdqn_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.751570 xuance-1.0.9/xuance/tensorflow/learners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2319 2023-12-18 09:16:20.000000 xuance-1.0.9/xuance/tensorflow/learners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3451 2023-12-18 11:10:06.000000 xuance-1.0.9/xuance/tensorflow/learners/learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.759570 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4782 2023-12-18 06:50:12.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/coma_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8735 2023-12-18 14:51:09.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/dcg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3740 2023-12-18 06:53:36.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/iddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5340 2023-12-18 10:15:58.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/ippo_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3317 2023-12-15 15:18:11.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/iql_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4039 2023-12-18 06:55:07.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/isac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3870 2023-12-18 06:57:53.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/maddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5534 2023-12-18 10:49:48.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/mappo_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4042 2023-12-18 06:59:18.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/masac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3949 2023-12-18 08:51:07.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/matd3_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3461 2023-12-18 09:07:01.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/mfac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3657 2023-12-18 07:00:35.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/mfq_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3768 2023-12-15 15:34:24.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/qmix_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6452 2023-12-15 16:20:03.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/qtran_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3612 2023-12-18 11:33:04.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/vdac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3498 2023-12-15 15:30:10.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/vdn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5335 2023-12-15 16:15:19.000000 xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/wqmix_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.759570 xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2067 2023-12-15 02:16:24.000000 xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/a2c_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2580 2023-12-18 08:04:47.000000 xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/ddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2911 2023-12-18 08:14:00.000000 xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/mpdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2865 2023-12-18 08:18:11.000000 xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/pdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1725 2023-12-15 11:08:41.000000 xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/pg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4673 2023-12-18 08:18:11.000000 xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/ppg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2411 2023-12-15 11:58:35.000000 xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/ppoclip_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2770 2023-12-15 02:16:24.000000 xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/ppokl_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2806 2023-12-18 08:18:11.000000 xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/sac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3169 2023-12-18 08:18:11.000000 xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/sacdis_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2867 2023-12-18 08:15:19.000000 xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/spdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3039 2023-12-18 08:18:11.000000 xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/td3_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.759570 xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2535 2023-12-15 05:11:09.000000 xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/c51_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2153 2023-12-15 05:50:16.000000 xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/ddqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2062 2023-12-15 07:32:39.000000 xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/dqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2516 2023-12-15 07:40:07.000000 xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/drqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2078 2023-12-15 08:02:34.000000 xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/dueldqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2153 2023-12-15 08:11:57.000000 xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/perdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2320 2023-12-15 08:16:49.000000 xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/qrdqn_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.759570 xuance-1.0.9/xuance/tensorflow/policies/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10285 2023-12-27 10:44:41.000000 xuance-1.0.9/xuance/tensorflow/policies/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11117 2023-12-15 13:41:09.000000 xuance-1.0.9/xuance/tensorflow/policies/categorical.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    17686 2023-12-27 10:46:13.000000 xuance-1.0.9/xuance/tensorflow/policies/categorical_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4383 2023-12-23 09:08:24.000000 xuance-1.0.9/xuance/tensorflow/policies/coordination_graph.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    42293 2023-12-22 09:37:01.000000 xuance-1.0.9/xuance/tensorflow/policies/deterministic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    32883 2023-12-27 13:06:20.000000 xuance-1.0.9/xuance/tensorflow/policies/deterministic_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11288 2023-12-15 11:31:24.000000 xuance-1.0.9/xuance/tensorflow/policies/gaussian.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16441 2023-12-27 10:46:13.000000 xuance-1.0.9/xuance/tensorflow/policies/gaussian_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8074 2023-12-23 08:58:45.000000 xuance-1.0.9/xuance/tensorflow/policies/mixers.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.759570 xuance-1.0.9/xuance/tensorflow/representations/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      906 2023-12-15 06:57:56.000000 xuance-1.0.9/xuance/tensorflow/representations/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1728 2023-12-15 06:57:56.000000 xuance-1.0.9/xuance/tensorflow/representations/cnn.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2022 2023-12-15 07:51:58.000000 xuance-1.0.9/xuance/tensorflow/representations/mlp.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       49 2023-12-15 06:57:56.000000 xuance-1.0.9/xuance/tensorflow/representations/rnn.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.759570 xuance-1.0.9/xuance/tensorflow/runners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      195 2023-12-15 02:02:01.000000 xuance-1.0.9/xuance/tensorflow/runners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1009 2023-12-15 08:54:19.000000 xuance-1.0.9/xuance/tensorflow/runners/runner_basic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6832 2023-12-15 06:06:26.000000 xuance-1.0.9/xuance/tensorflow/runners/runner_drl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21505 2023-12-18 06:37:57.000000 xuance-1.0.9/xuance/tensorflow/runners/runner_pettingzoo.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.759570 xuance-1.0.9/xuance/tensorflow/utils/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      618 2023-12-15 12:49:56.000000 xuance-1.0.9/xuance/tensorflow/utils/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2717 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/tensorflow/utils/distributions.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5119 2023-12-15 13:25:10.000000 xuance-1.0.9/xuance/tensorflow/utils/input_reformat.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4128 2023-12-15 06:51:54.000000 xuance-1.0.9/xuance/tensorflow/utils/layers.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3859 2023-12-15 11:37:34.000000 xuance-1.0.9/xuance/tensorflow/utils/operations.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.759570 xuance-1.0.9/xuance/torch/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/__init__.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.759570 xuance-1.0.9/xuance/torch/agents/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3856 2023-12-27 08:52:37.000000 xuance-1.0.9/xuance/torch/agents/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5916 2023-12-20 08:09:53.000000 xuance-1.0.9/xuance/torch/agents/agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3359 2023-12-20 02:58:26.000000 xuance-1.0.9/xuance/torch/agents/agents_marl.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.759570 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7853 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/coma_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6327 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/dcg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3347 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/iddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6410 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/ippo_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5188 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/iql_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3200 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/isac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3298 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/maddpg_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6713 2023-12-20 09:17:55.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/mappo_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3195 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/masac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3655 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/matd3_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5130 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/mfac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5462 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/mfq_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5378 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/qmix_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5770 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/qtran_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5858 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/vdac_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5234 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/vdn_agents.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5555 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/multi_agent_rl/wqmix_agents.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.759570 xuance-1.0.9/xuance/torch/agents/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/agents/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8077 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/policy_gradient/a2c_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6849 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/policy_gradient/ddpg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8203 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/policy_gradient/mpdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8391 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/policy_gradient/pdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7349 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/policy_gradient/pg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8945 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/policy_gradient/ppg_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8248 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/policy_gradient/ppoclip_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8191 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/policy_gradient/ppokl_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6480 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/policy_gradient/sac_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6813 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/policy_gradient/sacdis_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7767 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/policy_gradient/spdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6868 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/policy_gradient/td3_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.763570 xuance-1.0.9/xuance/torch/agents/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/agents/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6953 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/qlearning_family/c51_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7006 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/qlearning_family/ddqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6950 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/qlearning_family/dqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8187 2023-12-20 02:55:42.000000 xuance-1.0.9/xuance/torch/agents/qlearning_family/drqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7034 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/qlearning_family/dueldqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6988 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/qlearning_family/noisydqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7431 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/qlearning_family/perdqn_agent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7012 2023-12-20 02:55:43.000000 xuance-1.0.9/xuance/torch/agents/qlearning_family/qrdqn_agent.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.763570 xuance-1.0.9/xuance/torch/learners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2319 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/learners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4299 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/learners/learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.763570 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8825 2023-11-04 11:24:47.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/coma_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11559 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/dcg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3294 2023-10-20 05:41:16.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/iddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9879 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/ippo_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6037 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/iql_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3761 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/isac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3606 2023-10-20 05:41:18.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/maddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10538 2023-11-04 08:22:56.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/mappo_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3764 2023-10-20 05:41:16.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/masac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3811 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/matd3_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3290 2023-12-13 08:47:10.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/mfac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3145 2023-10-20 05:41:16.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/mfq_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6656 2023-10-20 05:41:16.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/qmix_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5382 2023-12-14 13:10:44.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/qtran_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6097 2023-12-14 14:54:20.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/vdac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6440 2023-10-20 05:41:18.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/vdn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10661 2023-10-20 05:41:18.000000 xuance-1.0.9/xuance/torch/learners/multi_agent_rl/wqmix_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.763570 xuance-1.0.9/xuance/torch/learners/policy_gradient/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/learners/policy_gradient/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1887 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/torch/learners/policy_gradient/a2c_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2056 2023-10-20 05:41:16.000000 xuance-1.0.9/xuance/torch/learners/policy_gradient/ddpg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2302 2023-12-14 06:23:29.000000 xuance-1.0.9/xuance/torch/learners/policy_gradient/mpdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2298 2023-12-14 06:01:04.000000 xuance-1.0.9/xuance/torch/learners/policy_gradient/pdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1558 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/torch/learners/policy_gradient/pg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3555 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/torch/learners/policy_gradient/ppg_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2681 2023-10-20 05:41:18.000000 xuance-1.0.9/xuance/torch/learners/policy_gradient/ppoclip_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2416 2023-10-20 05:41:18.000000 xuance-1.0.9/xuance/torch/learners/policy_gradient/ppokl_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2141 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/torch/learners/policy_gradient/sac_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2570 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/torch/learners/policy_gradient/sacdis_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2302 2023-12-14 07:59:27.000000 xuance-1.0.9/xuance/torch/learners/policy_gradient/spdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2432 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/torch/learners/policy_gradient/td3_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.763570 xuance-1.0.9/xuance/torch/learners/qlearning_family/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/learners/qlearning_family/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2256 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/torch/learners/qlearning_family/c51_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1881 2023-12-11 14:43:00.000000 xuance-1.0.9/xuance/torch/learners/qlearning_family/ddqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1810 2023-10-20 05:41:18.000000 xuance-1.0.9/xuance/torch/learners/qlearning_family/dqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2151 2023-10-20 05:41:15.000000 xuance-1.0.9/xuance/torch/learners/qlearning_family/drqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1818 2023-10-20 05:41:18.000000 xuance-1.0.9/xuance/torch/learners/qlearning_family/dueldqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1903 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/torch/learners/qlearning_family/perdqn_learner.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1907 2023-10-20 05:41:16.000000 xuance-1.0.9/xuance/torch/learners/qlearning_family/qrdqn_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.763570 xuance-1.0.9/xuance/torch/learners/ssl_rl/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/learners/ssl_rl/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/learners/ssl_rl/curl_learner.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.763570 xuance-1.0.9/xuance/torch/policies/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9922 2023-12-15 06:01:50.000000 xuance-1.0.9/xuance/torch/policies/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11438 2024-01-03 01:46:52.000000 xuance-1.0.9/xuance/torch/policies/categorical.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    15634 2023-12-22 03:23:27.000000 xuance-1.0.9/xuance/torch/policies/categorical_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3964 2023-12-18 12:16:47.000000 xuance-1.0.9/xuance/torch/policies/coordination_graph.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    38891 2023-12-22 09:37:01.000000 xuance-1.0.9/xuance/torch/policies/deterministic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    29206 2023-12-22 06:42:24.000000 xuance-1.0.9/xuance/torch/policies/deterministic_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11823 2023-12-23 04:25:09.000000 xuance-1.0.9/xuance/torch/policies/gaussian.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    13417 2023-12-22 12:05:49.000000 xuance-1.0.9/xuance/torch/policies/gaussian_marl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6646 2023-11-04 15:22:56.000000 xuance-1.0.9/xuance/torch/policies/mixers.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.763570 xuance-1.0.9/xuance/torch/representations/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1268 2023-12-15 05:00:06.000000 xuance-1.0.9/xuance/torch/representations/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4150 2023-10-20 05:41:16.000000 xuance-1.0.9/xuance/torch/representations/cnn.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2066 2023-10-20 05:41:17.000000 xuance-1.0.9/xuance/torch/representations/mlp.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3944 2023-10-20 05:41:16.000000 xuance-1.0.9/xuance/torch/representations/rnn.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.763570 xuance-1.0.9/xuance/torch/runners/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      429 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/runners/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      372 2023-11-08 08:20:22.000000 xuance-1.0.9/xuance/torch/runners/runner_basic.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7259 2023-12-14 05:40:06.000000 xuance-1.0.9/xuance/torch/runners/runner_drl.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9455 2023-11-09 12:03:08.000000 xuance-1.0.9/xuance/torch/runners/runner_football.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      193 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/runners/runner_magent.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21502 2023-12-14 14:55:34.000000 xuance-1.0.9/xuance/torch/runners/runner_pettingzoo.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21315 2024-01-02 02:35:29.000000 xuance-1.0.9/xuance/torch/runners/runner_sc2.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.763570 xuance-1.0.9/xuance/torch/utils/
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      548 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/utils/__init__.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2806 2023-10-27 12:18:06.000000 xuance-1.0.9/xuance/torch/utils/distributions.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5587 2023-10-20 05:41:16.000000 xuance-1.0.9/xuance/torch/utils/input_reformat.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4412 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/utils/layers.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3826 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/utils/operations.py
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3098 2023-10-20 05:39:12.000000 xuance-1.0.9/xuance/torch/utils/value_norm.py
-drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-01-05 13:22:05.731571 xuance-1.0.9/xuance.egg-info/
--rw-r--r--   0 wzliu     (1000) wzliu     (1000)     1732 2024-01-05 13:22:05.000000 xuance-1.0.9/xuance.egg-info/PKG-INFO
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    29843 2024-01-05 13:22:05.000000 xuance-1.0.9/xuance.egg-info/SOURCES.txt
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        1 2024-01-05 13:22:05.000000 xuance-1.0.9/xuance.egg-info/dependency_links.txt
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      397 2024-01-05 13:22:05.000000 xuance-1.0.9/xuance.egg-info/requires.txt
--rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        7 2024-01-05 13:22:05.000000 xuance-1.0.9/xuance.egg-info/top_level.txt
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.196396 xuance-1.1.0/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2023-12-25 08:46:35.000000 xuance-1.1.0/LICENSE.txt
+-rw-r--r--   0 wzliu     (1000) wzliu     (1000)     2693 2024-05-01 15:42:23.196396 xuance-1.1.0/PKG-INFO
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    19574 2024-04-14 03:11:12.000000 xuance-1.1.0/README.md
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       38 2024-05-01 15:42:23.196396 xuance-1.1.0/setup.cfg
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3603 2024-05-01 15:40:41.000000 xuance-1.1.0/setup.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      185 2024-04-11 09:02:57.000000 xuance-1.1.0/xuance/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/common/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      213 2023-12-18 07:52:17.000000 xuance-1.1.0/xuance/common/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    13861 2024-05-01 08:19:43.000000 xuance-1.1.0/xuance/common/common_tools.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    25239 2023-12-21 05:26:17.000000 xuance-1.1.0/xuance/common/memory_tools.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    36896 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/common/memory_tools_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2879 2023-12-19 13:13:16.000000 xuance-1.1.0/xuance/common/segtree_tool.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4606 2023-12-19 11:27:23.000000 xuance-1.1.0/xuance/common/statistic_tools.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1426 2023-12-18 07:52:53.000000 xuance-1.1.0/xuance/configs/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/a2c/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1133 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/a2c/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/a2c/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      749 2024-05-01 14:59:33.000000 xuance-1.1.0/xuance/configs/a2c/box2d/BipedalWalker-v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      726 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/a2c/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/a2c/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      747 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/a2c/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      750 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/a2c/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      751 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/a2c/classic_control/MountainCar-v0.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      770 2024-05-01 15:18:11.000000 xuance-1.1.0/xuance/configs/a2c/classic_control/Pendulum-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      764 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/a2c/mujoco.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      491 2024-01-18 07:00:38.000000 xuance-1.1.0/xuance/configs/basic.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/c51/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1110 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/c51/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/c51/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      811 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/c51/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      667 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/c51/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/c51/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      673 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/c51/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      674 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/c51/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      677 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/c51/classic_control/MountainCar-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/coma/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/coma/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1095 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/coma/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/coma/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1156 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/coma/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1153 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/coma/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1158 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/coma/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1154 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/coma/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1151 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/coma/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1160 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/coma/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1152 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/coma/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1160 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/coma/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1156 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/coma/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1160 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/coma/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/dcg/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/dcg/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1549 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/dcg/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/dcg/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1679 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/dcg/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1676 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dcg/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1681 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/dcg/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1677 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/dcg/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1675 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/dcg/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1684 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/dcg/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1675 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dcg/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1684 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/dcg/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1680 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/dcg/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1684 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dcg/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ddpg/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ddpg/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      683 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ddpg/box2d/BipedalWalker-v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ddpg/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      715 2024-05-01 15:18:41.000000 xuance-1.1.0/xuance/configs/ddpg/classic_control/Pendulum-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      832 2024-05-01 15:23:45.000000 xuance-1.1.0/xuance/configs/ddpg/drones.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      824 2024-05-01 15:23:45.000000 xuance-1.1.0/xuance/configs/ddpg/mujoco.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ddqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ddqn/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ddqn/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      784 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ddqn/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      637 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ddqn/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ddqn/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      645 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ddqn/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      646 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ddqn/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      649 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ddqn/classic_control/MountainCar-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/dqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1078 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dqn/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/dqn/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      781 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dqn/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      634 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dqn/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/dqn/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      648 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/dqn/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      649 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dqn/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      633 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/dqn/classic_control/MountainCar-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/drqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1145 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/drqn/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/drqn/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      870 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/drqn/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      793 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/drqn/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/drqn/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      793 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/drqn/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      794 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/drqn/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      789 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/drqn/classic_control/MountainCar-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/dueldqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1097 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dueldqn/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/dueldqn/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      793 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dueldqn/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      648 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/dueldqn/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/dueldqn/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      654 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/dueldqn/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      655 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/dueldqn/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      659 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/dueldqn/classic_control/MountainCar-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/iddpg/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1038 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/iddpg/drones.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/iddpg/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1044 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/iddpg/mpe/simple_adversary_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1039 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/iddpg/mpe/simple_push_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1037 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/iddpg/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/ippo/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ippo/football/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2014 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ippo/football/3v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ippo/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1474 2024-05-01 14:03:25.000000 xuance-1.1.0/xuance/configs/ippo/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/ippo/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1532 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ippo/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1551 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ippo/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1590 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ippo/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1530 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ippo/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1528 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ippo/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1561 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/ippo/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1550 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ippo/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1561 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ippo/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1553 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/ippo/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1558 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ippo/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/iql/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/iql/football/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1549 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/football/3v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/iql/magent2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1066 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/magent2/adversarial_pursuit_v4.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/iql/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      927 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/iql/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/iql/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1079 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1076 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/iql/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1101 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1077 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/iql/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1084 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1075 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1084 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1080 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/iql/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1084 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/iql/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/isac/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/isac/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1046 2024-05-01 14:18:17.000000 xuance-1.1.0/xuance/configs/isac/mpe/simple_adversary_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1041 2024-05-01 14:18:17.000000 xuance-1.1.0/xuance/configs/isac/mpe/simple_push_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1043 2024-05-01 14:18:17.000000 xuance-1.1.0/xuance/configs/isac/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.144395 xuance-1.1.0/xuance/configs/maddpg/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1035 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/maddpg/drones.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/maddpg/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1007 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/maddpg/mpe/simple_adversary_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1029 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/maddpg/mpe/simple_push_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      993 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/maddpg/mpe/simple_spread_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      976 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/maddpg/new_env_mas.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/mappo/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/mappo/football/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2002 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/mappo/football/1v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2017 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/mappo/football/3v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/mappo/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1530 2024-05-01 14:08:36.000000 xuance-1.1.0/xuance/configs/mappo/mpe/simple_adversary_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1525 2024-05-01 14:08:36.000000 xuance-1.1.0/xuance/configs/mappo/mpe/simple_push_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1535 2024-05-01 14:08:36.000000 xuance-1.1.0/xuance/configs/mappo/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/mappo/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1524 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/mappo/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1543 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/mappo/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1592 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/mappo/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1522 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/mappo/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1520 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/mappo/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1557 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/mappo/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1542 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/mappo/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1558 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/mappo/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1545 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/mappo/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1550 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/mappo/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/masac/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/masac/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1050 2024-05-01 14:18:17.000000 xuance-1.1.0/xuance/configs/masac/mpe/simple_adversary_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1045 2024-05-01 14:18:17.000000 xuance-1.1.0/xuance/configs/masac/mpe/simple_push_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1048 2024-05-01 14:18:17.000000 xuance-1.1.0/xuance/configs/masac/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/matd3/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/matd3/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      990 2024-05-01 14:14:07.000000 xuance-1.1.0/xuance/configs/matd3/mpe/simple_adversary_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      985 2024-05-01 14:14:07.000000 xuance-1.1.0/xuance/configs/matd3/mpe/simple_push_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      987 2024-05-01 14:14:06.000000 xuance-1.1.0/xuance/configs/matd3/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/mfac/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/mfac/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1642 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/mfac/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/mfq/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/mfq/magent2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1133 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/mfq/magent2/adversarial_pursuit_v4.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/mfq/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      993 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/mfq/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/mpdqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      725 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/mpdqn/Platform.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/noisydqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1093 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/noisydqn/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/noisydqn/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      796 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/noisydqn/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      649 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/noisydqn/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/noisydqn/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      655 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/noisydqn/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      656 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/noisydqn/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      659 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/noisydqn/classic_control/MountainCar-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/pdqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      720 2024-05-01 15:23:45.000000 xuance-1.1.0/xuance/configs/pdqn/Platform.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/perdqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1118 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/perdqn/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/perdqn/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      821 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/perdqn/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      684 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/perdqn/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/perdqn/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      680 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/perdqn/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      681 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/perdqn/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      684 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/perdqn/classic_control/MountainCar-v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/pg/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/pg/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      721 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/pg/box2d/BipedalWalker-v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      692 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/pg/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/pg/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      701 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/pg/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      702 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/pg/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      706 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/pg/classic_control/MountainCar-v0.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      731 2024-05-01 15:23:45.000000 xuance-1.1.0/xuance/configs/pg/classic_control/Pendulum-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      730 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/pg/mujoco.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/ppg/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/ppg/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      722 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppg/box2d/BipedalWalker-v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      691 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/ppg/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/ppg/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      703 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/ppg/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      698 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/ppg/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      707 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/ppg/classic_control/MountainCar-v0.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      727 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppg/classic_control/Pendulum-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      734 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppg/mujoco.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/ppo/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1285 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ppo/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/ppo/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      807 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppo/box2d/BipedalWalker-v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      983 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/ppo/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      782 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/ppo/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/ppo/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      789 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/ppo/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      790 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/ppo/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      793 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/ppo/classic_control/MountainCar-v0.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      813 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppo/classic_control/Pendulum-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1074 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppo/drones.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1102 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppo/metadrive.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      937 2024-05-01 13:26:43.000000 xuance-1.1.0/xuance/configs/ppo/minigrid.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      887 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/ppo/mujoco.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/qmix/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/qmix/football/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1667 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/qmix/football/3v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/qmix/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1046 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qmix/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/qmix/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1216 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/qmix/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1215 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qmix/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1218 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qmix/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1214 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qmix/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1212 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qmix/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1223 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/qmix/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1213 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/qmix/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1223 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/qmix/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1219 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qmix/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1223 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/qmix/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/qrdqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1098 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qrdqn/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/qrdqn/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      801 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qrdqn/box2d/CarRacing-v2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      654 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qrdqn/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/qrdqn/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      662 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/qrdqn/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      663 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/qrdqn/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      666 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/qrdqn/classic_control/MountainCar-v0.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/qtran/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/qtran/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1121 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/qtran/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.136395 xuance-1.1.0/xuance/configs/random/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/random/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      121 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/configs/random/mpe/simple_adversary.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      116 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/configs/random/mpe/simple_push.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      118 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/configs/random/mpe/simple_spread.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/sac/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1034 2024-05-01 13:26:44.000000 xuance-1.1.0/xuance/configs/sac/atari.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/sac/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      690 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/sac/box2d/BipedalWalker-v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      696 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/sac/box2d/LunarLander-v2.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/sac/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      702 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/sac/classic_control/Acrobot-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      695 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/sac/classic_control/CartPole-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      706 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/sac/classic_control/MountainCar-v0.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      695 2024-05-01 15:23:45.000000 xuance-1.1.0/xuance/configs/sac/classic_control/Pendulum-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      935 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/sac/metadrive.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      728 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/sac/mujoco.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/spdqn/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      656 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/spdqn/Platform.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/td3/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/td3/box2d/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      689 2024-05-01 15:23:45.000000 xuance-1.1.0/xuance/configs/td3/box2d/BipedalWalker-v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/td3/classic_control/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      727 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/td3/classic_control/Pendulum-v1.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      813 2024-05-01 15:23:44.000000 xuance-1.1.0/xuance/configs/td3/mujoco.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/vdac/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.152395 xuance-1.1.0/xuance/configs/vdac/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1676 2024-05-01 14:19:34.000000 xuance-1.1.0/xuance/configs/vdac/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/configs/vdac/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1664 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdac/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1721 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/vdac/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1665 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdac/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1662 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/vdac/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1464 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/vdac/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1730 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/vdac/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1719 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdac/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1730 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdac/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1723 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdac/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1728 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdac/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/configs/vdn/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/configs/vdn/football/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1560 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdn/football/3v1.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/configs/vdn/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      940 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdn/mpe/simple_spread_v3.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      977 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdn/new_env_mas.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/configs/vdn/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1095 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdn/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1092 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdn/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1097 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdn/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1093 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdn/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1091 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/vdn/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1100 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdn/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1091 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdn/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1100 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/vdn/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1095 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/vdn/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1100 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/vdn/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance/configs/wqmix/
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/configs/wqmix/mpe/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1287 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/wqmix/mpe/simple_spread_v3.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/configs/wqmix/sc2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1277 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/1c3s5z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1276 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/25m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1279 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/2m_vs_1z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1275 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/2s3z.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1273 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/3m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1284 2024-05-01 13:26:17.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/5m_vs_6m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1273 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/8m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1284 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/8m_vs_9m.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1278 2024-05-01 13:26:16.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/MMM2.yaml
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1284 2024-05-01 13:26:15.000000 xuance-1.1.0/xuance/configs/wqmix/sc2/corridor.yaml
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/environment/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6407 2024-04-24 07:21:56.000000 xuance-1.1.0/xuance/environment/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/environment/drones/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      336 2024-04-23 04:44:07.000000 xuance-1.1.0/xuance/environment/drones/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/environment/drones/customized/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3983 2024-02-23 12:32:58.000000 xuance-1.1.0/xuance/environment/drones/customized/HoverAviary.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6687 2024-04-16 12:40:23.000000 xuance-1.1.0/xuance/environment/drones/customized/MultiHoverAviary.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2024-02-23 12:27:09.000000 xuance-1.1.0/xuance/environment/drones/customized/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4266 2024-04-23 05:11:00.000000 xuance-1.1.0/xuance/environment/drones/drones_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4437 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/environment/drones/drones_vec_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9817 2024-03-01 08:07:09.000000 xuance-1.1.0/xuance/environment/drones/drones_vec_env_mas.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/environment/football/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2357 2024-04-23 04:42:48.000000 xuance-1.1.0/xuance/environment/football/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3526 2024-04-22 07:53:14.000000 xuance-1.1.0/xuance/environment/football/gfootball_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11382 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/environment/football/gfootball_vec_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4850 2024-04-22 07:54:05.000000 xuance-1.1.0/xuance/environment/football/raw_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/environment/gym/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      233 2024-04-22 07:42:41.000000 xuance-1.1.0/xuance/environment/gym/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10151 2023-12-14 05:19:51.000000 xuance-1.1.0/xuance/environment/gym/gym_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10348 2024-03-01 07:44:31.000000 xuance-1.1.0/xuance/environment/gym/gym_vec_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/environment/gym_platform/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      239 2019-05-17 10:11:51.000000 xuance-1.1.0/xuance/environment/gym_platform/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.156396 xuance-1.1.0/xuance/environment/gym_platform/envs/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       74 2023-12-14 06:11:08.000000 xuance-1.1.0/xuance/environment/gym_platform/envs/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21868 2023-12-14 05:45:17.000000 xuance-1.1.0/xuance/environment/gym_platform/envs/platform_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      742 2024-04-23 04:44:07.000000 xuance-1.1.0/xuance/environment/magent2/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/builtin/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/builtin/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/builtin/config/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/builtin/config/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1066 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/builtin/config/battle.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1372 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/builtin/config/double_attack.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1150 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/builtin/config/forest.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1015 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/builtin/config/pursuit.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1229 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/c_lib.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      702 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environment.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/environments/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      155 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/environments/adversarial_pursuit/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       60 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/adversarial_pursuit/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7541 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/environment/magent2/environments/adversarial_pursuit/adversarial_pursuit.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       91 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/adversarial_pursuit_v4.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/environments/battle/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       47 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/battle/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8888 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/environment/magent2/environments/battle/battle.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       61 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/battle_v4.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/environments/battlefield/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       52 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/battlefield/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8882 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/environment/magent2/environments/battlefield/battlefield.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       66 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/battlefield_v5.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/environments/combined_arms/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       54 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/combined_arms/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12397 2023-10-20 05:41:15.000000 xuance-1.1.0/xuance/environment/magent2/environments/combined_arms/combined_arms.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       68 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/combined_arms_v6.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/environments/gather/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       47 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/gather/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9543 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/environment/magent2/environments/gather/gather.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       61 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/gather_v5.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10576 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/magent_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.160395 xuance-1.1.0/xuance/environment/magent2/environments/tiger_deer/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       51 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/tiger_deer/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7817 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/environment/magent2/environments/tiger_deer/tiger_deer.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       65 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/environments/tiger_deer_v4.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    31405 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/gridworld.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)   166808 2023-12-12 04:50:11.000000 xuance-1.1.0/xuance/environment/magent2/libmagent.dylib
+-rwxrwxr-x   0 wzliu     (1000) wzliu     (1000)  2945728 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/libmagent.so
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)   126464 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/magent.dll
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3247 2024-02-20 07:58:49.000000 xuance-1.1.0/xuance/environment/magent2/magent_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      984 2024-01-08 03:46:25.000000 xuance-1.1.0/xuance/environment/magent2/magent_vec_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11270 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/render.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3233 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/environment/magent2/utility.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/metadrive/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       83 2024-04-23 04:44:07.000000 xuance-1.1.0/xuance/environment/metadrive/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1401 2024-04-23 05:11:00.000000 xuance-1.1.0/xuance/environment/metadrive/metadrive_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      826 2024-04-18 04:02:14.000000 xuance-1.1.0/xuance/environment/metadrive/metadrive_vec_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/minigrid/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      109 2024-04-23 04:44:07.000000 xuance-1.1.0/xuance/environment/minigrid/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2712 2023-12-27 02:21:08.000000 xuance-1.1.0/xuance/environment/minigrid/minigrid_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1242 2024-03-01 03:02:51.000000 xuance-1.1.0/xuance/environment/minigrid/minigrid_vec_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/new_env/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       86 2024-04-23 04:44:50.000000 xuance-1.1.0/xuance/environment/new_env/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2142 2024-05-01 08:48:40.000000 xuance-1.1.0/xuance/environment/new_env/new_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1230 2023-12-02 04:54:59.000000 xuance-1.1.0/xuance/environment/new_env/new_vec_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/new_env_mas/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      102 2024-04-23 04:44:50.000000 xuance-1.1.0/xuance/environment/new_env_mas/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3273 2024-03-28 11:11:38.000000 xuance-1.1.0/xuance/environment/new_env_mas/new_env_mas.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9939 2024-03-23 08:28:32.000000 xuance-1.1.0/xuance/environment/new_env_mas/new_vec_env_mas.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/pettingzoo/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      186 2024-04-23 04:44:50.000000 xuance-1.1.0/xuance/environment/pettingzoo/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5672 2024-04-22 07:52:00.000000 xuance-1.1.0/xuance/environment/pettingzoo/pettingzoo_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    18308 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/environment/pettingzoo/pettingzoo_vec_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/robotic_warehouse/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2024-02-21 11:20:19.000000 xuance-1.1.0/xuance/environment/robotic_warehouse/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2387 2024-02-21 12:24:01.000000 xuance-1.1.0/xuance/environment/robotic_warehouse/robotic_warehouse_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/starcraft2/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      103 2024-04-23 04:42:01.000000 xuance-1.1.0/xuance/environment/starcraft2/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2079 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/environment/starcraft2/sc2_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12562 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/environment/starcraft2/sc2_vec_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/environment/vector_envs/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      448 2024-04-22 07:42:41.000000 xuance-1.1.0/xuance/environment/vector_envs/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3990 2024-04-22 07:42:41.000000 xuance-1.1.0/xuance/environment/vector_envs/env_utils.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4649 2024-04-22 07:42:41.000000 xuance-1.1.0/xuance/environment/vector_envs/subproc_vec_env.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2198 2024-04-22 07:42:41.000000 xuance-1.1.0/xuance/environment/vector_envs/vector_env.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/mindspore/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.164395 xuance-1.1.0/xuance/mindspore/agents/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4007 2023-12-12 07:20:21.000000 xuance-1.1.0/xuance/mindspore/agents/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5252 2024-01-18 07:03:28.000000 xuance-1.1.0/xuance/mindspore/agents/agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2640 2023-12-11 07:21:42.000000 xuance-1.1.0/xuance/mindspore/agents/agents_marl.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.168396 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7347 2023-12-10 06:30:07.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/coma_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5758 2023-12-27 08:59:15.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/dcg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2776 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/iddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6168 2023-12-12 05:44:12.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/ippo_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4743 2023-12-27 09:00:15.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/iql_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2721 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/isac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2779 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/maddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6454 2023-12-13 03:46:25.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/mappo_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2769 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/masac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3045 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/matd3_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4653 2024-02-22 12:18:39.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/mfac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5055 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/mfq_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4910 2023-12-27 09:00:48.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/qmix_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5237 2023-12-27 09:01:17.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/qtran_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5479 2023-12-14 15:09:07.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/vdac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4777 2023-12-27 09:01:49.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/vdn_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5068 2023-12-27 08:49:17.000000 xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/wqmix_agents.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.168396 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7507 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/a2c_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6427 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ddpg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8389 2023-12-14 08:59:31.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/mpdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7622 2023-12-14 08:59:31.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/pdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6786 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/pg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8517 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ppg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7431 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ppoclip_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6552 2023-12-25 08:01:55.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ppokl_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5832 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/sac_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6167 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/sacdis_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8054 2023-12-14 08:59:32.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/spdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6261 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/policy_gradient/td3_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.168396 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6344 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/C51_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6351 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/ddqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6344 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/dqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7569 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/drqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6376 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/dueldqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6382 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/noisydqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6775 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/perdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6360 2024-01-18 07:02:49.000000 xuance-1.1.0/xuance/mindspore/agents/qlearning_family/qrdqn_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.168396 xuance-1.1.0/xuance/mindspore/learners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2445 2023-12-14 07:33:46.000000 xuance-1.1.0/xuance/mindspore/learners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3773 2023-12-12 05:18:55.000000 xuance-1.1.0/xuance/mindspore/learners/learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.172396 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5469 2023-12-10 07:25:06.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/coma_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9850 2023-12-11 05:36:13.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/dcg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3696 2023-12-12 04:28:24.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/iddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6130 2023-12-13 03:59:31.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/ippo_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2847 2023-12-12 07:23:31.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/iql_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4341 2023-12-13 04:22:33.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/isac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4010 2023-12-12 12:04:11.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/maddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6260 2023-12-13 04:02:46.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/mappo_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4346 2023-12-13 05:38:16.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/masac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5292 2023-12-13 05:53:16.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/matd3_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3566 2023-12-13 09:58:44.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/mfac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3448 2023-12-14 04:59:30.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/mfq_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3294 2023-12-14 12:28:36.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/qmix_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6262 2023-12-14 13:33:25.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/qtran_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3483 2023-12-14 15:09:41.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/vdac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3184 2023-12-14 15:17:55.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/vdn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4808 2023-12-14 15:23:28.000000 xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/wqmix_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.172396 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2422 2023-12-09 11:20:09.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/a2c_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2707 2023-12-11 08:46:06.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4558 2023-12-14 06:37:27.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/mpdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3227 2023-12-14 08:11:30.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/pdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2101 2023-12-14 11:00:21.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/pg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4400 2023-12-14 11:29:33.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ppg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2747 2023-12-14 11:47:36.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ppoclip_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2798 2023-12-15 02:16:25.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ppokl_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2738 2023-12-14 14:03:37.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/sac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3166 2023-12-14 13:57:10.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/sacdis_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4570 2023-12-14 08:16:36.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/spdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3100 2023-12-14 14:11:09.000000 xuance-1.1.0/xuance/mindspore/learners/policy_gradient/td3_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.172396 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3599 2023-12-10 02:53:02.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/c51_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2380 2023-12-11 14:44:06.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/ddqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2367 2023-12-11 14:52:23.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/dqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2750 2023-12-11 16:09:42.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/drqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2239 2023-12-12 02:46:31.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/dueldqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2440 2023-12-14 07:36:25.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/noisydqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2624 2023-12-14 10:42:40.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/perdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2988 2023-12-14 12:42:12.000000 xuance-1.1.0/xuance/mindspore/learners/qlearning_family/qrdqn_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.176396 xuance-1.1.0/xuance/mindspore/policies/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8887 2023-12-13 02:58:26.000000 xuance-1.1.0/xuance/mindspore/policies/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    14094 2023-12-14 13:56:24.000000 xuance-1.1.0/xuance/mindspore/policies/categorical.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16181 2023-12-27 08:44:15.000000 xuance-1.1.0/xuance/mindspore/policies/categorical_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4460 2023-12-23 08:58:45.000000 xuance-1.1.0/xuance/mindspore/policies/coordination_graph.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    40243 2023-12-22 09:37:01.000000 xuance-1.1.0/xuance/mindspore/policies/deterministic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    29574 2023-12-27 08:39:23.000000 xuance-1.1.0/xuance/mindspore/policies/deterministic_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10536 2023-12-23 04:26:37.000000 xuance-1.1.0/xuance/mindspore/policies/gaussian.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16781 2023-12-27 08:43:51.000000 xuance-1.1.0/xuance/mindspore/policies/gaussian_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6926 2023-12-23 08:58:45.000000 xuance-1.1.0/xuance/mindspore/policies/mixers.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.176396 xuance-1.1.0/xuance/mindspore/representations/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      939 2023-12-15 05:03:25.000000 xuance-1.1.0/xuance/mindspore/representations/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3706 2023-12-15 04:57:29.000000 xuance-1.1.0/xuance/mindspore/representations/cnn.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1570 2023-12-15 04:57:29.000000 xuance-1.1.0/xuance/mindspore/representations/mlp.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3600 2023-12-15 05:05:10.000000 xuance-1.1.0/xuance/mindspore/representations/rnn.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.176396 xuance-1.1.0/xuance/mindspore/runners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      198 2023-12-10 03:30:31.000000 xuance-1.1.0/xuance/mindspore/runners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      376 2023-12-08 14:07:56.000000 xuance-1.1.0/xuance/mindspore/runners/runner_basic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7274 2023-12-09 11:58:58.000000 xuance-1.1.0/xuance/mindspore/runners/runner_drl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21371 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/mindspore/runners/runner_pettingzoo.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.176396 xuance-1.1.0/xuance/mindspore/utils/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      555 2023-12-10 05:41:45.000000 xuance-1.1.0/xuance/mindspore/utils/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1726 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/utils/distributions.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4934 2023-12-15 06:04:32.000000 xuance-1.1.0/xuance/mindspore/utils/input_reformat.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3930 2023-12-15 05:03:25.000000 xuance-1.1.0/xuance/mindspore/utils/layers.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2421 2023-12-08 14:09:42.000000 xuance-1.1.0/xuance/mindspore/utils/operations.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1536 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/mindspore/utils/set_trainer.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.176396 xuance-1.1.0/xuance/tensorflow/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.176396 xuance-1.1.0/xuance/tensorflow/agents/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4028 2023-12-18 09:17:36.000000 xuance-1.1.0/xuance/tensorflow/agents/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5342 2024-01-18 07:03:28.000000 xuance-1.1.0/xuance/tensorflow/agents/agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2688 2023-12-15 14:37:25.000000 xuance-1.1.0/xuance/tensorflow/agents/agents_marl.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.176396 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7409 2023-12-15 14:01:47.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/coma_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5903 2023-12-27 11:01:48.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/dcg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2969 2024-02-22 12:18:39.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/iddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4844 2023-12-18 09:48:22.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/ippo_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5143 2023-12-15 15:11:06.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/iql_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2809 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/isac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2974 2024-02-22 12:18:39.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/maddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5487 2023-12-18 10:42:02.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/mappo_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2813 2024-02-22 12:18:39.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/masac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2969 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/matd3_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4789 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/mfac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4323 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/mfq_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5133 2023-12-15 15:32:48.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/qmix_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5415 2023-12-15 16:17:48.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/qtran_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5602 2023-12-18 11:20:47.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/vdac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4991 2023-12-15 15:22:26.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/vdn_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5291 2023-12-15 16:12:55.000000 xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/wqmix_agents.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.180396 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7251 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/a2c_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6212 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ddpg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7961 2023-12-18 08:14:46.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/mpdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7930 2023-12-15 09:02:49.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/pdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6780 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/pg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8848 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ppg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7501 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ppoclip_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7564 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ppokl_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5893 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/sac_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6194 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/sacdis_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7557 2023-12-15 09:13:28.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/spdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6267 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/td3_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.180396 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6221 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/c51_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6373 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/ddqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6366 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/dqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7533 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/drqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6398 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/dueldqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6353 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/noisydqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6797 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/perdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6383 2024-01-18 07:02:30.000000 xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/qrdqn_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.180396 xuance-1.1.0/xuance/tensorflow/learners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2319 2023-12-18 09:16:20.000000 xuance-1.1.0/xuance/tensorflow/learners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3451 2023-12-18 11:10:06.000000 xuance-1.1.0/xuance/tensorflow/learners/learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.180396 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4782 2023-12-18 06:50:12.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/coma_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8735 2023-12-18 14:51:09.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/dcg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3740 2023-12-18 06:53:36.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/iddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5340 2023-12-18 10:15:58.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/ippo_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3317 2023-12-15 15:18:11.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/iql_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4039 2023-12-18 06:55:07.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/isac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3870 2023-12-18 06:57:53.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/maddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5534 2023-12-18 10:49:48.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/mappo_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4042 2023-12-18 06:59:18.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/masac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3949 2023-12-18 08:51:07.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/matd3_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3461 2023-12-18 09:07:01.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/mfac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3657 2023-12-18 07:00:35.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/mfq_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3768 2023-12-15 15:34:24.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/qmix_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6452 2023-12-15 16:20:03.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/qtran_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3612 2023-12-18 11:33:04.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/vdac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3498 2023-12-15 15:30:10.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/vdn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5335 2023-12-15 16:15:19.000000 xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/wqmix_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.180396 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2067 2023-12-15 02:16:24.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/a2c_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2580 2023-12-18 08:04:47.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2911 2023-12-18 08:14:00.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/mpdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2865 2023-12-18 08:18:11.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/pdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1725 2023-12-15 11:08:41.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/pg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4673 2023-12-18 08:18:11.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ppg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2411 2023-12-15 11:58:35.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ppoclip_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2770 2023-12-15 02:16:24.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ppokl_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2806 2023-12-18 08:18:11.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/sac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3169 2023-12-18 08:18:11.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/sacdis_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2867 2023-12-18 08:15:19.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/spdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3039 2023-12-18 08:18:11.000000 xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/td3_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.180396 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2535 2023-12-15 05:11:09.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/c51_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2153 2023-12-15 05:50:16.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/ddqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2062 2023-12-15 07:32:39.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/dqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2516 2023-12-15 07:40:07.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/drqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2078 2023-12-15 08:02:34.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/dueldqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2153 2023-12-15 08:11:57.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/perdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2320 2023-12-15 08:16:49.000000 xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/qrdqn_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.180396 xuance-1.1.0/xuance/tensorflow/policies/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10285 2023-12-27 10:44:41.000000 xuance-1.1.0/xuance/tensorflow/policies/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11117 2023-12-15 13:41:09.000000 xuance-1.1.0/xuance/tensorflow/policies/categorical.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    17686 2023-12-27 10:46:13.000000 xuance-1.1.0/xuance/tensorflow/policies/categorical_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4383 2023-12-23 09:08:24.000000 xuance-1.1.0/xuance/tensorflow/policies/coordination_graph.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    42293 2023-12-22 09:37:01.000000 xuance-1.1.0/xuance/tensorflow/policies/deterministic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    32883 2023-12-27 13:06:20.000000 xuance-1.1.0/xuance/tensorflow/policies/deterministic_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11288 2023-12-15 11:31:24.000000 xuance-1.1.0/xuance/tensorflow/policies/gaussian.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16441 2023-12-27 10:46:13.000000 xuance-1.1.0/xuance/tensorflow/policies/gaussian_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8074 2023-12-23 08:58:45.000000 xuance-1.1.0/xuance/tensorflow/policies/mixers.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.184396 xuance-1.1.0/xuance/tensorflow/representations/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      906 2023-12-15 06:57:56.000000 xuance-1.1.0/xuance/tensorflow/representations/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1728 2023-12-15 06:57:56.000000 xuance-1.1.0/xuance/tensorflow/representations/cnn.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2022 2023-12-15 07:51:58.000000 xuance-1.1.0/xuance/tensorflow/representations/mlp.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)       49 2023-12-15 06:57:56.000000 xuance-1.1.0/xuance/tensorflow/representations/rnn.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.184396 xuance-1.1.0/xuance/tensorflow/runners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      195 2023-12-15 02:02:01.000000 xuance-1.1.0/xuance/tensorflow/runners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1009 2023-12-15 08:54:19.000000 xuance-1.1.0/xuance/tensorflow/runners/runner_basic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6832 2023-12-15 06:06:26.000000 xuance-1.1.0/xuance/tensorflow/runners/runner_drl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21509 2024-02-22 12:36:38.000000 xuance-1.1.0/xuance/tensorflow/runners/runner_pettingzoo.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.184396 xuance-1.1.0/xuance/tensorflow/utils/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      618 2023-12-15 12:49:56.000000 xuance-1.1.0/xuance/tensorflow/utils/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2717 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/tensorflow/utils/distributions.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5119 2023-12-15 13:25:10.000000 xuance-1.1.0/xuance/tensorflow/utils/input_reformat.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4128 2023-12-15 06:51:54.000000 xuance-1.1.0/xuance/tensorflow/utils/layers.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3859 2023-12-15 11:37:34.000000 xuance-1.1.0/xuance/tensorflow/utils/operations.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.184396 xuance-1.1.0/xuance/torch/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/torch/__init__.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.184396 xuance-1.1.0/xuance/torch/agents/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2678 2024-05-01 10:42:19.000000 xuance-1.1.0/xuance/torch/agents/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5897 2024-05-01 10:20:05.000000 xuance-1.1.0/xuance/torch/agents/agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3425 2024-05-01 09:48:01.000000 xuance-1.1.0/xuance/torch/agents/agents_marl.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.184396 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      638 2024-04-22 13:08:14.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7853 2023-12-20 02:55:43.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/coma_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6327 2023-12-20 02:55:43.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/dcg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3328 2024-02-22 12:18:39.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/iddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6649 2024-01-30 07:07:08.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/ippo_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5188 2023-12-20 02:55:42.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/iql_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3181 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/isac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3279 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/maddpg_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7007 2024-03-30 09:29:07.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/mappo_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3176 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/masac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3317 2024-05-01 14:32:15.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/matd3_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5111 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/mfac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5443 2024-02-22 12:18:38.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/mfq_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5378 2024-05-01 10:42:14.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/qmix_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5770 2023-12-20 02:55:43.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/qtran_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5858 2023-12-20 02:55:43.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/vdac_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5234 2023-12-20 02:55:42.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/vdn_agents.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5555 2023-12-20 02:55:42.000000 xuance-1.1.0/xuance/torch/agents/multi_agent_rl/wqmix_agents.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.184396 xuance-1.1.0/xuance/torch/agents/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      424 2024-04-22 13:07:06.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8083 2024-01-18 07:00:38.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/a2c_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6855 2024-01-30 08:04:24.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/ddpg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8203 2023-12-20 02:55:42.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/mpdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8391 2023-12-20 02:55:42.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/pdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7355 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/pg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8951 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/ppg_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8254 2024-04-17 04:33:18.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/ppoclip_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8045 2024-04-14 06:51:57.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/ppokl_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6487 2024-04-25 12:16:23.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/sac_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6819 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/sacdis_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7767 2023-12-20 02:55:42.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/spdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6874 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/policy_gradient/td3_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.188396 xuance-1.1.0/xuance/torch/agents/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      296 2024-04-22 13:07:15.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6959 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/c51_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7012 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/ddqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6956 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/dqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8193 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/drqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7040 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/dueldqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6994 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/noisydqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7437 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/perdqn_agent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7018 2024-01-18 07:01:27.000000 xuance-1.1.0/xuance/torch/agents/qlearning_family/qrdqn_agent.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.188396 xuance-1.1.0/xuance/torch/learners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1064 2024-04-22 13:00:21.000000 xuance-1.1.0/xuance/torch/learners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5119 2024-05-01 10:21:47.000000 xuance-1.1.0/xuance/torch/learners/learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.192396 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      640 2024-04-22 13:02:22.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     8825 2023-11-04 11:24:47.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/coma_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11559 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/dcg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3294 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/iddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9879 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/ippo_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6037 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/iql_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3761 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/isac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3606 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/maddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10946 2024-01-29 04:09:10.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/mappo_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3764 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/masac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3415 2024-05-01 14:31:15.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/matd3_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3290 2023-12-13 08:47:10.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/mfac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3145 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/mfq_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6656 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/qmix_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5382 2023-12-14 13:10:44.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/qtran_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6097 2023-12-14 14:54:20.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/vdac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6440 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/vdn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10661 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/torch/learners/multi_agent_rl/wqmix_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.192396 xuance-1.1.0/xuance/torch/learners/policy_gradient/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      472 2024-04-22 13:01:54.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1887 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/a2c_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2056 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/ddpg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2302 2023-12-14 06:23:29.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/mpdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2298 2023-12-14 06:01:04.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/pdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1558 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/pg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3555 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/ppg_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2681 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/ppoclip_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2416 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/ppokl_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2141 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/sac_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2570 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/sacdis_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2302 2023-12-14 07:59:27.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/spdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2432 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/policy_gradient/td3_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.192396 xuance-1.1.0/xuance/torch/learners/qlearning_family/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      281 2024-04-22 13:02:07.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2256 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/c51_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1881 2023-12-11 14:43:00.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/ddqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1810 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/dqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2151 2023-10-20 05:41:15.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/drqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1818 2023-10-20 05:41:18.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/dueldqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1903 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/perdqn_learner.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1907 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/learners/qlearning_family/qrdqn_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.192396 xuance-1.1.0/xuance/torch/learners/ssl_rl/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/torch/learners/ssl_rl/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        0 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/torch/learners/ssl_rl/curl_learner.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.192396 xuance-1.1.0/xuance/torch/policies/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    10442 2024-05-01 15:26:37.000000 xuance-1.1.0/xuance/torch/policies/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    11695 2024-04-22 13:06:16.000000 xuance-1.1.0/xuance/torch/policies/categorical.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    15749 2024-01-31 09:53:33.000000 xuance-1.1.0/xuance/torch/policies/categorical_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3964 2023-12-18 12:16:47.000000 xuance-1.1.0/xuance/torch/policies/coordination_graph.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    42041 2024-05-01 14:57:14.000000 xuance-1.1.0/xuance/torch/policies/deterministic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    29895 2024-05-01 14:57:14.000000 xuance-1.1.0/xuance/torch/policies/deterministic_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    12014 2024-05-01 15:29:30.000000 xuance-1.1.0/xuance/torch/policies/gaussian.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    13728 2024-05-01 14:00:37.000000 xuance-1.1.0/xuance/torch/policies/gaussian_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     6646 2023-11-04 15:22:56.000000 xuance-1.1.0/xuance/torch/policies/mixers.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.192396 xuance-1.1.0/xuance/torch/representations/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     1268 2023-12-15 05:00:06.000000 xuance-1.1.0/xuance/torch/representations/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4150 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/representations/cnn.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2066 2023-10-20 05:41:17.000000 xuance-1.1.0/xuance/torch/representations/mlp.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3944 2023-10-20 05:41:16.000000 xuance-1.1.0/xuance/torch/representations/rnn.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.196396 xuance-1.1.0/xuance/torch/runners/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      491 2024-02-22 11:27:05.000000 xuance-1.1.0/xuance/torch/runners/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      372 2023-11-08 08:20:22.000000 xuance-1.1.0/xuance/torch/runners/runner_basic.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     7016 2024-05-01 15:10:48.000000 xuance-1.1.0/xuance/torch/runners/runner_drl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     9455 2023-11-09 12:03:08.000000 xuance-1.1.0/xuance/torch/runners/runner_football.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      171 2024-01-18 07:00:38.000000 xuance-1.1.0/xuance/torch/runners/runner_magent.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    16013 2024-05-01 10:20:05.000000 xuance-1.1.0/xuance/torch/runners/runner_marl.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21469 2024-05-01 14:34:22.000000 xuance-1.1.0/xuance/torch/runners/runner_pettingzoo.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    21193 2024-05-01 10:46:01.000000 xuance-1.1.0/xuance/torch/runners/runner_sc2.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.196396 xuance-1.1.0/xuance/torch/utils/
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      935 2024-05-01 13:27:29.000000 xuance-1.1.0/xuance/torch/utils/__init__.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     2806 2023-10-27 12:18:06.000000 xuance-1.1.0/xuance/torch/utils/distributions.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     5748 2024-05-01 14:57:14.000000 xuance-1.1.0/xuance/torch/utils/input_reformat.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     4412 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/torch/utils/layers.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3826 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/torch/utils/operations.py
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)     3098 2023-10-20 05:39:12.000000 xuance-1.1.0/xuance/torch/utils/value_norm.py
+drwxrwxr-x   0 wzliu     (1000) wzliu     (1000)        0 2024-05-01 15:42:23.140395 xuance-1.1.0/xuance.egg-info/
+-rw-r--r--   0 wzliu     (1000) wzliu     (1000)     2693 2024-05-01 15:42:23.000000 xuance-1.1.0/xuance.egg-info/PKG-INFO
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)    30714 2024-05-01 15:42:23.000000 xuance-1.1.0/xuance.egg-info/SOURCES.txt
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        1 2024-05-01 15:42:23.000000 xuance-1.1.0/xuance.egg-info/dependency_links.txt
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)      451 2024-05-01 15:42:23.000000 xuance-1.1.0/xuance.egg-info/requires.txt
+-rw-rw-r--   0 wzliu     (1000) wzliu     (1000)        7 2024-05-01 15:42:23.000000 xuance-1.1.0/xuance.egg-info/top_level.txt
```

### Comparing `xuance-1.0.9/LICENSE.txt` & `xuance-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/README.md` & `xuance-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 </div>
 
 # XuanCe: A Comprehensive and Unified Deep Reinforcement Learning Library
 
 [![PyPI](https://img.shields.io/pypi/v/xuance)](https://pypi.org/project/xuance/)
 [![Documentation Status](https://readthedocs.org/projects/xuance/badge/?version=latest)](https://xuance.readthedocs.io)
 [![GitHub](https://img.shields.io/github/license/agi-brain/xuance)](https://github.com/agi-brain/xuance/blob/master/LICENSE.txt)
-[![Pepy Total Downlods](https://img.shields.io/pepy/dt/xuance)](https://www.pepy.tech/projects/xuance)
+[![Downloads](https://static.pepy.tech/badge/xuance)](https://pepy.tech/project/xuance)
 [![GitHub Repo stars](https://img.shields.io/github/stars/agi-brain/xuance?style=social)](https://github.com/agi-brain/xuance/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/agi-brain/xuance?style=social)](https://github.com/agi-brain/xuance/forks)
 [![GitHub watchers](https://img.shields.io/github/watchers/agi-brain/xuance?style=social)](https://github.com/agi-brain/xuance/watchers)
 
 [![PyTorch](https://img.shields.io/badge/PyTorch-%3E%3D1.13.0-red)](https://pytorch.org/get-started/locally/)
 [![TensorFlow](https://img.shields.io/badge/TensorFlow-%3E%3D2.6.0-orange)](https://www.tensorflow.org/install)
 [![MindSpore](https://img.shields.io/badge/MindSpore-%3E%3D1.10.1-blue)](https://www.mindspore.cn/install/en)
@@ -249,14 +249,38 @@
 <td> <center>
 <br/> <font color="AAAAAA">...</font>
 </center> </td>
 </tr>
 </table>
 </details>
 
+### [Drones Environments](https://github.com/utiasDSL/gym-pybullet-drones)
+
+[XuanCe's documentation for the installation and usage of gym-pybullet-drones](https://xuance.readthedocs.io/en/latest/documents/api/environments/drones.html).
+
+<details open>
+<summary>(Click to hide)</summary>
+
+<table rules="none" align="center"><tr>
+<td> <center>
+<img src="./docs/source/figures/drones/helix.gif" height=100" /><br/><font color="AAAAAA">Helix</font>
+</center></td>
+<td> <center>
+<img src="./docs/source/figures/drones/rl.gif" height=100" /> <br/> <font color="AAAAAA">Single-Agent Hover</font>
+</center> </td>
+<td> <center>
+<img src="./docs/source/figures/drones/marl.gif" height=100" /> <br/> <font color="AAAAAA">Multi-Agent Hover</font>
+</center> </td>
+<td> <center>
+<br/> <font color="AAAAAA">...</font>
+</center> </td>
+</tr>
+</table>
+</details>
+
 ### [MPE Environments](https://pettingzoo.farama.org/environments/mpe/)
 
 <details open>
 <summary>(Click to hide)</summary>
 
 <table rules="none" align="center"><tr>
 <td> <center>
@@ -406,24 +430,30 @@
 
 ## Community
 
 ### [Github Issue](https://github.com/agi-brain/xuance/issues)
 
 You can put your questions, advices, or the bugs you have found in the [Issues](https://github.com/agi-brain/xuance/issues). 
 
-### [Communication Group](https://github.com/agi-brain/xuance/blob/master/docs/source/figures/QQ_group.jpeg) on QQ App.
+### Social Accounts.
 
-Welcome to join the official communication group with QQ app. (Group number: 552432695)
+Welcome to join the official communication group with QQ app (Group number: 552432695), and the official account ("玄策 RLlib") on WeChat.
 
 <details open>
-<summary>(QR code for QQ group )</summary>
+<summary>(QR code for QQ group and official account)</summary>
 
-<div align="center">
-<img src="docs/source/figures/QQ_group.jpeg" width="200" height="auto" align=center />
-</div>
+<table rules="none" align="center"><tr>
+<td> <center>
+<img src="docs/source/figures/QQ_group.jpeg" width="200" height="auto" /><br/><font color="AAAAAA">QQ group</font>
+</center></td>
+<td> <center>
+<img src="docs/source/figures/Official_Account.jpg" width="200" height="auto" /> <br/> <font color="AAAAAA">Official account</font>
+</center> </td>
+</tr>
+</table>
 
 </details>
 
 [@TFBestPractices](https://twitter.com/TFBestPractices/status/1665770204398223361)
 
 ### Citations
```

### Comparing `xuance-1.0.9/xuance/common/common_tools.py` & `xuance-1.1.0/xuance/common/common_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import yaml
+import time
 import numpy as np
 import scipy.signal
 from copy import deepcopy
 from gym.spaces import Space, Dict
 from types import SimpleNamespace as SN
 from xuance.configs import method_list
 
@@ -20,15 +21,15 @@
         A dict mapping keys of basic_dict to the values of the same keys in target_dict.
         For example:
 
         basic_dict = {'a': 1, 'b': 2}
         target_dict = {'a': 3, 'c': 4}
         out_dict = recursive_dict_update(basic_dict, target_dict)
 
-        output_dict = {'a': 3, 'b': 2}
+        output_dict = {'a': 3, 'b': 2, 'c': 4}
     """
     out_dict = deepcopy(basic_dict)
     for key, value in target_dict.items():
         if isinstance(value, dict):
             out_dict[key] = recursive_dict_update(out_dict.get(key, {}), value)
         else:
             out_dict[key] = value
@@ -47,15 +48,15 @@
         try:
             config_dict = yaml.load(f, Loader=yaml.FullLoader)
         except yaml.YAMLError as exc:
             assert False, file_dir + " error: {}".format(exc)
     return config_dict
 
 
-def get_arguments(method, env, env_id, config_path=None, parser_args=None):
+def get_arguments(method, env, env_id, config_path=None, parser_args=None, is_test=False):
     """Get arguments from .yaml files
     Args:
         method: the algorithm name that will be implemented,
         env: The name of the environment,
         env_id: The name of the scenario in the environment.
         config_path: default is None, if None, the default configs (xuance/configs/.../*.yaml) will be loaded.
         parser_args: arguments that specified by parser tools.
@@ -68,23 +69,42 @@
     config_path_default = os.path.join(main_path_package, "configs")
 
     ''' get the arguments from xuance/config/basic.yaml '''
     config_basic = get_config(os.path.join(config_path_default, "basic.yaml"))
 
     ''' get the arguments from, e.g., xuance/config/dqn/box2d/CarRacing-v2.yaml '''
     if type(method) == list:  # for different groups of MARL algorithms.
-        file_name = env + "/" + env_id + ".yaml"
-        config_algo_default = [get_config(os.path.join(config_path_default, agent, file_name)) for agent in method]
+        if config_path is None:
+            config_path = []
+            file_name_env_id = env + "/" + env_id + ".yaml"
+            file_name_env = env + "/" + env_id + ".yaml"
+            config_path_env_id = [os.path.join(config_path_default, agent, file_name_env_id) for agent in method]
+            config_path_env = [os.path.join(config_path_default, agent, file_name_env) for agent in method]
+            for i_agent, agent in enumerate(method):
+                if os.path.exists(config_path_env_id[i_agent]):
+                    config_path.append(config_path_env_id[i_agent])
+                elif os.path.exists(config_path_env[i_agent]):
+                    config_path.append(config_path_env[i_agent])
+                else:
+                    raise RuntimeError(
+                        f"Cannot find file named '{config_path_env_id[i_agent]}' or '{config_path_env[i_agent]}'."
+                        f"You can also customize the configuration file by specifying the `config_path` parameter "
+                        f"in the `get_runner()` function.")
+        else:
+            config_path = [os.path.join(main_path, _path) for _path in config_path]
+        config_algo_default = [get_config(_path) for _path in config_path]
         configs = [recursive_dict_update(config_basic, config_i) for config_i in config_algo_default]
-        if config_path is not None:
-            config_algo = [get_config(os.path.join(main_path, _path)) for _path in config_path]
-            configs = [recursive_dict_update(config_i, config_algo[i]) for i, config_i in enumerate(configs)]
+        # load parser_args and rewrite the parameters if their names are same.
         if parser_args is not None:
             configs = [recursive_dict_update(config_i, parser_args.__dict__) for config_i in configs]
         args = [SN(**config_i) for config_i in configs]
+        if is_test:  # for test mode
+            for i_args in range(len(args)):
+                args[i_args].test_mode = int(is_test)
+                args[i_args].parallels = 1
     elif type(method) == str:
         if config_path is None:
             file_name_env_id = env + "/" + env_id + ".yaml"
             file_name_env = env + ".yaml"
             config_path_env_id = os.path.join(config_path_default, method, file_name_env_id)
             config_path_env = os.path.join(config_path_default, method, file_name_env)
             if os.path.exists(config_path_env_id):
@@ -104,14 +124,17 @@
         configs = recursive_dict_update(config_basic, config_algo_default)
         # load parser_args and rewrite the parameters if their names are same.
         if parser_args is not None:
             configs = recursive_dict_update(configs, parser_args.__dict__)
         if not ('env_id' in configs.keys()):
             configs['env_id'] = env_id
         args = SN(**configs)
+        if is_test:
+            args.test_mode = int(is_test)
+            args.parallels = 1
     else:
         raise RuntimeError("Unsupported agent_name or env_name!")
     return args
 
 
 def get_runner(method,
                env,
@@ -128,15 +151,15 @@
         config_path: default is None, if None, the default configs (xuance/configs/.../*.yaml) will be loaded.
         parser_args: arguments that specified by parser tools.
         is_test: default is False, if True, it will load the models and run the environment with rendering.
 
     Returns:
         An implementation of a runner that enables to run the DRL algorithms.
     """
-    args = get_arguments(method, env, env_id, config_path, parser_args)
+    args = get_arguments(method, env, env_id, config_path, parser_args, is_test)
 
     device = args[0].device if type(args) == list else args.device
     dl_toolbox = args[0].dl_toolbox if type(args) == list else args.dl_toolbox
     print("Calculating device:", device)
 
     if dl_toolbox == "torch":
         from xuance.torch.runners import REGISTRY as run_REGISTRY
@@ -184,18 +207,14 @@
                     raise RuntimeError(f"The method named '{method[i_alg]}' is currently not supported in XuanCe.")
                 elif args[i_alg].env not in method_list[method[i_alg]]:
                     raise RuntimeError(
                         f"The environment named '{args[i_alg].env}' is currently not supported for {method_list[method[i_alg]]}.")
                 else:
                     print("Failed to load arguments for the implementation!")
 
-            if is_test:
-                args[i_alg].test_mode = int(is_test)
-                args[i_alg].parallels = 1
-
         # print("Algorithm:", *[arg.agent for arg in args])
         print("Algorithm:", *agents_name_string)
         print("Environment:", args[0].env_name)
         print("Scenario:", args[0].env_id)
         for arg in args:
             if arg.agent_name != "random":
                 runner = run_REGISTRY[arg.runner](args)
@@ -213,17 +232,14 @@
             elif args.method not in method_list.keys():
                 raise RuntimeError(f"The method named '{args.method}' is currently not supported in XuanCe.")
             elif args.env not in method_list[args.method]:
                 raise RuntimeError(f"The environment named '{args.env}' is currently not supported for {args.method}.")
             else:
                 print("Failed to load arguments for the implementation!")
 
-        if is_test:
-            args.test_mode = int(is_test)
-            args.parallels = 1
         print("Algorithm:", args.agent)
         print("Environment:", args.env_name)
         print("Scenario:", args.env_id)
         runner = run_REGISTRY[args[0].runner](args) if type(args) == list else run_REGISTRY[args.runner](args)
         return runner
 
 
@@ -273,14 +289,16 @@
         observation_space: the space variable with type of gym.Space.
 
     Returns:
         The shape of the observation_space.
     """
     if isinstance(observation_space, Dict):
         return {key: observation_space[key].shape for key in observation_space.keys()}
+    elif isinstance(observation_space, tuple):
+        return observation_space
     else:
         return observation_space.shape
 
 
 def discount_cumsum(x, discount=0.99):
     """Get a discounted cumulated summation.
     Args:
@@ -294,7 +312,19 @@
     --------
     >>> x = [0, 1, 2, 2]
     >>> y = discount_cumsum(x, discount=0.99)
     [4.890798, 4.9402, 3.98, 2.0]
     """
     return scipy.signal.lfilter([1], [1, float(-discount)], x[::-1], axis=0)[::-1]
 
+
+def get_time_string():
+    t_now = time.localtime(time.time())
+    t_year = str(t_now.tm_year).zfill(4)
+    t_month = str(t_now.tm_mon).zfill(2)
+    t_day = str(t_now.tm_mday).zfill(2)
+    t_hour = str(t_now.tm_hour).zfill(2)
+    t_min = str(t_now.tm_min).zfill(2)
+    t_sec = str(t_now.tm_sec).zfill(2)
+    time_string = f"{t_year}_{t_month}{t_day}_{t_hour}{t_min}{t_sec}"
+    return time_string
+
```

### Comparing `xuance-1.0.9/xuance/common/memory_tools.py` & `xuance-1.1.0/xuance/common/memory_tools.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/common/memory_tools_marl.py` & `xuance-1.1.0/xuance/common/memory_tools_marl.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,16 +75,16 @@
             'obs': np.zeros((self.n_envs, self.n_size, self.n_agents) + self.obs_space).astype(np.float32),
             'actions': np.zeros((self.n_envs, self.n_size, self.n_agents) + self.act_space).astype(np.float32),
             'rewards': np.zeros((self.n_envs, self.n_size,) + self.rew_space).astype(np.float32),
             'returns': np.zeros((self.n_envs, self.n_size,) + self.rew_space).astype(np.float32),
             'values': np.zeros((self.n_envs, self.n_size, self.n_agents, 1)).astype(np.float32),
             'log_pi_old': np.zeros((self.n_envs, self.n_size, self.n_agents,)).astype(np.float32),
             'advantages': np.zeros((self.n_envs, self.n_size,) + self.rew_space).astype(np.float32),
-            'terminals': np.zeros((self.n_envs, self.n_size,) + self.done_space).astype(np.bool),
-            'agent_mask': np.ones((self.n_envs, self.n_size, self.n_agents)).astype(np.bool),
+            'terminals': np.zeros((self.n_envs, self.n_size,) + self.done_space).astype(np.bool_),
+            'agent_mask': np.ones((self.n_envs, self.n_size, self.n_agents)).astype(np.bool_),
         }
         if self.state_space is not None:
             self.data.update({'state': np.zeros((self.n_envs, self.n_size,) + self.state_space).astype(np.float32)})
         self.ptr, self.size = 0, 0
         self.start_ids = np.zeros(self.n_envs, np.int64)  # the start index of the last episode for each env.
 
     def store(self, step_data):
@@ -108,26 +108,33 @@
         # calculate advantages and returns
         rewards = np.array(self.data['rewards'][i_env, path_slice])
         vs = np.append(np.array(self.data['values'][i_env, path_slice]), [value], axis=0)
         dones = np.array(self.data['terminals'][i_env, path_slice])[:, :, None]
         returns = np.zeros_like(rewards)
         last_gae_lam = 0
         step_nums = len(path_slice)
+        use_value_norm = False if (value_normalizer is None) else True
 
         if self.use_gae:
             for t in reversed(range(step_nums)):
-                delta = rewards[t] + (1 - dones[t]) * self.gamma * vs[t + 1] - vs[t]
+                if use_value_norm:
+                    vs_t, vs_next = value_normalizer.denormalize(vs[t]), value_normalizer.denormalize(vs[t + 1])
+                else:
+                    vs_t, vs_next = vs[t], vs[t + 1]
+                delta = rewards[t] + (1 - dones[t]) * self.gamma * vs_next - vs_t
                 last_gae_lam = delta + (1 - dones[t]) * self.gamma * self.gae_lambda * last_gae_lam
-                returns[t] = last_gae_lam + vs[t]
+                returns[t] = last_gae_lam + vs_t
+            advantages = returns - value_normalizer.denormalize(vs[:-1]) if use_value_norm else returns - vs[:-1]
         else:
             returns = np.append(returns, [value], axis=0)
             for t in reversed(range(step_nums)):
                 returns[t] = rewards[t] + (1 - dones[t]) * self.gamma * returns[t + 1]
+            advantages = returns - value_normalizer.denormalize(vs) if use_value_norm else returns - vs
+            advantages = advantages[:-1]
 
-        advantages = returns - vs[:-1]
         self.data['returns'][i_env, path_slice] = returns
         self.data['advantages'][i_env, path_slice] = advantages
         self.start_ids[i_env] = self.ptr
 
     def sample(self, indexes):
         assert self.full, "Not enough transitions for on-policy buffer to random sample"
 
@@ -184,17 +191,17 @@
             'obs': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len + 1) + self.obs_space, np.float32),
             'actions': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len) + self.act_space, np.float32),
             'rewards': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len) + self.rew_space, np.float32),
             'returns': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len) + self.rew_space, np.float32),
             'values': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len) + self.rew_space, np.float32),
             'advantages': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len) + self.rew_space, np.float32),
             'log_pi_old': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len,), np.float32),
-            'terminals': np.zeros((self.buffer_size, self.max_eps_len) + self.done_space, np.bool),
-            'avail_actions': np.ones((self.buffer_size, self.n_agents, self.max_eps_len + 1, self.dim_act), np.bool),
-            'filled': np.zeros((self.buffer_size, self.max_eps_len, 1), np.bool)
+            'terminals': np.zeros((self.buffer_size, self.max_eps_len) + self.done_space, np.bool_),
+            'avail_actions': np.ones((self.buffer_size, self.n_agents, self.max_eps_len + 1, self.dim_act), np.bool_),
+            'filled': np.zeros((self.buffer_size, self.max_eps_len, 1), np.bool_)
         }
         if self.state_space is not None:
             self.data.update({
                 'state': np.zeros((self.buffer_size, self.max_eps_len + 1) + self.state_space, np.float32)
             })
         self.ptr, self.size = 0, 0
 
@@ -203,17 +210,17 @@
             'obs': np.zeros((self.n_envs, self.n_agents, self.max_eps_len + 1) + self.obs_space, dtype=np.float32),
             'actions': np.zeros((self.n_envs, self.n_agents, self.max_eps_len) + self.act_space, dtype=np.float32),
             'rewards': np.zeros((self.n_envs, self.n_agents, self.max_eps_len) + self.rew_space, dtype=np.float32),
             'returns': np.zeros((self.n_envs, self.n_agents, self.max_eps_len) + self.rew_space, np.float32),
             'values': np.zeros((self.n_envs, self.n_agents, self.max_eps_len) + self.rew_space, np.float32),
             'advantages': np.zeros((self.n_envs, self.n_agents, self.max_eps_len) + self.rew_space, np.float32),
             'log_pi_old': np.zeros((self.n_envs, self.n_agents, self.max_eps_len,), np.float32),
-            'terminals': np.zeros((self.n_envs, self.max_eps_len) + self.done_space, dtype=np.bool),
-            'avail_actions': np.ones((self.n_envs, self.n_agents, self.max_eps_len + 1, self.dim_act), dtype=np.bool),
-            'filled': np.zeros((self.n_envs, self.max_eps_len, 1), dtype=np.bool),
+            'terminals': np.zeros((self.n_envs, self.max_eps_len) + self.done_space, dtype=np.bool_),
+            'avail_actions': np.ones((self.n_envs, self.n_agents, self.max_eps_len + 1, self.dim_act), dtype=np.bool_),
+            'filled': np.zeros((self.n_envs, self.max_eps_len, 1), dtype=np.bool_),
         }
         if self.state_space is not None:
             self.episode_data.update({
                 'state': np.zeros((self.n_envs, self.max_eps_len + 1) + self.state_space, dtype=np.float32),
             })
 
     def store_transitions(self, t_envs, *transition_data):
@@ -335,16 +342,16 @@
             'obs': np.zeros((self.n_envs, self.n_size, self.n_agents) + self.obs_space).astype(np.float32),
             'actions': np.zeros((self.n_envs, self.n_size, self.n_agents) + self.act_space).astype(np.float32),
             'act_mean': np.zeros((self.n_envs, self.n_size,) + self.prob_space).astype(np.float32),
             'rewards': np.zeros((self.n_envs, self.n_size,) + self.rew_space).astype(np.float32),
             'returns': np.zeros((self.n_envs, self.n_size,) + self.rew_space).astype(np.float32),
             'values': np.zeros((self.n_envs, self.n_size, self.n_agents, 1)).astype(np.float32),
             'advantages': np.zeros((self.n_envs, self.n_size,) + self.rew_space).astype(np.float32),
-            'terminals': np.zeros((self.n_envs, self.n_size,) + self.done_space).astype(np.bool),
-            'agent_mask': np.ones((self.n_envs, self.n_size, self.n_agents)).astype(np.bool),
+            'terminals': np.zeros((self.n_envs, self.n_size,) + self.done_space).astype(np.bool_),
+            'agent_mask': np.ones((self.n_envs, self.n_size, self.n_agents)).astype(np.bool_),
         })
         if self.state_space is not None:
             self.data.update({'state': np.zeros((self.n_envs, self.n_size,) + self.state_space).astype(np.float32)})
         self.ptr = 0  # current pointer
         self.size = 0  # current buffer size
         self.start_ids = np.zeros(self.n_envs)
 
@@ -367,16 +374,16 @@
             'obs': np.zeros((self.n_envs, self.n_size, self.n_agents) + self.obs_space).astype(np.float32),
             'actions': np.zeros((self.n_envs, self.n_size, self.n_agents) + self.act_space).astype(np.float32),
             'actions_onehot': np.zeros((self.n_envs, self.n_size, self.n_agents, self.dim_act)).astype(np.float32),
             'rewards': np.zeros((self.n_envs, self.n_size,) + self.rew_space).astype(np.float32),
             'returns': np.zeros((self.n_envs, self.n_size,) + self.rew_space).astype(np.float32),
             'values': np.zeros((self.n_envs, self.n_size, self.n_agents, 1)).astype(np.float32),
             'log_pi_old': np.zeros((self.n_envs, self.n_size, self.n_agents,)).astype(np.float32),
-            'terminals': np.zeros((self.n_envs, self.n_size,) + self.done_space).astype(np.bool),
-            'agent_mask': np.ones((self.n_envs, self.n_size, self.n_agents)).astype(np.bool),
+            'terminals': np.zeros((self.n_envs, self.n_size,) + self.done_space).astype(np.bool_),
+            'agent_mask': np.ones((self.n_envs, self.n_size, self.n_agents)).astype(np.bool_),
         }
         if self.state_space is not None:
             self.data.update({'state': np.zeros((self.n_envs, self.n_size,) + self.state_space).astype(np.float32)})
         self.ptr, self.size = 0, 0
         self.start_ids = np.zeros(self.n_envs, np.int64)  # the start index of the last episode for each env.
 
     def finish_path(self, value, i_env, value_normalizer=None):  # when an episode is finished
@@ -435,17 +442,17 @@
             'actions_onehot': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len, self.dim_act)).astype(
                 np.float32),
             'rewards': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len) + self.rew_space, np.float32),
             'returns': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len) + self.rew_space, np.float32),
             'values': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len) + self.rew_space, np.float32),
             'advantages': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len) + self.rew_space, np.float32),
             'log_pi_old': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len,), np.float32),
-            'terminals': np.zeros((self.buffer_size, self.max_eps_len) + self.done_space, np.bool),
-            'avail_actions': np.ones((self.buffer_size, self.n_agents, self.max_eps_len + 1, self.dim_act), np.bool),
-            'filled': np.zeros((self.buffer_size, self.max_eps_len, 1), np.bool)
+            'terminals': np.zeros((self.buffer_size, self.max_eps_len) + self.done_space, np.bool_),
+            'avail_actions': np.ones((self.buffer_size, self.n_agents, self.max_eps_len + 1, self.dim_act), np.bool_),
+            'filled': np.zeros((self.buffer_size, self.max_eps_len, 1), np.bool_)
         }
         if self.state_space is not None:
             self.data.update({'state': np.zeros(
                 (self.buffer_size, self.max_eps_len + 1) + self.state_space, np.float32)})
         self.ptr, self.size = 0, 0
 
     def clear_episodes(self):
@@ -454,17 +461,17 @@
             'actions': np.zeros((self.n_envs, self.n_agents, self.max_eps_len) + self.act_space, dtype=np.float32),
             'actions_onehot': np.zeros((self.n_envs, self.n_agents, self.max_eps_len, self.dim_act), dtype=np.float32),
             'rewards': np.zeros((self.n_envs, self.n_agents, self.max_eps_len) + self.rew_space, dtype=np.float32),
             'returns': np.zeros((self.n_envs, self.n_agents, self.max_eps_len) + self.rew_space, np.float32),
             'values': np.zeros((self.n_envs, self.n_agents, self.max_eps_len) + self.rew_space, np.float32),
             'advantages': np.zeros((self.n_envs, self.n_agents, self.max_eps_len) + self.rew_space, np.float32),
             'log_pi_old': np.zeros((self.n_envs, self.n_agents, self.max_eps_len,), np.float32),
-            'terminals': np.zeros((self.n_envs, self.max_eps_len) + self.done_space, dtype=np.bool),
-            'avail_actions': np.ones((self.n_envs, self.n_agents, self.max_eps_len + 1, self.dim_act), dtype=np.bool),
-            'filled': np.zeros((self.n_envs, self.max_eps_len, 1), dtype=np.bool),
+            'terminals': np.zeros((self.n_envs, self.max_eps_len) + self.done_space, dtype=np.bool_),
+            'avail_actions': np.ones((self.n_envs, self.n_agents, self.max_eps_len + 1, self.dim_act), dtype=np.bool_),
+            'filled': np.zeros((self.n_envs, self.max_eps_len, 1), dtype=np.bool_),
         }
         if self.state_space is not None:
             self.episode_data.update({
                 'state': np.zeros((self.n_envs, self.max_eps_len + 1) + self.state_space, dtype=np.float32)
             })
 
     def store_transitions(self, t_envs, *transition_data):
@@ -542,16 +549,16 @@
 
     def clear(self):
         self.data = {
             'obs': np.zeros((self.n_envs, self.n_size, self.n_agents) + self.obs_space).astype(np.float32),
             'actions': np.zeros((self.n_envs, self.n_size, self.n_agents) + self.act_space).astype(np.float32),
             'obs_next': np.zeros((self.n_envs, self.n_size, self.n_agents) + self.obs_space).astype(np.float32),
             'rewards': np.zeros((self.n_envs, self.n_size) + self.rew_space).astype(np.float32),
-            'terminals': np.zeros((self.n_envs, self.n_size) + self.done_space).astype(np.bool),
-            'agent_mask': np.ones((self.n_envs, self.n_size, self.n_agents)).astype(np.bool)
+            'terminals': np.zeros((self.n_envs, self.n_size) + self.done_space).astype(np.bool_),
+            'agent_mask': np.ones((self.n_envs, self.n_size, self.n_agents)).astype(np.bool_)
         }
         if self.state_space is not None:
             self.data.update({'state': np.zeros((self.n_envs, self.n_size) + self.state_space).astype(np.float32),
                               'state_next': np.zeros((self.n_envs, self.n_size) + self.state_space).astype(np.float32)})
         self.ptr, self.size = 0, 0
 
     def store(self, step_data):
@@ -595,31 +602,31 @@
         self.clear_episodes()
 
     def clear(self):
         self.data = {
             'obs': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len + 1) + self.obs_space, np.float),
             'actions': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len) + self.act_space, np.float),
             'rewards': np.zeros((self.buffer_size, self.n_agents, self.max_eps_len) + self.rew_space, np.float),
-            'terminals': np.zeros((self.buffer_size, self.max_eps_len) + self.done_space, np.bool),
-            'avail_actions': np.ones((self.buffer_size, self.n_agents, self.max_eps_len + 1, self.dim_act), np.bool),
-            'filled': np.zeros((self.buffer_size, self.max_eps_len, 1)).astype(np.bool)
+            'terminals': np.zeros((self.buffer_size, self.max_eps_len) + self.done_space, np.bool_),
+            'avail_actions': np.ones((self.buffer_size, self.n_agents, self.max_eps_len + 1, self.dim_act), np.bool_),
+            'filled': np.zeros((self.buffer_size, self.max_eps_len, 1)).astype(np.bool_)
         }
         if self.state_space is not None:
             self.data.update({'state': np.zeros(
                 (self.buffer_size, self.max_eps_len + 1) + self.state_space).astype(np.float32)})
         self.ptr, self.size = 0, 0
 
     def clear_episodes(self):
         self.episode_data = {
             'obs': np.zeros((self.n_envs, self.n_agents, self.max_eps_len + 1) + self.obs_space, dtype=np.float32),
             'actions': np.zeros((self.n_envs, self.n_agents, self.max_eps_len) + self.act_space, dtype=np.float32),
             'rewards': np.zeros((self.n_envs, self.n_agents, self.max_eps_len) + self.rew_space, dtype=np.float32),
-            'terminals': np.zeros((self.n_envs, self.max_eps_len) + self.done_space, dtype=np.bool),
-            'avail_actions': np.ones((self.n_envs, self.n_agents, self.max_eps_len + 1, self.dim_act), dtype=np.bool),
-            'filled': np.zeros((self.n_envs, self.max_eps_len, 1), dtype=np.bool),
+            'terminals': np.zeros((self.n_envs, self.max_eps_len) + self.done_space, dtype=np.bool_),
+            'avail_actions': np.ones((self.n_envs, self.n_agents, self.max_eps_len + 1, self.dim_act), dtype=np.bool_),
+            'filled': np.zeros((self.n_envs, self.max_eps_len, 1), dtype=np.bool_),
         }
         if self.state_space is not None:
             self.episode_data.update({
                 'state': np.zeros((self.n_envs, self.max_eps_len + 1) + self.state_space, dtype=np.float32),
             })
 
     def store_transitions(self, t_envs, *transition_data):
```

### Comparing `xuance-1.0.9/xuance/common/segtree_tool.py` & `xuance-1.1.0/xuance/common/segtree_tool.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/common/statistic_tools.py` & `xuance-1.1.0/xuance/common/statistic_tools.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/configs/__init__.py` & `xuance-1.1.0/xuance/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/configs/a2c/atari.yaml` & `xuance-1.1.0/xuance/configs/a2c/atari.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [32, 32, 64, 64]
 kernels: [8, 4, 4, 4]
 strides: [4, 2, 2, 2]
 actor_hidden_size: [128, 128]
 critic_hidden_size: [128, 128]
-activation: "LeakyReLU"
+activation: "leaky_relu"
 
 seed: 1
 parallels: 5
 running_steps: 10000000  # 10M
 n_steps: 256  #
 n_epoch: 4
 n_minibatch: 8
```

### Comparing `xuance-1.0.9/xuance/configs/a2c/box2d/BipedalWalker-v3.yaml` & `xuance-1.1.0/xuance/configs/pg/box2d/LunarLander-v2.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-agent: "A2C"
+agent: "PG"
 env_name: "Box2D"
-env_id: "BipedalWalker-v3"
-vectorize: "Dummy_Gym"
-policy: "Gaussian_AC"
+env_id: "LunarLander-v2"
 representation: "Basic_MLP"
+vectorize: "Dummy_Gym"
+policy: "Categorical_Actor"
 runner: "DRL"
 
-representation_hidden_size: [64,]
-actor_hidden_size: [64,]
-critic_hidden_size: [64,]
-activation: 'LeakyReLU'
+representation_hidden_size: [128,]
+actor_hidden_size: [128,]
+activation: 'relu'
 
 seed: 1
 parallels: 10
-running_steps: 1000000
-n_steps: 128
-n_epoch: 5
+running_steps: 300000
+nsteps: 128
+nepoch: 3
+nminibatch: 1
 learning_rate: 0.0004
 
-vf_coef: 0.25
 ent_coef: 0.01
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.98
-use_gae: True
+use_gae: False
 gae_lambda: 0.95
-use_advnorm: True
+use_advnorm: False
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 5
-log_dir: "./logs/a2c/"
-model_dir: "./models/a2c/"
+test_episode: 1
+log_dir: "./logs/pg/"
+model_dir: "./models/pg/"
```

### Comparing `xuance-1.0.9/xuance/configs/a2c/box2d/LunarLander-v2.yaml` & `xuance-1.1.0/xuance/configs/a2c/box2d/LunarLander-v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 policy: "Categorical_AC"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [256,]
 actor_hidden_size: [256,]
 critic_hidden_size: [256,]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
 n_steps: 128
 n_epoch: 1
 learning_rate: 0.0004
```

### Comparing `xuance-1.0.9/xuance/configs/a2c/classic_control/Acrobot-v1.yaml` & `xuance-1.1.0/xuance/configs/a2c/classic_control/CartPole-v1.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 agent: "A2C"
 env_name: "Classic Control"
-env_id: "Acrobot-v1"
-vectorize: "Dummy_Gym"
+env_id: "CartPole-v1"
+vectorize: "Subproc_Gym"
 policy: "Categorical_AC"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [256,]
 actor_hidden_size: [256,]
 critic_hidden_size: [256,]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
 n_steps: 128
 n_epoch: 1
 n_minibatch: 1
```

### Comparing `xuance-1.0.9/xuance/configs/a2c/classic_control/CartPole-v1.yaml` & `xuance-1.1.0/xuance/configs/a2c/classic_control/MountainCar-v0.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 agent: "A2C"
 env_name: "Classic Control"
-env_id: "CartPole-v1"
-vectorize: "Subproc_Gym"
+env_id: "MountainCar-v0"
+vectorize: "Dummy_Gym"
 policy: "Categorical_AC"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [256,]
 actor_hidden_size: [256,]
 critic_hidden_size: [256,]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
 n_steps: 128
 n_epoch: 1
 n_minibatch: 1
```

### Comparing `xuance-1.0.9/xuance/configs/a2c/classic_control/MountainCar-v0.yaml` & `xuance-1.1.0/xuance/configs/pg/classic_control/MountainCar-v0.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-agent: "A2C"
+agent: "PG"
 env_name: "Classic Control"
 env_id: "MountainCar-v0"
-vectorize: "Dummy_Gym"
-policy: "Categorical_AC"
 representation: "Basic_MLP"
+vectorize: "Dummy_Gym"
+policy: "Categorical_Actor"
 runner: "DRL"
 
-representation_hidden_size: [256,]
-actor_hidden_size: [256,]
-critic_hidden_size: [256,]
-activation: 'LeakyReLU'
+representation_hidden_size: [128,]
+actor_hidden_size: [128,]
+activation: 'relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
 n_steps: 128
-n_epoch: 1
+n_epoch: 3
 n_minibatch: 1
 learning_rate: 0.0004
 
-vf_coef: 0.25
 ent_coef: 0.01
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.98
-use_gae: True
+use_gae: False
 gae_lambda: 0.95
-use_advnorm: True
+use_advnorm: False
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 3
-log_dir: "./logs/a2c/"
-model_dir: "./models/a2c/"
+test_episode: 1
+log_dir: "./logs/pg/"
+model_dir: "./models/pg/"
```

### Comparing `xuance-1.0.9/xuance/configs/a2c/classic_control/Pendulum-v1.yaml` & `xuance-1.1.0/xuance/configs/a2c/classic_control/Pendulum-v1.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 policy: "Gaussian_AC"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [256,]
 actor_hidden_size: [256,]
 critic_hidden_size: [256,]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
+activation_action: 'tanh'
 
 seed: 1
 parallels: 10
-running_steps: 300000
+running_steps: 500000
 n_steps: 64
 n_epoch: 1
 n_minibatch: 1
 learning_rate: 0.0004
 
 vf_coef: 0.25
 ent_coef: 0.01
```

### Comparing `xuance-1.0.9/xuance/configs/a2c/mujoco.yaml` & `xuance-1.1.0/xuance/configs/ppg/classic_control/Pendulum-v1.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-agent: "A2C"
-env_name: "MuJoCo"
-env_id: "Ant-v4"
+agent: "PPG"
+env_name: "Classic Control"
+env_id: "Pendulum-v1"
 vectorize: "Dummy_Gym"
-policy: "Gaussian_AC"
 representation: "Basic_MLP"
+policy: "Gaussian_PPG"
 runner: "DRL"
 
-representation_hidden_size: [256,]
-actor_hidden_size: [256,]
-critic_hidden_size: [256,]
-activation: "LeakyReLU"
+representation_hidden_size: [128,]
+actor_hidden_size: [128,]
+critic_hidden_size: [128,]
+activation: "leaky_relu"
+activation_action: 'tanh'
 
-seed: 6782
-parallels: 16
-running_steps: 1000000  # 1M
-n_steps: 16
+seed: 1
+parallels: 10
+running_steps: 300000
+n_steps: 256
 n_epoch: 1
+policy_nepoch: 4
+value_nepoch: 8 
+aux_nepoch: 8
 n_minibatch: 1
-learning_rate: 0.0007
+learning_rate: 0.001
 
-vf_coef: 0.25
-ent_coef: 0.0
-clip_grad: 0.5
-clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
-gamma: 0.99
+ent_coef: 0.01
+clip_range: 0.2
+kl_beta: 1.0
+gamma: 0.98
 use_gae: True
 gae_lambda: 0.95
 use_advnorm: True
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 5000
-test_episode: 5
-log_dir: "./logs/a2c/"
-model_dir: "./models/a2c/"
+eval_interval: 50000
+test_episode: 1
+log_dir: "./logs/ppg/"
+model_dir: "./models/ppg/"
```

### Comparing `xuance-1.0.9/xuance/configs/c51/atari.yaml` & `xuance-1.1.0/xuance/configs/c51/atari.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [32, 64, 64]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512, ]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1069
 parallels: 5
 n_size: 100000
 batch_size: 32  # 64
 learning_rate: 0.0001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/c51/box2d/CarRacing-v2.yaml` & `xuance-1.1.0/xuance/configs/c51/box2d/CarRacing-v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [16, 16, 32]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 2
 n_size: 10000
 batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/c51/box2d/LunarLander-v2.yaml` & `xuance-1.1.0/xuance/configs/c51/box2d/LunarLander-v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 vectorize: "Dummy_Gym"
 policy: "C51_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 20000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/c51/classic_control/Acrobot-v1.yaml` & `xuance-1.1.0/xuance/configs/c51/classic_control/MountainCar-v0.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 agent: "C51DQN"
 env_name: "Classic Control"
-env_id: "Acrobot-v1"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
 policy: "C51_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 20000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
@@ -21,15 +21,15 @@
 atom_num: 51
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 10000
 sync_frequency: 100
 training_frequency: 1
-running_steps: 300000
+running_steps: 200000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
```

### Comparing `xuance-1.0.9/xuance/configs/c51/classic_control/CartPole-v1.yaml` & `xuance-1.1.0/xuance/configs/ddqn/classic_control/CartPole-v1.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-agent: "C51DQN"
+agent: "DDQN"
 env_name: "Classic Control"
 env_id: "CartPole-v1"
 vectorize: "Dummy_Gym"
-policy: "C51_Q_network"
+policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 20000
-batch_size: 256
+batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
-vmin: 0
-vmax: 200
-atom_num: 51
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 10000
 sync_frequency: 100
 training_frequency: 1
-running_steps: 200000
+running_steps: 300000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/c51/"
-model_dir: "./models/c51/"
+log_dir: "./logs/ddqn/"
+model_dir: "./models/ddqn/"
+
```

### Comparing `xuance-1.0.9/xuance/configs/c51/classic_control/MountainCar-v0.yaml` & `xuance-1.1.0/xuance/configs/ddqn/classic_control/Acrobot-v1.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-agent: "C51DQN"
+agent: "DDQN"
 env_name: "Classic Control"
-env_id: "MountainCar-v0"
+env_id: "Acrobot-v1"
 vectorize: "Dummy_Gym"
-policy: "C51_Q_network"
+policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 20000
-batch_size: 256
+batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
-vmin: 0
-vmax: 200
-atom_num: 51
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 10000
 sync_frequency: 100
 training_frequency: 1
-running_steps: 200000
+running_steps: 300000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/c51/"
-model_dir: "./models/c51/"
+log_dir: "./logs/ddqn/"
+model_dir: "./models/ddqn/"
+
```

### Comparing `xuance-1.0.9/xuance/configs/coma/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/coma/mpe/simple_spread_v3.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 use_recurrent: False
 rnn:
 representation_hidden_size: [128, ]
 gain: 0.01
 
 actor_hidden_size: [128, ]
 critic_hidden_size: [128, ]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 10
 n_size: 250
 n_epoch: 10
 n_minibatch: 1
 learning_rate_actor: 0.0007
```

### Comparing `xuance-1.0.9/xuance/configs/coma/sc2/1c3s5z.yaml` & `xuance-1.1.0/xuance/configs/coma/sc2/1c3s5z.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
```

### Comparing `xuance-1.0.9/xuance/configs/coma/sc2/25m.yaml` & `xuance-1.1.0/xuance/configs/coma/sc2/2s3z.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "COMA"  # the learning algorithms_marl
 env_name: "StarCraft2"
-env_id: "25m"
+env_id: "2s3z"
 fps: 15
 policy: "Categorical_COMA_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 
 use_recurrent: True
@@ -16,15 +16,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
@@ -33,25 +33,25 @@
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.95  # discount factor
 td_lambda: 0.8
 
 start_greedy: 0.5
 end_greedy: 0.01
-decay_step_greedy: 1000000
+decay_step_greedy: 2500000
 sync_frequency: 200
 
 use_global_state: True  # if use global state to replace merged observations
 use_advnorm: False
 use_gae:
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 5000000
+running_steps: 2000000
 train_per_step: True
 training_frequency: 1
 
 test_steps: 10000
-eval_interval: 50000
+eval_interval: 20000
 test_episode: 16
 log_dir: "./logs/coma/"
 model_dir: "./models/coma/"
```

### Comparing `xuance-1.0.9/xuance/configs/coma/sc2/2m_vs_1z.yaml` & `xuance-1.1.0/xuance/configs/coma/sc2/3m.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "COMA"  # the learning algorithms_marl
 env_name: "StarCraft2"
-env_id: "2m_vs_1z"
+env_id: "3m"
 fps: 15
 policy: "Categorical_COMA_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 
 use_recurrent: True
@@ -16,15 +16,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
@@ -33,15 +33,15 @@
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.95  # discount factor
 td_lambda: 0.8
 
 start_greedy: 0.5
 end_greedy: 0.01
-decay_step_greedy: 2500000
+decay_step_greedy: 100000
 sync_frequency: 200
 
 use_global_state: True  # if use global state to replace merged observations
 use_advnorm: False
 use_gae:
 gae_lambda: 0.95
```

### Comparing `xuance-1.0.9/xuance/configs/coma/sc2/2s3z.yaml` & `xuance-1.1.0/xuance/configs/coma/sc2/5m_vs_6m.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "COMA"  # the learning algorithms_marl
 env_name: "StarCraft2"
-env_id: "2s3z"
+env_id: "5m_vs_6m"
 fps: 15
 policy: "Categorical_COMA_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 
 use_recurrent: True
@@ -16,15 +16,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
@@ -33,25 +33,25 @@
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.95  # discount factor
 td_lambda: 0.8
 
 start_greedy: 0.5
 end_greedy: 0.01
-decay_step_greedy: 2500000
+decay_step_greedy: 2000000
 sync_frequency: 200
 
 use_global_state: True  # if use global state to replace merged observations
 use_advnorm: False
 use_gae:
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 2000000
+running_steps: 10000000
 train_per_step: True
 training_frequency: 1
 
 test_steps: 10000
-eval_interval: 20000
+eval_interval: 100000
 test_episode: 16
 log_dir: "./logs/coma/"
 model_dir: "./models/coma/"
```

### Comparing `xuance-1.0.9/xuance/configs/coma/sc2/3m.yaml` & `xuance-1.1.0/xuance/configs/coma/sc2/2m_vs_1z.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "COMA"  # the learning algorithms_marl
 env_name: "StarCraft2"
-env_id: "3m"
+env_id: "2m_vs_1z"
 fps: 15
 policy: "Categorical_COMA_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 
 use_recurrent: True
@@ -16,15 +16,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
@@ -33,15 +33,15 @@
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.95  # discount factor
 td_lambda: 0.8
 
 start_greedy: 0.5
 end_greedy: 0.01
-decay_step_greedy: 100000
+decay_step_greedy: 2500000
 sync_frequency: 200
 
 use_global_state: True  # if use global state to replace merged observations
 use_advnorm: False
 use_gae:
 gae_lambda: 0.95
```

### Comparing `xuance-1.0.9/xuance/configs/coma/sc2/5m_vs_6m.yaml` & `xuance-1.1.0/xuance/configs/coma/sc2/MMM2.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "COMA"  # the learning algorithms_marl
 env_name: "StarCraft2"
-env_id: "5m_vs_6m"
+env_id: "MMM2"
 fps: 15
 policy: "Categorical_COMA_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 
 use_recurrent: True
@@ -16,15 +16,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
@@ -33,15 +33,15 @@
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.95  # discount factor
 td_lambda: 0.8
 
 start_greedy: 0.5
 end_greedy: 0.01
-decay_step_greedy: 2000000
+decay_step_greedy: 1000000
 sync_frequency: 200
 
 use_global_state: True  # if use global state to replace merged observations
 use_advnorm: False
 use_gae:
 gae_lambda: 0.95
```

### Comparing `xuance-1.0.9/xuance/configs/coma/sc2/8m.yaml` & `xuance-1.1.0/xuance/configs/coma/sc2/25m.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "COMA"  # the learning algorithms_marl
 env_name: "StarCraft2"
-env_id: "8m"
+env_id: "25m"
 fps: 15
 policy: "Categorical_COMA_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 
 use_recurrent: True
@@ -16,15 +16,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
@@ -33,25 +33,25 @@
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.95  # discount factor
 td_lambda: 0.8
 
 start_greedy: 0.5
 end_greedy: 0.01
-decay_step_greedy: 2500000
+decay_step_greedy: 1000000
 sync_frequency: 200
 
 use_global_state: True  # if use global state to replace merged observations
 use_advnorm: False
 use_gae:
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 1000000
+running_steps: 5000000
 train_per_step: True
 training_frequency: 1
 
 test_steps: 10000
-eval_interval: 10000
+eval_interval: 50000
 test_episode: 16
 log_dir: "./logs/coma/"
 model_dir: "./models/coma/"
```

### Comparing `xuance-1.0.9/xuance/configs/coma/sc2/8m_vs_9m.yaml` & `xuance-1.1.0/xuance/configs/coma/sc2/8m_vs_9m.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
```

### Comparing `xuance-1.0.9/xuance/configs/coma/sc2/MMM2.yaml` & `xuance-1.1.0/xuance/configs/coma/sc2/8m.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "COMA"  # the learning algorithms_marl
 env_name: "StarCraft2"
-env_id: "MMM2"
+env_id: "8m"
 fps: 15
 policy: "Categorical_COMA_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 
 use_recurrent: True
@@ -16,15 +16,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
@@ -33,25 +33,25 @@
 clip_grad: 10
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.95  # discount factor
 td_lambda: 0.8
 
 start_greedy: 0.5
 end_greedy: 0.01
-decay_step_greedy: 1000000
+decay_step_greedy: 2500000
 sync_frequency: 200
 
 use_global_state: True  # if use global state to replace merged observations
 use_advnorm: False
 use_gae:
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 10000000
+running_steps: 1000000
 train_per_step: True
 training_frequency: 1
 
 test_steps: 10000
-eval_interval: 100000
+eval_interval: 10000
 test_episode: 16
 log_dir: "./logs/coma/"
 model_dir: "./models/coma/"
```

### Comparing `xuance-1.0.9/xuance/configs/coma/sc2/corridor.yaml` & `xuance-1.1.0/xuance/configs/coma/sc2/corridor.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [128, 128]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 8
 n_epoch: 1
 n_minibatch: 1
 learning_rate_actor: 0.0007
```

### Comparing `xuance-1.0.9/xuance/configs/dcg/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/dcg/mpe/simple_spread_v3.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 rnn:
 representation_hidden_size: [32, ]
 q_hidden_size: [128, ]  # the units for each hidden layer
 hidden_utility_dim: 256  # hidden units of the utility function
 hidden_payoff_dim: 256  # hidden units of the payoff function
 bias_net: "Basic_MLP"
 hidden_bias_dim: [256, ]  # hidden units of the bias network with global states as input
-activation: "ReLU"
+activation: "relu"
 
 low_rank_payoff: False  # low-rank approximation of payoff function
 payoff_rank: 5  # the rank K in the paper
 graph_type: "FULL"  # specific type of the coordination graph
 n_msg_iterations: 1  # number of iterations for message passing during belief propagation
 msg_normalized: True  # Message normalization during greedy action selection (Kok and Vlassis, 2006)
```

### Comparing `xuance-1.0.9/xuance/configs/dcg/sc2/1c3s5z.yaml` & `xuance-1.1.0/xuance/configs/dcg/sc2/MMM2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "DCG"  # Options: DCG, DCG_S
 env_name: "StarCraft2"
-env_id: "1c3s5z"
+env_id: "MMM2"
 fps: 15
 policy: "DCG_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -19,15 +19,15 @@
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
 hidden_utility_dim: 64  # hidden units of the utility function
 hidden_payoff_dim: 64  # hidden units of the payoff function
 bias_net: "Basic_MLP"
 hidden_bias_dim: [64, ]  # hidden units of the bias network with global states as input
-activation: "ReLU"
+activation: "relu"
 
 low_rank_payoff: False  # low-rank approximation of payoff function
 payoff_rank: 5  # the rank K in the paper
 graph_type: "FULL"  # specific type of the coordination graph
 n_msg_iterations: 8  # number of iterations for message passing during belief propagation
 msg_normalized: True  # Message normalization during greedy action selection (Kok and Vlassis, 2006)
 
@@ -39,19 +39,19 @@
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
 decay_step_greedy: 50000
 start_training: 1000  # start training after n episodes
-running_steps: 2000000  # 2M
+running_steps: 10000000  # 10M
 train_per_step: False  # True: train model per step; False: train model per episode.training_frequency: 1
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 20000
+eval_interval: 100000
 test_episode: 16
 log_dir: "./logs/dcg/"
 model_dir: "./models/dcg/"
```

### Comparing `xuance-1.0.9/xuance/configs/dcg/sc2/25m.yaml` & `xuance-1.1.0/xuance/configs/dcg/sc2/25m.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
 hidden_utility_dim: 64  # hidden units of the utility function
 hidden_payoff_dim: 64  # hidden units of the payoff function
 bias_net: "Basic_MLP"
 hidden_bias_dim: [64, ]  # hidden units of the bias network with global states as input
-activation: "ReLU"
+activation: "relu"
 
 low_rank_payoff: False  # low-rank approximation of payoff function
 payoff_rank: 5  # the rank K in the paper
 graph_type: "FULL"  # specific type of the coordination graph
 n_msg_iterations: 8  # number of iterations for message passing during belief propagation
 msg_normalized: True  # Message normalization during greedy action selection (Kok and Vlassis, 2006)
```

### Comparing `xuance-1.0.9/xuance/configs/dcg/sc2/2m_vs_1z.yaml` & `xuance-1.1.0/xuance/configs/dcg/sc2/3m.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "DCG"  # Options: DCG, DCG_S
 env_name: "StarCraft2"
-env_id: "2m_vs_1z"
+env_id: "3m"
 fps: 15
 policy: "DCG_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -19,15 +19,15 @@
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
 hidden_utility_dim: 64  # hidden units of the utility function
 hidden_payoff_dim: 64  # hidden units of the payoff function
 bias_net: "Basic_MLP"
 hidden_bias_dim: [64, ]  # hidden units of the bias network with global states as input
-activation: "ReLU"
+activation: "relu"
 
 low_rank_payoff: False  # low-rank approximation of payoff function
 payoff_rank: 5  # the rank K in the paper
 graph_type: "FULL"  # specific type of the coordination graph
 n_msg_iterations: 8  # number of iterations for message passing during belief propagation
 msg_normalized: True  # Message normalization during greedy action selection (Kok and Vlassis, 2006)
```

### Comparing `xuance-1.0.9/xuance/configs/dcg/sc2/2s3z.yaml` & `xuance-1.1.0/xuance/configs/dcg/sc2/8m_vs_9m.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "DCG"  # Options: DCG, DCG_S
 env_name: "StarCraft2"
-env_id: "2s3z"
+env_id: "8m_vs_9m"
 fps: 15
 policy: "DCG_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -19,15 +19,15 @@
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
 hidden_utility_dim: 64  # hidden units of the utility function
 hidden_payoff_dim: 64  # hidden units of the payoff function
 bias_net: "Basic_MLP"
 hidden_bias_dim: [64, ]  # hidden units of the bias network with global states as input
-activation: "ReLU"
+activation: "relu"
 
 low_rank_payoff: False  # low-rank approximation of payoff function
 payoff_rank: 5  # the rank K in the paper
 graph_type: "FULL"  # specific type of the coordination graph
 n_msg_iterations: 8  # number of iterations for message passing during belief propagation
 msg_normalized: True  # Message normalization during greedy action selection (Kok and Vlassis, 2006)
 
@@ -39,19 +39,19 @@
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
 decay_step_greedy: 50000
 start_training: 1000  # start training after n episodes
-running_steps: 2000000  # 2M
+running_steps: 10000000  # 10M
 train_per_step: False  # True: train model per step; False: train model per episode.training_frequency: 1
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 20000
+eval_interval: 100000
 test_episode: 16
 log_dir: "./logs/dcg/"
 model_dir: "./models/dcg/"
```

### Comparing `xuance-1.0.9/xuance/configs/dcg/sc2/3m.yaml` & `xuance-1.1.0/xuance/configs/dcg/sc2/8m.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "DCG"  # Options: DCG, DCG_S
 env_name: "StarCraft2"
-env_id: "3m"
+env_id: "8m"
 fps: 15
 policy: "DCG_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -19,15 +19,15 @@
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
 hidden_utility_dim: 64  # hidden units of the utility function
 hidden_payoff_dim: 64  # hidden units of the payoff function
 bias_net: "Basic_MLP"
 hidden_bias_dim: [64, ]  # hidden units of the bias network with global states as input
-activation: "ReLU"
+activation: "relu"
 
 low_rank_payoff: False  # low-rank approximation of payoff function
 payoff_rank: 5  # the rank K in the paper
 graph_type: "FULL"  # specific type of the coordination graph
 n_msg_iterations: 8  # number of iterations for message passing during belief propagation
 msg_normalized: True  # Message normalization during greedy action selection (Kok and Vlassis, 2006)
```

### Comparing `xuance-1.0.9/xuance/configs/dcg/sc2/5m_vs_6m.yaml` & `xuance-1.1.0/xuance/configs/dcg/sc2/1c3s5z.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "DCG"  # Options: DCG, DCG_S
 env_name: "StarCraft2"
-env_id: "5m_vs_6m"
+env_id: "1c3s5z"
 fps: 15
 policy: "DCG_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -19,15 +19,15 @@
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
 hidden_utility_dim: 64  # hidden units of the utility function
 hidden_payoff_dim: 64  # hidden units of the payoff function
 bias_net: "Basic_MLP"
 hidden_bias_dim: [64, ]  # hidden units of the bias network with global states as input
-activation: "ReLU"
+activation: "relu"
 
 low_rank_payoff: False  # low-rank approximation of payoff function
 payoff_rank: 5  # the rank K in the paper
 graph_type: "FULL"  # specific type of the coordination graph
 n_msg_iterations: 8  # number of iterations for message passing during belief propagation
 msg_normalized: True  # Message normalization during greedy action selection (Kok and Vlassis, 2006)
 
@@ -39,19 +39,19 @@
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
 decay_step_greedy: 50000
 start_training: 1000  # start training after n episodes
-running_steps: 10000000  # 10M
+running_steps: 2000000  # 2M
 train_per_step: False  # True: train model per step; False: train model per episode.training_frequency: 1
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 100000
+eval_interval: 20000
 test_episode: 16
 log_dir: "./logs/dcg/"
 model_dir: "./models/dcg/"
```

### Comparing `xuance-1.0.9/xuance/configs/dcg/sc2/8m.yaml` & `xuance-1.1.0/xuance/configs/dcg/sc2/corridor.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "DCG"  # Options: DCG, DCG_S
 env_name: "StarCraft2"
-env_id: "8m"
+env_id: "corridor"
 fps: 15
 policy: "DCG_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -19,15 +19,15 @@
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
 hidden_utility_dim: 64  # hidden units of the utility function
 hidden_payoff_dim: 64  # hidden units of the payoff function
 bias_net: "Basic_MLP"
 hidden_bias_dim: [64, ]  # hidden units of the bias network with global states as input
-activation: "ReLU"
+activation: "relu"
 
 low_rank_payoff: False  # low-rank approximation of payoff function
 payoff_rank: 5  # the rank K in the paper
 graph_type: "FULL"  # specific type of the coordination graph
 n_msg_iterations: 8  # number of iterations for message passing during belief propagation
 msg_normalized: True  # Message normalization during greedy action selection (Kok and Vlassis, 2006)
 
@@ -39,19 +39,19 @@
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
 decay_step_greedy: 50000
 start_training: 1000  # start training after n episodes
-running_steps: 1000000  # 1M
+running_steps: 10000000  # 10M
 train_per_step: False  # True: train model per step; False: train model per episode.training_frequency: 1
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 10000
+eval_interval: 100000
 test_episode: 16
 log_dir: "./logs/dcg/"
 model_dir: "./models/dcg/"
```

### Comparing `xuance-1.0.9/xuance/configs/dcg/sc2/8m_vs_9m.yaml` & `xuance-1.1.0/xuance/configs/dcg/sc2/2m_vs_1z.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "DCG"  # Options: DCG, DCG_S
 env_name: "StarCraft2"
-env_id: "8m_vs_9m"
+env_id: "2m_vs_1z"
 fps: 15
 policy: "DCG_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -19,15 +19,15 @@
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
 hidden_utility_dim: 64  # hidden units of the utility function
 hidden_payoff_dim: 64  # hidden units of the payoff function
 bias_net: "Basic_MLP"
 hidden_bias_dim: [64, ]  # hidden units of the bias network with global states as input
-activation: "ReLU"
+activation: "relu"
 
 low_rank_payoff: False  # low-rank approximation of payoff function
 payoff_rank: 5  # the rank K in the paper
 graph_type: "FULL"  # specific type of the coordination graph
 n_msg_iterations: 8  # number of iterations for message passing during belief propagation
 msg_normalized: True  # Message normalization during greedy action selection (Kok and Vlassis, 2006)
 
@@ -39,19 +39,19 @@
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
 decay_step_greedy: 50000
 start_training: 1000  # start training after n episodes
-running_steps: 10000000  # 10M
+running_steps: 1000000  # 1M
 train_per_step: False  # True: train model per step; False: train model per episode.training_frequency: 1
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 100000
+eval_interval: 10000
 test_episode: 16
 log_dir: "./logs/dcg/"
 model_dir: "./models/dcg/"
```

### Comparing `xuance-1.0.9/xuance/configs/dcg/sc2/MMM2.yaml` & `xuance-1.1.0/xuance/configs/dcg/sc2/2s3z.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "DCG"  # Options: DCG, DCG_S
 env_name: "StarCraft2"
-env_id: "MMM2"
+env_id: "2s3z"
 fps: 15
 policy: "DCG_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -19,15 +19,15 @@
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
 hidden_utility_dim: 64  # hidden units of the utility function
 hidden_payoff_dim: 64  # hidden units of the payoff function
 bias_net: "Basic_MLP"
 hidden_bias_dim: [64, ]  # hidden units of the bias network with global states as input
-activation: "ReLU"
+activation: "relu"
 
 low_rank_payoff: False  # low-rank approximation of payoff function
 payoff_rank: 5  # the rank K in the paper
 graph_type: "FULL"  # specific type of the coordination graph
 n_msg_iterations: 8  # number of iterations for message passing during belief propagation
 msg_normalized: True  # Message normalization during greedy action selection (Kok and Vlassis, 2006)
 
@@ -39,19 +39,19 @@
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
 decay_step_greedy: 50000
 start_training: 1000  # start training after n episodes
-running_steps: 10000000  # 10M
+running_steps: 2000000  # 2M
 train_per_step: False  # True: train model per step; False: train model per episode.training_frequency: 1
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 100000
+eval_interval: 20000
 test_episode: 16
 log_dir: "./logs/dcg/"
 model_dir: "./models/dcg/"
```

### Comparing `xuance-1.0.9/xuance/configs/dcg/sc2/corridor.yaml` & `xuance-1.1.0/xuance/configs/dcg/sc2/5m_vs_6m.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "DCG"  # Options: DCG, DCG_S
 env_name: "StarCraft2"
-env_id: "corridor"
+env_id: "5m_vs_6m"
 fps: 15
 policy: "DCG_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -19,15 +19,15 @@
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
 hidden_utility_dim: 64  # hidden units of the utility function
 hidden_payoff_dim: 64  # hidden units of the payoff function
 bias_net: "Basic_MLP"
 hidden_bias_dim: [64, ]  # hidden units of the bias network with global states as input
-activation: "ReLU"
+activation: "relu"
 
 low_rank_payoff: False  # low-rank approximation of payoff function
 payoff_rank: 5  # the rank K in the paper
 graph_type: "FULL"  # specific type of the coordination graph
 n_msg_iterations: 8  # number of iterations for message passing during belief propagation
 msg_normalized: True  # Message normalization during greedy action selection (Kok and Vlassis, 2006)
```

### Comparing `xuance-1.0.9/xuance/configs/ddpg/box2d/BipedalWalker-v3.yaml` & `xuance-1.1.0/xuance/configs/ddpg/box2d/BipedalWalker-v3.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 vectorize: "Dummy_Gym"
 policy: "DDPG_Policy"
 representation: "Basic_Identical"
 runner: "DRL"
 
 actor_hidden_size: [256,]
 critic_hidden_size: [256,]
-activation: "ReLU"
+activation: "relu"
+activation_action: 'tanh'
 
 seed: 1
 parallels: 10
 n_size: 200000
 batch_size: 256
 actor_learning_rate: 0.001
 critic_learning_rate: 0.001
```

### Comparing `xuance-1.0.9/xuance/configs/ddpg/classic_control/Pendulum-v1.yaml` & `xuance-1.1.0/xuance/configs/sac/classic_control/Pendulum-v1.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-agent: "DDPG"
+agent: "SAC"
 env_name: "Classic Control"
 env_id: "Pendulum-v1"
 vectorize: "Dummy_Gym"
-policy: "DDPG_Policy"
-representation: "Basic_Identical"
+policy: "Gaussian_SAC"
+representation: "Basic_MLP"
 runner: "DRL"
 
+representation_hidden_size: [256,]
 actor_hidden_size: [256,]
 critic_hidden_size: [256,]
-activation: "ReLU"
+activation: "relu"
+activation_action: 'tanh'
 
 seed: 1
-parallels: 10
-n_size: 200000
+parallels: 16
+n_size: 20000
 batch_size: 256
 actor_learning_rate: 0.001
 critic_learning_rate: 0.001
 gamma: 0.98
 tau: 0.005
-learning_rate: 0.0007
 
-start_noise: 0.1
-end_noise: 0.1
-training_frequency: 1
+start_noise: 0.25
+end_noise: 0.05
+training_frequency: 2
 running_steps: 500000
-start_training: 1000
+start_training: 2000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 3
-log_dir: "./logs/ddpg/"
-model_dir: "./models/ddpg/"
+test_episode: 1
+log_dir: "./logs/sac/"
+model_dir: "./models/sac/"
```

### Comparing `xuance-1.0.9/xuance/configs/ddpg/mujoco.yaml` & `xuance-1.1.0/xuance/configs/ddpg/mujoco.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 policy: "DDPG_Policy"
 representation: "Basic_Identical"
 runner: "DRL"
 
 representation_hidden_size:  # If you choose Basic_Identical representation, then ignore this value
 actor_hidden_size: [400, 300]
 critic_hidden_size: [400, 300]
-activation: "LeakyReLU"
+activation: "leaky_relu"
+activation_action: 'tanh'
 
 seed: 19089
 parallels: 4  # number of environments
 n_size: 50000  # replay buffer size
 batch_size: 100
 actor_learning_rate: 0.001
 critic_learning_rate: 0.001
```

### Comparing `xuance-1.0.9/xuance/configs/ddqn/atari.yaml` & `xuance-1.1.0/xuance/configs/dqn/atari.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-agent: "DDQN"
+agent: "DQN"
 vectorize: "Dummy_Atari"
 env_name: "Atari"
 env_id: "ALE/Breakout-v5"
 obs_type: "grayscale"  # choice for Atari env: ram, rgb, grayscale
 img_size: [84, 84]  # default is 210 x 160 in gym[Atari]
 num_stack: 4  # frame stack trick
 frame_skip: 4  # frame skip trick
@@ -13,20 +13,20 @@
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [32, 64, 64]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512, ]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1069
 parallels: 5
 n_size: 100000
-batch_size: 32
+batch_size: 32  # 64
 learning_rate: 0.0001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.05
 decay_step_greedy: 1000000  # 1M
 sync_frequency: 500
@@ -37,10 +37,10 @@
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 500000
-test_episode: 3
-log_dir: "./logs/ddqn/"
-model_dir: "./models/ddqn/"
+test_episode: 5
+log_dir: "./logs/dqn/"
+model_dir: "./models/dqn/"
```

### Comparing `xuance-1.0.9/xuance/configs/ddqn/box2d/CarRacing-v2.yaml` & `xuance-1.1.0/xuance/configs/ddqn/box2d/CarRacing-v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [16, 16, 32]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 2
 n_size: 10000
 batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/ddqn/box2d/LunarLander-v2.yaml` & `xuance-1.1.0/xuance/configs/ddqn/box2d/LunarLander-v2.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 10000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/ddqn/classic_control/Acrobot-v1.yaml` & `xuance-1.1.0/xuance/configs/ddqn/classic_control/MountainCar-v0.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 agent: "DDQN"
 env_name: "Classic Control"
-env_id: "Acrobot-v1"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 20000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/ddqn/classic_control/CartPole-v1.yaml` & `xuance-1.1.0/xuance/configs/dqn/classic_control/CartPole-v1.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-agent: "DDQN"
+agent: "DQN"
 env_name: "Classic Control"
 env_id: "CartPole-v1"
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
-batch_size: 128
+n_size: 10000
+batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 10000
-sync_frequency: 100
+sync_frequency: 50
 training_frequency: 1
-running_steps: 300000
+running_steps: 200000  # 200k
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 50000
+eval_interval: 20000
 test_episode: 1
-log_dir: "./logs/ddqn/"
-model_dir: "./models/ddqn/"
-
+log_dir: "./logs/dqn/"
+model_dir: "./models/dqn/"
```

### Comparing `xuance-1.0.9/xuance/configs/ddqn/classic_control/MountainCar-v0.yaml` & `xuance-1.1.0/xuance/configs/dqn/box2d/LunarLander-v2.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-agent: "DDQN"
-env_name: "Classic Control"
-env_id: "MountainCar-v0"
+agent: "DQN"
+env_name: "Box2D"
+env_id: "LunarLander-v2"
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
-batch_size: 128
+n_size: 10000
+batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 10000
-sync_frequency: 100
+sync_frequency: 50
 training_frequency: 1
-running_steps: 300000
+running_steps: 200000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/ddqn/"
-model_dir: "./models/ddqn/"
-
+log_dir: "./logs/dqn/"
+model_dir: "./models/dqn/"
```

### Comparing `xuance-1.0.9/xuance/configs/dqn/atari.yaml` & `xuance-1.1.0/xuance/configs/perdqn/atari.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-agent: "DQN"
+agent: "PerDQN"
 vectorize: "Dummy_Atari"
 env_name: "Atari"
 env_id: "ALE/Breakout-v5"
 obs_type: "grayscale"  # choice for Atari env: ram, rgb, grayscale
 img_size: [84, 84]  # default is 210 x 160 in gym[Atari]
 num_stack: 4  # frame stack trick
 frame_skip: 4  # frame skip trick
@@ -13,15 +13,15 @@
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [32, 64, 64]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512, ]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1069
 parallels: 5
 n_size: 100000
 batch_size: 32  # 64
 learning_rate: 0.0001
 gamma: 0.99
@@ -35,12 +35,15 @@
 start_training: 10000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
+PER_alpha: 0.5
+PER_beta0: 0.4
+
 test_steps: 10000
 eval_interval: 500000
-test_episode: 5
-log_dir: "./logs/dqn/"
-model_dir: "./models/dqn/"
+test_episode: 1
+log_dir: "./logs/perdqn/"
+model_dir: "./models/perdqn/"
```

### Comparing `xuance-1.0.9/xuance/configs/dqn/box2d/CarRacing-v2.yaml` & `xuance-1.1.0/xuance/configs/dqn/box2d/CarRacing-v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [16, 16, 32]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 2
 n_size: 10000
 batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/dqn/box2d/LunarLander-v2.yaml` & `xuance-1.1.0/xuance/configs/dqn/classic_control/Acrobot-v1.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 agent: "DQN"
-env_name: "Box2D"
-env_id: "LunarLander-v2"
+env_name: "Classic Control"
+env_id: "Acrobot-v1"
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 10000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 10000
 sync_frequency: 50
 training_frequency: 1
-running_steps: 200000
+running_steps: 200000  # 200k
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 50000
+eval_interval: 20000
 test_episode: 1
 log_dir: "./logs/dqn/"
 model_dir: "./models/dqn/"
```

### Comparing `xuance-1.0.9/xuance/configs/dqn/classic_control/Acrobot-v1.yaml` & `xuance-1.1.0/xuance/configs/dueldqn/box2d/LunarLander-v2.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-agent: "DQN"
-env_name: "Classic Control"
-env_id: "Acrobot-v1"
+agent: "Duel_DQN"
+env_name: "Box2D"
+env_id: "LunarLander-v2"
 vectorize: "Dummy_Gym"
-policy: "Basic_Q_network"
+policy: "Duel_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [128,]
-q_hidden_size: [128,]
-activation: 'ReLU'
+representation_hidden_size: [128, ]
+q_hidden_size: [128, ]
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 10000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
-decay_step_greedy: 10000
+decay_step_greedy: 20000
 sync_frequency: 50
 training_frequency: 1
-running_steps: 200000  # 200k
+running_steps: 500000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 20000
+eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/dqn/"
-model_dir: "./models/dqn/"
+log_dir: "./logs/dueldqn/"
+model_dir: "./models/dueldqn/"
```

### Comparing `xuance-1.0.9/xuance/configs/dqn/classic_control/CartPole-v1.yaml` & `xuance-1.1.0/xuance/configs/dqn/classic_control/MountainCar-v0.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 agent: "DQN"
 env_name: "Classic Control"
-env_id: "CartPole-v1"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [128,]
-q_hidden_size: [128,]
-activation: 'ReLU'
+representation_hidden_size: [256, ]
+q_hidden_size: [256, ]
+activation: 'leaky_relu'
 
 seed: 1
 parallels: 10
-n_size: 10000
+n_size: 20000
 batch_size: 256
-learning_rate: 0.001
+learning_rate: 0.1
 gamma: 0.99
 
-start_greedy: 0.5
+start_greedy: 1.0
 end_greedy: 0.01
-decay_step_greedy: 10000
-sync_frequency: 50
-training_frequency: 1
-running_steps: 200000  # 200k
+sync_frequency: 200
+training_frequency: 2
+running_steps: 2000000  # 2M
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 20000
-test_episode: 1
+eval_interval: 50000
+test_episode: 5
 log_dir: "./logs/dqn/"
 model_dir: "./models/dqn/"
```

### Comparing `xuance-1.0.9/xuance/configs/dqn/classic_control/MountainCar-v0.yaml` & `xuance-1.1.0/xuance/configs/dueldqn/classic_control/Acrobot-v1.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-agent: "DQN"
+agent: "Duel_DQN"
 env_name: "Classic Control"
-env_id: "MountainCar-v0"
+env_id: "Acrobot-v1"
 vectorize: "Dummy_Gym"
-policy: "Basic_Q_network"
+policy: "Duel_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [256, ]
-q_hidden_size: [256, ]
-activation: 'LeakyReLU'
+representation_hidden_size: [128, ]
+q_hidden_size: [128, ]
+activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+n_size: 10000
 batch_size: 256
-learning_rate: 0.1
+learning_rate: 0.001
 gamma: 0.99
 
-start_greedy: 1.0
+start_greedy: 0.5
 end_greedy: 0.01
-sync_frequency: 200
-training_frequency: 2
-running_steps: 2000000  # 2M
+decay_step_greedy: 20000
+sync_frequency: 50
+training_frequency: 1
+running_steps: 500000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 5
-log_dir: "./logs/dqn/"
-model_dir: "./models/dqn/"
+test_episode: 1
+log_dir: "./logs/dueldqn/"
+model_dir: "./models/dueldqn/"
```

### Comparing `xuance-1.0.9/xuance/configs/drqn/atari.yaml` & `xuance-1.1.0/xuance/configs/drqn/atari.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 filters: [32, 64, 64]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 recurrent_hidden_size: 512
 recurrent_layer_N: 1
 dropout: 0
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 5
 n_size: 1000
 batch_size: 8  # batch size for training
 learning_rate: 0.0001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/drqn/box2d/CarRacing-v2.yaml` & `xuance-1.1.0/xuance/configs/drqn/box2d/CarRacing-v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 filters: [16, 16, 32]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 recurrent_hidden_size: 512
 recurrent_layer_N: 1
 dropout: 0
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 2
 n_size: 100
 batch_size: 8  # batch size for training
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/drqn/box2d/LunarLander-v2.yaml` & `xuance-1.1.0/xuance/configs/drqn/classic_control/MountainCar-v0.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 agent: "DRQN"  # deep recurrent Q-networks
 env_name: "Classic Control"
-env_id: "LunarLander-v2"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
 policy: "DRQN_Policy"
 representation: "Basic_MLP"
 runner: "DRL"
 rnn: "LSTM"
 
 representation_hidden_size: [128,]
 recurrent_hidden_size: 128
 recurrent_layer_N: 1
 dropout: 0
-activation: 'ReLU'
+activation: 'relu'
 
-seed: 1
 parallels: 10
-n_size: 50  # memory size for each parallel
+n_size: 10000  # memory size for each parallel
 batch_size: 8  # batch size for training
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
-decay_step_greedy: 5000
+decay_step_greedy: 10000
 sync_frequency: 50
 training_frequency: 1
 running_steps: 300000
 start_training: 1000
 lookup_length: 50
 
 use_obsnorm: False
```

### Comparing `xuance-1.0.9/xuance/configs/drqn/classic_control/Acrobot-v1.yaml` & `xuance-1.1.0/xuance/configs/drqn/classic_control/Acrobot-v1.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 runner: "DRL"
 rnn: "LSTM"
 
 representation_hidden_size: [128,]
 recurrent_hidden_size: 128
 recurrent_layer_N: 1
 dropout: 0
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 10000  # memory size for each parallel
 batch_size: 8  # batch size for training
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/drqn/classic_control/CartPole-v1.yaml` & `xuance-1.1.0/xuance/configs/drqn/classic_control/CartPole-v1.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 runner: "DRL"
 rnn: "LSTM"
 
 representation_hidden_size: [128,]
 recurrent_hidden_size: 128
 recurrent_layer_N: 1
 dropout: 0
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 10000  # memory size for each parallel
 batch_size: 8  # batch size for training
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/drqn/classic_control/MountainCar-v0.yaml` & `xuance-1.1.0/xuance/configs/iql/sc2/corridor.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,47 @@
-agent: "DRQN"  # deep recurrent Q-networks
-env_name: "Classic Control"
-env_id: "MountainCar-v0"
-vectorize: "Dummy_Gym"
-policy: "DRQN_Policy"
-representation: "Basic_MLP"
-runner: "DRL"
-rnn: "LSTM"
+agent: "IQL"  # the learning algorithms_marl
+env_name: "StarCraft2"
+env_id: "corridor"
+fps: 15
+policy: "Basic_Q_network_marl"
+representation: "Basic_RNN"
+vectorize: "Subproc_StarCraft2"
+runner: "StarCraft2_Runner"
+on_policy: False
 
-representation_hidden_size: [128,]
-recurrent_hidden_size: 128
+# recurrent settings for Basic_RNN representation
+use_recurrent: True
+rnn: "GRU"
 recurrent_layer_N: 1
+fc_hidden_sizes: [64, ]
+recurrent_hidden_size: 64
+N_recurrent_layers: 1
 dropout: 0
-activation: 'ReLU'
 
-parallels: 10
-n_size: 10000  # memory size for each parallel
-batch_size: 8  # batch size for training
-learning_rate: 0.001
-gamma: 0.99
-
-start_greedy: 0.5
-end_greedy: 0.01
-decay_step_greedy: 10000
-sync_frequency: 50
+representation_hidden_size: [64, ]
+q_hidden_size: [64, ]  # the units for each hidden layer
+activation: "relu"
+
+seed: 1
+parallels: 8
+buffer_size: 5000
+batch_size: 32
+learning_rate: 0.0007
+gamma: 0.99  # discount factor
+double_q: True  # use double q learning
+
+start_greedy: 1.0
+end_greedy: 0.05
+decay_step_greedy: 50000
+start_training: 1000  # start training after n episodes
+running_steps: 10000000  # 10M
+train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
-running_steps: 300000
-start_training: 1000
-lookup_length: 50
-
-use_obsnorm: False
-use_rewnorm: False
-obsnorm_range: 5
-rewnorm_range: 5
-
-test_steps: 10000
-eval_interval: 50000
-test_episode: 3
-log_dir: "./logs/drqn/"
-model_dir: "./models/drqn/"
+sync_frequency: 200
+
+use_grad_clip: False
+grad_clip_norm: 0.5
+
+eval_interval: 100000
+test_episode: 16
+log_dir: "./logs/iql/"
+model_dir: "./models/iql/"
```

### Comparing `xuance-1.0.9/xuance/configs/dueldqn/atari.yaml` & `xuance-1.1.0/xuance/configs/dueldqn/atari.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [32, 64, 64]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512, ]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1069
 parallels: 5
 n_size: 100000
 batch_size: 32  # 64
 learning_rate: 0.0001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/dueldqn/box2d/CarRacing-v2.yaml` & `xuance-1.1.0/xuance/configs/dueldqn/box2d/CarRacing-v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [16, 16, 32]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 2
 n_size: 10000
 batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/dueldqn/box2d/LunarLander-v2.yaml` & `xuance-1.1.0/xuance/configs/perdqn/classic_control/Acrobot-v1.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-agent: "Duel_DQN"
-env_name: "Box2D"
-env_id: "LunarLander-v2"
+agent: "PerDQN"
+env_name: "Classic Control"
+env_id: "Acrobot-v1"
 vectorize: "Dummy_Gym"
-policy: "Duel_Q_network"
+policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [128, ]
-q_hidden_size: [128, ]
-activation: 'ReLU'
+representation_hidden_size: [128,]
+q_hidden_size: [128,]
+activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 10000
-batch_size: 256
+n_size: 20000
+batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
-end_greedy: 0.01
+end_greedy: 0.1
 decay_step_greedy: 20000
-sync_frequency: 50
-training_frequency: 1
+sync_frequency: 100
+training_frequency: 4
 running_steps: 500000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
+PER_alpha: 0.5
+PER_beta0: 0.4
+
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/dueldqn/"
-model_dir: "./models/dueldqn/"
+log_dir: "./logs/perdqn/"
+model_dir: "./models/perdqn/"
```

### Comparing `xuance-1.0.9/xuance/configs/dueldqn/classic_control/Acrobot-v1.yaml` & `xuance-1.1.0/xuance/configs/dueldqn/classic_control/MountainCar-v0.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 agent: "Duel_DQN"
 env_name: "Classic Control"
-env_id: "Acrobot-v1"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
 policy: "Duel_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128, ]
 q_hidden_size: [128, ]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 10000
 batch_size: 256
-learning_rate: 0.001
+learning_rate: 0.0001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
 decay_step_greedy: 20000
 sync_frequency: 50
 training_frequency: 1
-running_steps: 500000
+running_steps: 300000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
```

### Comparing `xuance-1.0.9/xuance/configs/dueldqn/classic_control/CartPole-v1.yaml` & `xuance-1.1.0/xuance/configs/drqn/box2d/LunarLander-v2.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-agent: "Duel_DQN"
+agent: "DRQN"  # deep recurrent Q-networks
 env_name: "Classic Control"
-env_id: "CartPole-v1"
+env_id: "LunarLander-v2"
 vectorize: "Dummy_Gym"
-policy: "Duel_Q_network"
+policy: "DRQN_Policy"
 representation: "Basic_MLP"
 runner: "DRL"
+rnn: "LSTM"
 
-representation_hidden_size: [128, ]
-q_hidden_size: [128, ]
-activation: 'ReLU'
+representation_hidden_size: [128,]
+recurrent_hidden_size: 128
+recurrent_layer_N: 1
+dropout: 0
+activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 10000
-batch_size: 256
+n_size: 50  # memory size for each parallel
+batch_size: 8  # batch size for training
 learning_rate: 0.001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.01
-decay_step_greedy: 20000
+decay_step_greedy: 5000
 sync_frequency: 50
 training_frequency: 1
-running_steps: 500000
+running_steps: 300000
 start_training: 1000
+lookup_length: 50
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 1
-log_dir: "./logs/dueldqn/"
-model_dir: "./models/dueldqn/"
+test_episode: 3
+log_dir: "./logs/drqn/"
+model_dir: "./models/drqn/"
```

### Comparing `xuance-1.0.9/xuance/configs/dueldqn/classic_control/MountainCar-v0.yaml` & `xuance-1.1.0/xuance/configs/sac/classic_control/CartPole-v1.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-agent: "Duel_DQN"
+agent: "SACDIS"
 env_name: "Classic Control"
-env_id: "MountainCar-v0"
+env_id: "CartPole-v1"
 vectorize: "Dummy_Gym"
-policy: "Duel_Q_network"
+policy: "Discrete_SAC"
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [128, ]
-q_hidden_size: [128, ]
-activation: 'ReLU'
+representation_hidden_size: [128,]
+actor_hidden_size: [128,]
+critic_hidden_size: [128,]
+activation: "relu"
 
 seed: 1
 parallels: 10
-n_size: 10000
+n_size: 20000
 batch_size: 256
-learning_rate: 0.0001
-gamma: 0.99
+actor_learning_rate: 0.001
+critic_learning_rate: 0.01
+gamma: 0.98
+tau: 0.005
 
-start_greedy: 0.5
-end_greedy: 0.01
-decay_step_greedy: 20000
-sync_frequency: 50
-training_frequency: 1
-running_steps: 300000
-start_training: 1000
+start_noise: 0.25
+end_noise: 0.05
+training_frequency: 2
+running_steps: 500000
+start_training: 2000
+action_type: "DISCRETE"
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/dueldqn/"
-model_dir: "./models/dueldqn/"
+log_dir: "./logs/sac/"
+model_dir: "./models/sac/"
```

### Comparing `xuance-1.0.9/xuance/configs/iddpg/mpe/simple_adversary_v3.yaml` & `xuance-1.1.0/xuance/configs/iddpg/mpe/simple_push_v3.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 agent: "IDDPG"  # the learning algorithms_marl
 env_name: "mpe"
-env_id: "simple_adversary_v3"
+env_id: "simple_push_v3"
 continuous_action: True
 policy: "Independent_DDPG_Policy"
 representation: "Basic_Identical"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
 representation_hidden_size: [64, ]  # the units for each hidden layer
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 activation_action: 'sigmoid'
 
 seed: 1
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
```

### Comparing `xuance-1.0.9/xuance/configs/iddpg/mpe/simple_push_v3.yaml` & `xuance-1.1.0/xuance/configs/iddpg/mpe/simple_adversary_v3.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 agent: "IDDPG"  # the learning algorithms_marl
 env_name: "mpe"
-env_id: "simple_push_v3"
+env_id: "simple_adversary_v3"
 continuous_action: True
 policy: "Independent_DDPG_Policy"
 representation: "Basic_Identical"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
 representation_hidden_size: [64, ]  # the units for each hidden layer
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 activation_action: 'sigmoid'
 
 seed: 1
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
```

### Comparing `xuance-1.0.9/xuance/configs/iddpg/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/iddpg/mpe/simple_spread_v3.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 representation: "Basic_Identical"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
 representation_hidden_size: []  # the units for each hidden layer
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 activation_action: 'sigmoid'
 
 seed: 1
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
```

### Comparing `xuance-1.0.9/xuance/configs/ippo/football/3v1.yaml` & `xuance-1.1.0/xuance/configs/ippo/football/3v1.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 50
 n_size: 400
 n_epoch: 15
 n_minibatch: 2
 learning_rate: 5.0e-4
```

### Comparing `xuance-1.0.9/xuance/configs/ippo/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/ippo/mpe/simple_spread_v3.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 agent: "IPPO"
 env_name: "mpe"
 env_id: "simple_spread_v3"
-continuous_action: False
-policy: "Categorical_MAAC_Policy"
+continuous_action: True
+policy: "Gaussian_MAAC_Policy"
 representation: "Basic_MLP"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
 use_recurrent: False
 rnn:
 representation_hidden_size: [64, ]  # the units for each hidden layer
 gain: 0.01
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [256, ]
-activation: "ReLU"
+activation: "relu"
+activation_action: "sigmoid"
 
 seed: 1
 parallels: 128
 n_size: 3200
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007
```

### Comparing `xuance-1.0.9/xuance/configs/ippo/sc2/1c3s5z.yaml` & `xuance-1.1.0/xuance/configs/ippo/sc2/1c3s5z.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
```

### Comparing `xuance-1.0.9/xuance/configs/ippo/sc2/25m.yaml` & `xuance-1.1.0/xuance/configs/ippo/sc2/8m.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "IPPO"
 env_name: "StarCraft2"
-env_id: "25m"
+env_id: "8m"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: True
 
@@ -18,20 +18,20 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
-n_epoch: 10
+n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
@@ -51,14 +51,14 @@
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 5000000  # 5M
+running_steps: 1000000  # 1M
 training_frequency: 1
 
-eval_interval: 50000
+eval_interval: 10000
 test_episode: 16
 log_dir: "./logs/ippo/"
 model_dir: "./models/ippo/"
```

### Comparing `xuance-1.0.9/xuance/configs/ippo/sc2/2m_vs_1z.yaml` & `xuance-1.1.0/xuance/configs/ippo/sc2/2m_vs_1z.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
```

### Comparing `xuance-1.0.9/xuance/configs/ippo/sc2/2s3z.yaml` & `xuance-1.1.0/xuance/configs/ippo/sc2/3m.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "IPPO"
 env_name: "StarCraft2"
-env_id: "2s3z"
+env_id: "3m"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 
 # recurrent settings for Basic_RNN representation
@@ -17,15 +17,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
@@ -50,14 +50,14 @@
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 2000000
+running_steps: 1000000
 training_frequency: 1
 
-eval_interval: 20000
+eval_interval: 10000
 test_episode: 16
 log_dir: "./logs/ippo/"
 model_dir: "./models/ippo/"
```

### Comparing `xuance-1.0.9/xuance/configs/ippo/sc2/3m.yaml` & `xuance-1.1.0/xuance/configs/mappo/sc2/3m.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-agent: "IPPO"
+agent: "MAPPO"
 env_name: "StarCraft2"
 env_id: "3m"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
@@ -17,15 +17,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
@@ -37,15 +37,15 @@
 clip_range: 0.2
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99  # discount factor
 
 # tricks
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
-use_global_state: False  # if use global state to replace joint observations
+use_global_state: True  # if use global state to calculate values
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
 value_clip_range: 0.2
 use_value_norm: True  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
@@ -55,9 +55,9 @@
 
 start_training: 1
 running_steps: 1000000
 training_frequency: 1
 
 eval_interval: 10000
 test_episode: 16
-log_dir: "./logs/ippo/"
-model_dir: "./models/ippo/"
+log_dir: "./logs/mappo/"
+model_dir: "./models/mappo/"
```

### Comparing `xuance-1.0.9/xuance/configs/ippo/sc2/5m_vs_6m.yaml` & `xuance-1.1.0/xuance/configs/ippo/sc2/5m_vs_6m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
```

### Comparing `xuance-1.0.9/xuance/configs/ippo/sc2/8m.yaml` & `xuance-1.1.0/xuance/configs/ippo/sc2/8m_vs_9m.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "IPPO"
 env_name: "StarCraft2"
-env_id: "8m"
+env_id: "8m_vs_9m"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: True
 
@@ -18,47 +18,47 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
-clip_range: 0.2
+clip_range: 0.05
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99  # discount factor
 
 # tricks
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
 use_global_state: False  # if use global state to replace joint observations
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
-value_clip_range: 0.2
+value_clip_range: 0.05
 use_value_norm: True  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 1000000  # 1M
+running_steps: 10000000  # 10M
 training_frequency: 1
 
-eval_interval: 10000
+eval_interval: 100000
 test_episode: 16
 log_dir: "./logs/ippo/"
 model_dir: "./models/ippo/"
```

### Comparing `xuance-1.0.9/xuance/configs/ippo/sc2/8m_vs_9m.yaml` & `xuance-1.1.0/xuance/configs/ippo/sc2/corridor.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "IPPO"
 env_name: "StarCraft2"
-env_id: "8m_vs_9m"
+env_id: "corridor"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: True
 
@@ -18,39 +18,39 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
-n_epoch: 15
+n_epoch: 5
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
-clip_range: 0.05
+clip_range: 0.2
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99  # discount factor
 
 # tricks
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
 use_global_state: False  # if use global state to replace joint observations
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
-value_clip_range: 0.05
+value_clip_range: 0.2
 use_value_norm: True  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
```

### Comparing `xuance-1.0.9/xuance/configs/ippo/sc2/MMM2.yaml` & `xuance-1.1.0/xuance/configs/mappo/sc2/MMM2.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-agent: "IPPO"
+agent: "MAPPO"
 env_name: "StarCraft2"
 env_id: "MMM2"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
@@ -18,15 +18,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 1.0
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
 n_epoch: 5
 n_minibatch: 2
 learning_rate: 0.0007  # 7e-4
@@ -38,15 +38,15 @@
 clip_range: 0.2
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99  # discount factor
 
 # tricks
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
-use_global_state: False  # if use global state to replace joint observations
+use_global_state: True  # if use global state to calculate values
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
 value_clip_range: 0.2
 use_value_norm: True  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
@@ -56,9 +56,9 @@
 
 start_training: 1
 running_steps: 10000000  # 10M
 training_frequency: 1
 
 eval_interval: 100000
 test_episode: 16
-log_dir: "./logs/ippo/"
-model_dir: "./models/ippo/"
+log_dir: "./logs/mappo/"
+model_dir: "./models/mappo/"
```

### Comparing `xuance-1.0.9/xuance/configs/ippo/sc2/corridor.yaml` & `xuance-1.1.0/xuance/configs/mappo/sc2/corridor.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-agent: "IPPO"
+agent: "MAPPO"
 env_name: "StarCraft2"
 env_id: "corridor"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
@@ -18,15 +18,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
 n_epoch: 5
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
@@ -38,15 +38,15 @@
 clip_range: 0.2
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99  # discount factor
 
 # tricks
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
-use_global_state: False  # if use global state to replace joint observations
+use_global_state: True  # if use global state to calculate values
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
 value_clip_range: 0.2
 use_value_norm: True  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
@@ -56,9 +56,9 @@
 
 start_training: 1
 running_steps: 10000000  # 10M
 training_frequency: 1
 
 eval_interval: 100000
 test_episode: 16
-log_dir: "./logs/ippo/"
-model_dir: "./models/ippo/"
+log_dir: "./logs/mappo/"
+model_dir: "./models/mappo/"
```

### Comparing `xuance-1.0.9/xuance/configs/iql/football/3v1.yaml` & `xuance-1.1.0/xuance/configs/iql/football/3v1.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 fc_hidden_sizes: [128, ]
 recurrent_hidden_size: 128
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [128, ]
 q_hidden_size: [128, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 50
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
```

### Comparing `xuance-1.0.9/xuance/configs/iql/magent2/adversarial_pursuit_v4.yaml` & `xuance-1.1.0/xuance/configs/iql/magent2/adversarial_pursuit_v4.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 on_policy: False
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: False
 rnn:
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 10
 buffer_size: 20000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.95  # discount factor
```

### Comparing `xuance-1.0.9/xuance/configs/iql/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/iql/mpe/simple_spread_v3.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
 use_recurrent: False
 rnn:
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99  # discount factor
```

### Comparing `xuance-1.0.9/xuance/configs/iql/sc2/1c3s5z.yaml` & `xuance-1.1.0/xuance/configs/iql/sc2/1c3s5z.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
```

### Comparing `xuance-1.0.9/xuance/configs/iql/sc2/25m.yaml` & `xuance-1.1.0/xuance/configs/iql/sc2/25m.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
```

### Comparing `xuance-1.0.9/xuance/configs/iql/sc2/2m_vs_1z.yaml` & `xuance-1.1.0/xuance/configs/iql/sc2/3m.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 agent: "IQL"  # the learning algorithms_marl
-global_state: False
 env_name: "StarCraft2"
-env_id: "2m_vs_1z"
+env_id: "3m"
 fps: 15
 policy: "Basic_Q_network_marl"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -16,15 +15,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
```

### Comparing `xuance-1.0.9/xuance/configs/iql/sc2/2s3z.yaml` & `xuance-1.1.0/xuance/configs/iql/sc2/2s3z.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
```

### Comparing `xuance-1.0.9/xuance/configs/iql/sc2/3m.yaml` & `xuance-1.1.0/xuance/configs/iql/sc2/2m_vs_1z.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 agent: "IQL"  # the learning algorithms_marl
+global_state: False
 env_name: "StarCraft2"
-env_id: "3m"
+env_id: "2m_vs_1z"
 fps: 15
 policy: "Basic_Q_network_marl"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -15,15 +16,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
```

### Comparing `xuance-1.0.9/xuance/configs/iql/sc2/5m_vs_6m.yaml` & `xuance-1.1.0/xuance/configs/vdn/sc2/5m_vs_6m.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-agent: "IQL"  # the learning algorithms_marl
+agent: "VDN"  # the learning algorithms_marl
+global_state: False
 env_name: "StarCraft2"
 env_id: "5m_vs_6m"
 fps: 15
-policy: "Basic_Q_network_marl"
+policy: "Mixing_Q_network"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
@@ -15,15 +16,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
@@ -39,9 +40,9 @@
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
 eval_interval: 100000
 test_episode: 16
-log_dir: "./logs/iql/"
-model_dir: "./models/iql/"
+log_dir: "./logs/vdn/"
+model_dir: "./models/vdn/"
```

### Comparing `xuance-1.0.9/xuance/configs/iql/sc2/8m.yaml` & `xuance-1.1.0/xuance/configs/vdn/sc2/25m.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-agent: "IQL"  # the learning algorithms_marl
+agent: "VDN"  # the learning algorithms_marl
+global_state: False
 env_name: "StarCraft2"
-env_id: "8m"
+env_id: "25m"
 fps: 15
-policy: "Basic_Q_network_marl"
+policy: "Mixing_Q_network"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
@@ -15,33 +16,33 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
 decay_step_greedy: 50000
 start_training: 1000  # start training after n episodes
-running_steps: 1000000  # 1M
+running_steps: 5000000  # 5M
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 10000
+eval_interval: 50000
 test_episode: 16
-log_dir: "./logs/iql/"
-model_dir: "./models/iql/"
+log_dir: "./logs/vdn/"
+model_dir: "./models/vdn/"
```

### Comparing `xuance-1.0.9/xuance/configs/iql/sc2/8m_vs_9m.yaml` & `xuance-1.1.0/xuance/configs/vdn/sc2/8m_vs_9m.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-agent: "IQL"  # the learning algorithms_marl
+agent: "VDN"  # the learning algorithms_marl
+global_state: False
 env_name: "StarCraft2"
 env_id: "8m_vs_9m"
 fps: 15
-policy: "Basic_Q_network_marl"
+policy: "Mixing_Q_network"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
@@ -15,15 +16,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
@@ -39,9 +40,9 @@
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
 eval_interval: 100000
 test_episode: 16
-log_dir: "./logs/iql/"
-model_dir: "./models/iql/"
+log_dir: "./logs/vdn/"
+model_dir: "./models/vdn/"
```

### Comparing `xuance-1.0.9/xuance/configs/iql/sc2/MMM2.yaml` & `xuance-1.1.0/xuance/configs/vdn/sc2/2m_vs_1z.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-agent: "IQL"  # the learning algorithms_marl
+agent: "VDN"  # the learning algorithms_marl
+global_state: False
 env_name: "StarCraft2"
-env_id: "MMM2"
+env_id: "2m_vs_1z"
 fps: 15
-policy: "Basic_Q_network_marl"
+policy: "Mixing_Q_network"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
@@ -15,33 +16,33 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
 decay_step_greedy: 50000
 start_training: 1000  # start training after n episodes
-running_steps: 10000000  # 10M
+running_steps: 1000000  # 1M
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 100000
+eval_interval: 10000
 test_episode: 16
-log_dir: "./logs/iql/"
-model_dir: "./models/iql/"
+log_dir: "./logs/vdn/"
+model_dir: "./models/vdn/"
```

### Comparing `xuance-1.0.9/xuance/configs/iql/sc2/corridor.yaml` & `xuance-1.1.0/xuance/configs/iql/sc2/8m_vs_9m.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "IQL"  # the learning algorithms_marl
 env_name: "StarCraft2"
-env_id: "corridor"
+env_id: "8m_vs_9m"
 fps: 15
 policy: "Basic_Q_network_marl"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -15,15 +15,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
```

### Comparing `xuance-1.0.9/xuance/configs/isac/mpe/simple_adversary_v3.yaml` & `xuance-1.1.0/xuance/configs/masac/mpe/simple_adversary_v3.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-agent: "ISAC"  # the learning algorithms_marl
+agent: "MASAC"  # the learning algorithms_marl
 env_name: "mpe"
 env_id: "simple_adversary_v3"
 continuous_action: True
-policy: "Gaussian_ISAC_Policy"
+policy: "Gaussian_MASAC_Policy"
 representation: "Basic_Identical"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
-representation_hidden_size: [64, ]  # the units for each hidden layer
+representation_hidden_size: []  # the units for each hidden layer
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 activation_action: 'sigmoid'
 
 seed: 1
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
@@ -32,9 +32,9 @@
 training_frequency: 1
 
 use_grad_clip: True
 grad_clip_norm: 0.5
 
 eval_interval: 100000
 test_episode: 5
-log_dir: "./logs/isac/"
-model_dir: "./models/isac/"
+log_dir: "./logs/masac/"
+model_dir: "./models/masac/"
```

### Comparing `xuance-1.0.9/xuance/configs/isac/mpe/simple_push_v3.yaml` & `xuance-1.1.0/xuance/configs/masac/mpe/simple_push_v3.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-agent: "ISAC"  # the learning algorithms_marl
+agent: "MASAC"  # the learning algorithms_marl
 env_name: "mpe"
 env_id: "simple_push_v3"
 continuous_action: True
-policy: "Gaussian_ISAC_Policy"
+policy: "Gaussian_MASAC_Policy"
 representation: "Basic_Identical"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
-representation_hidden_size: [64, ]  # the units for each hidden layer
+representation_hidden_size: []  # the units for each hidden layer
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 activation_action: 'sigmoid'
 
 seed: 1
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
@@ -32,9 +32,9 @@
 training_frequency: 1
 
 use_grad_clip: True
 grad_clip_norm: 0.5
 
 eval_interval: 100000
 test_episode: 5
-log_dir: "./logs/isac/"
-model_dir: "./models/isac/"
+log_dir: "./logs/masac/"
+model_dir: "./models/masac/"
```

### Comparing `xuance-1.0.9/xuance/configs/isac/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/isac/mpe/simple_adversary_v3.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 agent: "ISAC"  # the learning algorithms_marl
 env_name: "mpe"
-env_id: "simple_spread_v3"
+env_id: "simple_adversary_v3"
 continuous_action: True
 policy: "Gaussian_ISAC_Policy"
 representation: "Basic_Identical"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
-representation_hidden_size: [64, ]  # the units for each hidden layer
+representation_hidden_size: []  # the units for each hidden layer
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 activation_action: 'sigmoid'
 
 seed: 1
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
```

### Comparing `xuance-1.0.9/xuance/configs/maddpg/mpe/simple_adversary_v3.yaml` & `xuance-1.1.0/xuance/configs/maddpg/mpe/simple_adversary_v3.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 on_policy: False
 
 representation_hidden_size: []  # the units for each hidden layer
 actor_hidden_size: [64, ]
 critic_hidden_size: [64, ]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 activation_action: 'sigmoid'
 
 seed: 1
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
```

### Comparing `xuance-1.0.9/xuance/configs/maddpg/mpe/simple_push_v3.yaml` & `xuance-1.1.0/xuance/configs/maddpg/mpe/simple_push_v3.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 representation: "Basic_Identical"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
 representation_hidden_size: []  # the units for each hidden layer
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 activation_action: 'sigmoid'
 
 seed: 1
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
```

### Comparing `xuance-1.0.9/xuance/configs/maddpg/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/maddpg/mpe/simple_spread_v3.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 representation: "Basic_Identical"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
 representation_hidden_size: []  # the units for each hidden layer
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 activation_action: 'sigmoid'
 
 seed: 1
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
```

### Comparing `xuance-1.0.9/xuance/configs/mappo/football/1v1.yaml` & `xuance-1.1.0/xuance/configs/mappo/football/3v1.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 agent: "MAPPO"  # the learning algorithms_marl
 global_state: True
 # environment settings
 env_name: "Football"
-scenario: "1_vs_1_easy"
+scenario: "academy_3_vs_1_with_keeper"
 use_stacked_frames: False  # Whether to use stacked_frames
-num_agent: 1
+num_agent: 3
 num_adversary: 0
 obs_type: "simple115v2"  # representation used to build the observation, choices: ["simple115v2", "extracted", "pixels_gray", "pixels"]
 rewards_type: "scoring,checkpoints"  # comma separated list of rewards to be added
 smm_width: 96  # width of super minimap
 smm_height: 72  # height of super minimap
 fps: 15
 policy: "Categorical_MAAC_Policy"
@@ -26,21 +26,21 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 50
-n_size: 100
-n_epoch: 10
-n_minibatch: 1
+n_size: 400
+n_epoch: 15
+n_minibatch: 2
 learning_rate: 5.0e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 clip_range: 0.2
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
```

### Comparing `xuance-1.0.9/xuance/configs/mappo/football/3v1.yaml` & `xuance-1.1.0/xuance/configs/mappo/football/1v1.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 agent: "MAPPO"  # the learning algorithms_marl
 global_state: True
 # environment settings
 env_name: "Football"
-scenario: "academy_3_vs_1_with_keeper"
+scenario: "1_vs_1_easy"
 use_stacked_frames: False  # Whether to use stacked_frames
-num_agent: 3
+num_agent: 1
 num_adversary: 0
 obs_type: "simple115v2"  # representation used to build the observation, choices: ["simple115v2", "extracted", "pixels_gray", "pixels"]
 rewards_type: "scoring,checkpoints"  # comma separated list of rewards to be added
 smm_width: 96  # width of super minimap
 smm_height: 72  # height of super minimap
 fps: 15
 policy: "Categorical_MAAC_Policy"
@@ -26,21 +26,21 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 50
-n_size: 400
-n_epoch: 15
-n_minibatch: 2
+n_size: 100
+n_epoch: 10
+n_minibatch: 1
 learning_rate: 5.0e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 clip_range: 0.2
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
```

### Comparing `xuance-1.0.9/xuance/configs/mappo/mpe/simple_adversary_v3.yaml` & `xuance-1.1.0/xuance/configs/mappo/mpe/simple_push_v3.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 agent: "MAPPO"
 env_name: "mpe"
-env_id: "simple_adversary_v3"
+env_id: "simple_push_v3"
 continuous_action: True
 policy: "Gaussian_MAAC_Policy"
 representation: "Basic_MLP"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: False
 rnn:
 representation_hidden_size: [64, ]  # the units for each hidden layer
 gain: 0.01
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [256, ]
-activation: "ReLU"
+activation: "relu"
+activation_action: "sigmoid"
 
 seed: 1
 parallels: 128
 n_size: 3200
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007
```

### Comparing `xuance-1.0.9/xuance/configs/mappo/mpe/simple_push_v3.yaml` & `xuance-1.1.0/xuance/configs/mappo/mpe/simple_adversary_v3.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 agent: "MAPPO"
 env_name: "mpe"
-env_id: "simple_push_v3"
+env_id: "simple_adversary_v3"
 continuous_action: True
 policy: "Gaussian_MAAC_Policy"
 representation: "Basic_MLP"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: False
 rnn:
 representation_hidden_size: [64, ]  # the units for each hidden layer
 gain: 0.01
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [256, ]
-activation: "ReLU"
+activation: "relu"
+activation_action: "sigmoid"
 
 seed: 1
 parallels: 128
 n_size: 3200
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007
```

### Comparing `xuance-1.0.9/xuance/configs/mappo/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/mappo/mpe/simple_spread_v3.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 use_recurrent: False
 rnn:
 representation_hidden_size: [64, ]  # the units for each hidden layer
 gain: 0.01
 
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: "ReLU"
+activation: "relu"
+activation_action: "sigmoid"
 
 seed: 1
 parallels: 8  # 128
 n_size: 3200
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007
```

### Comparing `xuance-1.0.9/xuance/configs/mappo/sc2/1c3s5z.yaml` & `xuance-1.1.0/xuance/configs/mappo/sc2/1c3s5z.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
```

### Comparing `xuance-1.0.9/xuance/configs/mappo/sc2/25m.yaml` & `xuance-1.1.0/xuance/configs/mappo/sc2/25m.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
```

### Comparing `xuance-1.0.9/xuance/configs/mappo/sc2/2m_vs_1z.yaml` & `xuance-1.1.0/xuance/configs/mappo/sc2/2m_vs_1z.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
```

### Comparing `xuance-1.0.9/xuance/configs/mappo/sc2/2s3z.yaml` & `xuance-1.1.0/xuance/configs/ippo/sc2/25m.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-agent: "MAPPO"
+agent: "IPPO"
 env_name: "StarCraft2"
-env_id: "2s3z"
+env_id: "25m"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
+on_policy: True
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
 rnn: "GRU"
 recurrent_layer_N: 1
 fc_hidden_sizes: [64, 64, 64]
 recurrent_hidden_size: 64
@@ -17,47 +18,47 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
-n_epoch: 15
+n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
 clip_range: 0.2
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99  # discount factor
 
 # tricks
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
-use_global_state: True  # if use global state to calculate values
+use_global_state: False  # if use global state to replace joint observations
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
 value_clip_range: 0.2
 use_value_norm: True  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 2000000
+running_steps: 5000000  # 5M
 training_frequency: 1
 
-eval_interval: 20000
+eval_interval: 50000
 test_episode: 16
-log_dir: "./logs/mappo/"
-model_dir: "./models/mappo/"
+log_dir: "./logs/ippo/"
+model_dir: "./models/ippo/"
```

### Comparing `xuance-1.0.9/xuance/configs/mappo/sc2/3m.yaml` & `xuance-1.1.0/xuance/configs/mappo/sc2/2s3z.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "MAPPO"
 env_name: "StarCraft2"
-env_id: "3m"
+env_id: "2s3z"
 fps: 15
 policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 
 # recurrent settings for Basic_RNN representation
@@ -17,15 +17,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
@@ -50,14 +50,14 @@
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 1000000
+running_steps: 2000000
 training_frequency: 1
 
-eval_interval: 10000
+eval_interval: 20000
 test_episode: 16
 log_dir: "./logs/mappo/"
 model_dir: "./models/mappo/"
```

### Comparing `xuance-1.0.9/xuance/configs/mappo/sc2/5m_vs_6m.yaml` & `xuance-1.1.0/xuance/configs/mappo/sc2/5m_vs_6m.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
 n_epoch: 10
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
```

### Comparing `xuance-1.0.9/xuance/configs/mappo/sc2/8m.yaml` & `xuance-1.1.0/xuance/configs/mappo/sc2/8m.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
```

### Comparing `xuance-1.0.9/xuance/configs/mappo/sc2/8m_vs_9m.yaml` & `xuance-1.1.0/xuance/configs/mappo/sc2/8m_vs_9m.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 n_size: 128
 n_epoch: 15
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
```

### Comparing `xuance-1.0.9/xuance/configs/mappo/sc2/MMM2.yaml` & `xuance-1.1.0/xuance/configs/vdac/sc2/8m.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,68 @@
-agent: "MAPPO"
+agent: "VDAC"
 env_name: "StarCraft2"
-env_id: "MMM2"
+env_id: "8m"
 fps: 15
-policy: "Categorical_MAAC_Policy"
+policy: "Categorical_MAAC_Policy_Share"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: True
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
 rnn: "GRU"
 recurrent_layer_N: 1
-fc_hidden_sizes: [64, 64, 64]
+fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
-gain: 1.0
+gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
+
+mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
+hidden_dim_mixing_net: 32  # hidden units of mixing network
+hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
-n_size: 128
-n_epoch: 5
-n_minibatch: 2
+n_size: 8
+n_epoch: 1
+n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
 clip_range: 0.2
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99  # discount factor
 
 # tricks
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
-use_global_state: True  # if use global state to calculate values
+use_global_state: False  # if use global state to replace joint observations
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
 value_clip_range: 0.2
 use_value_norm: True  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 10000000  # 10M
+running_steps: 1000000  # 1M
 training_frequency: 1
 
-eval_interval: 100000
+eval_interval: 5000
 test_episode: 16
-log_dir: "./logs/mappo/"
-model_dir: "./models/mappo/"
+log_dir: "./logs/vdac/"
+model_dir: "./models/vdac/"
```

### Comparing `xuance-1.0.9/xuance/configs/mappo/sc2/corridor.yaml` & `xuance-1.1.0/xuance/configs/vdac/sc2/corridor.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,56 @@
-agent: "MAPPO"
+agent: "VDAC"
 env_name: "StarCraft2"
 env_id: "corridor"
 fps: 15
-policy: "Categorical_MAAC_Policy"
+policy: "Categorical_MAAC_Policy_Share"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: True
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
 rnn: "GRU"
 recurrent_layer_N: 1
-fc_hidden_sizes: [64, 64, 64]
+fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
+
+mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
+hidden_dim_mixing_net: 32  # hidden units of mixing network
+hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
-n_size: 128
-n_epoch: 5
+n_size: 8
+n_epoch: 1
 n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
 clip_range: 0.2
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99  # discount factor
 
 # tricks
 use_linear_lr_decay: False  # if use linear learning rate decay
 end_factor_lr_decay: 0.5
-use_global_state: True  # if use global state to calculate values
+use_global_state: False  # if use global state to replace joint observations
 use_grad_norm: True  # gradient normalization
 max_grad_norm: 10.0
 use_value_clip: True  # limit the value range
 value_clip_range: 0.2
 use_value_norm: True  # use running mean and std to normalize rewards.
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
@@ -54,11 +58,11 @@
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
 running_steps: 10000000  # 10M
 training_frequency: 1
 
-eval_interval: 100000
+eval_interval: 50000
 test_episode: 16
-log_dir: "./logs/mappo/"
-model_dir: "./models/mappo/"
+log_dir: "./logs/vdac/"
+model_dir: "./models/vdac/"
```

### Comparing `xuance-1.0.9/xuance/configs/masac/mpe/simple_adversary_v3.yaml` & `xuance-1.1.0/xuance/configs/masac/mpe/simple_spread_v3.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 agent: "MASAC"  # the learning algorithms_marl
 env_name: "mpe"
-env_id: "simple_adversary_v3"
+env_id: "simple_spread_v3"
 continuous_action: True
 policy: "Gaussian_MASAC_Policy"
 representation: "Basic_Identical"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
-representation_hidden_size: [64, ]  # the units for each hidden layer
+representation_hidden_size: []  # the units for each hidden layer
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 activation_action: 'sigmoid'
 
 seed: 1
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
@@ -34,7 +34,8 @@
 use_grad_clip: True
 grad_clip_norm: 0.5
 
 eval_interval: 100000
 test_episode: 5
 log_dir: "./logs/masac/"
 model_dir: "./models/masac/"
+
```

### Comparing `xuance-1.0.9/xuance/configs/masac/mpe/simple_push_v3.yaml` & `xuance-1.1.0/xuance/configs/matd3/mpe/simple_spread_v3.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-agent: "MASAC"  # the learning algorithms_marl
+agent: "MATD3"  # the learning algorithms_marl
 env_name: "mpe"
-env_id: "simple_push_v3"
+env_id: "simple_spread_v3"
 continuous_action: True
-policy: "Gaussian_MASAC_Policy"
+policy: "MATD3_Policy"
 representation: "Basic_Identical"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
-representation_hidden_size: [64, ]  # the units for each hidden layer
+representation_hidden_size: []  # the units for each hidden layer
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 activation_action: 'sigmoid'
 
 seed: 1
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
 lr_c: 0.001  # learning rate for critic
 gamma: 0.95  # discount factor
 tau: 0.001  # soft update for target networks
-alpha: 0.01
 
 start_noise: 1.0
 end_noise: 0.01
-sigma: 0.1  # random noise for continuous actions
+sigma: 0.1
 start_training: 1000  # start training after n episodes
 running_steps: 10000000
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
 
 use_grad_clip: True
 grad_clip_norm: 0.5
 
 eval_interval: 100000
 test_episode: 5
-log_dir: "./logs/masac/"
-model_dir: "./models/masac/"
+log_dir: "./logs/matd3/"
+model_dir: "./models/matd3/"
```

### Comparing `xuance-1.0.9/xuance/configs/masac/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/matd3/mpe/simple_push_v3.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-agent: "MASAC"  # the learning algorithms_marl
+agent: "MATD3"  # the learning algorithms_marl
 env_name: "mpe"
-env_id: "simple_spread_v3"
+env_id: "simple_push_v3"
 continuous_action: True
-policy: "Gaussian_MASAC_Policy"
+policy: "MATD3_Policy"
 representation: "Basic_Identical"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
-representation_hidden_size: [64, ]  # the units for each hidden layer
+representation_hidden_size: []  # the units for each hidden layer
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 activation_action: 'sigmoid'
 
 seed: 1
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
 lr_c: 0.001  # learning rate for critic
 gamma: 0.95  # discount factor
 tau: 0.001  # soft update for target networks
-alpha: 0.01
 
 start_noise: 1.0
 end_noise: 0.01
-sigma: 0.1  # random noise for continuous actions
+sigma: 0.1
 start_training: 1000  # start training after n episodes
 running_steps: 10000000
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
 
 use_grad_clip: True
 grad_clip_norm: 0.5
 
 eval_interval: 100000
 test_episode: 5
-log_dir: "./logs/masac/"
-model_dir: "./models/masac/"
-
+log_dir: "./logs/matd3/"
+model_dir: "./models/matd3/"
```

### Comparing `xuance-1.0.9/xuance/configs/matd3/mpe/simple_adversary_v3.yaml` & `xuance-1.1.0/xuance/configs/matd3/mpe/simple_adversary_v3.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 env_id: "simple_adversary_v3"
 continuous_action: True
 policy: "MATD3_Policy"
 representation: "Basic_Identical"
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
-representation_hidden_size: [64, ]  # the units for each hidden layer
+representation_hidden_size: []  # the units for each hidden layer
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 activation_action: 'sigmoid'
 
 seed: 1
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 lr_a: 0.01  # learning rate for actor
```

### Comparing `xuance-1.0.9/xuance/configs/matd3/mpe/simple_push_v3.yaml` & `xuance-1.1.0/xuance/configs/maddpg/new_env_mas.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-agent: "MATD3"  # the learning algorithms_marl
-env_name: "mpe"
-env_id: "simple_push_v3"
+agent: "MADDPG"  # the learning algorithms_marl
+env_name: "NewEnv_MAS"
+env_id: "scenarios_0"
+max_episode_steps: 200
+render: False
+sleep: 0.01
 continuous_action: True
-policy: "MATD3_Policy"
+policy: "MADDPG_Policy"
 representation: "Basic_Identical"
-vectorize: "Dummy_Pettingzoo"
-runner: "Pettingzoo_Runner"
+vectorize: "Dummy_NewEnv_MAS"
+runner: "MARL"
+on_policy: False
 
-representation_hidden_size: [64, ]  # the units for each hidden layer
 actor_hidden_size: [64, 64]
 critic_hidden_size: [64, 64]
-activation: 'LeakyReLU'
-activation_action: 'sigmoid'
+activation: 'leaky_relu'
+activation_action: 'tanh'
 
 seed: 1
 parallels: 16
-buffer_size: 100000
-batch_size: 256
-lr_a: 0.01  # learning rate for actor
+buffer_size: 1000000
+batch_size: 1024
+lr_a: 0.001  # learning rate for actor
 lr_c: 0.001  # learning rate for critic
-gamma: 0.95  # discount factor
-tau: 0.001  # soft update for target networks
+gamma: 0.99  # discount factor
+tau: 0.005  # soft update for target networks
 
-start_noise: 1.0
-end_noise: 0.01
+start_noise: 0.1
+end_noise: 0.1
 sigma: 0.1
-start_training: 1000  # start training after n episodes
-running_steps: 10000000
-train_per_step: False  # True: train model per step; False: train model per episode.
+start_training: 2000  # start training after n episodes
+running_steps: 1000000
+train_per_step: True  # True: train model per step; False: train model per episode.
 training_frequency: 1
 
 use_grad_clip: True
 grad_clip_norm: 0.5
 
-eval_interval: 100000
+eval_interval: 10000
 test_episode: 5
-log_dir: "./logs/matd3/"
-model_dir: "./models/matd3/"
+log_dir: "./logs/maddpg/"
+model_dir: "./models/maddpg/"
```

### Comparing `xuance-1.0.9/xuance/configs/matd3/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/vdn/sc2/corridor.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,48 @@
-agent: "MATD3"  # the learning algorithms_marl
-env_name: "mpe"
-env_id: "simple_spread_v3"
-continuous_action: True
-policy: "MATD3_Policy"
-representation: "Basic_Identical"
-vectorize: "Dummy_Pettingzoo"
-runner: "Pettingzoo_Runner"
-
-representation_hidden_size: [64, ]  # the units for each hidden layer
-actor_hidden_size: [64, 64]
-critic_hidden_size: [64, 64]
-activation: 'LeakyReLU'
-activation_action: 'sigmoid'
+agent: "VDN"  # the learning algorithms_marl
+global_state: False
+env_name: "StarCraft2"
+env_id: "corridor"
+fps: 15
+policy: "Mixing_Q_network"
+representation: "Basic_RNN"
+vectorize: "Subproc_StarCraft2"
+runner: "StarCraft2_Runner"
+on_policy: False
+
+# recurrent settings for Basic_RNN representation
+use_recurrent: True
+rnn: "GRU"
+recurrent_layer_N: 1
+fc_hidden_sizes: [64, ]
+recurrent_hidden_size: 64
+N_recurrent_layers: 1
+dropout: 0
+
+representation_hidden_size: [64, ]
+q_hidden_size: [64, ]  # the units for each hidden layer
+activation: "relu"
 
 seed: 1
-parallels: 16
-buffer_size: 100000
-batch_size: 256
-lr_a: 0.01  # learning rate for actor
-lr_c: 0.001  # learning rate for critic
-gamma: 0.95  # discount factor
-tau: 0.001  # soft update for target networks
-
-start_noise: 1.0
-end_noise: 0.01
-sigma: 0.1
+parallels: 8
+buffer_size: 5000
+batch_size: 32
+learning_rate: 0.0007
+gamma: 0.99  # discount factor
+double_q: True  # use double q learning
+
+start_greedy: 1.0
+end_greedy: 0.05
+decay_step_greedy: 50000
 start_training: 1000  # start training after n episodes
-running_steps: 10000000
+running_steps: 10000000  # 10M
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
+sync_frequency: 200
 
-use_grad_clip: True
+use_grad_clip: False
 grad_clip_norm: 0.5
 
 eval_interval: 100000
-test_episode: 5
-log_dir: "./logs/matd3/"
-model_dir: "./models/matd3/"
+test_episode: 16
+log_dir: "./logs/vdn/"
+model_dir: "./models/vdn/"
```

### Comparing `xuance-1.0.9/xuance/configs/mfac/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/mfac/mpe/simple_spread_v3.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 use_recurrent: False
 rnn:
 representation_hidden_size: [64, ]  # the units for each hidden layer
 gain: 0.01
 
 actor_hidden_size: [128, ]
 critic_hidden_size: [128, ]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 activation_action: 'sigmoid'
 
 seed: 1
 parallels: 128
 buffer_size: 3200
 n_epoch: 10
 n_minibatch: 1
```

### Comparing `xuance-1.0.9/xuance/configs/mfq/magent2/adversarial_pursuit_v4.yaml` & `xuance-1.1.0/xuance/configs/mfq/magent2/adversarial_pursuit_v4.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 recurrent_layer_N: 1
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 
 representation_hidden_size: [512, ]  # the units for each hidden layer
 q_hidden_size: [512, ]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 10
 buffer_size: 2000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.95  # discount factor
```

### Comparing `xuance-1.0.9/xuance/configs/mfq/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/mfq/mpe/simple_spread_v3.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
 use_recurrent: False
 rnn:
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 16
 buffer_size: 200000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.95  # discount factor
```

### Comparing `xuance-1.0.9/xuance/configs/mpdqn/Platform.yaml` & `xuance-1.1.0/xuance/configs/mpdqn/Platform.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 policy: "MPDQN_Policy"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 conactor_hidden_size: [128,]
 qnetwork_hidden_size: [128, ]
-activation: "ReLU"
+activation: "relu"
+activation_action: 'tanh'
 
 n_size: 20000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 tau: 0.005
```

### Comparing `xuance-1.0.9/xuance/configs/noisydqn/atari.yaml` & `xuance-1.1.0/xuance/configs/noisydqn/atari.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [32, 64, 64]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512, ]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1069
 parallels: 5
 n_size: 100000
 batch_size: 32  # 64
 learning_rate: 0.0001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/noisydqn/box2d/CarRacing-v2.yaml` & `xuance-1.1.0/xuance/configs/noisydqn/box2d/CarRacing-v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [16, 16, 32]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 2
 n_size: 10000
 batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/noisydqn/box2d/LunarLander-v2.yaml` & `xuance-1.1.0/xuance/configs/noisydqn/box2d/LunarLander-v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 vectorize: "Dummy_Gym"
 policy: "Noisy_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 20000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/noisydqn/classic_control/Acrobot-v1.yaml` & `xuance-1.1.0/xuance/configs/noisydqn/classic_control/Acrobot-v1.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 vectorize: "Dummy_Gym"
 policy: "Noisy_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 20000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/noisydqn/classic_control/CartPole-v1.yaml` & `xuance-1.1.0/xuance/configs/noisydqn/classic_control/CartPole-v1.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 vectorize: "Dummy_Gym"
 policy: "Noisy_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 20000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/noisydqn/classic_control/MountainCar-v0.yaml` & `xuance-1.1.0/xuance/configs/noisydqn/classic_control/MountainCar-v0.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 vectorize: "Dummy_Gym"
 policy: "Noisy_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 20000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/pdqn/Platform.yaml` & `xuance-1.1.0/xuance/configs/pdqn/Platform.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 policy: "PDQN_Policy"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 conactor_hidden_size: [128,]
 qnetwork_hidden_size: [128, ]
-activation: "ReLU"
+activation: "relu"
+activation_action: 'tanh'
 
 n_size: 20000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 tau: 0.005
```

### Comparing `xuance-1.0.9/xuance/configs/perdqn/atari.yaml` & `xuance-1.1.0/xuance/configs/ddqn/atari.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-agent: "PerDQN"
+agent: "DDQN"
 vectorize: "Dummy_Atari"
 env_name: "Atari"
 env_id: "ALE/Breakout-v5"
 obs_type: "grayscale"  # choice for Atari env: ram, rgb, grayscale
 img_size: [84, 84]  # default is 210 x 160 in gym[Atari]
 num_stack: 4  # frame stack trick
 frame_skip: 4  # frame skip trick
@@ -13,20 +13,20 @@
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [32, 64, 64]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512, ]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1069
 parallels: 5
 n_size: 100000
-batch_size: 32  # 64
+batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
 
 start_greedy: 0.5
 end_greedy: 0.05
 decay_step_greedy: 1000000  # 1M
 sync_frequency: 500
@@ -35,15 +35,12 @@
 start_training: 10000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
-PER_alpha: 0.5
-PER_beta0: 0.4
-
 test_steps: 10000
 eval_interval: 500000
-test_episode: 1
-log_dir: "./logs/perdqn/"
-model_dir: "./models/perdqn/"
+test_episode: 3
+log_dir: "./logs/ddqn/"
+model_dir: "./models/ddqn/"
```

### Comparing `xuance-1.0.9/xuance/configs/perdqn/box2d/CarRacing-v2.yaml` & `xuance-1.1.0/xuance/configs/perdqn/box2d/CarRacing-v2.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [16, 16, 32]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 2
 n_size: 10000
 batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/perdqn/box2d/LunarLander-v2.yaml` & `xuance-1.1.0/xuance/configs/perdqn/classic_control/CartPole-v1.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 agent: "PerDQN"
 env_name: "Classic Control"
-env_id: "LunarLander-v2"
+env_id: "CartPole-v1"
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 20000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/perdqn/classic_control/Acrobot-v1.yaml` & `xuance-1.1.0/xuance/configs/perdqn/classic_control/MountainCar-v1.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 agent: "PerDQN"
 env_name: "Classic Control"
-env_id: "Acrobot-v1"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 20000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/perdqn/classic_control/CartPole-v1.yaml` & `xuance-1.1.0/xuance/configs/qrdqn/classic_control/MountainCar-v0.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-agent: "PerDQN"
+agent: "QRDQN"
 env_name: "Classic Control"
-env_id: "CartPole-v1"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
-policy: "Basic_Q_network"
+policy: "QR_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 20000
-batch_size: 128
+batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
+quantile_num: 20
 
-start_greedy: 0.5
-end_greedy: 0.1
-decay_step_greedy: 20000
+start_greedy: 0.25
+end_greedy: 0.01
+decay_step_greedy: 30000
 sync_frequency: 100
-training_frequency: 4
-running_steps: 500000
+training_frequency: 1
+running_steps: 300000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
-PER_alpha: 0.5
-PER_beta0: 0.4
-
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/perdqn/"
-model_dir: "./models/perdqn/"
+log_dir: "./logs/qrdqn/"
+model_dir: "./models/qrdqn/"
```

### Comparing `xuance-1.0.9/xuance/configs/perdqn/classic_control/MountainCar-v1.yaml` & `xuance-1.1.0/xuance/configs/perdqn/box2d/LunarLander-v2.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 agent: "PerDQN"
 env_name: "Classic Control"
-env_id: "MountainCar-v0"
+env_id: "LunarLander-v2"
 vectorize: "Dummy_Gym"
 policy: "Basic_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 20000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/pg/box2d/BipedalWalker-v3.yaml` & `xuance-1.1.0/xuance/configs/ppg/box2d/LunarLander-v2.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-agent: "PG"
+agent: "PPG"
 env_name: "Box2D"
-env_id: "BipedalWalker-v3"
-representation: "Basic_MLP"
+env_id: "LunarLander-v2"
 vectorize: "Dummy_Gym"
-policy: "Gaussian_Actor"
+representation: "Basic_MLP"
+policy: "Categorical_PPG"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
-activation: 'ReLU'
+critic_hidden_size: [128,]
+activation: "relu"
 
 seed: 1
 parallels: 10
-running_steps: 100000
-n_steps: 1024
-n_epoch: 3
+running_steps: 300000
+n_steps: 256
+n_epoch: 1
+policy_nepoch: 4
+value_nepoch: 8 
+aux_nepoch: 8
 n_minibatch: 1
 learning_rate: 0.0004
 
 ent_coef: 0.01
-clip_grad: 0.5
-clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
+clip_range: 0.2
+kl_beta: 1.0
 gamma: 0.98
-use_gae: False
+use_gae: True
 gae_lambda: 0.95
-use_advnorm: False
+use_advnorm: True
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 10000
+eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/pg/"
-model_dir: "./models/pg/"
+log_dir: "./logs/ppg/"
+model_dir: "./models/ppg/"
```

### Comparing `xuance-1.0.9/xuance/configs/pg/box2d/LunarLander-v2.yaml` & `xuance-1.1.0/xuance/configs/pg/classic_control/Acrobot-v1.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 agent: "PG"
-env_name: "Box2D"
-env_id: "LunarLander-v2"
+env_name: "Classic Control"
+env_id: "Acrobot-v1"
 representation: "Basic_MLP"
 vectorize: "Dummy_Gym"
 policy: "Categorical_Actor"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
-nsteps: 128
-nepoch: 3
-nminibatch: 1
+n_steps: 500
+n_epoch: 1
+n_minibatch: 1
 learning_rate: 0.0004
 
 ent_coef: 0.01
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.98
 use_gae: False
```

### Comparing `xuance-1.0.9/xuance/configs/pg/classic_control/Acrobot-v1.yaml` & `xuance-1.1.0/xuance/configs/pg/classic_control/CartPole-v1.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 agent: "PG"
 env_name: "Classic Control"
-env_id: "Acrobot-v1"
+env_id: "CartPole-v1"
 representation: "Basic_MLP"
 vectorize: "Dummy_Gym"
 policy: "Categorical_Actor"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
-n_steps: 500
+n_steps: 128
 n_epoch: 1
 n_minibatch: 1
 learning_rate: 0.0004
 
 ent_coef: 0.01
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
```

### Comparing `xuance-1.0.9/xuance/configs/pg/classic_control/CartPole-v1.yaml` & `xuance-1.1.0/xuance/configs/pg/mujoco.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 agent: "PG"
-env_name: "Classic Control"
-env_id: "CartPole-v1"
-representation: "Basic_MLP"
+env_name: "MuJoCo"
+env_id: "Ant-v4"
 vectorize: "Dummy_Gym"
-policy: "Categorical_Actor"
+policy: "Gaussian_Actor"
+representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [128,]
-actor_hidden_size: [128,]
-activation: 'ReLU'
+representation_hidden_size: [256, 256]
+actor_hidden_size: []
+activation: "leaky_relu"
+activation_action: 'tanh'
 
 seed: 1
-parallels: 10
-running_steps: 300000
-n_steps: 128
+parallels: 16
+running_steps: 1000000  # 1M
+n_steps: 256
 n_epoch: 1
 n_minibatch: 1
-learning_rate: 0.0004
+learning_rate: 0.0007  # 7e-4
 
-ent_coef: 0.01
+ent_coef: 0.0
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
-gamma: 0.98
+gamma: 0.99
 use_gae: False
 gae_lambda: 0.95
 use_advnorm: False
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 50000
-test_episode: 1
+eval_interval: 5000
+test_episode: 5
 log_dir: "./logs/pg/"
 model_dir: "./models/pg/"
```

### Comparing `xuance-1.0.9/xuance/configs/pg/classic_control/MountainCar-v0.yaml` & `xuance-1.1.0/xuance/configs/ppo/minigrid.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,45 @@
-agent: "PG"
-env_name: "Classic Control"
-env_id: "MountainCar-v0"
+agent: "PPO_Clip"  # choice: PPO_Clip, PPO_KL
+env_name: "MiniGrid"
+env_id: "MiniGrid-Empty-5x5-v0"
+RGBImgPartialObsWrapper: False
+ImgObsWrapper: False
+vectorize: "Dummy_MiniGrid"
+policy: "Categorical_AC"  # choice: Gaussian_AC for continuous actions, Categorical_AC for discrete actions.
 representation: "Basic_MLP"
-vectorize: "Dummy_Gym"
-policy: "Categorical_Actor"
 runner: "DRL"
 
-representation_hidden_size: [128,]
-actor_hidden_size: [128,]
-activation: 'ReLU'
-
-seed: 1
-parallels: 10
-running_steps: 300000
-n_steps: 128
-n_epoch: 3
-n_minibatch: 1
-learning_rate: 0.0004
-
-ent_coef: 0.01
-clip_grad: 0.5
-clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
-gamma: 0.98
-use_gae: False
+representation_hidden_size: [256,]
+actor_hidden_size: [256,]
+critic_hidden_size: [256,]
+activation: "leaky_relu"
+
+seed: 79811
+parallels: 16
+running_steps: 100000
+n_steps: 256
+n_epoch: 16
+n_minibatch: 8
+learning_rate: 0.0001
+
+use_grad_clip: True
+
+vf_coef: 0.25
+ent_coef: 0.0
+target_kl: 0.001  # for PPO_KL agent
+clip_range: 0.2  # for PPO_Clip agent
+clip_grad_norm: 0.5
+gamma: 0.99
+use_gae: True
 gae_lambda: 0.95
-use_advnorm: False
+use_advnorm: True
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 50000
-test_episode: 1
-log_dir: "./logs/pg/"
-model_dir: "./models/pg/"
+eval_interval: 1000
+test_episode: 5
+log_dir: "./logs/ppo/"
+model_dir: "./models/ppo/"
```

### Comparing `xuance-1.0.9/xuance/configs/pg/classic_control/Pendulum-v1.yaml` & `xuance-1.1.0/xuance/configs/pg/classic_control/Pendulum-v1.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 representation: "Basic_MLP"
 vectorize: "Dummy_Gym"
 policy: "Gaussian_Actor"
 runner: "DRL"
 
 representation_hidden_size: [256,]
 actor_hidden_size: [256,]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
+activation_action: 'tanh'
 
 seed: 1
 parallels: 10
 running_steps: 300000
 n_steps: 128
 n_epoch: 1
 n_minibatch: 1
```

### Comparing `xuance-1.0.9/xuance/configs/pg/mujoco.yaml` & `xuance-1.1.0/xuance/configs/a2c/mujoco.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-agent: "PG"
+agent: "A2C"
 env_name: "MuJoCo"
 env_id: "Ant-v4"
 vectorize: "Dummy_Gym"
-policy: "Gaussian_Actor"
+policy: "Gaussian_AC"
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [256, 256]
-actor_hidden_size: []
-activation: "LeakyReLU"
+representation_hidden_size: [256,]
+actor_hidden_size: [256,]
+critic_hidden_size: [256,]
+activation: "leaky_relu"
+activation_action: 'tanh'
 
-seed: 1
+seed: 6782
 parallels: 16
 running_steps: 1000000  # 1M
-n_steps: 256
+n_steps: 16
 n_epoch: 1
 n_minibatch: 1
-learning_rate: 0.0007  # 7e-4
+learning_rate: 0.0007
 
+vf_coef: 0.25
 ent_coef: 0.0
 clip_grad: 0.5
 clip_type: 1  # Gradient clip for Mindspore: 0: ms.ops.clip_by_value; 1: ms.nn.ClipByNorm()
 gamma: 0.99
-use_gae: False
+use_gae: True
 gae_lambda: 0.95
-use_advnorm: False
+use_advnorm: True
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 5000
 test_episode: 5
-log_dir: "./logs/pg/"
-model_dir: "./models/pg/"
+log_dir: "./logs/a2c/"
+model_dir: "./models/a2c/"
```

### Comparing `xuance-1.0.9/xuance/configs/ppg/box2d/BipedalWalker-v3.yaml` & `xuance-1.1.0/xuance/configs/ppg/box2d/BipedalWalker-v3.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 representation: "Basic_MLP"
 policy: "Gaussian_PPG"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
-activation: "LeakyReLU"
+activation: "leaky_relu"
+activation_action: 'tanh'
 
 seed: 1
 parallels: 10
 running_steps: 300000
 n_steps: 256
 n_epoch: 1
 policy_nepoch: 4
```

### Comparing `xuance-1.0.9/xuance/configs/ppg/box2d/LunarLander-v2.yaml` & `xuance-1.1.0/xuance/configs/ppg/classic_control/Acrobot-v1.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 agent: "PPG"
-env_name: "Box2D"
-env_id: "LunarLander-v2"
+env_name: "Classic Control"
+env_id: "Acrobot-v1"
 vectorize: "Dummy_Gym"
 representation: "Basic_MLP"
 policy: "Categorical_PPG"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
-activation: "ReLU"
+activation: "leaky_relu"
 
 seed: 1
 parallels: 10
 running_steps: 300000
 n_steps: 256
 n_epoch: 1
 policy_nepoch: 4
 value_nepoch: 8 
 aux_nepoch: 8
 n_minibatch: 1
-learning_rate: 0.0004
+learning_rate: 0.001
 
 ent_coef: 0.01
 clip_range: 0.2
 kl_beta: 1.0
 gamma: 0.98
 use_gae: True
 gae_lambda: 0.95
@@ -35,8 +35,8 @@
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
 log_dir: "./logs/ppg/"
-model_dir: "./models/ppg/"
+model_dir: "./models/ppg/"
```

### Comparing `xuance-1.0.9/xuance/configs/ppg/classic_control/Acrobot-v1.yaml` & `xuance-1.1.0/xuance/configs/ppg/classic_control/CartPole-v1.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 agent: "PPG"
 env_name: "Classic Control"
-env_id: "Acrobot-v1"
+env_id: "CartPole-v1"
 vectorize: "Dummy_Gym"
 representation: "Basic_MLP"
 policy: "Categorical_PPG"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
-activation: "LeakyReLU"
+activation: "relu"
 
 seed: 1
 parallels: 10
 running_steps: 300000
 n_steps: 256
 n_epoch: 1
 policy_nepoch: 4
 value_nepoch: 8 
 aux_nepoch: 8
 n_minibatch: 1
-learning_rate: 0.001
+learning_rate: 0.0004
 
 ent_coef: 0.01
 clip_range: 0.2
 kl_beta: 1.0
 gamma: 0.98
 use_gae: True
 gae_lambda: 0.95
@@ -35,8 +35,8 @@
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
 log_dir: "./logs/ppg/"
-model_dir: "./models/ppg/"
+model_dir: "./models/ppg/"
```

### Comparing `xuance-1.0.9/xuance/configs/ppg/classic_control/CartPole-v1.yaml` & `xuance-1.1.0/xuance/configs/ppo/classic_control/CartPole-v1.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-agent: "PPG"
+agent: "PPO_Clip"  # Choice: PPO_Clip, PPO_KL
 env_name: "Classic Control"
 env_id: "CartPole-v1"
 vectorize: "Dummy_Gym"
 representation: "Basic_MLP"
-policy: "Categorical_PPG"
+policy: "Categorical_AC"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
-activation: "ReLU"
+activation: 'leaky_relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
 n_steps: 256
-n_epoch: 1
-policy_nepoch: 4
-value_nepoch: 8 
-aux_nepoch: 8
-n_minibatch: 1
+n_epoch: 8
+n_minibatch: 8
 learning_rate: 0.0004
 
+use_grad_clip: True
+
+vf_coef: 0.25
 ent_coef: 0.01
-clip_range: 0.2
-kl_beta: 1.0
+target_kl: 0.001  # for PPO_KL agent
+clip_range: 0.2  # for PPO_Clip agent
+clip_grad_norm: 0.5
 gamma: 0.98
 use_gae: True
 gae_lambda: 0.95
 use_advnorm: True
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 1
-log_dir: "./logs/ppg/"
-model_dir: "./models/ppg/"
+test_episode: 3
+log_dir: "./logs/ppo/"
+model_dir: "./models/ppo/"
```

### Comparing `xuance-1.0.9/xuance/configs/ppg/classic_control/MountainCar-v0.yaml` & `xuance-1.1.0/xuance/configs/ppg/classic_control/MountainCar-v0.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 representation: "Basic_MLP"
 policy: "Categorical_PPG"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
-activation: "LeakyReLU"
+activation: "leaky_relu"
 
 seed: 1
 parallels: 10
 running_steps: 300000
 n_steps: 256
 n_epoch: 1
 policy_nepoch: 4
```

### Comparing `xuance-1.0.9/xuance/configs/ppg/classic_control/Pendulum-v1.yaml` & `xuance-1.1.0/xuance/configs/sac/classic_control/Acrobot-v1.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-agent: "PPG"
+agent: "SACDIS"
 env_name: "Classic Control"
-env_id: "Pendulum-v1"
+env_id: "Acrobot-v1"
 vectorize: "Dummy_Gym"
+policy: "Discrete_SAC"
 representation: "Basic_MLP"
-policy: "Gaussian_PPG"
 runner: "DRL"
 
-representation_hidden_size: [128,]
-actor_hidden_size: [128,]
-critic_hidden_size: [128,]
-activation: "LeakyReLU"
+representation_hidden_size: [256,]
+actor_hidden_size: [128,128,]
+critic_hidden_size: [128,128,]
+activation: "relu"
 
 seed: 1
-parallels: 10
-running_steps: 300000
-n_steps: 256
-n_epoch: 1
-policy_nepoch: 4
-value_nepoch: 8 
-aux_nepoch: 8
-n_minibatch: 1
-learning_rate: 0.001
-
-ent_coef: 0.01
-clip_range: 0.2
-kl_beta: 1.0
+parallels: 16
+n_size: 20000
+batch_size: 256
+actor_learning_rate: 0.001
+critic_learning_rate: 0.01
 gamma: 0.98
-use_gae: True
-gae_lambda: 0.95
-use_advnorm: True
+tau: 0.005
+
+start_noise: 0.25
+end_noise: 0.05
+training_frequency: 2
+running_steps: 500000
+start_training: 2000
+action_type: "DISCRETE"
 
-use_obsnorm: True
-use_rewnorm: True
+use_obsnorm: False
+use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/ppg/"
-model_dir: "./models/ppg/"
+log_dir: "./logs/sac/"
+model_dir: "./models/sac/"
```

### Comparing `xuance-1.0.9/xuance/configs/ppg/mujoco.yaml` & `xuance-1.1.0/xuance/configs/ppg/mujoco.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 representation: "Basic_MLP"
 policy: "Gaussian_PPG"
 runner: "DRL"
 
 representation_hidden_size: [256,]
 actor_hidden_size: [256,]
 critic_hidden_size: [256,]
-activation: "LeakyReLU"
+activation: "leaky_relu"
+activation_action: 'tanh'
 
 seed: 1
 parallels: 16
 running_steps: 1000000  # 1M
 n_steps: 256
 n_minibatch: 4
 n_epoch: 1
```

### Comparing `xuance-1.0.9/xuance/configs/ppo/atari.yaml` & `xuance-1.1.0/xuance/configs/ppo/atari.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-agent: "PPO_Clip"
+agent: "PPO_Clip"  # Choice: PPO_Clip, PPO_KL
 vectorize: "Dummy_Atari"
 env_name: "Atari"
 env_id: "ALE/Breakout-v5"
 obs_type: "grayscale"  # choice for Atari env: ram, rgb, grayscale
 img_size: [84, 84]  # default is 210 x 160 in gym[Atari]
 num_stack: 4  # frame stack trick
 frame_skip: 4  # frame skip trick
@@ -14,29 +14,30 @@
 # Good HyperParameters for Atari Games, Do not change them.
 filters: [32, 64, 64]
 kernels: [8, 4, 3]
 strides: [4, 2, 1]
 fc_hidden_sizes: [512, ]  # fully connected layer hidden sizes.
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 running_steps: 10000000  # 10M
 n_steps: 128
 n_epoch: 4
 n_minibatch: 4
 learning_rate: 0.00025
 
 use_grad_clip: True
 
 vf_coef: 0.25
 ent_coef: 0.01
-clip_range: 0.2
+target_kl: 0.25  # for PPO_KL agent
+clip_range: 0.2  # for PPO_Clip agent
 clip_grad_norm: 0.5
 gamma: 0.99
 use_gae: True
 gae_lambda: 0.95  # gae_lambda: Lambda parameter for calculating N-step advantage
 use_advnorm: True
 
 use_obsnorm: False
```

### Comparing `xuance-1.0.9/xuance/configs/ppo/box2d/BipedalWalker-v3.yaml` & `xuance-1.1.0/xuance/configs/ppo/box2d/LunarLander-v2.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 agent: "PPO_Clip"  # Choice: PPO_Clip, PPO_KL
 env_name: "Box2D"
-env_id: "BipedalWalker-v3"
+env_id: "LunarLander-v2"
 vectorize: "Dummy_Gym"
 representation: "Basic_MLP"
-policy: "Gaussian_AC"
+policy: "Categorical_AC"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
 n_steps: 256
 n_epoch: 8
 n_minibatch: 8
```

### Comparing `xuance-1.0.9/xuance/configs/ppo/box2d/CarRacing-v2.yaml` & `xuance-1.1.0/xuance/configs/ppo/box2d/CarRacing-v2.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # the following three arguments are for "Basic_CNN" representation.
 filters: [16, 16, 32]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 fc_hidden_sizes: [512, ]  # fully connected layer hidden sizes.
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 2
 running_steps: 300000
 n_steps: 256
 n_epoch: 8
 n_minibatch: 8
```

### Comparing `xuance-1.0.9/xuance/configs/ppo/box2d/LunarLander-v2.yaml` & `xuance-1.1.0/xuance/configs/ppo/box2d/BipedalWalker-v3.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 agent: "PPO_Clip"  # Choice: PPO_Clip, PPO_KL
 env_name: "Box2D"
-env_id: "LunarLander-v2"
+env_id: "BipedalWalker-v3"
 vectorize: "Dummy_Gym"
 representation: "Basic_MLP"
-policy: "Categorical_AC"
+policy: "Gaussian_AC"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
+activation_action: 'tanh'
 
 seed: 1
 parallels: 10
 running_steps: 300000
 n_steps: 256
 n_epoch: 8
 n_minibatch: 8
```

### Comparing `xuance-1.0.9/xuance/configs/ppo/classic_control/Acrobot-v1.yaml` & `xuance-1.1.0/xuance/configs/ppo/classic_control/Acrobot-v1.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 representation: "Basic_MLP"
 policy: "Categorical_AC"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
 n_steps: 256
 n_epoch: 8
 n_minibatch: 8
```

### Comparing `xuance-1.0.9/xuance/configs/ppo/classic_control/CartPole-v1.yaml` & `xuance-1.1.0/xuance/configs/ppo/classic_control/MountainCar-v0.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 agent: "PPO_Clip"  # Choice: PPO_Clip, PPO_KL
 env_name: "Classic Control"
-env_id: "CartPole-v1"
+env_id: "MountainCar-v0"
 vectorize: "Dummy_Gym"
 representation: "Basic_MLP"
 policy: "Categorical_AC"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
 
 seed: 1
 parallels: 10
 running_steps: 300000
 n_steps: 256
 n_epoch: 8
 n_minibatch: 8
```

### Comparing `xuance-1.0.9/xuance/configs/ppo/classic_control/MountainCar-v0.yaml` & `xuance-1.1.0/xuance/configs/ppo/classic_control/Pendulum-v1.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 agent: "PPO_Clip"  # Choice: PPO_Clip, PPO_KL
 env_name: "Classic Control"
-env_id: "MountainCar-v0"
+env_id: "Pendulum-v1"
 vectorize: "Dummy_Gym"
 representation: "Basic_MLP"
-policy: "Categorical_AC"
+policy: "Gaussian_AC"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 actor_hidden_size: [128,]
 critic_hidden_size: [128,]
-activation: 'LeakyReLU'
+activation: 'leaky_relu'
+activation_action: 'tanh'
 
 seed: 1
 parallels: 10
 running_steps: 300000
 n_steps: 256
 n_epoch: 8
 n_minibatch: 8
```

### Comparing `xuance-1.0.9/xuance/configs/ppo/classic_control/Pendulum-v1.yaml` & `xuance-1.1.0/xuance/configs/ppo/mujoco.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-agent: "PPO_Clip"  # Choice: PPO_Clip, PPO_KL
-env_name: "Classic Control"
-env_id: "Pendulum-v1"
+agent: "PPO_Clip"  # choice: PPO_Clip, PPO_KL
+env_name: "MuJoCo"
+env_id: "Ant-v4"
 vectorize: "Dummy_Gym"
+policy: "Gaussian_AC"  # choice: Gaussian_AC for continuous actions, Categorical_AC for discrete actions.
 representation: "Basic_MLP"
-policy: "Gaussian_AC"
 runner: "DRL"
 
-representation_hidden_size: [128,]
-actor_hidden_size: [128,]
-critic_hidden_size: [128,]
-activation: 'LeakyReLU'
-
-seed: 1
-parallels: 10
-running_steps: 300000
+representation_hidden_size: [256,]
+actor_hidden_size: [256,]
+critic_hidden_size: [256,]
+activation: "leaky_relu"
+activation_action: 'tanh'
+
+seed: 79811
+parallels: 16
+running_steps: 1000000
 n_steps: 256
-n_epoch: 8
+n_epoch: 16
 n_minibatch: 8
 learning_rate: 0.0004
 
 use_grad_clip: True
 
 vf_coef: 0.25
-ent_coef: 0.01
+ent_coef: 0.0
 target_kl: 0.001  # for PPO_KL agent
 clip_range: 0.2  # for PPO_Clip agent
 clip_grad_norm: 0.5
-gamma: 0.98
+gamma: 0.99
 use_gae: True
 gae_lambda: 0.95
 use_advnorm: True
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 50000
-test_episode: 3
+eval_interval: 5000
+test_episode: 5
 log_dir: "./logs/ppo/"
 model_dir: "./models/ppo/"
```

### Comparing `xuance-1.0.9/xuance/configs/ppo/drones.yaml` & `xuance-1.1.0/xuance/configs/ppo/drones.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 agent: "PPO_Clip"  # choice: PPO_Clip, PPO_KL
 env_name: "Drones"
-env_id: "CtrlAviary"  # choices: ['CtrlAviary', 'HoverAviary', 'VelocityAviary']
-continuous: True
+env_id: "HoverAviary"  # choices: ['CtrlAviary', 'HoverAviary', 'VelocityAviary']
+obs_type: 'kin'
+act_type: 'one_d_rpm'
 num_drones: 1
 record: False
-render: True
+render: False
 obstacles: True
-max_episode_steps: 200
-vectorize: "DummyVecEnv_Drone"
+max_episode_steps: 2000
+vectorize: "Dummy_Drone"
 policy: "Gaussian_AC"  # choice: Gaussian_AC for continuous actions, Categorical_AC for discrete actions.
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [512,]
 actor_hidden_size: [512,]
 critic_hidden_size: [512,]
-activation: "LeakyReLU"
+activation: "leaky_relu"
+activation_action: 'tanh'
 
 seed: 79811
-parallels: 1
+parallels: 10
 running_steps: 1000000
 n_steps: 256
 n_epoch: 16
 n_minibatch: 8
 learning_rate: 0.0004
 
 use_grad_clip: True
```

### Comparing `xuance-1.0.9/xuance/configs/ppo/minigrid.yaml` & `xuance-1.1.0/xuance/configs/ppo/metadrive.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 agent: "PPO_Clip"  # choice: PPO_Clip, PPO_KL
-env_name: "MiniGrid"
-env_id: "MiniGrid-Empty-5x5-v0"
-RGBImgPartialObsWrapper: False
-ImgObsWrapper: False
-vectorize: "DummyVecEnv_MiniGrid"
-policy: "Categorical_AC"  # choice: Gaussian_AC for continuous actions, Categorical_AC for discrete actions.
+env_name: "MetaDrive"
+env_id: "metadrive"
+env_config:  # the configs for MetaDrive environment
+  map: "C"  # see https://metadrive-simulator.readthedocs.io/en/latest/rl_environments.html#generalization-environment for choices
+render: False
+vectorize: "Subproc_MetaDrive"
+policy: "Gaussian_AC"  # choice: Gaussian_AC for continuous actions, Categorical_AC for discrete actions.
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [256,]
-actor_hidden_size: [256,]
-critic_hidden_size: [256,]
-activation: "LeakyReLU"
-
-seed: 79811
-parallels: 16
-running_steps: 100000
-n_steps: 256
-n_epoch: 16
-n_minibatch: 8
-learning_rate: 0.0001
+representation_hidden_size: [512,]
+actor_hidden_size: [512, 512]
+critic_hidden_size: [512, 512]
+activation: "leaky_relu"
+activation_action: 'tanh'
+
+seed: 1
+parallels: 10
+running_steps: 500000
+n_steps: 128
+n_epoch: 4
+n_minibatch: 4
+learning_rate: 0.00025
 
 use_grad_clip: True
 
 vf_coef: 0.25
 ent_coef: 0.0
 target_kl: 0.001  # for PPO_KL agent
 clip_range: 0.2  # for PPO_Clip agent
@@ -35,11 +37,11 @@
 
 use_obsnorm: True
 use_rewnorm: True
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 1000
+eval_interval: 5000
 test_episode: 5
 log_dir: "./logs/ppo/"
 model_dir: "./models/ppo/"
```

### Comparing `xuance-1.0.9/xuance/configs/ppo/mujoco.yaml` & `xuance-1.1.0/xuance/configs/sac/box2d/BipedalWalker-v3.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,39 @@
-agent: "PPO_Clip"  # choice: PPO_Clip, PPO_KL
-env_name: "MuJoCo"
-env_id: "Ant-v4"
+agent: "SAC"
+env_name: "Box2D"
+env_id: "BipedalWalker-v3"
 vectorize: "Dummy_Gym"
-policy: "Gaussian_AC"  # choice: Gaussian_AC for continuous actions, Categorical_AC for discrete actions.
+policy: "Gaussian_SAC"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [256,]
 actor_hidden_size: [256,]
 critic_hidden_size: [256,]
-activation: "LeakyReLU"
+activation: "relu"
+activation_action: 'tanh'
 
-seed: 79811
+seed: 1
 parallels: 16
-running_steps: 1000000
-n_steps: 256
-n_epoch: 16
-n_minibatch: 8
-learning_rate: 0.0004
+n_size: 20000
+batch_size: 256
+actor_learning_rate: 0.001
+critic_learning_rate: 0.001
+gamma: 0.98
+tau: 0.005
+
+start_noise: 0.25
+end_noise: 0.05
+training_frequency: 2
+running_steps: 500000
+start_training: 2000
 
-use_grad_clip: True
-
-vf_coef: 0.25
-ent_coef: 0.0
-target_kl: 0.001  # for PPO_KL agent
-clip_range: 0.2  # for PPO_Clip agent
-clip_grad_norm: 0.5
-gamma: 0.99
-use_gae: True
-gae_lambda: 0.95
-use_advnorm: True
-
-use_obsnorm: True
-use_rewnorm: True
+use_obsnorm: False
+use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 5000
-test_episode: 5
-log_dir: "./logs/ppo/"
-model_dir: "./models/ppo/"
+eval_interval: 50000
+test_episode: 1
+log_dir: "./logs/sac/"
+model_dir: "./models/sac/"
```

### Comparing `xuance-1.0.9/xuance/configs/qmix/football/3v1.yaml` & `xuance-1.1.0/xuance/configs/qmix/football/3v1.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 fc_hidden_sizes: [128, ]
 recurrent_hidden_size: 128
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [128, ]
 q_hidden_size: [128, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 hidden_dim_mixing_net: 128  # hidden units of mixing network
 hidden_dim_hyper_net: 128  # hidden units of hyper network
 
 seed: 1
 parallels: 50
 buffer_size: 5000
```

### Comparing `xuance-1.0.9/xuance/configs/qmix/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/qmix/mpe/simple_spread_v3.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
 use_recurrent: False
 rnn:
 representation_hidden_size: [64, ]
 q_hidden_size: [128, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 hidden_dim_mixing_net: 64  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 16
 buffer_size: 100000
```

### Comparing `xuance-1.0.9/xuance/configs/qmix/sc2/1c3s5z.yaml` & `xuance-1.1.0/xuance/configs/qmix/sc2/1c3s5z.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 32  # hidden units of hyper network
 
 seed: 1
 parallels: 8
 buffer_size: 5000
```

### Comparing `xuance-1.0.9/xuance/configs/qmix/sc2/25m.yaml` & `xuance-1.1.0/xuance/configs/qmix/sc2/25m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 32  # hidden units of hyper network
 
 seed: 1
 parallels: 8
 buffer_size: 5000
```

### Comparing `xuance-1.0.9/xuance/configs/qmix/sc2/2m_vs_1z.yaml` & `xuance-1.1.0/xuance/configs/qmix/sc2/2m_vs_1z.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 32  # hidden units of hyper network
 
 seed: 1
 parallels: 8
 buffer_size: 5000
```

### Comparing `xuance-1.0.9/xuance/configs/qmix/sc2/2s3z.yaml` & `xuance-1.1.0/xuance/configs/qmix/sc2/2s3z.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 32  # hidden units of hyper network
 
 seed: 1
 parallels: 8
 buffer_size: 5000
```

### Comparing `xuance-1.0.9/xuance/configs/qmix/sc2/3m.yaml` & `xuance-1.1.0/xuance/configs/qmix/sc2/3m.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 32  # hidden units of hyper network
 
 seed: 1
 parallels: 8
 buffer_size: 5000
```

### Comparing `xuance-1.0.9/xuance/configs/qmix/sc2/5m_vs_6m.yaml` & `xuance-1.1.0/xuance/configs/qmix/sc2/5m_vs_6m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 32  # hidden units of hyper network
 
 seed: 1
 parallels: 8
 buffer_size: 5000
```

### Comparing `xuance-1.0.9/xuance/configs/qmix/sc2/8m.yaml` & `xuance-1.1.0/xuance/configs/qmix/sc2/8m.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 32  # hidden units of hyper network
 
 seed: 1
 parallels: 8
 buffer_size: 5000
```

### Comparing `xuance-1.0.9/xuance/configs/qmix/sc2/8m_vs_9m.yaml` & `xuance-1.1.0/xuance/configs/qmix/sc2/8m_vs_9m.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 32  # hidden units of hyper network
 
 seed: 1
 parallels: 8
 buffer_size: 5000
```

### Comparing `xuance-1.0.9/xuance/configs/qmix/sc2/MMM2.yaml` & `xuance-1.1.0/xuance/configs/qmix/sc2/MMM2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 32  # hidden units of hyper network
 
 seed: 1
 parallels: 8
 buffer_size: 5000
```

### Comparing `xuance-1.0.9/xuance/configs/qmix/sc2/corridor.yaml` & `xuance-1.1.0/xuance/configs/qmix/sc2/corridor.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 32  # hidden units of hyper network
 
 seed: 1
 parallels: 8
 buffer_size: 5000
```

### Comparing `xuance-1.0.9/xuance/configs/qrdqn/atari.yaml` & `xuance-1.1.0/xuance/configs/qrdqn/atari.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [32, 64, 64]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512, ]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1069
 parallels: 5
 n_size: 100000
 batch_size: 32  # 64
 learning_rate: 0.0001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/qrdqn/box2d/CarRacing-v2.yaml` & `xuance-1.1.0/xuance/configs/qrdqn/box2d/CarRacing-v2.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # the following three arguments are for "Basic_CNN" representation.
 filters: [16, 16, 32]  #  [16, 16, 32, 32]
 kernels: [8, 4, 3]  # [8, 6, 4, 4]
 strides: [4, 2, 1]  # [2, 2, 2, 2]
 
 q_hidden_size: [512,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 2
 n_size: 10000
 batch_size: 32
 learning_rate: 0.0001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/qrdqn/box2d/LunarLander-v2.yaml` & `xuance-1.1.0/xuance/configs/qrdqn/box2d/LunarLander-v2.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 vectorize: "Dummy_Gym"
 policy: "QR_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 10000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/qrdqn/classic_control/Acrobot-v1.yaml` & `xuance-1.1.0/xuance/configs/qrdqn/classic_control/Acrobot-v1.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 vectorize: "Dummy_Gym"
 policy: "QR_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 20000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/qrdqn/classic_control/CartPole-v1.yaml` & `xuance-1.1.0/xuance/configs/qrdqn/classic_control/CartPole-v1.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 vectorize: "Dummy_Gym"
 policy: "QR_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 q_hidden_size: [128,]
-activation: 'ReLU'
+activation: 'relu'
 
 seed: 1
 parallels: 10
 n_size: 20000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
```

### Comparing `xuance-1.0.9/xuance/configs/qrdqn/classic_control/MountainCar-v0.yaml` & `xuance-1.1.0/xuance/configs/dueldqn/classic_control/CartPole-v1.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-agent: "QRDQN"
+agent: "Duel_DQN"
 env_name: "Classic Control"
-env_id: "MountainCar-v0"
+env_id: "CartPole-v1"
 vectorize: "Dummy_Gym"
-policy: "QR_Q_network"
+policy: "Duel_Q_network"
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [128,]
-q_hidden_size: [128,]
-activation: 'ReLU'
+representation_hidden_size: [128, ]
+q_hidden_size: [128, ]
+activation: 'relu'
 
 seed: 1
 parallels: 10
-n_size: 20000
+n_size: 10000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99
-quantile_num: 20
 
-start_greedy: 0.25
+start_greedy: 0.5
 end_greedy: 0.01
-decay_step_greedy: 30000
-sync_frequency: 100
+decay_step_greedy: 20000
+sync_frequency: 50
 training_frequency: 1
-running_steps: 300000
+running_steps: 500000
 start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/qrdqn/"
-model_dir: "./models/qrdqn/"
+log_dir: "./logs/dueldqn/"
+model_dir: "./models/dueldqn/"
```

### Comparing `xuance-1.0.9/xuance/configs/qtran/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/qtran/mpe/simple_spread_v3.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 vectorize: "Dummy_Pettingzoo"
 runner: "Pettingzoo_Runner"
 
 use_recurrent: False
 rnn:
 representation_hidden_size: [256, ]
 q_hidden_size: [256, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 hidden_dim_mixing_net: 64  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 qtran_net_hidden_dim: 64
 lambda_opt: 1.0
 lambda_nopt: 1.0
```

### Comparing `xuance-1.0.9/xuance/configs/sac/atari.yaml` & `xuance-1.1.0/xuance/configs/sac/atari.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 runner: "DRL"
 
 filters: [32, 32, 64, 64]
 kernels: [8, 4, 4, 4]
 strides: [4, 2, 2, 2]
 actor_hidden_size: [128, 128]
 critic_hidden_size: [128, 128]
-activation: "LeakyReLU"
+activation: "leaky_relu"
 
 seed: 1069
 parallels: 5
 n_size: 100000
 batch_size: 32  # 64
 actor_learning_rate: 0.001
 critic_learning_rate: 0.001
```

### Comparing `xuance-1.0.9/xuance/configs/sac/box2d/BipedalWalker-v3.yaml` & `xuance-1.1.0/xuance/configs/sac/box2d/LunarLander-v2.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-agent: "SAC"
+agent: "SACDIS"
 env_name: "Box2D"
-env_id: "BipedalWalker-v3"
+env_id: "LunarLander-v2"
 vectorize: "Dummy_Gym"
-policy: "Gaussian_SAC"
+policy: "Discrete_SAC"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [256,]
-actor_hidden_size: [256,]
-critic_hidden_size: [256,]
-activation: "ReLU"
+actor_hidden_size: [128,128,]
+critic_hidden_size: [128,128,]
+activation: "relu"
 
 seed: 1
 parallels: 16
 n_size: 20000
 batch_size: 256
 actor_learning_rate: 0.001
-critic_learning_rate: 0.001
+critic_learning_rate: 0.01
 gamma: 0.98
 tau: 0.005
 
 start_noise: 0.25
 end_noise: 0.05
 training_frequency: 2
 running_steps: 500000
 start_training: 2000
+action_type: "DISCRETE"
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
```

### Comparing `xuance-1.0.9/xuance/configs/sac/box2d/LunarLander-v2.yaml` & `xuance-1.1.0/xuance/configs/td3/mujoco.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-agent: "SACDIS"
-env_name: "Box2D"
-env_id: "LunarLander-v2"
+agent: "TD3"
+env_name: "MuJoCo"
+env_id: "Ant-v4"
 vectorize: "Dummy_Gym"
-policy: "Discrete_SAC"
-representation: "Basic_MLP"
+policy: "TD3_Policy"
+representation: "Basic_Identical"
 runner: "DRL"
 
-representation_hidden_size: [256,]
-actor_hidden_size: [128,128,]
-critic_hidden_size: [128,128,]
-activation: "ReLU"
+representation_hidden_size:  # If you choose Basic_Identical representation, then ignore this value
+actor_hidden_size: [400, 300]
+critic_hidden_size: [400, 300]
+activation: "leaky_relu"
+activation_action: 'tanh'
 
-seed: 1
-parallels: 16
-n_size: 20000
-batch_size: 256
+seed: 6782
+parallels: 4  # number of environments
+n_size: 50000
+batch_size: 100
 actor_learning_rate: 0.001
-critic_learning_rate: 0.01
-gamma: 0.98
+actor_update_delay: 2
+critic_learning_rate: 0.001
+gamma: 0.99
 tau: 0.005
 
-start_noise: 0.25
-end_noise: 0.05
-training_frequency: 2
-running_steps: 500000
-start_training: 2000
-action_type: "DISCRETE"
+start_noise: 0.5
+end_noise: 0.1
+training_frequency: 1
+running_steps: 1000000
+start_training: 10000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 50000
-test_episode: 1
-log_dir: "./logs/sac/"
-model_dir: "./models/sac/"
+eval_interval: 5000
+test_episode: 5
+log_dir: "./logs/td3/"
+model_dir: "./models/td3/"
```

### Comparing `xuance-1.0.9/xuance/configs/sac/classic_control/Acrobot-v1.yaml` & `xuance-1.1.0/xuance/configs/sac/metadrive.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-agent: "SACDIS"
-env_name: "Classic Control"
-env_id: "Acrobot-v1"
-vectorize: "Dummy_Gym"
-policy: "Discrete_SAC"
-representation: "Basic_MLP"
+agent: "SAC"
+env_name: "MetaDrive"
+env_id: "metadrive"
+env_config:  # the configs for MetaDrive environment
+  map: "C"  # see https://metadrive-simulator.readthedocs.io/en/latest/rl_environments.html#generalization-environment for choices
+render: False
+vectorize: "Subproc_MetaDrive"
+policy: "Gaussian_SAC"
+representation: "Basic_Identical"
 runner: "DRL"
 
-representation_hidden_size: [256,]
-actor_hidden_size: [128,128,]
-critic_hidden_size: [128,128,]
-activation: "ReLU"
+representation_hidden_size:
+actor_hidden_size: [512, 512]
+critic_hidden_size: [512, 512]
+activation: "relu"
+activation_action: 'tanh'
 
 seed: 1
-parallels: 16
-n_size: 20000
+parallels: 10
+n_size: 250000
 batch_size: 256
 actor_learning_rate: 0.001
-critic_learning_rate: 0.01
-gamma: 0.98
+critic_learning_rate: 0.001
+gamma: 0.99
+alpha: 0.2
 tau: 0.005
+learning_rate: 0.0003
 
 start_noise: 0.25
-end_noise: 0.05
-training_frequency: 2
-running_steps: 500000
-start_training: 2000
-action_type: "DISCRETE"
+end_noise: 0.01
+training_frequency: 1
+running_steps: 1000000
+start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 50000
-test_episode: 1
+eval_interval: 10000
+test_episode: 5
 log_dir: "./logs/sac/"
 model_dir: "./models/sac/"
```

### Comparing `xuance-1.0.9/xuance/configs/sac/classic_control/CartPole-v1.yaml` & `xuance-1.1.0/xuance/configs/td3/classic_control/Pendulum-v1.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-agent: "SACDIS"
+agent: "TD3"
 env_name: "Classic Control"
-env_id: "CartPole-v1"
+env_id: "Pendulum-v1"
 vectorize: "Dummy_Gym"
-policy: "Discrete_SAC"
-representation: "Basic_MLP"
+representation: "Basic_Identical"
+policy: "TD3_Policy"
 runner: "DRL"
 
-representation_hidden_size: [256,]
-actor_hidden_size: [128,128,]
-critic_hidden_size: [128,128,]
-activation: "ReLU"
+representation_hidden_size: [64]
+actor_hidden_size: [256, ]
+critic_hidden_size: [256, ]
+activation: "leaky_relu"
+activation_action: 'tanh'
 
 seed: 1
-parallels: 16
+parallels: 10
 n_size: 20000
 batch_size: 256
-actor_learning_rate: 0.001
-critic_learning_rate: 0.01
+actor_learning_rate: 0.0005
+critic_learning_rate: 0.001
 gamma: 0.98
 tau: 0.005
+actor_update_delay: 3
 
 start_noise: 0.25
 end_noise: 0.05
 training_frequency: 2
 running_steps: 500000
 start_training: 2000
-action_type: "DISCRETE"
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
 test_episode: 1
-log_dir: "./logs/sac/"
-model_dir: "./models/sac/"
+log_dir: "./logs/td3/"
+model_dir: "./models/td3/"
```

### Comparing `xuance-1.0.9/xuance/configs/sac/classic_control/MountainCar-v0.yaml` & `xuance-1.1.0/xuance/configs/sac/classic_control/MountainCar-v0.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 policy: "Discrete_SAC"
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [256,]
 actor_hidden_size: [128,128,]
 critic_hidden_size: [128,128,]
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 16
 n_size: 20000
 batch_size: 256
 actor_learning_rate: 0.001
 critic_learning_rate: 0.01
```

### Comparing `xuance-1.0.9/xuance/configs/sac/classic_control/Pendulum-v1.yaml` & `xuance-1.1.0/xuance/configs/ddpg/classic_control/Pendulum-v1.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-agent: "SAC"
+agent: "DDPG"
 env_name: "Classic Control"
 env_id: "Pendulum-v1"
 vectorize: "Dummy_Gym"
-policy: "Gaussian_SAC"
+policy: "DDPG_Policy"
 representation: "Basic_MLP"
 runner: "DRL"
 
-representation_hidden_size: [256,]
+representation_hidden_size: [64]
 actor_hidden_size: [256,]
 critic_hidden_size: [256,]
-activation: "ReLU"
+activation: "relu"
+activation_action: 'tanh'
 
 seed: 1
-parallels: 16
-n_size: 20000
+parallels: 10
+n_size: 200000
 batch_size: 256
 actor_learning_rate: 0.001
 critic_learning_rate: 0.001
 gamma: 0.98
 tau: 0.005
+learning_rate: 0.0007
 
-start_noise: 0.25
-end_noise: 0.05
-training_frequency: 2
+start_noise: 0.1
+end_noise: 0.1
+training_frequency: 1
 running_steps: 500000
-start_training: 2000
+start_training: 1000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
 eval_interval: 50000
-test_episode: 1
-log_dir: "./logs/sac/"
-model_dir: "./models/sac/"
+test_episode: 3
+log_dir: "./logs/ddpg/"
+model_dir: "./models/ddpg/"
```

### Comparing `xuance-1.0.9/xuance/configs/sac/mujoco.yaml` & `xuance-1.1.0/xuance/configs/sac/mujoco.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 policy: "Gaussian_SAC"
 representation: "Basic_Identical"
 runner: "DRL"
 
 representation_hidden_size:
 actor_hidden_size: [256, 256]
 critic_hidden_size: [256, 256]
-activation: "LeakyReLU"
+activation: "leaky_relu"
+activation_action: 'tanh'
 
 seed: 1
 parallels: 4
 n_size: 250000
 batch_size: 256
 actor_learning_rate: 0.001
 critic_learning_rate: 0.001
```

### Comparing `xuance-1.0.9/xuance/configs/spdqn/Platform.yaml` & `xuance-1.1.0/xuance/configs/spdqn/Platform.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 render: False
 representation: "Basic_MLP"
 runner: "DRL"
 
 representation_hidden_size: [128,]
 conactor_hidden_size: [128,]
 qnetwork_hidden_size: [128, ]
-activation: "ReLU"
+activation: "relu"
+activation_action: 'tanh'
 
 n_size: 20000
 batch_size: 128
 learning_rate: 0.001
 gamma: 0.99
 tau: 0.005
```

### Comparing `xuance-1.0.9/xuance/configs/td3/box2d/BipedalWalker-v3.yaml` & `xuance-1.1.0/xuance/configs/td3/box2d/BipedalWalker-v3.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 vectorize: "Dummy_Gym"
 representation: "Basic_Identical"
 policy: "TD3_Policy"
 runner: "DRL"
 
 actor_hidden_size: [256, ]
 critic_hidden_size: [256, ]
-activation: "LeakyReLU"
+activation: "leaky_relu"
+activation_action: 'tanh'
 
 seed: 1
 parallels: 10
 n_size: 20000
 batch_size: 256
 actor_learning_rate: 0.0005
 critic_learning_rate: 0.001
```

### Comparing `xuance-1.0.9/xuance/configs/td3/classic_control/Pendulum-v1.yaml` & `xuance-1.1.0/xuance/configs/ddpg/drones.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,46 @@
-agent: "TD3"
-env_name: "Classic Control"
-env_id: "Pendulum-v1"
-vectorize: "Dummy_Gym"
+agent: "DDPG"
+env_name: "Drones"
+env_id: "HoverAviary"
+obs_type: 'kin'
+act_type: 'one_d_rpm'
+num_drones: 1
+record: False
+obstacles: True
+max_episode_steps: 2000  #
+render: False
+sleep: 0.01
+vectorize: "Dummy_Drone"
+policy: "DDPG_Policy"
 representation: "Basic_Identical"
-policy: "TD3_Policy"
 runner: "DRL"
 
-actor_hidden_size: [256, ]
-critic_hidden_size: [256, ]
-activation: "LeakyReLU"
+actor_hidden_size: [64, 64]
+critic_hidden_size: [64, 64]
+activation: "leaky_relu"
+activation_action: 'tanh'
 
 seed: 1
 parallels: 10
-n_size: 20000
-batch_size: 256
-actor_learning_rate: 0.0005
+n_size: 1000000  # buffer
+batch_size: 1024
+actor_learning_rate: 0.001
 critic_learning_rate: 0.001
-gamma: 0.98
+gamma: 0.99
 tau: 0.005
-actor_update_delay: 3
 
-start_noise: 0.25
-end_noise: 0.05
-training_frequency: 2
-running_steps: 500000
+start_noise: 0.1
+end_noise: 0.1
+training_frequency: 1
+running_steps: 10000000 # total step
 start_training: 2000
 
 use_obsnorm: False
 use_rewnorm: False
 obsnorm_range: 5
 rewnorm_range: 5
 
 test_steps: 10000
-eval_interval: 50000
-test_episode: 1
-log_dir: "./logs/td3/"
-model_dir: "./models/td3/"
+eval_interval: 100000
+test_episode: 3
+log_dir: "./logs/ddpg/"
+model_dir: "./models/ddpg/"
```

### Comparing `xuance-1.0.9/xuance/configs/vdac/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/vdac/mpe/simple_spread_v3.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 use_recurrent: False
 rnn:
 representation_hidden_size: [64, ]  # the units for each hidden layer
 gain: 0.01
 
 actor_hidden_size: [64, ]
 critic_hidden_size: [64, ]
-activation: "ReLU"
+activation: "relu"
 
 mixer: "VDN"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 32  # hidden units of hyper network
 
 seed: 1
 parallels: 128
```

### Comparing `xuance-1.0.9/xuance/configs/vdac/sc2/1c3s5z.yaml` & `xuance-1.1.0/xuance/configs/vdac/sc2/2s3z.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "VDAC"
 env_name: "StarCraft2"
-env_id: "1c3s5z"
+env_id: "2s3z"
 fps: 15
 policy: "Categorical_MAAC_Policy_Share"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 
 # recurrent settings for Basic_RNN representation
@@ -17,15 +17,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
```

### Comparing `xuance-1.0.9/xuance/configs/vdac/sc2/25m.yaml` & `xuance-1.1.0/xuance/configs/vdac/sc2/25m.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
```

### Comparing `xuance-1.0.9/xuance/configs/vdac/sc2/2m_vs_1z.yaml` & `xuance-1.1.0/xuance/configs/vdac/sc2/2m_vs_1z.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
```

### Comparing `xuance-1.0.9/xuance/configs/vdac/sc2/2s3z.yaml` & `xuance-1.1.0/xuance/configs/vdac/sc2/1c3s5z.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "VDAC"
 env_name: "StarCraft2"
-env_id: "2s3z"
+env_id: "1c3s5z"
 fps: 15
 policy: "Categorical_MAAC_Policy_Share"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 
 # recurrent settings for Basic_RNN representation
@@ -17,15 +17,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
```

### Comparing `xuance-1.0.9/xuance/configs/vdac/sc2/3m.yaml` & `xuance-1.1.0/xuance/configs/vdac/sc2/3m.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 mixer: "QMIX"  # choices: Independent, VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
```

### Comparing `xuance-1.0.9/xuance/configs/vdac/sc2/5m_vs_6m.yaml` & `xuance-1.1.0/xuance/configs/vdac/sc2/5m_vs_6m.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
```

### Comparing `xuance-1.0.9/xuance/configs/vdac/sc2/8m.yaml` & `xuance-1.1.0/xuance/configs/vdac/sc2/MMM2.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "VDAC"
 env_name: "StarCraft2"
-env_id: "8m"
+env_id: "MMM2"
 fps: 15
 policy: "Categorical_MAAC_Policy_Share"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: True
 
@@ -14,29 +14,29 @@
 recurrent_layer_N: 1
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
-gain: 0.01
+gain: 1.0
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
 n_size: 8
 n_epoch: 1
-n_minibatch: 1
+n_minibatch: 2
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
 clip_range: 0.2
@@ -55,14 +55,14 @@
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 1000000  # 1M
+running_steps: 10000000  # 10M
 training_frequency: 1
 
-eval_interval: 5000
+eval_interval: 50000
 test_episode: 16
 log_dir: "./logs/vdac/"
 model_dir: "./models/vdac/"
```

### Comparing `xuance-1.0.9/xuance/configs/vdac/sc2/8m_vs_9m.yaml` & `xuance-1.1.0/xuance/configs/vdac/sc2/8m_vs_9m.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
 gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
+activation: "relu"
 
 mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 seed: 1
 parallels: 8
```

### Comparing `xuance-1.0.9/xuance/configs/vdac/sc2/MMM2.yaml` & `xuance-1.1.0/xuance/configs/ippo/sc2/2s3z.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-agent: "VDAC"
+agent: "IPPO"
 env_name: "StarCraft2"
-env_id: "MMM2"
+env_id: "2s3z"
 fps: 15
-policy: "Categorical_MAAC_Policy_Share"
+policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
-on_policy: True
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
 rnn: "GRU"
 recurrent_layer_N: 1
-fc_hidden_sizes: [64, ]
+fc_hidden_sizes: [64, 64, 64]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
-gain: 1.0
+gain: 0.01
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
-
-mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
-hidden_dim_mixing_net: 32  # hidden units of mixing network
-hidden_dim_hyper_net: 64  # hidden units of hyper network
+activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 8
-n_epoch: 1
-n_minibatch: 2
+n_size: 128
+n_epoch: 15
+n_minibatch: 1
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
 clip_range: 0.2
@@ -55,14 +50,14 @@
 use_huber_loss: True  # True: use huber loss; False: use MSE loss.
 huber_delta: 10.0
 use_advnorm: True  # use advantage normalization.
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
-running_steps: 10000000  # 10M
+running_steps: 2000000
 training_frequency: 1
 
-eval_interval: 50000
+eval_interval: 20000
 test_episode: 16
-log_dir: "./logs/vdac/"
-model_dir: "./models/vdac/"
+log_dir: "./logs/ippo/"
+model_dir: "./models/ippo/"
```

### Comparing `xuance-1.0.9/xuance/configs/vdac/sc2/corridor.yaml` & `xuance-1.1.0/xuance/configs/ippo/sc2/MMM2.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,38 @@
-agent: "VDAC"
+agent: "IPPO"
 env_name: "StarCraft2"
-env_id: "corridor"
+env_id: "MMM2"
 fps: 15
-policy: "Categorical_MAAC_Policy_Share"
+policy: "Categorical_MAAC_Policy"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: True
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
 rnn: "GRU"
 recurrent_layer_N: 1
-fc_hidden_sizes: [64, ]
+fc_hidden_sizes: [64, 64, 64]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 normalize: "LayerNorm"
 initialize: "orthogonal"
-gain: 0.01
+gain: 1.0
 
 actor_hidden_size: []
 critic_hidden_size: []
-activation: "ReLU"
-
-mixer: "QMIX"  # choices: VDN (sum), QMIX (monotonic)
-hidden_dim_mixing_net: 32  # hidden units of mixing network
-hidden_dim_hyper_net: 64  # hidden units of hyper network
+activation: "relu"
 
 seed: 1
 parallels: 8
-n_size: 8
-n_epoch: 1
-n_minibatch: 1
+n_size: 128
+n_epoch: 5
+n_minibatch: 2
 learning_rate: 0.0007  # 7e-4
 weight_decay: 0
 
 vf_coef: 1.0
 ent_coef: 0.01
 target_kl: 0.25
 clip_range: 0.2
@@ -58,11 +54,11 @@
 use_gae: True  # use GAE trick to calculate returns.
 gae_lambda: 0.95
 
 start_training: 1
 running_steps: 10000000  # 10M
 training_frequency: 1
 
-eval_interval: 50000
+eval_interval: 100000
 test_episode: 16
-log_dir: "./logs/vdac/"
-model_dir: "./models/vdac/"
+log_dir: "./logs/ippo/"
+model_dir: "./models/ippo/"
```

### Comparing `xuance-1.0.9/xuance/configs/vdn/football/3v1.yaml` & `xuance-1.1.0/xuance/configs/vdn/football/3v1.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 fc_hidden_sizes: [128, ]
 recurrent_hidden_size: 128
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [128, ]
 q_hidden_size: [128, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 50
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
```

### Comparing `xuance-1.0.9/xuance/configs/vdn/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/vdn/mpe/simple_spread_v3.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 runner: "Pettingzoo_Runner"
 on_policy: False
 
 use_recurrent: False
 rnn:
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 16
 buffer_size: 100000
 batch_size: 256
 learning_rate: 0.001
 gamma: 0.99  # discount factor
```

### Comparing `xuance-1.0.9/xuance/configs/vdn/sc2/1c3s5z.yaml` & `xuance-1.1.0/xuance/configs/vdn/sc2/1c3s5z.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
```

### Comparing `xuance-1.0.9/xuance/configs/vdn/sc2/25m.yaml` & `xuance-1.1.0/xuance/configs/wqmix/sc2/1c3s5z.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-agent: "VDN"  # the learning algorithms_marl
-global_state: False
+agent: "OWQMIX"  # choice: CWQMIX, OWQMIX
 env_name: "StarCraft2"
-env_id: "25m"
+env_id: "1c3s5z"
 fps: 15
-policy: "Mixing_Q_network"
+policy: "Weighted_Mixing_Q_network"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
@@ -16,33 +15,39 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
+alpha: 0.1
+
+hidden_dim_mixing_net: 32  # hidden units of mixing network
+hidden_dim_hyper_net: 64  # hidden units of hyper network
+
+hidden_dim_ff_mix_net: 256  # hidden units of mixing network
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
 decay_step_greedy: 50000
 start_training: 1000  # start training after n episodes
-running_steps: 5000000  # 5M
+running_steps: 2000000  # 2M
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 50000
+eval_interval: 20000
 test_episode: 16
-log_dir: "./logs/vdn/"
-model_dir: "./models/vdn/"
+log_dir: "./logs/wqmix/"
+model_dir: "./models/wqmix/"
```

### Comparing `xuance-1.0.9/xuance/configs/vdn/sc2/2m_vs_1z.yaml` & `xuance-1.1.0/xuance/configs/vdn/sc2/3m.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 agent: "VDN"  # the learning algorithms_marl
 global_state: False
 env_name: "StarCraft2"
-env_id: "2m_vs_1z"
+env_id: "3m"
 fps: 15
 policy: "Mixing_Q_network"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -16,15 +16,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
```

### Comparing `xuance-1.0.9/xuance/configs/vdn/sc2/2s3z.yaml` & `xuance-1.1.0/xuance/configs/vdn/sc2/8m.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 agent: "VDN"  # the learning algorithms_marl
 global_state: False
 env_name: "StarCraft2"
-env_id: "2s3z"
+env_id: "8m"
 fps: 15
 policy: "Mixing_Q_network"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -16,33 +16,33 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
 decay_step_greedy: 50000
 start_training: 1000  # start training after n episodes
-running_steps: 2000000  # 2M
+running_steps: 1000000  # 1M
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 20000
+eval_interval: 10000
 test_episode: 16
 log_dir: "./logs/vdn/"
 model_dir: "./models/vdn/"
```

### Comparing `xuance-1.0.9/xuance/configs/vdn/sc2/3m.yaml` & `xuance-1.1.0/xuance/configs/vdn/sc2/MMM2.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 agent: "VDN"  # the learning algorithms_marl
 global_state: False
 env_name: "StarCraft2"
-env_id: "3m"
+env_id: "MMM2"
 fps: 15
 policy: "Mixing_Q_network"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -16,33 +16,33 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
 decay_step_greedy: 50000
 start_training: 1000  # start training after n episodes
-running_steps: 1000000  # 1M
+running_steps: 10000000  # 1M
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 10000
+eval_interval: 100000
 test_episode: 16
 log_dir: "./logs/vdn/"
 model_dir: "./models/vdn/"
```

### Comparing `xuance-1.0.9/xuance/configs/vdn/sc2/5m_vs_6m.yaml` & `xuance-1.1.0/xuance/configs/iql/sc2/5m_vs_6m.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-agent: "VDN"  # the learning algorithms_marl
-global_state: False
+agent: "IQL"  # the learning algorithms_marl
 env_name: "StarCraft2"
 env_id: "5m_vs_6m"
 fps: 15
-policy: "Mixing_Q_network"
+policy: "Basic_Q_network_marl"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
@@ -16,15 +15,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
@@ -40,9 +39,9 @@
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
 eval_interval: 100000
 test_episode: 16
-log_dir: "./logs/vdn/"
-model_dir: "./models/vdn/"
+log_dir: "./logs/iql/"
+model_dir: "./models/iql/"
```

### Comparing `xuance-1.0.9/xuance/configs/vdn/sc2/8m.yaml` & `xuance-1.1.0/xuance/configs/iql/sc2/8m.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-agent: "VDN"  # the learning algorithms_marl
-global_state: False
+agent: "IQL"  # the learning algorithms_marl
 env_name: "StarCraft2"
 env_id: "8m"
 fps: 15
-policy: "Mixing_Q_network"
+policy: "Basic_Q_network_marl"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
@@ -16,15 +15,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
@@ -40,9 +39,9 @@
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
 eval_interval: 10000
 test_episode: 16
-log_dir: "./logs/vdn/"
-model_dir: "./models/vdn/"
+log_dir: "./logs/iql/"
+model_dir: "./models/iql/"
```

### Comparing `xuance-1.0.9/xuance/configs/vdn/sc2/8m_vs_9m.yaml` & `xuance-1.1.0/xuance/configs/iql/sc2/MMM2.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-agent: "VDN"  # the learning algorithms_marl
-global_state: False
+agent: "IQL"  # the learning algorithms_marl
 env_name: "StarCraft2"
-env_id: "8m_vs_9m"
+env_id: "MMM2"
 fps: 15
-policy: "Mixing_Q_network"
+policy: "Basic_Q_network_marl"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
@@ -16,15 +15,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
@@ -40,9 +39,9 @@
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
 eval_interval: 100000
 test_episode: 16
-log_dir: "./logs/vdn/"
-model_dir: "./models/vdn/"
+log_dir: "./logs/iql/"
+model_dir: "./models/iql/"
```

### Comparing `xuance-1.0.9/xuance/configs/vdn/sc2/MMM2.yaml` & `xuance-1.1.0/xuance/configs/vdn/sc2/2s3z.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 agent: "VDN"  # the learning algorithms_marl
 global_state: False
 env_name: "StarCraft2"
-env_id: "MMM2"
+env_id: "2s3z"
 fps: 15
 policy: "Mixing_Q_network"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -16,33 +16,33 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
 decay_step_greedy: 50000
 start_training: 1000  # start training after n episodes
-running_steps: 10000000  # 1M
+running_steps: 2000000  # 2M
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 100000
+eval_interval: 20000
 test_episode: 16
 log_dir: "./logs/vdn/"
 model_dir: "./models/vdn/"
```

### Comparing `xuance-1.0.9/xuance/configs/vdn/sc2/corridor.yaml` & `xuance-1.1.0/xuance/configs/wqmix/sc2/MMM2.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-agent: "VDN"  # the learning algorithms_marl
-global_state: False
+agent: "OWQMIX"  # choice: CWQMIX, OWQMIX
 env_name: "StarCraft2"
-env_id: "corridor"
+env_id: "3m"
 fps: 15
-policy: "Mixing_Q_network"
+policy: "Weighted_Mixing_Q_network"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
 # recurrent settings for Basic_RNN representation
 use_recurrent: True
@@ -16,33 +15,39 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
+alpha: 0.1
+
+hidden_dim_mixing_net: 32  # hidden units of mixing network
+hidden_dim_hyper_net: 64  # hidden units of hyper network
+
+hidden_dim_ff_mix_net: 256  # hidden units of mixing network
 
 seed: 1
 parallels: 8
 buffer_size: 5000
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
-decay_step_greedy: 50000
+decay_step_greedy: 1000000
 start_training: 1000  # start training after n episodes
 running_steps: 10000000  # 10M
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
 eval_interval: 100000
 test_episode: 16
-log_dir: "./logs/vdn/"
-model_dir: "./models/vdn/"
+log_dir: "./logs/wqmix/"
+model_dir: "./models/wqmix/"
```

### Comparing `xuance-1.0.9/xuance/configs/wqmix/mpe/simple_spread_v3.yaml` & `xuance-1.1.0/xuance/configs/wqmix/sc2/8m.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 agent: "OWQMIX"  # choice: CWQMIX, OWQMIX
-env_name: "mpe"
-env_id: "simple_spread_v3"
-continuous_action: False
+env_name: "StarCraft2"
+env_id: "8m"
+fps: 15
 policy: "Weighted_Mixing_Q_network"
-representation: "Basic_MLP"
-vectorize: "Dummy_Pettingzoo"
-runner: "Pettingzoo_Runner"
+representation: "Basic_RNN"
+vectorize: "Subproc_StarCraft2"
+runner: "StarCraft2_Runner"
 on_policy: False
 
-use_recurrent: False
+# recurrent settings for Basic_RNN representation
+use_recurrent: True
 rnn: "GRU"
 recurrent_layer_N: 1
-fc_hidden_sizes: [ 64, ]
+fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
-representation_hidden_size: [128, ]  # for Basic_MLP representation
-q_hidden_size: [128, ]  # the units for each hidden layer
-activation: "ReLU"
+representation_hidden_size: [64, ]
+q_hidden_size: [64, ]  # the units for each hidden layer
+activation: "relu"
 alpha: 0.1
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
+
 hidden_dim_ff_mix_net: 256  # hidden units of mixing network
 
 seed: 1
-parallels: 16
-buffer_size: 100000
-batch_size: 256
-learning_rate: 0.001
+parallels: 8
+buffer_size: 5000
+batch_size: 32
+learning_rate: 0.0007
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
-decay_step_greedy: 5000000
+decay_step_greedy: 50000
 start_training: 1000  # start training after n episodes
-running_steps: 10000000  # 10M
+running_steps: 1000000  # 1M
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 100000
-test_episode: 5
+eval_interval: 10000
+test_episode: 16
 log_dir: "./logs/wqmix/"
 model_dir: "./models/wqmix/"
```

### Comparing `xuance-1.0.9/xuance/configs/wqmix/sc2/1c3s5z.yaml` & `xuance-1.1.0/xuance/configs/wqmix/sc2/2s3z.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "OWQMIX"  # choice: CWQMIX, OWQMIX
 env_name: "StarCraft2"
-env_id: "1c3s5z"
+env_id: "2s3z"
 fps: 15
 policy: "Weighted_Mixing_Q_network"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -15,15 +15,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 alpha: 0.1
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 hidden_dim_ff_mix_net: 256  # hidden units of mixing network
```

### Comparing `xuance-1.0.9/xuance/configs/wqmix/sc2/25m.yaml` & `xuance-1.1.0/xuance/configs/wqmix/sc2/25m.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 alpha: 0.1
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 hidden_dim_ff_mix_net: 256  # hidden units of mixing network
```

### Comparing `xuance-1.0.9/xuance/configs/wqmix/sc2/2m_vs_1z.yaml` & `xuance-1.1.0/xuance/configs/wqmix/sc2/5m_vs_6m.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "OWQMIX"  # choice: CWQMIX, OWQMIX
 env_name: "StarCraft2"
-env_id: "2m_vs_1z"
+env_id: "5m_vs_6m"
 fps: 15
 policy: "Weighted_Mixing_Q_network"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -15,15 +15,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 alpha: 0.1
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 hidden_dim_ff_mix_net: 256  # hidden units of mixing network
 
@@ -33,21 +33,21 @@
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
-decay_step_greedy: 50000
+decay_step_greedy: 1000000
 start_training: 1000  # start training after n episodes
-running_steps: 1000000  # 1M
+running_steps: 10000000  # 10M
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 10000
+eval_interval: 100000
 test_episode: 16
 log_dir: "./logs/wqmix/"
 model_dir: "./models/wqmix/"
```

### Comparing `xuance-1.0.9/xuance/configs/wqmix/sc2/2s3z.yaml` & `xuance-1.1.0/xuance/configs/wqmix/sc2/2m_vs_1z.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "OWQMIX"  # choice: CWQMIX, OWQMIX
 env_name: "StarCraft2"
-env_id: "2s3z"
+env_id: "2m_vs_1z"
 fps: 15
 policy: "Weighted_Mixing_Q_network"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -15,15 +15,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 alpha: 0.1
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 hidden_dim_ff_mix_net: 256  # hidden units of mixing network
 
@@ -35,19 +35,19 @@
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
 decay_step_greedy: 50000
 start_training: 1000  # start training after n episodes
-running_steps: 2000000  # 2M
+running_steps: 1000000  # 1M
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 20000
+eval_interval: 10000
 test_episode: 16
 log_dir: "./logs/wqmix/"
 model_dir: "./models/wqmix/"
```

### Comparing `xuance-1.0.9/xuance/configs/wqmix/sc2/3m.yaml` & `xuance-1.1.0/xuance/configs/wqmix/sc2/3m.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 alpha: 0.1
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 hidden_dim_ff_mix_net: 256  # hidden units of mixing network
```

### Comparing `xuance-1.0.9/xuance/configs/wqmix/sc2/5m_vs_6m.yaml` & `xuance-1.1.0/xuance/configs/wqmix/sc2/corridor.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "OWQMIX"  # choice: CWQMIX, OWQMIX
 env_name: "StarCraft2"
-env_id: "5m_vs_6m"
+env_id: "corridor"
 fps: 15
 policy: "Weighted_Mixing_Q_network"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -15,15 +15,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 alpha: 0.1
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 hidden_dim_ff_mix_net: 256  # hidden units of mixing network
```

### Comparing `xuance-1.0.9/xuance/configs/wqmix/sc2/8m.yaml` & `xuance-1.1.0/xuance/configs/wqmix/sc2/8m_vs_9m.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 agent: "OWQMIX"  # choice: CWQMIX, OWQMIX
 env_name: "StarCraft2"
-env_id: "8m"
+env_id: "8m_vs_9m"
 fps: 15
 policy: "Weighted_Mixing_Q_network"
 representation: "Basic_RNN"
 vectorize: "Subproc_StarCraft2"
 runner: "StarCraft2_Runner"
 on_policy: False
 
@@ -15,15 +15,15 @@
 fc_hidden_sizes: [64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+activation: "relu"
 alpha: 0.1
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
 
 hidden_dim_ff_mix_net: 256  # hidden units of mixing network
 
@@ -33,21 +33,21 @@
 batch_size: 32
 learning_rate: 0.0007
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
-decay_step_greedy: 50000
+decay_step_greedy: 1000000
 start_training: 1000  # start training after n episodes
-running_steps: 1000000  # 1M
+running_steps: 10000000  # 10M
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
-eval_interval: 10000
+eval_interval: 100000
 test_episode: 16
 log_dir: "./logs/wqmix/"
 model_dir: "./models/wqmix/"
```

### Comparing `xuance-1.0.9/xuance/configs/wqmix/sc2/8m_vs_9m.yaml` & `xuance-1.1.0/xuance/configs/wqmix/mpe/simple_spread_v3.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 agent: "OWQMIX"  # choice: CWQMIX, OWQMIX
-env_name: "StarCraft2"
-env_id: "8m_vs_9m"
-fps: 15
+env_name: "mpe"
+env_id: "simple_spread_v3"
+continuous_action: False
 policy: "Weighted_Mixing_Q_network"
-representation: "Basic_RNN"
-vectorize: "Subproc_StarCraft2"
-runner: "StarCraft2_Runner"
+representation: "Basic_MLP"
+vectorize: "Dummy_Pettingzoo"
+runner: "Pettingzoo_Runner"
 on_policy: False
 
-# recurrent settings for Basic_RNN representation
-use_recurrent: True
+use_recurrent: False
 rnn: "GRU"
 recurrent_layer_N: 1
-fc_hidden_sizes: [64, ]
+fc_hidden_sizes: [ 64, ]
 recurrent_hidden_size: 64
 N_recurrent_layers: 1
 dropout: 0
 
-representation_hidden_size: [64, ]
-q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
+representation_hidden_size: [128, ]  # for Basic_MLP representation
+q_hidden_size: [128, ]  # the units for each hidden layer
+activation: "relu"
 alpha: 0.1
 
 hidden_dim_mixing_net: 32  # hidden units of mixing network
 hidden_dim_hyper_net: 64  # hidden units of hyper network
-
 hidden_dim_ff_mix_net: 256  # hidden units of mixing network
 
 seed: 1
-parallels: 8
-buffer_size: 5000
-batch_size: 32
-learning_rate: 0.0007
+parallels: 16
+buffer_size: 100000
+batch_size: 256
+learning_rate: 0.001
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
-decay_step_greedy: 1000000
+decay_step_greedy: 5000000
 start_training: 1000  # start training after n episodes
 running_steps: 10000000  # 10M
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
 sync_frequency: 200
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
 eval_interval: 100000
-test_episode: 16
+test_episode: 5
 log_dir: "./logs/wqmix/"
 model_dir: "./models/wqmix/"
```

### Comparing `xuance-1.0.9/xuance/configs/wqmix/sc2/corridor.yaml` & `xuance-1.1.0/xuance/configs/vdn/new_env_mas.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,43 @@
-agent: "OWQMIX"  # choice: CWQMIX, OWQMIX
-env_name: "StarCraft2"
-env_id: "corridor"
-fps: 15
-policy: "Weighted_Mixing_Q_network"
-representation: "Basic_RNN"
-vectorize: "Subproc_StarCraft2"
-runner: "StarCraft2_Runner"
+agent: "VDN"  # the learning algorithms_marl
+env_name: "NewEnv_MAS"
+env_id: "scenarios_1"
+max_episode_steps: 200
+render: False
+sleep: 0.01
+continuous_action: False
+policy: "Mixing_Q_network"
+representation: "Basic_MLP"
+vectorize: "Dummy_NewEnv_MAS"
+runner: "MARL"
 on_policy: False
 
-# recurrent settings for Basic_RNN representation
-use_recurrent: True
-rnn: "GRU"
-recurrent_layer_N: 1
-fc_hidden_sizes: [64, ]
-recurrent_hidden_size: 64
-N_recurrent_layers: 1
-dropout: 0
-
+use_recurrent: False
+rnn:
 representation_hidden_size: [64, ]
 q_hidden_size: [64, ]  # the units for each hidden layer
-activation: "ReLU"
-alpha: 0.1
-
-hidden_dim_mixing_net: 32  # hidden units of mixing network
-hidden_dim_hyper_net: 64  # hidden units of hyper network
-
-hidden_dim_ff_mix_net: 256  # hidden units of mixing network
+activation: "relu"
 
 seed: 1
-parallels: 8
-buffer_size: 5000
-batch_size: 32
-learning_rate: 0.0007
+parallels: 16
+buffer_size: 100000
+batch_size: 256
+learning_rate: 0.001
 gamma: 0.99  # discount factor
 double_q: True  # use double q learning
 
 start_greedy: 1.0
 end_greedy: 0.05
-decay_step_greedy: 1000000
+decay_step_greedy: 2500000
 start_training: 1000  # start training after n episodes
 running_steps: 10000000  # 10M
 train_per_step: False  # True: train model per step; False: train model per episode.
 training_frequency: 1
-sync_frequency: 200
+sync_frequency: 100
 
 use_grad_clip: False
 grad_clip_norm: 0.5
 
 eval_interval: 100000
-test_episode: 16
-log_dir: "./logs/wqmix/"
-model_dir: "./models/wqmix/"
+test_episode: 5
+log_dir: "./logs/vdn/"
+model_dir: "./models/vdn/"
```

### Comparing `xuance-1.0.9/xuance/environment/__init__.py` & `xuance-1.1.0/xuance/environment/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 from argparse import Namespace
 
-from xuance.environment.gym.gym_env import Gym_Env, MountainCar
+from xuance.environment.gym import Gym_Env, MountainCar
 from .pettingzoo import PETTINGZOO_ENVIRONMENTS
 
 from .vector_envs.vector_env import VecEnv
-from xuance.environment.gym.gym_vec_env import DummyVecEnv_Gym, SubprocVecEnv_Gym
-from xuance.environment.gym.gym_vec_env import DummyVecEnv_Atari, SubprocVecEnv_Atari
-from xuance.environment.pettingzoo.pettingzoo_vec_env import DummyVecEnv_Pettingzoo, SubprocVecEnv_Pettingzoo
-from xuance.environment.magent2.magent_vec_env import DummyVecEnv_MAgent
-from xuance.environment.starcraft2.sc2_vec_env import DummyVecEnv_StarCraft2, SubprocVecEnv_StarCraft2
-from xuance.environment.football.gfootball_vec_env import DummyVecEnv_GFootball, SubprocVecEnv_GFootball
-from xuance.environment.minigrid.minigrid_vec_env import DummyVecEnv_MiniGrid, SubprocVecEnv_MiniGrid
-from xuance.environment.drones.drones_vec_env import DummyVecEnv_Drones, SubprocVecEnv_Drones
-from xuance.environment.new_env.new_vec_env import DummyVecEnv_New, SubprocVecEnv_New
+from xuance.environment.gym import DummyVecEnv_Gym, SubprocVecEnv_Gym
+from xuance.environment.gym import DummyVecEnv_Atari, SubprocVecEnv_Atari
+from xuance.environment.pettingzoo import DummyVecEnv_Pettingzoo, SubprocVecEnv_Pettingzoo
+from xuance.environment.starcraft2 import DummyVecEnv_StarCraft2, SubprocVecEnv_StarCraft2
+from xuance.environment.football import DummyVecEnv_GFootball, SubprocVecEnv_GFootball
+from xuance.environment.minigrid import DummyVecEnv_MiniGrid, SubprocVecEnv_MiniGrid
+from xuance.environment.drones import DummyVecEnv_Drones, SubprocVecEnv_Drones
+from xuance.environment.drones import DummyVecEnv_Drones_MAS, SubprocVecEnv_Drones_MAS
+from xuance.environment.metadrive import SubprocVecEnv_MetaDrive
+from xuance.environment.new_env import DummyVecEnv_New, SubprocVecEnv_New
+from xuance.environment.new_env_mas import DummyVecEnv_New_MAS, SubprocVecEnv_New_MAS
 
 from .vector_envs.subproc_vec_env import SubprocVecEnv
 
 REGISTRY_VEC_ENV = {
     "Dummy_Gym": DummyVecEnv_Gym,
     "Dummy_Pettingzoo": DummyVecEnv_Pettingzoo,
-    "Dummy_MAgent": DummyVecEnv_MAgent,
     "Dummy_StarCraft2": DummyVecEnv_StarCraft2,
     "Dummy_Football": DummyVecEnv_GFootball,
     "Dummy_Atari": DummyVecEnv_Atari,
-    "DummyVecEnv_MiniGrid": DummyVecEnv_MiniGrid,
-    "DummyVecEnv_Drone": DummyVecEnv_Drones,
+    "Dummy_MiniGrid": DummyVecEnv_MiniGrid,
+    "Dummy_Drone": DummyVecEnv_Drones,
+    "Dummy_Drone_MAS": DummyVecEnv_Drones_MAS,
     "Dummy_NewEnv": DummyVecEnv_New,  # Add the newly defined vectorized environment
-
+    "Dummy_NewEnv_MAS": DummyVecEnv_New_MAS,  # Add the newly defined vectorized environment for multi-agent systems
 
     # multiprocess #
     "Subproc_Gym": SubprocVecEnv_Gym,
     "Subproc_Pettingzoo": SubprocVecEnv_Pettingzoo,
     "Subproc_StarCraft2": SubprocVecEnv_StarCraft2,
     "Subproc_Football": SubprocVecEnv_GFootball,
     "Subproc_Atari": SubprocVecEnv_Atari,
-    "SubprocVecEnv_MiniGrid": SubprocVecEnv_MiniGrid,
-    "SubprocVecEnv_Drone": SubprocVecEnv_Drones,
+    "Subproc_MiniGrid": SubprocVecEnv_MiniGrid,
+    "Subproc_Drone": SubprocVecEnv_Drones,
+    "Subproc_Drone_MAS": SubprocVecEnv_Drones_MAS,
+    "Subproc_MetaDrive": SubprocVecEnv_MetaDrive,
     "Subproc_NewEnv": SubprocVecEnv_New,  # Add the newly defined vectorized environment
+    "Subproc_NewEnv_MAS": SubprocVecEnv_New_MAS,  # Add the newly defined vectorized environment for multi-agent systems
 }
 
 
 def make_envs(config: Namespace):
     def _thunk():
         if config.env_name in PETTINGZOO_ENVIRONMENTS:
             from xuance.environment.pettingzoo.pettingzoo_env import PettingZoo_Env
@@ -61,14 +66,18 @@
             env = MAgent_Env(config.env_id, config.seed,
                              minimap_mode=config.minimap_mode,
                              max_cycles=config.max_cycles,
                              extra_features=config.extra_features,
                              map_size=config.map_size,
                              render_mode=config.render_mode)
 
+        elif config.env_name == "Robotic_WareHouse":
+            from xuance.environment.robotic_warehouse.robotic_warehouse_env import RoboticWarehouseEnv
+            env = RoboticWarehouseEnv()
+
         elif config.env_name == "Atari":
             from xuance.environment.gym.gym_env import Atari_Env
             env = Atari_Env(config.env_id, config.seed, config.render_mode,
                             config.obs_type, config.frame_skip, config.num_stack, config.img_size, config.noop_max)
 
         elif config.env_id.__contains__("MountainCar"):
             env = MountainCar(config.env_id, config.seed, config.render_mode)
@@ -86,23 +95,37 @@
                               rgb_img_partial_obs_wrapper=config.RGBImgPartialObsWrapper,
                               img_obs_wrapper=config.ImgObsWrapper)
 
         elif config.env_name == "Drones":
             from xuance.environment.drones.drones_env import Drones_Env
             env = Drones_Env(config)
 
+        elif config.env_name == "MetaDrive":
+            from xuance.environment.metadrive.metadrive_env import MetaDrive_Env
+            env = MetaDrive_Env(config)
+
         elif config.env_name == "NewEnv":  # Add the newly defined vectorized environment
             from xuance.environment.new_env.new_env import New_Env
             env = New_Env(config.env_id, config.seed, continuous=False)
 
+        elif config.env_name == "NewEnv_MAS":  # Add the newly defined vectorized environment
+            from xuance.environment.new_env_mas.new_env_mas import New_Env_MAS
+            env = New_Env_MAS(config, continuous=config.continuous_action)
+
         else:
             env = Gym_Env(config.env_id, config.seed, config.render_mode)
 
         return env
 
+    if config.vectorize in ["Dummy_MAgent", "Subproc_MAgent"]:  # for the support of magent2 environment
+        from xuance.environment.magent2.magent_vec_env import DummyVecEnv_MAgent, SubprocVecEnv_Magent
+        REGISTRY_VEC_ENV.update({
+            "Dummy_MAgent": DummyVecEnv_MAgent,
+            "Subproc_MAgent": SubprocVecEnv_Magent
+        })
     if config.vectorize in REGISTRY_VEC_ENV.keys():
         return REGISTRY_VEC_ENV[config.vectorize]([_thunk for _ in range(config.parallels)])
     elif config.vectorize == "NOREQUIRED":
         return _thunk()
     else:
         raise NotImplementedError
```

### Comparing `xuance-1.0.9/xuance/environment/drones/drones_env.py` & `xuance-1.1.0/xuance/environment/new_env/new_env.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,48 @@
-from gym.spaces import Box
-
-
-class Drones_Env():
-    def __init__(self, args):
-        # import scenarios of gym-pybullet-drones
-        from gym_pybullet_drones.envs.CtrlAviary import CtrlAviary
-        from gym_pybullet_drones.envs.HoverAviary import HoverAviary
-        from gym_pybullet_drones.envs.VelocityAviary import VelocityAviary
-        REGISTRY = {
-            "CtrlAviary": CtrlAviary,
-            "HoverAviary": HoverAviary,
-            "VelocityAviary": VelocityAviary
-        }
-        continuous = args.continuous
-        self.env_id = args.env_id
-
-        from gym_pybullet_drones.utils.enums import DroneModel, Physics
-        self.env = REGISTRY[args.env_id](
-            drone_model=DroneModel.CF2X,
-            initial_xyzs=None,
-            initial_rpys=None,
-            physics=Physics.PYB,
-            pyb_freq=240,
-            ctrl_freq=240,
-            gui=args.render,
-            record=args.record
-        )
-        self._episode_step = 0
-        self._episode_score = 0.0
-        self.observation_space = self.space_reshape(self.env.observation_space)
-        self.action_space = self.space_reshape(self.env.action_space)
-        self.max_episode_steps = args.max_episode_steps
-
-    def space_reshape(self, gym_space):
-        low = gym_space.low.reshape(-1)
-        high = gym_space.high.reshape(-1)
-        shape_obs = (gym_space.shape[-1], )
-        return Box(low=low, high=high, shape=shape_obs, dtype=gym_space.dtype)
+"""
+This is an example of creating a new environment in XuanCe.
+"""
+from gym.spaces import Box, Discrete
+import numpy as np
+
+
+class New_Env:
+    def __init__(self, env_id: str, seed: int, *args, **kwargs):
+        continuous = kwargs['continuous']
+        self.env_id = env_id  # The name of the map or scenario that to be specified.
+        self._episode_step = 0  # The count of steps for current episode.
+        self._episode_score = 0.0  # The cumulated rewards for current episode.
+        self.observation_space = Box(low=0, high=1, shape=[8, ], dtype=np.float, seed=seed)
+        if continuous:
+            """For environment with continuous action space."""
+            self.action_space = Box(low=0, high=1, shape=[2, ], dtype=np.float, seed=seed)
+        else:
+            """For environment with discrete action space."""
+            self.action_space = Discrete(n=2, seed=seed)
+        self.max_episode_steps = 100  # The max steps for each episode.
 
     def close(self):
-        self.env.close()
+        """Close your environment here"""
+        pass
 
-    def render(self):
-        return self.env.render()
+    def render(self, *args, **kwargs):
+        """Render the environment, and return the images"""
+        return np.zeros([2, 2, 2])
 
     def reset(self):
-        obs, info = self.env.reset()
+        """Reset your environment, and return initialized observations and other information."""
+        obs, info = self.observation_space.sample(), {}  # reset the environment and get observations and info here.
         self._episode_step = 0
         self._episode_score = 0.0
         info["episode_step"] = self._episode_step
-        return obs.reshape(-1), info
+        return obs, info
 
     def step(self, actions):
-        observation, reward, terminated, truncated, info = self.env.step(actions.reshape([1, -1]))
+        """Execute the actions and get next observations, rewards, and other information."""
+        observation, reward, terminated, info = self.observation_space.sample(), 0, False, {}
+        truncated = True if (self._episode_step >= self.max_episode_steps) else False
 
         self._episode_step += 1
         self._episode_score += reward
         info["episode_step"] = self._episode_step  # current episode step
         info["episode_score"] = self._episode_score  # the accumulated rewards
-
-        truncated = True if (self._episode_step >= self.max_episode_steps) else False
-
-        return observation.reshape(-1), reward, terminated, truncated, info
-
-
+        return observation, reward, terminated, truncated, info
```

### Comparing `xuance-1.0.9/xuance/environment/football/__init__.py` & `xuance-1.1.0/xuance/environment/football/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,27 +14,8 @@
     - academy_3_vs_1_with_keeper: Three of our players try to score from the edge of the box, one on each side, and the other at the center. Initially, the player at the center has the ball and is facing the defender. There is an opponent keeper.
     - academy_corner: Standard corner-kick situation, except that the corner taker can run with the ball from the corner.
     - academy_counterattack_easy: 4 versus 1 counter-attack with keeper; all the remaining players of both teams run back towards the ball.
     - academy_counterattack_hard: 4 versus 2 counter-attack with keeper; all the remaining players of both teams run back towards the ball.
     - academy_single_goal_versus_lazy: Full 11 versus 11 games, where the opponents cannot move but they can only intercept the ball if it is close enough to them. Our center back defender has the ball at first.
 """
 
-GFOOTBALL_ENV_ID = {
-    "1v1": "1_vs_1_easy",
-    "5v5": "5_vs_5",
-    "11v11_competition": "11_vs_11_competition",
-    "11v11_kaggle": "11_vs_11_kaggle",
-    "11v11": "11_vs_11_stochastic",
-    "11v11_easy": "11_vs_11_easy_stochastic",
-    "11v11_hard": "11_vs_11_hard_stochastic",
-    "3v1": "academy_3_vs_1_with_keeper",
-    "corner": "academy_corner",
-    "ca_easy": "academy_counterattack_easy",
-    "ca_hard": "academy_counterattack_hard",
-    "eg": "academy_empty_goal",
-    "eg_close": "academy_empty_goal_close",
-    "psk": "academy_pass_and_shoot_with_keeper",
-    "rpsk": "academy_run_pass_and_shoot_with_keeper",
-    "rs": "academy_run_to_score",
-    "rsk": "academy_run_to_score_with_keeper",
-    "single_gvl": "academy_single_goal_versus_lazy",
-}
+from xuance.environment.football.gfootball_vec_env import SubprocVecEnv_GFootball, DummyVecEnv_GFootball
```

### Comparing `xuance-1.0.9/xuance/environment/football/gfootball_env.py` & `xuance-1.1.0/xuance/environment/football/gfootball_env.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,25 +28,25 @@
         elif isinstance(self.action_space, Discrete):
             self.dim_act = self.n_actions = self.action_space.n
         else:
             raise "Unsupported action spaces"
         self.max_cycles = self.env.unwrapped.observation()[0]['steps_left']
         self._episode_step = 0
         self._episode_score = 0.0
-        self.filled = np.zeros([self.max_cycles, 1], np.bool)
+        self.filled = np.zeros([self.max_cycles, 1], np.bool_)
         self.env.reset()
         state = self.get_state()
         self.dim_state = state.shape[0]
         self.dim_reward = self.n_agents
 
     def close(self):
         """Close the environment."""
         self.env.close()
 
-    def render(self):
+    def render(self, *args, **kwargs):
         """Get one-step frame."""
         return self.env.get_frame()
 
     def reset(self):
         """Reset the environment."""
         obs, info = self.env.reset()
         obs = obs.reshape([self.n_agents, -1])
```

### Comparing `xuance-1.0.9/xuance/environment/football/gfootball_vec_env.py` & `xuance-1.1.0/xuance/environment/football/gfootball_vec_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,32 +85,32 @@
         self.dim_obs, self.dim_state, self.dim_act = env_info["dim_obs"], env_info["dim_state"], env_info["dim_act"]
         self.dim_reward = env_info["dim_reward"]
         self.action_space = Discrete(n=self.dim_act)
         self.state_space = Box(low=-np.inf, high=np.inf, shape=[self.dim_state, ])
 
         self.buf_obs = np.zeros(combined_shape(self.num_envs, self.obs_shape), dtype=np.float32)
         self.buf_state = np.zeros(combined_shape(self.num_envs, self.dim_state), dtype=np.float32)
-        self.buf_terminal = np.zeros((self.num_envs, 1), dtype=np.bool)
-        self.buf_truncation = np.zeros((self.num_envs, 1), dtype=np.bool)
-        self.buf_done = np.zeros((self.num_envs,), dtype=np.bool)
+        self.buf_terminal = np.zeros((self.num_envs, 1), dtype=np.bool_)
+        self.buf_truncation = np.zeros((self.num_envs, 1), dtype=np.bool_)
+        self.buf_done = np.zeros((self.num_envs,), dtype=np.bool_)
         self.buf_rew = np.zeros((self.num_envs,) + self.rew_shape, dtype=np.float32)
         self.buf_info = [{} for _ in range(self.num_envs)]
         self.actions = None
         self.battles_game = np.zeros(self.num_envs, np.int32)
         self.battles_won = np.zeros(self.num_envs, np.int32)
         self.max_episode_length = env_info["max_cycles"]
 
     def reset(self):
         for remote in self.remotes:
             remote.send(('reset', None))
         result = [remote.recv() for remote in self.remotes]
         result = flatten_list(result)
         obs, state, infos = zip(*result)
         self.buf_obs, self.buf_state, self.buf_info = np.array(obs), np.array(state), list(infos)
-        self.buf_done = np.zeros((self.num_envs,), dtype=np.bool)
+        self.buf_done = np.zeros((self.num_envs,), dtype=np.bool_)
         return self.buf_obs.copy(), self.buf_state.copy(), self.buf_info.copy()
 
     def step_async(self, actions):
         self._assert_not_closed()
         actions = np.array_split(actions, self.n_remotes)
         for env_done, remote, action in zip(self.buf_done, self.remotes, actions):
             if not env_done:
@@ -155,15 +155,15 @@
         for pipe in self.remotes:
             pipe.send(('render', mode))
         imgs = [pipe.recv() for pipe in self.remotes]
         imgs = flatten_list(imgs)
         return imgs
 
     def get_avail_actions(self):
-        return np.ones([self.num_envs, self.num_agents, self.dim_act], dtype=np.bool)
+        return np.ones([self.num_envs, self.num_agents, self.dim_act], dtype=np.bool_)
 
     def _assert_not_closed(self):
         assert not self.closed, "Trying to operate on a SubprocVecEnv after calling close()"
 
     def __del__(self):
         if not self.closed:
             self.close()
@@ -186,30 +186,30 @@
         self.dim_obs, self.dim_state, self.dim_act = env.dim_obs, env.dim_state, env.dim_act
         self.dim_reward = env.dim_reward
         self.action_space = Discrete(n=self.dim_act)
         self.state_space = Box(low=-np.inf, high=np.inf, shape=[self.dim_state, ])
 
         self.buf_obs = np.zeros(combined_shape(self.num_envs, self.obs_shape), dtype=np.float32)
         self.buf_state = np.zeros(combined_shape(self.num_envs, self.dim_state), dtype=np.float32)
-        self.buf_terminal = np.zeros((self.num_envs, 1), dtype=np.bool)
-        self.buf_truncation = np.zeros((self.num_envs, 1), dtype=np.bool)
-        self.buf_done = np.zeros((self.num_envs, ), dtype=np.bool)
+        self.buf_terminal = np.zeros((self.num_envs, 1), dtype=np.bool_)
+        self.buf_truncation = np.zeros((self.num_envs, 1), dtype=np.bool_)
+        self.buf_done = np.zeros((self.num_envs, ), dtype=np.bool_)
         self.buf_rew = np.zeros((self.num_envs, ) + self.rew_shape, dtype=np.float32)
         self.buf_info = [{} for _ in range(self.num_envs)]
         self.actions = None
         self.battles_game = np.zeros(self.num_envs, np.int32)
         self.battles_won = np.zeros(self.num_envs, np.int32)
         self.max_episode_length = env.max_cycles
 
     def reset(self):
         for i_env, env in enumerate(self.envs):
             obs, state, infos = env.reset()
             self.buf_obs[i_env], self.buf_state[i_env] = np.array(obs), np.array(state)
             self.buf_info[i_env] = infos
-        self.buf_done = np.zeros((self.num_envs,), dtype=np.bool)
+        self.buf_done = np.zeros((self.num_envs,), dtype=np.bool_)
         return self.buf_obs.copy(), self.buf_state.copy(), self.buf_info.copy()
 
     def step_async(self, actions):
         self.actions = actions
         self.waiting = True
 
     def step_wait(self):
@@ -234,11 +234,11 @@
 
     def close_extras(self):
         self.closed = True
         for env in self.envs:
             env.close()
 
     def render(self, mode):
-        return [env.render() for env in self.envs]
+        return [env.render(mode) for env in self.envs]
 
     def get_avail_actions(self):
-        return np.ones([self.num_envs, self.num_agents, self.dim_act], dtype=np.bool)
+        return np.ones([self.num_envs, self.num_agents, self.dim_act], dtype=np.bool_)
```

### Comparing `xuance-1.0.9/xuance/environment/football/raw_env.py` & `xuance-1.1.0/xuance/environment/football/raw_env.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 import gfootball.env as football_env
-from . import GFOOTBALL_ENV_ID
 from gfootball.env.football_env import FootballEnv
 from gfootball.env import config
-from gfootball.env.wrappers import Simple115StateWrapper
 import numpy as np
 
+GFOOTBALL_ENV_ID = {
+    "1v1": "1_vs_1_easy",
+    "5v5": "5_vs_5",
+    "11v11_competition": "11_vs_11_competition",
+    "11v11_kaggle": "11_vs_11_kaggle",
+    "11v11": "11_vs_11_stochastic",
+    "11v11_easy": "11_vs_11_easy_stochastic",
+    "11v11_hard": "11_vs_11_hard_stochastic",
+    "3v1": "academy_3_vs_1_with_keeper",
+    "corner": "academy_corner",
+    "ca_easy": "academy_counterattack_easy",
+    "ca_hard": "academy_counterattack_hard",
+    "eg": "academy_empty_goal",
+    "eg_close": "academy_empty_goal_close",
+    "psk": "academy_pass_and_shoot_with_keeper",
+    "rpsk": "academy_run_pass_and_shoot_with_keeper",
+    "rs": "academy_run_to_score",
+    "rsk": "academy_run_to_score_with_keeper",
+    "single_gvl": "academy_single_goal_versus_lazy",
+}
+
 
 class football_raw_env(FootballEnv):
     def __init__(self, args):
         write_goal_dumps = False
         dump_frequency = 1
         extra_players = None
         other_config_options = {}
@@ -29,15 +48,15 @@
             representation=args.obs_type,
             rewards=args.rewards_type,
             write_goal_dumps=write_goal_dumps,
             write_full_episode_dumps=write_full_episode_dumps,
             render=self.render,
             write_video=write_video,
             dump_frequency=dump_frequency,
-            log_dir=args.videos_dir,
+            logdir=args.videos_dir,
             extra_players=extra_players,
             number_of_left_players_agent_controls=args.num_agent,
             number_of_right_players_agent_controls=args.num_adversary,
             channel_dimensions=(args.smm_width, args.smm_height),
             other_config_options=other_config_options
         ).unwrapped
```

### Comparing `xuance-1.0.9/xuance/environment/gym/gym_env.py` & `xuance-1.1.0/xuance/environment/gym/gym_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/gym/gym_vec_env.py` & `xuance-1.1.0/xuance/environment/gym/gym_vec_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,16 @@
 
         self.obs_shape = space2shape(self.observation_space)
         if isinstance(self.observation_space, Dict):
             self.buf_obs = {k: np.zeros(combined_shape(self.num_envs, v)) for k, v in
                             zip(self.obs_shape.keys(), self.obs_shape.values())}
         else:
             self.buf_obs = np.zeros(combined_shape(self.num_envs, self.obs_shape), dtype=np.float32)
-        self.buf_dones = np.zeros((self.num_envs,), dtype=np.bool)
-        self.buf_trunctions = np.zeros((self.num_envs,), dtype=np.bool)
+        self.buf_dones = np.zeros((self.num_envs,), dtype=np.bool_)
+        self.buf_trunctions = np.zeros((self.num_envs,), dtype=np.bool_)
         self.buf_rews = np.zeros((self.num_envs,), dtype=np.float32)
         self.buf_infos = [{} for _ in range(self.num_envs)]
         self.actions = None
         self.remotes[0].send(('get_max_cycles', None))
         self.max_episode_length = self.remotes[0].recv().x
 
     def step_async(self, actions):
@@ -113,14 +113,15 @@
         self._assert_not_closed()
         for remote in self.remotes:
             remote.send(('reset', None))
         result = [remote.recv() for remote in self.remotes]
         result = flatten_list(result)
         obs, infos = zip(*result)
         self.buf_obs, self.buf_infos = np.array(obs), list(infos)
+        self.buf_dones = np.zeros((self.num_envs,), dtype=np.bool_)
         return self.buf_obs.copy(), self.buf_infos.copy()
 
     def close_extras(self):
         self.closed = True
         if self.waiting:
             for remote in self.remotes:
                 remote.recv()
@@ -160,16 +161,16 @@
         VecEnv.__init__(self, len(env_fns), env.observation_space, env.action_space)
         self.obs_shape = space2shape(self.observation_space)
         if isinstance(self.observation_space, Dict):
             self.buf_obs = {k: np.zeros(combined_shape(self.num_envs, v)) for k, v in
                             zip(self.obs_shape.keys(), self.obs_shape.values())}
         else:
             self.buf_obs = np.zeros(combined_shape(self.num_envs, self.obs_shape), dtype=np.float32)
-        self.buf_dones = np.zeros((self.num_envs,), dtype=np.bool)
-        self.buf_trunctions = np.zeros((self.num_envs,), dtype=np.bool)
+        self.buf_dones = np.zeros((self.num_envs,), dtype=np.bool_)
+        self.buf_trunctions = np.zeros((self.num_envs,), dtype=np.bool_)
         self.buf_rews = np.zeros((self.num_envs,), dtype=np.float32)
         self.buf_infos = [{} for _ in range(self.num_envs)]
         self.actions = None
         try:
             self.max_episode_length = env.max_episode_steps
         except AttributeError:
             self.max_episode_length=1000
```

### Comparing `xuance-1.0.9/xuance/environment/gym_platform/envs/platform_env.py` & `xuance-1.1.0/xuance/environment/gym_platform/envs/platform_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/builtin/config/battle.py` & `xuance-1.1.0/xuance/environment/magent2/builtin/config/battle.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/builtin/config/double_attack.py` & `xuance-1.1.0/xuance/environment/magent2/builtin/config/double_attack.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/builtin/config/forest.py` & `xuance-1.1.0/xuance/environment/magent2/builtin/config/forest.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/builtin/config/pursuit.py` & `xuance-1.1.0/xuance/environment/magent2/builtin/config/pursuit.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/c_lib.py` & `xuance-1.1.0/xuance/environment/magent2/c_lib.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/environment.py` & `xuance-1.1.0/xuance/environment/magent2/environment.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/environments/adversarial_pursuit/adversarial_pursuit.py` & `xuance-1.1.0/xuance/environment/magent2/environments/adversarial_pursuit/adversarial_pursuit.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/environments/battle/battle.py` & `xuance-1.1.0/xuance/environment/magent2/environments/battle/battle.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/environments/battlefield/battlefield.py` & `xuance-1.1.0/xuance/environment/magent2/environments/battlefield/battlefield.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/environments/combined_arms/combined_arms.py` & `xuance-1.1.0/xuance/environment/magent2/environments/combined_arms/combined_arms.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/environments/gather/gather.py` & `xuance-1.1.0/xuance/environment/magent2/environments/gather/gather.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/environments/magent_env.py` & `xuance-1.1.0/xuance/environment/magent2/environments/magent_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/environments/tiger_deer/tiger_deer.py` & `xuance-1.1.0/xuance/environment/magent2/environments/tiger_deer/tiger_deer.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/gridworld.py` & `xuance-1.1.0/xuance/environment/magent2/gridworld.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/libmagent.dylib` & `xuance-1.1.0/xuance/environment/magent2/libmagent.dylib`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/libmagent.so` & `xuance-1.1.0/xuance/environment/magent2/libmagent.so`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/magent.dll` & `xuance-1.1.0/xuance/environment/magent2/magent.dll`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/magent_env.py` & `xuance-1.1.0/xuance/environment/magent2/magent_env.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+import numpy as np
 from pettingzoo.utils.env import ParallelEnv
 from xuance.environment.pettingzoo.pettingzoo_env import PettingZoo_Env
 from xuance.environment.magent2 import AGENT_NAME_DICT
 import importlib
+from gymnasium.spaces.box import Box
 
 
 class MAgent_Env(PettingZoo_Env, ParallelEnv):
     metadata = {"render_modes": ["human"], "name": "rps_v2"}
+
     def __init__(self, env_id: str, seed: int, **kwargs):
         scenario = importlib.import_module('xuance.environment.magent2.environments.' + env_id)
 
         if env_id in ["adversarial_pursuit_v4"]:
             kwargs['minimap_mode'] = False
             kwargs['tag_penalty'] = -0.2
         if env_id in ["battle_v4", "battlefield_v4", "combined_arms_v6"]:
             kwargs['step_reward'] = -0.005
             kwargs['dead_penalty'] = -0.1
-            kwargs['attack_peanlty'] = -0.1
+            kwargs['attack_penalty'] = -0.1
             kwargs['attack_opponent_reward'] = 0.2
         if env_id in ["gather_v4"]:
             kwargs['step_reward'] = -0.01
             kwargs['dead_penalty'] = -1
             kwargs['attack_peanlty'] = -0.1
             kwargs['attack_food_reward'] = 0.5
         if env_id in ["tiger_deer_v3"]:
@@ -29,16 +32,21 @@
         self.env = scenario.env(**kwargs).unwrapped
         self.scenario_name = 'magent2.' + env_id
         self.n_handles = len(self.env.handles)
         self.side_names = AGENT_NAME_DICT[env_id]
         self.env.reset(seed)
 
         self.state_space = self.env.state_space
+        self.observation_spaces = {}
+        for k in self.env.agents:
+            obs_space = self.env.observation_spaces[k]
+            self.observation_spaces.update({
+                k: Box(np.min(obs_space.low), np.max(obs_space.high), [np.prod(obs_space.shape)], obs_space.dtype, seed)
+            })
         self.action_spaces = {k: self.env.action_spaces[k] for k in self.env.agents}
-        self.observation_spaces = {k: self.env.observation_spaces[k] for k in self.env.agents}
         self.agents = self.env.agents
         self.n_agents_all = len(self.agents)
 
         self.handles = self.env.handles
 
         self.agent_ids = [self.env.env.get_agent_id(h) for h in self.handles]
         self.n_agents = [self.env.env.get_num(h) for h in self.handles]
@@ -62,9 +70,7 @@
         observations, rewards, terminations, truncations, infos = self.env.step(actions)
         for k, v in rewards.items():
             self.individual_episode_reward[k] += v
             observations[k] = observations[k].reshape([-1])
         step_info = {"infos": infos,
                      "individual_episode_rewards": self.individual_episode_reward}
         return observations, rewards, terminations, truncations, step_info
-
-
```

### Comparing `xuance-1.0.9/xuance/environment/magent2/magent_vec_env.py` & `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/pg_agent.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,165 +1,147 @@
-import copy
+from xuance.mindspore.agents import *
 
-from xuance.environment.vector_envs.vector_env import VecEnv, AlreadySteppingError, NotSteppingError
-from xuance.environment.vector_envs.env_utils import obs_n_space_info
-from xuance.environment.pettingzoo.pettingzoo_vec_env import DummyVecEnv_Pettingzoo
-from operator import itemgetter
-import numpy as np
-import time
-
-
-class DummyVecEnv_MAgent(DummyVecEnv_Pettingzoo):
-    def __init__(self, env_fns):
-        self.waiting = False
-        self.envs = [fn() for fn in env_fns]
-        env = self.envs[0]
-        self.handles = env.handles
-        VecEnv.__init__(self, len(env_fns), env.observation_spaces, env.action_spaces)
-        self.state_space = env.state_space
-        self.state_shape = self.state_space.shape
-        self.state_dtype = self.state_space.dtype
-        obs_n_space = env.observation_spaces  # [Box(dim_o), Box(dim_o), ...] ----> dict
-        self.agent_ids = env.agent_ids
-        self.n_agents = [env.get_num(h) for h in self.handles]
-        self.side_names = env.side_names
-
-        self.keys, self.shapes, self.dtypes = obs_n_space_info(obs_n_space)
-        self.agent_keys = [[self.keys[k] for k in ids] for ids in self.agent_ids]
-        self.n_agent_all = len(self.keys)
-        # max_obs_shape = self._get_max_obs_shape(self.keys, self.observation_space)
-        self.obs_shapes = [self.shapes[self.agent_keys[h.value][0]] for h in self.handles]
-        self.obs_dtype = self.dtypes[self.keys[0]]
-
-        # buffer of dict data
-        self.buf_obs_dict = [{k: np.zeros(tuple(self.shapes[k]), dtype=self.dtypes[k]) for k in self.keys} for _ in
-                             range(self.num_envs)]
-        self.buf_rews_dict = [{k: 0.0 for k in self.keys} for _ in range(self.num_envs)]
-        self.buf_dones_dict = [{k: False for k in self.keys} for _ in range(self.num_envs)]
-        self.buf_trunctions_dict = [{k: False for k in self.keys} for _ in range(self.num_envs)]
-        self.buf_infos_dict = [{} for _ in range(self.num_envs)]
-        # buffer of numpy data
-        self.buf_state = np.zeros((self.num_envs,) + self.state_shape, dtype=self.state_dtype)
-        self.buf_agent_mask = [np.ones([self.num_envs, n], dtype=np.bool) for n in self.n_agents]
-        self.buf_obs = [np.zeros((self.num_envs, n, np.prod(self.obs_shapes[h])), dtype=self.obs_dtype) for h, n in
-                        enumerate(self.n_agents)]
-        self.buf_rews = [np.zeros((self.num_envs, n, 1), dtype=np.float32) for n in self.n_agents]
-        self.buf_dones = [np.ones((self.num_envs, n), dtype=np.bool) for n in self.n_agents]
-        self.buf_trunctions = [np.ones((self.num_envs, n), dtype=np.bool) for n in self.n_agents]
-
-        self.max_episode_length = env.max_cycles
-        self.actions = None
-
-    def empty_dict_buffers(self, i_env):
-        # buffer of dict data
-        self.buf_obs_dict[i_env] = {k: np.zeros(tuple(self.shapes[k]), dtype=self.dtypes[k]) for k in self.keys}
-        self.buf_rews_dict[i_env] = {k: 0.0 for k in self.keys}
-        self.buf_dones_dict[i_env] = {k: False for k in self.keys}
-        self.buf_trunctions_dict[i_env] = {k: False for k in self.keys}
-        self.buf_infos_dict[i_env] = {k: {} for k in self.keys}
-
-    def reset(self):
-        for e in range(self.num_envs):
-            obs, info = self.envs[e].reset()
-            self.buf_obs_dict[e].update(obs)
-            self.buf_infos_dict[e].update(info["infos"])
-            for h, agent_keys_h in enumerate(self.agent_keys):
-                self.buf_obs[h][e] = itemgetter(*agent_keys_h)(self.buf_obs_dict[e])
-        return self.buf_obs.copy(), self.buf_infos_dict.copy()
-
-    def reset_one_env(self, e):
-        o = self.envs[e].reset()
-        self.buf_obs_dict[e].update(o)
-        obs_e = []
-        for h, agent_keys_h in enumerate(self.agent_keys):
-            self.buf_obs[h][e] = itemgetter(*agent_keys_h)(self.buf_obs_dict[e])
-            obs_e.append(self.buf_obs[h][e])
-
-        return obs_e
-
-    def _get_max_obs_shape(self, k, observation_shape):
-        obs_shape_n = itemgetter(*list(k))(observation_shape)
-        size_obs_n = []
-        for shape in obs_shape_n:
-            size_obs_n.append(shape.shape)
-        return max(size_obs_n)
-
-    def step_async(self, actions):
-        if self.waiting:
-            raise AlreadySteppingError
-        listify = True
-        try:
-            if len(actions) == self.num_envs:
-                listify = False
-        except TypeError:
-            pass
-        if not listify:
-            self.actions = actions
-        else:
-            assert self.num_envs == 1, "actions {} is either not a list or has a wrong size - cannot match to {} environments".format(
-                actions, self.num_envs)
-            self.actions = [actions]
-        self.waiting = True
-
-    def step_wait(self):
-        if not self.waiting:
-            raise NotSteppingError
-
-        for e in range(self.num_envs):
-            action_n = self.actions[e]
-            o, r, d, t, info = self.envs[e].step(action_n)
-            if len(o.keys()) < self.n_agent_all:
-                self.empty_dict_buffers(e)
-            # update the data of alive agents
-            self.buf_obs_dict[e].update(o)
-            self.buf_rews_dict[e].update(r)
-            self.buf_dones_dict[e].update(d)
-            self.buf_trunctions_dict[e].update(t)
-            self.buf_infos_dict[e].update(info["infos"])
-
-            # resort the data as group-wise
-            episode_scores = []
-            mask = self.envs[e].get_agent_mask()
-            for h, agent_keys_h in enumerate(self.agent_keys):
-                getter = itemgetter(*agent_keys_h)
-                self.buf_agent_mask[h][e] = mask[self.agent_ids[h]]
-                self.buf_obs[h][e] = getter(self.buf_obs_dict[e])
-                self.buf_rews[h][e, :, 0] = getter(self.buf_rews_dict[e])
-                self.buf_dones[h][e] = getter(self.buf_dones_dict[e])
-                self.buf_trunctions[h][e] = getter(self.buf_trunctions_dict[e])
-                episode_scores.append(getter(info["individual_episode_rewards"]))
-            self.buf_infos_dict[e]["individual_episode_rewards"] = episode_scores
-
-            if all(self.buf_dones_dict[e].values()) or all(self.buf_trunctions_dict[e].values()):
-                obs_reset, _ = self.envs[e].reset()
-                state_reset = self.envs[e].state()
-                mask_reset = self.envs[e].get_agent_mask()
-                obs_reset_handles, mask_reset_handles = [], []
-                for h, agent_keys_h in enumerate(self.agent_keys):
-                    getter = itemgetter(*agent_keys_h)
-                    obs_reset_handles.append(np.array(getter(obs_reset)))
-                    mask_reset_handles.append(mask_reset[self.agent_ids[h]])
-
-                self.buf_infos_dict[e]["reset_obs"] = obs_reset_handles
-                self.buf_infos_dict[e]["reset_agent_mask"] = mask_reset_handles
-                self.buf_infos_dict[e]["reset_state"] = state_reset
-
-        self.waiting = False
-        return self.buf_obs.copy(), self.buf_rews.copy(), self.buf_dones.copy(), self.buf_trunctions.copy(), self.buf_infos_dict.copy()
-
-    def render(self, mode=None):
-        return [env.render() for env in self.envs]
-
-    def global_state(self):
-        return np.array([env.state() for env in self.envs])
-
-    def global_state_one_env(self, e):
-        return np.array(self.envs[e].state())
-
-    def agent_mask(self):
-        agent_mask = [np.ones([self.num_envs, n], dtype=np.bool) for n in self.n_agents]
-        for e, env in enumerate(self.envs):
-            mask = env.get_agent_mask()
-            for h, ids in enumerate(self.agent_ids):
-                agent_mask[h][e] = mask[ids]
 
-        return agent_mask
+class PG_Agent(Agent):
+    def __init__(self,
+                 config: Namespace,
+                 envs: DummyVecEnv_Gym,
+                 policy: nn.Cell,
+                 optimizer: nn.Optimizer,
+                 scheduler):
+        self.render = config.render
+        self.n_envs = envs.num_envs
+        self.n_steps = config.n_steps
+        self.n_minibatch = config.n_minibatch
+        self.n_epoch = config.n_epoch
+
+        self.gamma = config.gamma
+        self.gae_lam = config.gae_lambda
+        self.clip_grad = config.clip_grad
+        self.observation_space = envs.observation_space
+        self.action_space = envs.action_space
+        self.representation_info_shape = policy.representation.output_shapes
+        self.auxiliary_info_shape = {}
+        self.atari = True if config.env_name == "Atari" else False
+        Buffer = DummyOnPolicyBuffer_Atari if self.atari else DummyOnPolicyBuffer
+        self.buffer_size = self.n_envs * self.n_steps
+        self.batch_size = self.buffer_size // self.n_epoch
+        memory = Buffer(self.observation_space,
+                        self.action_space,
+                        self.auxiliary_info_shape,
+                        self.n_envs,
+                        self.n_steps,
+                        config.use_gae,
+                        config.use_advnorm,
+                        self.gamma,
+                        self.gae_lam)
+        learner = PG_Learner(policy,
+                             optimizer,
+                             scheduler,
+                             config.model_dir,
+                             config.ent_coef,
+                             config.clip_grad,
+                             config.clip_type)
+        super(PG_Agent, self).__init__(config, envs, policy, memory, learner, config.log_dir, config.model_dir)
+
+    def _action(self, obs):
+        _, act_probs = self.policy(ms.Tensor(obs))
+        acts = self.policy.actor.sample(act_probs).asnumpy()
+        return acts
+
+    def train(self, train_steps):
+        obs = self.envs.buf_obs
+        for _ in tqdm(range(train_steps)):
+            step_info = {}
+            self.obs_rms.update(obs)
+            obs = self._process_observation(obs)
+            acts = self._action(obs)
+            next_obs, rewards, terminals, trunctions, infos = self.envs.step(acts)
+            self.memory.store(obs, acts, self._process_reward(rewards), 0, terminals)
+            if self.memory.full:
+                for i in range(self.n_envs):
+                    self.memory.finish_path(self._process_reward(rewards)[i], i)
+                indexes = np.arange(self.buffer_size)
+                for _ in range(self.n_epoch):
+                    np.random.shuffle(indexes)
+                    for start in range(0, self.buffer_size, self.batch_size):
+                        end = start + self.batch_size
+                        sample_idx = indexes[start:end]
+                        obs_batch, act_batch, ret_batch, _, _, _ = self.memory.sample(sample_idx)
+                        step_info = self.learner.update(obs_batch, act_batch, ret_batch)
+                self.log_infos(step_info, self.current_step)
+                self.memory.clear()
+
+            self.returns = self.gamma * self.returns + rewards
+            obs = next_obs
+            for i in range(self.n_envs):
+                if terminals[i] or trunctions[i]:
+                    self.ret_rms.update(self.returns[i:i + 1])
+                    self.returns[i] = 0.0
+                    if self.atari and (~trunctions[i]):
+                        pass
+                    else:
+                        obs[i] = infos[i]["reset_obs"]
+                        self.memory.finish_path(0, i)
+                        self.current_episode[i] += 1
+                        if self.use_wandb:
+                            step_info["Episode-Steps/env-%d" % i] = infos[i]["episode_step"]
+                            step_info["Train-Episode-Rewards/env-%d" % i] = infos[i]["episode_score"]
+                        else:
+                            step_info["Episode-Steps"] = {"env-%d" % i: infos[i]["episode_step"]}
+                            step_info["Train-Episode-Rewards"] = {"env-%d" % i: infos[i]["episode_score"]}
+                        self.log_infos(step_info, self.current_step)
+            self.current_step += self.n_envs
+
+    def test(self, env_fn, test_episodes):
+        test_envs = env_fn()
+        num_envs = test_envs.num_envs
+        videos, episode_videos = [[] for _ in range(num_envs)], []
+        current_episode, scores, best_score = 0, [], -np.inf
+        obs, infos = test_envs.reset()
+        if self.config.render_mode == "rgb_array" and self.render:
+            images = test_envs.render(self.config.render_mode)
+            for idx, img in enumerate(images):
+                videos[idx].append(img)
+
+        while current_episode < test_episodes:
+            self.obs_rms.update(obs)
+            obs = self._process_observation(obs)
+            acts = self._action(obs)
+            next_obs, rewards, terminals, trunctions, infos = test_envs.step(acts)
+            if self.config.render_mode == "rgb_array" and self.render:
+                images = test_envs.render(self.config.render_mode)
+                for idx, img in enumerate(images):
+                    videos[idx].append(img)
+
+            obs = next_obs
+            for i in range(num_envs):
+                if terminals[i] or trunctions[i]:
+                    if self.atari and (~trunctions[i]):
+                        pass
+                    else:
+                        obs[i] = infos[i]["reset_obs"]
+                        scores.append(infos[i]["episode_score"])
+                        current_episode += 1
+                        if best_score < infos[i]["episode_score"]:
+                            best_score = infos[i]["episode_score"]
+                            episode_videos = videos[i].copy()
+                        if self.config.test_mode:
+                            print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
+
+        if self.config.render_mode == "rgb_array" and self.render:
+            # time, height, width, channel -> time, channel, height, width
+            videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
+
+        if self.config.test_mode:
+            print("Best Score: %.2f" % (best_score))
+
+        test_info = {
+            "Test-Episode-Rewards/Mean-Score": np.mean(scores),
+            "Test-Episode-Rewards/Std-Score": np.std(scores)
+        }
+        self.log_infos(test_info, self.current_step)
+
+        test_envs.close()
+
+        return scores
```

### Comparing `xuance-1.0.9/xuance/environment/magent2/render.py` & `xuance-1.1.0/xuance/environment/magent2/render.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/magent2/utility.py` & `xuance-1.1.0/xuance/environment/magent2/utility.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/minigrid/minigrid_env.py` & `xuance-1.1.0/xuance/environment/minigrid/minigrid_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/minigrid/minigrid_vec_env.py` & `xuance-1.1.0/xuance/environment/minigrid/minigrid_vec_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from xuance.environment.gym.gym_vec_env import SubprocVecEnv_Gym, DummyVecEnv_Gym, worker
+from xuance.environment.gym.gym_vec_env import SubprocVecEnv_Gym, DummyVecEnv_Gym
 
 
 class SubprocVecEnv_MiniGrid(SubprocVecEnv_Gym):
     """
     VecEnv that runs multiple environments in parallel in subproceses and communicates with them via pipes.
     Recommended to use when num_envs > 1 and step() can be a bottleneck.
     """
```

### Comparing `xuance-1.0.9/xuance/environment/new_env/new_env.py` & `xuance-1.1.0/xuance/environment/metadrive/metadrive_env.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-"""
-This is an example of creating a new environment in XuanCe.
-"""
-from gym.spaces import Box, Discrete
+from metadrive.envs.metadrive_env import MetaDriveEnv
 import numpy as np
 
 
-class New_Env:
-    def __init__(self, env_id: str, seed: int, *args, **kwargs):
-        continuous = kwargs['continuous']
-        self.env_id = env_id
-        self._episode_step = 0
-        self._episode_score = 0.0
-        self.observation_space = Box(low=0, high=1, shape=[8, ], dtype=np.float, seed=seed)
-        if continuous:
-            self.action_space = Box(low=0, high=1, shape=[2, ], dtype=np.float, seed=seed)
-        else:
-            self.action_space = Discrete(n=2, seed=seed)
-        self.max_episode_steps = 100
+class MetaDrive_Env:
+    def __init__(self, args):
+        self.env_id = args.env_id
+        args.env_config['use_render'] = args.render
+        self.env = MetaDriveEnv(config=args.env_config)
+
+        self._episode_step = 0  # The count of steps for current episode.
+        self._episode_score = 0.0  # The cumulated rewards for current episode.
+        self.observation_space = self.env.observation_space
+        self.action_space = self.env.action_space
+        self.max_episode_steps = self.env.episode_lengths
 
     def close(self):
-        pass
+        self.env.close()
 
-    def render(self):
-        pass
+    def render(self, *args, **kwargs):
+        return np.zeros([2, 2, 2])
 
     def reset(self):
-        obs, info = self.observation_space.sample(), {}  # reset the environment and get observations and info here.
-        self._episode_step = 0
-        self._episode_score = 0.0
+        obs, info = self.env.reset()
+        self._episode_step = 0  # The count of steps for current episode.
+        self._episode_score = 0.0  # The cumulated rewards for current episode.
         info["episode_step"] = self._episode_step
         return obs, info
 
     def step(self, actions):
-        # Execute the actions and get next observations, rewards, and other information.
-        observation, reward, terminated, truncated, info = self.observation_space.sample(), 0, False, False, {}
+        observation, reward, terminated, truncated, info = self.env.step(actions)
 
         self._episode_step += 1
         self._episode_score += reward
         info["episode_step"] = self._episode_step  # current episode step
         info["episode_score"] = self._episode_score  # the accumulated rewards
         return observation, reward, terminated, truncated, info
```

### Comparing `xuance-1.0.9/xuance/environment/new_env/new_vec_env.py` & `xuance-1.1.0/xuance/environment/new_env/new_vec_env.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/environment/pettingzoo/pettingzoo_env.py` & `xuance-1.1.0/xuance/environment/drones/drones_env.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,109 @@
-from pettingzoo.utils.env import ParallelEnv
 import numpy as np
-import ctypes
-import importlib
-from xuance.environment.pettingzoo import AGENT_NAME_DICT
-
-
-class PettingZoo_Env(ParallelEnv):
-    def __init__(self, env_name: str, env_id: str, seed: int, **kwargs):
-        super(PettingZoo_Env, self).__init__()
-        scenario = importlib.import_module('pettingzoo.' + env_name + '.' + env_id)
-        self.continuous_actions = kwargs["continuous"]
-        self.env = scenario.parallel_env(continuous_actions=self.continuous_actions,
-                                         render_mode=kwargs["render_mode"])
-        self.scenario_name = env_name + "." + env_id
-        self.n_handles = len(AGENT_NAME_DICT[self.scenario_name])
-        self.side_names = AGENT_NAME_DICT[self.scenario_name]
-        self.env.reset()
-        try:
-            self.state_space = self.env.state_space
-        except:
-            self.state_space = None
-
-        self.action_spaces = {k: self.env.action_space(k) for k in self.env.agents}
-        self.observation_spaces = {k: self.env.observation_space(k) for k in self.env.agents}
-        self.agents = self.env.agents
-        self.n_agents_all = len(self.agents)
-
-        self.handles = self.get_handles()
-
-        self.agent_ids = [self.get_ids(h) for h in self.handles]
-        self.n_agents = [self.get_num(h) for h in self.handles]
-
-        # self.reward_range = env.reward_range
-        self.metadata = self.env.metadata
-        # self._warn_double_wrap()
-        # assert self.spec.id in ENVIRONMENTS
-
-        self.max_cycles = self.env.aec_env.env.env.max_cycles
-        self.individual_episode_reward = {k: 0.0 for k in self.agents}
+from gym.spaces import Box
+import time
+from gym_pybullet_drones.envs.CtrlAviary import CtrlAviary
+from xuance.environment.drones.customized.HoverAviary import HoverAviary
+from gym_pybullet_drones.envs.VelocityAviary import VelocityAviary
+from xuance.environment.drones.customized.MultiHoverAviary import MultiHoverAviary
+from gym_pybullet_drones.utils.enums import ObservationType, ActionType
+
+
+class Drones_Env:
+    def __init__(self, args):
+        # import scenarios of gym-pybullet-drones
+        self.env_id = args.env_id
+
+        REGISTRY = {
+            "CtrlAviary": CtrlAviary,
+            "HoverAviary": HoverAviary,
+            "VelocityAviary": VelocityAviary,
+            "MultiHoverAviary": MultiHoverAviary,
+            # you can add your customized scenarios here.
+        }
+        self.gui = args.render  # Note: You cannot render multiple environments in parallel.
+        self.sleep = args.sleep
+        self.env_id = args.env_id
+
+        kwargs_env = {'gui': self.gui}
+        if self.env_id in ["HoverAviary", "MultiHoverAviary"]:
+            kwargs_env.update({'obs': ObservationType(args.obs_type),
+                               'act': ActionType(args.act_type)})
+        if self.env_id != "HoverAviary":
+            kwargs_env.update({'num_drones': args.num_drones})
+        self.env = REGISTRY[args.env_id](**kwargs_env)
+
+        self._episode_step = 0
+        self._episode_score = 0.0
+        if self.env_id == "MultiHoverAviary":
+            self.observation_space = self.env.observation_space
+            self.observation_shape = self.env.observation_space.shape
+            self.action_space = self.env.action_space
+            self.action_shape = self.env.action_space.shape
+        else:
+            self.observation_space = self.space_reshape(self.env.observation_space)
+            self.action_space = self.space_reshape(self.env.action_space)
+        self.max_episode_steps = self.max_cycles = args.max_episode_steps
+
+        self.n_agents = args.num_drones
+        self.env_info = {
+            "n_agents": self.n_agents,
+            "obs_shape": self.env.observation_space.shape,
+            "act_space": self.action_space,
+            "state_shape": 20,
+            "n_actions": self.env.action_space.shape[-1],
+            "episode_limit": self.max_episode_steps,
+        }
+
+    def space_reshape(self, gym_space):
+        low = gym_space.low.reshape(-1)
+        high = gym_space.high.reshape(-1)
+        shape_obs = (gym_space.shape[-1], )
+        return Box(low=low, high=high, shape=shape_obs, dtype=gym_space.dtype)
 
     def close(self):
         self.env.close()
 
-    def render(self):
-        return self.env.render()
+    def render(self, *args, **kwargs):
+        return np.zeros([2, 2, 2])
 
-    def reset(self, seed=None, options=None):
-        observations, infos = self.env.reset()
-        for agent_key in self.agents:
-            self.individual_episode_reward[agent_key] = 0.0
-        reset_info = {"infos": infos,
-                      "individual_episode_rewards": self.individual_episode_reward}
-        return observations, reset_info
+    def reset(self):
+        obs, info = self.env.reset()
+        info["episode_step"] = self._episode_step
+
+        self._episode_step = 0
+        if self.n_agents > 1:
+            self._episode_score = np.zeros([self.n_agents, 1])
+            obs_return = obs
+        else:
+            self._episode_score = 0.0
+            obs_return = obs.reshape(-1)
+        return obs_return, info
 
     def step(self, actions):
-        if self.continuous_actions:
-            for k, v in actions.items():
-                actions[k] = np.clip(v, self.action_spaces[k].low, self.action_spaces[k].high)
-        observations, rewards, terminations, truncations, infos = self.env.step(actions)
-        for k, v in rewards.items():
-            self.individual_episode_reward[k] += v
-        step_info = {"infos": infos,
-                     "individual_episode_rewards": self.individual_episode_reward}
-        return observations, rewards, terminations, truncations, step_info
+        if self.n_agents > 1:
+            obs, reward, terminated, truncated, info = self.env.step(actions)
+            obs_return = obs
+            terminated = [terminated for _ in range(self.n_agents)]
+        else:
+            obs, reward, terminated, truncated, info = self.env.step(actions.reshape([1, -1]))
+            obs_return = obs.reshape(-1)
 
-    def state(self):
-        try:
-            return np.array(self.env.state())
-        except:
-            return None
-
-    def get_num(self, handle):
-        try:
-            n = self.env.env.get_num(handle)
-        except:
-            n = len(self.get_ids(handle))
-        return n
-
-    def get_ids(self, handle):
-        try:
-            ids = self.env.env.get_agent_id(handle)
-        except:
-            agent_name = AGENT_NAME_DICT[self.scenario_name][handle.value]
-            ids_handle = []
-            for id, agent_key in enumerate(self.agents):
-                if agent_name in agent_key:
-                    ids_handle.append(id)
-            ids = ids_handle
-        return ids
+        self._episode_step += 1
+        self._episode_score += reward
+        if self.n_agents > 1:
+            truncated = [True for _ in range(self.n_agents)] if (self._episode_step >= self.max_episode_steps) else [False for _ in range(self.n_agents)]
+        else:
+            truncated = True if (self._episode_step >= self.max_episode_steps) else False
+        info["episode_step"] = self._episode_step  # current episode step
+        info["episode_score"] = self._episode_score  # the accumulated rewards
+
+        if self.gui:
+            time.sleep(self.sleep)
+
+        return obs_return, reward, terminated, truncated, info
 
     def get_agent_mask(self):
-        if self.handles is None:
-            return np.ones(self.n_agents_all, dtype=np.bool)  # all alive
-        else:
-            mask = np.zeros(self.n_agents_all, dtype=np.bool)  # all dead
-            for handle in self.handles:
-                try:
-                    alive_ids = self.get_ids(handle)
-                    mask[alive_ids] = True  # get alive agents
-                except AttributeError("Cannot get the ids for alive agents!"):
-                    return
-        return mask
-
-    def get_handles(self):
-        if hasattr(self.env, 'handles'):
-            return self.env.handles
-        else:
-            try:
-                return self.env.env.get_handles()
-            except:
-                handles = [ctypes.c_int(h) for h in range(self.n_handles)]
-                return handles
+        return np.ones(self.n_agents, dtype=np.bool_)  # 1 means available
+
+    def state(self):
+        return np.zeros([20])
```

### Comparing `xuance-1.0.9/xuance/environment/pettingzoo/pettingzoo_vec_env.py` & `xuance-1.1.0/xuance/environment/pettingzoo/pettingzoo_vec_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from abc import ABC
-
 from xuance.environment.vector_envs.vector_env import VecEnv, AlreadySteppingError, NotSteppingError
 from xuance.environment.vector_envs.env_utils import obs_n_space_info
 from xuance.environment.gym.gym_vec_env import DummyVecEnv_Gym
 from operator import itemgetter
 from gymnasium.spaces.box import Box
 import numpy as np
 from xuance.environment.vector_envs.subproc_vec_env import clear_mpi_env_vars, flatten_list, CloudpickleWrapper
@@ -109,20 +107,20 @@
                              range(self.num_envs)]
         self.buf_rews_dict = [{k: 0.0 for k in self.keys} for _ in range(self.num_envs)]
         self.buf_dones_dict = [{k: False for k in self.keys} for _ in range(self.num_envs)]
         self.buf_trunctions_dict = [{k: False for k in self.keys} for _ in range(self.num_envs)]
         self.buf_infos_dict = [{} for _ in range(self.num_envs)]
         # buffer of numpy data
         self.buf_state = np.zeros((self.num_envs,) + self.state_shape, dtype=self.state_dtype)
-        self.buf_agent_mask = [np.ones([self.num_envs, n], dtype=np.bool) for n in self.n_agents]
+        self.buf_agent_mask = [np.ones([self.num_envs, n], dtype=np.bool_) for n in self.n_agents]
         self.buf_obs = [np.zeros((self.num_envs, n) + tuple(self.obs_shapes[h]), dtype=self.obs_dtype) for h, n in
                         enumerate(self.n_agents)]
         self.buf_rews = [np.zeros((self.num_envs, n, 1), dtype=np.float32) for n in self.n_agents]
-        self.buf_dones = [np.ones((self.num_envs, n), dtype=np.bool) for n in self.n_agents]
-        self.buf_trunctions = [np.ones((self.num_envs, n), dtype=np.bool) for n in self.n_agents]
+        self.buf_dones = [np.ones((self.num_envs, n), dtype=np.bool_) for n in self.n_agents]
+        self.buf_trunctions = [np.ones((self.num_envs, n), dtype=np.bool_) for n in self.n_agents]
 
         self.max_episode_length = env_info["max_cycles"]
         self.actions = None
 
     def empty_dict_buffers(self, i_env):
         # buffer of dict data
         self.buf_obs_dict[i_env] = {k: np.zeros(tuple(self.shapes[k]), dtype=self.dtypes[k]) for k in self.keys}
@@ -238,15 +236,15 @@
     def global_state(self):
         return self.buf_state
 
     def agent_mask(self):
         return self.buf_agent_mask
 
     def available_actions(self):
-        act_mask = [np.ones([self.num_envs, n, self.act_dim[h]], dtype=np.bool) for h, n in enumerate(self.n_agents)]
+        act_mask = [np.ones([self.num_envs, n, self.act_dim[h]], dtype=np.bool_) for h, n in enumerate(self.n_agents)]
         return np.array(act_mask)
 
 
 class DummyVecEnv_Pettingzoo(DummyVecEnv_Gym):
     def __init__(self, env_fns):
         self.waiting = False
         self.envs = [fn() for fn in env_fns]
@@ -276,20 +274,20 @@
                              range(self.num_envs)]
         self.buf_rews_dict = [{k: 0.0 for k in self.keys} for _ in range(self.num_envs)]
         self.buf_dones_dict = [{k: False for k in self.keys} for _ in range(self.num_envs)]
         self.buf_trunctions_dict = [{k: False for k in self.keys} for _ in range(self.num_envs)]
         self.buf_infos_dict = [{} for _ in range(self.num_envs)]
         # buffer of numpy data
         self.buf_state = np.zeros((self.num_envs, ) + self.state_shape, dtype=self.state_dtype)
-        self.buf_agent_mask = [np.ones([self.num_envs, n], dtype=np.bool) for n in self.n_agents]
+        self.buf_agent_mask = [np.ones([self.num_envs, n], dtype=np.bool_) for n in self.n_agents]
         self.buf_obs = [np.zeros((self.num_envs, n) + tuple(self.obs_shapes[h]), dtype=self.obs_dtype) for h, n in
                         enumerate(self.n_agents)]
         self.buf_rews = [np.zeros((self.num_envs, n, 1), dtype=np.float32) for n in self.n_agents]
-        self.buf_dones = [np.ones((self.num_envs, n), dtype=np.bool) for n in self.n_agents]
-        self.buf_trunctions = [np.ones((self.num_envs, n), dtype=np.bool) for n in self.n_agents]
+        self.buf_dones = [np.ones((self.num_envs, n), dtype=np.bool_) for n in self.n_agents]
+        self.buf_trunctions = [np.ones((self.num_envs, n), dtype=np.bool_) for n in self.n_agents]
 
         self.max_episode_length = env.max_cycles
         self.actions = None
 
     def empty_dict_buffers(self, i_env):
         # buffer of dict data
         self.buf_obs_dict[i_env] = {k: np.zeros(tuple(self.shapes[k]), dtype=self.dtypes[k]) for k in self.keys}
@@ -377,9 +375,9 @@
     def global_state(self):
         return self.buf_state
 
     def agent_mask(self):
         return self.buf_agent_mask
 
     def available_actions(self):
-        act_mask = [np.ones([self.num_envs, n, self.act_dim[h]], dtype=np.bool) for h, n in enumerate(self.n_agents)]
+        act_mask = [np.ones([self.num_envs, n, self.act_dim[h]], dtype=np.bool_) for h, n in enumerate(self.n_agents)]
         return np.array(act_mask)
```

### Comparing `xuance-1.0.9/xuance/environment/starcraft2/sc2_env.py` & `xuance-1.1.0/xuance/environment/starcraft2/sc2_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.dim_reward = self.n_agents
 
         self.observation_space = (self.dim_obs,)
         self.action_space = (self.dim_act, )
         self.max_cycles = self.env_info["episode_limit"]
         self._episode_step = 0
         self._episode_score = 0
-        self.filled = np.zeros([self.max_cycles, 1], np.bool)
+        self.filled = np.zeros([self.max_cycles, 1], np.bool_)
         self.env.reset()
         self.buf_info = {
             'battle_won': 0,
             'dead_allies': 0,
             'dead_enemies': 0,
         }
```

### Comparing `xuance-1.0.9/xuance/environment/starcraft2/sc2_vec_env.py` & `xuance-1.1.0/xuance/environment/starcraft2/sc2_vec_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,17 +80,17 @@
         self.dim_obs, self.dim_state, self.dim_act = self.dim_obs, env_info["state_shape"], self.dim_act
         self.dim_reward = self.num_agents
         self.action_space = Discrete(n=self.dim_act)
         self.state_space = Box(low=-np.inf, high=np.inf, shape=[self.dim_state, ])
 
         self.buf_obs = np.zeros(combined_shape(self.num_envs, self.obs_shape), dtype=np.float32)
         self.buf_state = np.zeros(combined_shape(self.num_envs, self.dim_state), dtype=np.float32)
-        self.buf_terminal = np.zeros((self.num_envs, 1), dtype=np.bool)
-        self.buf_truncation = np.zeros((self.num_envs, 1), dtype=np.bool)
-        self.buf_done = np.zeros((self.num_envs,), dtype=np.bool)
+        self.buf_terminal = np.zeros((self.num_envs, 1), dtype=np.bool_)
+        self.buf_truncation = np.zeros((self.num_envs, 1), dtype=np.bool_)
+        self.buf_done = np.zeros((self.num_envs,), dtype=np.bool_)
         self.buf_rew = np.zeros((self.num_envs,) + self.rew_shape, dtype=np.float32)
         self.buf_info = [{} for _ in range(self.num_envs)]
         self.actions = None
         self.battles_game = np.zeros(self.num_envs, np.int32)
         self.battles_won = np.zeros(self.num_envs, np.int32)
         self.dead_allies_count = np.zeros(self.num_envs, np.int32)
         self.dead_enemies_count = np.zeros(self.num_envs, np.int32)
@@ -100,15 +100,15 @@
         self._assert_not_closed()
         for remote in self.remotes:
             remote.send(('reset', None))
         result = [remote.recv() for remote in self.remotes]
         result = flatten_list(result)
         obs, state, infos = zip(*result)
         self.buf_obs, self.buf_state, self.buf_info = np.array(obs), np.array(state), list(infos)
-        self.buf_done = np.zeros((self.num_envs,), dtype=np.bool)
+        self.buf_done = np.zeros((self.num_envs,), dtype=np.bool_)
         return self.buf_obs.copy(), self.buf_state.copy(), self.buf_info.copy()
 
     def step_async(self, actions):
         self._assert_not_closed()
         actions = np.array_split(actions, self.n_remotes)
         for env_done, remote, action in zip(self.buf_done, self.remotes, actions):
             if not env_done:
@@ -196,32 +196,32 @@
         self.dim_obs, self.dim_state, self.dim_act = self.dim_obs, env_info["state_shape"], self.dim_act
         self.dim_reward = self.num_agents
         self.action_space = Discrete(n=self.dim_act)
         self.state_space = Box(low=-np.inf, high=np.inf, shape=[self.dim_state, ])
 
         self.buf_obs = np.zeros(combined_shape(self.num_envs, self.obs_shape), dtype=np.float32)
         self.buf_state = np.zeros(combined_shape(self.num_envs, self.dim_state), dtype=np.float32)
-        self.buf_terminal = np.zeros((self.num_envs, 1), dtype=np.bool)
-        self.buf_truncation = np.zeros((self.num_envs, 1), dtype=np.bool)
-        self.buf_done = np.zeros((self.num_envs,), dtype=np.bool)
+        self.buf_terminal = np.zeros((self.num_envs, 1), dtype=np.bool_)
+        self.buf_truncation = np.zeros((self.num_envs, 1), dtype=np.bool_)
+        self.buf_done = np.zeros((self.num_envs,), dtype=np.bool_)
         self.buf_rew = np.zeros((self.num_envs,) + self.rew_shape, dtype=np.float32)
         self.buf_info = [{} for _ in range(self.num_envs)]
         self.actions = None
         self.battles_game = np.zeros(self.num_envs, np.int32)
         self.battles_won = np.zeros(self.num_envs, np.int32)
         self.dead_allies_count = np.zeros(self.num_envs, np.int32)
         self.dead_enemies_count = np.zeros(self.num_envs, np.int32)
         self.max_episode_length = env_info["episode_limit"]
 
     def reset(self):
         self._assert_not_closed()
         for i_env, env in enumerate(self.envs):
             obs, state, infos = env.reset()
             self.buf_obs[i_env], self.buf_state[i_env], self.buf_info[i_env] = np.array(obs), np.array(state), list(infos)
-        self.buf_done = np.zeros((self.num_envs,), dtype=np.bool)
+        self.buf_done = np.zeros((self.num_envs,), dtype=np.bool_)
         return self.buf_obs.copy(), self.buf_state.copy(), self.buf_info.copy()
 
     def step_async(self, actions):
         self._assert_not_closed()
         self.actions = actions
         self.waiting = True
```

### Comparing `xuance-1.0.9/xuance/environment/vector_envs/env_utils.py` & `xuance-1.1.0/xuance/environment/vector_envs/env_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     image_height = image_shape[0]
     image_width = image_shape[1]
 
     rows = (image_nums - 1) // 4 + 1
     if image_nums >= 4:
         cols = 4
     else:
-        cols = 0
+        cols = image_nums
 
     try:
         big_img = np.zeros(
             (rows * image_height + 10 * (rows - 1), cols * image_width + 10 * (cols - 1), image_shape[2]), np.uint8)
     except IndexError:
         big_img = np.zeros((rows * image_height + 10 * (rows - 1), cols * image_width + 10 * (cols - 1)), np.uint8)
```

### Comparing `xuance-1.0.9/xuance/environment/vector_envs/vector_env.py` & `xuance-1.1.0/xuance/environment/vector_envs/vector_env.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,37 +12,14 @@
 
 class NotSteppingError(Exception):
     def __init__(self):
         msg = 'not running an async step'
         Exception.__init__(self, msg)
 
 
-def tile_images(images):
-    image_nums = len(images)
-    image_shape = images[0].shape
-    image_height = image_shape[0]
-    image_width = image_shape[1]
-    rows = (image_nums - 1) // 4 + 1
-    if image_nums >= 4:
-        cols = 4
-    else:
-        cols = image_nums
-    try:
-        big_img = np.zeros(
-            (rows * image_height + 10 * (rows - 1), cols * image_width + 10 * (cols - 1), image_shape[2]), np.uint8)
-    except IndexError:
-        big_img = np.zeros((rows * image_height + 10 * (rows - 1), cols * image_width + 10 * (cols - 1)), np.uint8)
-    for i in range(image_nums):
-        c = i % 4
-        r = i // 4
-        big_img[10 * r + image_height * r:10 * r + image_height * r + image_height,
-        10 * c + image_width * c:10 * c + image_width * c + image_width] = images[i]
-    return big_img
-
-
 class VecEnv(ABC):
     def __init__(self, num_envs, observation_space, action_space):
         self.num_envs = num_envs
         self.observation_space = observation_space
         self.action_space = action_space
         self.closed = False
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/__init__.py` & `xuance-1.1.0/xuance/mindspore/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/agent.py` & `xuance-1.1.0/xuance/mindspore/agents/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
                  log_dir: str = "./logs/",
                  model_dir: str = "./models/"):
         self.config = config
         self.envs = envs
         self.policy = policy
         self.memory = memory
         self.learner = learner
+        self.fps = config.fps
 
         self.observation_space = envs.observation_space
         self.comm = MPI.COMM_WORLD
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space), comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/agents_marl.py` & `xuance-1.1.0/xuance/mindspore/agents/agents_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/coma_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/coma_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/dcg_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/dcg_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/iddpg_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/maddpg_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from xuance.mindspore.agents import *
 
 
-class IDDPG_Agents(MARLAgents):
+class MADDPG_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo):
         self.gamma = config.gamma
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         scheduler = [lr_decay_model(learning_rate=config.lr_a, decay_rate=0.5,
                                     decay_steps=get_total_iters(config.agent_name, config)),
                      lr_decay_model(learning_rate=config.lr_c, decay_rate=0.5,
                                     decay_steps=get_total_iters(config.agent_name, config))]
         optimizer = [Adam(policy.parameters_actor, scheduler[0], eps=1e-5),
                      Adam(policy.parameters_critic, scheduler[1], eps=1e-5)]
@@ -31,16 +31,16 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = IDDPG_Learner(config, policy, optimizer, scheduler, config.model_dir, config.gamma)
-        super(IDDPG_Agents, self).__init__(config, envs, policy, memory, learner, config.log_dir, config.model_dir)
+        learner = MADDPG_Learner(config, policy, optimizer, scheduler, config.model_dir, config.gamma)
+        super(MADDPG_Agents, self).__init__(config, envs, policy, memory, learner, config.log_dir, config.model_dir)
         self.on_policy = False
 
     def act(self, obs_n, test_mode):
         batch_size = len(obs_n)
         agents_id = ops.broadcast_to(self.expand_dims(self.eye(self.n_agents, self.n_agents, ms.float32), 0),
                                      (batch_size, -1, -1))
         _, actions = self.policy(Tensor(obs_n), agents_id)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/ippo_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/ippo_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/iql_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/iql_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/isac_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/masac_agents.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from xuance.mindspore.agents import *
 
 
-class ISAC_Agents(MARLAgents):
+class MASAC_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo):
         self.gamma = config.gamma
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         scheduler = [lr_decay_model(learning_rate=config.lr_a, decay_rate=0.5,
                                     decay_steps=get_total_iters(config.agent_name, config)),
                      lr_decay_model(learning_rate=config.lr_c, decay_rate=0.5,
                                     decay_steps=get_total_iters(config.agent_name, config))]
         optimizer = [Adam(policy.parameters_actor, scheduler[0], eps=1e-5),
                      Adam(policy.parameters_critic, scheduler[1], eps=1e-5)]
@@ -31,24 +31,24 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = ISAC_Learner(config, policy, optimizer, scheduler, config.model_dir, config.gamma)
-        super(ISAC_Agents, self).__init__(config, envs, policy, memory, learner, config.log_dir, config.model_dir)
+        learner = MASAC_Learner(config, policy, optimizer, scheduler, config.model_dir, config.gamma)
+        super(MASAC_Agents, self).__init__(config, envs, policy, memory, learner, config.log_dir, config.model_dir)
         self.on_policy = False
 
-    def act(self, obs_n, test_mode):
+    def act(self, obs_n, *rnn_hidden, avail_actions=None, state=None, test_mode=False):
         batch_size = len(obs_n)
         agents_id = ops.broadcast_to(self.expand_dims(self.eye(self.n_agents, self.n_agents, ms.float32), 0),
                                      (batch_size, -1, -1))
-        _, act_probs = self.policy(Tensor(obs_n), agents_id)
-        acts = self.policy.actor_net.sample(act_probs)
+        _, act_mu = self.policy(Tensor(obs_n), agents_id)
+        acts = self.policy.actor_net.sample(act_mu)
         actions = acts.asnumpy()
         return None, actions
 
     def train(self, i_episode):
         sample = self.memory.sample()
         info_train = self.learner.update(sample)
         return info_train
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/maddpg_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/isac_agents.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from xuance.mindspore.agents import *
 
 
-class MADDPG_Agents(MARLAgents):
+class ISAC_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo):
         self.gamma = config.gamma
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         scheduler = [lr_decay_model(learning_rate=config.lr_a, decay_rate=0.5,
                                     decay_steps=get_total_iters(config.agent_name, config)),
                      lr_decay_model(learning_rate=config.lr_c, decay_rate=0.5,
                                     decay_steps=get_total_iters(config.agent_name, config))]
         optimizer = [Adam(policy.parameters_actor, scheduler[0], eps=1e-5),
                      Adam(policy.parameters_critic, scheduler[1], eps=1e-5)]
@@ -31,25 +31,24 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = MADDPG_Learner(config, policy, optimizer, scheduler, config.model_dir, config.gamma)
-        super(MADDPG_Agents, self).__init__(config, envs, policy, memory, learner, config.log_dir, config.model_dir)
+        learner = ISAC_Learner(config, policy, optimizer, scheduler, config.model_dir, config.gamma)
+        super(ISAC_Agents, self).__init__(config, envs, policy, memory, learner, config.log_dir, config.model_dir)
         self.on_policy = False
 
     def act(self, obs_n, test_mode):
         batch_size = len(obs_n)
         agents_id = ops.broadcast_to(self.expand_dims(self.eye(self.n_agents, self.n_agents, ms.float32), 0),
                                      (batch_size, -1, -1))
-        _, actions = self.policy(Tensor(obs_n), agents_id)
-        actions = actions.asnumpy()
-        if not test_mode:
-            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
+        _, act_probs = self.policy(Tensor(obs_n), agents_id)
+        acts = self.policy.actor_net.sample(act_probs)
+        actions = acts.asnumpy()
         return None, actions
 
     def train(self, i_episode):
         sample = self.memory.sample()
         info_train = self.learner.update(sample)
         return info_train
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/mappo_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/mappo_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/masac_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/iddpg_agents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from xuance.mindspore.agents import *
 
 
-class MASAC_Agents(MARLAgents):
+class IDDPG_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo):
         self.gamma = config.gamma
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         scheduler = [lr_decay_model(learning_rate=config.lr_a, decay_rate=0.5,
                                     decay_steps=get_total_iters(config.agent_name, config)),
                      lr_decay_model(learning_rate=config.lr_c, decay_rate=0.5,
                                     decay_steps=get_total_iters(config.agent_name, config))]
         optimizer = [Adam(policy.parameters_actor, scheduler[0], eps=1e-5),
                      Adam(policy.parameters_critic, scheduler[1], eps=1e-5)]
@@ -31,24 +31,25 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = MASAC_Learner(config, policy, optimizer, scheduler, config.model_dir, config.gamma)
-        super(MASAC_Agents, self).__init__(config, envs, policy, memory, learner, config.log_dir, config.model_dir)
+        learner = IDDPG_Learner(config, policy, optimizer, scheduler, config.model_dir, config.gamma)
+        super(IDDPG_Agents, self).__init__(config, envs, policy, memory, learner, config.log_dir, config.model_dir)
         self.on_policy = False
 
-    def act(self, obs_n, *rnn_hidden, avail_actions=None, state=None, test_mode=False):
+    def act(self, obs_n, test_mode):
         batch_size = len(obs_n)
         agents_id = ops.broadcast_to(self.expand_dims(self.eye(self.n_agents, self.n_agents, ms.float32), 0),
                                      (batch_size, -1, -1))
-        _, act_mu = self.policy(Tensor(obs_n), agents_id)
-        acts = self.policy.actor_net.sample(act_mu)
-        actions = acts.asnumpy()
+        _, actions = self.policy(Tensor(obs_n), agents_id)
+        actions = actions.asnumpy()
+        if not test_mode:
+            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
         return None, actions
 
     def train(self, i_episode):
         sample = self.memory.sample()
         info_train = self.learner.update(sample)
         return info_train
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/matd3_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/matd3_agents.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo):
         self.gamma = config.gamma
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         scheduler = [lr_decay_model(learning_rate=config.lr_a, decay_rate=0.5,
                                     decay_steps=get_total_iters(config.agent_name, config)),
                      lr_decay_model(learning_rate=config.lr_c, decay_rate=0.5,
                                     decay_steps=get_total_iters(config.agent_name, config)),
                      lr_decay_model(learning_rate=config.lr_c, decay_rate=0.5,
                                     decay_steps=get_total_iters(config.agent_name, config))]
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/mfac_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/mfac_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy, gain=config.gain)
         scheduler = lr_decay_model(learning_rate=config.learning_rate, decay_rate=0.5,
                                    decay_steps=get_total_iters(config.agent_name, config))
         optimizer = Adam(policy.trainable_params(), scheduler, eps=1e-5)
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/mfq_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/mfq_agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.egreedy = self.start_greedy
         self.delta_egreedy = (self.start_greedy - self.end_greedy) / config.decay_step_greedy
         self.use_recurrent, self.rnn = config.use_recurrent, config.rnn
         self.rnn_hidden = None
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         scheduler = lr_decay_model(learning_rate=config.learning_rate, decay_rate=0.5,
                                    decay_steps=get_total_iters(config.agent_name, config))
         optimizer = Adam(policy.trainable_params(), scheduler, eps=1e-5)
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/qmix_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/qmix_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/qtran_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/qtran_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/vdac_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/vdac_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/vdn_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/vdn_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/multi_agent_rl/wqmix_agents.py` & `xuance-1.1.0/xuance/mindspore/agents/multi_agent_rl/wqmix_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/policy_gradient/a2c_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/a2c_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/policy_gradient/ddpg_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ddpg_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
                         episode_videos = videos[i].copy()
                     if self.config.test_mode:
                         print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/policy_gradient/mpdqn_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/mpdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/policy_gradient/pdqn_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/pdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/policy_gradient/pg_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/pg_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from xuance.mindspore.agents import *
+from xuance.tensorflow.agents import *
 
 
 class PG_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Gym,
-                 policy: nn.Cell,
-                 optimizer: nn.Optimizer,
-                 scheduler):
+                 policy: tk.Model,
+                 optimizer: tk.optimizers.Optimizer,
+                 device: str = 'cpu'):
         self.render = config.render
         self.n_envs = envs.num_envs
         self.n_steps = config.n_steps
         self.n_minibatch = config.n_minibatch
         self.n_epoch = config.n_epoch
 
         self.gamma = config.gamma
@@ -32,24 +32,24 @@
                         self.n_steps,
                         config.use_gae,
                         config.use_advnorm,
                         self.gamma,
                         self.gae_lam)
         learner = PG_Learner(policy,
                              optimizer,
-                             scheduler,
+                             config.device,
                              config.model_dir,
                              config.ent_coef,
-                             config.clip_grad,
-                             config.clip_type)
-        super(PG_Agent, self).__init__(config, envs, policy, memory, learner, config.log_dir, config.model_dir)
+                             config.clip_grad)
+        super(PG_Agent, self).__init__(config, envs, policy, memory, learner, device, config.log_dir, config.model_dir)
 
     def _action(self, obs):
-        _, act_probs = self.policy(ms.Tensor(obs))
-        acts = self.policy.actor.sample(act_probs).asnumpy()
+        _, _ = self.policy(obs)
+        acts = self.policy.actor.dist.stochastic_sample()
+        acts = acts.numpy()
         return acts
 
     def train(self, train_steps):
         obs = self.envs.buf_obs
         for _ in tqdm(range(train_steps)):
             step_info = {}
             self.obs_rms.update(obs)
@@ -127,15 +127,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/policy_gradient/ppg_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ppg_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                         episode_videos = videos[i].copy()
                     if self.config.test_mode:
                         print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/policy_gradient/ppoclip_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ppoclip_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/policy_gradient/ppokl_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/ppokl_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/policy_gradient/sac_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/sac_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                         episode_videos = videos[i].copy()
                     if self.config.test_mode:
                         print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/policy_gradient/sacdis_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/sacdis_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/policy_gradient/spdqn_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/spdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/agents/policy_gradient/td3_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/policy_gradient/td3_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                         episode_videos = videos[i].copy()
                     if self.config.test_mode:
                         print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/qlearning_family/C51_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/dueldqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from xuance.mindspore.agents import *
 
 
-class C51_Agent(Agent):
+class DuelDQN_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Gym,
                  policy: nn.Cell,
                  optimizer: nn.Optimizer,
                  scheduler):
         self.render = config.render
@@ -26,21 +26,21 @@
         Buffer = DummyOffPolicyBuffer_Atari if self.atari else DummyOffPolicyBuffer
         memory = Buffer(self.observation_space,
                         self.action_space,
                         self.auxiliary_info_shape,
                         self.n_envs,
                         config.n_size,
                         config.batch_size)
-        learner = C51_Learner(policy,
-                              optimizer,
-                              scheduler,
-                              config.model_dir,
-                              config.gamma,
-                              config.sync_frequency)
-        super(C51_Agent, self).__init__(config, envs, policy, memory, learner, config.log_dir, config.model_dir)
+        learner = DuelDQN_Learner(policy,
+                                  optimizer,
+                                  scheduler,
+                                  config.model_dir,
+                                  config.gamma,
+                                  config.sync_frequency)
+        super(DuelDQN_Agent, self).__init__(config, envs, policy, memory, learner, config.log_dir, config.model_dir)
 
     def _action(self, obs, egreedy=0.0):
         _, argmax_action, _ = self.policy(ms.Tensor(obs))
         random_action = np.random.choice(self.action_space.n, self.n_envs)
         if np.random.rand() < egreedy:
             action = random_action
         else:
@@ -119,15 +119,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/qlearning_family/ddqn_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/ddqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/qlearning_family/dqn_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/dqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/qlearning_family/drqn_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/drqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/qlearning_family/dueldqn_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/C51_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from xuance.mindspore.agents import *
 
 
-class DuelDQN_Agent(Agent):
+class C51_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Gym,
                  policy: nn.Cell,
                  optimizer: nn.Optimizer,
                  scheduler):
         self.render = config.render
@@ -26,21 +26,21 @@
         Buffer = DummyOffPolicyBuffer_Atari if self.atari else DummyOffPolicyBuffer
         memory = Buffer(self.observation_space,
                         self.action_space,
                         self.auxiliary_info_shape,
                         self.n_envs,
                         config.n_size,
                         config.batch_size)
-        learner = DuelDQN_Learner(policy,
-                                  optimizer,
-                                  scheduler,
-                                  config.model_dir,
-                                  config.gamma,
-                                  config.sync_frequency)
-        super(DuelDQN_Agent, self).__init__(config, envs, policy, memory, learner, config.log_dir, config.model_dir)
+        learner = C51_Learner(policy,
+                              optimizer,
+                              scheduler,
+                              config.model_dir,
+                              config.gamma,
+                              config.sync_frequency)
+        super(C51_Agent, self).__init__(config, envs, policy, memory, learner, config.log_dir, config.model_dir)
 
     def _action(self, obs, egreedy=0.0):
         _, argmax_action, _ = self.policy(ms.Tensor(obs))
         random_action = np.random.choice(self.action_space.n, self.n_envs)
         if np.random.rand() < egreedy:
             action = random_action
         else:
@@ -119,15 +119,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/qlearning_family/noisydqn_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/noisydqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/qlearning_family/perdqn_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/perdqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/agents/qlearning_family/qrdqn_agent.py` & `xuance-1.1.0/xuance/mindspore/agents/qlearning_family/qrdqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/mindspore/learners/__init__.py` & `xuance-1.1.0/xuance/mindspore/learners/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/learner.py` & `xuance-1.1.0/xuance/mindspore/learners/learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/coma_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/coma_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/dcg_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/dcg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/iddpg_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/iddpg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/ippo_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/ippo_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/iql_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/iql_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/isac_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/isac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/maddpg_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/maddpg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/mappo_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/mappo_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/masac_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/masac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/matd3_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/matd3_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/mfac_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/mfac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/mfq_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/mfq_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/qmix_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/qmix_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/qtran_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/qtran_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/vdac_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/vdac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/vdn_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/vdn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/multi_agent_rl/wqmix_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/multi_agent_rl/wqmix_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/policy_gradient/a2c_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/a2c_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/policy_gradient/ddpg_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ddpg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/policy_gradient/mpdqn_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/mpdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/policy_gradient/pdqn_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/pdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/policy_gradient/pg_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/pg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/policy_gradient/ppg_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ppg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/policy_gradient/ppoclip_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ppoclip_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/policy_gradient/ppokl_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/ppokl_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/policy_gradient/sac_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/sac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/policy_gradient/sacdis_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/sacdis_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/policy_gradient/spdqn_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/spdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/policy_gradient/td3_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/policy_gradient/td3_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/qlearning_family/c51_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/c51_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/qlearning_family/ddqn_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/ddqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/qlearning_family/dqn_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/dqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/qlearning_family/drqn_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/drqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/qlearning_family/dueldqn_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/dueldqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/qlearning_family/noisydqn_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/noisydqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/qlearning_family/perdqn_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/perdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/learners/qlearning_family/qrdqn_learner.py` & `xuance-1.1.0/xuance/mindspore/learners/qlearning_family/qrdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/policies/__init__.py` & `xuance-1.1.0/xuance/mindspore/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/policies/categorical.py` & `xuance-1.1.0/xuance/mindspore/policies/categorical.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/policies/categorical_marl.py` & `xuance-1.1.0/xuance/mindspore/policies/categorical_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/policies/coordination_graph.py` & `xuance-1.1.0/xuance/mindspore/policies/coordination_graph.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/policies/deterministic.py` & `xuance-1.1.0/xuance/mindspore/policies/deterministic.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/policies/deterministic_marl.py` & `xuance-1.1.0/xuance/mindspore/policies/deterministic_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/policies/gaussian.py` & `xuance-1.1.0/xuance/mindspore/policies/gaussian.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/policies/gaussian_marl.py` & `xuance-1.1.0/xuance/mindspore/policies/gaussian_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/policies/mixers.py` & `xuance-1.1.0/xuance/mindspore/policies/mixers.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/representations/__init__.py` & `xuance-1.1.0/xuance/mindspore/representations/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/representations/cnn.py` & `xuance-1.1.0/xuance/mindspore/representations/cnn.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/representations/mlp.py` & `xuance-1.1.0/xuance/mindspore/representations/mlp.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/representations/rnn.py` & `xuance-1.1.0/xuance/mindspore/representations/rnn.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/runners/runner_drl.py` & `xuance-1.1.0/xuance/mindspore/runners/runner_drl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/runners/runner_pettingzoo.py` & `xuance-1.1.0/xuance/mindspore/runners/runner_pettingzoo.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,16 +218,16 @@
                 data_step['act_mean'] = actions_dict['act_mean'][h]
             else:
                 pass
             mas_group.memory.store(data_step)
 
     def train_episode(self, n_episodes):
         act_mean_last = [np.zeros([self.n_envs, arg.dim_act]) for arg in self.args]
-        terminal_handle = np.zeros([self.n_handles, self.n_envs], dtype=np.bool)
-        truncate_handle = np.zeros([self.n_handles, self.n_envs], dtype=np.bool)
+        terminal_handle = np.zeros([self.n_handles, self.n_envs], dtype=np.bool_)
+        truncate_handle = np.zeros([self.n_handles, self.n_envs], dtype=np.bool_)
         episode_score = np.zeros([self.n_handles, self.n_envs, 1], dtype=np.float32)
         episode_info, train_info = {}, {}
         for _ in tqdm(range(n_episodes)):
             obs_n = self.envs.buf_obs
             state, agent_mask = self.envs.global_state(), self.envs.agent_mask()
             for step in range(self.episode_length):
                 actions_dict = self.get_actions(obs_n, False, act_mean_last, agent_mask, state)
@@ -303,16 +303,16 @@
         obs_n, infos = test_envs.reset()
         state, agent_mask = test_envs.global_state(), test_envs.agent_mask()
         if self.args_base.render_mode == "rgb_array" and self.render:
             images = test_envs.render(self.args_base.render_mode)
             for idx, img in enumerate(images):
                 videos[idx].append(img)
         act_mean_last = [np.zeros([num_envs, arg.dim_act]) for arg in self.args]
-        terminal_handle = np.zeros([self.n_handles, num_envs], dtype=np.bool)
-        truncate_handle = np.zeros([self.n_handles, num_envs], dtype=np.bool)
+        terminal_handle = np.zeros([self.n_handles, num_envs], dtype=np.bool_)
+        truncate_handle = np.zeros([self.n_handles, num_envs], dtype=np.bool_)
         episode_score = np.zeros([self.n_handles, num_envs, 1], dtype=np.float32)
 
         for step in range(self.episode_length):
             actions_dict = self.get_actions(obs_n, True, act_mean_last, agent_mask, state)
             actions_execute = self.combine_env_actions(actions_dict['actions_n'])
             next_obs_n, rew_n, terminated_n, truncated_n, infos = test_envs.step(actions_execute)
             if self.args_base.render_mode == "rgb_array" and self.render:
```

### Comparing `xuance-1.0.9/xuance/mindspore/utils/__init__.py` & `xuance-1.1.0/xuance/mindspore/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/utils/distributions.py` & `xuance-1.1.0/xuance/mindspore/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/utils/input_reformat.py` & `xuance-1.1.0/xuance/mindspore/utils/input_reformat.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/utils/layers.py` & `xuance-1.1.0/xuance/mindspore/utils/layers.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/utils/operations.py` & `xuance-1.1.0/xuance/mindspore/utils/operations.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/mindspore/utils/set_trainer.py` & `xuance-1.1.0/xuance/mindspore/utils/set_trainer.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/__init__.py` & `xuance-1.1.0/xuance/tensorflow/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
                  log_dir: str = "./logs/",
                  model_dir: str = "./models/"):
         self.config = config
         self.envs = envs
         self.policy = policy
         self.memory = memory
         self.learner = learner
+        self.fps = config.fps
 
         self.observation_space = envs.observation_space
         self.comm = MPI.COMM_WORLD
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space), comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/agents_marl.py` & `xuance-1.1.0/xuance/tensorflow/agents/agents_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/coma_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/coma_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/dcg_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/dcg_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/iddpg_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/iddpg_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo,
                  device: str = "cpu:0"):
         self.gamma = config.gamma
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5,
                                    total_iters=get_total_iters(config.agent_name, config)),
                         MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5,
                                    total_iters=get_total_iters(config.agent_name, config))]
         optimizer = [tk.optimizers.Adam(lr_scheduler[0]),
                      tk.optimizers.Adam(lr_scheduler[1])]
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/ippo_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/ippo_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/iql_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/iql_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/isac_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/isac_agents.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo,
                  device: str = "cpu:0"):
         self.gamma = config.gamma
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5,
                                    total_iters=get_total_iters(config.agent_name, config)),
                         MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5,
                                    total_iters=get_total_iters(config.agent_name, config))]
         optimizer = [tk.optimizers.Adam(lr_scheduler[0]),
                      tk.optimizers.Adam(lr_scheduler[1])]
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/maddpg_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/maddpg_agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo,
                  device: str = "cpu:0"):
         self.gamma = config.gamma
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5,
                                    total_iters=get_total_iters(config.agent_name, config)),
                         MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5,
                                    total_iters=get_total_iters(config.agent_name, config))]
         optimizer = [tk.optimizers.Adam(lr_scheduler[0]),
                      tk.optimizers.Adam(lr_scheduler[1])]
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/mappo_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/mappo_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/masac_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/matd3_agents.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from xuance.tensorflow.agents import *
 
 
-class MASAC_Agents(MARLAgents):
+class MATD3_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo,
                  device: str = "cpu:0"):
         self.gamma = config.gamma
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5,
                                    total_iters=get_total_iters(config.agent_name, config)),
                         MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5,
                                    total_iters=get_total_iters(config.agent_name, config))]
         optimizer = [tk.optimizers.Adam(lr_scheduler[0]),
                      tk.optimizers.Adam(lr_scheduler[1])]
@@ -32,26 +32,30 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = MASAC_Learner(config, policy, optimizer, config.device, config.model_dir, config.gamma)
-        super(MASAC_Agents, self).__init__(config, envs, policy, memory, learner, device,
+        learner = MATD3_Learner(config, policy, optimizer,
+                                config.device, config.model_dir, config.gamma)
+        super(MATD3_Agents, self).__init__(config, envs, policy, memory, learner, device,
                                            config.log_dir, config.model_dir)
         self.on_policy = False
 
     def act(self, obs_n, test_mode):
         batch_size = len(obs_n)
         with tf.device(self.device):
             agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
             inputs_policy = {"obs": tf.convert_to_tensor(obs_n), "ids": agents_id}
-            _, dists = self.policy(inputs_policy)
-            acts = dists.sample()
-        actions = acts.numpy()
-        return None, actions
+            _, actions = self.policy(inputs_policy)
+        actions = actions.numpy()
+        if test_mode:
+            return None, actions
+        else:
+            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
+            return None, actions
 
     def train(self, i_episode):
         sample = self.memory.sample()
         info_train = self.learner.update(sample)
         return info_train
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/matd3_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/masac_agents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from xuance.tensorflow.agents import *
 
 
-class MATD3_Agents(MARLAgents):
+class MASAC_Agents(MARLAgents):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo,
                  device: str = "cpu:0"):
         self.gamma = config.gamma
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         lr_scheduler = [MyLinearLR(config.lr_a, start_factor=1.0, end_factor=0.5,
                                    total_iters=get_total_iters(config.agent_name, config)),
                         MyLinearLR(config.lr_c, start_factor=1.0, end_factor=0.5,
                                    total_iters=get_total_iters(config.agent_name, config))]
         optimizer = [tk.optimizers.Adam(lr_scheduler[0]),
                      tk.optimizers.Adam(lr_scheduler[1])]
@@ -32,30 +32,26 @@
                                       config.obs_shape,
                                       config.act_shape,
                                       config.rew_shape,
                                       config.done_shape,
                                       envs.num_envs,
                                       config.buffer_size,
                                       config.batch_size)
-        learner = MATD3_Learner(config, policy, optimizer,
-                                config.device, config.model_dir, config.gamma)
-        super(MATD3_Agents, self).__init__(config, envs, policy, memory, learner, device,
+        learner = MASAC_Learner(config, policy, optimizer, config.device, config.model_dir, config.gamma)
+        super(MASAC_Agents, self).__init__(config, envs, policy, memory, learner, device,
                                            config.log_dir, config.model_dir)
         self.on_policy = False
 
     def act(self, obs_n, test_mode):
         batch_size = len(obs_n)
         with tf.device(self.device):
             agents_id = tf.tile(tf.expand_dims(tf.eye(self.n_agents), axis=0), multiples=(batch_size, 1, 1))
             inputs_policy = {"obs": tf.convert_to_tensor(obs_n), "ids": agents_id}
-            _, actions = self.policy(inputs_policy)
-        actions = actions.numpy()
-        if test_mode:
-            return None, actions
-        else:
-            actions += np.random.normal(0, self.args.sigma, size=actions.shape)
-            return None, actions
+            _, dists = self.policy(inputs_policy)
+            acts = dists.sample()
+        actions = acts.numpy()
+        return None, actions
 
     def train(self, i_episode):
         sample = self.memory.sample()
         info_train = self.learner.update(sample)
         return info_train
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/mfac_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/mfac_agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy, gain=config.gain)
         lr_scheduler = MyLinearLR(config.learning_rate, start_factor=1.0, end_factor=0.5,
                                   total_iters=get_total_iters(config.agent_name, config))
         optimizer = tk.optimizers.Adam(lr_scheduler)
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/mfq_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/mfq_agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.egreedy = self.start_greedy
         self.delta_egreedy = (self.start_greedy - self.end_greedy) / config.decay_step_greedy
         self.use_recurrent, self.rnn = config.use_recurrent, config.rnn
         self.rnn_hidden = None
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         lr_scheduler = MyLinearLR(config.learning_rate, start_factor=1.0, end_factor=0.5,
                                   total_iters=get_total_iters(config.agent_name, config))
         optimizer = tk.optimizers.Adam(lr_scheduler)
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/qmix_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/qmix_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/qtran_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/qtran_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/vdac_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/vdac_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/vdn_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/vdn_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/multi_agent_rl/wqmix_agents.py` & `xuance-1.1.0/xuance/tensorflow/agents/multi_agent_rl/wqmix_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/a2c_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/a2c_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/ddpg_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ddpg_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                         episode_videos = videos[i].copy()
                     if self.config.test_mode:
                         print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/mpdqn_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/mpdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/pdqn_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/pdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/pg_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ppoclip_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,116 +1,131 @@
 from xuance.tensorflow.agents import *
 
 
-class PG_Agent(Agent):
+class PPOCLIP_Agent(Agent):
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Gym,
                  policy: tk.Model,
                  optimizer: tk.optimizers.Optimizer,
                  device: str = 'cpu'):
         self.render = config.render
         self.n_envs = envs.num_envs
         self.n_steps = config.n_steps
         self.n_minibatch = config.n_minibatch
         self.n_epoch = config.n_epoch
 
         self.gamma = config.gamma
         self.gae_lam = config.gae_lambda
-        self.clip_grad = config.clip_grad
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
-        self.representation_info_shape = policy.representation.output_shapes
-        self.auxiliary_info_shape = {}
+        self.auxiliary_info_shape = {"old_logp": ()}
+
         self.atari = True if config.env_name == "Atari" else False
         Buffer = DummyOnPolicyBuffer_Atari if self.atari else DummyOnPolicyBuffer
         self.buffer_size = self.n_envs * self.n_steps
-        self.batch_size = self.buffer_size // self.n_epoch
+        self.batch_size = self.buffer_size // self.n_minibatch
         memory = Buffer(self.observation_space,
                         self.action_space,
                         self.auxiliary_info_shape,
                         self.n_envs,
                         self.n_steps,
                         config.use_gae,
                         config.use_advnorm,
                         self.gamma,
                         self.gae_lam)
-        learner = PG_Learner(policy,
-                             optimizer,
-                             config.device,
-                             config.model_dir,
-                             config.ent_coef,
-                             config.clip_grad)
-        super(PG_Agent, self).__init__(config, envs, policy, memory, learner, device, config.log_dir, config.model_dir)
+        learner = PPOCLIP_Learner(policy,
+                                  optimizer,
+                                  config.device,
+                                  config.model_dir,
+                                  config.vf_coef,
+                                  config.ent_coef,
+                                  config.clip_range)
+        super(PPOCLIP_Agent, self).__init__(config, envs, policy, memory, learner, device, config.log_dir,
+                                            config.model_dir)
 
     def _action(self, obs):
-        _, _ = self.policy(obs)
-        acts = self.policy.actor.dist.stochastic_sample()
+        _, _, vs = self.policy(obs)
+        dists = self.policy.actor.dist
+        acts = dists.stochastic_sample()
+        logps = dists.log_prob(acts)
+        vs = vs.numpy()
         acts = acts.numpy()
-        return acts
+        logps = logps.numpy()
+        return acts, vs, logps
 
     def train(self, train_steps):
         obs = self.envs.buf_obs
         for _ in tqdm(range(train_steps)):
             step_info = {}
             self.obs_rms.update(obs)
             obs = self._process_observation(obs)
-            acts = self._action(obs)
+            acts, value, logps = self._action(obs)
             next_obs, rewards, terminals, trunctions, infos = self.envs.step(acts)
-            self.memory.store(obs, acts, self._process_reward(rewards), 0, terminals)
+
+            self.memory.store(obs, acts, self._process_reward(rewards), value, terminals, {"old_logp": logps})
             if self.memory.full:
+                _, vals, _ = self._action(self._process_observation(next_obs))
                 for i in range(self.n_envs):
-                    self.memory.finish_path(self._process_reward(rewards)[i], i)
+                    if terminals[i]:
+                        self.memory.finish_path(0.0, i)
+                    else:
+                        self.memory.finish_path(vals[i], i)
                 indexes = np.arange(self.buffer_size)
                 for _ in range(self.n_epoch):
                     np.random.shuffle(indexes)
                     for start in range(0, self.buffer_size, self.batch_size):
                         end = start + self.batch_size
                         sample_idx = indexes[start:end]
-                        obs_batch, act_batch, ret_batch, _, _, _ = self.memory.sample(sample_idx)
-                        step_info = self.learner.update(obs_batch, act_batch, ret_batch)
+                        obs_batch, act_batch, ret_batch, value_batch, adv_batch, aux_batch = self.memory.sample(sample_idx)
+                        step_info.update(self.learner.update(obs_batch, act_batch, ret_batch, value_batch, adv_batch, aux_batch['old_logp']))
                 self.log_infos(step_info, self.current_step)
                 self.memory.clear()
 
-            self.returns = self.gamma * self.returns + rewards
+            self.returns = (1 - terminals) * self.gamma * self.returns + rewards
             obs = next_obs
             for i in range(self.n_envs):
                 if terminals[i] or trunctions[i]:
                     self.ret_rms.update(self.returns[i:i + 1])
                     self.returns[i] = 0.0
                     if self.atari and (~trunctions[i]):
                         pass
                     else:
+                        if terminals[i]:
+                            self.memory.finish_path(0.0, i)
+                        else:
+                            _, vals, _ = self._action(self._process_observation(next_obs))
+                            self.memory.finish_path(vals[i], i)
                         obs[i] = infos[i]["reset_obs"]
-                        self.memory.finish_path(0, i)
                         self.current_episode[i] += 1
                         if self.use_wandb:
                             step_info["Episode-Steps/env-%d" % i] = infos[i]["episode_step"]
                             step_info["Train-Episode-Rewards/env-%d" % i] = infos[i]["episode_score"]
                         else:
                             step_info["Episode-Steps"] = {"env-%d" % i: infos[i]["episode_step"]}
                             step_info["Train-Episode-Rewards"] = {"env-%d" % i: infos[i]["episode_score"]}
                         self.log_infos(step_info, self.current_step)
+
             self.current_step += self.n_envs
 
-    def test(self, env_fn, test_episodes):
+    def test(self, env_fn, test_episode):
         test_envs = env_fn()
         num_envs = test_envs.num_envs
         videos, episode_videos = [[] for _ in range(num_envs)], []
         current_episode, scores, best_score = 0, [], -np.inf
         obs, infos = test_envs.reset()
         if self.config.render_mode == "rgb_array" and self.render:
             images = test_envs.render(self.config.render_mode)
             for idx, img in enumerate(images):
                 videos[idx].append(img)
 
-        while current_episode < test_episodes:
+        while current_episode < test_episode:
             self.obs_rms.update(obs)
             obs = self._process_observation(obs)
-            acts = self._action(obs)
+            acts, rets, logps = self._action(obs)
             next_obs, rewards, terminals, trunctions, infos = test_envs.step(acts)
             if self.config.render_mode == "rgb_array" and self.render:
                 images = test_envs.render(self.config.render_mode)
                 for idx, img in enumerate(images):
                     videos[idx].append(img)
 
             obs = next_obs
@@ -127,15 +142,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/ppg_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ppg_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
                         episode_videos = videos[i].copy()
                     if self.config.test_mode:
                         print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/ppoclip_agent.py` & `xuance-1.1.0/xuance/torch/agents/policy_gradient/ppoclip_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,28 @@
-from xuance.tensorflow.agents import *
+from xuance.torch.agents import *
 
 
 class PPOCLIP_Agent(Agent):
+    """The implementation of PPO agent.
+
+    Args:
+        config: the Namespace variable that provides hyper-parameters and other settings.
+        envs: the vectorized environments.
+        policy: the neural network modules of the agent.
+        optimizer: the method of optimizing.
+        scheduler: the learning rate decay scheduler.
+        device: the calculating device of the model, such as CPU or GPU.
+    """
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Gym,
-                 policy: tk.Model,
-                 optimizer: tk.optimizers.Optimizer,
-                 device: str = 'cpu'):
+                 policy: nn.Module,
+                 optimizer: torch.optim.Optimizer,
+                 scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
+                 device: Optional[Union[int, str, torch.device]] = None):
         self.render = config.render
         self.n_envs = envs.num_envs
         self.n_steps = config.n_steps
         self.n_minibatch = config.n_minibatch
         self.n_epoch = config.n_epoch
 
         self.gamma = config.gamma
@@ -31,30 +42,32 @@
                         self.n_steps,
                         config.use_gae,
                         config.use_advnorm,
                         self.gamma,
                         self.gae_lam)
         learner = PPOCLIP_Learner(policy,
                                   optimizer,
+                                  scheduler,
                                   config.device,
                                   config.model_dir,
-                                  config.vf_coef,
-                                  config.ent_coef,
-                                  config.clip_range)
-        super(PPOCLIP_Agent, self).__init__(config, envs, policy, memory, learner, device, config.log_dir,
-                                            config.model_dir)
+                                  vf_coef=config.vf_coef,
+                                  ent_coef=config.ent_coef,
+                                  clip_range=config.clip_range,
+                                  clip_grad_norm=config.clip_grad_norm,
+                                  use_grad_clip=config.use_grad_clip)
+        super(PPOCLIP_Agent, self).__init__(config, envs, policy, memory, learner, device,
+                                            config.log_dir, config.model_dir)
 
     def _action(self, obs):
-        _, _, vs = self.policy(obs)
-        dists = self.policy.actor.dist
+        _, dists, vs = self.policy(obs)
         acts = dists.stochastic_sample()
         logps = dists.log_prob(acts)
-        vs = vs.numpy()
-        acts = acts.numpy()
-        logps = logps.numpy()
+        vs = vs.detach().cpu().numpy()
+        acts = acts.detach().cpu().numpy()
+        logps = logps.detach().cpu().numpy()
         return acts, vs, logps
 
     def train(self, train_steps):
         obs = self.envs.buf_obs
         for _ in tqdm(range(train_steps)):
             step_info = {}
             self.obs_rms.update(obs)
@@ -73,15 +86,15 @@
                 indexes = np.arange(self.buffer_size)
                 for _ in range(self.n_epoch):
                     np.random.shuffle(indexes)
                     for start in range(0, self.buffer_size, self.batch_size):
                         end = start + self.batch_size
                         sample_idx = indexes[start:end]
                         obs_batch, act_batch, ret_batch, value_batch, adv_batch, aux_batch = self.memory.sample(sample_idx)
-                        step_info.update(self.learner.update(obs_batch, act_batch, ret_batch, value_batch, adv_batch, aux_batch['old_logp']))
+                        step_info = self.learner.update(obs_batch, act_batch, ret_batch, value_batch, adv_batch, aux_batch['old_logp'])
                 self.log_infos(step_info, self.current_step)
                 self.memory.clear()
 
             self.returns = (1 - terminals) * self.gamma * self.returns + rewards
             obs = next_obs
             for i in range(self.n_envs):
                 if terminals[i] or trunctions[i]:
@@ -142,15 +155,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/ppokl_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/ppokl_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/sac_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/sac_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                         episode_videos = videos[i].copy()
                     if self.config.test_mode:
                         print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/sacdis_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/sacdis_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/spdqn_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/spdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/policy_gradient/td3_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/policy_gradient/td3_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                         episode_videos = videos[i].copy()
                     if self.config.test_mode:
                         print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/c51_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/c51_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {"Test-Episode-Rewards/Mean-Score": np.mean(scores)}
         self.log_infos(test_info, self.current_step)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/ddqn_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/ddqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/dqn_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/dqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/drqn_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/drqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/dueldqn_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/dueldqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/noisydqn_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/noisydqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/perdqn_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/perdqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/agents/qlearning_family/qrdqn_agent.py` & `xuance-1.1.0/xuance/tensorflow/agents/qlearning_family/qrdqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/__init__.py` & `xuance-1.1.0/xuance/tensorflow/learners/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/coma_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/coma_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/dcg_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/dcg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/iddpg_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/iddpg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/ippo_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/ippo_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/iql_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/iql_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/isac_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/isac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/maddpg_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/maddpg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/mappo_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/mappo_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/masac_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/masac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/matd3_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/matd3_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/mfac_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/mfac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/mfq_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/mfq_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/qmix_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/qmix_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/qtran_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/qtran_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/vdac_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/vdac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/vdn_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/vdn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/multi_agent_rl/wqmix_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/multi_agent_rl/wqmix_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/a2c_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/a2c_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/ddpg_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ddpg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/mpdqn_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/mpdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/pdqn_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/pdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/pg_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/pg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/ppg_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ppg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/ppoclip_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ppoclip_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/ppokl_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/ppokl_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/sac_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/sac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/sacdis_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/sacdis_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/spdqn_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/spdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/policy_gradient/td3_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/policy_gradient/td3_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/c51_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/c51_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/ddqn_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/ddqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/dqn_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/dqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/drqn_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/drqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/dueldqn_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/dueldqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/perdqn_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/perdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/learners/qlearning_family/qrdqn_learner.py` & `xuance-1.1.0/xuance/tensorflow/learners/qlearning_family/qrdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/policies/__init__.py` & `xuance-1.1.0/xuance/tensorflow/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/policies/categorical.py` & `xuance-1.1.0/xuance/tensorflow/policies/categorical.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/policies/categorical_marl.py` & `xuance-1.1.0/xuance/tensorflow/policies/categorical_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/policies/coordination_graph.py` & `xuance-1.1.0/xuance/tensorflow/policies/coordination_graph.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/policies/deterministic.py` & `xuance-1.1.0/xuance/tensorflow/policies/deterministic.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/policies/deterministic_marl.py` & `xuance-1.1.0/xuance/tensorflow/policies/deterministic_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/policies/gaussian.py` & `xuance-1.1.0/xuance/tensorflow/policies/gaussian.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/policies/gaussian_marl.py` & `xuance-1.1.0/xuance/tensorflow/policies/gaussian_marl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/policies/mixers.py` & `xuance-1.1.0/xuance/tensorflow/policies/mixers.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/representations/__init__.py` & `xuance-1.1.0/xuance/tensorflow/representations/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/representations/cnn.py` & `xuance-1.1.0/xuance/tensorflow/representations/cnn.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/representations/mlp.py` & `xuance-1.1.0/xuance/tensorflow/representations/mlp.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/runners/runner_basic.py` & `xuance-1.1.0/xuance/tensorflow/runners/runner_basic.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/runners/runner_drl.py` & `xuance-1.1.0/xuance/tensorflow/runners/runner_drl.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/runners/runner_pettingzoo.py` & `xuance-1.1.0/xuance/tensorflow/runners/runner_pettingzoo.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,16 +218,16 @@
                 data_step['act_mean'] = actions_dict['act_mean'][h]
             else:
                 pass
             mas_group.memory.store(data_step)
 
     def train_episode(self, n_episodes):
         act_mean_last = [np.zeros([self.n_envs, arg.dim_act]) for arg in self.args]
-        terminal_handle = np.zeros([self.n_handles, self.n_envs], dtype=np.bool)
-        truncate_handle = np.zeros([self.n_handles, self.n_envs], dtype=np.bool)
+        terminal_handle = np.zeros([self.n_handles, self.n_envs], dtype=np.bool_)
+        truncate_handle = np.zeros([self.n_handles, self.n_envs], dtype=np.bool_)
         episode_score = np.zeros([self.n_handles, self.n_envs, 1], dtype=np.float32)
         episode_info, train_info = {}, {}
         for _ in tqdm(range(n_episodes)):
             obs_n = self.envs.buf_obs
             state, agent_mask = self.envs.global_state(), self.envs.agent_mask()
             for step in range(self.episode_length):
                 actions_dict = self.get_actions(obs_n, False, act_mean_last, agent_mask, state)
@@ -302,16 +302,16 @@
         obs_n, infos = test_envs.reset()
         state, agent_mask = test_envs.global_state(), test_envs.agent_mask()
         if self.args_base.render_mode == "rgb_array" and self.render:
             images = test_envs.render(self.args_base.render_mode)
             for idx, img in enumerate(images):
                 videos[idx].append(img)
         act_mean_last = [np.zeros([num_envs, arg.dim_act]) for arg in self.args]
-        terminal_handle = np.zeros([self.n_handles, num_envs], dtype=np.bool)
-        truncate_handle = np.zeros([self.n_handles, num_envs], dtype=np.bool)
+        terminal_handle = np.zeros([self.n_handles, num_envs], dtype=np.bool_)
+        truncate_handle = np.zeros([self.n_handles, num_envs], dtype=np.bool_)
         episode_score = np.zeros([self.n_handles, num_envs, 1], dtype=np.float32)
 
         for step in range(self.episode_length):
             actions_dict = self.get_actions(obs_n, True, act_mean_last, agent_mask, state)
             actions_execute = self.combine_env_actions(actions_dict['actions_n'])
             next_obs_n, rew_n, terminated_n, truncated_n, infos = test_envs.step(actions_execute)
             if self.args_base.render_mode == "rgb_array" and self.render:
```

### Comparing `xuance-1.0.9/xuance/tensorflow/utils/__init__.py` & `xuance-1.1.0/xuance/tensorflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/utils/distributions.py` & `xuance-1.1.0/xuance/tensorflow/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/utils/input_reformat.py` & `xuance-1.1.0/xuance/tensorflow/utils/input_reformat.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/utils/layers.py` & `xuance-1.1.0/xuance/tensorflow/utils/layers.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/tensorflow/utils/operations.py` & `xuance-1.1.0/xuance/tensorflow/utils/operations.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/agents/agent.py` & `xuance-1.1.0/xuance/torch/agents/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import socket
-import time
 from pathlib import Path
 from xuance.torch.agents import *
+from xuance.common import get_time_string
 
 
 class Agent(ABC):
     """The class of basic agents.
 
     Args:
         config: the Namespace variable that provides hyper-parameters and other settings.
@@ -13,44 +13,45 @@
         policy: the neural network modules of the agent.
         memory: the experience replay buffer.
         learner: the learner for the corresponding agent.
         device: the calculating device of the model, such as CPU or GPU.
         log_dir: the directory of the log file.
         model_dir: the directory for models saving.
     """
+
     def __init__(self,
                  config: Namespace,
                  envs: DummyVecEnv_Gym,
                  policy: nn.Module,
                  memory: Buffer,
                  learner: Learner,
                  device: Optional[Union[str, int, torch.device]] = None,
                  log_dir: str = "./logs/",
                  model_dir: str = "./models/"):
         self.config = config
         self.envs = envs
         self.policy = policy
         self.memory = memory
         self.learner = learner
+        self.fps = config.fps
 
         self.observation_space = envs.observation_space
         self.comm = MPI.COMM_WORLD
         self.obs_rms = RunningMeanStd(shape=space2shape(self.observation_space), comm=self.comm, use_mpi=False)
         self.ret_rms = RunningMeanStd(shape=(), comm=self.comm, use_mpi=False)
         self.use_obsnorm = config.use_obsnorm
         self.use_rewnorm = config.use_rewnorm
         self.obsnorm_range = config.obsnorm_range
         self.rewnorm_range = config.rewnorm_range
         self.returns = np.zeros((self.envs.num_envs,), np.float32)
 
-        time_string = time.asctime().replace(" ", "").replace(":", "_")
+        time_string = get_time_string()
         seed = f"seed_{self.config.seed}_"
-        model_dir_save = os.path.join(os.getcwd(), model_dir, seed + time_string)
-        if (not os.path.exists(model_dir_save)) and (not config.test_mode):
-            os.makedirs(model_dir_save)
+        self.model_dir_save = os.path.join(os.getcwd(), model_dir, seed + time_string)
+        self.model_dir_load = model_dir
 
         # logger
         if config.logger == "tensorboard":
             log_dir = os.path.join(os.getcwd(), config.log_dir, seed + time_string)
             if not os.path.exists(log_dir):
                 os.makedirs(log_dir)
             self.writer = SummaryWriter(log_dir)
@@ -63,37 +64,37 @@
             wandb.init(config=config_dict,
                        project=config.project_name,
                        entity=config.wandb_user_name,
                        notes=socket.gethostname(),
                        dir=wandb_dir,
                        group=config.env_id,
                        job_type=config.agent,
-                       name=time.asctime(),
+                       name=time_string,
                        reinit=True,
                        settings=wandb.Settings(start_method="fork")
                        )
             # os.environ["WANDB_SILENT"] = "True"
             self.use_wandb = True
         else:
             raise "No logger is implemented."
 
         self.device = device
         self.log_dir = log_dir
-        self.model_dir_save = model_dir_save
-        self.model_dir_load = model_dir
         create_directory(log_dir)
         self.current_step = 0
         self.current_episode = np.zeros((self.envs.num_envs,), np.int32)
 
     def save_model(self, model_name):
-        model_path = self.model_dir_save + "/" + model_name
+        if not os.path.exists(self.model_dir_save):
+            os.makedirs(self.model_dir_save)
+        model_path = os.path.join(self.model_dir_save, model_name)
         self.learner.save_model(model_path)
 
-    def load_model(self, path, seed=1):
-        self.learner.load_model(path, seed)
+    def load_model(self, path, model=None):
+        self.learner.load_model(path, model)
 
     def log_infos(self, info: dict, x_index: int):
         """
         info: (dict) information to be visualized
         n_steps: current step
         """
         if self.use_wandb:
@@ -102,15 +103,15 @@
         else:
             for k, v in info.items():
                 try:
                     self.writer.add_scalar(k, v, x_index)
                 except:
                     self.writer.add_scalars(k, v, x_index)
 
-    def log_videos(self, info: dict, fps: int, x_index: int=0):
+    def log_videos(self, info: dict, fps: int, x_index: int = 0):
         if self.use_wandb:
             for k, v in info.items():
                 wandb.log({k: wandb.Video(v, fps=fps, format='gif')}, step=x_index)
         else:
             for k, v in info.items():
                 self.writer.add_video(k, v, fps=fps, global_step=x_index)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/agents_marl.py` & `xuance-1.1.0/xuance/torch/agents/agents_marl.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,22 +39,23 @@
         self.policy = policy
         self.memory = memory
         self.learner = learner
         self.device = device
         self.log_dir = log_dir
         self.model_dir_save, self.model_dir_load = config.model_dir_save, config.model_dir_load
         create_directory(log_dir)
-        create_directory(model_dir)
 
     def save_model(self, model_name):
+        if not os.path.exists(self.model_dir_save):
+            os.makedirs(self.model_dir_save)
         model_path = os.path.join(self.model_dir_save, model_name)
         self.learner.save_model(model_path)
 
-    def load_model(self, path, seed=1):
-        self.learner.load_model(path, seed)
+    def load_model(self, path, model=None):
+        self.learner.load_model(path, model)
 
     def act(self, **kwargs):
         raise NotImplementedError
 
     def train(self, **kwargs):
         raise NotImplementedError
```

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/coma_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/coma_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/dcg_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/dcg_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/iddpg_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/iddpg_agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.gamma = config.gamma
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         optimizer = [torch.optim.Adam(policy.parameters_actor, config.lr_a, eps=1e-5),
                      torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
         scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config)),
                      torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config))]
```

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/ippo_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/ippo_agents.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,21 @@
         else:
             config.dim_state, state_shape = None, None
 
         input_representation = get_repre_in(config)
         self.use_recurrent = config.use_recurrent
         self.use_global_state = config.use_global_state
         # create representation for actor
-        kwargs_rnn = {"N_recurrent_layers": config.N_recurrent_layers,
-                      "dropout": config.dropout,
-                      "rnn": config.rnn} if self.use_recurrent else {}
+        if self.use_recurrent:
+            input_representation[0] = (config.dim_obs + config.dim_act, )
+            kwargs_rnn = {"N_recurrent_layers": config.N_recurrent_layers,
+                          "dropout": config.dropout,
+                          "rnn": config.rnn}
+        else:
+            kwargs_rnn = {}
         representation = REGISTRY_Representation[config.representation](*input_representation, **kwargs_rnn)
         # create representation for critic
         input_representation[0] = (config.dim_state,) if self.use_global_state else (config.dim_obs,)
         representation_critic = REGISTRY_Representation[config.representation](*input_representation, **kwargs_rnn)
         # create policy
         input_policy = get_policy_in_marl(config, (representation, representation_critic))
         policy = REGISTRY_Policy[config.policy](*input_policy,
@@ -61,14 +65,16 @@
         self.share_values = True if config.rew_shape[0] == 1 else False
         self.on_policy = True
 
     def act(self, obs_n, *rnn_hidden, avail_actions=None, state=None, test_mode=False):
         batch_size = len(obs_n)
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
         obs_in = torch.Tensor(obs_n).view([batch_size, self.n_agents, -1]).to(self.device)
+        if avail_actions is not None:
+            avail_actions = torch.Tensor(avail_actions).to(self.device)
         if self.use_recurrent:
             batch_agents = batch_size * self.n_agents
             hidden_state, dists = self.policy(obs_in.view(batch_agents, 1, -1),
                                               agents_id.view(batch_agents, 1, -1),
                                               *rnn_hidden,
                                               avail_actions=avail_actions.reshape(batch_agents, 1, -1))
             actions = dists.stochastic_sample()
```

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/iql_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/iql_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/isac_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/isac_agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.gamma = config.gamma
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         optimizer = [torch.optim.Adam(policy.parameters_actor, config.lr_a, eps=1e-5),
                      torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
         scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config)),
                      torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config))]
```

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/maddpg_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/maddpg_agents.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.gamma = config.gamma
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         optimizer = [torch.optim.Adam(policy.parameters_actor, config.lr_a, eps=1e-5),
                      torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
         scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
                                                        total_iters=config.running_steps),
                      torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
                                                        total_iters=config.running_steps)]
```

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/mappo_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/mappo_agents.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import torch
+
 from xuance.torch.agents import *
 
 
 class MAPPO_Agents(MARLAgents):
     """The implementation of MAPPO agents.
 
     Args:
@@ -22,17 +24,21 @@
         else:
             config.dim_state, state_shape = None, None
 
         input_representation = get_repre_in(config)
         self.use_recurrent = config.use_recurrent
         self.use_global_state = config.use_global_state
         # create representation for actor
-        kwargs_rnn = {"N_recurrent_layers": config.N_recurrent_layers,
-                      "dropout": config.dropout,
-                      "rnn": config.rnn} if self.use_recurrent else {}
+        if self.use_recurrent:
+            input_representation[0] = (config.dim_obs + config.dim_act, )
+            kwargs_rnn = {"N_recurrent_layers": config.N_recurrent_layers,
+                          "dropout": config.dropout,
+                          "rnn": config.rnn}
+        else:
+            kwargs_rnn = {}
         representation = REGISTRY_Representation[config.representation](*input_representation, **kwargs_rnn)
         # create representation for critic
         if self.use_global_state:
             input_representation[0] = (config.dim_state + config.dim_obs * config.n_agents,)
         else:
             input_representation[0] = (config.dim_obs * config.n_agents,)
         representation_critic = REGISTRY_Representation[config.representation](*input_representation, **kwargs_rnn)
@@ -62,19 +68,21 @@
                                            config.log_dir, config.model_dir)
         self.share_values = True if config.rew_shape[0] == 1 else False
         self.on_policy = True
 
     def act(self, obs_n, *rnn_hidden, avail_actions=None, state=None, test_mode=False):
         batch_size = len(obs_n)
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
-        obs_in = torch.Tensor(obs_n).view([batch_size, self.n_agents, -1]).to(self.device)
-        if self.use_recurrent:
+        obs_in = torch.Tensor(obs_n).reshape([batch_size, self.n_agents, -1]).to(self.device)
+        if avail_actions is not None:
+            avail_actions = torch.Tensor(avail_actions).to(self.device)
+        if self.use_recurrent:  # use recurrent networks
             batch_agents = batch_size * self.n_agents
-            hidden_state, dists = self.policy(obs_in.view(batch_agents, 1, -1),
-                                              agents_id.view(batch_agents, 1, -1),
+            hidden_state, dists = self.policy(obs_in.reshape(batch_agents, 1, -1),
+                                              agents_id.reshape(batch_agents, 1, -1),
                                               *rnn_hidden,
                                               avail_actions=avail_actions.reshape(batch_agents, 1, -1))
             actions = dists.stochastic_sample()
             log_pi_a = dists.log_prob(actions).reshape(batch_size, self.n_agents)
             actions = actions.reshape(batch_size, self.n_agents)
         else:
             hidden_state, dists = self.policy(obs_in, agents_id, avail_actions=avail_actions)
@@ -84,19 +92,19 @@
 
     def values(self, obs_n, *rnn_hidden, state=None):
         batch_size = len(obs_n)
         agents_id = torch.eye(self.n_agents).unsqueeze(0).expand(batch_size, -1, -1).to(self.device)
         # build critic input
         if self.use_global_state:
             state = torch.Tensor(state).unsqueeze(1).to(self.device)
-            obs_n = torch.Tensor(obs_n).view([batch_size, 1, -1]).to(self.device)
+            obs_n = torch.Tensor(obs_n).reshape([batch_size, 1, -1]).to(self.device)
             critic_in = torch.concat([obs_n.expand(-1, self.n_agents, -1),
                                       state.expand(-1, self.n_agents, -1)], dim=-1)
         else:
-            critic_in = torch.Tensor(obs_n).view([batch_size, 1, -1]).to(self.device)
+            critic_in = torch.Tensor(obs_n).reshape([batch_size, 1, -1]).to(self.device)
             critic_in = critic_in.expand(-1, self.n_agents, -1)
         # get critic values
         if self.use_recurrent:
             hidden_state, values_n = self.policy.get_values(critic_in.unsqueeze(2),  # add a sequence length axis.
                                                             agents_id.unsqueeze(2),
                                                             *rnn_hidden)
             values_n = values_n.squeeze(2)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/masac_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/masac_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.gamma = config.gamma
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         optimizer = [torch.optim.Adam(policy.parameters_actor, config.lr_a, eps=1e-5),
                      torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
         scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config)),
                      torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config))]
```

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/matd3_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/matd3_agents.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,24 +13,21 @@
                  config: Namespace,
                  envs: DummyVecEnv_Pettingzoo,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.gamma = config.gamma
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         optimizer = [torch.optim.Adam(policy.parameters_actor, config.lr_a, eps=1e-5),
-                     torch.optim.Adam(policy.critic_net_A.parameters(), config.lr_c, eps=1e-5),
-                     torch.optim.Adam(policy.critic_net_B.parameters(), config.lr_c, eps=1e-5)]
+                     torch.optim.Adam(policy.parameters_critic, config.lr_c, eps=1e-5)]
         scheduler = [torch.optim.lr_scheduler.LinearLR(optimizer[0], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config)),
                      torch.optim.lr_scheduler.LinearLR(optimizer[1], start_factor=1.0, end_factor=0.5,
-                                                       total_iters=get_total_iters(config.agent_name, config)),
-                     torch.optim.lr_scheduler.LinearLR(optimizer[2], start_factor=1.0, end_factor=0.5,
                                                        total_iters=get_total_iters(config.agent_name, config))]
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
         self.auxiliary_info_shape = {}
 
         if config.state_space is not None:
```

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/mfac_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/mfac_agents.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         if config.state_space is not None:
             config.dim_state, state_shape = config.state_space.shape, config.state_space.shape
         else:
             config.dim_state, state_shape = None, None
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy, gain=config.gain)
         optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
         scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
                                                       total_iters=get_total_iters(config.agent_name, config))
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
```

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/mfq_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/mfq_agents.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.egreedy = self.start_greedy
         self.delta_egreedy = (self.start_greedy - self.end_greedy) / config.decay_step_greedy
         self.use_recurrent, self.rnn = config.use_recurrent, config.rnn
         self.rnn_hidden = None
 
         input_representation = get_repre_in(config)
         representation = REGISTRY_Representation[config.representation](*input_representation)
-        input_policy = get_policy_in_marl(config, representation, config.agent_keys)
+        input_policy = get_policy_in_marl(config, representation)
         policy = REGISTRY_Policy[config.policy](*input_policy)
         optimizer = torch.optim.Adam(policy.parameters(), config.learning_rate, eps=1e-5)
         scheduler = torch.optim.lr_scheduler.LinearLR(optimizer, start_factor=1.0, end_factor=0.5,
                                                       total_iters=get_total_iters(config.agent_name, config))
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.representation_info_shape = policy.representation.output_shapes
```

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/qmix_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/qmix_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/qtran_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/qtran_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/vdac_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/vdac_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/vdn_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/vdn_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/agents/multi_agent_rl/wqmix_agents.py` & `xuance-1.1.0/xuance/torch/agents/multi_agent_rl/wqmix_agents.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/agents/policy_gradient/a2c_agent.py` & `xuance-1.1.0/xuance/torch/agents/policy_gradient/a2c_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/policy_gradient/ddpg_agent.py` & `xuance-1.1.0/xuance/torch/agents/policy_gradient/ddpg_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                         episode_videos = videos[i].copy()
                     if self.config.test_mode:
                         print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/policy_gradient/mpdqn_agent.py` & `xuance-1.1.0/xuance/torch/agents/policy_gradient/mpdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/agents/policy_gradient/pdqn_agent.py` & `xuance-1.1.0/xuance/torch/agents/policy_gradient/pdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/agents/policy_gradient/pg_agent.py` & `xuance-1.1.0/xuance/torch/agents/policy_gradient/pg_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/policy_gradient/ppg_agent.py` & `xuance-1.1.0/xuance/torch/agents/policy_gradient/ppg_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
                         episode_videos = videos[i].copy()
                     if self.config.test_mode:
                         print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/policy_gradient/ppoclip_agent.py` & `xuance-1.1.0/xuance/torch/agents/policy_gradient/ppokl_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from xuance.torch.agents import *
 
 
-class PPOCLIP_Agent(Agent):
-    """The implementation of PPO agent.
+class PPOKL_Agent(Agent):
+    """The implementation of PPO agent with KL divergence.
 
     Args:
         config: the Namespace variable that provides hyper-parameters and other settings.
         envs: the vectorized environments.
         policy: the neural network modules of the agent.
         optimizer: the method of optimizing.
         scheduler: the learning rate decay scheduler.
@@ -25,76 +25,73 @@
         self.n_minibatch = config.n_minibatch
         self.n_epoch = config.n_epoch
 
         self.gamma = config.gamma
         self.gae_lam = config.gae_lambda
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
-        self.auxiliary_info_shape = {"old_logp": ()}
+        self.auxiliary_info_shape = {"old_dist": None}
 
         self.atari = True if config.env_name == "Atari" else False
-        Buffer = DummyOnPolicyBuffer_Atari if self.atari else DummyOnPolicyBuffer
+        Buffer = DummyOnPolicyBuffer_Atari if self.atari else DummyOnPolicyBuffer_Atari
         self.buffer_size = self.n_envs * self.n_steps
         self.batch_size = self.buffer_size // self.n_minibatch
         memory = Buffer(self.observation_space,
                         self.action_space,
                         self.auxiliary_info_shape,
                         self.n_envs,
                         self.n_steps,
                         config.use_gae,
                         config.use_advnorm,
                         self.gamma,
                         self.gae_lam)
-        learner = PPOCLIP_Learner(policy,
-                                  optimizer,
-                                  scheduler,
-                                  config.device,
-                                  config.model_dir,
-                                  vf_coef=config.vf_coef,
-                                  ent_coef=config.ent_coef,
-                                  clip_range=config.clip_range,
-                                  clip_grad_norm=config.clip_grad_norm,
-                                  use_grad_clip=config.use_grad_clip)
-        super(PPOCLIP_Agent, self).__init__(config, envs, policy, memory, learner, device,
-                                            config.log_dir, config.model_dir)
+        learner = PPOKL_Learner(policy,
+                                optimizer,
+                                scheduler,
+                                config.device,
+                                config.model_dir,
+                                config.vf_coef,
+                                config.ent_coef,
+                                config.target_kl)
+        super(PPOKL_Agent, self).__init__(config, envs, policy, memory, learner, device,
+                                          config.log_dir, config.model_dir)
 
     def _action(self, obs):
         _, dists, vs = self.policy(obs)
         acts = dists.stochastic_sample()
-        logps = dists.log_prob(acts)
         vs = vs.detach().cpu().numpy()
         acts = acts.detach().cpu().numpy()
-        logps = logps.detach().cpu().numpy()
-        return acts, vs, logps
+        return acts, vs, split_distributions(dists)
 
     def train(self, train_steps):
         obs = self.envs.buf_obs
         for _ in tqdm(range(train_steps)):
             step_info = {}
             self.obs_rms.update(obs)
             obs = self._process_observation(obs)
-            acts, value, logps = self._action(obs)
+            acts, values, dists = self._action(obs)
             next_obs, rewards, terminals, trunctions, infos = self.envs.step(acts)
 
-            self.memory.store(obs, acts, self._process_reward(rewards), value, terminals, {"old_logp": logps})
+            self.memory.store(obs, acts, self._process_reward(rewards), values, terminals, {"old_dist": dists})
             if self.memory.full:
                 _, vals, _ = self._action(self._process_observation(next_obs))
                 for i in range(self.n_envs):
                     if terminals[i]:
                         self.memory.finish_path(0.0, i)
                     else:
                         self.memory.finish_path(vals[i], i)
                 indexes = np.arange(self.buffer_size)
                 for _ in range(self.n_epoch):
                     np.random.shuffle(indexes)
                     for start in range(0, self.buffer_size, self.batch_size):
                         end = start + self.batch_size
                         sample_idx = indexes[start:end]
-                        obs_batch, act_batch, ret_batch, value_batch, adv_batch, aux_batch = self.memory.sample(sample_idx)
-                        step_info = self.learner.update(obs_batch, act_batch, ret_batch, value_batch, adv_batch, aux_batch['old_logp'])
+                        obs_batch, act_batch, ret_batch, value_batch, adv_batch, aux_batch = self.memory.sample(
+                            sample_idx)
+                        step_info = self.learner.update(obs_batch, act_batch, ret_batch, adv_batch, aux_batch['old_dist'])
                 self.log_infos(step_info, self.current_step)
                 self.memory.clear()
 
             self.returns = (1 - terminals) * self.gamma * self.returns + rewards
             obs = next_obs
             for i in range(self.n_envs):
                 if terminals[i] or trunctions[i]:
@@ -155,15 +152,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/policy_gradient/ppokl_agent.py` & `xuance-1.1.0/xuance/torch/agents/qlearning_family/drqn_agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from xuance.torch.agents import *
 
 
-class PPOKL_Agent(Agent):
-    """The implementation of PPO agent with KL divergence.
+class DRQN_Agent(Agent):
+    """The implementation of Deep Recurrent Q-Netowrk (DRQN) agent.
 
     Args:
         config: the Namespace variable that provides hyper-parameters and other settings.
         envs: the vectorized environments.
         policy: the neural network modules of the agent.
         optimizer: the method of optimizing.
         scheduler: the learning rate decay scheduler.
@@ -17,152 +17,144 @@
                  envs: DummyVecEnv_Gym,
                  policy: nn.Module,
                  optimizer: torch.optim.Optimizer,
                  scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
                  device: Optional[Union[int, str, torch.device]] = None):
         self.render = config.render
         self.n_envs = envs.num_envs
-        self.n_steps = config.n_steps
-        self.n_minibatch = config.n_minibatch
-        self.n_epoch = config.n_epoch
 
         self.gamma = config.gamma
-        self.gae_lam = config.gae_lambda
+        self.train_frequency = config.training_frequency
+        self.start_training = config.start_training
+        self.start_greedy = config.start_greedy
+        self.end_greedy = config.end_greedy
+        self.egreedy = config.start_greedy
+
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
-        self.representation_info_shape = policy.representation_actor.output_shapes
-        self.auxiliary_info_shape = {"old_dist": None}
+        self.auxiliary_info_shape = {}
 
         self.atari = True if config.env_name == "Atari" else False
-        Buffer = DummyOnPolicyBuffer_Atari if self.atari else DummyOnPolicyBuffer_Atari
-        self.buffer_size = self.n_envs * self.n_steps
-        self.batch_size = self.buffer_size // self.n_minibatch
-        memory = Buffer(self.observation_space,
-                        self.action_space,
-                        self.auxiliary_info_shape,
-                        self.n_envs,
-                        self.n_steps,
-                        config.use_gae,
-                        config.use_advnorm,
-                        self.gamma,
-                        self.gae_lam)
-        learner = PPOKL_Learner(policy,
-                                optimizer,
-                                scheduler,
-                                config.device,
-                                config.model_dir,
-                                config.vf_coef,
-                                config.ent_coef,
-                                config.target_kl)
-        super(PPOKL_Agent, self).__init__(config, envs, policy, memory, learner, device,
-                                          config.log_dir, config.model_dir)
-
-    def _action(self, obs):
-        _, dists, vs = self.policy(obs)
-        acts = dists.stochastic_sample()
-        vs = vs.detach().cpu().numpy()
-        acts = acts.detach().cpu().numpy()
-        return acts, vs, split_distributions(dists)
+        memory = RecurrentOffPolicyBuffer(self.observation_space,
+                                          self.action_space,
+                                          self.auxiliary_info_shape,
+                                          self.n_envs,
+                                          config.n_size,
+                                          config.batch_size,
+                                          episode_length=envs.max_episode_length,
+                                          lookup_length=config.lookup_length)
+        learner = DRQN_Learner(policy,
+                               optimizer,
+                               scheduler,
+                               config.device,
+                               config.model_dir,
+                               config.gamma,
+                               config.sync_frequency)
+        super(DRQN_Agent, self).__init__(config, envs, policy, memory, learner, device,
+                                         config.log_dir, config.model_dir)
+        self.lstm = True if config.rnn == "LSTM" else False
+
+    def _action(self, obs, egreedy=0.0, rnn_hidden=None):
+        _, argmax_action, _, rnn_hidden_next = self.policy(obs[:, np.newaxis], *rnn_hidden)
+        random_action = np.random.choice(self.action_space.n, self.n_envs)
+        if np.random.rand() < egreedy:
+            action = random_action
+        else:
+            action = argmax_action.detach().cpu().numpy()
+        return action, rnn_hidden_next
 
     def train(self, train_steps):
         obs = self.envs.buf_obs
+        episode_data = [EpisodeBuffer() for _ in range(self.n_envs)]
+        for i_env in range(self.n_envs):
+            episode_data[i_env].obs.append(self._process_observation(obs[i_env]))
+        self.rnn_hidden = self.policy.init_hidden(self.n_envs)
+        dones = [False for _ in range(self.n_envs)]
         for _ in tqdm(range(train_steps)):
             step_info = {}
             self.obs_rms.update(obs)
             obs = self._process_observation(obs)
-            acts, values, dists = self._action(obs)
+            acts, self.rnn_hidden = self._action(obs, self.egreedy, self.rnn_hidden)
             next_obs, rewards, terminals, trunctions, infos = self.envs.step(acts)
 
-            self.memory.store(obs, acts, self._process_reward(rewards), values, terminals, {"old_dist": dists})
-            if self.memory.full:
-                _, vals, _ = self._action(self._process_observation(next_obs))
-                for i in range(self.n_envs):
-                    if terminals[i]:
-                        self.memory.finish_path(0.0, i)
-                    else:
-                        self.memory.finish_path(vals[i], i)
-                indexes = np.arange(self.buffer_size)
-                for _ in range(self.n_epoch):
-                    np.random.shuffle(indexes)
-                    for start in range(0, self.buffer_size, self.batch_size):
-                        end = start + self.batch_size
-                        sample_idx = indexes[start:end]
-                        obs_batch, act_batch, ret_batch, value_batch, adv_batch, aux_batch = self.memory.sample(
-                            sample_idx)
-                        step_info = self.learner.update(obs_batch, act_batch, ret_batch, value_batch, adv_batch,
-                                                        aux_batch['old_logp'])
+            if (self.current_step > self.start_training) and (self.current_step % self.train_frequency == 0):
+                # training
+                obs_batch, act_batch, rew_batch, terminal_batch = self.memory.sample()
+                step_info = self.learner.update(obs_batch, act_batch, rew_batch, terminal_batch)
+                step_info["epsilon-greedy"] = self.egreedy
                 self.log_infos(step_info, self.current_step)
-                self.memory.clear()
 
-            self.returns = (1 - terminals) * self.gamma * self.returns + rewards
             obs = next_obs
             for i in range(self.n_envs):
+                episode_data[i].put([self._process_observation(obs[i]), acts[i], self._process_reward(rewards[i]), terminals[i]])
                 if terminals[i] or trunctions[i]:
-                    self.ret_rms.update(self.returns[i:i + 1])
-                    self.returns[i] = 0.0
                     if self.atari and (~trunctions[i]):
                         pass
                     else:
-                        if terminals[i]:
-                            self.memory.finish_path(0.0, i)
-                        else:
-                            _, vals, _ = self._action(self._process_observation(next_obs))
-                            self.memory.finish_path(vals[i], i)
-                        obs[i] = infos[i]["reset_obs"]
+                        self.rnn_hidden = self.policy.init_hidden_item(self.rnn_hidden, i)
+                        dones[i] = True
                         self.current_episode[i] += 1
                         if self.use_wandb:
                             step_info["Episode-Steps/env-%d" % i] = infos[i]["episode_step"]
                             step_info["Train-Episode-Rewards/env-%d" % i] = infos[i]["episode_score"]
                         else:
                             step_info["Episode-Steps"] = {"env-%d" % i: infos[i]["episode_step"]}
                             step_info["Train-Episode-Rewards"] = {"env-%d" % i: infos[i]["episode_score"]}
                         self.log_infos(step_info, self.current_step)
+                        self.memory.store(episode_data[i])
+                        episode_data[i] = EpisodeBuffer()
+                        obs[i] = infos[i]["reset_obs"]
+                        episode_data[i].obs.append(self._process_observation(obs[i]))
 
             self.current_step += self.n_envs
+            if self.egreedy > self.end_greedy:
+                self.egreedy = self.egreedy - (self.start_greedy - self.end_greedy) / self.config.decay_step_greedy
 
-    def test(self, env_fn, test_episode):
+    def test(self, env_fn, test_episodes):
         test_envs = env_fn()
         num_envs = test_envs.num_envs
         videos, episode_videos = [[] for _ in range(num_envs)], []
         current_episode, scores, best_score = 0, [], -np.inf
         obs, infos = test_envs.reset()
         if self.config.render_mode == "rgb_array" and self.render:
             images = test_envs.render(self.config.render_mode)
             for idx, img in enumerate(images):
                 videos[idx].append(img)
 
-        while current_episode < test_episode:
+        rnn_hidden = self.policy.init_hidden(num_envs)
+        while current_episode < test_episodes:
             self.obs_rms.update(obs)
             obs = self._process_observation(obs)
-            acts, rets, logps = self._action(obs)
+            acts, rnn_hidden = self._action(obs, egreedy=0.0, rnn_hidden=rnn_hidden)
             next_obs, rewards, terminals, trunctions, infos = test_envs.step(acts)
             if self.config.render_mode == "rgb_array" and self.render:
                 images = test_envs.render(self.config.render_mode)
                 for idx, img in enumerate(images):
                     videos[idx].append(img)
 
             obs = next_obs
             for i in range(num_envs):
                 if terminals[i] or trunctions[i]:
                     if self.atari and (~trunctions[i]):
                         pass
                     else:
                         obs[i] = infos[i]["reset_obs"]
+                        rnn_hidden = self.policy.init_hidden_item(rnn_hidden, i)
                         scores.append(infos[i]["episode_score"])
                         current_episode += 1
                         if best_score < infos[i]["episode_score"]:
                             best_score = infos[i]["episode_score"]
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/policy_gradient/sac_agent.py` & `xuance-1.1.0/xuance/torch/agents/policy_gradient/sac_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                               config.model_dir,
                               config.gamma,
                               config.tau)
         super(SAC_Agent, self).__init__(config, envs, policy, memory, learner, device, config.log_dir, config.model_dir)
 
     def _action(self, obs):
         _, act_dist = self.policy(obs)
-        action = act_dist.sample()
+        action = act_dist.rsample()
         action = action.detach().cpu().numpy()
         return action
 
     def train(self, train_steps):
         obs = self.envs.buf_obs
         for _ in tqdm(range(train_steps)):
             step_info = {}
@@ -121,15 +121,15 @@
                         episode_videos = videos[i].copy()
                     if self.config.test_mode:
                         print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/policy_gradient/sacdis_agent.py` & `xuance-1.1.0/xuance/torch/agents/policy_gradient/sacdis_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/policy_gradient/spdqn_agent.py` & `xuance-1.1.0/xuance/torch/agents/policy_gradient/spdqn_agent.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/agents/policy_gradient/td3_agent.py` & `xuance-1.1.0/xuance/torch/agents/policy_gradient/td3_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                         episode_videos = videos[i].copy()
                     if self.config.test_mode:
                         print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/qlearning_family/c51_agent.py` & `xuance-1.1.0/xuance/torch/agents/qlearning_family/c51_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/qlearning_family/ddqn_agent.py` & `xuance-1.1.0/xuance/torch/agents/qlearning_family/ddqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/qlearning_family/dqn_agent.py` & `xuance-1.1.0/xuance/torch/agents/qlearning_family/qrdqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from xuance.torch.agents import *
 
 
-class DQN_Agent(Agent):
-    """The implementation of DQN agent.
+class QRDQN_Agent(Agent):
+    """The implementation of QRDQN agent.
 
     Args:
         config: the Namespace variable that provides hyper-parameters and other settings.
         envs: the vectorized environments.
         policy: the neural network modules of the agent.
         optimizer: the method of optimizing.
         scheduler: the learning rate decay scheduler.
@@ -28,30 +28,32 @@
         self.start_greedy = config.start_greedy
         self.end_greedy = config.end_greedy
         self.egreedy = config.start_greedy
 
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.auxiliary_info_shape = {}
+
         self.atari = True if config.env_name == "Atari" else False
         Buffer = DummyOffPolicyBuffer_Atari if self.atari else DummyOffPolicyBuffer
         memory = Buffer(self.observation_space,
                         self.action_space,
                         self.auxiliary_info_shape,
                         self.n_envs,
                         config.n_size,
                         config.batch_size)
-        learner = DQN_Learner(policy,
-                              optimizer,
-                              scheduler,
-                              config.device,
-                              config.model_dir,
-                              config.gamma,
-                              config.sync_frequency)
-        super(DQN_Agent, self).__init__(config, envs, policy, memory, learner, device, config.log_dir, config.model_dir)
+        learner = QRDQN_Learner(policy,
+                                optimizer,
+                                scheduler,
+                                config.device,
+                                config.model_dir,
+                                config.gamma,
+                                config.sync_frequency)
+        super(QRDQN_Agent, self).__init__(config, envs, policy, memory, learner, device,
+                                          config.log_dir, config.model_dir)
 
     def _action(self, obs, egreedy=0.0):
         _, argmax_action, _ = self.policy(obs)
         random_action = np.random.choice(self.action_space.n, self.n_envs)
         if np.random.rand() < egreedy:
             action = random_action
         else:
@@ -88,15 +90,15 @@
                             step_info["Train-Episode-Rewards/env-%d" % i] = infos[i]["episode_score"]
                         else:
                             step_info["Episode-Steps"] = {"env-%d" % i: infos[i]["episode_step"]}
                             step_info["Train-Episode-Rewards"] = {"env-%d" % i: infos[i]["episode_score"]}
                         self.log_infos(step_info, self.current_step)
 
             self.current_step += self.n_envs
-            if self.egreedy >= self.end_greedy:
+            if self.egreedy > self.end_greedy:
                 self.egreedy = self.egreedy - (self.start_greedy - self.end_greedy) / self.config.decay_step_greedy
 
     def test(self, env_fn, test_episodes):
         test_envs = env_fn()
         num_envs = test_envs.num_envs
         videos, episode_videos = [[] for _ in range(num_envs)], []
         current_episode, scores, best_score = 0, [], -np.inf
@@ -130,15 +132,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/qlearning_family/drqn_agent.py` & `xuance-1.1.0/xuance/torch/agents/qlearning_family/dqn_agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from xuance.torch.agents import *
 
 
-class DRQN_Agent(Agent):
-    """The implementation of Deep Recurrent Q-Netowrk (DRQN) agent.
+class DQN_Agent(Agent):
+    """The implementation of DQN agent.
 
     Args:
         config: the Namespace variable that provides hyper-parameters and other settings.
         envs: the vectorized environments.
         policy: the neural network modules of the agent.
         optimizer: the method of optimizing.
         scheduler: the learning rate decay scheduler.
@@ -28,133 +28,117 @@
         self.start_greedy = config.start_greedy
         self.end_greedy = config.end_greedy
         self.egreedy = config.start_greedy
 
         self.observation_space = envs.observation_space
         self.action_space = envs.action_space
         self.auxiliary_info_shape = {}
-
         self.atari = True if config.env_name == "Atari" else False
-        memory = RecurrentOffPolicyBuffer(self.observation_space,
-                                          self.action_space,
-                                          self.auxiliary_info_shape,
-                                          self.n_envs,
-                                          config.n_size,
-                                          config.batch_size,
-                                          episode_length=envs.max_episode_length,
-                                          lookup_length=config.lookup_length)
-        learner = DRQN_Learner(policy,
-                               optimizer,
-                               scheduler,
-                               config.device,
-                               config.model_dir,
-                               config.gamma,
-                               config.sync_frequency)
-        super(DRQN_Agent, self).__init__(config, envs, policy, memory, learner, device,
-                                         config.log_dir, config.model_dir)
-        self.lstm = True if config.rnn == "LSTM" else False
+        Buffer = DummyOffPolicyBuffer_Atari if self.atari else DummyOffPolicyBuffer
+        memory = Buffer(self.observation_space,
+                        self.action_space,
+                        self.auxiliary_info_shape,
+                        self.n_envs,
+                        config.n_size,
+                        config.batch_size)
+        learner = DQN_Learner(policy,
+                              optimizer,
+                              scheduler,
+                              config.device,
+                              config.model_dir,
+                              config.gamma,
+                              config.sync_frequency)
+        super(DQN_Agent, self).__init__(config, envs, policy, memory, learner, device, config.log_dir, config.model_dir)
 
-    def _action(self, obs, egreedy=0.0, rnn_hidden=None):
-        _, argmax_action, _, rnn_hidden_next = self.policy(obs[:, np.newaxis], *rnn_hidden)
+    def _action(self, obs, egreedy=0.0):
+        _, argmax_action, _ = self.policy(obs)
         random_action = np.random.choice(self.action_space.n, self.n_envs)
         if np.random.rand() < egreedy:
             action = random_action
         else:
             action = argmax_action.detach().cpu().numpy()
-        return action, rnn_hidden_next
+        return action
 
     def train(self, train_steps):
         obs = self.envs.buf_obs
-        episode_data = [EpisodeBuffer() for _ in range(self.n_envs)]
-        for i_env in range(self.n_envs):
-            episode_data[i_env].obs.append(self._process_observation(obs[i_env]))
-        self.rnn_hidden = self.policy.init_hidden(self.n_envs)
-        dones = [False for _ in range(self.n_envs)]
         for _ in tqdm(range(train_steps)):
             step_info = {}
             self.obs_rms.update(obs)
             obs = self._process_observation(obs)
-            acts, self.rnn_hidden = self._action(obs, self.egreedy, self.rnn_hidden)
+            acts = self._action(obs, self.egreedy)
             next_obs, rewards, terminals, trunctions, infos = self.envs.step(acts)
 
-            if (self.current_step > self.start_training) and (self.current_step % self.train_frequency == 0):
+            self.memory.store(obs, acts, self._process_reward(rewards), terminals, self._process_observation(next_obs))
+            if self.current_step > self.start_training and self.current_step % self.train_frequency == 0:
                 # training
-                obs_batch, act_batch, rew_batch, terminal_batch = self.memory.sample()
-                step_info = self.learner.update(obs_batch, act_batch, rew_batch, terminal_batch)
+                obs_batch, act_batch, rew_batch, terminal_batch, next_batch = self.memory.sample()
+                step_info = self.learner.update(obs_batch, act_batch, rew_batch, next_batch, terminal_batch)
                 step_info["epsilon-greedy"] = self.egreedy
                 self.log_infos(step_info, self.current_step)
 
             obs = next_obs
             for i in range(self.n_envs):
-                episode_data[i].put([self._process_observation(obs[i]), acts[i], self._process_reward(rewards[i]), terminals[i]])
                 if terminals[i] or trunctions[i]:
                     if self.atari and (~trunctions[i]):
                         pass
                     else:
-                        self.rnn_hidden = self.policy.init_hidden_item(self.rnn_hidden, i)
-                        dones[i] = True
+                        obs[i] = infos[i]["reset_obs"]
                         self.current_episode[i] += 1
                         if self.use_wandb:
                             step_info["Episode-Steps/env-%d" % i] = infos[i]["episode_step"]
                             step_info["Train-Episode-Rewards/env-%d" % i] = infos[i]["episode_score"]
                         else:
                             step_info["Episode-Steps"] = {"env-%d" % i: infos[i]["episode_step"]}
                             step_info["Train-Episode-Rewards"] = {"env-%d" % i: infos[i]["episode_score"]}
                         self.log_infos(step_info, self.current_step)
-                        self.memory.store(episode_data[i])
-                        episode_data[i] = EpisodeBuffer()
-                        obs[i] = infos[i]["reset_obs"]
-                        episode_data[i].obs.append(self._process_observation(obs[i]))
 
             self.current_step += self.n_envs
-            if self.egreedy > self.end_greedy:
+            if self.egreedy >= self.end_greedy:
                 self.egreedy = self.egreedy - (self.start_greedy - self.end_greedy) / self.config.decay_step_greedy
 
     def test(self, env_fn, test_episodes):
         test_envs = env_fn()
         num_envs = test_envs.num_envs
         videos, episode_videos = [[] for _ in range(num_envs)], []
         current_episode, scores, best_score = 0, [], -np.inf
         obs, infos = test_envs.reset()
         if self.config.render_mode == "rgb_array" and self.render:
             images = test_envs.render(self.config.render_mode)
             for idx, img in enumerate(images):
                 videos[idx].append(img)
 
-        rnn_hidden = self.policy.init_hidden(num_envs)
         while current_episode < test_episodes:
             self.obs_rms.update(obs)
             obs = self._process_observation(obs)
-            acts, rnn_hidden = self._action(obs, egreedy=0.0, rnn_hidden=rnn_hidden)
+            acts = self._action(obs, egreedy=0.0)
             next_obs, rewards, terminals, trunctions, infos = test_envs.step(acts)
             if self.config.render_mode == "rgb_array" and self.render:
                 images = test_envs.render(self.config.render_mode)
                 for idx, img in enumerate(images):
                     videos[idx].append(img)
 
             obs = next_obs
             for i in range(num_envs):
                 if terminals[i] or trunctions[i]:
                     if self.atari and (~trunctions[i]):
                         pass
                     else:
                         obs[i] = infos[i]["reset_obs"]
-                        rnn_hidden = self.policy.init_hidden_item(rnn_hidden, i)
                         scores.append(infos[i]["episode_score"])
                         current_episode += 1
                         if best_score < infos[i]["episode_score"]:
                             best_score = infos[i]["episode_score"]
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/qlearning_family/dueldqn_agent.py` & `xuance-1.1.0/xuance/torch/agents/qlearning_family/dueldqn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/qlearning_family/noisydqn_agent.py` & `xuance-1.1.0/xuance/torch/agents/qlearning_family/noisydqn_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/agents/qlearning_family/perdqn_agent.py` & `xuance-1.1.0/xuance/torch/agents/qlearning_family/perdqn_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
                             episode_videos = videos[i].copy()
                         if self.config.test_mode:
                             print("Episode: %d, Score: %.2f" % (current_episode, infos[i]["episode_score"]))
 
         if self.config.render_mode == "rgb_array" and self.render:
             # time, height, width, channel -> time, channel, height, width
             videos_info = {"Videos_Test": np.array([episode_videos], dtype=np.uint8).transpose((0, 1, 4, 2, 3))}
-            self.log_videos(info=videos_info, fps=50, x_index=self.current_step)
+            self.log_videos(info=videos_info, fps=self.fps, x_index=self.current_step)
 
         if self.config.test_mode:
             print("Best Score: %.2f" % (best_score))
 
         test_info = {
             "Test-Episode-Rewards/Mean-Score": np.mean(scores),
             "Test-Episode-Rewards/Std-Score": np.std(scores)
```

### Comparing `xuance-1.0.9/xuance/torch/learners/learner.py` & `xuance-1.1.0/xuance/torch/learners/learner.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,36 +20,45 @@
         self.device = device
         self.model_dir = model_dir
         self.iterations = 0
 
     def save_model(self, model_path):
         torch.save(self.policy.state_dict(), model_path)
 
-    def load_model(self, path, seed=1):
+    def load_model(self, path, model=None):
         file_names = os.listdir(path)
-        for f in file_names:
-            '''Change directory to the specified seed (if exists)'''
-            if f"seed_{seed}" in f:
-                path = os.path.join(path, f)
-                break
+        if model is not None:
+            path = os.path.join(path, model)
+            if model not in file_names:
+                raise RuntimeError(f"The folder '{path}' does not exist, please specify a correct path to load model.")
+        else:
+            for f in file_names:
+                if "seed_" not in f:
+                    file_names.remove(f)
+            file_names.sort()
+            path = os.path.join(path, file_names[-1])
+
         model_names = os.listdir(path)
         if os.path.exists(path + "/obs_rms.npy"):
             model_names.remove("obs_rms.npy")
+        if len(model_names) == 0:
+            raise RuntimeError(f"There is no model file in '{path}'!")
         model_names.sort()
         model_path = os.path.join(path, model_names[-1])
         self.policy.load_state_dict(torch.load(model_path, map_location={
             "cuda:0": self.device,
             "cuda:1": self.device,
             "cuda:2": self.device,
             "cuda:3": self.device,
             "cuda:4": self.device,
             "cuda:5": self.device,
             "cuda:6": self.device,
             "cuda:7": self.device
         }))
+        print(f"Successfully load model from '{path}'.")
 
     @abstractmethod
     def update(self, *args):
         raise NotImplementedError
 
 
 class LearnerMAS(ABC):
@@ -81,36 +90,45 @@
 
     def onehot_action(self, actions_int, num_actions):
         return F.one_hot(actions_int.long(), num_classes=num_actions)
 
     def save_model(self, model_path):
         torch.save(self.policy.state_dict(), model_path)
 
-    def load_model(self, path, seed=1):
+    def load_model(self, path, model=None):
         file_names = os.listdir(path)
-        for f in file_names:
-            '''Change directory to the specified seed (if exists)'''
-            if f"seed_{seed}" in f:
-                path = os.path.join(path, f)
-                break
+        if model is not None:
+            path = os.path.join(path, model)
+            if model not in file_names:
+                raise RuntimeError(f"The folder '{path}' does not exist, please specify a correct path to load model.")
+        else:
+            for f in file_names:
+                if "seed_" not in f:
+                    file_names.remove(f)
+            file_names.sort()
+            path = os.path.join(path, file_names[-1])
+
         model_names = os.listdir(path)
         if os.path.exists(path + "/obs_rms.npy"):
             model_names.remove("obs_rms.npy")
+        if len(model_names) == 0:
+            raise RuntimeError(f"There is no model file in '{path}'!")
         model_names.sort()
         model_path = os.path.join(path, model_names[-1])
         self.policy.load_state_dict(torch.load(model_path, map_location={
             "cuda:0": self.device,
             "cuda:1": self.device,
             "cuda:2": self.device,
             "cuda:3": self.device,
             "cuda:4": self.device,
             "cuda:5": self.device,
             "cuda:6": self.device,
             "cuda:7": self.device
         }))
+        print(f"Successfully load model from '{path}'.")
 
     @abstractmethod
     def update(self, *args):
         raise NotImplementedError
 
     def update_recurrent(self, *args):
         pass
```

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/coma_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/coma_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/dcg_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/dcg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/iddpg_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/iddpg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/ippo_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/ippo_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/iql_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/iql_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/isac_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/isac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/maddpg_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/maddpg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/mappo_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/mappo_learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,32 +69,40 @@
         entropy = pi_dist.entropy().reshape(agent_mask.shape) * agent_mask
         loss_e = entropy.mean()
 
         # critic loss
         critic_in = torch.Tensor(obs).reshape([batch_size, 1, -1]).to(self.device)
         critic_in = critic_in.expand(-1, self.n_agents, -1)
         _, value_pred = self.policy.get_values(critic_in, IDs)
-        value_pred = value_pred
-        value_target = returns
+        value_pred = value_pred.reshape(-1, 1)
+        value_target = returns.reshape(-1, 1)
+        values = values.reshape(-1, 1)
+        agent_mask_flatten = agent_mask.reshape(-1, 1)
         if self.use_value_clip:
             value_clipped = values + (value_pred - values).clamp(-self.value_clip_range, self.value_clip_range)
+            if self.use_value_norm:
+                self.value_normalizer.update(value_target)
+                value_target = self.value_normalizer.normalize(value_target)
             if self.use_huber_loss:
                 loss_v = self.huber_loss(value_pred, value_target)
                 loss_v_clipped = self.huber_loss(value_clipped, value_target)
             else:
                 loss_v = (value_pred - value_target) ** 2
                 loss_v_clipped = (value_clipped - value_target) ** 2
-            loss_c = torch.max(loss_v, loss_v_clipped) * agent_mask
-            loss_c = loss_c.sum() / agent_mask.sum()
+            loss_c = torch.max(loss_v, loss_v_clipped) * agent_mask_flatten
+            loss_c = loss_c.sum() / agent_mask_flatten.sum()
         else:
+            if self.use_value_norm:
+                self.value_normalizer.update(value_target)
+                value_target = self.value_normalizer.normalize(value_target)
             if self.use_huber_loss:
-                loss_v = self.huber_loss(value_pred, value_target) * agent_mask
+                loss_v = self.huber_loss(value_pred, value_target) * agent_mask_flatten
             else:
-                loss_v = ((value_pred - value_target) ** 2) * agent_mask
-            loss_c = loss_v.sum() / agent_mask.sum()
+                loss_v = ((value_pred - value_target) ** 2) * agent_mask_flatten
+            loss_c = loss_v.sum() / agent_mask_flatten.sum()
 
         loss = loss_a + self.vf_coef * loss_c - self.ent_coef * loss_e
         self.optimizer.zero_grad()
         loss.backward()
         if self.use_grad_norm:
             grad_norm = torch.nn.utils.clip_grad_norm_(self.policy.parameters(), self.max_grad_norm)
             info["gradient_norm"] = grad_norm.item()
@@ -156,19 +164,18 @@
         # critic loss
         rnn_hidden_critic = self.policy.representation_critic.init_hidden(batch_size * self.n_agents)
         if self.use_global_state:
             critic_in_obs = obs[:, :, :-1].transpose(1, 2).reshape(batch_size, episode_length, -1)
             critic_in_obs = critic_in_obs.unsqueeze(1).expand(-1, self.n_agents, -1, -1)
             critic_in_state = state[:, :, :-1]
             critic_in = torch.concat([critic_in_obs, critic_in_state], dim=-1)
-            _, value_pred = self.policy.get_values(critic_in, IDs[:, :, :-1], *rnn_hidden_critic)
         else:
             critic_in = obs[:, :, :-1].transpose(1, 2).reshape(batch_size, episode_length, -1)
             critic_in = critic_in.unsqueeze(1).expand(-1, self.n_agents, -1, -1)
-            _, value_pred = self.policy.get_values(critic_in, IDs[:, :, :-1], *rnn_hidden_critic)
+        _, value_pred = self.policy.get_values(critic_in, IDs[:, :, :-1], *rnn_hidden_critic)
         value_target = returns.reshape(-1, 1)
         values = values.reshape(-1, 1)
         value_pred = value_pred.reshape(-1, 1)
         filled_all = filled_n.reshape(-1, 1)
         if self.use_value_clip:
             value_clipped = values + (value_pred - values).clamp(-self.value_clip_range, self.value_clip_range)
             if self.use_value_norm:
@@ -181,15 +188,15 @@
                 loss_v = (value_pred - value_target) ** 2
                 loss_v_clipped = (value_clipped - value_target) ** 2
             loss_c = torch.max(loss_v, loss_v_clipped) * filled_all
             loss_c = loss_c.sum() / filled_all.sum()
         else:
             if self.use_value_norm:
                 self.value_normalizer.update(value_target)
-                value_pred = self.value_normalizer.normalize(value_pred)
+                value_pred = self.value_normalizer.normalize(value_target)
             if self.use_huber_loss:
                 loss_v = self.huber_loss(value_pred, value_target)
             else:
                 loss_v = (value_pred - value_target) ** 2
             loss_c = (loss_v * filled_all).sum() / filled_all.sum()
 
         loss = loss_a + self.vf_coef * loss_c - self.ent_coef * loss_e
```

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/masac_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/masac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/matd3_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/matd3_learner.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,21 +20,19 @@
         self.tau = config.tau
         self.delay = delay
         self.sync_frequency = sync_frequency
         self.mse_loss = nn.MSELoss()
         super(MATD3_Learner, self).__init__(config, policy, optimizer, scheduler, device, model_dir)
         self.optimizer = {
             'actor': optimizer[0],
-            'critic_A': optimizer[1],
-            'critic_B': optimizer[2]
+            'critic': optimizer[1]
         }
         self.scheduler = {
             'actor': scheduler[0],
-            'critic_A': scheduler[1],
-            'critic_B': scheduler[2]
+            'critic': scheduler[1]
         }
 
     def update(self, sample):
         self.iterations += 1
         obs = torch.Tensor(sample['obs']).to(self.device)
         actions = torch.Tensor(sample['actions']).to(self.device)
         obs_next = torch.Tensor(sample['obs_next']).to(self.device)
@@ -47,44 +45,38 @@
         _, action_q = self.policy.Qaction(obs, actions, IDs)
         actions_next = self.policy.target_actor(obs_next, IDs)
         _, target_q = self.policy.Qtarget(obs_next, actions_next, IDs)
         q_target = rewards + (1 - terminals) * self.args.gamma * target_q
         td_error = (action_q - q_target.detach()) * agent_mask
         loss_c = (td_error ** 2).sum() / agent_mask.sum()
         # loss_c = F.mse_loss(torch.tile(q_target.detach(), (1, 2)), action_q)
-        self.optimizer['critic_B'].zero_grad()
-        self.optimizer['critic_A'].zero_grad()
+        self.optimizer['critic'].zero_grad()
         loss_c.backward()
         torch.nn.utils.clip_grad_norm_(self.policy.parameters_critic, self.args.grad_clip_norm)
-        self.optimizer['critic_A'].step()
-        self.optimizer['critic_B'].step()
-        if self.scheduler['critic_A'] is not None:
-            self.scheduler['critic_A'].step()
-            self.scheduler['critic_B'].step()
+        self.optimizer['critic'].step()
+        if self.scheduler['critic'] is not None:
+            self.scheduler['critic'].step()
 
         # actor update
         if self.iterations % self.delay == 0:
             _, actions_eval = self.policy(obs, IDs)
             _, policy_q = self.policy.Qpolicy(obs, actions_eval, IDs)
             p_loss = -policy_q.mean()
             self.optimizer['actor'].zero_grad()
             p_loss.backward()
             self.optimizer['actor'].step()
-            if self.scheduler is not None:
+            if self.scheduler['actor'] is not None:
                 self.scheduler['actor'].step()
             self.policy.soft_update(self.tau)
 
         lr_a = self.optimizer['actor'].state_dict()['param_groups'][0]['lr']
-        lr_c_A = self.optimizer['critic_A'].state_dict()['param_groups'][0]['lr']
-        lr_c_B = self.optimizer['critic_B'].state_dict()['param_groups'][0]['lr']
+        lr_c = self.optimizer['critic'].state_dict()['param_groups'][0]['lr']
 
         info = {
             "learning_rate_actor": lr_a,
-            "learning_rate_critic_A": lr_c_A,
-            "learning_rate_critic_B": lr_c_B,
-            "loss_critic_A": loss_c.item(),
-            "loss_critic_B": loss_c.item()
+            "learning_rate_critic": lr_c,
+            "loss_critic": loss_c.item()
         }
         if self.iterations % self.delay == 0:
             info["loss_actor"] = p_loss.item()
 
         return info
```

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/mfac_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/mfac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/mfq_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/mfq_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/qmix_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/qmix_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/qtran_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/qtran_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/vdac_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/vdac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/vdn_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/vdn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/multi_agent_rl/wqmix_learner.py` & `xuance-1.1.0/xuance/torch/learners/multi_agent_rl/wqmix_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/policy_gradient/a2c_learner.py` & `xuance-1.1.0/xuance/torch/learners/policy_gradient/a2c_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/policy_gradient/ddpg_learner.py` & `xuance-1.1.0/xuance/torch/learners/policy_gradient/ddpg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/policy_gradient/mpdqn_learner.py` & `xuance-1.1.0/xuance/torch/learners/policy_gradient/mpdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/policy_gradient/pdqn_learner.py` & `xuance-1.1.0/xuance/torch/learners/policy_gradient/pdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/policy_gradient/pg_learner.py` & `xuance-1.1.0/xuance/torch/learners/policy_gradient/pg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/policy_gradient/ppg_learner.py` & `xuance-1.1.0/xuance/torch/learners/policy_gradient/ppg_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/policy_gradient/ppoclip_learner.py` & `xuance-1.1.0/xuance/torch/learners/policy_gradient/ppoclip_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/policy_gradient/ppokl_learner.py` & `xuance-1.1.0/xuance/torch/learners/policy_gradient/ppokl_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/policy_gradient/sac_learner.py` & `xuance-1.1.0/xuance/torch/learners/policy_gradient/sac_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/policy_gradient/sacdis_learner.py` & `xuance-1.1.0/xuance/torch/learners/policy_gradient/sacdis_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/policy_gradient/spdqn_learner.py` & `xuance-1.1.0/xuance/torch/learners/policy_gradient/spdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/policy_gradient/td3_learner.py` & `xuance-1.1.0/xuance/torch/learners/policy_gradient/td3_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/qlearning_family/c51_learner.py` & `xuance-1.1.0/xuance/torch/learners/qlearning_family/c51_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/qlearning_family/ddqn_learner.py` & `xuance-1.1.0/xuance/torch/learners/qlearning_family/ddqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/qlearning_family/dqn_learner.py` & `xuance-1.1.0/xuance/torch/learners/qlearning_family/dqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/qlearning_family/drqn_learner.py` & `xuance-1.1.0/xuance/torch/learners/qlearning_family/drqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/qlearning_family/dueldqn_learner.py` & `xuance-1.1.0/xuance/torch/learners/qlearning_family/dueldqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/qlearning_family/perdqn_learner.py` & `xuance-1.1.0/xuance/torch/learners/qlearning_family/perdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/learners/qlearning_family/qrdqn_learner.py` & `xuance-1.1.0/xuance/torch/learners/qlearning_family/qrdqn_learner.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/policies/__init__.py` & `xuance-1.1.0/xuance/torch/policies/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,98 +74,103 @@
     "Gaussian_MAAC_Policy": Gaussain_MAAC,
     "Gaussian_ISAC_Policy": Gaussian_ISAC,
     "Gaussian_MASAC_Policy": Gaussian_MASAC,
     "MATD3_Policy": MATD3_policy
 }
 
 Policy_Inputs = {
+    # DRL (discrete action spaces) #
     "Categorical_AC": ["action_space", "representation", "actor_hidden_size", "critic_hidden_size",
                        "normalize", "initialize", "activation", "device"],
     "Categorical_Actor": ["action_space", "representation", "actor_hidden_size",
                           "normalize", "initialize", "activation", "device"],
     "Discrete_SAC": ["action_space", "representation", "actor_hidden_size", "critic_hidden_size",
                      "normalize", "initialize", "activation", "device"],
     "Categorical_PPG": ["action_space", "representation", "actor_hidden_size", "critic_hidden_size",
                         "normalize", "initialize", "activation", "device"],
-    "Gaussian_AC": ["action_space", "representation", "actor_hidden_size", "critic_hidden_size",
-                    "normalize", "initialize", "activation", "device"],
-    "Gaussian_SAC": ["action_space", "representation", "actor_hidden_size", "critic_hidden_size",
-                     "normalize", "initialize", "activation", "device"],
-    "Gaussian_Actor": ["action_space", "representation", "actor_hidden_size",
-                       "normalize", "initialize", "activation", "device", "fixed_std"],
-    "Gaussian_PPG": ["action_space", "representation", "actor_hidden_size", "critic_hidden_size",
-                     "normalize", "initialize", "activation", "device"],
     "Basic_Q_network": ["action_space", "representation", "hidden_sizes",
                         "normalize", "initialize", "activation", "device"],
     "Duel_Q_network": ["action_space", "representation", "hidden_sizes",
                        "normalize", "initialize", "activation", "device"],
     "Noisy_Q_network": ["action_space", "representation", "hidden_sizes",
                         "normalize", "initialize", "activation", "device"],
     "C51_Q_network": ["action_space", "atom_num", "vmin", "vmax", "representation", "hidden_sizes",
                       "normalize", "initialize", "activation", "device"],
     "QR_Q_network": ["action_space", "quantile_num", "representation", "hidden_sizes",
                      "normalize", "initialize", "activation", "device"],
+    # DRL (continuous action spaces) #
+    "Gaussian_AC": ["action_space", "representation", "actor_hidden_size", "critic_hidden_size",
+                    "normalize", "initialize", "activation", "activation_action", "device"],
+    "Gaussian_SAC": ["action_space", "representation", "actor_hidden_size", "critic_hidden_size",
+                     "normalize", "initialize", "activation", "activation_action", "device"],
+    "Gaussian_Actor": ["action_space", "representation", "actor_hidden_size",
+                       "normalize", "initialize", "activation", "activation_action", "device", "fixed_std"],
+    "Gaussian_PPG": ["action_space", "representation", "actor_hidden_size", "critic_hidden_size",
+                     "normalize", "initialize", "activation", "activation_action", "device"],
     "DDPG_Policy": ["action_space", "representation", "actor_hidden_size", "critic_hidden_size",
-                    "initialize", "activation", "device"],
+                    "initialize", "activation", "activation_action", "device"],
     "SAC_Policy": ["action_space", "representation", "actor_hidden_size", "critic_hidden_size",
-                   "normalize", "initialize", "activation", "device"],
+                   "normalize", "initialize", "activation", "activation_action", "device"],
     "TD3_Policy": ["action_space", "representation", "actor_hidden_size", "critic_hidden_size",
-                   "normalize", "initialize", "activation", "device"],
+                   "normalize", "initialize", "activation", "activation_action", "device"],
+    # DRL (hybrid action spaces) #
     "PDQN_Policy": ['observation_space', 'action_space', 'representation', 'conactor_hidden_size',
-                    'qnetwork_hidden_size',
-                    'normalize', 'initialize', 'activation', 'device'],
+                    'qnetwork_hidden_size', 'normalize', 'initialize', 'activation', 'device'],
     "MPDQN_Policy": ['observation_space', 'action_space', 'representation', 'conactor_hidden_size',
-                     'qnetwork_hidden_size',
-                     'normalize', 'initialize', 'activation', 'device'],
+                     'qnetwork_hidden_size', 'normalize', 'initialize', 'activation', 'device'],
     "SPDQN_Policy": ['observation_space', 'action_space', 'representation', 'conactor_hidden_size',
-                     'qnetwork_hidden_size',
-                     'normalize', 'initialize', 'activation', 'device'],
-    #  MARL policies  #
+                     'qnetwork_hidden_size', 'normalize', 'initialize', 'activation', 'device'],
+    #  MARL policies (discrete action spaces) #
     "Basic_Q_network_marl": ["action_space", "n_agents", "representation", "hidden_sizes",
                              "normalize", "initialize", "activation", "device"],
     "Mixing_Q_network": ["action_space", "n_agents", "representation", "mixer", "hidden_sizes",
                          "normalize", "initialize", "activation", "device"],
     "Weighted_Mixing_Q_network": ["action_space", "n_agents", "representation", "mixer", "ff_mixer", "hidden_sizes",
                                   "normalize", "initialize", "activation", "device"],
     "Qtran_Mixing_Q_network": ["action_space", "n_agents", "representation", "mixer", "qtran_mixer", "hidden_sizes",
                                "normalize", "initialize", "activation", "device"],
     "Categorical_MAAC_Policy": ["action_space", "n_agents", "representation", "mixer", "actor_hidden_size",
                                 "critic_hidden_size", "normalize", "initialize", "activation", "device"],
     "Categorical_MAAC_Policy_Share": ["action_space", "n_agents", "representation", "mixer", "actor_hidden_size",
-                                "critic_hidden_size", "normalize", "initialize", "activation", "device"],
+                                      "critic_hidden_size", "normalize", "initialize", "activation", "device"],
     "Categorical_MFAC_Policy": ["action_space", "n_agents", "representation", "actor_hidden_size",
                                 "critic_hidden_size", "normalize", "initialize", "activation", "device"],
     "Categorical_COMA_Policy": ["action_space", "n_agents", "representation", "actor_hidden_size",
                                 "critic_hidden_size", "normalize", "initialize", "activation", "device"],
-    "Independent_DDPG_Policy": ["action_space", "n_agents", "representation", "actor_hidden_size",
-                                "critic_hidden_size", "normalize", "initialize", "activation", "device"],
-    "MADDPG_Policy": ["action_space", "n_agents", "representation", "actor_hidden_size", "critic_hidden_size",
-                      "normalize", "initialize", "activation", "device"],
     "MF_Q_network": ["action_space", "n_agents", "representation", "hidden_sizes",
                      "normalize", "initialize", "activation", "device"],
+    #  MARL policies (continuous action spaces) #
+    "Independent_DDPG_Policy": ["action_space", "n_agents", "representation", "actor_hidden_size",
+                                "critic_hidden_size", "normalize", "initialize", "activation", "activation_action",
+                                "device"],
+    "MADDPG_Policy": ["action_space", "n_agents", "representation", "actor_hidden_size", "critic_hidden_size",
+                      "normalize", "initialize", "activation", "activation_action", "device"],
     "Gaussian_MAAC_Policy": ["action_space", "n_agents", "representation", "mixer", "actor_hidden_size",
-                             "critic_hidden_size", "normalize", "initialize", "activation", "device"],
+                             "critic_hidden_size", "normalize", "initialize", "activation", "activation_action",
+                             "device"],
     "Gaussian_ISAC_Policy": ["action_space", "n_agents", "representation", "actor_hidden_size",
-                             "critic_hidden_size", "normalize", "initialize", "activation", "device"],
+                             "critic_hidden_size", "normalize", "initialize", "activation", "activation_action",
+                             "device"],
     "Gaussian_MASAC_Policy": ["action_space", "n_agents", "representation", "actor_hidden_size", "critic_hidden_size",
-                              "normalize", "initialize", "activation", "device"],
+                              "normalize", "initialize", "activation", "activation_action", "device"],
     "MATD3_Policy": ["action_space", "n_agents", "representation", "actor_hidden_size", "critic_hidden_size",
-                     "normalize", "initialize", "activation", "device"],
+                     "normalize", "initialize", "activation", "activation_action", "device"],
 }
 
 Policy_Inputs_All = {
     "state_dim": None,
     "action_space": None,
-    "n_agents": None,
+    "n_agents": 1,
     "representation": None,
     "mixer": None,
     "ff_mixer": None,
     "qtran_mixer": None,
     "hidden_sizes": None,
     "actor_hidden_size": None,
     "critic_hidden_size": None,
     "normalize": None,
     "initialize": None,
     "activation": None,
+    "activation_action": None,
     "device": None,
     "fixed_std": None
 }
```

### Comparing `xuance-1.0.9/xuance/torch/policies/categorical.py` & `xuance-1.1.0/xuance/torch/policies/categorical.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import torch.distributions
 from xuance.torch.policies import *
 from xuance.torch.utils import *
+import numpy as np
 
 
 def _init_layer(layer, gain=np.sqrt(2), bias=0.0):
     nn.init.orthogonal_(layer.weight, gain=gain)
     nn.init.constant_(layer.bias, bias)
     return layer
 
@@ -194,51 +195,56 @@
                  critic_hidden_size: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(SACDISPolicy, self).__init__()
         self.action_dim = action_space.n
-        self.representation = representation
-        self.representation_critic = copy.deepcopy(representation)
-        self.representation_info_shape = self.representation.output_shapes
+        self.representation_info_shape = representation.output_shapes
+
+        self.actor_representation = representation
+        self.critic_representation = copy.deepcopy(representation)
+        self.target_critic_representation = copy.deepcopy(representation)
+
         self.actor = ActorNet_SACDIS(representation.output_shapes['state'][0], self.action_dim, actor_hidden_size,
                                      normalize, initialize, activation, device)
         self.critic = CriticNet_SACDIS(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
                                        initialize, activation, device)
-        self.target_representation_critic = copy.deepcopy(self.representation_critic)
         self.target_critic = copy.deepcopy(self.critic)
 
+        self.actor_parameters = list(self.actor_representation.parameters()) + list(self.actor.parameters())
+        self.critic_parameters = list(self.critic_representation.parameters()) + list(self.critic.parameters())
+
     def forward(self, observation: Union[np.ndarray, dict]):
-        outputs = self.representation(observation)
+        outputs = self.actor_representation(observation)
         act_prob, act_distribution = self.actor(outputs['state'])
         return outputs, act_prob, act_distribution
 
     def Qtarget(self, observation: Union[np.ndarray, dict]):
-        outputs_actor = self.representation(observation)
-        outputs_critic = self.target_representation_critic(observation)
+        outputs_actor = self.actor_representation(observation)
+        outputs_critic = self.target_critic_representation(observation)
         act_prob, act_distribution = self.actor(outputs_actor['state'])
         # z = act_prob == 0.0
         # z = z.float() * 1e-8
         log_action_prob = torch.log(act_prob + 1e-5)
         return act_prob, log_action_prob, self.target_critic(outputs_critic['state'])
 
     def Qaction(self, observation: Union[np.ndarray, dict]):
-        outputs_critic = self.representation_critic(observation)
+        outputs_critic = self.critic_representation(observation)
         return outputs_critic, self.critic(outputs_critic['state'])
 
     def Qpolicy(self, observation: Union[np.ndarray, dict]):
-        outputs_actor = self.representation(observation)
-        outputs_critic = self.representation(observation)
+        outputs_actor = self.actor_representation(observation)
+        outputs_critic = self.critic_representation(observation)
         act_prob, act_distribution = self.actor(outputs_actor['state'])
         # z = act_prob == 0.0
         # z = z.float() * 1e-8
         log_action_prob = torch.log(act_prob + 1e-5)
         return act_prob, log_action_prob, self.critic(outputs_critic['state'])
 
     def soft_update(self, tau=0.005):
-        for ep, tp in zip(self.representation_critic.parameters(), self.target_representation_critic.parameters()):
+        for ep, tp in zip(self.critic_representation.parameters(), self.target_critic_representation.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
         for ep, tp in zip(self.critic.parameters(), self.target_critic.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
```

### Comparing `xuance-1.0.9/xuance/torch/policies/categorical_marl.py` & `xuance-1.1.0/xuance/torch/policies/categorical_marl.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,16 @@
         self.critic = CriticNet(self.representation_critic.output_shapes['state'][0], n_agents, critic_hidden_size,
                                 normalize, initialize, activation, device)
         self.mixer = mixer
         self.pi_dist = CategoricalDistribution(self.action_dim)
 
     def forward(self, observation: torch.Tensor, agent_ids: torch.Tensor,
                 *rnn_hidden: torch.Tensor, avail_actions=None):
+        if avail_actions is not None:
+            observation = torch.concat([observation, avail_actions], dim=-1)
         if self.use_rnn:
             outputs = self.representation(observation, *rnn_hidden)
             rnn_hidden = (outputs['rnn_hidden'], outputs['rnn_cell'])
         else:
             outputs = self.representation(observation)
             rnn_hidden = None
         actor_input = torch.concat([outputs['state'], agent_ids], dim=-1)
```

### Comparing `xuance-1.0.9/xuance/torch/policies/coordination_graph.py` & `xuance-1.1.0/xuance/torch/policies/coordination_graph.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/policies/deterministic.py` & `xuance-1.1.0/xuance/torch/policies/deterministic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from xuance.torch.policies import *
 from xuance.torch.utils import *
+import numpy as np
 
 
 class BasicQhead(nn.Module):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
                  hidden_sizes: Sequence[int],
@@ -363,22 +364,23 @@
 class ActorNet(nn.Module):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
                  hidden_sizes: Sequence[int],
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(ActorNet, self).__init__()
         layers = []
         input_shape = (state_dim,)
         for h in hidden_sizes:
             mlp, input_shape = mlp_block(input_shape[0], h, None, activation, initialize, device)
             layers.extend(mlp)
-        layers.extend(mlp_block(input_shape[0], action_dim, None, nn.Tanh, initialize, device)[0])
+        layers.extend(mlp_block(input_shape[0], action_dim, None, activation_action, initialize, device)[0])
         self.model = nn.Sequential(*layers)
 
     def forward(self, x: torch.tensor):
         return self.model(x)
 
 
 class CriticNet(nn.Module):
@@ -406,114 +408,158 @@
     def __init__(self,
                  action_space: Space,
                  representation: nn.Module,
                  actor_hidden_size: Sequence[int],
                  critic_hidden_size: Sequence[int],
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(DDPGPolicy, self).__init__()
         self.action_dim = action_space.shape[0]
         self.representation_info_shape = representation.output_shapes
-        self.representation = representation
+        self.actor_representation = representation
+        self.critic_representation = copy.deepcopy(representation)
+        self.target_actor_representation = copy.deepcopy(representation)
+        self.target_critic_representation = copy.deepcopy(representation)
         self.actor = ActorNet(representation.output_shapes['state'][0], self.action_dim, actor_hidden_size, initialize,
-                              activation, device)
+                              activation, activation_action, device)
         self.critic = CriticNet(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
                                 initialize, activation, device)
         self.target_actor = copy.deepcopy(self.actor)
         self.target_critic = copy.deepcopy(self.critic)
+        
+        # parameters
+        self.actor_parameters = list(self.actor_representation.parameters()) + list(self.actor.parameters())
+        self.critic_parameters = list(self.critic_representation.parameters()) + list(self.critic.parameters())
 
     def forward(self, observation: Union[np.ndarray, dict]):
-        outputs = self.representation(observation)
+        outputs = self.actor_representation(observation)
         act = self.actor(outputs['state'])
         return outputs, act
 
     def Qtarget(self, observation: Union[np.ndarray, dict]):
-        outputs = self.representation(observation)
-        act = self.target_actor(outputs['state'])
+        outputs_actor = self.target_actor_representation(observation)
+        outputs_critic = self.target_critic_representation(observation) 
+        act = self.target_actor(outputs_actor['state'])
         # noise = torch.randn_like(act).clamp(-1, 1) * 0.1
         # act = (act + noise).clamp(-1, 1)
-        return self.target_critic(outputs['state'], act)
+        return self.target_critic(outputs_critic['state'], act)
 
     def Qaction(self, observation: Union[np.ndarray, dict], action: torch.Tensor):
-        outputs = self.representation(observation)
+        outputs = self.critic_representation(observation)
         return self.critic(outputs['state'], action)
 
     def Qpolicy(self, observation: Union[np.ndarray, dict]):
-        outputs = self.representation(observation)
-        return self.critic(outputs['state'], self.actor(outputs['state']))
+        outputs_actor = self.actor_representation(observation)
+        outputs_critic = self.critic_representation(observation)
+        return self.critic(outputs_critic['state'], self.actor(outputs_actor['state']))
 
     def soft_update(self, tau=0.005):
+        for ep, tp in zip(self.actor_representation.parameters(), self.target_actor_representation.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
         for ep, tp in zip(self.actor.parameters(), self.target_actor.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
+        for ep, tp in zip(self.critic_representation.parameters(), self.target_critic_representation.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
         for ep, tp in zip(self.critic.parameters(), self.target_critic.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
 
 
 class TD3Policy(nn.Module):
     def __init__(self,
                  action_space: Space,
                  representation: nn.Module,
                  actor_hidden_size: Sequence[int],
                  critic_hidden_size: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(TD3Policy, self).__init__()
         self.action_dim = action_space.shape[0]
-        self.representation = representation
-        self.representation_info_shape = self.representation.output_shapes
+        self.representation_info_shape = representation.output_shapes
+
+        self.actor_representation = representation
+        self.criticA_representation = copy.deepcopy(representation)
+        self.criticB_representation = copy.deepcopy(representation)
+
+        self.target_actor_representation = copy.deepcopy(representation)
+        self.target_criticA_representation = copy.deepcopy(representation)
+        self.target_criticB_representation = copy.deepcopy(representation)
+
         self.actor = ActorNet(representation.output_shapes['state'][0], self.action_dim, actor_hidden_size,
-                              initialize, activation, device)
+                              initialize, activation, activation_action, device)
         self.criticA = CriticNet(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
                                  initialize, activation, device)
         self.criticB = CriticNet(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
                                  initialize, activation, device)
         self.target_actor = copy.deepcopy(self.actor)
         self.target_criticA = copy.deepcopy(self.criticA)
         self.target_criticB = copy.deepcopy(self.criticB)
 
+        # parameters
+        self.actor_parameters = list(self.actor_representation.parameters()) + list(self.actor.parameters())
+        self.critic_parameters = list(self.criticA_representation.parameters()) + list(self.criticA.parameters()) + list(self.criticB_representation.parameters()) + list(self.criticB.parameters())
+
     def action(self, observation: Union[np.ndarray, dict]):
-        outputs = self.representation(observation)
+        outputs = self.actor_representation(observation)
         act = self.actor(outputs['state'])
         return outputs, act
 
     def Qtarget(self, observation: Union[np.ndarray, dict]):
-        outputs = self.representation(observation)
-        act = self.target_actor(outputs['state'])
+        outputs_actor = self.target_actor_representation(observation)
+        outputs_criticA = self.target_criticA_representation(observation)
+        outputs_criticB = self.target_criticB_representation(observation)
+        act = self.target_actor(outputs_actor['state'])
         noise = torch.randn_like(act).clamp(-0.1, 0.1) * 0.1
         act = (act + noise).clamp(-1, 1)
-        qa = self.target_criticA(outputs['state'], act).unsqueeze(dim=1)
-        qb = self.target_criticB(outputs['state'], act).unsqueeze(dim=1)
+
+        qa = self.target_criticA(outputs_criticA['state'], act).unsqueeze(dim=1)
+        qb = self.target_criticB(outputs_criticB['state'], act).unsqueeze(dim=1)
         mim_q = torch.minimum(qa, qb)
-        return outputs, mim_q
+        return outputs_actor, mim_q
 
     def Qaction(self, observation: Union[np.ndarray, dict], action: torch.Tensor):
-        outputs = self.representation(observation)
-        qa = self.criticA(outputs['state'], action).unsqueeze(dim=1)
-        qb = self.criticB(outputs['state'], action).unsqueeze(dim=1)
-        return outputs, torch.cat((qa, qb), axis=-1)
+        outputs_criticA = self.criticA_representation(observation)
+        outputs_criticB = self.criticB_representation(observation)
+        qa = self.criticA(outputs_criticA['state'], action).unsqueeze(dim=1)
+        qb = self.criticB(outputs_criticB['state'], action).unsqueeze(dim=1)
+        return outputs_criticA, torch.cat((qa, qb), axis=-1)
 
     def Qpolicy(self, observation: Union[np.ndarray, dict]):
-        outputs = self.representation(observation)
-        act = self.actor(outputs['state'])
-        qa = self.criticA(outputs['state'], act).unsqueeze(dim=1)
-        qb = self.criticB(outputs['state'], act).unsqueeze(dim=1)
-        return outputs, (qa + qb) / 2.0
+        outputs_actor = self.actor_representation(observation)
+        outputs_criticA = self.criticA_representation(observation)
+        outputs_criticB = self.criticB_representation(observation)
+        act = self.actor(outputs_actor['state'])
+        qa = self.criticA(outputs_criticA['state'], act).unsqueeze(dim=1)
+        qb = self.criticB(outputs_criticB['state'], act).unsqueeze(dim=1)
+        return outputs_actor, (qa + qb) / 2.0
 
     def soft_update(self, tau=0.005):
+        for ep, tp in zip(self.actor_representation.parameters(), self.target_actor_representation.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
         for ep, tp in zip(self.actor.parameters(), self.target_actor.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
+        for ep, tp in zip(self.criticA_representation.parameters(), self.target_criticA_representation.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
         for ep, tp in zip(self.criticA.parameters(), self.target_criticA.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
+        for ep, tp in zip(self.criticB_representation.parameters(), self.target_criticB_representation.parameters()):
+            tp.data.mul_(1 - tau)
+            tp.data.add_(tau * ep.data)
         for ep, tp in zip(self.criticB.parameters(), self.target_criticB.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
 
 
 class PDQNPolicy(nn.Module):
     def __init__(self,
@@ -521,29 +567,29 @@
                  action_space,
                  representation: nn.Module,
                  conactor_hidden_size: Sequence[int],
                  qnetwork_hidden_size: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(PDQNPolicy, self).__init__()
         self.representation = representation
         self.target_representation = copy.deepcopy(representation)
         self.observation_space = observation_space
         self.action_space = action_space
         self.num_disact = self.action_space.spaces[0].n
         self.conact_sizes = np.array([self.action_space.spaces[i].shape[0] for i in range(1, self.num_disact + 1)])
         self.conact_size = int(self.conact_sizes.sum())
 
         self.qnetwork = BasicQhead(self.observation_space.shape[0] + self.conact_size, self.num_disact,
-                                   qnetwork_hidden_size, normalize,
-                                   initialize, torch.nn.modules.activation.ReLU, device)
+                                   qnetwork_hidden_size, normalize, initialize, activation, device)
         self.conactor = ActorNet(self.observation_space.shape[0], self.conact_size, conactor_hidden_size,
-                                 initialize, torch.nn.modules.activation.ReLU, device)
+                                 initialize, activation, activation_action, device)
         self.target_conactor = copy.deepcopy(self.conactor)
         self.target_qnetwork = copy.deepcopy(self.qnetwork)
 
     def Atarget(self, state):
         target_conact = self.target_conactor(state)
         return target_conact
 
@@ -585,30 +631,31 @@
                  action_space,
                  representation: nn.Module,
                  conactor_hidden_size: Sequence[int],
                  qnetwork_hidden_size: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(MPDQNPolicy, self).__init__()
         self.representation = representation
         self.target_representation = copy.deepcopy(representation)
         self.observation_space = observation_space
         self.obs_size = self.observation_space.shape[0]
         self.action_space = action_space
         self.num_disact = self.action_space.spaces[0].n
         self.conact_sizes = np.array([self.action_space.spaces[i].shape[0] for i in range(1, self.num_disact + 1)])
         self.conact_size = int(self.conact_sizes.sum())
 
         self.qnetwork = BasicQhead(self.observation_space.shape[0] + self.conact_size, self.num_disact,
                                    qnetwork_hidden_size, normalize,
-                                   initialize, torch.nn.modules.activation.ReLU, device)
+                                   initialize, activation, device)
         self.conactor = ActorNet(self.observation_space.shape[0], self.conact_size, conactor_hidden_size,
-                                 initialize, torch.nn.modules.activation.ReLU, device)
+                                 initialize, activation, activation_action, device)
         self.target_conactor = copy.deepcopy(self.conactor)
         self.target_qnetwork = copy.deepcopy(self.qnetwork)
 
         self.offsets = self.conact_sizes.cumsum()
         self.offsets = np.insert(self.offsets, 0, 0)
 
     def Atarget(self, state):
@@ -692,30 +739,31 @@
                  action_space,
                  representation: nn.Module,
                  conactor_hidden_size: Sequence[int],
                  qnetwork_hidden_size: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(SPDQNPolicy, self).__init__()
         self.representation = representation
         self.target_representation = copy.deepcopy(representation)
         self.observation_space = observation_space
         self.action_space = action_space
         self.num_disact = self.action_space.spaces[0].n
         self.conact_sizes = np.array([self.action_space.spaces[i].shape[0] for i in range(1, self.num_disact + 1)])
         self.conact_size = int(self.conact_sizes.sum())
         self.qnetwork = nn.ModuleList()
         for k in range(self.num_disact):
             self.qnetwork.append(
                 BasicQhead(self.observation_space.shape[0] + self.conact_sizes[k], 1, qnetwork_hidden_size, normalize,
-                           initialize, torch.nn.modules.activation.ReLU, device))
+                           initialize, activation, device))
         self.conactor = ActorNet(self.observation_space.shape[0], self.conact_size, conactor_hidden_size,
-                                 initialize, torch.nn.modules.activation.ReLU, device)
+                                 initialize, activation, activation_action, device)
         self.target_conactor = copy.deepcopy(self.conactor)
         self.target_qnetwork = copy.deepcopy(self.qnetwork)
 
         self.offsets = self.conact_sizes.cumsum()
         self.offsets = np.insert(self.offsets, 0, 0)
 
     def Atarget(self, state):
```

### Comparing `xuance-1.0.9/xuance/torch/policies/deterministic_marl.py` & `xuance-1.1.0/xuance/torch/policies/deterministic_marl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from xuance.torch.policies import *
 from xuance.torch.utils import *
+from torch.distributions import Categorical
 from gymnasium import spaces as spaces_pettingzoo
 
 
 class BasicQhead(nn.Module):
     def __init__(self,
                  state_dim: int,
-                 action_dim: int,
+                 n_actions: int,
                  n_agents: int,
                  hidden_sizes: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(BasicQhead, self).__init__()
         layers_ = []
         input_shape = (state_dim + n_agents,)
         for h in hidden_sizes:
             mlp, input_shape = mlp_block(input_shape[0], h, normalize, activation, initialize, device)
             layers_.extend(mlp)
-        layers_.extend(mlp_block(input_shape[0], action_dim, None, None, None, device)[0])
+        layers_.extend(mlp_block(input_shape[0], n_actions, None, None, None, device)[0])
         self.model = nn.Sequential(*layers_)
 
     def forward(self, x: torch.Tensor):
         return self.model(x)
 
 
 class BasicQnetwork(nn.Module):
@@ -34,21 +35,21 @@
                  hidden_size: Sequence[int] = None,
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None,
                  **kwargs):
         super(BasicQnetwork, self).__init__()
-        self.action_dim = action_space.n
+        self.n_actions = action_space.n
         self.representation = representation
         self.target_representation = copy.deepcopy(self.representation)
         self.representation_info_shape = self.representation.output_shapes
         self.lstm = True if kwargs["rnn"] == "LSTM" else False
         self.use_rnn = True if kwargs["use_recurrent"] else False
-        self.eval_Qhead = BasicQhead(self.representation.output_shapes['state'][0], self.action_dim, n_agents,
+        self.eval_Qhead = BasicQhead(self.representation.output_shapes['state'][0], self.n_actions, n_agents,
                                      hidden_size, normalize, initialize, activation, device)
         self.target_Qhead = copy.deepcopy(self.eval_Qhead)
 
     def forward(self, observation: torch.Tensor, agent_ids: torch.Tensor,
                 *rnn_hidden: torch.Tensor, avail_actions=None):
         if self.use_rnn:
             outputs = self.representation(observation, *rnn_hidden)
@@ -91,20 +92,20 @@
                  representation: nn.Module,
                  hidden_size: Sequence[int] = None,
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(MFQnetwork, self).__init__()
-        self.action_dim = action_space.n
+        self.n_actions = action_space.n
         self.representation = representation
         self.target_representation = copy.deepcopy(self.representation)
         self.representation_info_shape = self.representation.output_shapes
 
-        self.eval_Qhead = BasicQhead(self.representation.output_shapes['state'][0] + self.action_dim, self.action_dim,
+        self.eval_Qhead = BasicQhead(self.representation.output_shapes['state'][0] + self.n_actions, self.n_actions,
                                      n_agents, hidden_size, normalize, initialize, activation, device)
         self.target_Qhead = copy.deepcopy(self.eval_Qhead)
 
     def forward(self, observation: torch.Tensor, actions_mean: torch.Tensor, agent_ids: torch.Tensor):
         outputs = self.representation(observation)
         q_inputs = torch.concat([outputs['state'], actions_mean, agent_ids], dim=-1)
         evalQ = self.eval_Qhead(q_inputs)
@@ -136,21 +137,21 @@
                  hidden_size: Sequence[int] = None,
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None,
                  **kwargs):
         super(MixingQnetwork, self).__init__()
-        self.action_dim = action_space.n
+        self.n_actions = action_space.n
         self.representation = representation
         self.target_representation = copy.deepcopy(self.representation)
         self.representation_info_shape = self.representation.output_shapes
         self.lstm = True if kwargs["rnn"] == "LSTM" else False
         self.use_rnn = True if kwargs["use_recurrent"] else False
-        self.eval_Qhead = BasicQhead(self.representation.output_shapes['state'][0], self.action_dim, n_agents,
+        self.eval_Qhead = BasicQhead(self.representation.output_shapes['state'][0], self.n_actions, n_agents,
                                      hidden_size, normalize, initialize, activation, device)
         self.target_Qhead = copy.deepcopy(self.eval_Qhead)
         self.eval_Qtot = mixer
         self.target_Qtot = copy.deepcopy(self.eval_Qtot)
 
     def forward(self, observation: torch.Tensor, agent_ids: torch.Tensor,
                 *rnn_hidden: torch.Tensor, avail_actions=None):
@@ -256,21 +257,21 @@
                  hidden_size: Sequence[int] = None,
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None,
                  **kwargs):
         super(Qtran_MixingQnetwork, self).__init__()
-        self.action_dim = action_space.n
+        self.n_actions = action_space.n
         self.representation = representation
         self.target_representation = copy.deepcopy(self.representation)
         self.representation_info_shape = self.representation.output_shapes
         self.lstm = True if kwargs["rnn"] == "LSTM" else False
         self.use_rnn = True if kwargs["use_recurrent"] else False
-        self.eval_Qhead = BasicQhead(self.representation.output_shapes['state'][0], self.action_dim, n_agents,
+        self.eval_Qhead = BasicQhead(self.representation.output_shapes['state'][0], self.n_actions, n_agents,
                                      hidden_size, normalize, initialize, activation, device)
         self.target_Qhead = copy.deepcopy(self.eval_Qhead)
         self.qtran_net = qtran_mixer
         self.target_qtran_net = copy.deepcopy(qtran_mixer)
         self.q_tot = mixer
 
     def forward(self, observation: torch.Tensor, agent_ids: torch.Tensor,
@@ -322,15 +323,15 @@
                  hidden_size_bias: Sequence[int] = None,
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None,
                  **kwargs):
         super(DCG_policy, self).__init__()
-        self.action_dim = action_space.n
+        self.n_actions = action_space.n
         self.representation = representation
         self.target_representation = copy.deepcopy(self.representation)
         self.lstm = True if kwargs["rnn"] == "LSTM" else False
         self.use_rnn = True if kwargs["use_recurrent"] else False
         self.utility = utility
         self.target_utility = copy.deepcopy(self.utility)
         self.payoffs = payoffs
@@ -374,28 +375,28 @@
                 tp.data.copy_(ep)
 
 
 class ActorNet(nn.Module):
     def __init__(self,
                  state_dim: int,
                  n_agents: int,
-                 action_space: spaces_pettingzoo,
+                 action_dim: int,
                  hidden_sizes: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(ActorNet, self).__init__()
         layers = []
         input_shape = (state_dim + n_agents,)
-        action_dim = action_space.shape[0]
         for h in hidden_sizes:
             mlp, input_shape = mlp_block(input_shape[0], h, normalize, activation, initialize, device)
             layers.extend(mlp)
-        layers.extend(mlp_block(input_shape[0], action_dim, None, nn.Sigmoid, initialize, device)[0])
+        layers.extend(mlp_block(input_shape[0], action_dim, None, activation_action, initialize, device)[0])
         self.model = nn.Sequential(*layers)
 
     def forward(self, x: torch.tensor):
         return self.model(x)
 
 
 class CriticNet(nn.Module):
@@ -424,32 +425,33 @@
 
     def forward(self, x: torch.tensor):
         return self.model(x)
 
 
 class Basic_DDPG_policy(nn.Module):
     def __init__(self,
-                 action_space: spaces_pettingzoo,
+                 action_space: Space,
                  n_agents: int,
                  representation: nn.Module,
                  actor_hidden_size: Sequence[int],
                  critic_hidden_size: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
-                 device: Optional[Union[str, int, torch.device]] = None
+                 activation_action: Optional[ModuleType] = None,
+                 device: Optional[Union[str, int, torch.device]] = None,
                  ):
         super(Basic_DDPG_policy, self).__init__()
-        self.action_dim = action_space.shape[0]
+        self.action_dim = action_space.shape[-1]
         self.n_agents = n_agents
         self.representation = representation
         self.representation_info_shape = self.representation.output_shapes
 
-        self.actor_net = ActorNet(representation.output_shapes['state'][0], n_agents, action_space,
-                                  actor_hidden_size, normalize, initialize, activation, device)
+        self.actor_net = ActorNet(representation.output_shapes['state'][0], n_agents, self.action_dim,
+                                  actor_hidden_size, normalize, initialize, activation, activation_action, device)
         self.critic_net = CriticNet(True, representation.output_shapes['state'][0], n_agents, self.action_dim,
                                     critic_hidden_size, normalize, initialize, activation, device)
         self.target_actor_net = copy.deepcopy(self.actor_net)
         self.target_critic_net = copy.deepcopy(self.critic_net)
         self.parameters_actor = list(self.representation.parameters()) + list(self.actor_net.parameters())
         self.parameters_critic = self.critic_net.parameters()
 
@@ -481,27 +483,28 @@
         for ep, tp in zip(self.critic_net.parameters(), self.target_critic_net.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
 
 
 class MADDPG_policy(Basic_DDPG_policy):
     def __init__(self,
-                 action_space: spaces_pettingzoo,
+                 action_space: Space,
                  n_agents: int,
                  representation: nn.Module,
                  actor_hidden_size: Sequence[int],
                  critic_hidden_size: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None
                  ):
         super(MADDPG_policy, self).__init__(action_space, n_agents, representation,
                                             actor_hidden_size, critic_hidden_size,
-                                            normalize, initialize, activation, device)
+                                            normalize, initialize, activation, activation_action, device)
         self.critic_net = CriticNet(False, representation.output_shapes['state'][0], n_agents, self.action_dim,
                                     critic_hidden_size, normalize, initialize, activation, device)
         self.target_critic_net = copy.deepcopy(self.critic_net)
         self.parameters_critic = self.critic_net.parameters()
 
     def critic(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
         bs = observation.shape[0]
@@ -514,36 +517,46 @@
         bs = observation.shape[0]
         outputs_n = self.representation(observation)['state'].view(bs, 1, -1).expand(-1, self.n_agents, -1)
         actions_n = actions.view(bs, 1, -1).expand(-1, self.n_agents, -1)
         critic_in = torch.concat([outputs_n, actions_n, agent_ids], dim=-1)
         return self.target_critic_net(critic_in)
 
 
-class MATD3_policy(Basic_DDPG_policy):
+class MATD3_policy(Basic_DDPG_policy, nn.Module):
     def __init__(self,
                  action_space: Space,
                  n_agents: int,
                  representation: nn.Module,
                  actor_hidden_size: Sequence[int],
                  critic_hidden_size: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None
                  ):
-        super(MATD3_policy, self).__init__(action_space, n_agents, representation,
-                                           actor_hidden_size, critic_hidden_size,
-                                           normalize, initialize, activation, device)
+        nn.Module.__init__(self)
+        self.action_dim = action_space.shape[-1]
+        self.n_agents = n_agents
+        self.representation = representation
+        self.representation_info_shape = self.representation.output_shapes
+
+        self.actor_net = ActorNet(representation.output_shapes['state'][0], n_agents, self.action_dim,
+                                  actor_hidden_size, normalize, initialize, activation, activation_action, device)
+        self.target_actor_net = copy.deepcopy(self.actor_net)
+
         self.critic_net_A = CriticNet(False, representation.output_shapes['state'][0], n_agents, self.action_dim,
                                       critic_hidden_size, normalize, initialize, activation, device)
         self.critic_net_B = CriticNet(False, representation.output_shapes['state'][0], n_agents, self.action_dim,
                                       critic_hidden_size, normalize, initialize, activation, device)
         self.target_critic_net_A = copy.deepcopy(self.critic_net_A)
         self.target_critic_net_B = copy.deepcopy(self.critic_net_B)
-        # self.parameters_critic = self.critic_net.parameters()
+
+        self.parameters_actor = list(self.representation.parameters()) + list(self.actor_net.parameters())
+        self.parameters_critic = list(self.critic_net_A.parameters()) + list(self.critic_net_B.parameters())
 
     def Qpolicy(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
         bs = observation.shape[0]
         outputs_n = self.representation(observation)['state'].view(bs, 1, -1).expand(-1, self.n_agents, -1)
         actions_n = actions.view(bs, 1, -1).expand(-1, self.n_agents, -1)
         critic_in = torch.concat([outputs_n, actions_n, agent_ids], dim=-1)
         qa = self.critic_net_A(critic_in)
```

### Comparing `xuance-1.0.9/xuance/torch/policies/gaussian.py` & `xuance-1.1.0/xuance/torch/policies/gaussian.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from xuance.torch.policies import *
 from xuance.torch.utils import *
+from torch.distributions import Normal
+import numpy as np
 
 
 class ActorNet(nn.Module):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
                  hidden_sizes: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(ActorNet, self).__init__()
         layers = []
         input_shape = (state_dim,)
         for h in hidden_sizes:
             mlp, input_shape = mlp_block(input_shape[0], h, normalize, activation, initialize, device)
             layers.extend(mlp)
-        layers.extend(mlp_block(input_shape[0], action_dim, None, None, initialize, device)[0])
+        layers.extend(mlp_block(input_shape[0], action_dim, None, activation_action, initialize, device)[0])
         self.mu = nn.Sequential(*layers)
         self.logstd = nn.Parameter(-torch.ones((action_dim,), device=device))
         self.dist = DiagGaussianDistribution(action_dim)
 
     def forward(self, x: torch.Tensor):
         self.dist.set_param(self.mu(x), self.logstd.exp())
         return self.dist
@@ -53,21 +56,22 @@
                  action_space: Space,
                  representation: nn.Module,
                  actor_hidden_size: Sequence[int] = None,
                  critic_hidden_size: Sequence[int] = None,
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(ActorCriticPolicy, self).__init__()
         self.action_dim = action_space.shape[0]
         self.representation = representation
         self.representation_info_shape = representation.output_shapes
         self.actor = ActorNet(representation.output_shapes['state'][0], self.action_dim, actor_hidden_size,
-                              normalize, initialize, activation, device)
+                              normalize, initialize, activation, activation_action, device)
         self.critic = CriticNet(representation.output_shapes['state'][0], critic_hidden_size,
                                 normalize, initialize, activation, device)
 
     def forward(self, observation: Union[np.ndarray, dict]):
         outputs = self.representation(observation)
         a = self.actor(outputs['state'])
         v = self.critic(outputs['state'])
@@ -78,22 +82,23 @@
     def __init__(self,
                  action_space: Space,
                  representation: nn.Module,
                  actor_hidden_size: Sequence[int] = None,
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None,
                  fixed_std: bool = True):
         super(ActorPolicy, self).__init__()
         self.action_dim = action_space.shape[0]
         self.representation = representation
         self.representation_info_shape = self.representation.output_shapes
         self.actor = ActorNet(representation.output_shapes['state'][0], self.action_dim, actor_hidden_size,
-                              normalize, initialize, activation, device)
+                              normalize, initialize, activation, activation_action, device)
 
     def forward(self, observation: Union[np.ndarray, dict]):
         outputs = self.representation(observation)
         a = self.actor(outputs['state'])
         return outputs, a
 
 
@@ -102,22 +107,23 @@
                  action_space: Space,
                  representation: nn.Module,
                  actor_hidden_size: Sequence[int] = None,
                  critic_hidden_size: Sequence[int] = None,
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(PPGActorCritic, self).__init__()
         self.action_dim = action_space.shape[0]
         self.actor_representation = representation
         self.critic_representation = copy.deepcopy(representation)
         self.representation_info_shape = self.actor_representation.output_shapes
         self.actor = ActorNet(representation.output_shapes['state'][0], self.action_dim, actor_hidden_size,
-                              normalize, initialize, activation, device)
+                              normalize, initialize, activation, activation_action, device)
         self.critic = CriticNet(representation.output_shapes['state'][0], critic_hidden_size,
                                 normalize, initialize, activation, device)
         self.aux_critic = CriticNet(representation.output_shapes['state'][0], critic_hidden_size,
                                     normalize, initialize, activation, device)
 
     def forward(self, observation: Union[np.ndarray, dict]):
         policy_outputs = self.actor_representation(observation)
@@ -132,35 +138,34 @@
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
                  hidden_sizes: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(ActorNet_SAC, self).__init__()
         layers = []
         input_shape = (state_dim,)
         for h in hidden_sizes:
             mlp, input_shape = mlp_block(input_shape[0], h, normalize, activation, initialize, device)
             layers.extend(mlp)
         self.device = device
         self.output = nn.Sequential(*layers)
-        self.out_mu = nn.Sequential(nn.Linear(hidden_sizes[-1], action_dim, device=device), nn.Tanh())
+        self.out_mu = nn.Sequential(*mlp_block(hidden_sizes[-1], action_dim, normalize, activation_action, initialize, device)[0])
         self.out_std = nn.Linear(hidden_sizes[-1], action_dim, device=device)
 
     def forward(self, x: torch.tensor):
         output = self.output(x)
         mu = self.out_mu(output)
-        # std = torch.tanh(self.out_std(output))
         std = torch.clamp(self.out_std(output), -20, 2)
         std = std.exp()
-        # dia_std = torch.diag_embed(std)
-        self.dist = torch.distributions.Normal(mu, std)
-        return self.dist
+        dist = Normal(mu, std)
+        return dist
 
 
 class CriticNet_SAC(nn.Module):
     def __init__(self,
                  state_dim: int,
                  action_dim: int,
                  hidden_sizes: Sequence[int],
@@ -186,61 +191,59 @@
                  action_space: Space,
                  representation: nn.Module,
                  actor_hidden_size: Sequence[int],
                  critic_hidden_size: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(SACPolicy, self).__init__()
         self.action_dim = action_space.shape[0]
         self.representation_info_shape = representation.output_shapes
-        self.representation_actor = representation
-        self.representation_critic = copy.deepcopy(representation)
+        
+        # representations
+        self.actor_representation = representation
+        self.critic_representation = copy.deepcopy(representation)
+        self.target_critic_representation = copy.deepcopy(representation)
+
         self.actor = ActorNet_SAC(representation.output_shapes['state'][0], self.action_dim, actor_hidden_size,
-                                  normalize, initialize, activation, device)
+                                  normalize, initialize, activation, activation_action, device)
         self.critic = CriticNet_SAC(representation.output_shapes['state'][0], self.action_dim, critic_hidden_size,
                                     normalize, initialize, activation, device)
-
-        self.target_representation_actor = copy.deepcopy(self.representation_actor)
-        self.target_actor = copy.deepcopy(self.actor)
-        self.target_representation_critic = copy.deepcopy(self.representation_critic)
         self.target_critic = copy.deepcopy(self.critic)
 
+        self.actor_parameters = list(self.actor_representation.parameters()) + list(self.actor.parameters())
+        self.critic_parameters = list(self.critic_representation.parameters()) + list(self.critic.parameters())
+
     def forward(self, observation: Union[np.ndarray, dict]):
-        outputs_actor = self.representation_actor(observation)
+        outputs_actor = self.actor_representation(observation)
         act_dist = self.actor(outputs_actor['state'])
         return outputs_actor, act_dist
 
     def Qtarget(self, observation: Union[np.ndarray, dict]):
-        outputs_actor = self.target_representation_actor(observation)
-        outputs_critic = self.target_representation_critic(observation)
-        act_dist = self.target_actor(outputs_actor['state'])
+        outputs_actor = self.actor_representation(observation)
+        outputs_critic = self.target_critic_representation(observation)
+        act_dist = self.actor(outputs_actor['state'])
         act = act_dist.rsample()
         act_log = act_dist.log_prob(act).sum(-1)
         return act_log, self.target_critic(outputs_critic['state'], act)
 
     def Qaction(self, observation: Union[np.ndarray, dict], action: torch.Tensor):
-        outputs_critic = self.representation_critic(observation)
+        outputs_critic = self.critic_representation(observation)
         return self.critic(outputs_critic['state'], action)
 
     def Qpolicy(self, observation: Union[np.ndarray, dict]):
-        outputs_actor = self.representation_actor(observation)
-        outputs_critic = self.representation_critic(observation)
+        outputs_actor = self.actor_representation(observation)
+        outputs_critic = self.critic_representation(observation)
         act_dist = self.actor(outputs_actor['state'])
         act = act_dist.rsample()
         act_log = act_dist.log_prob(act).sum(-1)
         return act_log, self.critic(outputs_critic['state'], act)
 
     def soft_update(self, tau=0.005):
-        for ep, tp in zip(self.representation_actor.parameters(), self.target_representation_actor.parameters()):
-            tp.data.mul_(1 - tau)
-            tp.data.add_(tau * ep.data)
-        for ep, tp in zip(self.representation_critic.parameters(), self.target_representation_critic.parameters()):
-            tp.data.mul_(1 - tau)
-            tp.data.add_(tau * ep.data)
-        for ep, tp in zip(self.actor.parameters(), self.target_actor.parameters()):
+        for ep, tp in zip(self.critic_representation.parameters(), self.target_critic_representation.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
         for ep, tp in zip(self.critic.parameters(), self.target_critic.parameters()):
             tp.data.mul_(1 - tau)
             tp.data.add_(tau * ep.data)
```

### Comparing `xuance-1.0.9/xuance/torch/policies/gaussian_marl.py` & `xuance-1.1.0/xuance/torch/policies/gaussian_marl.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,24 +68,24 @@
                  state_dim: int,
                  n_agents: int,
                  action_dim: int,
                  hidden_sizes: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None):
         super(ActorNet, self).__init__()
         self.device = device
         layers = []
         input_shape = (state_dim + n_agents,)
         for h in hidden_sizes:
             mlp, input_shape = mlp_block(input_shape[0], h, normalize, activation, initialize, device)
             layers.extend(mlp)
-        layers.append(nn.Linear(hidden_sizes[0], action_dim, device=device))
-        # layers.append(nn.Sigmoid())
+        layers.extend(mlp_block(input_shape[0], action_dim, activation=activation_action, device=device)[0])
         self.mu = nn.Sequential(*layers)
         self.log_std = nn.Parameter(-torch.ones((action_dim,), device=device))
         self.dist = DiagGaussianDistribution(action_dim)
 
     def forward(self, x: torch.Tensor):
         self.dist.set_param(self.mu(x), self.log_std.exp())
         return self.dist
@@ -125,27 +125,28 @@
                  representation: nn.Module,
                  mixer: Optional[VDN_mixer] = None,
                  actor_hidden_size: Sequence[int] = None,
                  critic_hidden_size: Sequence[int] = None,
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None,
                  **kwargs):
         super(MAAC_Policy, self).__init__()
         self.device = device
         self.action_dim = action_space.shape[0]
         self.n_agents = n_agents
         self.representation = representation[0]
         self.representation_critic = representation[1]
         self.representation_info_shape = self.representation.output_shapes
         self.lstm = True if kwargs["rnn"] == "LSTM" else False
         self.use_rnn = True if kwargs["use_recurrent"] else False
         self.actor = ActorNet(self.representation.output_shapes['state'][0], n_agents, self.action_dim,
-                              actor_hidden_size, normalize, initialize, activation, device)
+                              actor_hidden_size, normalize, initialize, activation, activation_action, device)
         dim_input_critic = self.representation_critic.output_shapes['state'][0]
         self.critic = CriticNet(dim_input_critic, n_agents, critic_hidden_size,
                                 normalize, initialize, activation, device)
         self.mixer = mixer
         self.pi_dist = None
 
     def forward(self, observation: torch.Tensor, agent_ids: torch.Tensor,
@@ -191,24 +192,25 @@
                  n_agents: int,
                  representation: nn.Module,
                  actor_hidden_size: Sequence[int],
                  critic_hidden_size: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None
                  ):
         super(Basic_ISAC_policy, self).__init__()
         self.action_dim = action_space.shape[0]
         self.n_agents = n_agents
         self.representation = representation
         self.representation_info_shape = self.representation.output_shapes
 
         self.actor_net = ActorNet(representation.output_shapes['state'][0], n_agents, self.action_dim,
-                                  actor_hidden_size, normalize, initialize, activation, device)
+                                  actor_hidden_size, normalize, initialize, activation, activation_action, device)
         dim_input_critic = representation.output_shapes['state'][0] + self.action_dim
         self.critic_net = CriticNet(dim_input_critic, n_agents, critic_hidden_size,
                                     normalize, initialize, activation, device)
         self.target_actor_net = copy.deepcopy(self.actor_net)
         self.target_critic_net = copy.deepcopy(self.critic_net)
         self.parameters_actor = list(self.representation.parameters()) + list(self.actor_net.parameters())
         self.parameters_critic = self.critic_net.parameters()
@@ -249,19 +251,20 @@
                  n_agents: int,
                  representation: nn.Module,
                  actor_hidden_size: Sequence[int],
                  critic_hidden_size: Sequence[int],
                  normalize: Optional[ModuleType] = None,
                  initialize: Optional[Callable[..., torch.Tensor]] = None,
                  activation: Optional[ModuleType] = None,
+                 activation_action: Optional[ModuleType] = None,
                  device: Optional[Union[str, int, torch.device]] = None
                  ):
         super(MASAC_policy, self).__init__(action_space, n_agents, representation,
                                            actor_hidden_size, critic_hidden_size,
-                                           normalize, initialize, activation, device)
+                                           normalize, initialize, activation, activation_action, device)
         dim_input_critic = (representation.output_shapes['state'][0] + self.action_dim) * self.n_agents
         self.critic_net = CriticNet(dim_input_critic, n_agents, critic_hidden_size,
                                     normalize, initialize, activation, device)
         self.target_critic_net = copy.deepcopy(self.critic_net)
         self.parameters_critic = self.critic_net.parameters()
 
     def critic(self, observation: torch.Tensor, actions: torch.Tensor, agent_ids: torch.Tensor):
```

### Comparing `xuance-1.0.9/xuance/torch/policies/mixers.py` & `xuance-1.1.0/xuance/torch/policies/mixers.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/representations/__init__.py` & `xuance-1.1.0/xuance/torch/representations/__init__.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/representations/cnn.py` & `xuance-1.1.0/xuance/torch/representations/cnn.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/representations/mlp.py` & `xuance-1.1.0/xuance/torch/representations/mlp.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/representations/rnn.py` & `xuance-1.1.0/xuance/torch/representations/rnn.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/runners/runner_drl.py` & `xuance-1.1.0/xuance/torch/runners/runner_drl.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,21 +37,16 @@
         input_policy = get_policy_in(self.args, representation)
         if self.agent_name == "DRQN":
             policy = REGISTRY_Policy[self.args.policy](**input_policy)
         else:
             policy = REGISTRY_Policy[self.args.policy](*input_policy)
 
         if self.agent_name in ["DDPG", "TD3", "SAC", "SACDIS"]:
-            actor_optimizer = torch.optim.Adam(policy.actor.parameters(), self.args.actor_learning_rate)
-            if self.agent_name == "TD3":
-                critic_optimizer = torch.optim.Adam(
-                    itertools.chain(policy.criticA.parameters(), policy.criticB.parameters()),
-                    self.args.critic_learning_rate)
-            else:
-                critic_optimizer = torch.optim.Adam(policy.critic.parameters(), self.args.critic_learning_rate)
+            actor_optimizer = torch.optim.Adam(policy.actor_parameters, self.args.actor_learning_rate)
+            critic_optimizer = torch.optim.Adam(policy.critic_parameters, self.args.critic_learning_rate)
             actor_lr_scheduler = torch.optim.lr_scheduler.LinearLR(actor_optimizer, start_factor=1.0, end_factor=0.25,
                                                                    total_iters=get_total_iters(self.agent_name,
                                                                                                self.args))
             critic_lr_scheduler = torch.optim.lr_scheduler.LinearLR(critic_optimizer, start_factor=1.0, end_factor=0.25,
                                                                     total_iters=get_total_iters(self.agent_name,
                                                                                                 self.args))
             self.agent = REGISTRY_Agent[self.agent_name](self.args, self.envs, policy,
@@ -75,17 +70,18 @@
                                                          self.args.device)
 
     def run(self):
         if self.args.test_mode:
             def env_fn():
                 args_test = deepcopy(self.args)
                 args_test.parallels = 1
+                args_test.render = True
                 return make_envs(args_test)
             self.agent.render = True
-            self.agent.load_model(self.agent.model_dir_load, self.args.seed)
+            self.agent.load_model(self.agent.model_dir_load)
             scores = self.agent.test(env_fn, self.args.test_episode)
             print(f"Mean Score: {np.mean(scores)}, Std: {np.std(scores)}")
             print("Finish testing.")
         else:
             n_train_steps = self.args.running_steps // self.n_envs
             self.agent.train(n_train_steps)
             print("Finish training.")
```

### Comparing `xuance-1.0.9/xuance/torch/runners/runner_football.py` & `xuance-1.1.0/xuance/torch/runners/runner_football.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/runners/runner_pettingzoo.py` & `xuance-1.1.0/xuance/torch/runners/runner_pettingzoo.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,31 @@
 import socket
 import time
 from pathlib import Path
 import wandb
 from torch.utils.tensorboard import SummaryWriter
 from .runner_basic import Runner_Base, make_envs
 from xuance.torch.agents import REGISTRY as REGISTRY_Agent
+from xuance.common import get_time_string
 from gymnasium.spaces.box import Box
 from tqdm import tqdm
 import numpy as np
 from copy import deepcopy
 
 
 class Pettingzoo_Runner(Runner_Base):
     def __init__(self, args):
         self.args = args if type(args) == list else [args]
-        self.fps = 20
+        self.fps = args[0].fps if type(args) == list else args.fps
 
-        time_string = time.asctime().replace(" ", "").replace(":", "_")
+        time_string = get_time_string()
         for arg in self.args:
             seed = f"seed_{arg.seed}_"
             arg.model_dir_load = arg.model_dir
             arg.model_dir_save = os.path.join(os.getcwd(), arg.model_dir, seed + time_string)
-            if (not os.path.exists(arg.model_dir_save)) and (not arg.test_mode):
-                os.makedirs(arg.model_dir_save)
 
             if arg.logger == "tensorboard":
                 log_dir = os.path.join(os.getcwd(), arg.log_dir, seed + time_string)
                 if not os.path.exists(log_dir):
                     os.makedirs(log_dir)
                 self.writer = SummaryWriter(log_dir)
                 self.use_wandb = False
@@ -65,25 +64,28 @@
                     wandb.init(config=config_dict,
                                project=arg.project_name,
                                entity=arg.wandb_user_name,
                                notes=socket.gethostname(),
                                dir=wandb_dir,
                                group=arg.env_id,
                                job_type=arg.agent,
-                               name=time.asctime(),
+                               name=time_string,
                                reinit=True)
                 break
 
         self.episode_length = self.envs.max_episode_length
 
         # environment details, representations, policies, optimizers, and agents.
         for h, arg in enumerate(self.args):
             arg.handle_name = self.envs.side_names[h]
             if self.n_handles > 1 and arg.agent != "RANDOM":
                 arg.model_dir += "{}/".format(arg.handle_name)
+            if len(self.args) != self.n_handles:
+                n_methods = len(self.args)
+                raise AttributeError(f"{self.n_handles} methods should be specified in this environment, while get {n_methods}!")
             arg.handle, arg.n_agents = h, self.envs.n_agents[h]
             arg.agent_keys, arg.agent_ids = self.agent_keys[h], self.agent_ids[h]
             arg.state_space = self.envs.state_space
             arg.observation_space = self.envs.observation_space
             if isinstance(self.envs.action_space[self.agent_keys[h][0]], Box):
                 arg.dim_act = self.envs.action_space[self.agent_keys[h][0]].shape[0]
                 arg.act_shape = (arg.dim_act,)
@@ -96,16 +98,14 @@
                 arg.dim_obs = arg.obs_shape[0]
             else:
                 arg.obs_shape = self.envs.observation_space[self.agent_keys[h][0]].shape
                 arg.dim_obs = arg.obs_shape[0]
             arg.rew_shape, arg.done_shape, arg.act_prob_shape = (arg.n_agents, 1), (arg.n_agents,), (arg.dim_act,)
             self.marl_agents.append(REGISTRY_Agent[arg.agent](arg, self.envs, arg.device))
             self.marl_names.append(arg.agent)
-            if arg.test_mode:
-                self.marl_agents[h].load_model(arg.model_dir, arg.seed)
 
         self.print_infos(self.args)
 
     def log_infos(self, info: dict, x_index: int):
         """
         info: (dict) information to be visualized
         n_steps: current step
@@ -135,14 +135,21 @@
             if arg.n_agents == 1:
                 infos.append(agent_name + ": {} agent".format(arg.n_agents) + ", {}".format(arg.agent))
             else:
                 infos.append(agent_name + ": {} agents".format(arg.n_agents) + ", {}".format(arg.agent))
         print(infos)
         time.sleep(0.01)
 
+    def finish(self):
+        self.envs.close()
+        if self.use_wandb:
+            wandb.finish()
+        else:
+            self.writer.close()
+
     def combine_env_actions(self, actions):
         actions_envs = []
         num_env = actions[0].shape[0]
         for e in range(num_env):
             act_handle = {}
             for h, keys in enumerate(self.agent_keys):
                 act_handle.update({agent_name: actions[h][e][i] for i, agent_name in enumerate(keys)})
@@ -218,16 +225,16 @@
                 data_step['act_mean'] = actions_dict['act_mean'][h]
             else:
                 pass
             mas_group.memory.store(data_step)
 
     def train_episode(self, n_episodes):
         act_mean_last = [np.zeros([self.n_envs, arg.dim_act]) for arg in self.args]
-        terminal_handle = np.zeros([self.n_handles, self.n_envs], dtype=np.bool)
-        truncate_handle = np.zeros([self.n_handles, self.n_envs], dtype=np.bool)
+        terminal_handle = np.zeros([self.n_handles, self.n_envs], dtype=np.bool_)
+        truncate_handle = np.zeros([self.n_handles, self.n_envs], dtype=np.bool_)
         episode_score = np.zeros([self.n_handles, self.n_envs, 1], dtype=np.float32)
         episode_info, train_info = {}, {}
         for _ in tqdm(range(n_episodes)):
             obs_n = self.envs.buf_obs
             state, agent_mask = self.envs.global_state(), self.envs.agent_mask()
             for step in range(self.episode_length):
                 actions_dict = self.get_actions(obs_n, False, act_mean_last, agent_mask, state)
@@ -302,16 +309,16 @@
         obs_n, infos = test_envs.reset()
         state, agent_mask = test_envs.global_state(), test_envs.agent_mask()
         if self.args_base.render_mode == "rgb_array" and self.render:
             images = test_envs.render(self.args_base.render_mode)
             for idx, img in enumerate(images):
                 videos[idx].append(img)
         act_mean_last = [np.zeros([num_envs, arg.dim_act]) for arg in self.args]
-        terminal_handle = np.zeros([self.n_handles, num_envs], dtype=np.bool)
-        truncate_handle = np.zeros([self.n_handles, num_envs], dtype=np.bool)
+        terminal_handle = np.zeros([self.n_handles, num_envs], dtype=np.bool_)
+        truncate_handle = np.zeros([self.n_handles, num_envs], dtype=np.bool_)
         episode_score = np.zeros([self.n_handles, num_envs, 1], dtype=np.float32)
 
         for step in range(self.episode_length):
             actions_dict = self.get_actions(obs_n, True, act_mean_last, agent_mask, state)
             actions_execute = self.combine_env_actions(actions_dict['actions_n'])
             next_obs_n, rew_n, terminated_n, truncated_n, infos = test_envs.step(actions_execute)
             if self.args_base.render_mode == "rgb_array" and self.render:
@@ -360,29 +367,25 @@
             def env_fn():
                 args_test = deepcopy(self.args_base)
                 args_test.parallels = args_test.test_episode
                 return make_envs(args_test)
 
             self.render = True
             for h, mas_group in enumerate(self.marl_agents):
-                mas_group.load_model(mas_group.model_dir_load, mas_group.args.seed)
+                mas_group.load_model(mas_group.model_dir_load)
             self.test_episode(env_fn)
             print("Finish testing.")
         else:
             n_train_episodes = self.args_base.running_steps // self.episode_length // self.n_envs
             self.train_episode(n_train_episodes)
             print("Finish training.")
             for h, mas_group in enumerate(self.marl_agents):
                 mas_group.save_model("final_train_model.pth")
 
-        self.envs.close()
-        if self.use_wandb:
-            wandb.finish()
-        else:
-            self.writer.close()
+        self.finish()
 
     def benchmark(self):
         def env_fn():
             args_test = deepcopy(self.args_base)
             args_test.parallels = args_test.test_episode
             return make_envs(args_test)
 
@@ -417,12 +420,8 @@
 
         # end benchmarking
         print("Finish benchmarking.")
         for h in range(self.n_handles):
             print("Best Score for {}: ".format(self.envs.envs[0].side_names[h]))
             print("Mean: ", best_scores[h]["mean"], "Std: ", best_scores[h]["std"])
 
-        self.envs.close()
-        if self.use_wandb:
-            wandb.finish()
-        else:
-            self.writer.close()
+        self.finish()
```

### Comparing `xuance-1.0.9/xuance/torch/runners/runner_sc2.py` & `xuance-1.1.0/xuance/torch/runners/runner_sc2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import socket
 from pathlib import Path
 from .runner_basic import Runner_Base
 from xuance.torch.agents import REGISTRY as REGISTRY_Agent
+from xuance.common import get_time_string
 import wandb
 from torch.utils.tensorboard import SummaryWriter
 import time
 import numpy as np
 from copy import deepcopy
 
 
@@ -14,20 +15,18 @@
     def __init__(self, args):
         super(SC2_Runner, self).__init__(args)
         self.fps = args.fps
         self.args = args
         self.render = args.render
         self.test_envs = None
 
-        time_string = time.asctime().replace(" ", "").replace(":", "_")
+        time_string = get_time_string()
         seed = f"seed_{self.args.seed}_"
         self.args.model_dir_load = args.model_dir
         self.args.model_dir_save = os.path.join(os.getcwd(), args.model_dir, seed + time_string)
-        if (not os.path.exists(self.args.model_dir_save)) and (not args.test_mode):
-            os.makedirs(self.args.model_dir_save)
 
         if args.logger == "tensorboard":
             log_dir = os.path.join(os.getcwd(), args.log_dir, seed + time_string)
             if not os.path.exists(log_dir):
                 os.makedirs(log_dir)
             self.writer = SummaryWriter(log_dir)
             self.use_wandb = False
@@ -39,15 +38,15 @@
             wandb.init(config=config_dict,
                        project=args.project_name,
                        entity=args.wandb_user_name,
                        notes=socket.gethostname(),
                        dir=wandb_dir,
                        group=args.env_id,
                        job_type=args.agent,
-                       name=args.seed,
+                       name=time_string,
                        reinit=True)
             self.use_wandb = True
         else:
             raise RuntimeError(f"The logger named {args.logger} is implemented!")
 
         self.running_steps = args.running_steps
         self.training_frequency = args.training_frequency
```

### Comparing `xuance-1.0.9/xuance/torch/utils/distributions.py` & `xuance-1.1.0/xuance/torch/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/utils/input_reformat.py` & `xuance-1.1.0/xuance/torch/utils/input_reformat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from xuance.common import space2shape
 from copy import deepcopy
 from xuance.torch.utils import ActivationFunctions, NormalizeFunctions, InitializeFunctions
 from xuance.torch.policies import Policy_Inputs, Policy_Inputs_All
 from xuance.torch.representations import Representation_Inputs, Representation_Inputs_All
 from operator import itemgetter
+from gymnasium.spaces import Box, Discrete
 import torch
 
 
 def get_repre_in(args, name=None):
     representation_name = args.representation if name is None else name
     input_dict = deepcopy(Representation_Inputs_All)
     if args.env_name in ["StarCraft2", "Football", "MAgent2"]:
@@ -67,50 +68,55 @@
     else:
         input_dict["actor_hidden_size"] = args.actor_hidden_size
         if policy_name in ["Categorical_AC", "Categorical_PPG", "Gaussian_AC", "Discrete_SAC", "Gaussian_SAC", "Gaussian_PPG", "DDPG_Policy", "TD3_Policy"]:
             input_dict["critic_hidden_size"] = args.critic_hidden_size
     input_dict["normalize"] = NormalizeFunctions[args.normalize] if hasattr(args, "normalize") else None
     input_dict["initialize"] = torch.nn.init.orthogonal_
     input_dict["activation"] = ActivationFunctions[args.activation]
+    try: input_dict["activation_action"] = ActivationFunctions[args.activation_action]
+    except: pass
     input_dict["device"] = args.device
+
     if policy_name == "Gaussian_Actor":
         input_dict["fixed_std"] = None
     if policy_name == "DRQN_Policy":
         return input_dict
     input_list = itemgetter(*Policy_Inputs[policy_name])(input_dict)
     return list(input_list)
 
 
 def get_policy_in_marl(args, representation, mixer=None, ff_mixer=None, qtran_mixer=None):
     policy_name = args.policy
     input_dict = deepcopy(Policy_Inputs_All)
     try: input_dict["state_dim"] = args.dim_state[0]
-    except: input_dict["state_dim"] = None
+    except: pass
 
-    if args.env_name in ["StarCraft2", "Football"]:
-        input_dict["action_space"] = args.action_space
-    else:
+    if isinstance(args.action_space, dict):
         input_dict["action_space"] = args.action_space[args.agent_keys[0]]
+    else:
+        input_dict["action_space"] = args.action_space
 
     try: input_dict["n_agents"] = args.n_agents
-    except: input_dict["n_agents"] = 1
+    except: pass
     input_dict["representation"] = representation
     input_dict["mixer"] = mixer
     input_dict["ff_mixer"] = ff_mixer
     input_dict["qtran_mixer"] = qtran_mixer
     if policy_name in ["Basic_Q_network_marl", "Mixing_Q_network", "Weighted_Mixing_Q_network",
                        "Qtran_Mixing_Q_network", "MF_Q_network"]:
         input_dict["hidden_sizes"] = args.q_hidden_size
     else:
         input_dict["actor_hidden_size"] = args.actor_hidden_size
         try: input_dict["critic_hidden_size"] = args.critic_hidden_size
-        except: input_dict["critic_hidden_size"] = None
+        except: pass
 
     input_dict["initialize"] = InitializeFunctions[args.initialize] if hasattr(args, "initialize") else None
     input_dict["normalize"] = NormalizeFunctions[args.normalize] if hasattr(args, "normalize") else None
     input_dict["activation"] = ActivationFunctions[args.activation]
+    try: input_dict["activation_action"] = ActivationFunctions[args.activation_action]
+    except: pass
 
     input_dict["device"] = args.device
     if policy_name == "Gaussian_Actor":
         input_dict["fixed_std"] = None
     input_list = itemgetter(*Policy_Inputs[policy_name])(input_dict)
     return list(input_list)
```

### Comparing `xuance-1.0.9/xuance/torch/utils/layers.py` & `xuance-1.1.0/xuance/torch/utils/layers.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/utils/operations.py` & `xuance-1.1.0/xuance/torch/utils/operations.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance/torch/utils/value_norm.py` & `xuance-1.1.0/xuance/torch/utils/value_norm.py`

 * *Files identical despite different names*

### Comparing `xuance-1.0.9/xuance.egg-info/SOURCES.txt` & `xuance-1.1.0/xuance.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 xuance/configs/dcg/sc2/2s3z.yaml
 xuance/configs/dcg/sc2/3m.yaml
 xuance/configs/dcg/sc2/5m_vs_6m.yaml
 xuance/configs/dcg/sc2/8m.yaml
 xuance/configs/dcg/sc2/8m_vs_9m.yaml
 xuance/configs/dcg/sc2/MMM2.yaml
 xuance/configs/dcg/sc2/corridor.yaml
+xuance/configs/ddpg/drones.yaml
 xuance/configs/ddpg/mujoco.yaml
 xuance/configs/ddpg/box2d/BipedalWalker-v3.yaml
 xuance/configs/ddpg/classic_control/Pendulum-v1.yaml
 xuance/configs/ddqn/atari.yaml
 xuance/configs/ddqn/box2d/CarRacing-v2.yaml
 xuance/configs/ddqn/box2d/LunarLander-v2.yaml
 xuance/configs/ddqn/classic_control/Acrobot-v1.yaml
@@ -74,14 +75,15 @@
 xuance/configs/drqn/classic_control/MountainCar-v0.yaml
 xuance/configs/dueldqn/atari.yaml
 xuance/configs/dueldqn/box2d/CarRacing-v2.yaml
 xuance/configs/dueldqn/box2d/LunarLander-v2.yaml
 xuance/configs/dueldqn/classic_control/Acrobot-v1.yaml
 xuance/configs/dueldqn/classic_control/CartPole-v1.yaml
 xuance/configs/dueldqn/classic_control/MountainCar-v0.yaml
+xuance/configs/iddpg/drones.yaml
 xuance/configs/iddpg/mpe/simple_adversary_v3.yaml
 xuance/configs/iddpg/mpe/simple_push_v3.yaml
 xuance/configs/iddpg/mpe/simple_spread_v3.yaml
 xuance/configs/ippo/football/3v1.yaml
 xuance/configs/ippo/mpe/simple_spread_v3.yaml
 xuance/configs/ippo/sc2/1c3s5z.yaml
 xuance/configs/ippo/sc2/25m.yaml
@@ -105,14 +107,16 @@
 xuance/configs/iql/sc2/8m.yaml
 xuance/configs/iql/sc2/8m_vs_9m.yaml
 xuance/configs/iql/sc2/MMM2.yaml
 xuance/configs/iql/sc2/corridor.yaml
 xuance/configs/isac/mpe/simple_adversary_v3.yaml
 xuance/configs/isac/mpe/simple_push_v3.yaml
 xuance/configs/isac/mpe/simple_spread_v3.yaml
+xuance/configs/maddpg/drones.yaml
+xuance/configs/maddpg/new_env_mas.yaml
 xuance/configs/maddpg/mpe/simple_adversary_v3.yaml
 xuance/configs/maddpg/mpe/simple_push_v3.yaml
 xuance/configs/maddpg/mpe/simple_spread_v3.yaml
 xuance/configs/mappo/football/1v1.yaml
 xuance/configs/mappo/football/3v1.yaml
 xuance/configs/mappo/mpe/simple_adversary_v3.yaml
 xuance/configs/mappo/mpe/simple_push_v3.yaml
@@ -162,14 +166,15 @@
 xuance/configs/ppg/box2d/LunarLander-v2.yaml
 xuance/configs/ppg/classic_control/Acrobot-v1.yaml
 xuance/configs/ppg/classic_control/CartPole-v1.yaml
 xuance/configs/ppg/classic_control/MountainCar-v0.yaml
 xuance/configs/ppg/classic_control/Pendulum-v1.yaml
 xuance/configs/ppo/atari.yaml
 xuance/configs/ppo/drones.yaml
+xuance/configs/ppo/metadrive.yaml
 xuance/configs/ppo/minigrid.yaml
 xuance/configs/ppo/mujoco.yaml
 xuance/configs/ppo/box2d/BipedalWalker-v3.yaml
 xuance/configs/ppo/box2d/CarRacing-v2.yaml
 xuance/configs/ppo/box2d/LunarLander-v2.yaml
 xuance/configs/ppo/classic_control/Acrobot-v1.yaml
 xuance/configs/ppo/classic_control/CartPole-v1.yaml
@@ -194,14 +199,15 @@
 xuance/configs/qrdqn/classic_control/CartPole-v1.yaml
 xuance/configs/qrdqn/classic_control/MountainCar-v0.yaml
 xuance/configs/qtran/mpe/simple_spread_v3.yaml
 xuance/configs/random/mpe/simple_adversary.yaml
 xuance/configs/random/mpe/simple_push.yaml
 xuance/configs/random/mpe/simple_spread.yaml
 xuance/configs/sac/atari.yaml
+xuance/configs/sac/metadrive.yaml
 xuance/configs/sac/mujoco.yaml
 xuance/configs/sac/box2d/BipedalWalker-v3.yaml
 xuance/configs/sac/box2d/LunarLander-v2.yaml
 xuance/configs/sac/classic_control/Acrobot-v1.yaml
 xuance/configs/sac/classic_control/CartPole-v1.yaml
 xuance/configs/sac/classic_control/MountainCar-v0.yaml
 xuance/configs/sac/classic_control/Pendulum-v1.yaml
@@ -216,14 +222,15 @@
 xuance/configs/vdac/sc2/2s3z.yaml
 xuance/configs/vdac/sc2/3m.yaml
 xuance/configs/vdac/sc2/5m_vs_6m.yaml
 xuance/configs/vdac/sc2/8m.yaml
 xuance/configs/vdac/sc2/8m_vs_9m.yaml
 xuance/configs/vdac/sc2/MMM2.yaml
 xuance/configs/vdac/sc2/corridor.yaml
+xuance/configs/vdn/new_env_mas.yaml
 xuance/configs/vdn/football/3v1.yaml
 xuance/configs/vdn/mpe/simple_spread_v3.yaml
 xuance/configs/vdn/sc2/1c3s5z.yaml
 xuance/configs/vdn/sc2/25m.yaml
 xuance/configs/vdn/sc2/2m_vs_1z.yaml
 xuance/configs/vdn/sc2/2s3z.yaml
 xuance/configs/vdn/sc2/3m.yaml
@@ -243,14 +250,18 @@
 xuance/configs/wqmix/sc2/8m_vs_9m.yaml
 xuance/configs/wqmix/sc2/MMM2.yaml
 xuance/configs/wqmix/sc2/corridor.yaml
 xuance/environment/__init__.py
 xuance/environment/drones/__init__.py
 xuance/environment/drones/drones_env.py
 xuance/environment/drones/drones_vec_env.py
+xuance/environment/drones/drones_vec_env_mas.py
+xuance/environment/drones/customized/HoverAviary.py
+xuance/environment/drones/customized/MultiHoverAviary.py
+xuance/environment/drones/customized/__init__.py
 xuance/environment/football/__init__.py
 xuance/environment/football/gfootball_env.py
 xuance/environment/football/gfootball_vec_env.py
 xuance/environment/football/raw_env.py
 xuance/environment/gym/__init__.py
 xuance/environment/gym/gym_env.py
 xuance/environment/gym/gym_vec_env.py
@@ -290,23 +301,31 @@
 xuance/environment/magent2/environments/battlefield/battlefield.py
 xuance/environment/magent2/environments/combined_arms/__init__.py
 xuance/environment/magent2/environments/combined_arms/combined_arms.py
 xuance/environment/magent2/environments/gather/__init__.py
 xuance/environment/magent2/environments/gather/gather.py
 xuance/environment/magent2/environments/tiger_deer/__init__.py
 xuance/environment/magent2/environments/tiger_deer/tiger_deer.py
+xuance/environment/metadrive/__init__.py
+xuance/environment/metadrive/metadrive_env.py
+xuance/environment/metadrive/metadrive_vec_env.py
 xuance/environment/minigrid/__init__.py
 xuance/environment/minigrid/minigrid_env.py
 xuance/environment/minigrid/minigrid_vec_env.py
 xuance/environment/new_env/__init__.py
 xuance/environment/new_env/new_env.py
 xuance/environment/new_env/new_vec_env.py
+xuance/environment/new_env_mas/__init__.py
+xuance/environment/new_env_mas/new_env_mas.py
+xuance/environment/new_env_mas/new_vec_env_mas.py
 xuance/environment/pettingzoo/__init__.py
 xuance/environment/pettingzoo/pettingzoo_env.py
 xuance/environment/pettingzoo/pettingzoo_vec_env.py
+xuance/environment/robotic_warehouse/__init__.py
+xuance/environment/robotic_warehouse/robotic_warehouse_env.py
 xuance/environment/starcraft2/__init__.py
 xuance/environment/starcraft2/sc2_env.py
 xuance/environment/starcraft2/sc2_vec_env.py
 xuance/environment/vector_envs/__init__.py
 xuance/environment/vector_envs/env_utils.py
 xuance/environment/vector_envs/subproc_vec_env.py
 xuance/environment/vector_envs/vector_env.py
@@ -627,14 +646,15 @@
 xuance/torch/representations/mlp.py
 xuance/torch/representations/rnn.py
 xuance/torch/runners/__init__.py
 xuance/torch/runners/runner_basic.py
 xuance/torch/runners/runner_drl.py
 xuance/torch/runners/runner_football.py
 xuance/torch/runners/runner_magent.py
+xuance/torch/runners/runner_marl.py
 xuance/torch/runners/runner_pettingzoo.py
 xuance/torch/runners/runner_sc2.py
 xuance/torch/utils/__init__.py
 xuance/torch/utils/distributions.py
 xuance/torch/utils/input_reformat.py
 xuance/torch/utils/layers.py
 xuance/torch/utils/operations.py
```

