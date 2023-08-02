# Comparing `tmp/gymnasium_connect_four-1.2.7.tar.gz` & `tmp/gymnasium_connect_four-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnasium_connect_four-1.2.7.tar", last modified: Sun Jul 30 17:35:50 2023, max compression
+gzip compressed data, was "gymnasium_connect_four-1.2.8.tar", last modified: Wed Aug  2 19:17:18 2023, max compression
```

## Comparing `gymnasium_connect_four-1.2.7.tar` & `gymnasium_connect_four-1.2.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 17:35:50.079176 gymnasium_connect_four-1.2.7/
--rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.7/LICENSE
--rw-rw-rw-   0        0        0      251 2023-07-30 17:35:50.077672 gymnasium_connect_four-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    11454 2023-07-30 17:35:07.000000 gymnasium_connect_four-1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 17:35:50.052651 gymnasium_connect_four-1.2.7/connect_four_gymnasium/
--rw-rw-rw-   0        0        0     9241 2023-07-30 08:06:17.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/ConnectFourEnv.py
--rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 17:35:50.066160 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/
--rw-rw-rw-   0        0        0     4654 2023-07-30 16:49:29.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/AdultPlayer.py
--rw-rw-rw-   0        0        0     4378 2023-07-30 16:49:19.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/AdultSmarterPlayer.py
--rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/BabyPlayer.py
--rw-rw-rw-   0        0        0      649 2023-07-30 17:27:29.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/BabySmarterPlayer.py
--rw-rw-rw-   0        0        0     1920 2023-07-30 16:50:55.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ChildPlayer.py
--rw-rw-rw-   0        0        0     2248 2023-07-30 16:50:49.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ChildSmarterPlayer.py
--rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ConsolePlayer.py
--rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ModelPlayer.py
--rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/Player.py
--rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/SimulatePlayer.py
--rw-rw-rw-   0        0        0     3163 2023-07-30 16:49:44.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/TeenagerPlayer.py
--rw-rw-rw-   0        0        0     4378 2023-07-30 16:49:36.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
--rw-rw-rw-   0        0        0      496 2023-07-30 16:31:44.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 17:35:50.069668 gymnasium_connect_four-1.2.7/connect_four_gymnasium/tools/
--rw-rw-rw-   0        0        0     4082 2023-07-30 17:34:52.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/tools/EloLeaderboard.py
--rw-rw-rw-   0        0        0     4805 2023-07-30 16:46:39.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/tools/Update_bot_elo.py
--rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.7/connect_four_gymnasium/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 17:35:50.074673 gymnasium_connect_four-1.2.7/gymnasium_connect_four.egg-info/
--rw-rw-rw-   0        0        0      251 2023-07-30 17:35:49.000000 gymnasium_connect_four-1.2.7/gymnasium_connect_four.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1166 2023-07-30 17:35:50.000000 gymnasium_connect_four-1.2.7/gymnasium_connect_four.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 17:35:49.000000 gymnasium_connect_four-1.2.7/gymnasium_connect_four.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-30 17:35:49.000000 gymnasium_connect_four-1.2.7/gymnasium_connect_four.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-30 17:35:49.000000 gymnasium_connect_four-1.2.7/gymnasium_connect_four.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 17:35:50.079176 gymnasium_connect_four-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-07-30 17:35:43.000000 gymnasium_connect_four-1.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 17:35:50.077672 gymnasium_connect_four-1.2.7/test/
--rw-rw-rw-   0        0        0     4722 2023-07-29 17:17:01.000000 gymnasium_connect_four-1.2.7/test/test_no_opponant.py
--rw-rw-rw-   0        0        0    21564 2023-07-29 17:15:09.000000 gymnasium_connect_four-1.2.7/test/test_power_4_logic.py
--rw-rw-rw-   0        0        0     2372 2023-07-29 17:18:55.000000 gymnasium_connect_four-1.2.7/test/test_ppo_env.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:17:18.092477 gymnasium_connect_four-1.2.8/
+-rw-rw-rw-   0        0        0     1091 2023-07-23 15:11:33.000000 gymnasium_connect_four-1.2.8/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-08-02 19:17:18.090965 gymnasium_connect_four-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0    11454 2023-07-30 17:35:07.000000 gymnasium_connect_four-1.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 19:17:18.050360 gymnasium_connect_four-1.2.8/connect_four_gymnasium/
+-rw-rw-rw-   0        0        0     9269 2023-08-02 18:59:02.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/ConnectFourEnv.py
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:39:37.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:17:18.071167 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/
+-rw-rw-rw-   0        0        0     4654 2023-07-30 16:49:29.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/AdultPlayer.py
+-rw-rw-rw-   0        0        0     4378 2023-07-30 16:49:19.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/AdultSmarterPlayer.py
+-rw-rw-rw-   0        0        0      532 2023-07-29 14:17:34.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/BabyPlayer.py
+-rw-rw-rw-   0        0        0      649 2023-07-30 17:27:29.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/BabySmarterPlayer.py
+-rw-rw-rw-   0        0        0     1920 2023-07-30 16:50:55.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ChildPlayer.py
+-rw-rw-rw-   0        0        0     2248 2023-07-30 16:50:49.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ChildSmarterPlayer.py
+-rw-rw-rw-   0        0        0      652 2023-07-24 06:02:21.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ConsolePlayer.py
+-rw-rw-rw-   0        0        0      609 2023-07-29 09:51:35.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ModelPlayer.py
+-rw-rw-rw-   0        0        0      443 2023-07-24 06:00:39.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/Player.py
+-rw-rw-rw-   0        0        0      574 2023-07-25 13:46:25.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/SimulatePlayer.py
+-rw-rw-rw-   0        0        0     3163 2023-07-30 16:49:44.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/TeenagerPlayer.py
+-rw-rw-rw-   0        0        0     4378 2023-07-30 16:49:36.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/TeenagerSmarterPlayer.py
+-rw-rw-rw-   0        0        0      496 2023-07-30 16:31:44.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:17:18.075350 gymnasium_connect_four-1.2.8/connect_four_gymnasium/tools/
+-rw-rw-rw-   0        0        0     4056 2023-08-02 18:56:57.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/tools/EloLeaderboard.py
+-rw-rw-rw-   0        0        0     4805 2023-07-30 16:46:39.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/tools/Update_bot_elo.py
+-rw-rw-rw-   0        0        0       42 2023-07-23 16:29:17.000000 gymnasium_connect_four-1.2.8/connect_four_gymnasium/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:17:18.084500 gymnasium_connect_four-1.2.8/gymnasium_connect_four.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-08-02 19:17:17.000000 gymnasium_connect_four-1.2.8/gymnasium_connect_four.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1166 2023-08-02 19:17:17.000000 gymnasium_connect_four-1.2.8/gymnasium_connect_four.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 19:17:17.000000 gymnasium_connect_four-1.2.8/gymnasium_connect_four.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-08-02 19:17:17.000000 gymnasium_connect_four-1.2.8/gymnasium_connect_four.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-08-02 19:17:17.000000 gymnasium_connect_four-1.2.8/gymnasium_connect_four.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 19:17:18.092477 gymnasium_connect_four-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-08-02 19:17:08.000000 gymnasium_connect_four-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 19:17:18.089966 gymnasium_connect_four-1.2.8/test/
+-rw-rw-rw-   0        0        0     4722 2023-07-29 17:17:01.000000 gymnasium_connect_four-1.2.8/test/test_no_opponant.py
+-rw-rw-rw-   0        0        0    21564 2023-08-02 19:14:09.000000 gymnasium_connect_four-1.2.8/test/test_power_4_logic.py
+-rw-rw-rw-   0        0        0     2372 2023-07-29 17:18:55.000000 gymnasium_connect_four-1.2.8/test/test_ppo_env.py
```

### Comparing `gymnasium_connect_four-1.2.7/LICENSE` & `gymnasium_connect_four-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/README.md` & `gymnasium_connect_four-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/connect_four_gymnasium/ConnectFourEnv.py` & `gymnasium_connect_four-1.2.8/connect_four_gymnasium/ConnectFourEnv.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 
     def __init__(self, opponent=None, render_mode=None, first_player=None):
         self._opponent = opponent  # Define the opponent
         # Define the action and observation spaces
         self.action_space = spaces.Discrete(self.COLUMNS_COUNT)
 
         # 1 is you, -1 is the opponent
