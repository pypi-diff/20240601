# Comparing `tmp/joyrl-0.6.0.1.tar.gz` & `tmp/joyrl-0.6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joyrl-0.6.0.1.tar", last modified: Sat Jun  1 09:17:54 2024, max compression
+gzip compressed data, was "joyrl-0.6.0.2.tar", last modified: Sat Jun  1 09:20:51 2024, max compression
```

## Comparing `joyrl-0.6.0.1.tar` & `joyrl-0.6.0.2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.506810 joyrl-0.6.0.1/
--rw-r--r--   0 johnjim    (501) staff       (20)     1077 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/LICENSE
--rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-01 09:17:54.506694 joyrl-0.6.0.1/PKG-INFO
--rw-r--r--   0 johnjim    (501) staff       (20)    10670 2024-06-01 08:59:02.000000 joyrl-0.6.0.1/README.md
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.495797 joyrl-0.6.0.1/joyrl/
--rw-r--r--   0 johnjim    (501) staff       (20)      377 2024-06-01 09:17:53.000000 joyrl-0.6.0.1/joyrl/__init__.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.496707 joyrl-0.6.0.1/joyrl/algos/
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.497207 joyrl-0.6.0.1/joyrl/algos/DDPG/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DDPG/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1517 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DDPG/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      152 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DDPG/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     5540 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DDPG/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.497703 joyrl-0.6.0.1/joyrl/algos/DQN/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1950 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      158 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3507 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.498158 joyrl-0.6.0.1/joyrl/algos/DoubleDQN/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DoubleDQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1703 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DoubleDQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      350 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DoubleDQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3696 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DoubleDQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.498647 joyrl-0.6.0.1/joyrl/algos/DuelingDQN/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DuelingDQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      907 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DuelingDQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      337 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DuelingDQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3948 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/DuelingDQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.499127 joyrl-0.6.0.1/joyrl/algos/NoisyDQN/
--rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/NoisyDQN/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1071 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/NoisyDQN/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      341 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/NoisyDQN/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     4445 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/NoisyDQN/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.499632 joyrl-0.6.0.1/joyrl/algos/PPO/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/PPO/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2071 2024-05-09 17:05:41.000000 joyrl-0.6.0.1/joyrl/algos/PPO/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3195 2024-06-01 05:12:21.000000 joyrl-0.6.0.1/joyrl/algos/PPO/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     9208 2024-05-27 16:17:38.000000 joyrl-0.6.0.1/joyrl/algos/PPO/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.500139 joyrl-0.6.0.1/joyrl/algos/QLearning/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/QLearning/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/QLearning/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.0.1/joyrl/algos/QLearning/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1964 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/QLearning/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.500580 joyrl-0.6.0.1/joyrl/algos/Sarsa/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/Sarsa/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/Sarsa/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.0.1/joyrl/algos/Sarsa/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2144 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/Sarsa/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.501035 joyrl-0.6.0.1/joyrl/algos/TD3/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/TD3/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1277 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/TD3/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)      153 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/TD3/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)     7726 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/TD3/policy.py
--rw-r--r--   0 johnjim    (501) staff       (20)      366 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/__init__.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.502444 joyrl-0.6.0.1/joyrl/algos/base/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/base/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)    10713 2024-05-26 12:17:32.000000 joyrl-0.6.0.1/joyrl/algos/base/action_layer.py
--rw-r--r--   0 johnjim    (501) staff       (20)     8643 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/base/base_layer.py
--rw-r--r--   0 johnjim    (501) staff       (20)    86089 2024-06-01 05:31:25.000000 joyrl-0.6.0.1/joyrl/algos/base/buffer.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2755 2024-06-01 05:12:03.000000 joyrl-0.6.0.1/joyrl/algos/base/data_handler.py
--rw-r--r--   0 johnjim    (501) staff       (20)      131 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/base/experience.py
--rw-r--r--   0 johnjim    (501) staff       (20)    14978 2024-05-27 01:50:26.000000 joyrl-0.6.0.1/joyrl/algos/base/network.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1313 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/base/noise.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2407 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/algos/base/optm.py
--rw-r--r--   0 johnjim    (501) staff       (20)     7605 2024-05-27 15:36:54.000000 joyrl-0.6.0.1/joyrl/algos/base/policy.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.503527 joyrl-0.6.0.1/joyrl/envs/
--rw-r--r--   0 johnjim    (501) staff       (20)       51 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/envs/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     4258 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/envs/blackjack.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2706 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/envs/cliff_walking.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3871 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/envs/gridworld.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3485 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/envs/gridworld_env.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.503884 joyrl-0.6.0.1/joyrl/envs/gym/
--rw-r--r--   0 johnjim    (501) staff       (20)      221 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/envs/gym/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      525 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/envs/gym/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)    11068 2024-05-09 16:41:09.000000 joyrl-0.6.0.1/joyrl/envs/gym/wrappers.py
--rw-r--r--   0 johnjim    (501) staff       (20)     9890 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/envs/racetrack.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1445 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/envs/register.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1311 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/envs/stochastic_mdp.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2615 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/envs/windy_gridworld.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.505392 joyrl-0.6.0.1/joyrl/framework/
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/framework/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)     1069 2024-05-30 09:43:52.000000 joyrl-0.6.0.1/joyrl/framework/base.py
--rw-r--r--   0 johnjim    (501) staff       (20)     4442 2024-06-01 08:53:39.000000 joyrl-0.6.0.1/joyrl/framework/collector.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2294 2024-06-01 06:35:14.000000 joyrl-0.6.0.1/joyrl/framework/config.py
--rw-r--r--   0 johnjim    (501) staff       (20)     5619 2024-06-01 08:53:09.000000 joyrl-0.6.0.1/joyrl/framework/interactor.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2874 2024-06-01 08:53:20.000000 joyrl-0.6.0.1/joyrl/framework/learner.py
--rw-r--r--   0 johnjim    (501) staff       (20)      821 2024-05-28 01:37:10.000000 joyrl-0.6.0.1/joyrl/framework/message.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2923 2024-06-01 03:33:53.000000 joyrl-0.6.0.1/joyrl/framework/policy_mgr.py
--rw-r--r--   0 johnjim    (501) staff       (20)     5272 2024-05-30 09:48:58.000000 joyrl-0.6.0.1/joyrl/framework/recorder.py
--rw-r--r--   0 johnjim    (501) staff       (20)     3961 2024-05-31 03:30:30.000000 joyrl-0.6.0.1/joyrl/framework/tester.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2242 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/framework/tracker.py
--rw-r--r--   0 johnjim    (501) staff       (20)     7020 2024-06-01 08:53:33.000000 joyrl-0.6.0.1/joyrl/framework/trainer.py
--rw-r--r--   0 johnjim    (501) staff       (20)     2524 2024-05-31 14:51:57.000000 joyrl-0.6.0.1/joyrl/framework/utils.py
--rw-r--r--   0 johnjim    (501) staff       (20)     8002 2024-06-01 09:17:47.000000 joyrl-0.6.0.1/joyrl/run.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.505606 joyrl-0.6.0.1/joyrl/scripts/
--rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/scripts/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)      520 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/scripts/scripts.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.505940 joyrl-0.6.0.1/joyrl/utils/
--rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/utils/__init__.py
--rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.1/joyrl/utils/plot.py
--rw-r--r--   0 johnjim    (501) staff       (20)    37181 2024-05-30 09:48:17.000000 joyrl-0.6.0.1/joyrl/utils/utils.py
-drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:17:54.506149 joyrl-0.6.0.1/joyrl.egg-info/
--rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-01 09:17:54.000000 joyrl-0.6.0.1/joyrl.egg-info/PKG-INFO
--rw-r--r--   0 johnjim    (501) staff       (20)     2455 2024-06-01 09:17:54.000000 joyrl-0.6.0.1/joyrl.egg-info/SOURCES.txt
--rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-06-01 09:17:54.000000 joyrl-0.6.0.1/joyrl.egg-info/dependency_links.txt
--rw-r--r--   0 johnjim    (501) staff       (20)       53 2024-06-01 09:17:54.000000 joyrl-0.6.0.1/joyrl.egg-info/entry_points.txt
--rw-r--r--   0 johnjim    (501) staff       (20)      256 2024-06-01 09:17:54.000000 joyrl-0.6.0.1/joyrl.egg-info/requires.txt
--rw-r--r--   0 johnjim    (501) staff       (20)        6 2024-06-01 09:17:54.000000 joyrl-0.6.0.1/joyrl.egg-info/top_level.txt
--rw-r--r--   0 johnjim    (501) staff       (20)      940 2024-06-01 09:17:54.507163 joyrl-0.6.0.1/setup.cfg
--rw-r--r--   0 johnjim    (501) staff       (20)     1886 2024-06-01 09:01:11.000000 joyrl-0.6.0.1/setup.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.190507 joyrl-0.6.0.2/
+-rw-r--r--   0 johnjim    (501) staff       (20)     1077 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/LICENSE
+-rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-01 09:20:51.190405 joyrl-0.6.0.2/PKG-INFO
+-rw-r--r--   0 johnjim    (501) staff       (20)    10670 2024-06-01 08:59:02.000000 joyrl-0.6.0.2/README.md
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.179150 joyrl-0.6.0.2/joyrl/
+-rw-r--r--   0 johnjim    (501) staff       (20)      377 2024-06-01 09:19:57.000000 joyrl-0.6.0.2/joyrl/__init__.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.180176 joyrl-0.6.0.2/joyrl/algos/
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.180736 joyrl-0.6.0.2/joyrl/algos/DDPG/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DDPG/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1517 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DDPG/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      152 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DDPG/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5540 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DDPG/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.181224 joyrl-0.6.0.2/joyrl/algos/DQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1950 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      158 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3507 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.181714 joyrl-0.6.0.2/joyrl/algos/DoubleDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DoubleDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1703 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DoubleDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      350 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DoubleDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3696 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DoubleDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.182189 joyrl-0.6.0.2/joyrl/algos/DuelingDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DuelingDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      907 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DuelingDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      337 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DuelingDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3948 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/DuelingDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.182640 joyrl-0.6.0.2/joyrl/algos/NoisyDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/NoisyDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1071 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/NoisyDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      341 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/NoisyDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4445 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/NoisyDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.183125 joyrl-0.6.0.2/joyrl/algos/PPO/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/PPO/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2071 2024-05-09 17:05:41.000000 joyrl-0.6.0.2/joyrl/algos/PPO/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2979 2024-06-01 09:19:48.000000 joyrl-0.6.0.2/joyrl/algos/PPO/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     9208 2024-05-27 16:17:38.000000 joyrl-0.6.0.2/joyrl/algos/PPO/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.183583 joyrl-0.6.0.2/joyrl/algos/QLearning/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/QLearning/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/QLearning/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.0.2/joyrl/algos/QLearning/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1964 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/QLearning/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.184073 joyrl-0.6.0.2/joyrl/algos/Sarsa/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/Sarsa/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/Sarsa/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.0.2/joyrl/algos/Sarsa/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2144 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/Sarsa/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.184519 joyrl-0.6.0.2/joyrl/algos/TD3/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/TD3/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1277 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/TD3/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      153 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/TD3/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7726 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/TD3/policy.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      366 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/__init__.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.185981 joyrl-0.6.0.2/joyrl/algos/base/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/base/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    10713 2024-05-26 12:17:32.000000 joyrl-0.6.0.2/joyrl/algos/base/action_layer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     8643 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/base/base_layer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    86089 2024-06-01 05:31:25.000000 joyrl-0.6.0.2/joyrl/algos/base/buffer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2755 2024-06-01 05:12:03.000000 joyrl-0.6.0.2/joyrl/algos/base/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      131 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/base/experience.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    14978 2024-05-27 01:50:26.000000 joyrl-0.6.0.2/joyrl/algos/base/network.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1313 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/base/noise.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2407 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/algos/base/optm.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7605 2024-05-27 15:36:54.000000 joyrl-0.6.0.2/joyrl/algos/base/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.187120 joyrl-0.6.0.2/joyrl/envs/
+-rw-r--r--   0 johnjim    (501) staff       (20)       51 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4258 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/blackjack.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2706 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/cliff_walking.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3871 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/gridworld.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3485 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/gridworld_env.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.187485 joyrl-0.6.0.2/joyrl/envs/gym/
+-rw-r--r--   0 johnjim    (501) staff       (20)      221 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/gym/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      525 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/gym/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    11068 2024-05-09 16:41:09.000000 joyrl-0.6.0.2/joyrl/envs/gym/wrappers.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     9890 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/racetrack.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1445 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/register.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1311 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/stochastic_mdp.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2615 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/envs/windy_gridworld.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.189026 joyrl-0.6.0.2/joyrl/framework/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/framework/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1069 2024-05-30 09:43:52.000000 joyrl-0.6.0.2/joyrl/framework/base.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4442 2024-06-01 08:53:39.000000 joyrl-0.6.0.2/joyrl/framework/collector.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2294 2024-06-01 06:35:14.000000 joyrl-0.6.0.2/joyrl/framework/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5619 2024-06-01 08:53:09.000000 joyrl-0.6.0.2/joyrl/framework/interactor.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2874 2024-06-01 08:53:20.000000 joyrl-0.6.0.2/joyrl/framework/learner.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      821 2024-05-28 01:37:10.000000 joyrl-0.6.0.2/joyrl/framework/message.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2923 2024-06-01 03:33:53.000000 joyrl-0.6.0.2/joyrl/framework/policy_mgr.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5272 2024-05-30 09:48:58.000000 joyrl-0.6.0.2/joyrl/framework/recorder.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3961 2024-05-31 03:30:30.000000 joyrl-0.6.0.2/joyrl/framework/tester.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2242 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/framework/tracker.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7020 2024-06-01 08:53:33.000000 joyrl-0.6.0.2/joyrl/framework/trainer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2524 2024-05-31 14:51:57.000000 joyrl-0.6.0.2/joyrl/framework/utils.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     8002 2024-06-01 09:17:47.000000 joyrl-0.6.0.2/joyrl/run.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.189256 joyrl-0.6.0.2/joyrl/scripts/
+-rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/scripts/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      520 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/scripts/scripts.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.189583 joyrl-0.6.0.2/joyrl/utils/
+-rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/utils/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0.2/joyrl/utils/plot.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    37181 2024-05-30 09:48:17.000000 joyrl-0.6.0.2/joyrl/utils/utils.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:20:51.189837 joyrl-0.6.0.2/joyrl.egg-info/
+-rw-r--r--   0 johnjim    (501) staff       (20)    11639 2024-06-01 09:20:51.000000 joyrl-0.6.0.2/joyrl.egg-info/PKG-INFO
+-rw-r--r--   0 johnjim    (501) staff       (20)     2455 2024-06-01 09:20:51.000000 joyrl-0.6.0.2/joyrl.egg-info/SOURCES.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-06-01 09:20:51.000000 joyrl-0.6.0.2/joyrl.egg-info/dependency_links.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)       53 2024-06-01 09:20:51.000000 joyrl-0.6.0.2/joyrl.egg-info/entry_points.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)      256 2024-06-01 09:20:51.000000 joyrl-0.6.0.2/joyrl.egg-info/requires.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)        6 2024-06-01 09:20:51.000000 joyrl-0.6.0.2/joyrl.egg-info/top_level.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)      940 2024-06-01 09:20:51.190828 joyrl-0.6.0.2/setup.cfg
+-rw-r--r--   0 johnjim    (501) staff       (20)     1886 2024-06-01 09:01:11.000000 joyrl-0.6.0.2/setup.py
```

### Comparing `joyrl-0.6.0.1/LICENSE` & `joyrl-0.6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/PKG-INFO` & `joyrl-0.6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.6.0.1
+Version: 0.6.0.2
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.6.0.1/README.md` & `joyrl-0.6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/DDPG/config.py` & `joyrl-0.6.0.2/joyrl/algos/DDPG/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/DDPG/policy.py` & `joyrl-0.6.0.2/joyrl/algos/DDPG/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/DQN/config.py` & `joyrl-0.6.0.2/joyrl/algos/DQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/DQN/policy.py` & `joyrl-0.6.0.2/joyrl/algos/DQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/DoubleDQN/config.py` & `joyrl-0.6.0.2/joyrl/algos/DoubleDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/DoubleDQN/policy.py` & `joyrl-0.6.0.2/joyrl/algos/DoubleDQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/DuelingDQN/config.py` & `joyrl-0.6.0.2/joyrl/algos/DuelingDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/DuelingDQN/policy.py` & `joyrl-0.6.0.2/joyrl/algos/DuelingDQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/NoisyDQN/config.py` & `joyrl-0.6.0.2/joyrl/algos/NoisyDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/NoisyDQN/policy.py` & `joyrl-0.6.0.2/joyrl/algos/NoisyDQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/PPO/config.py` & `joyrl-0.6.0.2/joyrl/algos/PPO/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/PPO/data_handler.py` & `joyrl-0.6.0.2/joyrl/algos/PPO/data_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-05-17 01:08:36
 LastEditor: JiangJi
