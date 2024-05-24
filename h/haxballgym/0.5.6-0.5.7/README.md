# Comparing `tmp/haxballgym-0.5.6.tar.gz` & `tmp/haxballgym-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haxballgym-0.5.6.tar", max compression
+gzip compressed data, was "haxballgym-0.5.7.tar", max compression
```

## Comparing `haxballgym-0.5.6.tar` & `haxballgym-0.5.7.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0       24 2023-02-05 18:42:56.861260 haxballgym-0.5.6/haxballgym/__init__.py
--rw-r--r--   0        0        0       64 2022-05-26 15:12:42.549646 haxballgym-0.5.6/haxballgym/envs/__init__.py
--rw-r--r--   0        0        0      821 2023-02-12 13:26:09.145355 haxballgym-0.5.6/haxballgym/envs/environment.py
--rw-r--r--   0        0        0     4878 2023-02-12 13:54:21.309867 haxballgym-0.5.6/haxballgym/envs/match.py
--rw-r--r--   0        0        0     2896 2023-02-12 14:11:44.324957 haxballgym-0.5.6/haxballgym/gym.py
--rw-r--r--   0        0        0     2377 2023-02-05 18:38:40.827224 haxballgym-0.5.6/haxballgym/make.py
--rw-r--r--   0        0        0      136 2023-02-05 18:39:29.102453 haxballgym-0.5.6/haxballgym/utils/__init__.py
--rw-r--r--   0        0        0      123 2022-05-26 15:12:42.559646 haxballgym-0.5.6/haxballgym/utils/action_parsers/__init__.py
--rw-r--r--   0        0        0     1024 2023-02-05 18:43:23.537150 haxballgym-0.5.6/haxballgym/utils/action_parsers/action_parser.py
--rw-r--r--   0        0        0      956 2023-02-05 18:44:27.589079 haxballgym-0.5.6/haxballgym/utils/action_parsers/default_act.py
--rw-r--r--   0        0        0     1256 2023-02-05 18:43:29.303835 haxballgym-0.5.6/haxballgym/utils/action_parsers/discrete_act.py
--rw-r--r--   0        0        0       66 2022-05-26 15:12:42.559646 haxballgym-0.5.6/haxballgym/utils/common_values.py
--rw-r--r--   0        0        0       35 2022-05-26 15:12:42.560646 haxballgym-0.5.6/haxballgym/utils/gamestates/__init__.py
--rw-r--r--   0        0        0     1405 2023-02-05 18:43:35.198805 haxballgym-0.5.6/haxballgym/utils/gamestates/game_state.py
--rw-r--r--   0        0        0       74 2022-05-26 15:12:42.560646 haxballgym-0.5.6/haxballgym/utils/obs_builders/__init__.py
--rw-r--r--   0        0        0     1639 2023-02-05 18:43:39.729179 haxballgym-0.5.6/haxballgym/utils/obs_builders/default_obs.py
--rw-r--r--   0        0        0     1758 2023-02-05 18:43:43.073149 haxballgym-0.5.6/haxballgym/utils/obs_builders/obs_builder.py
--rw-r--r--   0        0        0      133 2022-05-26 15:12:42.561646 haxballgym-0.5.6/haxballgym/utils/reward_functions/__init__.py
--rw-r--r--   0        0        0     3642 2023-02-05 18:44:21.661152 haxballgym-0.5.6/haxballgym/utils/reward_functions/combined_reward.py
--rw-r--r--   0        0        0       63 2022-05-26 15:12:42.561646 haxballgym-0.5.6/haxballgym/utils/reward_functions/common_rewards/__init__.py
--rw-r--r--   0        0        0     2324 2023-02-05 18:44:31.756853 haxballgym-0.5.6/haxballgym/utils/reward_functions/common_rewards/conditional_rewards.py
--rw-r--r--   0        0        0     4465 2023-02-05 18:44:17.361942 haxballgym-0.5.6/haxballgym/utils/reward_functions/common_rewards/misc_rewards.py
--rw-r--r--   0        0        0      847 2023-02-05 18:44:20.410893 haxballgym-0.5.6/haxballgym/utils/reward_functions/default_reward.py
--rw-r--r--   0        0        0     2132 2023-02-05 18:44:19.584697 haxballgym-0.5.6/haxballgym/utils/reward_functions/reward_function.py
--rw-r--r--   0        0        0     2601 2023-02-05 18:44:07.765900 haxballgym-0.5.6/haxballgym/utils/reward_functions/velocity_reward.py
--rw-r--r--   0        0        0       85 2022-05-26 15:12:42.563646 haxballgym-0.5.6/haxballgym/utils/terminal_conditions/__init__.py
--rw-r--r--   0        0        0     3040 2023-02-05 18:44:39.130037 haxballgym-0.5.6/haxballgym/utils/terminal_conditions/common_conditions.py
--rw-r--r--   0        0        0      972 2023-02-05 18:44:47.144864 haxballgym-0.5.6/haxballgym/utils/terminal_conditions/terminal_condition.py
--rw-r--r--   0        0        0      496 2023-02-12 14:40:15.247617 haxballgym-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      877 2022-11-26 19:12:22.350286 haxballgym-0.5.6/README.md
--rw-r--r--   0        0        0     1931 1970-01-01 00:00:00.000000 haxballgym-0.5.6/setup.py
--rw-r--r--   0        0        0     1444 1970-01-01 00:00:00.000000 haxballgym-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      850 2024-05-24 20:15:56.144304 haxballgym-0.5.7/README.md
+-rw-r--r--   0        0        0       23 2024-05-24 20:15:56.144560 haxballgym-0.5.7/haxballgym/__init__.py
+-rw-r--r--   0        0        0       62 2024-05-24 20:15:56.144725 haxballgym-0.5.7/haxballgym/envs/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-24 20:15:56.144812 haxballgym-0.5.7/haxballgym/envs/environment.py
+-rw-r--r--   0        0        0     4885 2024-05-24 20:15:56.144966 haxballgym-0.5.7/haxballgym/envs/match.py
+-rw-r--r--   0        0        0     2812 2024-05-24 20:15:56.145058 haxballgym-0.5.7/haxballgym/gym.py
+-rw-r--r--   0        0        0     2458 2024-05-24 20:15:56.145143 haxballgym-0.5.7/haxballgym/make.py
+-rw-r--r--   0        0        0      133 2024-05-24 20:15:56.145304 haxballgym-0.5.7/haxballgym/utils/__init__.py
+-rw-r--r--   0        0        0      120 2024-05-24 20:15:56.145441 haxballgym-0.5.7/haxballgym/utils/action_parsers/__init__.py
+-rw-r--r--   0        0        0      986 2024-05-24 20:15:56.145532 haxballgym-0.5.7/haxballgym/utils/action_parsers/action_parser.py
+-rw-r--r--   0        0        0      924 2024-05-24 20:15:56.145616 haxballgym-0.5.7/haxballgym/utils/action_parsers/default_act.py
+-rw-r--r--   0        0        0     1221 2024-05-24 20:15:56.145726 haxballgym-0.5.7/haxballgym/utils/action_parsers/discrete_act.py
+-rw-r--r--   0        0        0       62 2024-05-24 20:15:56.145828 haxballgym-0.5.7/haxballgym/utils/common_values.py
+-rw-r--r--   0        0        0       34 2024-05-24 20:15:56.145991 haxballgym-0.5.7/haxballgym/utils/gamestates/__init__.py
+-rw-r--r--   0        0        0     1363 2024-05-24 20:15:56.146101 haxballgym-0.5.7/haxballgym/utils/gamestates/game_state.py
+-rw-r--r--   0        0        0       72 2024-05-24 20:15:56.146251 haxballgym-0.5.7/haxballgym/utils/obs_builders/__init__.py
+-rw-r--r--   0        0        0     1639 2024-05-24 20:15:56.146344 haxballgym-0.5.7/haxballgym/utils/obs_builders/default_obs.py
+-rw-r--r--   0        0        0     1711 2024-05-24 20:15:56.146440 haxballgym-0.5.7/haxballgym/utils/obs_builders/obs_builder.py
+-rw-r--r--   0        0        0      130 2024-05-24 20:15:56.146597 haxballgym-0.5.7/haxballgym/utils/reward_functions/__init__.py
+-rw-r--r--   0        0        0     3537 2024-05-24 20:15:56.146733 haxballgym-0.5.7/haxballgym/utils/reward_functions/combined_reward.py
+-rw-r--r--   0        0        0       62 2024-05-24 20:15:56.146914 haxballgym-0.5.7/haxballgym/utils/reward_functions/common_rewards/__init__.py
+-rw-r--r--   0        0        0     2257 2024-05-24 20:15:56.147015 haxballgym-0.5.7/haxballgym/utils/reward_functions/common_rewards/conditional_rewards.py
+-rw-r--r--   0        0        0     4339 2024-05-24 20:15:56.147161 haxballgym-0.5.7/haxballgym/utils/reward_functions/common_rewards/misc_rewards.py
+-rw-r--r--   0        0        0      847 2024-05-24 20:15:56.147258 haxballgym-0.5.7/haxballgym/utils/reward_functions/default_reward.py
+-rw-r--r--   0        0        0     2078 2024-05-24 20:15:56.147358 haxballgym-0.5.7/haxballgym/utils/reward_functions/reward_function.py
+-rw-r--r--   0        0        0     2523 2024-05-24 20:15:56.147453 haxballgym-0.5.7/haxballgym/utils/reward_functions/velocity_reward.py
+-rw-r--r--   0        0        0      116 2024-05-24 20:15:56.147604 haxballgym-0.5.7/haxballgym/utils/state_setters/__init__.py
+-rw-r--r--   0        0        0      262 2024-05-24 20:15:56.147691 haxballgym-0.5.7/haxballgym/utils/state_setters/default_state.py
+-rw-r--r--   0        0        0      255 2024-05-24 20:15:56.147789 haxballgym-0.5.7/haxballgym/utils/state_setters/random_state.py
+-rw-r--r--   0        0        0      324 2024-05-24 20:15:56.147891 haxballgym-0.5.7/haxballgym/utils/state_setters/state_setter.py
+-rw-r--r--   0        0        0       83 2024-05-24 20:15:56.148054 haxballgym-0.5.7/haxballgym/utils/terminal_conditions/__init__.py
+-rw-r--r--   0        0        0     2943 2024-05-24 20:15:56.148159 haxballgym-0.5.7/haxballgym/utils/terminal_conditions/common_conditions.py
+-rw-r--r--   0        0        0      939 2024-05-24 20:15:56.148264 haxballgym-0.5.7/haxballgym/utils/terminal_conditions/terminal_condition.py
+-rw-r--r--   0        0        0      480 2024-05-24 20:22:44.383268 haxballgym-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     1401 1970-01-01 00:00:00.000000 haxballgym-0.5.7/PKG-INFO
```

### Comparing `haxballgym-0.5.6/haxballgym/gym.py` & `haxballgym-0.5.7/haxballgym/gym.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-"""
-    The HaxBall gym environment.
-"""
-
-from typing import Dict, List, Tuple, Union
-
-import numpy as np
-from gym import Env
-
-from haxballgym.envs.match import Match
-
-
-class Gym(Env):
-    def __init__(self, match: Match):
-        super().__init__()
-
-        self._match = match
-        self.observation_space = match.observation_space
-        self.action_space = match.action_space
-
-        self._prev_state = None
-
-    def reset(self, return_info=False, save_recording=False) -> Union[List, Tuple]:
-        """
-        The environment reset function.
-        When called, this will reset the state of the environment.
-        This should be called once when the environment is initialized,
-        then every time the `done` flag from the `step()` function is `True`.
-        """
-
-        self._match.get_reset_state(save_recording)
-        state = self._receive_state()
-        self._match.episode_reset(state)
-        self._prev_state = state
-
-        obs = self._match.build_observations(state)
-        if return_info:
-            info = {"state": state, "result": self._match.get_result(state)}
-            return obs, info
-        return obs
-
-    def step(self, actions: list[int] | np.ndarray) -> Tuple[List, List, bool, Dict]:
-        """
-        The step function will send the list of provided actions to the game,
-        then advance the game forward by `tick_skip` physics ticks using that action.
-        We then get the `GameState` object, which gets passed to the configuration
-        objects to determine the rewards, next observation, and done signal.
-
-        :param actions: An object containing actions, in the correct format
-        :return: A tuple containing (obs, rewards, done, info)
-        """
-        actions = self._match.parse_actions(actions, self._prev_state)
-        actions_all = self._get_all_actions(actions)
-
-        for _ in range(self._match._tick_skip + 1):
-            self._match._game.step(actions_all)
-
-        state = self._receive_state()
-        obs = self._match.build_observations(state)
-        done = self._match.is_done(state)
-        reward = self._match.get_rewards(state, done)
-        self._prev_state = state
-
-        info = {"state": state, "result": self._match.get_result(state)}
-
-        return obs, reward, done, info
-
-    def _receive_state(self):
-        self._match._game_state.update(self._match._game)
-        return self._match._game_state
-
-    def _get_all_actions(self, actions: list[int] | np.ndarray):
-        if self._match._bots is None:
-            return actions
-
-        actions_all = [p.step(self._match._game) for p in self._match._game.players]
-
-        i = 0
-        for j, act in enumerate(actions_all):
-            if act is None:
-                actions_all[j] = actions[i]
-                i += 1
-
-        return actions_all
+"""
+    The HaxBall gym environment.
+"""
+
+from typing import Dict, List, Tuple, Union
+
+import numpy as np
+from gym import Env
+
+from haxballgym.envs.match import Match
+
+
+class Gym(Env):
+    def __init__(self, match: Match):
+        super().__init__()
+
+        self._match = match
+        self.observation_space = match.observation_space
+        self.action_space = match.action_space
+
+        self._prev_state = None
+
+    def reset(self, return_info=False, save_recording=False) -> Union[List, Tuple]:
+        """
+        The environment reset function.
+        When called, this will reset the state of the environment.
+        This should be called once when the environment is initialized,
+        then every time the `done` flag from the `step()` function is `True`.
+        """
+
+        self._match.get_reset_state(save_recording)
+        state = self._receive_state()
+        self._match.episode_reset(state)
+        self._prev_state = state
+
+        obs = self._match.build_observations(state)
+        if return_info:
+            info = {"state": state, "result": self._match.get_result(state)}
+            return obs, info
+        return obs
+
+    def step(self, actions: list[int] | np.ndarray) -> Tuple[List, List, bool, Dict]:
+        """
+        The step function will send the list of provided actions to the game,
+        then advance the game forward by `tick_skip` physics ticks using that action.
+        We then get the `GameState` object, which gets passed to the configuration
+        objects to determine the rewards, next observation, and done signal.
+
+        :param actions: An object containing actions, in the correct format
+        :return: A tuple containing (obs, rewards, done, info)
+        """
+        actions = self._match.parse_actions(actions, self._prev_state)
+        actions_all = self._get_all_actions(actions)
+
+        for _ in range(self._match._tick_skip + 1):
+            self._match._game.step(actions_all)
+
+        state = self._receive_state()
+        obs = self._match.build_observations(state)
+        done = self._match.is_done(state)
+        reward = self._match.get_rewards(state, done)
+        self._prev_state = state
+
+        info = {"state": state, "result": self._match.get_result(state)}
+
+        return obs, reward, done, info
+
+    def _receive_state(self):
+        self._match._game_state.update(self._match._game)
+        return self._match._game_state
+
+    def _get_all_actions(self, actions: list[int] | np.ndarray):
+        if self._match._bots is None:
+            return actions
+
+        actions_all = [p.step(self._match._game) for p in self._match._game.players]
+
+        i = 0
+        for j, act in enumerate(actions_all):
+            if act is None:
+                actions_all[j] = actions[i]
+                i += 1
+
+        return actions_all
```

### Comparing `haxballgym-0.5.6/haxballgym/make.py` & `haxballgym-0.5.7/haxballgym/make.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,74 @@
-from typing import List
-
-from ursinaxball import Game, common_values
-from ursinaxball.modules import Bot, GameScore, PlayerHandler
-
-from haxballgym.envs import Match
-from haxballgym.gym import Gym
-from haxballgym.utils.action_parsers import ActionParser, DefaultAction
-from haxballgym.utils.obs_builders import DefaultObs, ObsBuilder
-from haxballgym.utils.reward_functions import RewardFunction, common_rewards
-from haxballgym.utils.terminal_conditions import TerminalCondition, common_conditions
-
-
-def make(
-    game: Game = Game(),
-    tick_skip: int = 15,
-    team_size: int = 1,
-    bots: list[Bot] | None = None,
-    terminal_conditions: List[TerminalCondition] = (
-        common_conditions.TimeoutCondition(1 * 60 * 60 / 15),
-        common_conditions.GoalScoredCondition(),
-    ),
-    reward_fn: RewardFunction = common_rewards.EventReward(
-        team_goal=1, team_concede=-1, touch=0.1, kick=0.1
-    ),
-    obs_builder: ObsBuilder = DefaultObs(),
-    action_parser: ActionParser = DefaultAction(),
-):
-    """
-    :param tick_skip: The amount of physics ticks your action will be repeated for
-    :param team_size: Players per team
-    :param terminal_conditions: List of terminal condition objects
-    :param reward_fn: Reward function object
-    :param obs_builder: Observation builder object
-    :param action_parser: Action parser object
-    :param state_setter: State Setter object
-    :return: Gym object
-    """
-
-    game.score = GameScore(time_limit=0, score_limit=0)
-
-    players_red = [
-        PlayerHandler(f"P{i}", common_values.TeamID.RED) for i in range(team_size)
-    ]
-    if bots is None:
-        players_blue = [
-            PlayerHandler(f"P{team_size + i}", common_values.TeamID.BLUE)
-            for i in range(team_size)
-        ]
-    else:
-        players_blue = [
-            PlayerHandler(f"P{team_size + i}", common_values.TeamID.BLUE, bot=bot)
-            for i, bot in enumerate(bots)
-        ]
-
-    players = players_red + players_blue
-
-    game.add_players(players)
-
-    match = Match(
-        game=game,
-        reward_function=reward_fn,
-        terminal_conditions=terminal_conditions,
-        obs_builder=obs_builder,
-        action_parser=action_parser,
-        team_size=team_size,
-        tick_skip=tick_skip,
-        bots=bots,
-    )
-
-    return Gym(match)
+from typing import List
+
+from ursinaxball import Game, common_values
+from ursinaxball.modules import Bot, GameScore, PlayerHandler
+
+from haxballgym.envs import Match
+from haxballgym.gym import Gym
+from haxballgym.utils.action_parsers import ActionParser, DefaultAction
+from haxballgym.utils.obs_builders import DefaultObs, ObsBuilder
+from haxballgym.utils.reward_functions import RewardFunction, common_rewards
+from haxballgym.utils.terminal_conditions import TerminalCondition, common_conditions
+from haxballgym.utils.state_setters import StateSetter, DefaultState
+
+
+def make(
+    game: Game = Game(),
+    tick_skip: int = 15,
+    team_size: int = 1,
+    bots: list[Bot] | None = None,
+    terminal_conditions: List[TerminalCondition] = (
+        common_conditions.TimeoutCondition(1 * 60 * 60 / 15),
+        common_conditions.GoalScoredCondition(),
+    ),
+    reward_fn: RewardFunction = common_rewards.EventReward(
+        team_goal=1, team_concede=-1, touch=0.1, kick=0.1
+    ),
+    obs_builder: ObsBuilder = DefaultObs(),
+    action_parser: ActionParser = DefaultAction(),
+    state_setter: StateSetter = DefaultState(),
+):
+    """
+    :param tick_skip: The amount of physics ticks your action will be repeated for
+    :param team_size: Players per team
+    :param terminal_conditions: List of terminal condition objects
+    :param reward_fn: Reward function object
+    :param obs_builder: Observation builder object
+    :param action_parser: Action parser object
+    :param state_setter: State Setter object
+    :return: Gym object
+    """
+
+    game.score = GameScore(time_limit=0, score_limit=0)
+
+    players_red = [
+        PlayerHandler(f"P{i}", common_values.TeamID.RED) for i in range(team_size)
+    ]
+    if bots is None:
+        players_blue = [
+            PlayerHandler(f"P{team_size + i}", common_values.TeamID.BLUE)
+            for i in range(team_size)
+        ]
+    else:
+        players_blue = [
+            PlayerHandler(f"P{team_size + i}", common_values.TeamID.BLUE, bot=bot)
+            for i, bot in enumerate(bots)
+        ]
+
+    players = players_red + players_blue
+
+    game.add_players(players)
+
+    match = Match(
+        game=game,
+        reward_function=reward_fn,
+        terminal_conditions=terminal_conditions,
+        obs_builder=obs_builder,
+        action_parser=action_parser,
+        state_setter=state_setter,
+        team_size=team_size,
+        tick_skip=tick_skip,
+        bots=bots,
+    )
+
+    return Gym(match)
```

### Comparing `haxballgym-0.5.6/haxballgym/utils/action_parsers/default_act.py` & `haxballgym-0.5.7/haxballgym/utils/action_parsers/action_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,38 @@
-from typing import List, Union
-
-import gym.spaces
-import numpy as np
-
-from haxballgym.utils.action_parsers import DiscreteAction
-from haxballgym.utils.common_values import NUM_ACTIONS
-from haxballgym.utils.gamestates import GameState
-
-
-class DefaultAction(DiscreteAction):
-    def __init__(self):
-        super().__init__()
-
-    def get_action_space(self) -> gym.spaces.Space:
-        return super().get_action_space()
-
-    def parse_actions(
-        self,
-        actions: Union[np.ndarray, List[np.ndarray], List[float]],
-        state: GameState,
-    ) -> np.ndarray:
-
-        if type(actions) != np.ndarray:
-            actions = np.asarray(actions)
-
-        if len(actions.shape) == 1:
-            actions = actions.reshape((-1, NUM_ACTIONS))
-        elif len(actions.shape) > 2:
-            raise ValueError("{} is not a valid action shape".format(actions.shape))
-
-        return super().parse_actions(actions, state)
+"""
+The action parser.
+"""
+
+from abc import ABC, abstractmethod
+from typing import Any
+
+import gym.spaces
+import numpy as np
+
+from haxballgym.utils.gamestates import GameState
+
+
+class ActionParser(ABC):
+    def __init__(self):
+        pass
+
+    @abstractmethod
+    def get_action_space(self) -> gym.spaces.Space:
+        """
+        Function that returns the action space type.
+        It will be called during the initialization of the environment.
+
+        :return: The type of the action space
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def parse_actions(self, actions: Any, state: GameState) -> np.ndarray:
+        """
+        Function that parses actions from the action space into the correct format.
+
+        :param actions: An object of actions, as passed to the `env.step` function.
+        :param state: The GameState object that was used to generate the actions.
+
+        :return: the parsed actions.
+        """
+        raise NotImplementedError
```

### Comparing `haxballgym-0.5.6/haxballgym/utils/action_parsers/discrete_act.py` & `haxballgym-0.5.7/haxballgym/utils/action_parsers/default_act.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-import gym.spaces
-import numpy as np
-
-from haxballgym.utils.action_parsers import ActionParser
-from haxballgym.utils.common_values import NUM_ACTIONS
-from haxballgym.utils.gamestates import GameState
-
-
-class DiscreteAction(ActionParser):
-    """
-    Simple discrete action space.
-    All the analog actions have 3 bins by default: -1, 0 and 1.
-    Mapping of the actions is as follows:
-    - Left/Right: 1 for right, 0 for nothing, -1 for left
-    - Up/Down: 1 for up, 0 for nothing, -1 for down
-    - Kick: 1 for kick, 0 for nothing
-    """
-
-    def __init__(self, n_bins=3):
-        super().__init__()
-        assert n_bins % 2 == 1, "n_bins must be an odd number"
-        self._n_bins = n_bins
-
-    def get_action_space(self) -> gym.spaces.Space:
-        return gym.spaces.MultiDiscrete([self._n_bins] * 2 + [2])
-
-    def parse_actions(self, actions: np.ndarray, state: GameState) -> np.ndarray:
-        actions = actions.reshape((-1, NUM_ACTIONS))
-
-        # map all ternary actions from {0, 1, 2} to {-1, 0, 1}.
-        actions[..., :2] = actions[..., :2] / (self._n_bins // 2) - 1
-        # map all binary actions from {0, 1} to {True, False}.
-        actions[..., 2] = actions[..., 2] == 1
-
-        return actions
+from typing import List, Union
+
+import gym.spaces
+import numpy as np
+
+from haxballgym.utils.action_parsers import DiscreteAction
+from haxballgym.utils.common_values import NUM_ACTIONS
+from haxballgym.utils.gamestates import GameState
+
+
+class DefaultAction(DiscreteAction):
+    def __init__(self):
+        super().__init__()
+
+    def get_action_space(self) -> gym.spaces.Space:
+        return super().get_action_space()
+
+    def parse_actions(
+        self,
+        actions: Union[np.ndarray, List[np.ndarray], List[float]],
+        state: GameState,
+    ) -> np.ndarray:
+
+        if type(actions) != np.ndarray:
+            actions = np.asarray(actions)
+
+        if len(actions.shape) == 1:
+            actions = actions.reshape((-1, NUM_ACTIONS))
+        elif len(actions.shape) > 2:
+            raise ValueError("{} is not a valid action shape".format(actions.shape))
+
+        return super().parse_actions(actions, state)
```

### Comparing `haxballgym-0.5.6/haxballgym/utils/gamestates/game_state.py` & `haxballgym-0.5.7/haxballgym/utils/gamestates/game_state.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""
-    Object to contain all relevant information about the game state.
-"""
-
-from typing import List, Optional
-
-from ursinaxball import Game
-from ursinaxball.modules import PlayerHandler
-from ursinaxball.objects.base import Disc
-
-
-class GameState(object):
-    def __init__(self, game_object: Game):
-        self.red_score: int = game_object.score.red
-        self.blue_score: int = game_object.score.blue
-
-        self.last_touch: Optional[int] = -1
-        self.last_touch_time: Optional[int] = -1
-
-        self.last_kick: Optional[int] = -1
-        self.last_kick_time: Optional[int] = -1
-
-        self.players: List[PlayerHandler] = game_object.players
-        self.ball: Disc = game_object.stadium_game.discs[0]
-
-    def update(self, game_object: Game):
-        self.red_score = game_object.score.red
-        self.blue_score = game_object.score.blue
-
-        self.players = game_object.players
-        self.ball = game_object.stadium_game.discs[0]
-
-        for player in self.players:
-            p_data = player.player_data
-
-            if p_data.last_touch_time > self.last_touch_time:
-                self.last_touch_time = p_data.last_touch_time
-                self.last_touch = player.id
-
-            if p_data.last_kick_time > self.last_kick_time:
-                self.last_kick_time = p_data.last_kick_time
-                self.last_kick = player.id
+"""
+    Object to contain all relevant information about the game state.
+"""
+
+from typing import List, Optional
+
+from ursinaxball import Game
+from ursinaxball.modules import PlayerHandler
+from ursinaxball.objects.base import Disc
+
+
+class GameState(object):
+    def __init__(self, game_object: Game):
+        self.red_score: int = game_object.score.red
+        self.blue_score: int = game_object.score.blue
+
+        self.last_touch: Optional[int] = -1
+        self.last_touch_time: Optional[int] = -1
+
+        self.last_kick: Optional[int] = -1
+        self.last_kick_time: Optional[int] = -1
+
+        self.players: List[PlayerHandler] = game_object.players
+        self.ball: Disc = game_object.stadium_game.discs[0]
+
+    def update(self, game_object: Game):
+        self.red_score = game_object.score.red
+        self.blue_score = game_object.score.blue
+
+        self.players = game_object.players
+        self.ball = game_object.stadium_game.discs[0]
+
+        for player in self.players:
+            p_data = player.player_data
+
+            if p_data.last_touch_time > self.last_touch_time:
+                self.last_touch_time = p_data.last_touch_time
+                self.last_touch = player.id
+
+            if p_data.last_kick_time > self.last_kick_time:
+                self.last_kick_time = p_data.last_kick_time
+                self.last_kick = player.id
```

### Comparing `haxballgym-0.5.6/haxballgym/utils/obs_builders/default_obs.py` & `haxballgym-0.5.7/haxballgym/utils/obs_builders/default_obs.py`

 * *Files identical despite different names*

### Comparing `haxballgym-0.5.6/haxballgym/utils/obs_builders/obs_builder.py` & `haxballgym-0.5.7/haxballgym/utils/obs_builders/obs_builder.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-"""
-The observation builder.
-"""
-
-from abc import ABC, abstractmethod
-from typing import Any
-
-import numpy as np
-from ursinaxball.modules import PlayerHandler
-
-from haxballgym.utils.gamestates import GameState
-
-
-class ObsBuilder(ABC):
-    def __init__(self):
-        pass
-
-    @abstractmethod
-    def reset(self, initial_state: GameState):
-        """
-        Function to be called each time the environment is reset. Note that this does not need to return anything,
-        the environment will call `build_obs` automatically after reset, so the initial observation for a policy will be
-        constructed in the same way as every other observation.
-
-        :param initial_state: The initial game state of the reset environment.
-        """
-        raise NotImplementedError
-
-    @abstractmethod
-    def build_obs(
-        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
-    ) -> Any:
-        """
-        Function to build observations for a policy. This is where all observations will be constructed every step and
-        every reset. This function is given a player argument, and it is expected that the observation returned by this
-        function will contain information from the perspective of that player. This function is called once for each
-        agent automatically at every step.
-
-        :param player: The player to build an observation for. The observation returned should be from the perspective of
-        this player.
-
-        :param state: The current state of the game.
-        :param previous_action: The action taken at the previous environment step.
-
-        :return: An observation for the player provided.
-        """
-        raise NotImplementedError
+"""
+The observation builder.
+"""
+
+from abc import ABC, abstractmethod
+from typing import Any
+
+import numpy as np
+from ursinaxball.modules import PlayerHandler
+
+from haxballgym.utils.gamestates import GameState
+
+
+class ObsBuilder(ABC):
+    def __init__(self):
+        pass
+
+    @abstractmethod
+    def reset(self, initial_state: GameState):
+        """
+        Function to be called each time the environment is reset. Note that this does not need to return anything,
+        the environment will call `build_obs` automatically after reset, so the initial observation for a policy will be
+        constructed in the same way as every other observation.
+
+        :param initial_state: The initial game state of the reset environment.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def build_obs(
+        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
+    ) -> Any:
+        """
+        Function to build observations for a policy. This is where all observations will be constructed every step and
+        every reset. This function is given a player argument, and it is expected that the observation returned by this
+        function will contain information from the perspective of that player. This function is called once for each
+        agent automatically at every step.
+
+        :param player: The player to build an observation for. The observation returned should be from the perspective of
+        this player.
+
+        :param state: The current state of the game.
+        :param previous_action: The action taken at the previous environment step.
+
+        :return: An observation for the player provided.
+        """
+        raise NotImplementedError
```

### Comparing `haxballgym-0.5.6/haxballgym/utils/reward_functions/common_rewards/misc_rewards.py` & `haxballgym-0.5.7/haxballgym/utils/reward_functions/common_rewards/misc_rewards.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-import numpy as np
-from ursinaxball.common_values import TeamID
-from ursinaxball.modules.player import PlayerHandler
-from ursinaxball.objects import Stadium
-
-from haxballgym.utils.gamestates import GameState
-from haxballgym.utils.reward_functions import RewardFunction
-
-
-class EventReward(RewardFunction):
-    def __init__(self, team_goal=0.0, team_concede=-0.0, touch=0.0, kick=0.0):
-        """
-        :param team_goal: reward for goal scored by player's team.
-        :param team_concede: reward for goal scored by opponents.
-        :param touch: reward for touching the ball.
-        :param kick: reward for kicking the ball.
-        """
-        super().__init__()
-        self.weights = np.array([team_goal, team_concede, touch, kick])
-
-        # Need to keep track of last registered value to detect changes
-        self.last_registered_values = {}
-
-    @staticmethod
-    def _extract_values(player: PlayerHandler, state: GameState):
-        if player.team == TeamID.RED:
-            team, opponent = state.red_score, state.blue_score
-        else:
-            team, opponent = state.blue_score, state.red_score
-
-        return np.array(
-            [
-                team,
-                opponent,
-                player.player_data.number_touch,
-                player.player_data.number_kick,
-            ]
-        )
-
-    def reset(self, initial_state: GameState, optional_data=None):
-        self.last_registered_values = {}
-        for player in initial_state.players:
-            self.last_registered_values[player.id] = self._extract_values(
-                player, initial_state
-            )
-
-    def get_reward(
-        self,
-        player: PlayerHandler,
-        state: GameState,
-        previous_action: np.ndarray,
-        optional_data=None,
-    ):
-        old_values = self.last_registered_values[player.id]
-        new_values = self._extract_values(player, state)
-
-        diff_values = new_values - old_values
-        diff_values[diff_values < 0] = 0  # We only care about increasing values
-
-        reward = np.dot(self.weights, diff_values)
-
-        self.last_registered_values[player.id] = new_values
-        return reward
-
-
-class VelocityReward(RewardFunction):
-    # Simple reward function to ensure the model is training.
-    def __init__(self, negative=False):
-        super().__init__()
-        self.negative = negative
-
-    def reset(self, initial_state: GameState):
-        pass
-
-    def get_reward(
-        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
-    ) -> float:
-        return np.linalg.norm(player.disc.velocity) / 10 * (1 - 2 * self.negative)
-
-
-class ConstantReward(RewardFunction):
-    def reset(self, initial_state: GameState):
-        pass
-
-    def get_reward(
-        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
-    ) -> float:
-        return 1
-
-
-class AlignBallGoal(RewardFunction):
-    def __init__(self, stadium: Stadium, defense=1.0, offense=1.0):
-        super().__init__()
-        self.defense = defense
-        self.defense_goal = [goal for goal in stadium.goals if goal.team == "red"][0]
-        self.offense = offense
-        self.offense_goal = [goal for goal in stadium.goals if goal.team == "blue"][0]
-
-    def reset(self, initial_state: GameState):
-        pass
-
-    def get_reward(
-        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
-    ) -> float:
-        ball = state.ball.position
-        pos = player.car_data.position
-        protecc = (self.defense_goal.points[0] + self.defense_goal.points[1]) / 2
-        attacc = (self.offense_goal.points[0] + self.offense_goal.points[1]) / 2
-        if player.team == TeamID.BLUE:
-            protecc, attacc = attacc, protecc
-
-        # Align player->ball and net->player vectors
-        cosine_similarity_def = np.dot(
-            ball - pos / np.linalg.norm(ball - pos),
-            pos - protecc / np.linalg.norm(pos - protecc),
-        )
-        defensive_reward = self.defense * cosine_similarity_def
-
-        # Align player->ball and player->net vectors
-        cosine_similarity_off = np.dot(
-            ball - pos / np.linalg.norm(ball - pos),
-            attacc - pos / np.linalg.norm(attacc - pos),
-        )
-        offensive_reward = self.offense * cosine_similarity_off
-
-        return defensive_reward + offensive_reward
+import numpy as np
+from ursinaxball.common_values import TeamID
+from ursinaxball.modules.player import PlayerHandler
+from ursinaxball.objects import Stadium
+
+from haxballgym.utils.gamestates import GameState
+from haxballgym.utils.reward_functions import RewardFunction
+
+
+class EventReward(RewardFunction):
+    def __init__(self, team_goal=0.0, team_concede=-0.0, touch=0.0, kick=0.0):
+        """
+        :param team_goal: reward for goal scored by player's team.
+        :param team_concede: reward for goal scored by opponents.
+        :param touch: reward for touching the ball.
+        :param kick: reward for kicking the ball.
+        """
+        super().__init__()
+        self.weights = np.array([team_goal, team_concede, touch, kick])
+
+        # Need to keep track of last registered value to detect changes
+        self.last_registered_values = {}
+
+    @staticmethod
+    def _extract_values(player: PlayerHandler, state: GameState):
+        if player.team == TeamID.RED:
+            team, opponent = state.red_score, state.blue_score
+        else:
+            team, opponent = state.blue_score, state.red_score
+
+        return np.array(
+            [
+                team,
+                opponent,
+                player.player_data.number_touch,
+                player.player_data.number_kick,
+            ]
+        )
+
+    def reset(self, initial_state: GameState, optional_data=None):
+        self.last_registered_values = {}
+        for player in initial_state.players:
+            self.last_registered_values[player.id] = self._extract_values(
+                player, initial_state
+            )
+
+    def get_reward(
+        self,
+        player: PlayerHandler,
+        state: GameState,
+        previous_action: np.ndarray,
+        optional_data=None,
+    ):
+        old_values = self.last_registered_values[player.id]
+        new_values = self._extract_values(player, state)
+
+        diff_values = new_values - old_values
+        diff_values[diff_values < 0] = 0  # We only care about increasing values
+
+        reward = np.dot(self.weights, diff_values)
+
+        self.last_registered_values[player.id] = new_values
+        return reward
+
+
+class VelocityReward(RewardFunction):
+    # Simple reward function to ensure the model is training.
+    def __init__(self, negative=False):
+        super().__init__()
+        self.negative = negative
+
+    def reset(self, initial_state: GameState):
+        pass
+
+    def get_reward(
+        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
+    ) -> float:
+        return np.linalg.norm(player.disc.velocity) / 10 * (1 - 2 * self.negative)
+
+
+class ConstantReward(RewardFunction):
+    def reset(self, initial_state: GameState):
+        pass
+
+    def get_reward(
+        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
+    ) -> float:
+        return 1
+
+
+class AlignBallGoal(RewardFunction):
+    def __init__(self, stadium: Stadium, defense=1.0, offense=1.0):
+        super().__init__()
+        self.defense = defense
+        self.defense_goal = [goal for goal in stadium.goals if goal.team == "red"][0]
+        self.offense = offense
+        self.offense_goal = [goal for goal in stadium.goals if goal.team == "blue"][0]
+
+    def reset(self, initial_state: GameState):
+        pass
+
+    def get_reward(
+        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
+    ) -> float:
+        ball = state.ball.position
+        pos = player.car_data.position
+        protecc = (self.defense_goal.points[0] + self.defense_goal.points[1]) / 2
+        attacc = (self.offense_goal.points[0] + self.offense_goal.points[1]) / 2
+        if player.team == TeamID.BLUE:
+            protecc, attacc = attacc, protecc
+
+        # Align player->ball and net->player vectors
+        cosine_similarity_def = np.dot(
+            ball - pos / np.linalg.norm(ball - pos),
+            pos - protecc / np.linalg.norm(pos - protecc),
+        )
+        defensive_reward = self.defense * cosine_similarity_def
+
+        # Align player->ball and player->net vectors
+        cosine_similarity_off = np.dot(
+            ball - pos / np.linalg.norm(ball - pos),
+            attacc - pos / np.linalg.norm(attacc - pos),
+        )
+        offensive_reward = self.offense * cosine_similarity_off
+
+        return defensive_reward + offensive_reward
```

### Comparing `haxballgym-0.5.6/haxballgym/utils/reward_functions/default_reward.py` & `haxballgym-0.5.7/haxballgym/utils/reward_functions/default_reward.py`

 * *Files identical despite different names*

### Comparing `haxballgym-0.5.6/haxballgym/utils/reward_functions/reward_function.py` & `haxballgym-0.5.7/haxballgym/utils/reward_functions/reward_function.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-"""
-The reward function.
-"""
-
-from abc import ABC, abstractmethod
-
-import numpy as np
-from ursinaxball.modules import PlayerHandler
-
-from haxballgym.utils.gamestates import GameState
-
-
-class RewardFunction(ABC):
-    @abstractmethod
-    def reset(self, initial_state: GameState):
-        """
-        Function to be called each time the environment is reset. This is meant to enable users to design stateful reward
-        functions that maintain information about the game throughout an episode to determine a reward.
-
-        :param initial_state: The initial state of the reset environment.
-        """
-        raise NotImplementedError
-
-    @abstractmethod
-    def get_reward(
-        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
-    ) -> float:
-        """
-        Function to compute the reward for a player. This function is given a player argument, and it is expected that
-        the reward returned by this function will be for that player.
-
-        :param player: Player to compute the reward for.
-        :param state: The current state of the game.
-        :param previous_action: The action taken at the previous environment step.
-
-        :return: A reward for the player provided.
-        """
-        raise NotImplementedError
-
-    def get_final_reward(
-        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
-    ) -> float:
-        """
-        Function to compute the reward for a player at the final step of an episode. This will be called only once, when
-        it is determined that the current state is a terminal one. This may be useful for sparse reward signals that only
-        produce a value at the final step of an environment. By default, the regular get_reward is used.
-
-        :param player: Player to compute the reward for.
-        :param state: The current state of the game.
-        :param previous_action: The action taken at the previous environment step.
-
-        :return: A reward for the player provided.
-        """
-        return self.get_reward(player, state, previous_action)
+"""
+The reward function.
+"""
+
+from abc import ABC, abstractmethod
+
+import numpy as np
+from ursinaxball.modules import PlayerHandler
+
+from haxballgym.utils.gamestates import GameState
+
+
+class RewardFunction(ABC):
+    @abstractmethod
+    def reset(self, initial_state: GameState):
+        """
+        Function to be called each time the environment is reset. This is meant to enable users to design stateful reward
+        functions that maintain information about the game throughout an episode to determine a reward.
+
+        :param initial_state: The initial state of the reset environment.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def get_reward(
+        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
+    ) -> float:
+        """
+        Function to compute the reward for a player. This function is given a player argument, and it is expected that
+        the reward returned by this function will be for that player.
+
+        :param player: Player to compute the reward for.
+        :param state: The current state of the game.
+        :param previous_action: The action taken at the previous environment step.
+
+        :return: A reward for the player provided.
+        """
+        raise NotImplementedError
+
+    def get_final_reward(
+        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
+    ) -> float:
+        """
+        Function to compute the reward for a player at the final step of an episode. This will be called only once, when
+        it is determined that the current state is a terminal one. This may be useful for sparse reward signals that only
+        produce a value at the final step of an environment. By default, the regular get_reward is used.
+
+        :param player: Player to compute the reward for.
+        :param state: The current state of the game.
+        :param previous_action: The action taken at the previous environment step.
+
+        :return: A reward for the player provided.
+        """
+        return self.get_reward(player, state, previous_action)
```

### Comparing `haxballgym-0.5.6/haxballgym/utils/reward_functions/velocity_reward.py` & `haxballgym-0.5.7/haxballgym/utils/reward_functions/velocity_reward.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-import numpy as np
-from ursinaxball.common_values import TeamID
-from ursinaxball.modules import PlayerHandler
-from ursinaxball.objects import Stadium
-
-from haxballgym.utils.gamestates import GameState
-from haxballgym.utils.reward_functions import RewardFunction
-
-
-class VelocityPlayerToBallReward(RewardFunction):
-    def __init__(self):
-        super().__init__()
-
-    def reset(self, initial_state: GameState):
-        pass
-
-    def get_reward(
-        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
-    ) -> float:
-        vel = np.copy(player.disc.velocity)
-        pos_diff = state.ball.position - player.disc.position
-        player_max_speed = (
-            player.disc.acceleration
-            * player.disc.damping
-            / (1 - player.disc.acceleration)
-        )
-
-        norm_pos_diff = pos_diff / np.linalg.norm(pos_diff)
-        vel /= player_max_speed
-        return float(np.dot(norm_pos_diff, vel))
-
-
-def position_diff_point_segment(
-    p: np.ndarray, v: np.ndarray, w: np.ndarray
-) -> np.ndarray:
-    """
-    Calculates the distance between a point and a segment
-    :param p: Point
-    :param v: Start of segment
-    :param w: End of segment
-    :return: Difference vector
-    """
-    return p - (v + (w - v) * np.dot(p - v, w - v) / np.dot(w - v, w - v))
-
-
-class VelocityBallToGoalReward(RewardFunction):
-    def __init__(self, stadium: Stadium, own_goal=False):
-        super().__init__()
-        self.own_goal = own_goal
-        self.red_goal = [goal for goal in stadium.goals if goal.team == "red"][0]
-        self.blue_goal = [goal for goal in stadium.goals if goal.team == "blue"][0]
-
-    def reset(self, initial_state: GameState):
-        pass
-
-    def get_reward(
-        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
-    ) -> float:
-        if (player.team == TeamID.RED and not self.own_goal) or (
-            player.team == TeamID.BLUE and self.own_goal
-        ):
-            objective = self.blue_goal
-        else:
-            objective = self.red_goal
-
-        vel = np.copy(state.ball.velocity)
-        pos_diff = -position_diff_point_segment(
-            state.ball.position, objective.points[0], objective.points[1]
-        )
-        player_max_speed = (
-            player.disc.acceleration
-            * player.disc.damping
-            / (1 - player.disc.acceleration)
-        )
-
-        norm_pos_diff = pos_diff / np.linalg.norm(pos_diff)
-        vel /= player_max_speed
-        return float(np.dot(norm_pos_diff, vel))
+import numpy as np
+from ursinaxball.common_values import TeamID
+from ursinaxball.modules import PlayerHandler
+from ursinaxball.objects import Stadium
+
+from haxballgym.utils.gamestates import GameState
+from haxballgym.utils.reward_functions import RewardFunction
+
+
+class VelocityPlayerToBallReward(RewardFunction):
+    def __init__(self):
+        super().__init__()
+
+    def reset(self, initial_state: GameState):
+        pass
+
+    def get_reward(
+        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
+    ) -> float:
+        vel = np.copy(player.disc.velocity)
+        pos_diff = state.ball.position - player.disc.position
+        player_max_speed = (
+            player.disc.acceleration
+            * player.disc.damping
+            / (1 - player.disc.acceleration)
+        )
+
+        norm_pos_diff = pos_diff / np.linalg.norm(pos_diff)
+        vel /= player_max_speed
+        return float(np.dot(norm_pos_diff, vel))
+
+
+def position_diff_point_segment(
+    p: np.ndarray, v: np.ndarray, w: np.ndarray
+) -> np.ndarray:
+    """
+    Calculates the distance between a point and a segment
+    :param p: Point
+    :param v: Start of segment
+    :param w: End of segment
+    :return: Difference vector
+    """
+    return p - (v + (w - v) * np.dot(p - v, w - v) / np.dot(w - v, w - v))
+
+
+class VelocityBallToGoalReward(RewardFunction):
+    def __init__(self, stadium: Stadium, own_goal=False):
+        super().__init__()
+        self.own_goal = own_goal
+        self.red_goal = [goal for goal in stadium.goals if goal.team == "red"][0]
+        self.blue_goal = [goal for goal in stadium.goals if goal.team == "blue"][0]
+
+    def reset(self, initial_state: GameState):
+        pass
+
+    def get_reward(
+        self, player: PlayerHandler, state: GameState, previous_action: np.ndarray
+    ) -> float:
+        if (player.team == TeamID.RED and not self.own_goal) or (
+            player.team == TeamID.BLUE and self.own_goal
+        ):
+            objective = self.blue_goal
+        else:
+            objective = self.red_goal
+
+        vel = np.copy(state.ball.velocity)
+        pos_diff = -position_diff_point_segment(
+            state.ball.position, objective.points[0], objective.points[1]
+        )
+        player_max_speed = (
+            player.disc.acceleration
+            * player.disc.damping
+            / (1 - player.disc.acceleration)
+        )
+
+        norm_pos_diff = pos_diff / np.linalg.norm(pos_diff)
+        vel /= player_max_speed
+        return float(np.dot(norm_pos_diff, vel))
```

### Comparing `haxballgym-0.5.6/haxballgym/utils/terminal_conditions/terminal_condition.py` & `haxballgym-0.5.7/haxballgym/utils/terminal_conditions/terminal_condition.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""
-A terminal condition.
-"""
-
-from abc import ABC, abstractmethod
-
-from haxballgym.utils.gamestates import GameState
-
-
-class TerminalCondition(ABC):
-    def __init__(self):
-        pass
-
-    @abstractmethod
-    def reset(self, initial_state: GameState):
-        """
-        Function to be called each time the environment is reset.
-
-        :param initial_state: The initial state of the reset environment.
-        """
-        raise NotImplementedError
-
-    @abstractmethod
-    def is_terminal(self, current_state: GameState) -> bool:
-        """
-        Function to determine if a game state is terminal. This will be called once per step, and must return either
-        `True` or `False` if the current episode should be terminated at this state.
-
-        :param current_state: The current state of the game.
-
-        :return: Bool representing whether the current state is a terminal one.
-        """
-        raise NotImplementedError
+"""
+A terminal condition.
+"""
+
+from abc import ABC, abstractmethod
+
+from haxballgym.utils.gamestates import GameState
+
+
+class TerminalCondition(ABC):
+    def __init__(self):
+        pass
+
+    @abstractmethod
+    def reset(self, initial_state: GameState):
+        """
+        Function to be called each time the environment is reset.
+
+        :param initial_state: The initial state of the reset environment.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def is_terminal(self, current_state: GameState) -> bool:
+        """
+        Function to determine if a game state is terminal. This will be called once per step, and must return either
+        `True` or `False` if the current episode should be terminated at this state.
+
+        :param current_state: The current state of the game.
+
+        :return: Bool representing whether the current state is a terminal one.
+        """
+        raise NotImplementedError
```

### Comparing `haxballgym-0.5.6/README.md` & `haxballgym-0.5.7/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# HaxBallGym
-
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-HaxBallGym is a Python package that can be used to treat the game [HaxBall](https://www.haxball.com) as though it were an [OpenAI Gym](https://gym.openai.com)-style environment for Reinforcement Learning projects.
-
-## Requirements
-
-- Python >= 3.10
-
-## Installation
-
-Install the library via pip:
-
-```bash
-pip install haxballgym
-```
-
-That's it! Run `example.py` to see if the installation was successful. The script assumes you have a recordings folder from where you run the script.
-
-## Recordings
-
-To watch recordings, go to my [HaxBall clone](https://wazarr94.github.io/) and load the recording file.
-
-## Discord
-
-[![Join our Discord server!](https://invidget.switchblade.xyz/TpKPeCe7y6)](https://discord.gg/TpKPeCe7y6)
+# HaxBallGym
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+HaxBallGym is a Python package that can be used to treat the game [HaxBall](https://www.haxball.com) as though it were an [OpenAI Gym](https://gym.openai.com)-style environment for Reinforcement Learning projects.
+
+## Requirements
+
+- Python >= 3.10
+
+## Installation
+
+Install the library via pip:
+
+```bash
+pip install haxballgym
+```
+
+That's it! Run `example.py` to see if the installation was successful. The script assumes you have a recordings folder from where you run the script.
+
+## Recordings
+
+To watch recordings, go to my [HaxBall clone](https://wazarr94.github.io/) and load the recording file.
+
+## Discord
+
+[![Join our Discord server!](https://invidget.switchblade.xyz/TpKPeCe7y6)](https://discord.gg/TpKPeCe7y6)
```

### Comparing `haxballgym-0.5.6/PKG-INFO` & `haxballgym-0.5.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: haxballgym
-Version: 0.5.6
+Version: 0.5.7
 Summary: HaxBallGym is a python package that can be used to treat the game HaxBall as though it were an OpenAI-style environment for Reinforcement Learning projects.
 Author: Wazarr
 Author-email: jeje_04@live.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: gym (==0.21.0)
+Requires-Dist: gym (>=0.26.2,<0.27.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: ursinaxball (==0.2.3)
 Description-Content-Type: text/markdown
 
 # HaxBallGym
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