-        self.observation_space = spaces.Box(low=-1, high=1, shape=(self.ROWS_COUNT, self.COLUMNS_COUNT), dtype=np.int32)
+        self.observation_space = spaces.Box(low=-1, high=1, shape=(self.ROWS_COUNT, self.COLUMNS_COUNT), dtype=np.int8)
 
         # Check if the render mode is valid
         assert render_mode is None or render_mode in self.metadata["render_modes"]
         assert first_player is None or first_player in [1, -1]
         self.render_mode = render_mode
         self.last_render_time = None
         self.window = None
         self.first_player = first_player
 
     def reset(self, seed=None, options=None):
         super().reset(seed=seed)
-        self.board = np.zeros((self.ROWS_COUNT, self.COLUMNS_COUNT))
+        self.board = np.zeros((self.ROWS_COUNT, self.COLUMNS_COUNT), dtype=np.int8)
         self._render_for_human()
 
         if self.first_player is None:
             self.next_player_to_play = np.random.choice([1, -1])
         else:
             self.next_player_to_play = self.first_player
 
@@ -119,18 +119,19 @@
         return newBoard, result, IsFinish, isTruncated, newself
 
     def step(self, action, play_opponent=True):
         action = action.item() if isinstance(action, np.ndarray) else action
 
         result, is_finish = self._play_action(action, 1)
 
