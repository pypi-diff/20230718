# Comparing `tmp/pymahjong-1.0.2-cp39-cp39-win_amd64.whl.zip` & `tmp/pymahjong-1.0.3-cp39-cp39-manylinux_2_34_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,16 @@
-Zip file size: 288463 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat   631296 b- defN 22-Apr-07 11:15 MahjongPyWrapper.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      206 b- defN 22-Mar-31 10:04 pymahjong/__init__.py
--rw-rw-rw-  2.0 fat     5584 b- defN 22-Mar-31 10:05 pymahjong/base_modules.py
--rw-rw-rw-  2.0 fat    17169 b- defN 22-Mar-31 10:05 pymahjong/env_pymahjong.py
--rw-rw-rw-  2.0 fat     9740 b- defN 22-Mar-31 10:05 pymahjong/models.py
--rw-rw-rw-  2.0 fat    30995 b- defN 22-Mar-31 10:04 pymahjong/tenhou_paipu_check.py
--rw-rw-rw-  2.0 fat     3064 b- defN 22-Mar-31 10:05 pymahjong/test.py
--rw-rw-rw-  2.0 fat     2910 b- defN 22-Apr-07 11:15 pymahjong-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 22-Apr-07 11:15 pymahjong-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 22-Apr-07 11:15 pymahjong-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      883 b- defN 22-Apr-07 11:15 pymahjong-1.0.2.dist-info/RECORD
-11 files, 701957 bytes uncompressed, 286985 bytes compressed:  59.1%
+Zip file size: 362326 bytes, number of entries: 14
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-18 09:08 pymahjong/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-18 09:08 pymahjong-1.0.3.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-18 09:08 pymahjong.libs/
+-rwxr-xr-x  2.0 unx   822744 b- defN 23-Jul-18 09:08 MahjongPyWrapper.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     9529 b- defN 23-Jul-18 09:08 pymahjong/models.py
+-rw-r--r--  2.0 unx    16794 b- defN 23-Jul-18 09:08 pymahjong/env_pymahjong.py
+-rw-r--r--  2.0 unx     5421 b- defN 23-Jul-18 09:08 pymahjong/base_modules.py
+-rw-r--r--  2.0 unx     2990 b- defN 23-Jul-18 09:08 pymahjong/test.py
+-rw-r--r--  2.0 unx    31096 b- defN 23-Jul-18 09:08 pymahjong/tenhou_paipu_check.py
+-rw-r--r--  2.0 unx      200 b- defN 23-Jul-18 09:08 pymahjong/__init__.py
+-rw-r--r--  2.0 unx     2540 b- defN 23-Jul-18 09:08 pymahjong-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      112 b- defN 23-Jul-18 09:08 pymahjong-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-18 09:08 pymahjong-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      906 b- defN 23-Jul-18 09:08 pymahjong-1.0.3.dist-info/RECORD
+14 files, 892342 bytes uncompressed, 360494 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -1,34 +1,43 @@
-Filename: MahjongPyWrapper.cp39-win_amd64.pyd
+Filename: pymahjong/
 Comment: 
 
-Filename: pymahjong/__init__.py
+Filename: pymahjong-1.0.3.dist-info/
 Comment: 
 
-Filename: pymahjong/base_modules.py
+Filename: pymahjong.libs/
 Comment: 
 
-Filename: pymahjong/env_pymahjong.py
+Filename: MahjongPyWrapper.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
 Filename: pymahjong/models.py
 Comment: 
 
-Filename: pymahjong/tenhou_paipu_check.py
+Filename: pymahjong/env_pymahjong.py
+Comment: 
+
+Filename: pymahjong/base_modules.py
 Comment: 
 
 Filename: pymahjong/test.py
 Comment: 
 
-Filename: pymahjong-1.0.2.dist-info/METADATA
+Filename: pymahjong/tenhou_paipu_check.py
+Comment: 
+
+Filename: pymahjong/__init__.py
+Comment: 
+
+Filename: pymahjong-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: pymahjong-1.0.2.dist-info/WHEEL
+Filename: pymahjong-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: pymahjong-1.0.2.dist-info/top_level.txt
+Filename: pymahjong-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pymahjong-1.0.2.dist-info/RECORD
+Filename: pymahjong-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## pymahjong/__init__.py

 * *Ordering differences only*

```diff
@@ -1,6 +1,6 @@
-from .env_pymahjong import MahjongEnv, SingleAgentMahjongEnv
-from .test import test, test_with_pretrained
-from .tenhou_paipu_check import paipu_replay, paipu_replay_1
-from MahjongPyWrapper import *
-
-
+from .env_pymahjong import MahjongEnv, SingleAgentMahjongEnv
+from .test import test, test_with_pretrained
+from .tenhou_paipu_check import paipu_replay, paipu_replay_1
+from MahjongPyWrapper import *
+
+
```

## pymahjong/base_modules.py

 * *Ordering differences only*