-LastEditTime: 2024-06-01 13:12:16
+LastEditTime: 2024-06-01 17:19:43
 Discription: 
 '''
 import numpy as np
 import torch
 from joyrl.algos.base.data_handler import BaseDataHandler
 class DataHandler(BaseDataHandler):
     def __init__(self, cfg):
@@ -49,19 +49,17 @@
             exps[t].normed_return_gae = return_gae_normed[t]
         exps = exps[:exp_len]
         return exps
     
     def add_exps(self, exps):
         exps = self.handle_exps_after_interact(exps)
         self.batch_exps.extend(exps)
-        # print(f"[DataHandler.add_exps] len(self.batch_exps): {len(self.batch_exps)}, interactor_id: {exps[0].interactor_id}")
         if len(self.batch_exps) >= self.cfg.batch_size:
             self.buffer.push(self.batch_exps)
             self.batch_exps = []
-        # print(f"[DataHandler.add_exps] len(self.batch_exps): {len(self.batch_exps)}")
 
     def _handle_exps_before_train(self, exps: list):
         ''' convert exps to training data
         '''
         super()._handle_exps_before_train(exps)
 
         log_probs = [exp.log_prob for exp in exps] # [batch_size]
```

### Comparing `joyrl-0.6.0.1/joyrl/algos/PPO/policy.py` & `joyrl-0.6.0.2/joyrl/algos/PPO/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/QLearning/data_handler.py` & `joyrl-0.6.0.2/joyrl/algos/QLearning/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/QLearning/policy.py` & `joyrl-0.6.0.2/joyrl/algos/QLearning/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/Sarsa/data_handler.py` & `joyrl-0.6.0.2/joyrl/algos/Sarsa/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/Sarsa/policy.py` & `joyrl-0.6.0.2/joyrl/algos/Sarsa/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/TD3/config.py` & `joyrl-0.6.0.2/joyrl/algos/TD3/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/TD3/policy.py` & `joyrl-0.6.0.2/joyrl/algos/TD3/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/base/action_layer.py` & `joyrl-0.6.0.2/joyrl/algos/base/action_layer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/base/base_layer.py` & `joyrl-0.6.0.2/joyrl/algos/base/base_layer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/base/buffer.py` & `joyrl-0.6.0.2/joyrl/algos/base/buffer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/base/data_handler.py` & `joyrl-0.6.0.2/joyrl/algos/base/data_handler.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/base/network.py` & `joyrl-0.6.0.2/joyrl/algos/base/network.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/base/noise.py` & `joyrl-0.6.0.2/joyrl/algos/base/noise.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/base/optm.py` & `joyrl-0.6.0.2/joyrl/algos/base/optm.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/algos/base/policy.py` & `joyrl-0.6.0.2/joyrl/algos/base/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/envs/blackjack.py` & `joyrl-0.6.0.2/joyrl/envs/blackjack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/envs/cliff_walking.py` & `joyrl-0.6.0.2/joyrl/envs/cliff_walking.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/envs/gridworld.py` & `joyrl-0.6.0.2/joyrl/envs/gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/envs/gridworld_env.py` & `joyrl-0.6.0.2/joyrl/envs/gridworld_env.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/envs/gym/config.py` & `joyrl-0.6.0.2/joyrl/envs/gym/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/envs/gym/wrappers.py` & `joyrl-0.6.0.2/joyrl/envs/gym/wrappers.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/envs/racetrack.py` & `joyrl-0.6.0.2/joyrl/envs/racetrack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/envs/register.py` & `joyrl-0.6.0.2/joyrl/envs/register.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/envs/stochastic_mdp.py` & `joyrl-0.6.0.2/joyrl/envs/stochastic_mdp.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/envs/windy_gridworld.py` & `joyrl-0.6.0.2/joyrl/envs/windy_gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/framework/base.py` & `joyrl-0.6.0.2/joyrl/framework/base.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/framework/collector.py` & `joyrl-0.6.0.2/joyrl/framework/collector.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/framework/config.py` & `joyrl-0.6.0.2/joyrl/framework/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/framework/interactor.py` & `joyrl-0.6.0.2/joyrl/framework/interactor.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/framework/learner.py` & `joyrl-0.6.0.2/joyrl/framework/learner.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/framework/message.py` & `joyrl-0.6.0.2/joyrl/framework/message.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/framework/policy_mgr.py` & `joyrl-0.6.0.2/joyrl/framework/policy_mgr.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/framework/recorder.py` & `joyrl-0.6.0.2/joyrl/framework/recorder.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/framework/tester.py` & `joyrl-0.6.0.2/joyrl/framework/tester.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/framework/tracker.py` & `joyrl-0.6.0.2/joyrl/framework/tracker.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/framework/trainer.py` & `joyrl-0.6.0.2/joyrl/framework/trainer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/framework/utils.py` & `joyrl-0.6.0.2/joyrl/framework/utils.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/run.py` & `joyrl-0.6.0.2/joyrl/run.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/scripts/scripts.py` & `joyrl-0.6.0.2/joyrl/scripts/scripts.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl/utils/utils.py` & `joyrl-0.6.0.2/joyrl/utils/utils.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/joyrl.egg-info/PKG-INFO` & `joyrl-0.6.0.2/joyrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.6.0.1
+Version: 0.6.0.2
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
```

### Comparing `joyrl-0.6.0.1/joyrl.egg-info/SOURCES.txt` & `joyrl-0.6.0.2/joyrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/setup.cfg` & `joyrl-0.6.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `joyrl-0.6.0.1/setup.py` & `joyrl-0.6.0.2/setup.py`

 * *Files identical despite different names*

