# Comparing `tmp/joyrl-0.6.0.2.tar.gz` & `tmp/joyrl-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joyrl-0.6.0.2.tar", last modified: Sat Jun  1 09:20:51 2024, max compression
+gzip compressed data, was "joyrl-0.6.1.tar", last modified: Sat Jun  1 16:28:17 2024, max compression
```

## Comparing `joyrl-0.6.0.2.tar` & `joyrl-0.6.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.190507 joyrl-0.6.0.2/
--rw-r--r--   0 johnjim    (501) staff       (20)     1077 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/LICENSE
--rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-01 09:20:51.190405 joyrl-0.6.0.2/PKG-INFO
--rw-r--r--   0 johnjim    (501) staff       (20)    10670 2024-06-01 08:59:02.000000 joyrl-0.6.0.2/README.md
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.179150 joyrl-0.6.0.2/joyrl/
--rw-r--r--   0 johnjim    (501) staff       (20)      377 2024-06-01 09:19:57.000000 joyrl-0.6.0.2/joyrl/__init__.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.180176 joyrl-0.6.0.2/joyrl/algos/
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.180736 joyrl-0.6.0.2/joyrl/algos/DDPG/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DDPG/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1517 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DDPG/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      152 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DDPG/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     5540 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DDPG/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.181224 joyrl-0.6.0.2/joyrl/algos/DQN/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1950 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      158 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3507 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.181714 joyrl-0.6.0.2/joyrl/algos/DoubleDQN/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DoubleDQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1703 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DoubleDQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      350 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DoubleDQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3696 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DoubleDQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.182189 joyrl-0.6.0.2/joyrl/algos/DuelingDQN/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DuelingDQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      907 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DuelingDQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      337 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DuelingDQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3948 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DuelingDQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.182640 joyrl-0.6.0.2/joyrl/algos/NoisyDQN/
--rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/NoisyDQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1071 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/NoisyDQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      341 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/NoisyDQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     4445 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/NoisyDQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.183125 joyrl-0.6.0.2/joyrl/algos/PPO/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/PPO/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2071 2024-05-09 17:05:41.000000 joyrl-0.6.0.2/joyrl/algos/PPO/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2979 2024-06-01 09:19:48.000000 joyrl-0.6.0.2/joyrl/algos/PPO/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     9208 2024-05-27 16:17:38.000000 joyrl-0.6.0.2/joyrl/algos/PPO/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.183583 joyrl-0.6.0.2/joyrl/algos/QLearning/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/QLearning/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/QLearning/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.0.2/joyrl/algos/QLearning/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1964 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/QLearning/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.184073 joyrl-0.6.0.2/joyrl/algos/Sarsa/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/Sarsa/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/Sarsa/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.0.2/joyrl/algos/Sarsa/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2144 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/Sarsa/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.184519 joyrl-0.6.0.2/joyrl/algos/TD3/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/TD3/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1277 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/TD3/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      153 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/TD3/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     7726 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/TD3/policy.py
--rw-r--r--   0 johnjim    (501) staff       (20)      366 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/__init__.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.185981 joyrl-0.6.0.2/joyrl/algos/base/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/base/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)    10713 2024-05-26 12:17:32.000000 joyrl-0.6.0.2/joyrl/algos/base/action_layer.py
--rw-r--r--   0 johnjim    (501) staff       (20)     8643 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/base/base_layer.py
--rw-r--r--   0 johnjim    (501) staff       (20)    86089 2024-06-01 05:31:25.000000 joyrl-0.6.0.2/joyrl/algos/base/buffer.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2755 2024-06-01 05:12:03.000000 joyrl-0.6.0.2/joyrl/algos/base/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)      131 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/base/experience.py
--rw-r--r--   0 johnjim    (501) staff       (20)    14978 2024-05-27 01:50:26.000000 joyrl-0.6.0.2/joyrl/algos/base/network.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1313 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/base/noise.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2407 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/base/optm.py
--rw-r--r--   0 johnjim    (501) staff       (20)     7605 2024-05-27 15:36:54.000000 joyrl-0.6.0.2/joyrl/algos/base/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.187120 joyrl-0.6.0.2/joyrl/envs/
--rw-r--r--   0 johnjim    (501) staff       (20)       51 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     4258 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/blackjack.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2706 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/cliff_walking.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3871 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/gridworld.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3485 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/gridworld_env.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.187485 joyrl-0.6.0.2/joyrl/envs/gym/
--rw-r--r--   0 johnjim    (501) staff       (20)      221 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/gym/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      525 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/gym/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)    11068 2024-05-09 16:41:09.000000 joyrl-0.6.0.2/joyrl/envs/gym/wrappers.py
--rw-r--r--   0 johnjim    (501) staff       (20)     9890 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/racetrack.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1445 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/register.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1311 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/stochastic_mdp.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2615 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/windy_gridworld.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.189026 joyrl-0.6.0.2/joyrl/framework/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/framework/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1069 2024-05-30 09:43:52.000000 joyrl-0.6.0.2/joyrl/framework/base.py
--rw-r--r--   0 johnjim    (501) staff       (20)     4442 2024-06-01 08:53:39.000000 joyrl-0.6.0.2/joyrl/framework/collector.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2294 2024-06-01 06:35:14.000000 joyrl-0.6.0.2/joyrl/framework/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     5619 2024-06-01 08:53:09.000000 joyrl-0.6.0.2/joyrl/framework/interactor.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2874 2024-06-01 08:53:20.000000 joyrl-0.6.0.2/joyrl/framework/learner.py
--rw-r--r--   0 johnjim    (501) staff       (20)      821 2024-05-28 01:37:10.000000 joyrl-0.6.0.2/joyrl/framework/message.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2923 2024-06-01 03:33:53.000000 joyrl-0.6.0.2/joyrl/framework/policy_mgr.py
--rw-r--r--   0 johnjim    (501) staff       (20)     5272 2024-05-30 09:48:58.000000 joyrl-0.6.0.2/joyrl/framework/recorder.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3961 2024-05-31 03:30:30.000000 joyrl-0.6.0.2/joyrl/framework/tester.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2242 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/framework/tracker.py
--rw-r--r--   0 johnjim    (501) staff       (20)     7020 2024-06-01 08:53:33.000000 joyrl-0.6.0.2/joyrl/framework/trainer.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2524 2024-05-31 14:51:57.000000 joyrl-0.6.0.2/joyrl/framework/utils.py
--rw-r--r--   0 johnjim    (501) staff       (20)     8002 2024-06-01 09:17:47.000000 joyrl-0.6.0.2/joyrl/run.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.189256 joyrl-0.6.0.2/joyrl/scripts/
--rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/scripts/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      520 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/scripts/scripts.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.189583 joyrl-0.6.0.2/joyrl/utils/
--rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/utils/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/utils/plot.py
--rw-r--r--   0 johnjim    (501) staff       (20)    37181 2024-05-30 09:48:17.000000 joyrl-0.6.0.2/joyrl/utils/utils.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.189837 joyrl-0.6.0.2/joyrl.egg-info/
--rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-01 09:20:51.000000 joyrl-0.6.0.2/joyrl.egg-info/PKG-INFO
--rw-r--r--   0 johnjim    (501) staff       (20)     2455 2024-06-01 09:20:51.000000 joyrl-0.6.0.2/joyrl.egg-info/SOURCES.txt
--rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-06-01 09:20:51.000000 joyrl-0.6.0.2/joyrl.egg-info/dependency_links.txt
--rw-r--r--   0 johnjim    (501) staff       (20)       53 2024-06-01 09:20:51.000000 joyrl-0.6.0.2/joyrl.egg-info/entry_points.txt
--rw-r--r--   0 johnjim    (501) staff       (20)      256 2024-06-01 09:20:51.000000 joyrl-0.6.0.2/joyrl.egg-info/requires.txt
--rw-r--r--   0 johnjim    (501) staff       (20)        6 2024-06-01 09:20:51.000000 joyrl-0.6.0.2/joyrl.egg-info/top_level.txt
--rw-r--r--   0 johnjim    (501) staff       (20)      940 2024-06-01 09:20:51.190828 joyrl-0.6.0.2/setup.cfg
--rw-r--r--   0 johnjim    (501) staff       (20)     1886 2024-06-01 09:01:11.000000 joyrl-0.6.0.2/setup.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.637101 joyrl-0.6.1/
+-rw-r--r--   0 johnjim    (501) staff       (20)     1077 2024-02-25 07:46:04.000000 joyrl-0.6.1/LICENSE
+-rw-r--r--   0 johnjim    (501) staff       (20)    11637 2024-06-01 16:28:17.637005 joyrl-0.6.1/PKG-INFO
+-rw-r--r--   0 johnjim    (501) staff       (20)    10670 2024-06-01 08:59:02.000000 joyrl-0.6.1/README.md
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.621262 joyrl-0.6.1/joyrl/
+-rw-r--r--   0 johnjim    (501) staff       (20)      375 2024-06-01 16:28:07.000000 joyrl-0.6.1/joyrl/__init__.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.622270 joyrl-0.6.1/joyrl/algos/
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.623082 joyrl-0.6.1/joyrl/algos/DDPG/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DDPG/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1517 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DDPG/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      152 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DDPG/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5540 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DDPG/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.623720 joyrl-0.6.1/joyrl/algos/DQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1950 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      158 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3519 2024-06-01 16:19:56.000000 joyrl-0.6.1/joyrl/algos/DQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.624266 joyrl-0.6.1/joyrl/algos/DoubleDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DoubleDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1703 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DoubleDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      350 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DoubleDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3696 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DoubleDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.624906 joyrl-0.6.1/joyrl/algos/DuelingDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DuelingDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      907 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DuelingDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      337 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DuelingDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3948 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/DuelingDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.625500 joyrl-0.6.1/joyrl/algos/NoisyDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/NoisyDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1071 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/NoisyDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      341 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/NoisyDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4445 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/NoisyDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.626554 joyrl-0.6.1/joyrl/algos/PPO/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/PPO/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2071 2024-05-09 17:05:41.000000 joyrl-0.6.1/joyrl/algos/PPO/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2979 2024-06-01 09:19:48.000000 joyrl-0.6.1/joyrl/algos/PPO/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     6921 2024-06-01 10:23:56.000000 joyrl-0.6.1/joyrl/algos/PPO/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.627293 joyrl-0.6.1/joyrl/algos/QLearning/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/QLearning/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/QLearning/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.1/joyrl/algos/QLearning/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1964 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/QLearning/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.627889 joyrl-0.6.1/joyrl/algos/Sarsa/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/Sarsa/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/Sarsa/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.1/joyrl/algos/Sarsa/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2144 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/Sarsa/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.628365 joyrl-0.6.1/joyrl/algos/TD3/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/TD3/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1277 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/TD3/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      153 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/TD3/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7726 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/TD3/policy.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      366 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/__init__.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.630721 joyrl-0.6.1/joyrl/algos/base/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/base/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    10114 2024-06-01 16:17:16.000000 joyrl-0.6.1/joyrl/algos/base/action_layer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     8643 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/base/base_layer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    86089 2024-06-01 05:31:25.000000 joyrl-0.6.1/joyrl/algos/base/buffer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2755 2024-06-01 05:12:03.000000 joyrl-0.6.1/joyrl/algos/base/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      131 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/base/experience.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    13933 2024-06-01 16:11:14.000000 joyrl-0.6.1/joyrl/algos/base/network.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1313 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/base/noise.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2407 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/algos/base/optm.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7635 2024-06-01 16:21:28.000000 joyrl-0.6.1/joyrl/algos/base/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.632256 joyrl-0.6.1/joyrl/envs/
+-rw-r--r--   0 johnjim    (501) staff       (20)       51 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4258 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/blackjack.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2706 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/cliff_walking.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3871 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/gridworld.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3485 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/gridworld_env.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.632703 joyrl-0.6.1/joyrl/envs/gym/
+-rw-r--r--   0 johnjim    (501) staff       (20)      221 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/gym/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      525 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/gym/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    11068 2024-05-09 16:41:09.000000 joyrl-0.6.1/joyrl/envs/gym/wrappers.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     9890 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/racetrack.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1445 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/register.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1311 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/stochastic_mdp.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2615 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/envs/windy_gridworld.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.635296 joyrl-0.6.1/joyrl/framework/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/framework/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1069 2024-05-30 09:43:52.000000 joyrl-0.6.1/joyrl/framework/base.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4442 2024-06-01 08:53:39.000000 joyrl-0.6.1/joyrl/framework/collector.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2294 2024-06-01 06:35:14.000000 joyrl-0.6.1/joyrl/framework/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5619 2024-06-01 08:53:09.000000 joyrl-0.6.1/joyrl/framework/interactor.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2874 2024-06-01 08:53:20.000000 joyrl-0.6.1/joyrl/framework/learner.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      821 2024-05-28 01:37:10.000000 joyrl-0.6.1/joyrl/framework/message.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2923 2024-06-01 03:33:53.000000 joyrl-0.6.1/joyrl/framework/policy_mgr.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5272 2024-05-30 09:48:58.000000 joyrl-0.6.1/joyrl/framework/recorder.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3961 2024-05-31 03:30:30.000000 joyrl-0.6.1/joyrl/framework/tester.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2242 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/framework/tracker.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7020 2024-06-01 08:53:33.000000 joyrl-0.6.1/joyrl/framework/trainer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2524 2024-05-31 14:51:57.000000 joyrl-0.6.1/joyrl/framework/utils.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     8002 2024-06-01 09:17:47.000000 joyrl-0.6.1/joyrl/run.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.635790 joyrl-0.6.1/joyrl/scripts/
+-rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/scripts/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      520 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/scripts/scripts.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.636298 joyrl-0.6.1/joyrl/utils/
+-rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/utils/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.1/joyrl/utils/plot.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    37181 2024-05-30 09:48:17.000000 joyrl-0.6.1/joyrl/utils/utils.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 16:28:17.636509 joyrl-0.6.1/joyrl.egg-info/
+-rw-r--r--   0 johnjim    (501) staff       (20)    11637 2024-06-01 16:28:17.000000 joyrl-0.6.1/joyrl.egg-info/PKG-INFO
+-rw-r--r--   0 johnjim    (501) staff       (20)     2455 2024-06-01 16:28:17.000000 joyrl-0.6.1/joyrl.egg-info/SOURCES.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-06-01 16:28:17.000000 joyrl-0.6.1/joyrl.egg-info/dependency_links.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)       53 2024-06-01 16:28:17.000000 joyrl-0.6.1/joyrl.egg-info/entry_points.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)      256 2024-06-01 16:28:17.000000 joyrl-0.6.1/joyrl.egg-info/requires.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)        6 2024-06-01 16:28:17.000000 joyrl-0.6.1/joyrl.egg-info/top_level.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)      940 2024-06-01 16:28:17.637437 joyrl-0.6.1/setup.cfg
+-rw-r--r--   0 johnjim    (501) staff       (20)     1886 2024-06-01 09:01:11.000000 joyrl-0.6.1/setup.py
```

### Comparing `joyrl-0.6.0.2/LICENSE` & `joyrl-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/PKG-INFO` & `joyrl-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.6.0.2
+Version: 0.6.1
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.6.0.2/README.md` & `joyrl-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/DDPG/config.py` & `joyrl-0.6.1/joyrl/algos/DDPG/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/DDPG/policy.py` & `joyrl-0.6.1/joyrl/algos/DDPG/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/DQN/config.py` & `joyrl-0.6.1/joyrl/algos/DQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/DQN/policy.py` & `joyrl-0.6.1/joyrl/algos/DoubleDQN/policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,90 +1,92 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
-Date: 2024-01-25 09:58:33
+Date: 2023-12-22 23:02:13
 LastEditor: JiangJi