```diff
@@ -1,163 +1,163 @@
-import torch
-import torch.nn as nn
-import numpy as np
-import torch.nn.functional as F
-import torch.distributions as dis
-import warnings
-
-
-class MinusOneModule(nn.Module):
-    def __init__(self):
-        super(MinusOneModule, self).__init__()
-
-    def forward(self, x):
-        return x - 1
-
-
-class MahjongNet(nn.Module):
-    def __init__(self, n_channels):
-        super(MahjongNet, self).__init__()
-
-        self.n_channels = n_channels
-
-        cnn_list = nn.ModuleList()
-        cnn_list.append(nn.Conv1d(n_channels, 64, 3, 1, 1))
-        cnn_list.append(nn.Conv1d(64, 64, 3, 1, 1))
-        cnn_list.append(nn.ReLU())
-        cnn_list.append(nn.Conv1d(64, 64, 3, 1, 1))
-        cnn_list.append(nn.ReLU())
-        cnn_list.append(nn.Conv1d(64, 32, 3, 1, 1))
-        cnn_list.append(nn.ReLU())
-        cnn_list.append(nn.Flatten())
-
-        self.cnn = nn.Sequential(*cnn_list)
-        # 1088
-
-        self.phi_size = 1088
-
-    def forward(self, x):
-        # Shape of x: [batch_size x n_channels x 34]
-
-        phi = self.cnn(x)
-
-        return phi
-
-
-def make_cnn(resolution, n_channels):
-    if resolution == "10x10":
-        # -------- MinAtar ---------
-        cnn_module_list = nn.ModuleList()
-        cnn_module_list.append(nn.Conv2d(n_channels, 16, 3, 1, 0))
-        cnn_module_list.append(nn.ReLU())
-        cnn_module_list.append(nn.Conv2d(16, 32, 3, 1, 0))
-        cnn_module_list.append(nn.ReLU())
-        cnn_module_list.append(nn.Conv2d(32, 128, 4, 2, 0))
-        cnn_module_list.append(nn.ReLU())
-        cnn_module_list.append(nn.Conv2d(128, 256, 2, 1, 0))
-        cnn_module_list.append(nn.ReLU())
-        cnn_module_list.append(nn.Flatten())
-        phi_size = 256
-
-    elif resolution == "34":
-        # -------- for Mahjong ---------
-        mahjong_net = MahjongNet(n_channels)
-        phi_size = mahjong_net.phi_size
-        return mahjong_net, phi_size
-
-    return nn.Sequential(*cnn_module_list), phi_size
-
-
-class DiscreteActionQNetwork(nn.Module):
-    def __init__(self, input_size, output_size, hidden_layers=None, dueling=False, act_fn=nn.ReLU):
-        super(DiscreteActionQNetwork, self).__init__()
-
-        if hidden_layers is None:
-            hidden_layers = [256, 256]
-        self.input_size = input_size
-        self.output_size = output_size
-        self.hidden_layers = hidden_layers
-        self.dueling = dueling
-
-        self.network_modules = nn.ModuleList()
-
-        last_layer_size = input_size
-        for layer_size in hidden_layers:
-            self.network_modules.append(nn.Linear(last_layer_size, layer_size))
-            self.network_modules.append(act_fn())
-            last_layer_size = layer_size
-
-        if not dueling:
-            self.network_modules.append(nn.Linear(last_layer_size, output_size))
-        else:
-            self.value_layer = nn.Linear(last_layer_size, 1)
-            self.advantage_layer = nn.Linear(last_layer_size, output_size)
-
-        self.main_network = nn.Sequential(*self.network_modules)
-
-    def forward(self, x):
-
-        if not self.dueling:
-            q = self.main_network(x)
-        else:
-            h = self.main_network(x)
-            v = self.value_layer(h).repeat_interleave(self.output_size, dim=-1)
-            q0 = self.advantage_layer(h)
-            a = q0 - torch.mean(q0, dim=-1, keepdim=True).repeat_interleave(self.output_size, dim=-1)
-            q = v + a
-
-        return q
-
-    def get_log_prob(self, x, q_target):
-
-        return - 0.5 * (self.forward(x) - q_target).pow(2)
-
-
-class DiscreteActionPolicyNetwork(nn.Module):
-    def __init__(self, input_size, output_size, hidden_layers=None, act_fn=nn.ReLU, logit_clip=None, device='cpu'):
-        super(DiscreteActionPolicyNetwork, self).__init__()
-
-        if logit_clip is None:
-            logit_clip = [-np.inf, np.inf]
-        if hidden_layers is None:
-            hidden_layers = [256, 256]
-        self.input_size = input_size
-        self.output_size = output_size
-        self.hidden_layers = hidden_layers
-
-        self.device = device
-        self.network_modules = nn.ModuleList()
-
-        last_layer_size = input_size
-        for layer_size in hidden_layers:
-            self.network_modules.append(nn.Linear(last_layer_size, layer_size))
-            self.network_modules.append(act_fn())
-            last_layer_size = layer_size
-
-        self.network_modules.append(nn.Linear(last_layer_size, output_size))
-
-        self.main_network = nn.Sequential(*self.network_modules)
-
-        self.logit_clip = logit_clip
-
-    def forward(self, x):
-        logit_pi = self.main_network(x).clamp(self.logit_clip[0], self.logit_clip[1])
-
-        return logit_pi
-
-    def sample_action(self, x, action_mask=None, greedy=False):
-
-        pi = F.softmax(self.forward(x).clamp(self.logit_clip[0], self.logit_clip[1]), dim=-1)
-        pi_np = (pi.cpu().detach() * action_mask).numpy()
-        if greedy:
-            if np.any(pi_np > 0):
-                a = np.argmax(pi_np, axis=-1)
-            else:
-                a = np.random.choice(action_mask.shape[-1], 1, p=action_mask.numpy().reshape([-1]) / action_mask.numpy().sum())
-                # warnings.warn("No preferred action, select action {}".format(a[0]))
-        else:
-            size_a = pi_np.shape[-1]
-            a = np.zeros_like(pi_np[:, 0], dtype=np.int)
-            for i in range(pi_np.shape[0]):
-                a[i] = np.random.choice(size_a, p=pi_np[i, :] / pi_np[i, :].sum())
-        return a
-
+import torch
+import torch.nn as nn
+import numpy as np
+import torch.nn.functional as F
+import torch.distributions as dis
+import warnings
+
+
+class MinusOneModule(nn.Module):
+    def __init__(self):
+        super(MinusOneModule, self).__init__()
+
+    def forward(self, x):
+        return x - 1
+
+
+class MahjongNet(nn.Module):
+    def __init__(self, n_channels):
+        super(MahjongNet, self).__init__()
+
+        self.n_channels = n_channels
+
+        cnn_list = nn.ModuleList()
+        cnn_list.append(nn.Conv1d(n_channels, 64, 3, 1, 1))
+        cnn_list.append(nn.Conv1d(64, 64, 3, 1, 1))
+        cnn_list.append(nn.ReLU())
+        cnn_list.append(nn.Conv1d(64, 64, 3, 1, 1))
+        cnn_list.append(nn.ReLU())
+        cnn_list.append(nn.Conv1d(64, 32, 3, 1, 1))
+        cnn_list.append(nn.ReLU())
+        cnn_list.append(nn.Flatten())
+
+        self.cnn = nn.Sequential(*cnn_list)
+        # 1088
+
+        self.phi_size = 1088
+
+    def forward(self, x):
+        # Shape of x: [batch_size x n_channels x 34]
+
+        phi = self.cnn(x)
+
+        return phi
+
+
+def make_cnn(resolution, n_channels):
+    if resolution == "10x10":
+        # -------- MinAtar ---------
+        cnn_module_list = nn.ModuleList()
+        cnn_module_list.append(nn.Conv2d(n_channels, 16, 3, 1, 0))
+        cnn_module_list.append(nn.ReLU())
+        cnn_module_list.append(nn.Conv2d(16, 32, 3, 1, 0))
+        cnn_module_list.append(nn.ReLU())
+        cnn_module_list.append(nn.Conv2d(32, 128, 4, 2, 0))
+        cnn_module_list.append(nn.ReLU())
+        cnn_module_list.append(nn.Conv2d(128, 256, 2, 1, 0))
+        cnn_module_list.append(nn.ReLU())
+        cnn_module_list.append(nn.Flatten())
+        phi_size = 256
+
+    elif resolution == "34":
+        # -------- for Mahjong ---------
+        mahjong_net = MahjongNet(n_channels)
+        phi_size = mahjong_net.phi_size
+        return mahjong_net, phi_size
+
+    return nn.Sequential(*cnn_module_list), phi_size
+
+
+class DiscreteActionQNetwork(nn.Module):
+    def __init__(self, input_size, output_size, hidden_layers=None, dueling=False, act_fn=nn.ReLU):
+        super(DiscreteActionQNetwork, self).__init__()
+
+        if hidden_layers is None:
+            hidden_layers = [256, 256]
+        self.input_size = input_size
+        self.output_size = output_size
+        self.hidden_layers = hidden_layers
+        self.dueling = dueling
+
+        self.network_modules = nn.ModuleList()
+
+        last_layer_size = input_size
+        for layer_size in hidden_layers:
+            self.network_modules.append(nn.Linear(last_layer_size, layer_size))
+            self.network_modules.append(act_fn())
+            last_layer_size = layer_size
+
+        if not dueling:
+            self.network_modules.append(nn.Linear(last_layer_size, output_size))
+        else:
+            self.value_layer = nn.Linear(last_layer_size, 1)
+            self.advantage_layer = nn.Linear(last_layer_size, output_size)
+
+        self.main_network = nn.Sequential(*self.network_modules)
+
+    def forward(self, x):
+
+        if not self.dueling:
+            q = self.main_network(x)
+        else:
+            h = self.main_network(x)
+            v = self.value_layer(h).repeat_interleave(self.output_size, dim=-1)
+            q0 = self.advantage_layer(h)
+            a = q0 - torch.mean(q0, dim=-1, keepdim=True).repeat_interleave(self.output_size, dim=-1)
+            q = v + a
+
+        return q
+
+    def get_log_prob(self, x, q_target):
+
+        return - 0.5 * (self.forward(x) - q_target).pow(2)
+
+
+class DiscreteActionPolicyNetwork(nn.Module):
+    def __init__(self, input_size, output_size, hidden_layers=None, act_fn=nn.ReLU, logit_clip=None, device='cpu'):
+        super(DiscreteActionPolicyNetwork, self).__init__()
+
+        if logit_clip is None:
+            logit_clip = [-np.inf, np.inf]
+        if hidden_layers is None:
+            hidden_layers = [256, 256]
+        self.input_size = input_size
+        self.output_size = output_size
+        self.hidden_layers = hidden_layers
+
+        self.device = device
+        self.network_modules = nn.ModuleList()
+
+        last_layer_size = input_size
+        for layer_size in hidden_layers:
+            self.network_modules.append(nn.Linear(last_layer_size, layer_size))
+            self.network_modules.append(act_fn())
+            last_layer_size = layer_size
+
+        self.network_modules.append(nn.Linear(last_layer_size, output_size))
+
+        self.main_network = nn.Sequential(*self.network_modules)
+
+        self.logit_clip = logit_clip
+
+    def forward(self, x):
+        logit_pi = self.main_network(x).clamp(self.logit_clip[0], self.logit_clip[1])
+
+        return logit_pi
+
+    def sample_action(self, x, action_mask=None, greedy=False):
+
+        pi = F.softmax(self.forward(x).clamp(self.logit_clip[0], self.logit_clip[1]), dim=-1)
+        pi_np = (pi.cpu().detach() * action_mask).numpy()
+        if greedy:
+            if np.any(pi_np > 0):
+                a = np.argmax(pi_np, axis=-1)
+            else:
+                a = np.random.choice(action_mask.shape[-1], 1, p=action_mask.numpy().reshape([-1]) / action_mask.numpy().sum())
+                # warnings.warn("No preferred action, select action {}".format(a[0]))
+        else:
+            size_a = pi_np.shape[-1]
+            a = np.zeros_like(pi_np[:, 0], dtype=np.int)
+            for i in range(pi_np.shape[0]):
+                a[i] = np.random.choice(size_a, p=pi_np[i, :] / pi_np[i, :].sum())
+        return a
+
```

## pymahjong/env_pymahjong.py

