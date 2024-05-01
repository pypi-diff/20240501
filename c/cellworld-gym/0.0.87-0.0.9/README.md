# Comparing `tmp/cellworld_gym-0.0.87.tar.gz` & `tmp/cellworld_gym-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellworld_gym-0.0.87.tar", last modified: Wed May  1 01:43:06 2024, max compression
+gzip compressed data, was "cellworld_gym-0.0.9.tar", last modified: Thu Apr 18 15:03:36 2024, max compression
```

## Comparing `cellworld_gym-0.0.87.tar` & `cellworld_gym-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 01:43:06.151226 cellworld_gym-0.0.87/
--rw-rw-rw-   0        0        0       35 2024-05-01 01:43:05.000000 cellworld_gym-0.0.87/MANIFEST.in
--rw-rw-rw-   0        0        0      455 2024-05-01 01:43:06.151226 cellworld_gym-0.0.87/PKG-INFO
--rw-rw-rw-   0        0        0       40 2024-05-01 01:43:05.000000 cellworld_gym-0.0.87/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 01:43:06.104239 cellworld_gym-0.0.87/cellworld_gym/
--rw-rw-rw-   0        0        0       40 2024-05-01 01:43:05.000000 cellworld_gym-0.0.87/cellworld_gym/README.md
--rw-rw-rw-   0        0        0       90 2024-04-30 14:54:10.000000 cellworld_gym-0.0.87/cellworld_gym/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 01:43:06.124277 cellworld_gym-0.0.87/cellworld_gym/__pycache__/
--rw-rw-rw-   0        0        0      253 2024-04-30 15:10:42.000000 cellworld_gym-0.0.87/cellworld_gym/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     4221 2024-04-30 15:10:42.000000 cellworld_gym-0.0.87/cellworld_gym/__pycache__/core.cpython-312.pyc
--rw-rw-rw-   0        0        0     2156 2024-04-30 14:54:10.000000 cellworld_gym-0.0.87/cellworld_gym/core.py
-drwxrwxrwx   0        0        0        0 2024-05-01 01:43:06.146160 cellworld_gym-0.0.87/cellworld_gym/envs/
--rw-rw-rw-   0        0        0      499 2024-04-30 14:54:10.000000 cellworld_gym-0.0.87/cellworld_gym/envs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 01:43:06.149153 cellworld_gym-0.0.87/cellworld_gym/envs/__pycache__/
--rw-rw-rw-   0        0        0      751 2024-04-30 15:10:42.000000 cellworld_gym-0.0.87/cellworld_gym/envs/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     9657 2024-04-30 21:04:11.000000 cellworld_gym-0.0.87/cellworld_gym/envs/__pycache__/bot_evade.cpython-312.pyc
--rw-rw-rw-   0        0        0    11508 2024-04-30 20:58:13.000000 cellworld_gym-0.0.87/cellworld_gym/envs/__pycache__/dual_evade.cpython-312.pyc
--rw-rw-rw-   0        0        0     9750 2024-04-30 20:58:13.000000 cellworld_gym-0.0.87/cellworld_gym/envs/__pycache__/oasis.cpython-312.pyc
--rw-rw-rw-   0        0        0     5577 2024-05-01 00:37:25.000000 cellworld_gym-0.0.87/cellworld_gym/envs/bot_evade.py
--rw-rw-rw-   0        0        0     7518 2024-04-30 20:57:51.000000 cellworld_gym-0.0.87/cellworld_gym/envs/dual_evade.py
--rw-rw-rw-   0        0        0     5810 2024-04-30 20:57:51.000000 cellworld_gym-0.0.87/cellworld_gym/envs/oasis.py
--rw-rw-rw-   0        0        0     1636 2024-05-01 01:43:05.000000 cellworld_gym-0.0.87/cellworld_gym/license.txt
--rw-rw-rw-   0        0        0      180 2024-05-01 01:43:05.000000 cellworld_gym-0.0.87/cellworld_gym/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-01 01:43:06.150223 cellworld_gym-0.0.87/cellworld_gym.egg-info/
--rw-rw-rw-   0        0        0      455 2024-05-01 01:43:06.000000 cellworld_gym-0.0.87/cellworld_gym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      818 2024-05-01 01:43:06.000000 cellworld_gym-0.0.87/cellworld_gym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 01:43:06.000000 cellworld_gym-0.0.87/cellworld_gym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-01 01:43:06.000000 cellworld_gym-0.0.87/cellworld_gym.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2024-05-01 01:43:06.000000 cellworld_gym-0.0.87/cellworld_gym.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-01 01:43:06.000000 cellworld_gym-0.0.87/cellworld_gym.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 01:43:06.152267 cellworld_gym-0.0.87/setup.cfg
--rw-rw-rw-   0        0        0      652 2024-05-01 01:43:05.000000 cellworld_gym-0.0.87/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:03:36.908794 cellworld_gym-0.0.9/
+-rw-rw-rw-   0        0        0       35 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      415 2024-04-18 15:03:36.907727 cellworld_gym-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 15:03:36.873624 cellworld_gym-0.0.9/cellworld_gym/
+-rw-rw-rw-   0        0        0       40 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym/README.md
+-rw-rw-rw-   0        0        0       72 2024-04-18 15:03:01.000000 cellworld_gym-0.0.9/cellworld_gym/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 15:03:36.904706 cellworld_gym-0.0.9/cellworld_gym/envs/
+-rw-rw-rw-   0        0        0      141 2024-04-18 14:54:55.000000 cellworld_gym-0.0.9/cellworld_gym/envs/__init__.py
+-rw-rw-rw-   0        0        0     5839 2024-04-17 20:14:13.000000 cellworld_gym-0.0.9/cellworld_gym/envs/bot_evade.py
+-rw-rw-rw-   0        0        0     1636 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym/license.txt
+-rw-rw-rw-   0        0        0      192 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 15:03:36.906775 cellworld_gym-0.0.9/cellworld_gym.egg-info/
+-rw-rw-rw-   0        0        0      415 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/cellworld_gym.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 15:03:36.908794 cellworld_gym-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      605 2024-04-18 15:03:36.000000 cellworld_gym-0.0.9/setup.py
```

### Comparing `cellworld_gym-0.0.87/cellworld_gym/envs/oasis.py` & `cellworld_gym-0.0.9/cellworld_gym/envs/bot_evade.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,147 +1,127 @@
-import typing
-import cellworld_game as cwgame
-import numpy as np
-import math
-
-from ..core import Observation
-from cellworld_game import AgentState
-from gymnasium import Env
-from gymnasium import spaces
-
-
-class OasisObservation(Observation):
-    fields = ["prey_x",
-              "prey_y",
-              "prey_direction",
-              "predator_x",
-              "predator_y",
-              "predator_direction",
-              "prey_goal_distance",
-              "predator_prey_distance",
-              "puffed",
-              "puff_cooled_down",
-              "finished",
-              "goal_attained",
-              "goal_time_left"]
-
-
-class OasisEnv(Env):
-    def __init__(self,
-                 world_name: str,
-                 goal_locations: typing.List[typing.Tuple[float, float]],
-                 use_lppos: bool,
-                 use_predator: bool,
-                 goal_sequence_generator: typing.Callable[[None], typing.List[int]] = None,
-                 max_step: int = 300,
-                 reward_function: typing.Callable[[OasisObservation], float] = lambda x: 0,
-                 time_step: float = .25,
-                 render: bool = False,
-                 real_time: bool = False):
-
-        self.max_step = max_step
-        self.reward_function = reward_function
-        self.time_step = time_step
-        self.loader = cwgame.CellWorldLoader(world_name=world_name)
-        self.observation = OasisObservation()
-        self.observation_space = spaces.Box(-np.inf, np.inf, (len(self.observation),), dtype=np.float32)
-        if use_lppos:
-            self.action_list = self.loader.tlppo_action_list
-        else:
-            self.action_list = self.loader.full_action_list
-
-        self.action_space = spaces.Discrete(len(self.action_list))
-
-        self.model = cwgame.Oasis(world_name="21_05",
-                                  real_time=real_time,
-                                  render=render,
-                                  use_predator=use_predator,
-                                  goal_locations=goal_locations,
-                                  goal_sequence_generator=goal_sequence_generator)
-        self.prey_trajectory_length = 0
-        self.predator_trajectory_length = 0
-        self.episode_reward = 0
-        self.step_count = 0
-
-    def __update_observation__(self):
-        self.observation.prey_x = self.model.prey.state.location[0]
-        self.observation.prey_y = self.model.prey.state.location[1]
-        self.observation.prey_direction = math.radians(self.model.prey.state.direction)
-
-        if self.model.use_predator and self.model.visibility.line_of_sight(self.model.prey.state.location, self.model.predator.state.location):
-            self.observation.predator_x = self.model.predator.state.location[0]
-            self.observation.predator_y = self.model.predator.state.location[1]
-            self.observation.predator_direction = math.radians(self.model.predator.state.direction)
-        else:
-            self.observation.predator_x = 0
-            self.observation.predator_y = 0
-            self.observation.predator_direction = 0
-
-        self.observation.prey_goal_distance = self.model.prey_goal_distance
-        self.observation.predator_prey_distance = self.model.predator_prey_distance
-        self.observation.puffed = self.model.puffed
-        self.observation.puff_cooled_down = self.model.puff_cool_down
-        self.observation.goal_attained = self.model.goal_achieved
-        if self.observation.goal_attained:
-            self.observation.goal_time_left = self.model.goal_time - self.model.goal_achieved_time
-        else:
-            self.observation.goal_time_left = 0
-        self.observation.finished = not self.model.running
-        return self.observation
-
-    def set_action(self, action: int):
-        self.model.prey.set_destination(self.action_list[action])
-
-    def __step__(self):
-        truncated = (self.step_count >= self.max_step)
-        obs = self.__update_observation__()
-        reward = self.reward_function(obs)
-        self.episode_reward += reward
-
-        if self.model.puffed:
-            self.model.puffed = False
-        if not self.model.running or truncated:
-            survived = 1 if not self.model.running and self.model.puff_count == 0 else 0
-            info = {"captures": self.model.puff_count,
-                    "reward": self.episode_reward,
-                    "is_success": survived,
-                    "survived": survived,
-                    "agents": {}}
-            for agent_name, agent in self.model.agents.items():
-                info["agents"][agent_name] = {}
-                info["agents"][agent_name] = agent.get_stats()
-        else:
-            info = {}
-        self.step_count += 1
-        return obs, reward, not self.model.running, truncated, info
-
-    def replay_step(self, agents_state: typing.Dict[str, AgentState]):
-        self.model.set_agents_state(agents_state=agents_state,
-                                    delta_t=self.time_step)
-        return self.__step__()
-
-    def step(self, action: int):
-        self.set_action(action=action)
-        model_t = self.model.time + self.time_step
-        while self.model.running and self.model.time < model_t:
-            self.model.step()
-        return self.__step__()
-
-    def __reset__(self):
-        self.episode_reward = 0
-        self.step_count = 0
-        return self.__update_observation__(), {}
-
-    def reset(self,
-              options={},
-              seed=None):
-        self.model.reset()
-        return self.__reset__()
-
-    def replay_reset(self, agents_state: typing.Dict[str, AgentState]):
-        self.model.reset()
-        self.model.set_agents_state(agents_state=agents_state)
-        return self.__reset__()
-
-    def close(self):
-        self.model.close()
-        Env.close(self=self)
+from cellworld_game import Model, Robot, Mouse, MouseObservation, AgentState, View, distance, CellWorldLoader
+from gymnasium import Env
+from gymnasium import spaces
+import numpy as np
+import math
+
+
+class BotEvade(Env):
+    def __init__(self,
+                 world_name: str,
+                 use_lppos: bool,
+                 use_predator: bool,
+                 max_step: int = 200,
+                 reward_function=lambda x: 0,
+                 step_wait: int = 5,
+                 render: bool = False,
+                 real_time: bool = False):
+        self.max_step = max_step
+        self.reward_function = reward_function
+        self.step_wait = step_wait
+        self.loader = CellWorldLoader(world_name=world_name)
+        self.observation = MouseObservation()
+        self.observation_space = spaces.Box(-np.inf, np.inf, (len(self.observation),), dtype=np.float32)
+        self.action_space = spaces.Discrete(len(self.loader.tlppo_action_list)
+                                            if use_lppos
+                                            else len(self.loader.open_locations))
+        if use_lppos:
+            self.action_list = self.loader.tlppo_action_list
+        else:
+            self.action_list = self.loader.full_action_list
+
+        self.model = Model(arena=self.loader.arena,
+                           occlusions=self.loader.occlusions,
+                           time_step=.025,
+                           real_time=real_time)
+        if use_predator:
+            self.predator = Robot(start_locations=self.loader.robot_start_locations,
+                                  open_locations=self.loader.open_locations,
+                                  navigation=self.loader.navigation)
+            self.model.add_agent("predator", self.predator)
+
+        self.prey = Mouse(start_state=AgentState(location=(.05, .5),
+                                                 direction=0),
+                          goal_location=(1, .5),
+                          goal_threshold=.1,
+                          puff_threshold=.1,
+                          puff_cool_down_time=.5,
+                          navigation=self.loader.navigation,
+                          actions=self.action_list,
+                          predator=self.predator)
+        self.model.add_agent("prey", self.prey)
+        self.view = None
+        self.render_steps = render
+        self.step_count = 0
+        self.captures = 0
+        self.prey_trajectory_length = 0
+        self.predator_trajectory_length = 0
+        self.episode_reward = 0
+
+    def get_observation(self):
+        self.observation[MouseObservation.Field.prey_x] = self.prey.state.location[0]
+        self.observation[MouseObservation.Field.prey_y] = self.prey.state.location[1]
+        self.observation[MouseObservation.Field.prey_direction] = math.radians(self.prey.state.direction)
+
+        if self.model.visibility.line_of_sight(self.prey.state.location, self.predator.state.location):
+            self.observation[MouseObservation.Field.predator_x] = self.predator.state.location[0]
+            self.observation[MouseObservation.Field.predator_y] = self.predator.state.location[1]
+            self.observation[MouseObservation.Field.predator_direction] = math.radians(
+                self.predator.state.direction)
+            predator_distance = distance(self.prey.state.location, self.predator.state.location)
+        else:
+            self.observation[MouseObservation.Field.predator_x] = 0
+            self.observation[MouseObservation.Field.predator_y] = 0
+            self.observation[MouseObservation.Field.predator_direction] = 0
+            predator_distance = 1
+
+        goal_distance = distance(self.prey.goal_location, self.prey.state.location)
+        self.observation[MouseObservation.Field.goal_distance] = goal_distance
+        self.observation[MouseObservation.Field.predator_distance] = predator_distance
+        self.observation[MouseObservation.Field.puffed] = self.prey.puffed
+        self.observation[MouseObservation.Field.puff_cooled_down] = self.prey.puff_cool_down
+        self.observation[MouseObservation.Field.finished] = self.prey.finished
+        return self.observation
+
+    def set_action(self, action: int):
+        self.prey.set_action(action)
+
+    def step(self, action: int):
+        self.step_count += 1
+        self.set_action(action=action)
+        for i in range(self.step_wait):
+            self.model.step()
+            if self.render_steps:
+                self.render()
+        truncated = (self.step_count >= self.max_step)
+        obs = self.get_observation()
+        reward = self.reward_function(obs)
+        self.episode_reward += reward
+
+        if self.prey.puffed:
+            self.captures += 1
+            self.prey.puffed = False
+        if self.prey.finished or truncated:
+            info = {"captures": self.captures,
+                    "reward": self.episode_reward,
+                    "is_success": 1 if self.prey.finished and self.captures == 0 else 0,
+                    "survived": 1 if self.prey.finished and self.captures == 0 else 0,
+                    "agents": {}}
+            for agent_name, agent in self.model.agents.items():
+                info["agents"][agent_name] = {}
+                info["agents"][agent_name] = agent.get_stats()
+        else:
+            info = {}
+        return obs, reward, self.prey.finished, truncated, info
+
+    def reset(self, seed=None):
+        self.captures = 0
+        self.step_count = 0
+        self.episode_reward = 0
+        self.model.reset()
+        obs = self.get_observation()
+        return obs, {}
+
+    def render(self):
+        if self.view is None:
+            self.view = View(model=self.model)
+        self.view.draw()
```

### Comparing `cellworld_gym-0.0.87/cellworld_gym/license.txt` & `cellworld_gym-0.0.9/cellworld_gym/license.txt`

 * *Files identical despite different names*