-LastEditTime: 2024-01-27 11:59:15
+LastEditTime: 2024-01-27 12:00:29
 Discription: 
 '''
 import torch
 import torch.nn as nn
-import math,random
+import math, random
 import numpy as np
 from joyrl.algos.base.policy import BasePolicy
 from joyrl.algos.base.network import QNetwork
-
 class Policy(BasePolicy):
     def __init__(self,cfg) -> None:
         super(Policy, self).__init__(cfg)
         self.cfg = cfg
+        self.obs_space = cfg.obs_space
+        self.action_space = cfg.action_space
         self.gamma = cfg.gamma  
         # e-greedy parameters
         self.epsilon_start = cfg.epsilon_start
         self.epsilon_end = cfg.epsilon_end
         self.epsilon_decay = cfg.epsilon_decay
         self.target_update = cfg.target_update
         self.sample_count = 0
         self.update_step = 0
         self.create_graph() # create graph and optimizer
         self.create_summary() # create summary
-        self.to(self.device)
-        
-    def create_graph(self):
 
+    def create_graph(self):
         self.policy_net = QNetwork(self.cfg,self.state_size_list).to(self.device)
         self.target_net = QNetwork(self.cfg,self.state_size_list).to(self.device)
         self.target_net.load_state_dict(self.policy_net.state_dict()) # or use this to copy parameters
         self.create_optimizer()
 
-    def sample_action(self, state,  **kwargs):
+    def sample_action(self, state, **kwargs):
         ''' sample action
         '''
         # epsilon must decay(linear,exponential and etc.) for balancing exploration and exploitation
         self.sample_count += 1
         self.epsilon = self.epsilon_end + (self.epsilon_start - self.epsilon_end) * \
             math.exp(-1. * self.sample_count / self.epsilon_decay) 
         if random.random() > self.epsilon:
-            # before update, the network inference time may be longer
-            action = self.predict_action(state) 
+            action = self.predict_action(state)
         else:
             action = [self.action_space.sample()]
         return action
     
     @torch.no_grad()
-    def predict_action(self,state, **kwargs):
+    def predict_action(self,state,**kwargs):
         ''' predict action
         '''
         state = [torch.tensor(np.array(state), device=self.device, dtype=torch.float32).unsqueeze(dim=0)]
         _ = self.policy_net(state)
         actions = self.policy_net.action_layers.get_actions()
         return actions
-    
+
     def learn(self, **kwargs):
-        ''' learn policy
+        ''' train policy
         '''
         states, actions, next_states, rewards, dones = kwargs.get('states'), kwargs.get('actions'), kwargs.get('next_states'), kwargs.get('rewards'), kwargs.get('dones')