-        if is_finish:
+        self.switch_player()
+
+        if is_finish:            
             return self.board, result, True, False, {}
 
-        self.switch_player()
 
         if  play_opponent and self._opponent is not None:
             opponent_action = self._opponent.play(self.board)
             opponent_result = self.step(opponent_action, play_opponent=False)
             return self.board,-1* opponent_result[1], opponent_result[2], opponent_result[3], opponent_result[4]
             
         return self.board, 0, False, False, {}
```

### Comparing `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/AdultPlayer.py` & `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/AdultPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/AdultSmarterPlayer.py` & `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/AdultSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/BabyPlayer.py` & `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/BabyPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/BabySmarterPlayer.py` & `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/BabySmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ChildPlayer.py` & `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ChildPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ChildSmarterPlayer.py` & `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ChildSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ConsolePlayer.py` & `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ConsolePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/ModelPlayer.py` & `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/ModelPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/SimulatePlayer.py` & `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/SimulatePlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/TeenagerPlayer.py` & `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/TeenagerPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/connect_four_gymnasium/players/TeenagerSmarterPlayer.py` & `gymnasium_connect_four-1.2.8/connect_four_gymnasium/players/TeenagerSmarterPlayer.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/connect_four_gymnasium/tools/EloLeaderboard.py` & `gymnasium_connect_four-1.2.8/connect_four_gymnasium/tools/EloLeaderboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
                 actualElo = self.update_elo(actualElo, opponent_elo, player_won, k_factor, draw)
                 gamePlayed += 1
 
         return actualElo
 
     def get_elo(self, player, num_matches=100):
         actualElo = player.getElo() if player.getElo() is not None else 1400
-        actualElo = 1400
         return self.play_rounds(player, actualElo, num_matches)
 
     def get_scores(self, player, opponents):
         envs = [ConnectFourEnv(opponent=opponent) for opponent in opponents]
         obs_list = [obs for obs, _ in [env.reset() for env in envs]]
         scores = [0] * len(opponents)
         remaining_indices = list(range(len(opponents)))