```diff
@@ -1,411 +1,411 @@
-import gym
-import numpy as np
-import warnings
-from gym.spaces import Discrete, Box
-import MahjongPyWrapper as pm
-
-np.set_printoptions(threshold=np.inf)
-
-
-class MahjongEnv(gym.Env):
-
-    PLAYER_OBS_DIM = 93
-    ORACLE_OBS_DIM = 18
-    ACTION_DIM = 47
-    MAHJONG_TILE_TYPES = 34
-    INIT_POINTS = 25000
-
-    # ACTION INDICES
-    CHILEFT = 34
-    CHIMIDDLE = 35
-    CHIRIGHT = 36
-    PON = 37
-    ANKAN = 38
-    MINKAN = 39
-    KAKAN = 40
-
-    RIICHI = 41
-    RON = 42
-    TSUMO = 43
-    PUSH = 44
-
-    PASS_RESPONSE = 45
-    PASS_RIICHI = 46
-
-    # corresponding to self.t.get_phase()
-    Phases = ("P1_ACTION", "P2_ACTION", "P3_ACTION", "P4_ACTION", "P1_RESPONSE", "P2_RESPONSE", "P3_RESPONSE",
-              "P4_RESPONSE", "P1_抢杠RESPONSE", "P2_抢杠RESPONSE", "P3_抢杠RESPONSE", "P4_抢杠RESPONSE",
-              "P1_抢暗杠RESPONSE", "P2_抢暗杠RESPONSE", " P3_抢暗杠RESPONSE", " P4_抢暗杠RESPONSE", "GAME_OVER",
-              "P1_DRAW, P2_DRAW, P3_DRAW, P4_DRAW")
-
-    # pymahjhong.BaseAction
-    ACTION_TYPES = [pm.BaseAction.Play] * MAHJONG_TILE_TYPES + [pm.BaseAction.Chi] * 3 + [pm.BaseAction.Pon] \
-                   + [pm.BaseAction.AnKan] + [pm.BaseAction.Kan] + [pm.BaseAction.KaKan] \
-                   + [pm.BaseAction.Riichi] + [pm.BaseAction.Ron] + [pm.BaseAction.Tsumo] \
-                   + [pm.BaseAction.KyuShuKyuHai] + [pm.BaseAction.Pass] * 2
-
-    def __init__(self):
-        self.t = pm.Table()
-        self.game_count = 0
-
-        self.observation_space = Box(dtype=bool, low=0, high=1,
-                                     shape=[self.PLAYER_OBS_DIM, self.MAHJONG_TILE_TYPES])
-        self.oracle_observation_space = Box(dtype=bool, low=0, high=1,
-                                            shape=[self.ORACLE_OBS_DIM, self.MAHJONG_TILE_TYPES])
-        self.full_observation_space = Box(dtype=bool, low=0, high=1,
-                                          shape=[self.PLAYER_OBS_DIM + self.ORACLE_OBS_DIM, self.MAHJONG_TILE_TYPES])
-
-        self.action_space = Discrete(self.ACTION_DIM)
-
-        self.obs_container = np.zeros([self.PLAYER_OBS_DIM + self.ORACLE_OBS_DIM, self.MAHJONG_TILE_TYPES], dtype=np.int8)
-        self.act_container = np.zeros([self.ACTION_DIM], dtype=np.int8)
-
-    def _check_player(self, player_id):
-        if not player_id == self.t.who_make_selection():
-            raise ValueError("You are trying to obtain information from a player who is not making decision !!!! \
-                (current acting player ID is {}, you are trying to get information of player {}".format(
-                    self.t.who_make_selection(), player_id))
-
-    def _proceed(self):
-        while not self.is_over():  # continue until game over or one player has choices
-            phase = self.t.get_phase()
-            if phase < 4:
-                aval_actions = self.t.get_self_actions()
-            elif phase < 16:
-                aval_actions = self.t.get_response_actions()
-            else:
-                aval_actions = [-1]
-            if len(aval_actions) > 1:
-                break
-            else:
-                self.t.make_selection(0)
-
-    def _get_num_aval_actions(self):
-
-        phase = self.t.get_phase()
-
-        if phase < 4:
-            aval_actions = self.t.get_self_actions()
-        elif phase < 16:
-            aval_actions = self.t.get_response_actions()
-        else:
-            aval_actions = [-1]
-
-        return len(aval_actions)
-
-    def reset(self, oya=None, game_wind=None, seed=None, debug_mode=None):
-        if oya is None:
-            oya = self.game_count % 4  # Each player alternatively be the "Oya" (parent)
-        else:
-            assert oya in [0, 1, 2, 3]
-
-        if game_wind is None:
-            game_wind = "east"
-        else:
-            assert game_wind in ["east", "south", "west", "north"]
-
-        self.t = pm.Table()
-        if seed is not None:
-            self.t.seed = seed
-		
-        if debug_mode is not None:
-            self.t.set_debug_mode(debug_mode)
-
-        self.t.game_init_with_metadata({"oya": str(oya), "wind": game_wind})
-        self.riichi_stage2 = False
-        self.may_riichi_tile_id = None
-
-        self.game_count += 1
-
-        self._proceed()
-
-    def step(self, player_id: int, action: int):
-        # Different from single-agent gym env, one should not get the information needed here,
-        # because the next player to act may be different from the current player.
-        # Instead, one should get the information need as follows:
-        # Use .is_over() to know whether this game has finished
-        # Use get_obs(player_id) or get_full_obs(player_id) or get_oracle_obs(player_id) to get observation
-        # For rewards, after the game is over, one may use .get_payoffs
-
-        if not player_id == self.get_curr_player_id():
-            raise ValueError("current acting player ID is {}, but you are trying to ask player {} to act !!".format(
-                self.get_curr_player_id(), player_id))
-
-        if not self.riichi_stage2:
-            self.act_container.fill(0)
-            curr_pid = self.get_curr_player_id()
-            pm.encode_action(self.t, curr_pid, self.act_container)  # no need zeros
-
-            if self.act_container[action] == 0:
-                raise ValueError("Not an action in available actions! (use get_valid_actions(player_id))")
-
-            # ------- IF riichi is possible -------------
-            # riichi is divided to 2 steps: first choosing a tile to discard, then decide if to riichi (if possible)
-            if self.act_container[self.RIICHI]:
-                riichi_tiles = pm.get_riichi_tiles(self.t)
-                riichi_tiles_id = set()
-                for riichi_tile in riichi_tiles:
-                    riichi_tiles_id.add(int(riichi_tile))
-                if action in riichi_tiles_id:
-                    self.riichi_stage2 = True
-                    self.may_riichi_tile_id = action
-
-            # not involving riichi
-            if not self.riichi_stage2:
-                action_type = self.ACTION_TYPES[action]
-
-                if action < self.MAHJONG_TILE_TYPES:
-                    corresponding_tiles = [action]
-
-                elif action in (self.CHILEFT, self.CHIMIDDLE, self.CHIRIGHT):
-                    chi_tile_id = int(self.t.get_selected_action_tile().tile)
-                    if action == self.CHILEFT:
-                        corresponding_tiles = [chi_tile_id + 1, chi_tile_id + 2]
-                    elif action == self.CHIMIDDLE:
-                        corresponding_tiles = [chi_tile_id - 1, chi_tile_id + 1]
-                    elif action == self.CHIRIGHT:
-                        corresponding_tiles = [chi_tile_id - 2, chi_tile_id - 1]
-
-                elif action == self.PON:
-                    pon_tile_id = int(self.t.get_selected_action_tile().tile)
-                    corresponding_tiles = [pon_tile_id, pon_tile_id]
-
-                elif action == self.MINKAN:
-                    kan_tile_id = int(self.t.get_selected_action_tile().tile)
-                    corresponding_tiles = [kan_tile_id] * 3
-
-                # Here we have an approximation, it a player has multiple options to KaKan or AnKan,
-                # the player will random select one if action == ANKAN or KAKAN
-                # However, this case should be very rare in normal play
-
-                elif action == self.ANKAN:
-                    kan_tile_id = np.random.choice(np.argwhere(self.get_obs(curr_pid)[3]).flatten())
-                    corresponding_tiles = [kan_tile_id] * 4
-
-                elif action == self.KAKAN:
-                    obs = self.get_obs(curr_pid)
-                    kan_tile_id = np.random.choice(
-                        np.argwhere((np.sum(obs[:4], axis=0) == 1) * (np.sum(obs[6:10], axis=0) == 3)).flatten())
-                    corresponding_tiles = [kan_tile_id]
-
-                elif action == self.RON:
-                    # include Chan-Kan, Chan-An-Kan
-                    corresponding_tiles = []
-
-                elif action in (self.TSUMO, self.PUSH, self.PASS_RESPONSE):
-                    corresponding_tiles = []
-
-                else:
-                    raise SystemError("This should not happen, please report to the authors")
-
-                try:
-                    if action == self.RON:  # normal ron-agari, chan-kan or chan-an-kan
-                        for ron_type in [pm.BaseAction.Ron, pm.BaseAction.ChanKan, pm.BaseAction.ChanAnKan]:
-                            try:
-                                self.t.make_selection_from_action_basetile(
-                                    ron_type, corresponding_tiles, action >= self.MAHJONG_TILE_TYPES)
-                            except:
-                                pass
-                    else:
-                        self.t.make_selection_from_action_basetile(
-                            action_type, corresponding_tiles, action >= self.MAHJONG_TILE_TYPES)
-
-                except Exception as inst:
-                    print("-------------- execption in make_selection_from_action_basetile ------------------")
-                    print(inst)
-                    print(action_type, corresponding_tiles)
-                    obs = self.get_obs(curr_pid)
-                    print(obs.astype(int))
-                    self.render()
-                    raise SystemError
-
-        else:  # riichi step 2
-            assert action in (self.RIICHI, self.PASS_RIICHI)
-            if action == self.RIICHI:
-                action_type = pm.BaseAction.Riichi
-            else:
-                action_type = pm.BaseAction.Play
-
-            self.t.make_selection_from_action_basetile(action_type, [self.may_riichi_tile_id], False)
-            self.riichi_stage2 = False
-            self.may_riichi_tile_id = None
-
-        self._proceed()
-
-    def _get_obs_from_table(self, player_id):
-        self.obs_container.fill(0)  # passing zeros array to C++
-        pm.encode_table(self.t, player_id, True, self.obs_container)
-        if self.riichi_stage2:
-            pm.encode_table_riichi_step2(self.t, self.may_riichi_tile_id, self.obs_container)
-
-    def get_obs(self, player_id: int):
-        self._check_player(player_id)
-        self._get_obs_from_table(player_id)
-        return self.obs_container[:self.PLAYER_OBS_DIM].astype(bool)
-
-    def get_oracle_obs(self, player_id: int):
-        self._check_player(player_id)
-        self._get_obs_from_table(player_id)
-        return self.obs_container[-self.ORACLE_OBS_DIM:].astype(bool)
-
-    def get_full_obs(self, player_id: int):
-        self._check_player(player_id)
-        self._get_obs_from_table(player_id)
-        return self.obs_container.copy().astype(bool)
-
-    def get_valid_actions(self, nhot=False):
-        if not self.riichi_stage2:
-            self.act_container.fill(0)
-            pm.encode_action(self.t, self.get_curr_player_id(), self.act_container)
-            act_container = self.act_container.copy().astype(bool)
-            act_container[self.RIICHI] = 0
-            act_container[self.PASS_RIICHI] = 0
-        else:
-            act_container = np.zeros([self.ACTION_DIM], dtype=bool)
-            act_container[self.RIICHI] = 1
-            act_container[self.PASS_RIICHI] = 1
-
-        if nhot:
-            return act_container
-        else:
-            return np.argwhere(act_container).reshape([-1])
-
-    def get_payoffs(self):
-        payoffs = np.zeros([4], dtype=np.float32)
-        for i in range(4):
-            payoffs[i] = self.t.get_result().score[i] - self.INIT_POINTS
-        return payoffs
-
-    def is_over(self):
-        return self.Phases[self.t.get_phase()] == "GAME_OVER"
-
-    def get_curr_player_id(self):
-        if self.t.get_phase() < 16:
-            return self.t.who_make_selection()
-        elif self.t.get_phase() == 16:
-            warnings.warn("This game has ended, get_curr_player_id return -1 !!")
-            return -1
-        else:
-            raise SystemError
-
-    def render(self, mode='human'):
-        print("----------- current player: {} -----------------".format(self.get_curr_player_id()))
-        print("[Player 0]")
-        print(self.t.players[0].to_string())
-        print("[Player 1]")
-        print(self.t.players[1].to_string())
-        print("[Player 2]")
-        print(self.t.players[2].to_string())
-        print("[Player 3]")
-        print(self.t.players[3].to_string())
-
-
-class SingleAgentMahjongEnv(gym.Env):
-    THIS_AGENT_ID = 0
-    # The agent is the player 0 in MahjongEnv (while Oya may be others)
-
-    def __init__(self, opponent_agent="random"):
-
-        super(SingleAgentMahjongEnv, self).__init__()
-
-        if opponent_agent == "random":
-            self.opponent_agent = "random"
-        else:
-            try:
-                import torch
-                from .models import VLOGMahjong
-                state_dict = torch.load(opponent_agent, map_location="cpu")
-                if "f_s2q.network_modules.0.weight" in state_dict:
-                    alg = "ddqn"
-                elif "f_s2pi0.network_modules.0.weight" in state_dict:
-                    alg = "bc"
-                else:
-                    raise Exception("Unknown model")
-                self.opponent_agent = VLOGMahjong(algorithm=alg)
-
-                keys = list(state_dict.keys())
-                for key in keys:
-                    if key not in list(self.opponent_agent.state_dict().keys()):
-                        state_dict.pop(key)
-                self.opponent_agent.load_state_dict(state_dict)
-
-                if torch.cuda.is_available():
-                    device = torch.device("cuda")
-                    self.opponent_agent.device = device
-                    self.opponent_agent.to(device=device)
-                    print("----- CUDA detected, using CUDA for inference. -----")
-                
-                self.opponent_agent.eval()  # not necessary now, but remained for future
-                
-            except Exception as e:
-                print(e)
-                raise FileNotFoundError("opponent_agent should be 'random' or the path of a pre-trained model (You can download the pre-trained model from pymahjong github release: https://github.com/Agony5757/mahjong/releases ")
-
-        self.env = MahjongEnv()
-
-        self.observation_space = self.env.observation_space
-        self.oracle_observation_space = self.env.oracle_observation_space
-        self.full_observation_space = self.env.full_observation_space
-        self.action_space = self.env.action_space
-
-    def _proceed_until_agent_turn(self):
-        while (not self.env.is_over()) and self.env.get_curr_player_id() != self.THIS_AGENT_ID:
-            if self.opponent_agent == "random":
-                aval_actions = self.env.get_valid_actions(nhot=False)
-                self.env.step(self.env.get_curr_player_id(), np.random.choice(aval_actions))
-            else:
-                action_mask =  self.env.get_valid_actions(nhot=True)
-                obs = self.env.get_obs(self.env.get_curr_player_id())
-                action = self.opponent_agent.select(obs, action_mask=action_mask, greedy=True)
-                self.env.step(self.env.get_curr_player_id(), action)
-
-    def reset(self, oya=None, game_wind=None, seed=None):
-        self.env.reset(oya=oya, game_wind=game_wind, seed=seed)
-        self._proceed_until_agent_turn()
-
-        if self.env.is_over():
-            # if espisode length == 0 for the current player, ignore this game and re-start a new game
-            return self.reset()
-        else:
-            return self.get_obs()
-
-    def step(self, action):
-        assert self.env.get_curr_player_id() == self.THIS_AGENT_ID
-
-        self.env.step(0, action)
-        self._proceed_until_agent_turn()
-
-        if self.env.is_over():
-            r = self.env.get_payoffs()[self.THIS_AGENT_ID]
-            done = True
-        else:
-            r = 0
-            done = False
-
-        return self.env.get_obs(self.THIS_AGENT_ID), r, done, {}
-
-    def get_obs(self):
-        return self.env.get_obs(self.THIS_AGENT_ID)
-
-    def get_oracle_obs(self):
-        return self.env.get_oracle_obs(self.THIS_AGENT_ID)
-
-    def get_full_obs(self):
-        return self.env.get_full_obs(self.THIS_AGENT_ID)
-
-    def get_valid_actions(self):
-        return self.env.get_valid_actions(nhot=False)
-
-    def render(self, mode='human'):
-        print("-----------------------------------")
-        print("[Player 0 (this agent)]")
-        print(self.env.t.players[0].to_string())
-        print("[Player 1 (the first opponent counterclockwise)]")
-        print(self.env.t.players[1].to_string())
-        print("[Player 2 (the second opponent counterclockwise)]")
-        print(self.env.t.players[2].to_string())
-        print("[Player 3 (the third opponent counterclockwise)]")
-        print(self.env.t.players[3].to_string())
-
-
-
+import gym
+import numpy as np
+import warnings
+from gym.spaces import Discrete, Box
+import MahjongPyWrapper as pm
+
+np.set_printoptions(threshold=np.inf)
+
+
+class MahjongEnv(gym.Env):
+
+    PLAYER_OBS_DIM = 93
+    ORACLE_OBS_DIM = 18
+    ACTION_DIM = 47
+    MAHJONG_TILE_TYPES = 34
+    INIT_POINTS = 25000
+
+    # ACTION INDICES
+    CHILEFT = 34
+    CHIMIDDLE = 35
+    CHIRIGHT = 36
+    PON = 37
+    ANKAN = 38
+    MINKAN = 39
+    KAKAN = 40
+
+    RIICHI = 41
+    RON = 42
+    TSUMO = 43
+    PUSH = 44
+
+    PASS_RESPONSE = 45
+    PASS_RIICHI = 46
+
+    # corresponding to self.t.get_phase()
+    Phases = ("P1_ACTION", "P2_ACTION", "P3_ACTION", "P4_ACTION", "P1_RESPONSE", "P2_RESPONSE", "P3_RESPONSE",
+              "P4_RESPONSE", "P1_抢杠RESPONSE", "P2_抢杠RESPONSE", "P3_抢杠RESPONSE", "P4_抢杠RESPONSE",
+              "P1_抢暗杠RESPONSE", "P2_抢暗杠RESPONSE", " P3_抢暗杠RESPONSE", " P4_抢暗杠RESPONSE", "GAME_OVER",
+              "P1_DRAW, P2_DRAW, P3_DRAW, P4_DRAW")
+
+    # pymahjhong.BaseAction
+    ACTION_TYPES = [pm.BaseAction.Discard] * MAHJONG_TILE_TYPES + [pm.BaseAction.Chi] * 3 + [pm.BaseAction.Pon] \
+                   + [pm.BaseAction.AnKan] + [pm.BaseAction.Kan] + [pm.BaseAction.KaKan] \
+                   + [pm.BaseAction.Riichi] + [pm.BaseAction.Ron] + [pm.BaseAction.Tsumo] \
+                   + [pm.BaseAction.Kyushukyuhai] + [pm.BaseAction.Pass] * 2
+
+    def __init__(self):
+        self.t = pm.Table()
+        self.game_count = 0
+
+        self.observation_space = Box(dtype=bool, low=0, high=1,
+                                     shape=[self.PLAYER_OBS_DIM, self.MAHJONG_TILE_TYPES])
+        self.oracle_observation_space = Box(dtype=bool, low=0, high=1,
+                                            shape=[self.ORACLE_OBS_DIM, self.MAHJONG_TILE_TYPES])
+        self.full_observation_space = Box(dtype=bool, low=0, high=1,
+                                          shape=[self.PLAYER_OBS_DIM + self.ORACLE_OBS_DIM, self.MAHJONG_TILE_TYPES])
+
+        self.action_space = Discrete(self.ACTION_DIM)
+
+        self.obs_container = np.zeros([self.PLAYER_OBS_DIM + self.ORACLE_OBS_DIM, self.MAHJONG_TILE_TYPES], dtype=np.int8)
+        self.act_container = np.zeros([self.ACTION_DIM], dtype=np.int8)
+
+    def _check_player(self, player_id):
+        if not player_id == self.t.who_make_selection():
+            raise ValueError("You are trying to obtain information from a player who is not making decision !!!! \
+                (current acting player ID is {}, you are trying to get information of player {}".format(
+                    self.t.who_make_selection(), player_id))
+
+    def _proceed(self):
+        while not self.is_over():  # continue until game over or one player has choices
+            phase = self.t.get_phase()
+            if phase < 4:
+                aval_actions = self.t.get_self_actions()
+            elif phase < 16:
+                aval_actions = self.t.get_response_actions()
+            else:
+                aval_actions = [-1]
+            if len(aval_actions) > 1:
+                break
+            else:
+                self.t.make_selection(0)
+
+    def _get_num_aval_actions(self):
+
+        phase = self.t.get_phase()
+
+        if phase < 4:
+            aval_actions = self.t.get_self_actions()
+        elif phase < 16:
+            aval_actions = self.t.get_response_actions()
+        else:
+            aval_actions = [-1]
+
+        return len(aval_actions)
+
+    def reset(self, oya=None, game_wind=None, seed=None, debug_mode=None):
+        if oya is None:
+            oya = self.game_count % 4  # Each player alternatively be the "Oya" (parent)
+        else:
+            assert oya in [0, 1, 2, 3]
+
+        if game_wind is None:
+            game_wind = "east"
+        else:
+            assert game_wind in ["east", "south", "west", "north"]
+
+        self.t = pm.Table()
+        if seed is not None:
+            self.t.seed = seed
+		
+        if debug_mode is not None:
+            self.t.set_debug_mode(debug_mode)
+
+        self.t.game_init_with_metadata({"oya": str(oya), "wind": game_wind})
+        self.riichi_stage2 = False
+        self.may_riichi_tile_id = None
+
+        self.game_count += 1
+
+        self._proceed()
+
+    def step(self, player_id: int, action: int):
+        # Different from single-agent gym env, one should not get the information needed here,
+        # because the next player to act may be different from the current player.
+        # Instead, one should get the information need as follows:
+        # Use .is_over() to know whether this game has finished
+        # Use get_obs(player_id) or get_full_obs(player_id) or get_oracle_obs(player_id) to get observation
+        # For rewards, after the game is over, one may use .get_payoffs
+
+        if not player_id == self.get_curr_player_id():
+            raise ValueError("current acting player ID is {}, but you are trying to ask player {} to act !!".format(
+                self.get_curr_player_id(), player_id))
+
+        if not self.riichi_stage2:
+            self.act_container.fill(0)
+            curr_pid = self.get_curr_player_id()
+            pm.encv1_encode_action(self.t, curr_pid, self.act_container)  # no need zeros
+
+            if self.act_container[action] == 0:
+                raise ValueError("Not an action in available actions! (use get_valid_actions(player_id))")
+
+            # ------- IF riichi is possible -------------
+            # riichi is divided to 2 steps: first choosing a tile to discard, then decide if to riichi (if possible)
+            if self.act_container[self.RIICHI]:
+                riichi_tiles = pm.encv1_get_riichi_tiles(self.t)
+                riichi_tiles_id = set()
+                for riichi_tile in riichi_tiles:
+                    riichi_tiles_id.add(int(riichi_tile))
+                if action in riichi_tiles_id:
+                    self.riichi_stage2 = True
+                    self.may_riichi_tile_id = action
+
+            # not involving riichi
+            if not self.riichi_stage2:
+                action_type = self.ACTION_TYPES[action]
+
+                if action < self.MAHJONG_TILE_TYPES:
+                    corresponding_tiles = [action]
+
+                elif action in (self.CHILEFT, self.CHIMIDDLE, self.CHIRIGHT):
+                    chi_tile_id = int(self.t.get_selected_action_tile().tile)
+                    if action == self.CHILEFT:
+                        corresponding_tiles = [chi_tile_id + 1, chi_tile_id + 2]
+                    elif action == self.CHIMIDDLE:
+                        corresponding_tiles = [chi_tile_id - 1, chi_tile_id + 1]
+                    elif action == self.CHIRIGHT:
+                        corresponding_tiles = [chi_tile_id - 2, chi_tile_id - 1]
+
+                elif action == self.PON:
+                    pon_tile_id = int(self.t.get_selected_action_tile().tile)
+                    corresponding_tiles = [pon_tile_id, pon_tile_id]
+
+                elif action == self.MINKAN:
+                    kan_tile_id = int(self.t.get_selected_action_tile().tile)
+                    corresponding_tiles = [kan_tile_id] * 3
+
+                # Here we have an approximation, it a player has multiple options to KaKan or AnKan,
+                # the player will random select one if action == ANKAN or KAKAN
+                # However, this case should be very rare in normal play
+
+                elif action == self.ANKAN:
+                    kan_tile_id = np.random.choice(np.argwhere(self.get_obs(curr_pid)[3]).flatten())
+                    corresponding_tiles = [kan_tile_id] * 4
+
+                elif action == self.KAKAN:
+                    obs = self.get_obs(curr_pid)
+                    kan_tile_id = np.random.choice(
+                        np.argwhere((np.sum(obs[:4], axis=0) == 1) * (np.sum(obs[6:10], axis=0) == 3)).flatten())
+                    corresponding_tiles = [kan_tile_id]
+
+                elif action == self.RON:
+                    # include Chan-Kan, Chan-An-Kan
+                    corresponding_tiles = []
+
+                elif action in (self.TSUMO, self.PUSH, self.PASS_RESPONSE):
+                    corresponding_tiles = []
+
+                else:
+                    raise SystemError("This should not happen, please report to the authors")
+
+                try:
+                    if action == self.RON:  # normal ron-agari, chan-kan or chan-an-kan
+                        for ron_type in [pm.BaseAction.Ron, pm.BaseAction.ChanKan, pm.BaseAction.ChanAnKan]:
+                            try:
+                                self.t.make_selection_from_action_basetile(
+                                    ron_type, corresponding_tiles, action >= self.MAHJONG_TILE_TYPES)
+                            except:
+                                pass
+                    else:
+                        self.t.make_selection_from_action_basetile(
+                            action_type, corresponding_tiles, action >= self.MAHJONG_TILE_TYPES)
+
+                except Exception as inst:
+                    print("-------------- execption in make_selection_from_action_basetile ------------------")
+                    print(inst)
+                    print(action_type, corresponding_tiles)
+                    obs = self.get_obs(curr_pid)
+                    print(obs.astype(int))
+                    self.render()
+                    raise SystemError
+
+        else:  # riichi step 2
+            assert action in (self.RIICHI, self.PASS_RIICHI)
+            if action == self.RIICHI:
+                action_type = pm.BaseAction.Riichi
+            else:
+                action_type = pm.BaseAction.Discard
+
+            self.t.make_selection_from_action_basetile(action_type, [self.may_riichi_tile_id], False)
+            self.riichi_stage2 = False
+            self.may_riichi_tile_id = None
+
+        self._proceed()
+
+    def _get_obs_from_table(self, player_id):
+        self.obs_container.fill(0)  # passing zeros array to C++
+        pm.encv1_encode_table(self.t, player_id, True, self.obs_container)
+        if self.riichi_stage2:
+            pm.encv1_encode_table_riichi_step2(self.t, self.may_riichi_tile_id, self.obs_container)
+
+    def get_obs(self, player_id: int):
+        self._check_player(player_id)
+        self._get_obs_from_table(player_id)
+        return self.obs_container[:self.PLAYER_OBS_DIM].astype(bool)
+
+    def get_oracle_obs(self, player_id: int):
+        self._check_player(player_id)
+        self._get_obs_from_table(player_id)
+        return self.obs_container[-self.ORACLE_OBS_DIM:].astype(bool)
+
+    def get_full_obs(self, player_id: int):
+        self._check_player(player_id)
+        self._get_obs_from_table(player_id)
+        return self.obs_container.copy().astype(bool)
+
+    def get_valid_actions(self, nhot=False):
+        if not self.riichi_stage2:
+            self.act_container.fill(0)
+            pm.encv1_encode_action(self.t, self.get_curr_player_id(), self.act_container)
+            act_container = self.act_container.copy().astype(bool)
+            act_container[self.RIICHI] = 0
+            act_container[self.PASS_RIICHI] = 0
+        else:
+            act_container = np.zeros([self.ACTION_DIM], dtype=bool)
+            act_container[self.RIICHI] = 1
+            act_container[self.PASS_RIICHI] = 1
+
+        if nhot:
+            return act_container
+        else:
+            return np.argwhere(act_container).reshape([-1])
+
+    def get_payoffs(self):
+        payoffs = np.zeros([4], dtype=np.float32)
+        for i in range(4):
+            payoffs[i] = self.t.get_result().score[i] - self.INIT_POINTS
+        return payoffs
+
+    def is_over(self):
+        return self.Phases[self.t.get_phase()] == "GAME_OVER"
+
+    def get_curr_player_id(self):
+        if self.t.get_phase() < 16:
+            return self.t.who_make_selection()
+        elif self.t.get_phase() == 16:
+            warnings.warn("This game has ended, get_curr_player_id return -1 !!")
+            return -1
+        else:
+            raise SystemError
+
+    def render(self, mode='human'):
+        print("----------- current player: {} -----------------".format(self.get_curr_player_id()))
+        print("[Player 0]")
+        print(self.t.players[0].to_string())
+        print("[Player 1]")
+        print(self.t.players[1].to_string())
+        print("[Player 2]")
+        print(self.t.players[2].to_string())
+        print("[Player 3]")
+        print(self.t.players[3].to_string())
+
+
+class SingleAgentMahjongEnv(gym.Env):
+    THIS_AGENT_ID = 0
+    # The agent is the player 0 in MahjongEnv (while Oya may be others)
+
+    def __init__(self, opponent_agent="random"):
+
+        super(SingleAgentMahjongEnv, self).__init__()
+
+        if opponent_agent == "random":
+            self.opponent_agent = "random"
+        else:
+            try:
+                import torch
+                from .models import VLOGMahjong
+                state_dict = torch.load(opponent_agent, map_location="cpu")
+                if "f_s2q.network_modules.0.weight" in state_dict:
+                    alg = "ddqn"
+                elif "f_s2pi0.network_modules.0.weight" in state_dict:
+                    alg = "bc"
+                else:
+                    raise Exception("Unknown model")
+                self.opponent_agent = VLOGMahjong(algorithm=alg)
+
+                keys = list(state_dict.keys())
+                for key in keys:
+                    if key not in list(self.opponent_agent.state_dict().keys()):
+                        state_dict.pop(key)
+                self.opponent_agent.load_state_dict(state_dict)
+
+                if torch.cuda.is_available():
+                    device = torch.device("cuda")
+                    self.opponent_agent.device = device
+                    self.opponent_agent.to(device=device)
+                    print("----- CUDA detected, using CUDA for inference. -----")
+                
+                self.opponent_agent.eval()  # not necessary now, but remained for future
+                
+            except Exception as e:
+                print(e)
+                raise FileNotFoundError("opponent_agent should be 'random' or the path of a pre-trained model (You can download the pre-trained model from pymahjong github release: https://github.com/Agony5757/mahjong/releases ")
+
+        self.env = MahjongEnv()
+
+        self.observation_space = self.env.observation_space
+        self.oracle_observation_space = self.env.oracle_observation_space
+        self.full_observation_space = self.env.full_observation_space
+        self.action_space = self.env.action_space
+
+    def _proceed_until_agent_turn(self):
+        while (not self.env.is_over()) and self.env.get_curr_player_id() != self.THIS_AGENT_ID:
+            if self.opponent_agent == "random":
+                aval_actions = self.env.get_valid_actions(nhot=False)
+                self.env.step(self.env.get_curr_player_id(), np.random.choice(aval_actions))
+            else:
+                action_mask =  self.env.get_valid_actions(nhot=True)
+                obs = self.env.get_obs(self.env.get_curr_player_id())
+                action = self.opponent_agent.select(obs, action_mask=action_mask, greedy=True)
+                self.env.step(self.env.get_curr_player_id(), action)
+
+    def reset(self, oya=None, game_wind=None, seed=None):
+        self.env.reset(oya=oya, game_wind=game_wind, seed=seed)
+        self._proceed_until_agent_turn()
+
+        if self.env.is_over():
+            # if espisode length == 0 for the current player, ignore this game and re-start a new game
+            return self.reset()
+        else:
+            return self.get_obs()
+
+    def step(self, action):
+        assert self.env.get_curr_player_id() == self.THIS_AGENT_ID
+
+        self.env.step(0, action)
+        self._proceed_until_agent_turn()
+
+        if self.env.is_over():
+            r = self.env.get_payoffs()[self.THIS_AGENT_ID]
+            done = True
+        else:
+            r = 0
+            done = False
+
+        return self.env.get_obs(self.THIS_AGENT_ID), r, done, {}
+
+    def get_obs(self):
+        return self.env.get_obs(self.THIS_AGENT_ID)
+
+    def get_oracle_obs(self):
+        return self.env.get_oracle_obs(self.THIS_AGENT_ID)
+
+    def get_full_obs(self):
+        return self.env.get_full_obs(self.THIS_AGENT_ID)
+
+    def get_valid_actions(self):
+        return self.env.get_valid_actions(nhot=False)
+
+    def render(self, mode='human'):
+        print("-----------------------------------")
+        print("[Player 0 (this agent)]")
+        print(self.env.t.players[0].to_string())
+        print("[Player 1 (the first opponent counterclockwise)]")
+        print(self.env.t.players[1].to_string())
+        print("[Player 2 (the second opponent counterclockwise)]")
+        print(self.env.t.players[2].to_string())
+        print("[Player 3 (the third opponent counterclockwise)]")
+        print(self.env.t.players[3].to_string())
+
+
+
```