-        # compute current Q values
         _ = self.policy_net(states)
         q_values = self.policy_net.action_layers.get_qvalues()
         actual_qvalues = q_values.gather(1, actions.long())
-        # compute next max q value
+
+        # compute next Q values Q(s_t+1, a)
+        _ = self.policy_net(next_states)
+        next_q_values = self.policy_net.action_layers.get_qvalues()
+
+        # compute next target Q values Q'(s_t+1, a)，which is different from DQN
         _ = self.target_net(next_states)
-        next_q_values_max = self.target_net.action_layers.get_qvalues().max(1)[0].unsqueeze(dim=1)
-        # compute target Q values
-        target_q_values = rewards + (1 - dones) * self.gamma * next_q_values_max
-        # compute loss
-        self.loss = nn.MSELoss()(actual_qvalues, target_q_values)
-        self.optimizer.zero_grad()
-        self.loss.backward()
+        next_target_qvalues = self.target_net.action_layers.get_qvalues()
+
+        next_target_q_values_action = next_target_qvalues.gather(1, torch.max(next_q_values, 1)[1].unsqueeze(1))
+
+        expected_q_values = rewards + self.gamma * next_target_q_values_action * (1 - dones)  
+        self.loss = nn.MSELoss()(actual_qvalues, expected_q_values)  
+        self.optimizer.zero_grad()  
+        self.loss.backward()  
         # clip to avoid gradient explosion
         for param in self.policy_net.parameters():
             param.grad.data.clamp_(-1, 1)
         self.optimizer.step()
         # update target net every C steps
         if self.update_step % self.target_update == 0: 
             self.target_net.load_state_dict(self.policy_net.state_dict())
         self.update_step += 1