```

### Comparing `gymnasium_connect_four-1.2.7/connect_four_gymnasium/tools/Update_bot_elo.py` & `gymnasium_connect_four-1.2.8/connect_four_gymnasium/tools/Update_bot_elo.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/gymnasium_connect_four.egg-info/SOURCES.txt` & `gymnasium_connect_four-1.2.8/gymnasium_connect_four.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/setup.py` & `gymnasium_connect_four-1.2.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='gymnasium_connect_four',
-    version='1.2.7',
+    version='1.2.8',
     description='A connect 4 (connect four) environment for OpenAI Gym and Gymnasium',
     author='Lucas Bertola',
     url='https://github.com/lucasBertola/Connect-4-env',  
     # author_email='your.email@example.com',
     packages=find_packages(),
     install_requires=[
         'pygame==2.1.3',
```

### Comparing `gymnasium_connect_four-1.2.7/test/test_no_opponant.py` & `gymnasium_connect_four-1.2.8/test/test_no_opponant.py`

 * *Files identical despite different names*

### Comparing `gymnasium_connect_four-1.2.7/test/test_power_4_logic.py` & `gymnasium_connect_four-1.2.8/test/test_power_4_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,17 +153,17 @@
         [-1, -1, -1, 0, 0, 0, 0]
     ])
     
     expected_model_view = np.array([
         [ 0,  0, 0, 0, 0, 0, 0],
         [ 0,  0, 0, 0, 0, 0, 0],
         [ 0,  0, 0, 0, 0, 0, 0],
-        [ 0, -1, 0, 0, 0, 0, 0],
-        [-1, -1, 0, 0, 0, 0, 0],
-        [ 1,  1, 1, 1, 0, 0, 0]
+        [ 0,  1, 0, 0, 0, 0, 0],
+        [ 1,  1, 0, 0, 0, 0, 0],
+        [-1, -1,-1,-1, 0, 0, 0]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
 def test_place_a_simple_game_vertical_win():
     simulatePlayer = SimulatePlayer()
@@ -262,20 +262,20 @@
     board, rewards, dones, truncated, info = env.step(nextAction)
 
     assert rewards == 1, f"Expected reward: 1 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == True, f"Expected dones: True but got {dones}"
         
     expected_model_view = np.array([
-        [0, 0, 0,  0, 0,  0,  0],
-        [0, 0, 0,  0, 0,  0,  0],
-        [0, 1, 0,  0, 0,  0,  0],
-        [0, 1, 0,  0, 0,  0,  0],
-        [0, 1, 0,  0, 0,  0,  0],
-        [0, 1, 0, -1, 0, -1, -1]
+        [0,  0, 0, 0, 0, 0, 0],
+        [0,  0, 0, 0, 0, 0, 0],
+        [0, -1, 0, 0, 0, 0, 0],
+        [0, -1, 0, 0, 0, 0, 0],
+        [0, -1, 0, 0, 0, 0, 0],
+        [0, -1, 0, 1, 0, 1, 1]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
 
 def test_place_a_simple_game_updiagonal_win():
@@ -433,20 +433,20 @@
     board, rewards, dones, truncated, info = env.step(nextAction)
 
     assert rewards == 1, f"Expected reward: 1 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == True, f"Expected dones: True but got {dones}"
     
     expected_model_view = np.array([
-        [0,  0,  0,  0, 0, 0, 0],
-        [0,  0,  0,  0, 0, 0, 0],
-        [0,  0,  1,  1, 0, 0, 0],
-        [0,  0,  1, -1, 0, 0, 0],
-        [0,  1, -1, -1, 0, 0, 0],
-        [1, -1, -1,  1, 0, 0, 0]
+        [ 0,  0,  0,  0, 0, 0, 0],
+        [ 0,  0,  0,  0, 0, 0, 0],
+        [ 0,  0, -1, -1, 0, 0, 0],
+        [ 0,  0, -1,  1, 0, 0, 0],
+        [ 0, -1,  1,  1, 0, 0, 0],
+        [-1,  1,  1, -1, 0, 0, 0]
     ])
     
     assert np.array_equal(simulatePlayer.lastBoardView, expected_opponant_view), f"expected_opponant_view:\n{expected_opponant_view}\nbut got:\n{simulatePlayer.lastBoardView}"
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"   
 
 def test_place_a_simple_game_downdiagonal_win():
     simulatePlayer = SimulatePlayer()
@@ -473,20 +473,20 @@
     simulatePlayer.set_next_move(1)
     board, rewards, dones, truncated, info = env.step(nextAction)
 
     nextAction = 2
     board, rewards, dones, truncated, info = env.step(nextAction)
 
     expected_model_view = np.array([
-        [0,  0,  0,  0,  0, 0, 0],
-        [0,  0,  0,  0,  0, 0, 0],
-        [0,  0,  1,  0,  0, 0, 0],
-        [0,  0,  1,  1,  0, 0, 0],
-        [0,  0, -1, -1,  1, 0, 0],
-        [0, -1,  1, -1, -1, 1, 0]
+        [0,  0,  0,  0,  0,  0, 0],
+        [0,  0,  0,  0,  0,  0, 0],
+        [0,  0, -1,  0,  0,  0, 0],
+        [0,  0, -1, -1,  0,  0, 0],
+        [0,  0,  1,  1, -1,  0, 0],
+        [0,  1, -1,  1,  1, -1, 0]
     ])
 
     assert np.array_equal(board, expected_model_view), f"Expected board:\n{expected_model_view}\nbut got:\n{board}"
 
     assert rewards == 1, f"Expected reward: 1 but got {rewards}"
     assert truncated == False, f"Expected truncated: False but got {truncated}"
     assert dones == True, f"Expected dones: True but got {dones}"
```

### Comparing `gymnasium_connect_four-1.2.7/test/test_ppo_env.py` & `gymnasium_connect_four-1.2.8/test/test_ppo_env.py`

 * *Files identical despite different names*