## pymahjong/models.py

 * *Ordering differences only*

```diff
@@ -1,211 +1,211 @@
-import torch
-import torch.nn as nn
-import numpy as np
-import torch.distributions as dis
-from .base_modules import *
-
-torch.set_default_dtype(torch.float32)
-
-INFINITY = 1e9
-
-
-class VLOGMahjong(nn.Module):
-
-    def __init__(self, **kwargs):
-
-        super(VLOGMahjong, self).__init__()
-
-        self.action_size = 47
-        self.algorithm = kwargs["algorithm"] if ("algorithm" in kwargs) else 'ddqn'
-
-        self.hidden_layer_width = kwargs["hidden_layer_width"] if ("hidden_layer_width" in kwargs) else 1024
-        self.half_hidden_layer_depth = kwargs["half_hidden_layer_depth"] if ("half_hidden_layer_depth" in kwargs) else 2
-        self.act_fn = kwargs["act_fn"] if ("act_fn" in kwargs) else 'relu'
-        self.z_stochastic_size = kwargs["z_stochastic_size"] if ("z_stochastic_size" in kwargs) else None
-
-        self.type = kwargs["type"] if ("type" in kwargs) else "vlog"
-
-        # ---------------------------------------- type settings ----------------------------------------
-        # Available options:
-        if self.type not in ["baseline", "oracle", "vlog", "vlog-self", "suphx", "opd", "vlog-oracle"]:
-            raise ValueError(
-                "Model type must be one of these: ['baseline', 'oracle', 'vlog', 'vlog-self', 'suphx', 'opd', 'vlog-oracle']")
-
-        if self.type not in ["oracle", "suphx", "vlog-oracle"]:
-            self.input_forward_size = [93, 34]
-        else:
-            self.input_forward_size = [111, 34]
-
-        if self.type not in ["vlog-self"]:
-            self.input_oracle_size = [111, 34]
-        else:
-            self.input_oracle_size = self.input_forward_size
-
-        if self.type in ["baseline", "oracle", "suphx", "opd"]:
-            self.use_prior_only = True
-        else:
-            self.use_prior_only = False
-
-        self.device = 'cpu'
-
-        if self.z_stochastic_size is None:
-            if self.type in ["vlog", "vlog-self", "vlog-oracle"]:
-                self.z_stochastic_size = int(self.hidden_layer_width / 2)
-            else:
-                self.z_stochastic_size = 0
-        # ---------------------------------------- setting for OPD ----------------------------------------
-        if self.type == "opd":
-            self.opd_mu = kwargs["opd_mu"]  # weight of distillation loss
-            self.opd_teacher_model = kwargs["opd_teacher_model"]
-
-        # -------------------- Define Network Connections ------------------
-        if self.act_fn == "relu":
-            self.forward_act_fn = nn.ReLU
-        elif self.act_fn == "tanh":
-            self.forward_act_fn = nn.Tanh
-        else:
-            raise ValueError("activation function should be tanh or relu")
-
-        self.latent_module = nn.ModuleList()
-
-        if len(self.input_forward_size) == 1:
-            self.encoder = nn.Sequential(nn.Linear(self.input_forward_size[0], self.hidden_layer_width),
-                                         self.forward_act_fn()
-                                         )
-            self.encoder_oracle = nn.Sequential(nn.Linear(self.input_oracle_size[0], self.hidden_layer_width),
-                                                self.forward_act_fn()
-                                                )
-            self.phi_size = self.hidden_layer_width
-            self.phi_size_oracle = self.hidden_layer_width
-
-        else:
-            if len(self.input_forward_size) == 2:
-                resolution = "{}".format(self.input_forward_size[1])
-            elif len(self.input_forward_size) == 3:
-                resolution = "{}x{}".format(self.input_forward_size[1], self.input_forward_size[2])
-            else:
-                raise NotImplementedError
-
-            self.encoder, self.phi_size = make_cnn(resolution, self.input_forward_size[0])
-            self.encoder_oracle, self.phi_size_oracle = make_cnn(resolution, self.input_oracle_size[0])
-
-        self.latent_module.append(self.encoder_oracle)
-        self.latent_module.append(self.encoder)
-
-        forward_fnns = nn.ModuleList()
-        last_layer_size = self.phi_size
-        for _ in range(self.half_hidden_layer_depth - 1):
-            forward_fnns.append(nn.Linear(last_layer_size, self.hidden_layer_width))
-            forward_fnns.append(self.forward_act_fn())
-            last_layer_size = self.hidden_layer_width
-        self.forward_fnn = nn.Sequential(*forward_fnns)
-        self.latent_module.append(self.forward_fnn)
-
-        pre_zp_size = self.hidden_layer_width
-
-        if self.z_stochastic_size:
-            self.f_h2muzp = nn.Linear(pre_zp_size, self.z_stochastic_size)
-            self.f_h2logsigzp = nn.Sequential(nn.Linear(pre_zp_size, self.z_stochastic_size),
-                                              MinusOneModule()
-                                              )
-            self.latent_module.append(self.f_h2logsigzp)
-            self.latent_module.append(self.f_h2muzp)
-
-        else:
-            self.f_h2zp = nn.Sequential(nn.Linear(pre_zp_size, self.hidden_layer_width),
-                                        self.forward_act_fn())
-            self.latent_module.append(self.f_h2zp)
-
-        if not self.use_prior_only:
-            oracle_fnns = nn.ModuleList()
-            last_layer_size = self.phi_size_oracle
-            for _ in range(self.half_hidden_layer_depth - 1):
-                oracle_fnns.append(nn.Linear(last_layer_size, self.hidden_layer_width))
-                oracle_fnns.append(self.forward_act_fn())
-                last_layer_size = self.hidden_layer_width
-
-            self.oracle_fnn = nn.Sequential(*oracle_fnns)
-            self.latent_module.append(self.oracle_fnn)
-
-            pre_zq_size = self.hidden_layer_width
-            if self.z_stochastic_size:
-                self.f_hb2muzq = nn.Linear(pre_zq_size, self.z_stochastic_size)
-                self.f_hb2logsigzq = nn.Sequential(nn.Linear(pre_zq_size, self.z_stochastic_size),
-                                                   MinusOneModule())
-                self.latent_module.append(self.f_hb2logsigzq)
-                self.latent_module.append(self.f_hb2muzq)
-            else:
-                self.f_hb2zq = nn.Sequential(nn.Linear(pre_zq_size, self.hidden_layer_width),
-                                             self.forward_act_fn())
-                self.latent_module.append(self.f_hb2zq)
-
-        # ----------------------------- RL part -----------------------------
-        self.alg_config = kwargs["alg_config"] if ("alg_config" in kwargs) else {}
-
-        pre_rl_size = self.z_stochastic_size if self.z_stochastic_size else self.hidden_layer_width
-
-        if self.algorithm == 'ddqn':
-            self.epsilon = kwargs["epsilon"] if ("epsilon" in kwargs) else 0.05
-            self.dueling = self.alg_config["dueling"] if ("dueling" in self.alg_config) else True
-            self.alg_type = 'value_based'
-            self.f_s2q = DiscreteActionQNetwork(pre_rl_size, self.action_size,
-                                                 hidden_layers=[self.hidden_layer_width] * self.half_hidden_layer_depth,
-                                                 dueling=self.dueling, act_fn=self.forward_act_fn)
-
-        elif self.algorithm == 'bc':
-            self.f_s2pi0 = DiscreteActionPolicyNetwork(pre_rl_size, self.action_size,
-                                                       hidden_layers=[self.hidden_layer_width] * self.half_hidden_layer_depth,
-                                                       act_fn=self.forward_act_fn, device=self.device)
-            self.alg_type = 'supervised'
-
-        else:
-            raise NotImplementedError("algorithm can only be 'bc' or 'ddqn'")
-
-
-    def select(self, x, action_mask=None, greedy=True):
-
-        with torch.no_grad():
-
-            if action_mask is not None:
-                action_mask = torch.from_numpy(
-                    action_mask.astype(np.float32).reshape([1, self.action_size]))
-
-            x = torch.from_numpy(x.astype(np.float32).reshape([1, *list(x.shape)])).to(device=self.device)
-
-            x = self.encoder(x)
-            e = self.forward_fnn(x)
-            muz = self.f_h2muzp(e)
-            logsigz = self.f_h2logsigzp(e)
-            dist = dis.normal.Normal(muz, torch.exp(logsigz))
-            z = dist.sample()
-
-            self.h_t = z
-            self.zp_tm1 = z
-
-            if self.algorithm == 'bc':
-
-                a = self.f_s2pi0.sample_action(self.h_t, action_mask=action_mask, greedy=greedy).item()
-
-            elif self.algorithm == 'ddqn':
-                q = self.f_s2q(self.h_t).detach().cpu()
-                if action_mask is not None:
-                    q = q.clamp(-INFINITY, INFINITY) * action_mask - 2 * INFINITY * (1 - action_mask)
-
-                if greedy:
-                    a = torch.argmax(q, dim=-1)
-                    if np.prod(a.shape) == 1:
-                        a = a.item()  # discrete action
-                else:
-                    if np.random.rand() < self.epsilon:
-                        if action_mask is None:
-                            a = np.random.randint(self.action_size)
-                        else:
-                            valid_action_ind = np.nonzero(action_mask.cpu().numpy().reshape([-1]))
-                            valid_actions = np.arange(self.action_size)[valid_action_ind]
-                            a = int(valid_actions[np.random.randint(len(valid_actions))])
-                    else:
-                        a = torch.argmax(q, dim=-1)
-                        if np.prod(a.shape) == 1:
-                            a = int(a.item())  # discrete action
-
-        return a
+import torch
+import torch.nn as nn
+import numpy as np
+import torch.distributions as dis
+from .base_modules import *
+
+torch.set_default_dtype(torch.float32)
+
+INFINITY = 1e9
+
+
+class VLOGMahjong(nn.Module):
+
+    def __init__(self, **kwargs):
+
+        super(VLOGMahjong, self).__init__()
+
+        self.action_size = 47
+        self.algorithm = kwargs["algorithm"] if ("algorithm" in kwargs) else 'ddqn'
+
+        self.hidden_layer_width = kwargs["hidden_layer_width"] if ("hidden_layer_width" in kwargs) else 1024
+        self.half_hidden_layer_depth = kwargs["half_hidden_layer_depth"] if ("half_hidden_layer_depth" in kwargs) else 2
+        self.act_fn = kwargs["act_fn"] if ("act_fn" in kwargs) else 'relu'
+        self.z_stochastic_size = kwargs["z_stochastic_size"] if ("z_stochastic_size" in kwargs) else None
+
+        self.type = kwargs["type"] if ("type" in kwargs) else "vlog"
+
+        # ---------------------------------------- type settings ----------------------------------------
+        # Available options:
+        if self.type not in ["baseline", "oracle", "vlog", "vlog-self", "suphx", "opd", "vlog-oracle"]:
+            raise ValueError(
+                "Model type must be one of these: ['baseline', 'oracle', 'vlog', 'vlog-self', 'suphx', 'opd', 'vlog-oracle']")
+
+        if self.type not in ["oracle", "suphx", "vlog-oracle"]:
+            self.input_forward_size = [93, 34]
+        else:
+            self.input_forward_size = [111, 34]
+
+        if self.type not in ["vlog-self"]:
+            self.input_oracle_size = [111, 34]
+        else:
+            self.input_oracle_size = self.input_forward_size
+
+        if self.type in ["baseline", "oracle", "suphx", "opd"]:
+            self.use_prior_only = True
+        else:
+            self.use_prior_only = False
+
+        self.device = 'cpu'
+
+        if self.z_stochastic_size is None:
+            if self.type in ["vlog", "vlog-self", "vlog-oracle"]:
+                self.z_stochastic_size = int(self.hidden_layer_width / 2)
+            else:
+                self.z_stochastic_size = 0
+        # ---------------------------------------- setting for OPD ----------------------------------------
+        if self.type == "opd":
+            self.opd_mu = kwargs["opd_mu"]  # weight of distillation loss
+            self.opd_teacher_model = kwargs["opd_teacher_model"]
+
+        # -------------------- Define Network Connections ------------------
+        if self.act_fn == "relu":
+            self.forward_act_fn = nn.ReLU
+        elif self.act_fn == "tanh":
+            self.forward_act_fn = nn.Tanh
+        else:
+            raise ValueError("activation function should be tanh or relu")
+
+        self.latent_module = nn.ModuleList()
+
+        if len(self.input_forward_size) == 1:
+            self.encoder = nn.Sequential(nn.Linear(self.input_forward_size[0], self.hidden_layer_width),
+                                         self.forward_act_fn()
+                                         )
+            self.encoder_oracle = nn.Sequential(nn.Linear(self.input_oracle_size[0], self.hidden_layer_width),
+                                                self.forward_act_fn()
+                                                )
+            self.phi_size = self.hidden_layer_width
+            self.phi_size_oracle = self.hidden_layer_width
+
+        else:
+            if len(self.input_forward_size) == 2:
+                resolution = "{}".format(self.input_forward_size[1])
+            elif len(self.input_forward_size) == 3:
+                resolution = "{}x{}".format(self.input_forward_size[1], self.input_forward_size[2])
+            else:
+                raise NotImplementedError
+
+            self.encoder, self.phi_size = make_cnn(resolution, self.input_forward_size[0])
+            self.encoder_oracle, self.phi_size_oracle = make_cnn(resolution, self.input_oracle_size[0])
+
+        self.latent_module.append(self.encoder_oracle)
+        self.latent_module.append(self.encoder)
+
+        forward_fnns = nn.ModuleList()
+        last_layer_size = self.phi_size
+        for _ in range(self.half_hidden_layer_depth - 1):
+            forward_fnns.append(nn.Linear(last_layer_size, self.hidden_layer_width))
+            forward_fnns.append(self.forward_act_fn())
+            last_layer_size = self.hidden_layer_width
+        self.forward_fnn = nn.Sequential(*forward_fnns)
+        self.latent_module.append(self.forward_fnn)
+
+        pre_zp_size = self.hidden_layer_width
+
+        if self.z_stochastic_size:
+            self.f_h2muzp = nn.Linear(pre_zp_size, self.z_stochastic_size)
+            self.f_h2logsigzp = nn.Sequential(nn.Linear(pre_zp_size, self.z_stochastic_size),
+                                              MinusOneModule()
+                                              )
+            self.latent_module.append(self.f_h2logsigzp)
+            self.latent_module.append(self.f_h2muzp)
+
+        else:
+            self.f_h2zp = nn.Sequential(nn.Linear(pre_zp_size, self.hidden_layer_width),
+                                        self.forward_act_fn())
+            self.latent_module.append(self.f_h2zp)
+
+        if not self.use_prior_only:
+            oracle_fnns = nn.ModuleList()
+            last_layer_size = self.phi_size_oracle
+            for _ in range(self.half_hidden_layer_depth - 1):
+                oracle_fnns.append(nn.Linear(last_layer_size, self.hidden_layer_width))
+                oracle_fnns.append(self.forward_act_fn())
+                last_layer_size = self.hidden_layer_width
+
+            self.oracle_fnn = nn.Sequential(*oracle_fnns)
+            self.latent_module.append(self.oracle_fnn)
+
+            pre_zq_size = self.hidden_layer_width
+            if self.z_stochastic_size:
+                self.f_hb2muzq = nn.Linear(pre_zq_size, self.z_stochastic_size)
+                self.f_hb2logsigzq = nn.Sequential(nn.Linear(pre_zq_size, self.z_stochastic_size),
+                                                   MinusOneModule())
+                self.latent_module.append(self.f_hb2logsigzq)
+                self.latent_module.append(self.f_hb2muzq)
+            else:
+                self.f_hb2zq = nn.Sequential(nn.Linear(pre_zq_size, self.hidden_layer_width),
+                                             self.forward_act_fn())
+                self.latent_module.append(self.f_hb2zq)
+
+        # ----------------------------- RL part -----------------------------
+        self.alg_config = kwargs["alg_config"] if ("alg_config" in kwargs) else {}
+
+        pre_rl_size = self.z_stochastic_size if self.z_stochastic_size else self.hidden_layer_width
+
+        if self.algorithm == 'ddqn':
+            self.epsilon = kwargs["epsilon"] if ("epsilon" in kwargs) else 0.05
+            self.dueling = self.alg_config["dueling"] if ("dueling" in self.alg_config) else True
+            self.alg_type = 'value_based'
+            self.f_s2q = DiscreteActionQNetwork(pre_rl_size, self.action_size,
+                                                 hidden_layers=[self.hidden_layer_width] * self.half_hidden_layer_depth,
+                                                 dueling=self.dueling, act_fn=self.forward_act_fn)
+
+        elif self.algorithm == 'bc':
+            self.f_s2pi0 = DiscreteActionPolicyNetwork(pre_rl_size, self.action_size,
+                                                       hidden_layers=[self.hidden_layer_width] * self.half_hidden_layer_depth,
+                                                       act_fn=self.forward_act_fn, device=self.device)
+            self.alg_type = 'supervised'
+
+        else:
+            raise NotImplementedError("algorithm can only be 'bc' or 'ddqn'")
+
+
+    def select(self, x, action_mask=None, greedy=True):
+
+        with torch.no_grad():
+
+            if action_mask is not None:
+                action_mask = torch.from_numpy(
+                    action_mask.astype(np.float32).reshape([1, self.action_size]))
+
+            x = torch.from_numpy(x.astype(np.float32).reshape([1, *list(x.shape)])).to(device=self.device)
+
+            x = self.encoder(x)
+            e = self.forward_fnn(x)
+            muz = self.f_h2muzp(e)
+            logsigz = self.f_h2logsigzp(e)
+            dist = dis.normal.Normal(muz, torch.exp(logsigz))
+            z = dist.sample()
+
+            self.h_t = z
+            self.zp_tm1 = z
+
+            if self.algorithm == 'bc':
+
+                a = self.f_s2pi0.sample_action(self.h_t, action_mask=action_mask, greedy=greedy).item()
+
+            elif self.algorithm == 'ddqn':
+                q = self.f_s2q(self.h_t).detach().cpu()
+                if action_mask is not None:
+                    q = q.clamp(-INFINITY, INFINITY) * action_mask - 2 * INFINITY * (1 - action_mask)
+
+                if greedy:
+                    a = torch.argmax(q, dim=-1)
+                    if np.prod(a.shape) == 1:
+                        a = a.item()  # discrete action
+                else:
+                    if np.random.rand() < self.epsilon:
+                        if action_mask is None:
+                            a = np.random.randint(self.action_size)
+                        else:
+                            valid_action_ind = np.nonzero(action_mask.cpu().numpy().reshape([-1]))
+                            valid_actions = np.arange(self.action_size)[valid_action_ind]
+                            a = int(valid_actions[np.random.randint(len(valid_actions))])
+                    else:
+                        a = torch.argmax(q, dim=-1)
+                        if np.prod(a.shape) == 1:
+                            a = int(a.item())  # discrete action
+
+        return a
```