-        self.update_summary() # update summary
- 
+        self.update_summary() # update summary
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `joyrl-0.6.0.2/joyrl/algos/DoubleDQN/config.py` & `joyrl-0.6.1/joyrl/algos/DoubleDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/DoubleDQN/policy.py` & `joyrl-0.6.1/joyrl/algos/DuelingDQN/policy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
-Date: 2023-12-22 23:02:13
+Date: 2022-11-14 23:50:59
 LastEditor: JiangJi
-LastEditTime: 2024-01-27 12:00:29
+LastEditTime: 2023-12-24 20:35:14
 Discription: 
 '''
 import torch
 import torch.nn as nn
-import math, random
+import math,random
 import numpy as np
 from joyrl.algos.base.policy import BasePolicy
 from joyrl.algos.base.network import QNetwork
+        
 class Policy(BasePolicy):
     def __init__(self,cfg) -> None:
         super(Policy, self).__init__(cfg)
         self.cfg = cfg
-        self.obs_space = cfg.obs_space
-        self.action_space = cfg.action_space
         self.gamma = cfg.gamma  
         # e-greedy parameters
         self.epsilon_start = cfg.epsilon_start
         self.epsilon_end = cfg.epsilon_end
         self.epsilon_decay = cfg.epsilon_decay
         self.target_update = cfg.target_update
         self.sample_count = 0
         self.update_step = 0
         self.create_graph() # create graph and optimizer
         self.create_summary() # create summary
+        self.to(self.device)
 
     def create_graph(self):
-        self.policy_net = QNetwork(self.cfg,self.state_size_list).to(self.device)
-        self.target_net = QNetwork(self.cfg,self.state_size_list).to(self.device)
+        self.state_size_list, self.action_size_list = self.get_state_action_size()
+        self.policy_net = QNetwork(self.cfg, self.state_size_list, self.action_size_list).to(self.device)
+        self.target_net = QNetwork(self.cfg, self.state_size_list, self.action_size_list).to(self.device)
         self.target_net.load_state_dict(self.policy_net.state_dict()) # or use this to copy parameters
         self.create_optimizer()
 
-    def sample_action(self, state, **kwargs):
+    def sample_action(self, state,  **kwargs):
         ''' sample action
         '''
         # epsilon must decay(linear,exponential and etc.) for balancing exploration and exploitation
         self.sample_count += 1
         self.epsilon = self.epsilon_end + (self.epsilon_start - self.epsilon_end) * \
             math.exp(-1. * self.sample_count / self.epsilon_decay) 
         if random.random() > self.epsilon:
             action = self.predict_action(state)
         else:
-            action = [self.action_space.sample()]
+            action = self.action_space.sample()
         return action
     
-    @torch.no_grad()
-    def predict_action(self,state,**kwargs):
+    def predict_action(self,state, **kwargs):
         ''' predict action
         '''
-        state = [torch.tensor(np.array(state), device=self.device, dtype=torch.float32).unsqueeze(dim=0)]
-        _ = self.policy_net(state)
-        actions = self.policy_net.action_layers.get_actions()
-        return actions
-
+        with torch.no_grad():
+            state = torch.tensor(np.array(state), device=self.device, dtype=torch.float32).unsqueeze(dim=0)
+            q_values = self.policy_net(state)
+            action = q_values.max(1)[1].item() # choose action corresponding to the maximum q value
+        return action  
+    
     def learn(self, **kwargs):
         ''' train policy
         '''
         states, actions, next_states, rewards, dones = kwargs.get('states'), kwargs.get('actions'), kwargs.get('next_states'), kwargs.get('rewards'), kwargs.get('dones')
-        _ = self.policy_net(states)
-        q_values = self.policy_net.action_layers.get_qvalues()
-        actual_qvalues = q_values.gather(1, actions.long())
-
-        # compute next Q values Q(s_t+1, a)
-        _ = self.policy_net(next_states)
-        next_q_values = self.policy_net.action_layers.get_qvalues()
-
-        # compute next target Q values Q'(s_t+1, a)，which is different from DQN
-        _ = self.target_net(next_states)
-        next_target_qvalues = self.target_net.action_layers.get_qvalues()
-
-        next_target_q_values_action = next_target_qvalues.gather(1, torch.max(next_q_values, 1)[1].unsqueeze(1))
-
-        expected_q_values = rewards + self.gamma * next_target_q_values_action * (1 - dones)  
-        self.loss = nn.MSELoss()(actual_qvalues, expected_q_values)  
-        self.optimizer.zero_grad()  
-        self.loss.backward()  
+        # convert numpy to tensor
+        states = torch.tensor(states, device=self.device, dtype=torch.float32)
+        actions = torch.tensor(actions, device=self.device, dtype=torch.int64).unsqueeze(dim=1)
+        next_states = torch.tensor(next_states, device=self.device, dtype=torch.float32)
+        rewards = torch.tensor(rewards, device=self.device, dtype=torch.float32).unsqueeze(dim=1)
+        dones = torch.tensor(dones, device=self.device, dtype=torch.float32).unsqueeze(dim=1)
+        # compute current Q values
+        q_values = self.policy_net(states).gather(1, actions)
+        # compute next max q value
+        next_q_values = self.target_net(next_states).max(1)[0].unsqueeze(dim=1)
+        # compute target Q values
+        target_q_values = rewards + (1 - dones) * self.gamma * next_q_values
+        # compute loss
+        self.loss = nn.MSELoss()(q_values, target_q_values)
+        self.optimizer.zero_grad()
+        self.loss.backward()
         # clip to avoid gradient explosion
         for param in self.policy_net.parameters():
             param.grad.data.clamp_(-1, 1)
         self.optimizer.step()
         # update target net every C steps
         if self.update_step % self.target_update == 0: 
             self.target_net.load_state_dict(self.policy_net.state_dict())
         self.update_step += 1
-        self.update_summary() # update summary
+        self.update_summary() # update summary
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `joyrl-0.6.0.2/joyrl/algos/DuelingDQN/config.py` & `joyrl-0.6.1/joyrl/algos/DuelingDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/DuelingDQN/policy.py` & `joyrl-0.6.1/joyrl/algos/NoisyDQN/policy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,85 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
-Date: 2022-11-14 23:50:59
+Date: 2023-04-17 11:23:49
 LastEditor: JiangJi
-LastEditTime: 2023-12-24 20:35:14
+LastEditTime: 2023-12-25 00:18:41
 Discription: 
 '''
 import torch
 import torch.nn as nn
-import math,random
+import torch.optim as optim
+import torch.nn.functional as F
 import numpy as np
+import math
+import random
+
 from joyrl.algos.base.policy import BasePolicy
 from joyrl.algos.base.network import QNetwork
-        
+
 class Policy(BasePolicy):
     def __init__(self,cfg) -> None:
         super(Policy, self).__init__(cfg)
         self.cfg = cfg
+        self.device = torch.device(cfg.device) 
         self.gamma = cfg.gamma  
         # e-greedy parameters
         self.epsilon_start = cfg.epsilon_start
         self.epsilon_end = cfg.epsilon_end
         self.epsilon_decay = cfg.epsilon_decay
+        self.batch_size = cfg.batch_size
         self.target_update = cfg.target_update
         self.sample_count = 0
         self.update_step = 0
         self.create_graph() # create graph and optimizer
         self.create_summary() # create summary
-        self.to(self.device)
 
     def create_graph(self):
         self.state_size_list, self.action_size_list = self.get_state_action_size()
         self.policy_net = QNetwork(self.cfg, self.state_size_list, self.action_size_list).to(self.device)
         self.target_net = QNetwork(self.cfg, self.state_size_list, self.action_size_list).to(self.device)
         self.target_net.load_state_dict(self.policy_net.state_dict()) # or use this to copy parameters
+        # for noise parameters
+        # if self.cfg.mode == 'train': 
+        #     self.policy_net.train()
+        #     self.target_net.train()
+        # elif self.cfg.mode == 'test':
+        #     self.policy_net.eval()
+        #     self.target_net.eval()
         self.create_optimizer()
 
     def sample_action(self, state,  **kwargs):
         ''' sample action
         '''
         # epsilon must decay(linear,exponential and etc.) for balancing exploration and exploitation
         self.sample_count += 1
         self.epsilon = self.epsilon_end + (self.epsilon_start - self.epsilon_end) * \
             math.exp(-1. * self.sample_count / self.epsilon_decay) 
         if random.random() > self.epsilon:
             action = self.predict_action(state)
         else:
             action = self.action_space.sample()
         return action
-    
     def predict_action(self,state, **kwargs):
         ''' predict action
         '''
         with torch.no_grad():
             state = torch.tensor(np.array(state), device=self.device, dtype=torch.float32).unsqueeze(dim=0)
             q_values = self.policy_net(state)
             action = q_values.max(1)[1].item() # choose action corresponding to the maximum q value
         return action  
-    
+
     def learn(self, **kwargs):
         ''' train policy
         '''
         states, actions, next_states, rewards, dones = kwargs.get('states'), kwargs.get('actions'), kwargs.get('next_states'), kwargs.get('rewards'), kwargs.get('dones')
+        update_step = kwargs.get('update_step')
         # convert numpy to tensor
         states = torch.tensor(states, device=self.device, dtype=torch.float32)
         actions = torch.tensor(actions, device=self.device, dtype=torch.int64).unsqueeze(dim=1)
         next_states = torch.tensor(next_states, device=self.device, dtype=torch.float32)
         rewards = torch.tensor(rewards, device=self.device, dtype=torch.float32).unsqueeze(dim=1)
         dones = torch.tensor(dones, device=self.device, dtype=torch.float32).unsqueeze(dim=1)
         # compute current Q values
@@ -84,9 +96,11 @@
         for param in self.policy_net.parameters():
             param.grad.data.clamp_(-1, 1)
         self.optimizer.step()
         # update target net every C steps
         if self.update_step % self.target_update == 0: 
             self.target_net.load_state_dict(self.policy_net.state_dict())
         self.update_step += 1
+        self.policy_net.reset_noise()
+        self.target_net.reset_noise()
         self.update_summary() # update summary
- 
+
```

### Comparing `joyrl-0.6.0.2/joyrl/algos/NoisyDQN/config.py` & `joyrl-0.6.1/joyrl/algos/NoisyDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/PPO/config.py` & `joyrl-0.6.1/joyrl/algos/PPO/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/PPO/data_handler.py` & `joyrl-0.6.1/joyrl/algos/PPO/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/PPO/policy.py` & `joyrl-0.6.1/joyrl/algos/PPO/policy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,26 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-22 23:02:13
 LastEditor: JiangJi
-LastEditTime: 2024-05-28 00:17:20
+LastEditTime: 2024-06-01 18:23:54
 Discription: 
 '''
-import copy
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
 import torch.optim as optim
-from torch.distributions import Categorical,Normal
 import torch.utils.data as Data
 import numpy as np
 from joyrl.algos.base.network import ActorCriticNetwork, CriticNetwork, ActorNetwork
 from joyrl.algos.base.policy import BasePolicy
 from joyrl.framework.config import MergedConfig
 
-import torch.nn as nn
-import torch.optim as optim
-import torch.nn.functional as F
-from torch.distributions import Normal
-
-def init_linear_weights(m):
-    if isinstance(m, nn.Linear):
-        nn.init.normal_(m.weight, mean=0., std=0.1)
-        nn.init.constant_(m.bias, 0.1)
-
-class Model(nn.Module):
-    def __init__(self, input_dim, output_dim, hidden_dim, std=0.0):
-        super(Model, self).__init__()
-        
-        self.critic = nn.Sequential(
-            nn.Linear(input_dim, hidden_dim),
-            nn.ReLU(),
-            # nn.Linear(hidden_dim, hidden_dim),
-            # nn.ReLU(),
-            nn.Linear(hidden_dim, 1)
-        )
-        
-        self.actor = nn.Sequential(
-            nn.Linear(input_dim, hidden_dim),
-            nn.ReLU(),
-            # nn.Linear(hidden_dim, hidden_dim),
-            # nn.ReLU(),
-            nn.Linear(hidden_dim, output_dim),
-        )
-        self.log_std = nn.Parameter(torch.ones(1, output_dim) * std)
-        
-        # self.apply(init_linear_weights)
-        
-    def forward(self, x):
-        value = self.critic(x)
-        mu = self.actor(x)
-        mu = torch.tanh(mu)
-        std = self.log_std.exp().expand_as(mu)
-        return mu, std, value
-
 class Policy(BasePolicy):
     def __init__(self, cfg: MergedConfig) -> None:
         super(Policy, self).__init__(cfg)
         self.independ_actor = cfg.independ_actor
         self.share_optimizer = cfg.share_optimizer
         self.ppo_type = 'clip' # clip or kl
         if self.ppo_type == 'kl':