## pymahjong/tenhou_paipu_check.py

```diff
@@ -338,21 +338,22 @@
                 # 骰子数字
                 dice_numbers = [int(child.get("seed").split(",")[3]) + 1, int(child.get("seed").split(",")[4]) + 1]
                 self.log("骰子的数字是", dice_numbers)
 
                 # 牌山
                 inst = mp.TenhouShuffle.instance()
                 yama = inst.generate_yama()
-                #self.log("牌山是: ", yama)
+                self.log("牌山(count={}): ".format(len(yama)), yama)
 
                 # 利用PaiPuReplayer进行重放
                 replayer = mp.PaipuReplayer()
                 if self.write_log:
                     replayer.set_write_log(True)
-                #self.log(f'Replayer.init: {yama} {scores} {riichi_sticks} {honba} {game_order // 4} {oya_id}')
+                
+                self.log(f'Replayer.init: {yama} {scores} {riichi_sticks} {honba} {game_order // 4} {oya_id}')
                 replayer.init(yama, scores, riichi_sticks, honba, game_order // 4, oya_id)
                 #self.log('Init over.')
 
                 # 开局的dora
                 dora_tiles = [int(child.get("seed").split(",")[5])]
                 self.log("开局DORA：{}".format(dora_tiles[-1]))
 
@@ -420,15 +421,15 @@
 
                     if not ret:
                         self.log('phase', int(phase))
                         self.log(f'要打 {get_tile_from_id(discarded_tile)}, Fail.\n')
                             
                         raise ActionException('立直打牌', paipu, game_order, honba)
                 else:                    
-                    selection = replayer.get_selection_from_action(mp.BaseAction.Play, [discarded_tile])
+                    selection = replayer.get_selection_from_action(mp.BaseAction.Discard, [discarded_tile])
                     self.log(f'Select: {selection}')
                     ret = replayer.make_selection(selection)
 
                     if not ret:
                         self.log('phase', int(phase))
                         self.log(f'要打 {get_tile_from_id(discarded_tile)}, Fail.')
                             
@@ -595,15 +596,15 @@
                         raise ActionException('牌局未结束', paipu, game_order, honba)
 
                     result = replayer.get_result()
                     result_score = result.score
                     target_score = [score_changes[i] + scores[i] for i in range(4)]                    
                     result_score_change = [result_score[i] - scores[i] for i in range(4)]    
                     self.log(score_changes1, score_changes2, scores, result_score)
-                    self.log(result.to_string())
+                    # self.log(result.to_string())
                     for i in range(4):
                         if score_changes[i] + scores[i] == result_score[i]:
                             continue
                         else:
                             raise ScoreException(f'Now: {result_score}({result_score_change}) Expect: {target_score}({score_changes}) Original: {scores}', paipu, game_order, honba)
                     
                     self.log('OK!')
@@ -702,20 +703,21 @@
 
     def paipu_replay_1(self, paipu_name, path = None):
         if not path:
             basepath = os.getcwd()
             path = basepath + "/paipuxmls"
         self._paipu_replay(path, paipu_name)
 
-def paipu_replay(path = None, mode = 'debug'):
+def paipu_replay(path = None, write_log = False, mode = 'debug'):
     if mode == 'debug':
         _logger = Logger(fp = 'stdout')
     else:
         _logger = Logger()
     replayer = PaipuReplay()
+    replayer.write_log = write_log
     replayer.logger = _logger
     replayer.paipu_replay(path, mode)
     print(replayer.progress())
     return replayer
 
 def paipu_replay_1(filename, path = None):
     replayer = PaipuReplay()
```

## pymahjong/test.py

```diff
@@ -1,101 +1,102 @@
-import time
-import numpy as np
-from .env_pymahjong import MahjongEnv, SingleAgentMahjongEnv
-
-
-def test(num_games=100):
-
-    env = MahjongEnv()
-
-    start_time = time.time()
-    game = 0
-    success_games = 0
-
-    while game < num_games:
-
-        try:
-
-            env.reset(oya=game % 4, game_wind="east", debug_mode=1)
-
-            while not env.is_over():
-
-                curr_player_id = env.get_curr_player_id()
-
-                # --------- get decision information -------------
-
-                valid_actions_mask = env.get_valid_actions(nhot=True)
-                executor_obs = env.get_obs(curr_player_id)
-
-                # oracle_obs = env.get_oracle_obs(curr_player_id)
-                # full_obs = env.get_full_obs(curr_player_id)
-                # full_obs = np.concatenate([executor_obs, oracle_obs], axis=0)
-
-                # --------- make decision -------------
-
-                a = np.random.choice(np.argwhere(
-                    valid_actions_mask).reshape([-1]))
-
-                env.step(curr_player_id, a)
-
-            # ----------------------- get result ---------------------------------
-
-            payoffs = np.array(env.get_payoffs())
-            print("Game {}, payoffs: {}".format(game, payoffs))
-
-            success_games += 1
-            game += 1
-
-        except Exception as inst:
-            game += 1
-            time.sleep(0.1)
-            print(
-                "-------------- execption in game {} -------------------------".format(game))
-            print(inst)
-            env.render()
-            print("-------------- replayable log -------------------------------")
-            env.t.print_debug_replay()
-            continue
-
-    print("Total {} random-play games, {} games without error, takes {} s".format(
-        num_games, success_games, time.time() - start_time))
-
-
-def test_with_pretrained(opponent_agent, num_games=100):
-    
-    env = SingleAgentMahjongEnv(opponent_agent)
-
-    start_time = time.time()
-    success_games = 0
-
-    for game in range(num_games):
-
-        try:
-            env.reset()
-            payoff = 0
-
-            while True:
-
-                valid_actions = env.get_valid_actions()
-
-                a = np.random.choice(valid_actions)
-
-                obs, reward, done, _ = env.step(a)
-
-                payoff = payoff + reward  # reward may != 0 only when done
-
-                if done:
-                    success_games += 1
-                    print("Game {}, agent payoff {}".format(game, payoff))
-                    break
-
-        except Exception as inst:
-            game += 1
-            time.sleep(0.1)
-            print(
-                "-------------- execption in game {} -------------------------".format(game))
-            print(inst)
-            env.render()
-            continue
-
-    print("Total {} random-play games with pretrained VLOG models as opponents, {} games without error, takes {} s".format(
-        num_games, success_games, time.time() - start_time))
+import time
+import numpy as np
+from .env_pymahjong import MahjongEnv, SingleAgentMahjongEnv
+
+
+def test(num_games=100):
+
+    env = MahjongEnv()
+
+    start_time = time.time()
+    game = 0
+    success_games = 0
+
+    while game < num_games:
+
+        try:
+
+            env.reset(oya=game % 4, game_wind="east", debug_mode=1)
+
+            while not env.is_over():
+
+                curr_player_id = env.get_curr_player_id()
+
+                # --------- get decision information -------------
+
+                valid_actions_mask = env.get_valid_actions(nhot=True)
+                executor_obs = env.get_obs(curr_player_id)
+
+                # oracle_obs = env.get_oracle_obs(curr_player_id)
+                # full_obs = env.get_full_obs(curr_player_id)
+                # full_obs = np.concatenate([executor_obs, oracle_obs], axis=0)
+
+                # --------- make decision -------------
+
+                a = np.random.choice(np.argwhere(
+                    valid_actions_mask).reshape([-1]))
+
+                env.step(curr_player_id, a)
+
+            # ----------------------- get result ---------------------------------
+
+            payoffs = np.array(env.get_payoffs())
+            print("Game {}, payoffs: {}".format(game, payoffs))
+            # env.render()
+
+            success_games += 1
+            game += 1
+
+        except Exception as inst:
+            game += 1
+            time.sleep(0.1)
+            print(
+                "-------------- execption in game {} -------------------------".format(game))
+            print(inst)
+            env.render()
+            print("-------------- replayable log -------------------------------")
+            env.t.print_debug_replay()
+            continue
+
+    print("Total {} random-play games, {} games without error, takes {} s".format(
+        num_games, success_games, time.time() - start_time))
+
+
+def test_with_pretrained(opponent_agent, num_games=100):
+    
+    env = SingleAgentMahjongEnv(opponent_agent)
+
+    start_time = time.time()
+    success_games = 0
+
+    for game in range(num_games):
+
+        try:
+            env.reset()
+            payoff = 0
+
+            while True:
+
+                valid_actions = env.get_valid_actions()
+
+                a = np.random.choice(valid_actions)
+
+                obs, reward, done, _ = env.step(a)
+
+                payoff = payoff + reward  # reward may != 0 only when done
+
+                if done:
+                    success_games += 1
+                    print("Game {}, agent payoff {}".format(game, payoff))
+                    break
+
+        except Exception as inst:
+            game += 1
+            time.sleep(0.1)
+            print(
+                "-------------- execption in game {} -------------------------".format(game))
+            print(inst)
+            env.render()
+            continue
+
+    print("Total {} random-play games with pretrained VLOG models as opponents, {} games without error, takes {} s".format(
+        num_games, success_games, time.time() - start_time))
```