@@ -103,64 +60,41 @@
             self.summary['scalar']['tot_loss'] = np.mean(self.tot_losses_epoch)
         self.summary['scalar']['actor_loss'] = np.mean(self.actor_losses_epoch)
         self.summary['scalar']['critic_loss'] = np.mean(self.critic_losses_epoch)
 
     def create_model(self):
         self.model = ActorCriticNetwork(self.cfg, self.state_size_list).to(self.device)
 
-        
-        # self.model = Model(self.state_size_list[0][1], self.action_size_list[0], 256, std=0.0).to(self.device)
-
     def create_optimizer(self):
-        self.optimizer = optim.Adam(self.model.parameters(), lr = self.cfg.lr)
-        # if not self.independ_actor:
-        #     self.optimizer = optim.Adam(self.policy_net.parameters(), lr=self.cfg.lr) 
-        # else:
-        #     self.actor_optimizer = optim.Adam(self.actor.parameters(), lr=self.cfg.actor_lr)
-        #     self.critic_optimizer = optim.Adam(self.critic.parameters(), lr=self.cfg.critic_lr)  
+        self.optimizer = optim.Adam(self.model.parameters(), lr = self.cfg.lr)  
 
     def update_policy_transition(self):
         self.policy_transition = {'value': self.value.detach().cpu().numpy().item(), 'log_prob': self.log_prob}
 
     def sample_action(self, state, **kwargs):
         state = torch.tensor(np.array(state), device=self.device, dtype=torch.float32)
         # single state shape must be [batch_size, state_dim]
         if state.dim() == 1: 
             state = state.unsqueeze(dim=0)
-        self.value, self.actor_outputs = self.model(state)
-        actions, self.log_prob = self.model.action_layers.get_actions_and_log_probs(mode = 'sample', actor_outputs = self.actor_outputs)
+        model_outputs = self.model(state)
+        self.value = model_outputs['value']
+        actor_outputs = model_outputs['actor_outputs']
+        actions, self.log_prob = self.model.action_layers.get_actions_and_log_probs(mode = 'sample', actor_outputs = actor_outputs)
         self.update_policy_transition()
         return actions
 
-    def compute_return_mc(self, rewards, masks):
-        returns = []
-        discounted_return = 0
-        for step in reversed(range(len(rewards))):
-            discounted_return = rewards[step] + self.gamma * discounted_return * masks[step]
-            returns.insert(0, discounted_return)
-        # return returns
-        # print("return",returns)
-        # print("masks",masks)
-        # print(rewards)
-        # normalize can help to stabilize training
-        returns = torch.cat(returns)
-        normed_returns = (returns - returns.mean()) / (returns.std() + 1e-5)
-        # normed_returns = []
-        # for ret in returns:
-        #     normed_returns.append((ret - ret.mean()) / (ret.std() + 1e-5))
-        return normed_returns
-
     @torch.no_grad()
     def predict_action(self, state, **kwargs):
         state = torch.tensor(np.array(state), device=self.device, dtype=torch.float32)
         # single state shape must be [batch_size, state_dim]
         if state.dim() == 1: 
             state = state.unsqueeze(dim=0)
-        self.value, self.actor_outputs = self.model(state)
-        actions = self.model.action_layers.get_actions(mode = 'predict', actor_outputs = self.actor_outputs)
+        model_outputs = self.model(state)
+        actor_outputs = model_outputs['actor_outputs']
+        actions = self.model.action_layers.get_actions(mode = 'predict', actor_outputs = actor_outputs)
         return actions
 
     def learn(self, **kwargs):
         states, actions, next_states, rewards, dones, returns = kwargs.get('states'), kwargs.get('actions'), kwargs.get('next_states'), kwargs.get('rewards'), kwargs.get('dones'), kwargs.get('returns')
         old_log_probs  = kwargs.get('log_probs')
         torch_dataset = Data.TensorDataset(*states, *actions, old_log_probs, returns)
         train_loader = Data.DataLoader(dataset = torch_dataset, batch_size = self.sgd_batch_size, shuffle = True)
@@ -175,15 +109,17 @@
                 # multi-head action
                 old_actions = []
                 for i in range(len(actions)):
                     old_actions.append(data[idx+i])
                 idx += len(actions)
                 old_log_probs = data[idx]
                 returns = data[idx+1]
-                values, actor_outputs = self.model(old_states)
+                model_outputs = self.model(old_states)
+                values = model_outputs['value']
+                actor_outputs = model_outputs['actor_outputs']
                 new_log_probs = self.model.action_layers.get_log_probs_action(actor_outputs, old_actions)
                 # new_log_probs = self.model.action_layers.get_log_probs_action(old_actions)
                 entropy_mean = self.model.action_layers.get_mean_entropy(actor_outputs)
                 advantages = returns - values.detach() # shape:[batch_size,1]
                 # get action probabilities
                 # compute ratio (pi_theta / pi_theta__old):
                 ratio = torch.exp(new_log_probs - old_log_probs) # shape: [batch_size, 1]
```

### Comparing `joyrl-0.6.0.2/joyrl/algos/QLearning/data_handler.py` & `joyrl-0.6.1/joyrl/algos/QLearning/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/QLearning/policy.py` & `joyrl-0.6.1/joyrl/algos/QLearning/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/Sarsa/data_handler.py` & `joyrl-0.6.1/joyrl/algos/Sarsa/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/Sarsa/policy.py` & `joyrl-0.6.1/joyrl/algos/Sarsa/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/TD3/config.py` & `joyrl-0.6.1/joyrl/algos/TD3/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/TD3/policy.py` & `joyrl-0.6.1/joyrl/algos/TD3/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/base/action_layer.py` & `joyrl-0.6.1/joyrl/algos/base/action_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-25 09:28:26
 LastEditor: JiangJi
-LastEditTime: 2024-05-26 20:17:08
+LastEditTime: 2024-06-02 00:17:16
 Discription: 
 '''
 from enum import Enum
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.distributions import Categorical,Normal
@@ -59,36 +59,23 @@
         if self.dueling:
             state_value = self.state_value_layer(x)
             action_value = self.action_value_layer(x)
             q_value = state_value + action_value - action_value.mean(dim=1, keepdim=True)
         else:
             q_value = self.action_value_layer(x)
         output = {"q_value": q_value}
-        self.q_value = q_value
         return output
     
-    def get_qvalue(self):
-        return self.q_value
-    
-    def get_action(self, **kwargs):
-        mode = kwargs.get("mode", "sample")
-        if mode == "sample":
-            return self.sample_action()
-        elif mode == "predict":
-            return self.predict_action()
-        else:
-            raise NotImplementedError
-        
-    def sample_action(self):
-        return torch.argmax(self.q_value).detach().cpu().numpy().item()
+    def sample_action(self, **kwargs):
+        q_value = kwargs.get("q_value", None)
+        return {"action": torch.argmax(q_value).detach().cpu().numpy().item()}
     
-    def predict_action(self):
-        ''' get action
-        '''
-        return torch.argmax(self.q_value).detach().cpu().numpy().item()
+    def predict_action(self, **kwargs):
+        q_value = kwargs.get("q_value", None)
+        return {"action": torch.argmax(q_value).detach().cpu().numpy().item()}
 
 class DiscreteActionLayer(BaseActionLayer):
     def __init__(self, cfg, input_size, action_dim, id = 0, **kwargs):
         super(DiscreteActionLayer, self).__init__(cfg=cfg, input_size=input_size, action_dim=action_dim, id=id)
         self.min_policy = cfg.min_policy
         self.action_dim = action_dim
         output_size = input_size
@@ -159,50 +146,39 @@
         self.action_dim = action_dim
         output_size = input_size
         mu_layer_cfg = LayerConfig(layer_type='linear', layer_size=[self.action_dim], activation='tanh')
         self.mu_layer, _ = create_layer(output_size, mu_layer_cfg)
         self.log_std = nn.Parameter(torch.zeros(1, self.action_dim))
 
     def forward(self,x, **kwargs):
-        mu = self.mu_layer(x)
+        mu = self.mu_layer(x) # [batch_size, 1]
         sigma = torch.ones_like(mu) * torch.exp(self.log_std)
         # log_prob = -0.5 * (sigma.log() + ((mu - x) / sigma).pow(2) + math.log(2 * math.pi))
         # sigma = F.softplus(self.fc4(x)) + 0.001 # std of normal distribution, add a small value to avoid 0
         # sigma = torch.clamp(sigma, min=-0.25, max=0.25) # clamp the std between 0.001 and 1
-        self.mu = mu # [batch_size, 1]
-        self.sigma = sigma # [batch_size]
-        self.mean = self.mu * self.action_scale + self.action_bias
-        self.std = self.sigma
-        output = {"mu": self.mu, "sigma": self.sigma, "mean": self.mean, "std": self.std}
+        mean = mu * self.action_scale + self.action_bias
+        std = sigma
+        output = {"mu": mu, "sigma": sigma, "mean": mean, "std": std}
         return output
     
     def sample_action(self, **kwargs):
         ''' get action
         '''
         mean = kwargs.get("mean", None)
         std = kwargs.get("std", None)
         dist = Normal(mean, std)
         action = dist.sample()
         log_prob = dist.log_prob(action)
         return {"action": action.detach().cpu().numpy().item(), "log_prob": log_prob.detach().cpu().numpy().item()}
-
-
+    
     def predict_action(self, **kwargs):
         ''' get action
         '''
-        return {"action": self.mean.detach().cpu().numpy().item(), "log_prob": None}
-    
-    def get_log_prob(self, **kwargs):
-        ''' get log_probs
-        '''
         mean = kwargs.get("mean", None)
-        std = kwargs.get("std", None)
-        dist = Normal(mean, std)
-        action = dist.sample()
-        return self.log_prob
+        return {"action": mean.detach().cpu().numpy().item(), "log_prob": None}
     
     def get_log_prob_action(self, actor_output, action):
         ''' get log_probs
         '''
         # action shape is [batch_size, action_dim]
         mean = actor_output.get("mean", None)
         std = actor_output.get("std", None)
```

### Comparing `joyrl-0.6.0.2/joyrl/algos/base/base_layer.py` & `joyrl-0.6.1/joyrl/algos/base/base_layer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/base/buffer.py` & `joyrl-0.6.1/joyrl/algos/base/buffer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/base/data_handler.py` & `joyrl-0.6.1/joyrl/algos/base/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/base/network.py` & `joyrl-0.6.1/joyrl/algos/base/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-22 23:02:13
 LastEditor: JiangJi
-LastEditTime: 2024-05-27 09:50:26
+LastEditTime: 2024-06-02 00:11:14
 Discription: 
 '''
 import copy
 import torch
 import torch.nn as nn
 from joyrl.algos.base.base_layer import create_layer, LayerConfig
 from joyrl.algos.base.action_layer import ActionLayerType, DiscreteActionLayer, ContinuousActionLayer, DPGActionLayer, DQNActionLayer
@@ -124,37 +124,36 @@
             mus.append(action_layer.get_mu())
         return mus[0]
     
     def get_qvalues(self):
         qvalues = []
         for _, action_layer in enumerate(self.action_layers):
             qvalues.append(action_layer.get_qvalue())
-        return qvalues[0]
+        return qvalues
     
     def get_actions(self, **kwargs):
         mode = kwargs.get('mode', 'train')
-        actor_outputs = kwargs.get('actor_outputs', self.actor_outputs)
+        actor_outputs = kwargs.get('actor_outputs', None)
         actions = []
         for i, action_layer in enumerate(self.action_layers):
             action_layer_output = action_layer.get_action(mode = mode, actor_output = actor_outputs[i])
             actions.append(action_layer_output['action'])
         return actions
     
     def get_actions_and_log_probs(self, **kwargs):
         mode = kwargs.get('mode', 'train')
-        actor_outputs = kwargs.get('actor_outputs', self.actor_outputs)
+        actor_outputs = kwargs.get('actor_outputs')
         actions = []
         log_probs_sum = 0
         for i, action_layer in enumerate(self.action_layers):
             action_layer_output = action_layer.get_action(mode = mode, actor_output = actor_outputs[i])
             actions.append(action_layer_output['action'])
             log_probs_sum += action_layer_output['log_prob']
         return actions, log_probs_sum
     
-    
     def get_log_probs_action(self, actor_outputs, actions):
         log_prob_sum = 0
         for i, action_layer in enumerate(self.action_layers):
             actor_output = actor_outputs[i]
             action = actions[i]
             log_prob = action_layer.get_log_prob_action(actor_output, action)
             log_prob_sum += log_prob
@@ -183,15 +182,14 @@
         return x
     
 class QNetwork(BaseNework):
     ''' Q network, for value-based methods like DQN
     '''
     def __init__(self, cfg: MergedConfig, input_size_list: list) -> None:
         '''_summary_
-
         Args:
             cfg (_type_): _description_
             state_size (_type_): [[None, state_dim_1], [None, None, state_dim_2], ...]
             action_size (_type_): [action_dim_1, action_dim_2, ...]
         Raises:
             ValueError: _description_
         '''