## Comparing `pymahjong-1.0.2.dist-info/METADATA` & `pymahjong-1.0.3.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pymahjong
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Japanese Mahjong environment for decision AI research.
 Author: Agony
 Author-email: chenzhaoyun@iai.ustc.edu.cn
-License: UNKNOWN
 Project-URL: Source Code, https://github.com/Agony5757/mahjong
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -30,33 +28,34 @@
 Requires-Dist: gym
 
 
 # Japanese Riichi Mahjong
 
 [![PyPI version](https://badge.fury.io/py/pymahjong.svg)](https://badge.fury.io/py/pymahjong)
 
-|Branch| Build | Code Analysis |
-|:----:|:----:|:----:|
-|master|[![Build-and-test](https://github.com/Agony5757/mahjong/actions/workflows/build-and-test.yml/badge.svg?branch=master)](https://github.com/Agony5757/mahjong/actions/workflows/build-and-test.yml)|[![Microsoft C++ Code Analysis](https://github.com/Agony5757/mahjong/actions/workflows/msvc.yml/badge.svg?branch=master)](https://github.com/Agony5757/mahjong/actions/workflows/msvc.yml)|
-|develop|[![Build-and-test](https://github.com/Agony5757/mahjong/actions/workflows/build-and-test.yml/badge.svg?branch=develop)](https://github.com/Agony5757/mahjong/actions/workflows/build-and-test.yml)|[![Microsoft C++ Code Analysis](https://github.com/Agony5757/mahjong/actions/workflows/msvc.yml/badge.svg?branch=develop)](https://github.com/Agony5757/mahjong/actions/workflows/msvc.yml)|
+|Branch| Build |
+|:----:|:----:|
+|master|[![Build-and-test](https://github.com/Agony5757/mahjong/actions/workflows/build-and-test.yml/badge.svg?branch=master)](https://github.com/Agony5757/mahjong/actions/workflows/build-and-test.yml)|
+|develop|[![Build-and-test](https://github.com/Agony5757/mahjong/actions/workflows/build-and-test.yml/badge.svg?branch=develop)](https://github.com/Agony5757/mahjong/actions/workflows/build-and-test.yml)|
 
 Simulator of Japanese Riichi Mahjong (https://en.wikipedia.org/wiki/Japanese_Mahjong) written in C++. [关于C++部分的说明（中文版）](https://github.com/Agony5757/mahjong/blob/master/%E8%AF%BB%E6%88%91.md)
 
 
 # See [here](https://github.com/Agony5757/mahjong/tree/master/pymahjong) for the Python APIs for e.g., decision AI research.
 
 
-
 ## Citation
 ```
 @inproceedings{
 han2022variational,
 title={Variational oracle guiding for reinforcement learning},
 author={Dongqi Han and Tadashi Kozuno and Xufang Luo and Zhao-Yun Chen and Kenji Doya and Yuqing Yang and Dongsheng Li},
 booktitle={International Conference on Learning Representations},
 year={2022},
 url={https://openreview.net/forum?id=pjqqxepwoMy}
 }
 ```
 
+## Contact us
 
-
+Email:    hdqhdq58@outlook.com
+QQ group: 608064044
```