@@ -202,45 +200,27 @@
 
     def create_graph(self):
         self.branch_layers = BranchLayers(self.cfg.branch_layers, self.input_size_list)
         self.merge_layer = MergeLayer(self.cfg.merge_layers, self.branch_layers.output_size_list)
         action_type_list = ['dqnaction'] * len(self.cfg.action_type_list) 
         setattr(self.cfg, 'action_type_list', action_type_list)
         self.action_layers = ActionLayers(self.cfg, self.merge_layer.output_size)
-        # if self.dueling:
-        #     state_value_layer_cfg = LayerConfig(layer_type='linear', layer_size=[1], activation='none')
-        #     self.state_value_layer, _ = create_layer(self.merge_layer.output_size, state_value_layer_cfg)
-        #     action_value_layer_cfg = LayerConfig(layer_type='linear', layer_size=[self.action_size_list[0]], activation='none')
-        #     self.action_value_layer, _ = create_layer(self.merge_layer.output_size, action_value_layer_cfg)
-        # else:
-        #     action_layer_cfg = LayerConfig(layer_type='linear', layer_size=[self.action_size_list[0]], activation='none')
-        #     self.action_value_layer, _ = create_layer(self.merge_layer.output_size, action_layer_cfg)
 
     def forward(self, x):
         x = self.branch_layers(x)
         x = self.merge_layer(x)
         actor_outputs = self.action_layers(x)
-        return actor_outputs
-    
-    
-        if self.dueling:
-            state_value = self.state_value_layer(x)
-            action_value = self.action_value_layer(x)
-            q_value = state_value + action_value - action_value.mean(dim=1, keepdim=True)
-        else:
-            q_value = self.action_value_layer(x)
-        return q_value
+        return {"actor_outputs": actor_outputs}
     
     def reset_noise(self):
         ''' reset noise for noisy layers
         '''
         self.branch_layers.reset_noise()
         self.merge_layer.reset_noise()
 
-   
 class ActorCriticNetwork(BaseNework):
     ''' Value network, for policy-based methods,  in which the branch_layers and critic share the same network
     '''
     def __init__(self, cfg: MergedConfig, input_size_list: list) -> None:
         super(ActorCriticNetwork, self).__init__(cfg, input_size_list)
         self.action_type_list = self.cfg.action_type_list
         self.create_graph()
@@ -251,17 +231,16 @@
         self.value_layer, _ = create_layer(self.merge_layer.output_size, LayerConfig(layer_type='linear', layer_size=[1], activation='none'))
         self.action_layers = ActionLayers(self.cfg, self.merge_layer.output_size,)
         
     def forward(self, x, pre_legal_actions=None):
         x = self.branch_layers(x)
         x = self.merge_layer(x)
         value = self.value_layer(x)
-        action_outputs = self.action_layers(x, pre_legal_actions = pre_legal_actions)
-        return value, action_outputs
-
+        actor_outputs = self.action_layers(x, pre_legal_actions = pre_legal_actions)
+        return {'value': value, 'actor_outputs': actor_outputs}
 
 class ActorNetwork(BaseNework):
     def __init__(self, cfg: MergedConfig, input_size_list) -> None:
         super(ActorNetwork, self).__init__(cfg, input_size_list)
         self.action_type_list = self.cfg.action_type_list
         self.create_graph()
```

### Comparing `joyrl-0.6.0.2/joyrl/algos/base/noise.py` & `joyrl-0.6.1/joyrl/algos/base/noise.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/base/optm.py` & `joyrl-0.6.1/joyrl/algos/base/optm.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/algos/base/policy.py` & `joyrl-0.6.1/joyrl/algos/base/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         self.action_space = cfg.action_space
         self.policy_transition = {}
         self.data_after_train = {}
         self.get_state_size()
         self.get_action_size()
         self.create_model()
         self.create_optimizer()
+        self.create_summary()
     
     def get_state_size(self):
         ''' get state size
         '''
         # state_size must be [[None, state_dim_1], [None, state_dim_2], ...]
         if isinstance(self.obs_space, Box):
             if len(self.obs_space.shape) == 3:
```

### Comparing `joyrl-0.6.0.2/joyrl/envs/blackjack.py` & `joyrl-0.6.1/joyrl/envs/blackjack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/envs/cliff_walking.py` & `joyrl-0.6.1/joyrl/envs/cliff_walking.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/envs/gridworld.py` & `joyrl-0.6.1/joyrl/envs/gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/envs/gridworld_env.py` & `joyrl-0.6.1/joyrl/envs/gridworld_env.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/envs/gym/config.py` & `joyrl-0.6.1/joyrl/envs/gym/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/envs/gym/wrappers.py` & `joyrl-0.6.1/joyrl/envs/gym/wrappers.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/envs/racetrack.py` & `joyrl-0.6.1/joyrl/envs/racetrack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/envs/register.py` & `joyrl-0.6.1/joyrl/envs/register.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/envs/stochastic_mdp.py` & `joyrl-0.6.1/joyrl/envs/stochastic_mdp.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/envs/windy_gridworld.py` & `joyrl-0.6.1/joyrl/envs/windy_gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/framework/base.py` & `joyrl-0.6.1/joyrl/framework/base.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/framework/collector.py` & `joyrl-0.6.1/joyrl/framework/collector.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/framework/config.py` & `joyrl-0.6.1/joyrl/framework/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/framework/interactor.py` & `joyrl-0.6.1/joyrl/framework/interactor.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/framework/learner.py` & `joyrl-0.6.1/joyrl/framework/learner.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/framework/message.py` & `joyrl-0.6.1/joyrl/framework/message.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/framework/policy_mgr.py` & `joyrl-0.6.1/joyrl/framework/policy_mgr.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/framework/recorder.py` & `joyrl-0.6.1/joyrl/framework/recorder.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/framework/tester.py` & `joyrl-0.6.1/joyrl/framework/tester.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/framework/tracker.py` & `joyrl-0.6.1/joyrl/framework/tracker.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/framework/trainer.py` & `joyrl-0.6.1/joyrl/framework/trainer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/framework/utils.py` & `joyrl-0.6.1/joyrl/framework/utils.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/run.py` & `joyrl-0.6.1/joyrl/run.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/scripts/scripts.py` & `joyrl-0.6.1/joyrl/scripts/scripts.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl/utils/utils.py` & `joyrl-0.6.1/joyrl/utils/utils.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/joyrl.egg-info/PKG-INFO` & `joyrl-0.6.1/joyrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.6.0.2
+Version: 0.6.1
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.6.0.2/joyrl.egg-info/SOURCES.txt` & `joyrl-0.6.1/joyrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/setup.cfg` & `joyrl-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.2/setup.py` & `joyrl-0.6.1/setup.py`

 * *Files identical despite different names*

