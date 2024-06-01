# Comparing `tmp/joyrl-0.5.2.tar.gz` & `tmp/joyrl-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joyrl-0.5.2.tar", last modified: Sat Jan 27 14:58:05 2024, max compression
+gzip compressed data, was "joyrl-0.6.0.tar", last modified: Sat Jun  1 09:12:28 2024, max compression
```

## Comparing `joyrl-0.5.2.tar` & `joyrl-0.6.0.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.759156 joyrl-0.5.2/
--rw-r--r--   0 jj         (502) staff       (20)     1077 2023-12-22 05:01:23.000000 joyrl-0.5.2/LICENSE
--rw-r--r--   0 jj         (502) staff       (20)    11227 2024-01-27 14:58:05.759309 joyrl-0.5.2/PKG-INFO
--rw-r--r--   0 jj         (502) staff       (20)    10785 2024-01-26 03:07:50.000000 joyrl-0.5.2/README.md
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.731581 joyrl-0.5.2/joyrl/
--rw-r--r--   0 jj         (502) staff       (20)      375 2024-01-27 14:54:03.000000 joyrl-0.5.2/joyrl/__init__.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.733851 joyrl-0.5.2/joyrl/algos/
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.735008 joyrl-0.5.2/joyrl/algos/DDPG/
--rw-r--r--   0 jj         (502) staff       (20)        0 2023-12-24 11:13:11.000000 joyrl-0.5.2/joyrl/algos/DDPG/__init__.py
--rw-r--r--   0 jj         (502) staff       (20)     1517 2024-01-25 04:01:39.000000 joyrl-0.5.2/joyrl/algos/DDPG/config.py
--rw-r--r--   0 jj         (502) staff       (20)      152 2023-12-24 11:13:11.000000 joyrl-0.5.2/joyrl/algos/DDPG/data_handler.py
--rw-r--r--   0 jj         (502) staff       (20)     5540 2024-01-27 14:55:47.000000 joyrl-0.5.2/joyrl/algos/DDPG/policy.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.736419 joyrl-0.5.2/joyrl/algos/DQN/
--rw-rw-r--   0 jj         (502) staff       (20)        0 2023-12-20 15:39:18.000000 joyrl-0.5.2/joyrl/algos/DQN/__init__.py
--rw-rw-r--   0 jj         (502) staff       (20)     1950 2024-01-22 15:09:56.000000 joyrl-0.5.2/joyrl/algos/DQN/config.py
--rw-rw-r--   0 jj         (502) staff       (20)      158 2023-12-20 15:39:18.000000 joyrl-0.5.2/joyrl/algos/DQN/data_handler.py
--rw-r--r--   0 jj         (502) staff       (20)     3507 2024-01-27 04:00:09.000000 joyrl-0.5.2/joyrl/algos/DQN/policy.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.738139 joyrl-0.5.2/joyrl/algos/DoubleDQN/
--rw-r--r--   0 jj         (502) staff       (20)        0 2023-12-22 05:01:02.000000 joyrl-0.5.2/joyrl/algos/DoubleDQN/__init__.py
--rw-r--r--   0 jj         (502) staff       (20)     1703 2024-01-26 02:14:47.000000 joyrl-0.5.2/joyrl/algos/DoubleDQN/config.py
--rw-r--r--   0 jj         (502) staff       (20)      350 2023-12-25 01:28:26.000000 joyrl-0.5.2/joyrl/algos/DoubleDQN/data_handler.py
--rw-r--r--   0 jj         (502) staff       (20)     3696 2024-01-27 04:00:29.000000 joyrl-0.5.2/joyrl/algos/DoubleDQN/policy.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.739527 joyrl-0.5.2/joyrl/algos/DuelingDQN/
--rw-r--r--   0 jj         (502) staff       (20)        0 2023-12-22 05:01:02.000000 joyrl-0.5.2/joyrl/algos/DuelingDQN/__init__.py
--rw-r--r--   0 jj         (502) staff       (20)      907 2024-01-22 15:09:56.000000 joyrl-0.5.2/joyrl/algos/DuelingDQN/config.py
--rw-r--r--   0 jj         (502) staff       (20)      337 2023-12-25 01:28:26.000000 joyrl-0.5.2/joyrl/algos/DuelingDQN/data_handler.py
--rw-r--r--   0 jj         (502) staff       (20)     3948 2024-01-25 01:58:33.000000 joyrl-0.5.2/joyrl/algos/DuelingDQN/policy.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.740776 joyrl-0.5.2/joyrl/algos/NoisyDQN/
--rw-r--r--   0 jj         (502) staff       (20)      184 2023-12-22 05:01:23.000000 joyrl-0.5.2/joyrl/algos/NoisyDQN/__init__.py
--rw-r--r--   0 jj         (502) staff       (20)     1071 2024-01-22 15:09:56.000000 joyrl-0.5.2/joyrl/algos/NoisyDQN/config.py
--rw-r--r--   0 jj         (502) staff       (20)      341 2023-12-25 01:28:26.000000 joyrl-0.5.2/joyrl/algos/NoisyDQN/data_handler.py
--rw-r--r--   0 jj         (502) staff       (20)     4445 2024-01-25 01:58:33.000000 joyrl-0.5.2/joyrl/algos/NoisyDQN/policy.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.742430 joyrl-0.5.2/joyrl/algos/PPO/
--rw-r--r--   0 jj         (502) staff       (20)        0 2023-12-22 05:01:02.000000 joyrl-0.5.2/joyrl/algos/PPO/__init__.py
--rw-r--r--   0 jj         (502) staff       (20)     2023 2024-01-26 04:28:23.000000 joyrl-0.5.2/joyrl/algos/PPO/config.py
--rw-r--r--   0 jj         (502) staff       (20)     5297 2024-01-27 10:30:47.000000 joyrl-0.5.2/joyrl/algos/PPO/data_handler.py
--rw-r--r--   0 jj         (502) staff       (20)     7837 2024-01-26 05:22:19.000000 joyrl-0.5.2/joyrl/algos/PPO/policy.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.743476 joyrl-0.5.2/joyrl/algos/QLearning/
--rw-r--r--   0 jj         (502) staff       (20)        0 2023-12-24 11:13:11.000000 joyrl-0.5.2/joyrl/algos/QLearning/__init__.py
--rw-r--r--   0 jj         (502) staff       (20)      431 2023-12-24 11:13:11.000000 joyrl-0.5.2/joyrl/algos/QLearning/config.py
--rw-r--r--   0 jj         (502) staff       (20)     1300 2024-01-13 10:02:14.000000 joyrl-0.5.2/joyrl/algos/QLearning/data_handler.py
--rw-r--r--   0 jj         (502) staff       (20)     1964 2024-01-13 10:26:43.000000 joyrl-0.5.2/joyrl/algos/QLearning/policy.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.744428 joyrl-0.5.2/joyrl/algos/Sarsa/
--rw-r--r--   0 jj         (502) staff       (20)        0 2024-01-13 10:35:16.000000 joyrl-0.5.2/joyrl/algos/Sarsa/__init__.py
--rw-r--r--   0 jj         (502) staff       (20)      431 2024-01-13 10:35:16.000000 joyrl-0.5.2/joyrl/algos/Sarsa/config.py
--rw-r--r--   0 jj         (502) staff       (20)     1300 2024-01-13 10:35:16.000000 joyrl-0.5.2/joyrl/algos/Sarsa/data_handler.py
--rw-r--r--   0 jj         (502) staff       (20)     2144 2024-01-13 10:37:45.000000 joyrl-0.5.2/joyrl/algos/Sarsa/policy.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.745649 joyrl-0.5.2/joyrl/algos/TD3/
--rw-r--r--   0 jj         (502) staff       (20)        0 2023-12-25 01:28:26.000000 joyrl-0.5.2/joyrl/algos/TD3/__init__.py
--rw-r--r--   0 jj         (502) staff       (20)     1277 2024-01-27 03:54:20.000000 joyrl-0.5.2/joyrl/algos/TD3/config.py
--rw-r--r--   0 jj         (502) staff       (20)      153 2023-12-25 01:28:26.000000 joyrl-0.5.2/joyrl/algos/TD3/data_handler.py
--rw-r--r--   0 jj         (502) staff       (20)     7334 2024-01-27 14:52:40.000000 joyrl-0.5.2/joyrl/algos/TD3/policy.py
--rw-r--r--   0 jj         (502) staff       (20)      366 2023-12-25 04:52:47.000000 joyrl-0.5.2/joyrl/algos/__init__.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.749130 joyrl-0.5.2/joyrl/algos/base/
--rw-rw-r--   0 jj         (502) staff       (20)        0 2023-12-20 15:39:18.000000 joyrl-0.5.2/joyrl/algos/base/__init__.py
--rw-r--r--   0 jj         (502) staff       (20)    10028 2024-01-27 14:46:59.000000 joyrl-0.5.2/joyrl/algos/base/action_layer.py
--rw-r--r--   0 jj         (502) staff       (20)     8643 2024-01-25 05:26:08.000000 joyrl-0.5.2/joyrl/algos/base/base_layer.py
--rw-rw-r--   0 jj         (502) staff       (20)    86085 2024-01-27 14:50:46.000000 joyrl-0.5.2/joyrl/algos/base/buffer.py
--rw-r--r--   0 jj         (502) staff       (20)     1963 2024-01-27 03:58:27.000000 joyrl-0.5.2/joyrl/algos/base/data_handler.py
--rw-rw-r--   0 jj         (502) staff       (20)      131 2023-12-20 15:39:18.000000 joyrl-0.5.2/joyrl/algos/base/experience.py
--rw-r--r--   0 jj         (502) staff       (20)    14349 2024-01-26 02:00:43.000000 joyrl-0.5.2/joyrl/algos/base/network.py
--rw-rw-r--   0 jj         (502) staff       (20)     1313 2023-12-20 15:39:18.000000 joyrl-0.5.2/joyrl/algos/base/noise.py
--rw-rw-r--   0 jj         (502) staff       (20)     2407 2024-01-07 16:39:12.000000 joyrl-0.5.2/joyrl/algos/base/optm.py
--rw-r--r--   0 jj         (502) staff       (20)     7324 2024-01-27 14:46:11.000000 joyrl-0.5.2/joyrl/algos/base/policy.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.751949 joyrl-0.5.2/joyrl/envs/
--rw-r--r--   0 jj         (502) staff       (20)       51 2023-12-22 05:01:23.000000 joyrl-0.5.2/joyrl/envs/__init__.py
--rw-r--r--   0 jj         (502) staff       (20)     4258 2023-12-22 05:01:02.000000 joyrl-0.5.2/joyrl/envs/blackjack.py
--rw-r--r--   0 jj         (502) staff       (20)     2706 2023-12-22 05:01:02.000000 joyrl-0.5.2/joyrl/envs/cliff_walking.py
--rw-r--r--   0 jj         (502) staff       (20)     3871 2023-12-22 05:01:02.000000 joyrl-0.5.2/joyrl/envs/gridworld.py
--rw-r--r--   0 jj         (502) staff       (20)     3485 2023-12-22 05:01:02.000000 joyrl-0.5.2/joyrl/envs/gridworld_env.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.752686 joyrl-0.5.2/joyrl/envs/gym/
--rw-r--r--   0 jj         (502) staff       (20)      221 2024-01-10 05:19:23.000000 joyrl-0.5.2/joyrl/envs/gym/__init__.py
--rw-r--r--   0 jj         (502) staff       (20)      525 2024-01-13 10:45:55.000000 joyrl-0.5.2/joyrl/envs/gym/config.py
--rw-r--r--   0 jj         (502) staff       (20)     5754 2024-01-25 16:38:25.000000 joyrl-0.5.2/joyrl/envs/gym/wrappers.py
--rw-r--r--   0 jj         (502) staff       (20)     9890 2023-12-22 05:01:23.000000 joyrl-0.5.2/joyrl/envs/racetrack.py
--rw-r--r--   0 jj         (502) staff       (20)     1445 2023-12-25 01:28:26.000000 joyrl-0.5.2/joyrl/envs/register.py
--rw-r--r--   0 jj         (502) staff       (20)     1311 2023-12-22 05:01:02.000000 joyrl-0.5.2/joyrl/envs/stochastic_mdp.py
--rw-r--r--   0 jj         (502) staff       (20)     2615 2023-12-22 05:01:02.000000 joyrl-0.5.2/joyrl/envs/windy_gridworld.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.756971 joyrl-0.5.2/joyrl/framework/
--rw-rw-r--   0 jj         (502) staff       (20)        0 2023-12-20 15:39:18.000000 joyrl-0.5.2/joyrl/framework/__init__.py
--rw-r--r--   0 jj         (502) staff       (20)     1247 2024-01-05 01:35:40.000000 joyrl-0.5.2/joyrl/framework/base.py
--rw-r--r--   0 jj         (502) staff       (20)     3929 2024-01-21 10:07:31.000000 joyrl-0.5.2/joyrl/framework/collector.py
--rw-r--r--   0 jj         (502) staff       (20)     2235 2024-01-25 02:01:44.000000 joyrl-0.5.2/joyrl/framework/config.py
--rw-r--r--   0 jj         (502) staff       (20)     6383 2024-01-23 05:30:05.000000 joyrl-0.5.2/joyrl/framework/interactor.py
--rw-r--r--   0 jj         (502) staff       (20)     4010 2024-01-15 15:49:09.000000 joyrl-0.5.2/joyrl/framework/learner.py
--rw-r--r--   0 jj         (502) staff       (20)      819 2024-01-05 01:35:40.000000 joyrl-0.5.2/joyrl/framework/message.py
--rw-r--r--   0 jj         (502) staff       (20)     2966 2024-01-21 09:45:29.000000 joyrl-0.5.2/joyrl/framework/policy_mgr.py
--rw-r--r--   0 jj         (502) staff       (20)     5236 2024-01-11 05:19:23.000000 joyrl-0.5.2/joyrl/framework/recorder.py
--rw-r--r--   0 jj         (502) staff       (20)     3659 2024-01-13 10:02:14.000000 joyrl-0.5.2/joyrl/framework/tester.py
--rw-rw-r--   0 jj         (502) staff       (20)     2242 2024-01-03 09:16:07.000000 joyrl-0.5.2/joyrl/framework/tracker.py
--rw-r--r--   0 jj         (502) staff       (20)     5644 2024-01-21 10:01:28.000000 joyrl-0.5.2/joyrl/framework/trainer.py
--rw-r--r--   0 jj         (502) staff       (20)     8237 2024-01-25 16:58:56.000000 joyrl-0.5.2/joyrl/run.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.757754 joyrl-0.5.2/joyrl/scripts/
--rw-rw-r--   0 jj         (502) staff       (20)      184 2023-12-22 06:07:34.000000 joyrl-0.5.2/joyrl/scripts/__init__.py
--rw-r--r--   0 jj         (502) staff       (20)      520 2023-12-22 06:07:35.000000 joyrl-0.5.2/joyrl/scripts/scripts.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.758773 joyrl-0.5.2/joyrl/utils/
--rw-r--r--   0 jj         (502) staff       (20)        1 2023-12-22 05:01:23.000000 joyrl-0.5.2/joyrl/utils/__init__.py
--rw-rw-r--   0 jj         (502) staff       (20)        0 2023-12-20 15:39:18.000000 joyrl-0.5.2/joyrl/utils/plot.py
--rw-r--r--   0 jj         (502) staff       (20)    37103 2024-01-05 01:35:40.000000 joyrl-0.5.2/joyrl/utils/utils.py
-drwxr-xr-x   0 jj         (502) staff       (20)        0 2024-01-27 14:58:05.733602 joyrl-0.5.2/joyrl.egg-info/
--rw-r--r--   0 jj         (502) staff       (20)    11227 2024-01-27 14:58:05.000000 joyrl-0.5.2/joyrl.egg-info/PKG-INFO
--rw-r--r--   0 jj         (502) staff       (20)     2430 2024-01-27 14:58:05.000000 joyrl-0.5.2/joyrl.egg-info/SOURCES.txt
--rw-r--r--   0 jj         (502) staff       (20)        1 2024-01-27 14:58:05.000000 joyrl-0.5.2/joyrl.egg-info/dependency_links.txt
--rw-r--r--   0 jj         (502) staff       (20)       54 2024-01-27 14:58:05.000000 joyrl-0.5.2/joyrl.egg-info/entry_points.txt
--rw-r--r--   0 jj         (502) staff       (20)      350 2024-01-27 14:58:05.000000 joyrl-0.5.2/joyrl.egg-info/requires.txt
--rw-r--r--   0 jj         (502) staff       (20)        6 2024-01-27 14:58:05.000000 joyrl-0.5.2/joyrl.egg-info/top_level.txt
--rw-r--r--   0 jj         (502) staff       (20)      940 2024-01-27 14:58:05.760487 joyrl-0.5.2/setup.cfg
--rw-r--r--   0 jj         (502) staff       (20)     2057 2023-12-24 11:39:41.000000 joyrl-0.5.2/setup.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.951351 joyrl-0.6.0/
+-rw-r--r--   0 johnjim    (501) staff       (20)     1077 2024-02-25 07:46:04.000000 joyrl-0.6.0/LICENSE
+-rw-r--r--   0 johnjim    (501) staff       (20)    11637 2024-06-01 09:12:28.951111 joyrl-0.6.0/PKG-INFO
+-rw-r--r--   0 johnjim    (501) staff       (20)    10670 2024-06-01 08:59:02.000000 joyrl-0.6.0/README.md
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.940184 joyrl-0.6.0/joyrl/
+-rw-r--r--   0 johnjim    (501) staff       (20)      375 2024-06-01 08:57:47.000000 joyrl-0.6.0/joyrl/__init__.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.941102 joyrl-0.6.0/joyrl/algos/
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.941565 joyrl-0.6.0/joyrl/algos/DDPG/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DDPG/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1517 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DDPG/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      152 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DDPG/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5540 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DDPG/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.942042 joyrl-0.6.0/joyrl/algos/DQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1950 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      158 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3507 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.942545 joyrl-0.6.0/joyrl/algos/DoubleDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DoubleDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1703 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DoubleDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      350 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DoubleDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3696 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DoubleDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.943024 joyrl-0.6.0/joyrl/algos/DuelingDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DuelingDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      907 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DuelingDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      337 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DuelingDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3948 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/DuelingDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.943477 joyrl-0.6.0/joyrl/algos/NoisyDQN/
+-rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/NoisyDQN/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1071 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/NoisyDQN/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      341 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/NoisyDQN/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4445 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/NoisyDQN/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.943938 joyrl-0.6.0/joyrl/algos/PPO/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/PPO/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2071 2024-05-09 17:05:41.000000 joyrl-0.6.0/joyrl/algos/PPO/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3195 2024-06-01 05:12:21.000000 joyrl-0.6.0/joyrl/algos/PPO/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     9208 2024-05-27 16:17:38.000000 joyrl-0.6.0/joyrl/algos/PPO/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.944383 joyrl-0.6.0/joyrl/algos/QLearning/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/QLearning/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/QLearning/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.0/joyrl/algos/QLearning/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1964 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/QLearning/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.944886 joyrl-0.6.0/joyrl/algos/Sarsa/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/Sarsa/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      431 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/Sarsa/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1302 2024-05-27 05:48:19.000000 joyrl-0.6.0/joyrl/algos/Sarsa/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2144 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/Sarsa/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.945330 joyrl-0.6.0/joyrl/algos/TD3/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/TD3/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1277 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/TD3/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      153 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/TD3/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7726 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/TD3/policy.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      366 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/__init__.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.946649 joyrl-0.6.0/joyrl/algos/base/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/base/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    10713 2024-05-26 12:17:32.000000 joyrl-0.6.0/joyrl/algos/base/action_layer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     8643 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/base/base_layer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    86089 2024-06-01 05:31:25.000000 joyrl-0.6.0/joyrl/algos/base/buffer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2755 2024-06-01 05:12:03.000000 joyrl-0.6.0/joyrl/algos/base/data_handler.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      131 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/base/experience.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    14978 2024-05-27 01:50:26.000000 joyrl-0.6.0/joyrl/algos/base/network.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1313 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/base/noise.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2407 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/algos/base/optm.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7605 2024-05-27 15:36:54.000000 joyrl-0.6.0/joyrl/algos/base/policy.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.947711 joyrl-0.6.0/joyrl/envs/
+-rw-r--r--   0 johnjim    (501) staff       (20)       51 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/envs/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4258 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/envs/blackjack.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2706 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/envs/cliff_walking.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3871 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/envs/gridworld.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3485 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/envs/gridworld_env.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.948078 joyrl-0.6.0/joyrl/envs/gym/
+-rw-r--r--   0 johnjim    (501) staff       (20)      221 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/envs/gym/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      525 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/envs/gym/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    11068 2024-05-09 16:41:09.000000 joyrl-0.6.0/joyrl/envs/gym/wrappers.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     9890 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/envs/racetrack.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1445 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/envs/register.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1311 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/envs/stochastic_mdp.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2615 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/envs/windy_gridworld.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.949790 joyrl-0.6.0/joyrl/framework/
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/framework/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     1069 2024-05-30 09:43:52.000000 joyrl-0.6.0/joyrl/framework/base.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     4442 2024-06-01 08:53:39.000000 joyrl-0.6.0/joyrl/framework/collector.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2294 2024-06-01 06:35:14.000000 joyrl-0.6.0/joyrl/framework/config.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5619 2024-06-01 08:53:09.000000 joyrl-0.6.0/joyrl/framework/interactor.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2874 2024-06-01 08:53:20.000000 joyrl-0.6.0/joyrl/framework/learner.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      821 2024-05-28 01:37:10.000000 joyrl-0.6.0/joyrl/framework/message.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2923 2024-06-01 03:33:53.000000 joyrl-0.6.0/joyrl/framework/policy_mgr.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     5272 2024-05-30 09:48:58.000000 joyrl-0.6.0/joyrl/framework/recorder.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     3961 2024-05-31 03:30:30.000000 joyrl-0.6.0/joyrl/framework/tester.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2242 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/framework/tracker.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     7020 2024-06-01 08:53:33.000000 joyrl-0.6.0/joyrl/framework/trainer.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     2524 2024-05-31 14:51:57.000000 joyrl-0.6.0/joyrl/framework/utils.py
+-rw-r--r--   0 johnjim    (501) staff       (20)     8061 2024-06-01 08:57:32.000000 joyrl-0.6.0/joyrl/run.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.950014 joyrl-0.6.0/joyrl/scripts/
+-rw-r--r--   0 johnjim    (501) staff       (20)      184 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/scripts/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)      520 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/scripts/scripts.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.950314 joyrl-0.6.0/joyrl/utils/
+-rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/utils/__init__.py
+-rw-r--r--   0 johnjim    (501) staff       (20)        0 2024-02-25 07:46:04.000000 joyrl-0.6.0/joyrl/utils/plot.py
+-rw-r--r--   0 johnjim    (501) staff       (20)    37181 2024-05-30 09:48:17.000000 joyrl-0.6.0/joyrl/utils/utils.py
+drwxr-xr-x   0 johnjim    (501) staff       (20)        0 2024-06-01 09:12:28.950556 joyrl-0.6.0/joyrl.egg-info/
+-rw-r--r--   0 johnjim    (501) staff       (20)    11637 2024-06-01 09:12:28.000000 joyrl-0.6.0/joyrl.egg-info/PKG-INFO
+-rw-r--r--   0 johnjim    (501) staff       (20)     2455 2024-06-01 09:12:28.000000 joyrl-0.6.0/joyrl.egg-info/SOURCES.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)        1 2024-06-01 09:12:28.000000 joyrl-0.6.0/joyrl.egg-info/dependency_links.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)       53 2024-06-01 09:12:28.000000 joyrl-0.6.0/joyrl.egg-info/entry_points.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)      256 2024-06-01 09:12:28.000000 joyrl-0.6.0/joyrl.egg-info/requires.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)        6 2024-06-01 09:12:28.000000 joyrl-0.6.0/joyrl.egg-info/top_level.txt
+-rw-r--r--   0 johnjim    (501) staff       (20)      940 2024-06-01 09:12:28.951684 joyrl-0.6.0/setup.cfg
+-rw-r--r--   0 johnjim    (501) staff       (20)     1886 2024-06-01 09:01:11.000000 joyrl-0.6.0/setup.py
```

### Comparing `joyrl-0.5.2/LICENSE` & `joyrl-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/PKG-INFO` & `joyrl-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,25 @@
-Metadata-Version: 2.1
-Name: joyrl
-Version: 0.5.2
-Summary: A Library for Deep Reinforcement Learning
-Home-page: https://github.com/datawhalechina/joyrl
-Author: johnjim0816
-Author-email: johnjim0816@gmail.com
-License: MIT
-Keywords: reinforcement learning platform pytorch
-Platform: any
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: atari
-Provides-Extra: mujoco
-Provides-Extra: pybullet
-License-File: LICENSE
-
 # JoyRL
 
 [![PyPI](https://img.shields.io/pypi/v/joyrl)](https://pypi.org/project/joyrl/)  [![GitHub issues](https://img.shields.io/github/issues/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/issues) [![GitHub stars](https://img.shields.io/github/stars/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/stargazers) [![GitHub forks](https://img.shields.io/github/forks/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/network) [![GitHub license](https://img.shields.io/github/license/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/blob/master/LICENSE)
 
 `JoyRL` is a parallel reinforcement learning library based on PyTorch and Ray. Unlike existing RL libraries, `JoyRL` is helping users to release the burden of implementing algorithms with tough details, unfriendly APIs, and etc. JoyRL is designed for users to train and test RL algorithms with **only hyperparameters configuration**, which is mush easier for beginners to learn and use. Also, JoyRL supports plenties of state-of-art RL algorithms including **RLHF(core of ChatGPT)**(See algorithms below). JoyRL provides a **modularized framework** for users as well to customize their own algorithms and environments. 
 
 ## Install
 
 ⚠️ Note that donot install JoyRL through any mirror image!!!
 
 ```bash
 # you need to install Anaconda first
-conda create -n joyrl python=3.8
+conda create -n joyrl python=3.10
 conda activate joyrl
 pip install -U joyrl
 ```
 
-Torch install:
-
-Pip install is recommended, but if you encounter network error, you can try conda install or pip install with mirrors.
+Torch GPU install:
 
 ```bash
 # pip CPU only
 pip install torch==1.10.0 torchvision==0.11.0 torchaudio==0.10.0
 # if network error, then GPU with mirror image
 pip install torch==1.10.0+cu113 torchvision==0.11.0+cu113 torchaudio==0.10.0 --extra-index-url https://download.pytorch.org/whl/cu113
 # CPU only
@@ -126,9 +107,8 @@
         <td>
             <a href="https://github.com/yyysjz1997"><img width="70" height="70" src="https://github.com/yyysjz1997.png?s=40" alt="pic"></a><br>
             <a href="https://github.com/yyysjz1997">Yiyuan Yang</a> 
             <p>University of Oxford</p>
         </td>
     </tr>
   </tbody>
-</table>
-
+</table>
```

### Comparing `joyrl-0.5.2/README.md` & `joyrl-0.6.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,57 @@
+Metadata-Version: 2.1
+Name: joyrl
+Version: 0.6.0
+Summary: A Library for Deep Reinforcement Learning
+Home-page: https://github.com/datawhalechina/joyrl
+Author: johnjim0816
+Author-email: johnjim0816@gmail.com
+License: MIT
+Keywords: reinforcement learning platform pytorch
+Platform: any
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ray[default]==2.6.3
+Requires-Dist: torch==2.2.1
+Requires-Dist: torchaudio==2.2.1
+Requires-Dist: torchvision==0.17.1
+Requires-Dist: gymnasium==0.29.1
+Requires-Dist: tensorboard==2.16.2
+Requires-Dist: matplotlib==3.8.4
+Requires-Dist: seaborn==0.13.2
+Requires-Dist: dill==0.3.8
+Requires-Dist: scipy==1.13.0
+Requires-Dist: pygame==2.5.2
+Provides-Extra: atari
+Requires-Dist: atari_py; extra == "atari"
+Requires-Dist: opencv-python; extra == "atari"
+Provides-Extra: mujoco
+Requires-Dist: mujoco_py; extra == "mujoco"
+Provides-Extra: pybullet
+Requires-Dist: pybullet; extra == "pybullet"
+
 # JoyRL
 
 [![PyPI](https://img.shields.io/pypi/v/joyrl)](https://pypi.org/project/joyrl/)  [![GitHub issues](https://img.shields.io/github/issues/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/issues) [![GitHub stars](https://img.shields.io/github/stars/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/stargazers) [![GitHub forks](https://img.shields.io/github/forks/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/network) [![GitHub license](https://img.shields.io/github/license/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/blob/master/LICENSE)
 
 `JoyRL` is a parallel reinforcement learning library based on PyTorch and Ray. Unlike existing RL libraries, `JoyRL` is helping users to release the burden of implementing algorithms with tough details, unfriendly APIs, and etc. JoyRL is designed for users to train and test RL algorithms with **only hyperparameters configuration**, which is mush easier for beginners to learn and use. Also, JoyRL supports plenties of state-of-art RL algorithms including **RLHF(core of ChatGPT)**(See algorithms below). JoyRL provides a **modularized framework** for users as well to customize their own algorithms and environments. 
 
 ## Install
 
 ⚠️ Note that donot install JoyRL through any mirror image!!!
 
 ```bash
 # you need to install Anaconda first
-conda create -n joyrl python=3.8
+conda create -n joyrl python=3.10
 conda activate joyrl
 pip install -U joyrl
 ```
 
-Torch install:
-
-Pip install is recommended, but if you encounter network error, you can try conda install or pip install with mirrors.
+Torch GPU install:
 
 ```bash
 # pip CPU only
 pip install torch==1.10.0 torchvision==0.11.0 torchaudio==0.10.0
 # if network error, then GPU with mirror image
 pip install torch==1.10.0+cu113 torchvision==0.11.0+cu113 torchaudio==0.10.0 --extra-index-url https://download.pytorch.org/whl/cu113
 # CPU only
@@ -109,8 +139,8 @@
         <td>
             <a href="https://github.com/yyysjz1997"><img width="70" height="70" src="https://github.com/yyysjz1997.png?s=40" alt="pic"></a><br>
             <a href="https://github.com/yyysjz1997">Yiyuan Yang</a> 
             <p>University of Oxford</p>
         </td>
     </tr>
   </tbody>
-</table>
+</table>
```

### Comparing `joyrl-0.5.2/joyrl/algos/DDPG/config.py` & `joyrl-0.6.0/joyrl/algos/DDPG/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/DDPG/policy.py` & `joyrl-0.6.0/joyrl/algos/DDPG/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/DQN/config.py` & `joyrl-0.6.0/joyrl/algos/DQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/DQN/policy.py` & `joyrl-0.6.0/joyrl/algos/DQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/DoubleDQN/config.py` & `joyrl-0.6.0/joyrl/algos/DoubleDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/DoubleDQN/policy.py` & `joyrl-0.6.0/joyrl/algos/DoubleDQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/DuelingDQN/config.py` & `joyrl-0.6.0/joyrl/algos/DuelingDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/DuelingDQN/policy.py` & `joyrl-0.6.0/joyrl/algos/DuelingDQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/NoisyDQN/config.py` & `joyrl-0.6.0/joyrl/algos/NoisyDQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/NoisyDQN/policy.py` & `joyrl-0.6.0/joyrl/algos/NoisyDQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/PPO/config.py` & `joyrl-0.6.0/joyrl/algos/PPO/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-02-20 21:53:39
 LastEditor: JiangJi
-LastEditTime: 2024-01-26 12:28:23
+LastEditTime: 2024-05-10 01:05:41
 Discription: 
 '''
 class AlgoConfig(object):
     def __init__(self):
         self.independ_actor = True # whether to use independent actor
         # whether actor and critic share the same optimizer
         self.share_optimizer = False # if True, lr for actor and critic will be the same
         self.ppo_type = 'clip' # clip or kl
         self.eps_clip = 0.2 # clip parameter for PPO
+        self.gae_lambda = 0.95 # lambda for GAE
         # for kl penalty version of PPO
         self.kl_target = 0.1 # target KL divergence
         self.kl_lambda = 0.5 # lambda for KL penalty, 0.5 is the default value in the paper
         self.kl_beta = 1.5 # beta for KL penalty, 1.5 is the default value in the paper
         self.kl_alpha = 2 # alpha for KL penalty, 2 is the default value in the paper
         self.action_type_list = "continuous" # continuous action space
         self.gamma = 0.99 # discount factor
```

### Comparing `joyrl-0.5.2/joyrl/algos/QLearning/data_handler.py` & `joyrl-0.6.0/joyrl/algos/QLearning/data_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
     def sample_training_data(self):
         ''' sample training data from buffer
         '''
         if len(self.buffer) == 0:
             return None
         exp = self.buffer.pop()[0]
-        return self.handle_exps_before_train(exp)
-    def handle_exps_before_train(self, exp, **kwargs):
+        return self._handle_exps_before_train(exp)
+    def _handle_exps_before_train(self, exp, **kwargs):
         ''' convert exps to training data
         '''
         state = np.array(exp.state)
         action = np.array(exp.action)
         reward = np.array(exp.reward)
         next_state = np.array(exp.next_state)
         done = np.array(exp.done)
```

### Comparing `joyrl-0.5.2/joyrl/algos/QLearning/policy.py` & `joyrl-0.6.0/joyrl/algos/QLearning/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/Sarsa/data_handler.py` & `joyrl-0.6.0/joyrl/algos/Sarsa/data_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
     def sample_training_data(self):
         ''' sample training data from buffer
         '''
         if len(self.buffer) == 0:
             return None
         exp = self.buffer.pop()[0]
-        return self.handle_exps_before_train(exp)
-    def handle_exps_before_train(self, exp, **kwargs):
+        return self._handle_exps_before_train(exp)
+    def _handle_exps_before_train(self, exp, **kwargs):
         ''' convert exps to training data
         '''
         state = np.array(exp.state)
         action = np.array(exp.action)
         reward = np.array(exp.reward)
         next_state = np.array(exp.next_state)
         done = np.array(exp.done)
```

### Comparing `joyrl-0.5.2/joyrl/algos/Sarsa/policy.py` & `joyrl-0.6.0/joyrl/algos/Sarsa/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/TD3/config.py` & `joyrl-0.6.0/joyrl/algos/TD3/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/TD3/policy.py` & `joyrl-0.6.0/joyrl/algos/TD3/policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
         self.expl_noise = cfg.expl_noise # std of Gaussian exploration noise
         self.policy_freq = cfg.policy_freq # policy update frequency
         self.tau = cfg.tau
         self.sample_count = 0
         self.update_step = 0
         self.explore_steps = cfg.explore_steps # exploration steps before training
         self.device = torch.device(cfg.device)
+        self.action_high = torch.FloatTensor(self.action_space.high).to(self.device)
+        self.action_low = torch.FloatTensor(self.action_space.low).to(self.device)
         self.action_scale = torch.tensor((self.action_space.high - self.action_space.low)/2, device=self.device, dtype=torch.float32)
         self.action_bias = torch.tensor((self.action_space.high + self.action_space.low)/2, device=self.device, dtype=torch.float32)
         self.create_graph() # create graph and optimizer
         self.create_summary() # create summary
         self.to(self.device)
 
     def get_action_size(self):
@@ -85,33 +87,34 @@
 
     def sample_action(self, state,  **kwargs):
         self.sample_count += 1
         if self.sample_count < self.explore_steps:
             return self.action_space.sample()
         else:
             action = self.predict_action(state, **kwargs)
-            action_noise = np.random.normal(0, self.action_scale * self.expl_noise, size=self.action_size_list[0])
+            action_noise = self.expl_noise * np.random.normal(0, self.action_scale.cpu().detach().numpy(), size=self.action_size_list[0])
             action = (action + action_noise).clip(self.action_space.low, self.action_space.high)
             return action
 
     @torch.no_grad()
     def predict_action(self, state,  **kwargs):
-        state = [torch.tensor(state, device=self.device, dtype=torch.float32).unsqueeze(dim=0)]
+        state = [torch.tensor(np.array(state), device=self.device, dtype=torch.float32).unsqueeze(dim=0)]
         _ = self.actor(state)
         action = self.actor.action_layers.get_actions()
         return action[0]
 
     def learn(self, **kwargs):
         # state, action, reward, next_state, done = self.memory.sample(self.batch_size)
         states, actions, next_states, rewards, dones = kwargs.get('states'), kwargs.get('actions'), kwargs.get('next_states'), kwargs.get('rewards'), kwargs.get('dones')
    
         # update critic
         noise = (torch.randn_like(actions) * self.policy_noise).clamp(-self.noise_clip, self.noise_clip)
         next_actions = self.target_actor(next_states)[0]['mu']
-        next_actions = ((next_actions + noise) * self.action_scale + self.action_bias).clamp(-self.action_scale+self.action_bias, self.action_scale+ self.action_bias)
+        # next_actions = ((next_actions + noise) * self.action_scale + self.action_bias).clamp(-self.action_scale+self.action_bias, self.action_scale+ self.action_bias)
+        next_actions = (next_actions * self.action_scale + self.action_bias + noise).clamp(self.action_low, self.action_high)
         target_q1, target_q2 = self.target_critic_1([next_states, next_actions]).detach(), self.target_critic_2([next_states, next_actions]).detach()
         target_q = torch.min(target_q1, target_q2) # shape:[train_batch_size,n_actions]
         target_q = rewards + self.gamma * target_q * (1 - dones)
         current_q1, current_q2 = self.critic_1([states, actions]), self.critic_2([states, actions])
         # compute critic loss
         critic_1_loss = F.mse_loss(current_q1, target_q)
         critic_2_loss = F.mse_loss(current_q2, target_q)
@@ -123,15 +126,16 @@
         critic_2_loss.backward()
         self.critic_2_optimizer.step()
         self.soft_update(self.critic_1, self.target_critic_1, self.tau)
         self.soft_update(self.critic_2, self.target_critic_2, self.tau)
         # Delayed policy updates
         if self.sample_count % self.policy_freq == 0:
             # compute actor loss
-            actor_loss = -self.critic_1([states, self.actor(states)[0]['mu']]).mean()
+            act_ = self.actor(states)[0]['mu'] * self.action_scale + self.action_bias
+            actor_loss = -self.critic_1([states, act_]).mean()
             self.policy_loss = actor_loss
             self.tot_loss = self.policy_loss + self.value_loss1 + self.value_loss2
             self.actor_optimizer.zero_grad()
             actor_loss.backward()
             self.actor_optimizer.step()
             self.soft_update(self.actor, self.target_actor, self.tau)   
         self.update_step += 1
```

### Comparing `joyrl-0.5.2/joyrl/algos/base/action_layer.py` & `joyrl-0.6.0/joyrl/algos/base/action_layer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-25 09:28:26
 LastEditor: JiangJi
-LastEditTime: 2024-01-27 22:46:52
+LastEditTime: 2024-05-26 20:17:08
 Discription: 
 '''
 from enum import Enum
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.distributions import Categorical,Normal
@@ -28,18 +28,19 @@
     def __init__(self,cfg, input_size, action_dim, id = 0, **kwargs):
         super(BaseActionLayer, self).__init__()
         self.cfg = cfg
         self.id = id
 
     def get_action(self, **kwargs):
         mode = kwargs.get("mode", "sample")
+        actor_output = kwargs.get("actor_output", None)
         if mode == "sample":
-            return self.sample_action()
+            return self.sample_action(**actor_output)
         elif mode == "predict":
-            return self.predict_action()
+            return self.predict_action(**actor_output)
         else:
             raise NotImplementedError
         
 class DQNActionLayer(BaseActionLayer):
     def __init__(self, cfg, input_size, action_dim, id = 0, **kwargs):
         super(DQNActionLayer, self).__init__(cfg=cfg, input_size=input_size, action_dim=action_dim, id=id)
         self.action_dim = action_dim
@@ -163,63 +164,73 @@
 
     def forward(self,x, **kwargs):
         mu = self.mu_layer(x)
         sigma = torch.ones_like(mu) * torch.exp(self.log_std)
         # log_prob = -0.5 * (sigma.log() + ((mu - x) / sigma).pow(2) + math.log(2 * math.pi))
         # sigma = F.softplus(self.fc4(x)) + 0.001 # std of normal distribution, add a small value to avoid 0
         # sigma = torch.clamp(sigma, min=-0.25, max=0.25) # clamp the std between 0.001 and 1
-        self.mu = mu.squeeze(dim=1) # [batch_size]
-        self.sigma = sigma.squeeze(dim=1) # [batch_size]
-        output = {"mu": self.mu, "sigma": self.sigma}
+        self.mu = mu # [batch_size, 1]
+        self.sigma = sigma # [batch_size]
         self.mean = self.mu * self.action_scale + self.action_bias
         self.std = self.sigma
+        output = {"mu": self.mu, "sigma": self.sigma, "mean": self.mean, "std": self.std}
         return output
     
-    def sample_action(self):
+    def sample_action(self, **kwargs):
         ''' get action
         '''
-        dist = Normal(self.mean,self.std)
+        mean = kwargs.get("mean", None)
+        std = kwargs.get("std", None)
+        dist = Normal(mean, std)
         action = dist.sample()
-        self.log_prob = dist.log_prob(action)
-        action = torch.clamp(action, torch.tensor(self.action_low, device=self.cfg.device, dtype=torch.float32), torch.tensor(self.action_high, device=self.cfg.device, dtype=torch.float32))
-        return action.detach().cpu().numpy().item()
+        log_prob = dist.log_prob(action)
+        return {"action": action.detach().cpu().numpy().item(), "log_prob": log_prob.detach().cpu().numpy().item()}
 
-    def predict_action(self):
+
+    def predict_action(self, **kwargs):
         ''' get action
         '''
-        return self.mean.detach().cpu().numpy().item()
+        return {"action": self.mean.detach().cpu().numpy().item(), "log_prob": None}
     
-    def get_log_prob(self):
+    def get_log_prob(self, **kwargs):
+        ''' get log_probs
+        '''
+        mean = kwargs.get("mean", None)
+        std = kwargs.get("std", None)
+        dist = Normal(mean, std)
+        action = dist.sample()
         return self.log_prob
     
-    def get_log_prob_action(self, action):
+    def get_log_prob_action(self, actor_output, action):
         ''' get log_probs
         '''
         # action shape is [batch_size, action_dim]
-        dist = Normal(self.mean, self.std)
-        if not isinstance(action, torch.Tensor):
-            action = torch.tensor(action, dtype=torch.float32, device=self.mean.device)
-            # action = action.squeeze(dim=0)
+        mean = actor_output.get("mean", None)
+        std = actor_output.get("std", None)
+        dist = Normal(mean, std)
         log_prob = dist.log_prob(action)
-
         return log_prob
     
-    def get_mean_entropy(self):
+    def get_entropy(self, actor_output):
         ''' get entropy
         '''
-        dist = Normal(self.mean,self.std)
+        mean = actor_output.get("mean", None)
+        std = actor_output.get("std", None)
+        dist = Normal(mean, std)
         entropy = dist.entropy()
         entropy_mean = torch.mean(entropy)
         return entropy_mean
     
 class DPGActionLayer(BaseActionLayer):
     def __init__(self, cfg, input_size, action_dim, id = 0, **kwargs):
         super(DPGActionLayer, self).__init__(cfg=cfg, input_size=input_size, action_dim=action_dim, id=id)
-        self.action_high = self.cfg.action_high_list[self.id]
-        self.action_low = self.cfg.action_low_list[self.id]
+        # self.action_high = self.cfg.action_high_list[self.id]
+        # self.action_low = self.cfg.action_low_list[self.id]
+        self.action_high = self.cfg.action_space.high
+        self.action_low = self.cfg.action_space.low
         self.action_scale = (self.action_high - self.action_low)/2
         self.action_bias = (self.action_high + self.action_low)/2
         self.action_dim = action_dim
         self.output_size = input_size
         action_layer_cfg = LayerConfig(layer_type='linear', layer_size=[self.action_dim], activation='tanh')
         self.action_layer, layer_out_size = create_layer(self.output_size, action_layer_cfg)
         self.output_size = layer_out_size
@@ -233,28 +244,31 @@
     def get_mu(self):
         ''' get mu
         '''
         return self.mu
     
     def get_action(self, **kwargs):
         mode = kwargs.get("mode", "sample")
+        actor_output = kwargs.get("actor_output", None)
         if mode == "sample":
-            return self.sample_action()
+            return self.sample_action(actor_output)
         elif mode == "predict":
-            return self.predict_action()
+            return self.predict_action(actor_output)
         else:
             raise NotImplementedError
         
-    def sample_action(self):
+    def sample_action(self, actor_outputs):
         ''' get action
         '''
-        action = self.action_scale * self.mu + self.action_bias
+        device_ = self.mu.device 
+        action = torch.FloatTensor(self.action_scale).to(device_) * self.mu + torch.FloatTensor(self.action_bias).to(device_)
         action = action.detach().cpu().numpy()[0]
         return action
     
-    def predict_action(self):
+    def predict_action(self, actor_outputs):
         ''' get action
         '''
-        action = self.action_scale * self.mu + self.action_bias
+        device_ = self.mu.device 
+        action = torch.FloatTensor(self.action_scale).to(device_) * self.mu + torch.FloatTensor(self.action_bias).to(device_)
         action = action.detach().cpu().numpy()[0]
         return action
```

### Comparing `joyrl-0.5.2/joyrl/algos/base/base_layer.py` & `joyrl-0.6.0/joyrl/algos/base/base_layer.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/base/buffer.py` & `joyrl-0.6.0/joyrl/algos/base/buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,22 +111,24 @@
 class OnPolicyBufferQue(ReplayBufferQue):
     '''replay buffer for policy gradient based methods, each time these methods will sample all transitions
     Args:
         ReplayBufferQue (_type_): _description_
     '''
     def __init__(self, cfg: MergedConfig):
         self.cfg = cfg
-        self.buffer = deque(maxlen=128)
+        self.buffer = deque(maxlen=1)
+        
     def push(self, exps: list):
         self.buffer.append(exps)
+
     def sample(self,**kwargs):
         ''' sample all the transitions
         '''
         if len(self.buffer) == 0: return None
-        batch = self.buffer.popleft()
+        batch = self.buffer.pop()
         # batch = list(self.buffer)
         # self.buffer.clear() # on policy buffer will clear the buffer after sampling
         return batch
     
 class SumTree:
     def __init__(self, capacity):
         self.capacity = capacity
```

### Comparing `joyrl-0.5.2/joyrl/algos/base/data_handler.py` & `joyrl-0.6.0/joyrl/algos/base/data_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,77 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-02 15:02:30
 LastEditor: JiangJi
-LastEditTime: 2024-01-27 11:58:27
+LastEditTime: 2024-06-01 13:11:59
 Discription: 
 '''
 import torch
 import numpy as np
 from joyrl.algos.base.buffer import BufferCreator
 from joyrl.algos.base.experience import Exp
 
 class BaseDataHandler:
     ''' Basic data handler
     '''
     def __init__(self,cfg) -> None:
         self.cfg = cfg
         self.buffer = BufferCreator(cfg)()
         self.data_after_train = {}
-
+        
+    def _get_exp_len(self, exps, max_step: int = 1):
+        ''' get exp len
+        '''
+        exp_len = len(exps)
+        if exp_len <= max_step or exps[-1].done:
+            exp_len = max(exp_len, 0)
+        else:
+            exp_len = exp_len - max_step
+        return exp_len
+    
+    def handle_exps_after_interact(self, exps: list) -> list:
+        ''' handle exps after interact
+        '''
+        return exps
+    
     def add_exps(self, exps):
+        exps = self.handle_exps_after_interact(exps)
         self.buffer.push(exps)
         
     def sample_training_data(self):
         ''' sample training data from buffer
         '''
         exps = self.buffer.sample()
         if exps is not None:
-            return self.handle_exps_before_train(exps)
+            self._handle_exps_before_train(exps)
+            return self.data_after_train
         else:
             return None
 
-    def handle_exps_before_train(self, exps, **kwargs):
+    def _handle_exps_before_train(self, exps: list):
         ''' convert exps to training data
         '''
-        states = np.array([exp.state for exp in exps])
-        actions = np.array([exp.action for exp in exps])
-        rewards = np.array([exp.reward for exp in exps])
-        next_states = np.array([exp.next_state for exp in exps])
-        dones = np.array([exp.done for exp in exps])
-        # convert numpy to tensor
-        states = torch.tensor(states, device=self.cfg.device, dtype=torch.float32)
-        actions = torch.tensor(actions, device=self.cfg.device, dtype=torch.float32)
-        next_states = torch.tensor(next_states, device=self.cfg.device, dtype=torch.float32)
-        rewards = torch.tensor(rewards, device=self.cfg.device, dtype=torch.float32).unsqueeze(dim=1)
-        dones = torch.tensor(dones, device=self.cfg.device, dtype=torch.float32).unsqueeze(dim=1)
-        data = {'states': states, 'actions': actions, 'rewards': rewards, 'next_states': next_states, 'dones': dones}
-        return data
+        model_steps = np.array([exp.model_step for exp in exps]) # [batch_size]
+        states = np.array([exp.state for exp in exps]) # [batch_size, state_dim]
+        actions = np.array([exp.action for exp in exps]) # [batch_size, action_dim]
+        rewards = np.array([exp.reward for exp in exps]) # [batch_size]
+        next_states = np.array([exp.next_state for exp in exps]) # [batch_size, state_dim]
+        dones = np.array([exp.done for exp in exps]) # [batch_size]
+
+        # multi-head state
+        states = [ torch.tensor(states, dtype = torch.float32, device = self.cfg.device) ]
+        # multi-head action
+        actions = [ torch.tensor(actions, dtype = torch.float32, device = self.cfg.device) ]
+        rewards = torch.tensor(rewards, dtype = torch.float32, device = self.cfg.device).unsqueeze(dim=1)
+        next_states = torch.tensor(next_states, dtype = torch.float32, device = self.cfg.device)
+        dones = torch.tensor(dones, dtype = torch.float32, device = self.cfg.device).unsqueeze(dim=1)
+        
+        self.data_after_train = {'model_steps': model_steps, 'states': states, 'actions': actions, 'rewards': rewards, 'next_states': next_states, 'dones': dones}
+
     
     def handle_exps_after_train(self):
         ''' handle exps after train
         '''
         pass
```

### Comparing `joyrl-0.5.2/joyrl/algos/base/network.py` & `joyrl-0.6.0/joyrl/algos/base/network.py`

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
-LastEditTime: 2024-01-26 09:59:44
+LastEditTime: 2024-05-27 09:50:26
 Discription: 
 '''
 import copy
 import torch
 import torch.nn as nn
 from joyrl.algos.base.base_layer import create_layer, LayerConfig
 from joyrl.algos.base.action_layer import ActionLayerType, DiscreteActionLayer, ContinuousActionLayer, DPGActionLayer, DQNActionLayer
@@ -109,17 +109,17 @@
             elif action_type == ActionLayerType.DQNACTION:
                 action_layer = DQNActionLayer(self.cfg, self.input_size, action_size, id = i)
             else:
                 raise ValueError("action_type must be specified in discrete, continuous or dpg")
             self.action_layers.append(action_layer)
 
     def forward(self, x, **kwargs):
-        self.actor_outputs = []
+        self.actor_outputs = {}
         for i, action_layer in enumerate(self.action_layers):
-            self.actor_outputs.append(action_layer(x, **kwargs))
+            self.actor_outputs[i] = action_layer(x, **kwargs)
         return self.actor_outputs
     
     def get_mus(self):
         mus = []
         for _, action_layer in enumerate(self.action_layers):
             mus.append(action_layer.get_mu())
         return mus[0]
@@ -127,39 +127,52 @@
     def get_qvalues(self):
         qvalues = []
         for _, action_layer in enumerate(self.action_layers):
             qvalues.append(action_layer.get_qvalue())
         return qvalues[0]
     
     def get_actions(self, **kwargs):
+        mode = kwargs.get('mode', 'train')
+        actor_outputs = kwargs.get('actor_outputs', self.actor_outputs)
+        actions = []
+        for i, action_layer in enumerate(self.action_layers):
+            action_layer_output = action_layer.get_action(mode = mode, actor_output = actor_outputs[i])
+            actions.append(action_layer_output['action'])
+        return actions
+    
+    def get_actions_and_log_probs(self, **kwargs):
+        mode = kwargs.get('mode', 'train')
+        actor_outputs = kwargs.get('actor_outputs', self.actor_outputs)
         actions = []
+        log_probs_sum = 0
         for i, action_layer in enumerate(self.action_layers):
-            actions.append(action_layer.get_action(**kwargs))
-        return actions # [action_1, action_2, ...]
+            action_layer_output = action_layer.get_action(mode = mode, actor_output = actor_outputs[i])
+            actions.append(action_layer_output['action'])
+            log_probs_sum += action_layer_output['log_prob']
+        return actions, log_probs_sum
     
-    def get_log_probs(self):
-        return self.action_layers[0].get_log_prob()
     
-    def get_log_probs_action(self, actions):
-        return self.action_layers[0].get_log_prob_action(actions)
-        # log_prob_sum = 0
-        # for i, action_layer in enumerate(self.action_layers):
-        #     log_prob_sum += action_layer.get_log_prob(actions[i])
-        # return log_prob_sum
-    
-    def get_mean_entropy(self):
-        return self.action_layers[0].get_mean_entropy()
-        # entropy_sum = 0
-        # for i, action_layer in enumerate(self.action_layers):
-        #     entropy_sum += action_layer.get_entropy()
-        # entropy_mean = entropy_sum / len(self.action_layers)
-        # return entropy_mean
+    def get_log_probs_action(self, actor_outputs, actions):
+        log_prob_sum = 0
+        for i, action_layer in enumerate(self.action_layers):
+            actor_output = actor_outputs[i]
+            action = actions[i]
+            log_prob = action_layer.get_log_prob_action(actor_output, action)
+            log_prob_sum += log_prob
+        return log_prob_sum
     
+    def get_mean_entropy(self, actor_outputs):
+        entropy_sum = 0
+        for i, action_layer in enumerate(self.action_layers):
+            entropy_sum += action_layer.get_entropy(actor_outputs[i])
+        entropy_mean = entropy_sum / len(self.action_layers)
+        return entropy_mean
+     
 class BaseNework(nn.Module):
-    def __init__(self, cfg: MergedConfig, input_size_list, **kwargs) -> None:
+    def __init__(self, cfg: MergedConfig, input_size_list) -> None:
         super(BaseNework, self).__init__()
         self.cfg = cfg
         self.input_size_list = input_size_list
         
     def create_graph(self):
         self.branch_layers = BranchLayers(self.cfg.branch_layers, self.input_size_list)
         self.merge_layer = MergeLayer(self.cfg.merge_layers, self.branch_layers.output_size_list)
@@ -223,31 +236,30 @@
         self.branch_layers.reset_noise()
         self.merge_layer.reset_noise()
 
    
 class ActorCriticNetwork(BaseNework):
     ''' Value network, for policy-based methods,  in which the branch_layers and critic share the same network
     '''
-    def __init__(self, cfg: MergedConfig) -> None:
-        super(ActorCriticNetwork, self).__init__(cfg)
+    def __init__(self, cfg: MergedConfig, input_size_list: list) -> None:
+        super(ActorCriticNetwork, self).__init__(cfg, input_size_list)
         self.action_type_list = self.cfg.action_type_list
         self.create_graph()
         
     def create_graph(self):
-        self.branch_layers = BranchLayers(self.cfg.branch_layers, self.state_size_list)
+        self.branch_layers = BranchLayers(self.cfg.branch_layers, self.input_size_list)
         self.merge_layer = MergeLayer(self.cfg.merge_layers, self.branch_layers.output_size_list)
-        self.value_layer_cfg = LayerConfig(layer_type='linear', layer_size=[1], activation='none')
-        self.value_layer, _ = create_layer(self.merge_layer.output_size, self.value_layer_cfg)
-        self.action_layers = ActionLayers(self.cfg, self.merge_layer.output_size, self.action_type_list, self.action_size_list)
+        self.value_layer, _ = create_layer(self.merge_layer.output_size, LayerConfig(layer_type='linear', layer_size=[1], activation='none'))
+        self.action_layers = ActionLayers(self.cfg, self.merge_layer.output_size,)
         
     def forward(self, x, pre_legal_actions=None):
         x = self.branch_layers(x)
         x = self.merge_layer(x)
         value = self.value_layer(x)
-        action_outputs = self.action_layers(x, pre_legal_actions)
+        action_outputs = self.action_layers(x, pre_legal_actions = pre_legal_actions)
         return value, action_outputs
 
 
 class ActorNetwork(BaseNework):
     def __init__(self, cfg: MergedConfig, input_size_list) -> None:
         super(ActorNetwork, self).__init__(cfg, input_size_list)
         self.action_type_list = self.cfg.action_type_list
```

### Comparing `joyrl-0.5.2/joyrl/algos/base/noise.py` & `joyrl-0.6.0/joyrl/algos/base/noise.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/base/optm.py` & `joyrl-0.6.0/joyrl/algos/base/optm.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/algos/base/policy.py` & `joyrl-0.6.0/joyrl/algos/base/policy.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 import torch
 import torch.nn as nn
 import torch.optim as optim
 import numpy as np
 from collections import defaultdict
 from gymnasium.spaces import Box, Discrete
 from joyrl.algos.base.action_layer import ActionLayerType
-class BasePolicy(nn.Module):
+from joyrl.framework.config import MergedConfig
+from joyrl.algos.base.network import BaseNework
+class BasePolicy(object):
     ''' base policy for DRL
     '''
-    def __init__(self,cfg) -> None:
-        super().__init__()
+    def __init__(self, cfg : MergedConfig) -> None:
         self.cfg = cfg
         self.device = torch.device(cfg.device) 
         self.obs_space = cfg.obs_space
         self.action_space = cfg.action_space
-        self.optimizer = None
         self.policy_transition = {}
         self.data_after_train = {}
         self.get_state_size()
         self.get_action_size()
-
+        self.create_model()
+        self.create_optimizer()
+    
     def get_state_size(self):
         ''' get state size
         '''
         # state_size must be [[None, state_dim_1], [None, state_dim_2], ...]
         if isinstance(self.obs_space, Box):
             if len(self.obs_space.shape) == 3:
                 self.state_size_list = [[None, self.obs_space.shape[0], self.obs_space.shape[1], self.obs_space.shape[2]]]
@@ -54,26 +56,31 @@
         else:
             raise ValueError('action_space type error')
         setattr(self.cfg, 'action_size_list', self.action_size_list)
         setattr(self.cfg, 'action_type_list', self.action_type_list)
         setattr(self.cfg, 'action_high_list', self.action_high_list)
         setattr(self.cfg, 'action_low_list', self.action_low_list)
     
+    def create_model(self):
+        ''' create model
+        '''
+        self.model = BaseNework(self.cfg, [None, 1])
+
     def create_optimizer(self):
-        self.optimizer = optim.Adam(self.parameters(), lr=self.cfg.lr) 
+        self.optimizer = optim.Adam(self.model.parameters(), lr=self.cfg.lr) 
 
     def get_model_params(self):
         ''' get model params
         '''
-        return copy.deepcopy(self.state_dict())
+        return self.model.state_dict()
     
     def put_model_params(self, model_params):
         ''' put model params
         '''
-        self.load_state_dict(model_params)
+        self.model.load_state_dict(model_params)
 
     def get_action(self, state, **kwargs):
         ''' get action
         '''
         mode = kwargs.get('mode', None)
         if mode is None: 
             mode = 'sample' if self.cfg.mode == 'train' else 'predict'
@@ -88,14 +95,15 @@
         ''' sample action
         '''
         raise NotImplementedError
     def predict_action(self, state, **kwargs):
         ''' predict action
         '''
         raise NotImplementedError
+    
     def update_policy_transition(self):
         ''' update policy transition
         '''
         self.policy_transition = {}
         
     def get_policy_transition(self):
         return self.policy_transition
@@ -123,22 +131,22 @@
         '''
         self.data_after_train = {}
     def get_data_after_learn(self):
         return self.data_after_train
     def save_model(self, fpath):
         ''' save model
         '''
-        torch.save(self.state_dict(), fpath)
+        torch.save(self.model.state_dict(), fpath)
     def load_model(self, fpath):
         ''' load model
         '''
         try:
-            self.load_state_dict(torch.load(fpath, map_location=self.device))
+            self.model.load_state_dict(torch.load(fpath, map_location=self.device))
         except:
-            print(f"load model from {fpath} failed, try to load model from cpu")
+            print(f"[BasePolicy.load_model] load model from {fpath} failed, please check the model path!")
 
 class ToyPolicy:
     ''' base policy for traditional RL or non DRL
     '''
     def __init__(self, cfg) -> None:
         super().__init__()
         self.cfg = cfg
```

### Comparing `joyrl-0.5.2/joyrl/envs/blackjack.py` & `joyrl-0.6.0/joyrl/envs/blackjack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/envs/cliff_walking.py` & `joyrl-0.6.0/joyrl/envs/cliff_walking.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/envs/gridworld.py` & `joyrl-0.6.0/joyrl/envs/gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/envs/gridworld_env.py` & `joyrl-0.6.0/joyrl/envs/gridworld_env.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/envs/gym/config.py` & `joyrl-0.6.0/joyrl/envs/gym/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/envs/racetrack.py` & `joyrl-0.6.0/joyrl/envs/racetrack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/envs/register.py` & `joyrl-0.6.0/joyrl/envs/register.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/envs/stochastic_mdp.py` & `joyrl-0.6.0/joyrl/envs/stochastic_mdp.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/envs/windy_gridworld.py` & `joyrl-0.6.0/joyrl/envs/windy_gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/framework/base.py` & `joyrl-0.6.0/joyrl/framework/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-02 17:30:36
 LastEditor: JiangJi
-LastEditTime: 2024-01-04 23:48:51
+LastEditTime: 2024-05-30 17:43:52
 Discription: 
 '''
 import ray
 from joyrl.framework.config import MergedConfig
 from joyrl.framework.message import Msg
 from joyrl.utils.utils import Logger, create_module
 
+
 class Moduler(object):
     def __init__(self, cfg: MergedConfig, **kwargs) -> None:
         self.cfg = cfg
-        self.use_ray = kwargs.get('use_ray', False)
-        # self.logger = Logger(self.cfg.log_dir)
-        self.logger = create_module(Logger, self.use_ray, {'num_cpus':0} , self.cfg.log_dir)
+        self.name = kwargs.get('name', 'Moduler')
+        self.logger = Logger(self.cfg.log_dir, log_name = self.name)
         
     def _t_start(self):
         ''' start threads
         '''
         raise NotImplementedError
     
     def _p_start(self):
@@ -41,12 +41,8 @@
         raise NotImplementedError
     
     def run(self):
         ''' run module
         '''
         raise NotImplementedError
 
-    def ray_run(self):
-        ''' asyn run module in ray
-        '''
-        raise NotImplementedError
```

### Comparing `joyrl-0.5.2/joyrl/framework/collector.py` & `joyrl-0.6.0/joyrl/framework/collector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,105 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-22 23:02:13
 LastEditor: JiangJi
-LastEditTime: 2024-01-21 18:07:31
+LastEditTime: 2024-06-01 16:52:10
 Discription: 
 '''
 import ray
 import time
 import multiprocessing as mp
 from queue import Queue, Empty, Full
 import threading
 from joyrl.framework.message import Msg, MsgType
 from joyrl.framework.config import MergedConfig
-from joyrl.algos.base.data_handler import BaseDataHandler
 from joyrl.framework.base import Moduler
 from joyrl.utils.utils import exec_method
+from joyrl.framework.utils import DeQueue
 
 class Collector(Moduler):
     ''' Collector for collecting training data
     '''
     def __init__(self, cfg: MergedConfig, **kwargs) -> None:
         super().__init__(cfg, **kwargs)
         self.data_handler = kwargs['data_handler']
-        self._raw_exps_que = kwargs['raw_exps_que']
-        self._training_data_que = Queue(maxsize = 1)
+        self._get_training_data_time = time.time()
+        self._consumed_exp_len = 0
+        self._handle_exps_time = time.time()
+        self._produced_exp_len = 0
+        self._t_interval = 3
         self._t_start()
 
     def _t_start(self):
-        # pass
-        self._t_handle_exps = threading.Thread(target=self._handle_exps)
-        self._t_handle_exps.setDaemon(True)
-        self._t_handle_exps.start()
-        self._t_prepare_training_data = threading.Thread(target=self._prepare_training_data)
-        self._t_prepare_training_data.setDaemon(True)
-        self._t_prepare_training_data.start()  
+        exec_method(self.logger, 'info', 'get', "[Collector._t_start] Start collector!") 
 
     def pub_msg(self, msg: Msg):
         ''' publish message
         '''
         msg_type, msg_data = msg.type, msg.data
         if msg_type == MsgType.COLLECTOR_PUT_EXPS:
             exps = msg_data
-            # self.data_handler.add_exps(exps)
-            while True:
-                try:
-                    self._raw_exps_que.put(exps, block=True, timeout=0.01)
-                    break
-                except Full:
-                    exec_method(self.logger, 'warning', True, "[Collector.pub_msg] raw_exps_que is full!")
-                    time.sleep(0.002)
+            self._handle_exps(exps)
         elif msg_type == MsgType.COLLECTOR_GET_TRAINING_DATA:
             try:
-                return self._training_data_que.get(block=True,timeout=0.01)
+                training_data = self._get_training_data()
+                if training_data is None:
+                    return None
+                self._consumed_exp_len += training_data['dones'].shape[0]
+                if time.time() - self._get_training_data_time >= self._t_interval:
+                    exec_method(self.logger, 'info', 'remote', f"[Collector.pub_msg] SAMPLE CONSUMPTION SPEED per second: {self._consumed_exp_len/self._t_interval:.2f}")
+                    self._get_training_data_time = time.time()
+                    self._consumed_exp_len = 0
+                return training_data
             except Empty:
-                # exec_method(self.logger, 'warning', True, "[Collector.pub_msg] training_data_que is empty!")
+                # exec_method(self.logger, 'warning', 'get', "[Collector.pub_msg] training_data_que is empty!")
                 return None
-            # return self._get_training_data()
         elif msg_type == MsgType.COLLECTOR_GET_BUFFER_LENGTH:
             return self.get_buffer_length()
         else:
             raise NotImplementedError
 
-    def _handle_exps(self):
+    def _handle_exps(self, exps):
         ''' handle exps
         '''
-        while True:
-            try:
-                exps = self._raw_exps_que.get() # get exps from raw_exps_que
-                self.data_handler.add_exps(exps) # add exps to data handler
-                # exec_method(self.logger, 'info', True, "[Collector._handle_exps] add exps to data handler")
-            except Empty:
-                # exec_method(self.logger, 'warning', True, "[Collector._handle_exps] raw_exps_que is empty!")
-                pass
+        self._produced_exp_len += len(exps)
+        exec_method(self.data_handler, 'add_exps', 'remote', exps)
+        if time.time() - self._handle_exps_time >= self._t_interval:
+            exec_method(self.logger, 'info', 'remote', f"[Collector._handle_exps] SAMPLE PRODUCTION SPEED per second: {self._produced_exp_len/self._t_interval:.2f}")
+            self._handle_exps_time = time.time()
+            self._produced_exp_len = 0
             
     def _prepare_training_data(self):
         ''' 
         '''
         while True:
-            if not self._training_data_que.full():
-                training_data = self._get_training_data()
-                if training_data is not None:
-                    try:
-                        self._training_data_que.put(training_data, block = True, timeout=0.1)
-                    except Full:
-                        exec_method(self.logger, 'warning', True, "[Collector._prepare_training_data] training_data_que is full!")
-            # exec_method(self.logger, 'warning', True, "[Collector._prepare_training_data] training_data_que is full!")
-            time.sleep(0.002)
+            training_data = self._get_training_data()
+            if training_data is not None:
+                self._training_data_que.append(training_data)
+                # try:
+                #     self._training_data_que.put(training_data, block = False, timeout=0.1)
+                # except Full:
+                #     pass
+            # if not self._training_data_que.full():
+            #     training_data = self._get_training_data()
+            #     if training_data is not None:
+            #         try:
+            #             self._training_data_que.put(training_data, block = True, timeout=0.1)
+            #             consumed_exp_len += training_data['dones'].shape[0]
+            #             if time.time() - s_t >= t_interval:
+            #                 exec_method(self.logger, 'info', 'remote', f"[Collector._prepare_training_data] SAMPLE CONSUMPTION SPEED per second: {consumed_exp_len/t_interval:.2f}")
+            #                 s_t = time.time()
+            #                 consumed_exp_len = 0
+            #         except Full:
+            #             pass
+                        # exec_method(self.logger, 'warning', 'get', "[Collector._prepare_training_data] training_data_que is full!")
+            # time.sleep(0.002)
             
     def _get_training_data(self):
-        training_data = self.data_handler.sample_training_data() # sample training data
+        training_data = exec_method(self.data_handler, 'sample_training_data', 'get')
         return training_data
     
-    def handle_data_after_learn(self, policy_data_after_learn, *args, **kwargs):
-        return 
-    
     def get_buffer_length(self):
         return len(self.data_handler.buffer)
```

### Comparing `joyrl-0.5.2/joyrl/framework/config.py` & `joyrl-0.6.0/joyrl/framework/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-02 15:30:09
 LastEditor: JiangJi
-LastEditTime: 2024-01-25 10:01:41
+LastEditTime: 2024-06-01 14:35:10
 Discription: 
 '''
 class DefaultConfig:
     ''' Default parameters for running
     '''
     def __init__(self) -> None:
         pass
@@ -33,14 +33,15 @@
         # basic settings
         self.joyrl_version = "0.5.0"
         self.env_name = "gym" # name of environment
         self.algo_name = "DQN" # name of algorithm
         self.mode = "train" # train, test
         self.device = "cpu" # device to use
         self.seed = 0 # random seed
+        self.is_learner_async = True # if learner is async
         self.max_episode = -1 # number of episodes for training, set -1 to keep running
         self.max_step = -1 # number of episodes for testing, set -1 means unlimited steps
         self.collect_traj = False # if collect trajectory or not
         # multiprocessing settings
         self.n_interactors = 1 # number of workers
         self.exps_trucation_size = 1 # size of exps to truncate
         self.n_learners = 1 # number of learners if using multi-processing, default 1
```

### Comparing `joyrl-0.5.2/joyrl/framework/interactor.py` & `joyrl-0.6.0/joyrl/framework/trainer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,132 +1,154 @@
-import gymnasium as gym
-import ray
-import time
+#!/usr/bin/env python
+# coding=utf-8
+'''
+Author: JiangJi
+Email: johnjim0816@gmail.com
+Date: 2023-12-02 15:02:30
+LastEditor: JiangJi
+LastEditTime: 2024-06-01 16:53:24
+Discription: 
+'''
 import copy
-from joyrl.algos.base.experience import Exp
+import time
+import ray
+from ray.util.queue import Queue as RayQueue
 from joyrl.framework.message import Msg, MsgType
 from joyrl.framework.config import MergedConfig
 from joyrl.framework.base import Moduler
+from joyrl.framework.collector import Collector
+from joyrl.framework.tracker import Tracker
+from joyrl.framework.interactor import Interactor
+from joyrl.framework.learner import Learner
+from joyrl.framework.tester import OnlineTester
+from joyrl.framework.policy_mgr import PolicyMgr
 from joyrl.framework.recorder import Recorder
 from joyrl.utils.utils import exec_method, create_module
+from joyrl.utils.utils import Logger
+from joyrl.framework.utils import SharedData
 
-class BaseInteractor(object):
-    def __init__(self, cfg: MergedConfig, **kwargs) -> None:
-        self.cfg = cfg 
-
-class Interactor:
-    def __init__(self, cfg: MergedConfig, **kwargs) -> None:
-        self.cfg = cfg
-        self.id = kwargs.get('id', 0)
-        self.env = kwargs.get('env', None)
-        self.policy = kwargs.get('policy', None)
-        self._raw_exps_que = kwargs.get('raw_exps_que', None)
-        self.tracker = kwargs['tracker']
-        self.collector = kwargs['collector']
-        self.recorder = kwargs['recorder']
-        self.policy_mgr = kwargs['policy_mgr']
-        self.logger = kwargs['logger']
-        self.use_ray = kwargs['use_ray']
-        self.seed = self.cfg.seed + self.id
-        self.exps = [] # reset experiences
-        self.summary = [] # reset summary
-        self.ep_reward, self.ep_step = 0, 0 # reset params per episode
-        self.curr_obs, self.curr_info = self.env.reset(seed = self.seed) # reset env
-        self._init_n_sample_steps()
-
-    def _init_n_sample_steps(self):
-        ''' when learner_mode is serial, learner will run after interact finishes n_sample_steps
-        '''
-        if self.cfg.on_policy:
-            self.n_sample_steps = self.cfg.batch_size 
-        else:
-            self.n_sample_steps = 1
-            if self.use_ray: # async mode, set n_sample_steps to inf
-                self.n_sample_steps = float('inf')
-                
-    def _put_exps(self):
-        ''' put exps to collector
-        '''
-        while True:
-            try:
-                self._raw_exps_que.put(self.exps, block=True, timeout=0.01)
-                break
-            except:
-                exec_method(self.logger, 'warning', True, "[Collector.pub_msg] raw_exps_que is full!")
-                time.sleep(0.01)
-        self.exps = []
-
-    def run(self):
-        ''' run in sync mode
-        '''
-        run_step = 0 # local run step
-        while True:
-            model_params = exec_method(self.policy_mgr, 'pub_msg', True,  Msg(type = MsgType.MODEL_MGR_GET_MODEL_PARAMS)) # get model params
-            self.policy.put_model_params(model_params)
-            action = self.policy.get_action(self.curr_obs)
-            obs, reward, terminated, truncated, info = self.env.step(action)
-            interact_transition = {'interactor_id': self.id, 'state': self.curr_obs, 'action': action,'reward': reward, 'next_state': obs, 'done': terminated or truncated, 'info': info}
-            policy_transition = self.policy.get_policy_transition()
-            self.exps.append(Exp(**interact_transition, **policy_transition))
-            self.curr_obs, self.curr_info = obs, info
-            self.ep_reward += reward
-            self.ep_step += 1
-            if terminated or truncated or self.ep_step >= self.cfg.max_step > 0:
-                global_episode = exec_method(self.tracker, 'pub_msg', True, Msg(type = MsgType.TRACKER_GET_EPISODE))
-                exec_method(self.tracker, 'pub_msg', False, Msg(MsgType.TRACKER_INCREASE_EPISODE))
-                if global_episode % self.cfg.interact_summary_fre == 0: 
-                    exec_method(self.logger, 'info', True, f"Interactor {self.id} finished episode {global_episode} with reward {self.ep_reward:.3f} in {self.ep_step} steps, truncated: {truncated}, terminated: {terminated}")
-                    # put summary to recorder
-                    interact_summary = {'reward':self.ep_reward,'step':self.ep_step}
-                    self.summary.append((global_episode, interact_summary))
-                    exec_method(self.recorder, 'pub_msg', True, Msg(type = MsgType.RECORDER_PUT_SUMMARY, data = self.summary)) # put summary to stats recorder
-                    self.summary = [] # reset summary
-                self.ep_reward, self.ep_step = 0, 0
-                self.curr_obs, self.curr_info = self.env.reset(seed = self.seed)
-            if self.cfg.on_policy:
-                if len(self.exps) >= self.cfg.batch_size:
-                    self._put_exps()
-                    # exec_method(self.collector, 'pub_msg', True, Msg(type = MsgType.COLLECTOR_PUT_EXPS, data = self.exps))
-                    # self.exps = []
-            else:
-                if len(self.exps) >= self.cfg.exps_trucation_size or terminated or truncated or self.ep_step >= self.cfg.max_step:
-                    self._put_exps()
-                    # exec_method(self.collector, 'pub_msg', True, Msg(type = MsgType.COLLECTOR_PUT_EXPS, data = self.exps))
-                    
-            run_step += 1
-            if run_step >= self.n_sample_steps:
-                break
-
-class InteractorMgr(Moduler):
-    ''' Interactor manager for managing interactors
+class Trainer(Moduler):
+    ''' Collector for collecting training data
     '''
-    def __init__(self, cfg: MergedConfig, **kwargs) -> None:
+    def __init__(self, cfg: MergedConfig,**kwargs) -> None:
         super().__init__(cfg, **kwargs)
         self.env = kwargs['env']
         self.policy = kwargs['policy']
-        self.raw_exps_que = kwargs['raw_exps_que']
-        self.recorder = create_module(Recorder, self.use_ray, {'num_cpus':0}, self.cfg, type = 'interactor')
-        self.n_interactors = self.cfg.n_interactors
-        self.interactors = [create_module(Interactor, self.use_ray, {'num_cpus':1 }, self.cfg,
-            id = i,
-            env = copy.deepcopy(self.env),
+        self.data_handler = kwargs['data_handler']
+        self._print_cfgs() # print parameters
+        self._create_shared_data() # create data queues
+        self._create_modules() # create modules
+        
+    def _create_shared_data(self):
+        self.latest_model_params_dict = SharedData.options(**{'num_cpus': 0}).remote({'step': 0, 'model_params': self.policy.get_model_params()})
+        
+    def _create_modules(self):
+        ''' create modules
+        '''
+        if self.cfg.online_eval:
+            recorder = ray.remote(Recorder).options(**{'num_cpus': 0}).remote(self.cfg,
+                                                                            name = 'RecorderOnlineTester',
+                                                                            type = 'online_tester')
+            self.online_tester = OnlineTester(
+                self.cfg, 
+                name = 'OnlineTester',
+                env = copy.deepcopy(self.env), 
+                policy = copy.deepcopy(self.policy),
+                recorder = recorder,
+            )
+        self.tracker = ray.remote(Tracker).remote(self.cfg)
+        self.collector = ray.remote(Collector).options(**{'num_cpus': 1}).remote(
+            self.cfg,
+            name = 'Collector',
+            data_handler = self.data_handler,
+        )
+        self.policy_mgr = ray.remote(PolicyMgr).options(**{'num_cpus': 0}).remote(
+            self.cfg,
+            name = 'PolicyMgr',
             policy = copy.deepcopy(self.policy),
-            tracker = kwargs.get('tracker', None),
-            collector = kwargs.get('collector', None),
-            recorder = self.recorder,
-            policy_mgr = kwargs.get('policy_mgr', None),
-            raw_exps_que = self.raw_exps_que,
-            logger = self.logger,
-            use_ray = self.use_ray,
-            ) for i in range(self.n_interactors)
-            ]
-        exec_method(self.logger, 'info', True, f"[InteractorMgr] Create {self.n_interactors} interactors!, use_ray: {self.use_ray}")
+            latest_model_params_dict = self.latest_model_params_dict,
+        )
+        self.interactors = []
+        recorder = ray.remote(Recorder).options(**{'num_cpus': 0}).remote(self.cfg,
+                                                                            name = 'RecorderInteractor',
+                                                                            type = 'interactor')
+        for i in range(self.cfg.n_interactors):
+            interactor = ray.remote(Interactor).options(**{'num_cpus': 1}).remote(
+                self.cfg,
+                id = i,
+                name = f"Interactor_{i}",
+                env = copy.deepcopy(self.env),
+                policy = copy.deepcopy(self.policy),
+                data_handler = copy.deepcopy(self.data_handler),  # only use the static method handle_exps_after_interact
+                tracker = self.tracker,
+                collector = self.collector,
+                recorder = recorder,
+                policy_mgr = self.policy_mgr,
+                latest_model_params_dict = self.latest_model_params_dict,
+                )
+            self.interactors.append(interactor)
+        self.learners = []
+        recorder = ray.remote(Recorder).options(**{'num_cpus': 0}).remote(self.cfg,
+                                                                            name = 'RecorderLearner',
+                                                                            type = 'learner')
+        for i in range(self.cfg.n_learners):
+            learner = ray.remote(Learner).remote(
+                self.cfg,
+                id = i,
+                name = f"Learner_{i}",
+                policy = copy.deepcopy(self.policy),
+                policy_mgr = self.policy_mgr,
+                collector = self.collector,
+                data_handler = self.data_handler,
+                tracker = self.tracker,
+                recorder = recorder,
+                )
+            self.learners.append(learner)
+
+    def _print_cfgs(self):
+        ''' print parameters
+        '''
+        def print_cfg(cfg, name = ''):
+            cfg_dict = vars(cfg)
+            exec_method(self.logger, 'info', 'get', f"{name}:")
+            exec_method(self.logger, 'info', 'get', ''.join(['='] * 80))
+            tplt = "{:^20}\t{:^20}\t{:^20}"
+            exec_method(self.logger, 'info', 'get', tplt.format("Name", "Value", "Type"))
+            for k, v in cfg_dict.items():
+                if v.__class__.__name__ == 'list': # convert list to str
+                    v = str(v)
+                if v is None: # avoid NoneType
+                    v = 'None'
+                if "support" in k: # avoid ndarray
+                    v = str(v[0])
+                exec_method(self.logger, 'info', 'get', tplt.format(k, v, str(type(v))))
+            exec_method(self.logger, 'info', 'get', ''.join(['='] * 80))
+        print_cfg(self.cfg.general_cfg, name = 'General Configs')
+        print_cfg(self.cfg.algo_cfg, name = 'Algo Configs')
+        print_cfg(self.cfg.env_cfg, name = 'Env Configs')
 
     def run(self):
-        ''' run interactors
+        ''' run the trainer
         '''
-        need_get = False
-        if self.cfg.on_policy and self.use_ray:
-            need_get = True
-        for i in range(self.n_interactors):
-            exec_method(self.interactors[i], 'run', need_get)
-            
+        exec_method(self.logger, 'info', 'get', f"[Trainer.run] Start {self.cfg.mode}ing!")
+        s_t = time.time()
+        if not self.cfg.is_learner_async:
+            while True:
+                ray.get([interactor.run.remote() for interactor in self.interactors])
+                ray.get([learner.run.remote() for learner in self.learners])
+                if exec_method(self.tracker, 'pub_msg', 'get', Msg(type = MsgType.TRACKER_CHECK_TASK_END)):
+                    e_t = time.time()
+                    exec_method(self.logger, 'info', 'get', f"[Trainer.run] Finish {self.cfg.mode}ing! Time cost: {e_t - s_t:.3f} s")
+                    time.sleep(5)
+                    ray.shutdown()
+                    break
+        else:
+            [interactor.run.remote() for interactor in self.interactors]
+            [learner.run.remote() for learner in self.learners]
+            while True:
+                if exec_method(self.tracker, 'pub_msg', 'get', Msg(type = MsgType.TRACKER_CHECK_TASK_END)):
+                    e_t = time.time()
+                    exec_method(self.logger, 'info', 'get', f"[Trainer.run] Finish {self.cfg.mode}ing! Time cost: {e_t - s_t:.3f} s")
+                    time.sleep(5)
+                    ray.shutdown()
+                    break
+                time.sleep(1)
```

### Comparing `joyrl-0.5.2/joyrl/framework/message.py` & `joyrl-0.6.0/joyrl/framework/message.py`

 * *Files 25% similar despite different names*

```diff
@@ -24,14 +24,14 @@
     COLLECTOR_GET_TRAINING_DATA = 31
     COLLECTOR_GET_BUFFER_LENGTH = 32
 
     # recorder
     RECORDER_PUT_SUMMARY = 40
     
     # policy_mgr
-    MODEL_MGR_PUT_MODEL_PARAMS = 70
-    MODEL_MGR_GET_MODEL_PARAMS = 71
+    POLICY_MGR_PUT_MODEL_PARAMS = 70
+    POLICY_MGR_GET_MODEL_PARAMS = 71
 
 @dataclass
 class Msg(object):
     type: MsgType
     data: Optional[Any] = None
```

### Comparing `joyrl-0.5.2/joyrl/framework/policy_mgr.py` & `joyrl-0.6.0/joyrl/framework/policy_mgr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-22 23:02:13
 LastEditor: JiangJi
-LastEditTime: 2024-01-21 17:45:27
+LastEditTime: 2024-06-01 11:33:53
 Discription: 
 '''
 import time
 import copy
 import threading
 import torch
 from typing import Dict, List
@@ -23,55 +23,54 @@
 
 class PolicyMgr(Moduler):
     ''' model manager
     '''
     def __init__(self, cfg: MergedConfig, *args, **kwargs) -> None:
         super().__init__(cfg, *args, **kwargs)
         self.policy = copy.deepcopy(kwargs['policy'])
-        self._latest_model_params_dict = {'step': 0, 'model_params': self.policy.get_model_params()}
-        self._saved_model_que = RayQueue(maxsize = 128) if self.use_ray else Queue(maxsize = 128)
+        self._latest_model_params_dict = kwargs.get('latest_model_params_dict', None)
+        self._saved_model_que = RayQueue(maxsize = 128)
         self._t_start()
         
     def _t_start(self):
-        exec_method(self.logger, 'info', False, "[PolicyMgr._t_start] Start policy manager!")
+        exec_method(self.logger, 'info', 'get', "[PolicyMgr._t_start] Start policy manager!")
         self._t_save_policy = threading.Thread(target=self._save_policy)
         self._t_save_policy.setDaemon(True)
         self._t_save_policy.start()
     
     def pub_msg(self, msg: Msg):
         ''' publish message
         '''
         msg_type, msg_data = msg.type, msg.data
-        if msg_type == MsgType.MODEL_MGR_PUT_MODEL_PARAMS:
+        if msg_type == MsgType.POLICY_MGR_PUT_MODEL_PARAMS:
             self._put_model_params(msg_data)
-        elif msg_type == MsgType.MODEL_MGR_GET_MODEL_PARAMS:
+        elif msg_type == MsgType.POLICY_MGR_GET_MODEL_PARAMS: # not used in this version
             return self._get_model_params()
         else:
             raise NotImplementedError
         
     def _put_model_params(self, msg_data):
         ''' put model params
         '''
         update_step, model_params = msg_data
-        if update_step > self._latest_model_params_dict['step']:
-            self._latest_model_params_dict['step'] = update_step
-            self._latest_model_params_dict['model_params'] = model_params
+        exec_method(self._latest_model_params_dict, 'set_value', 'get', {'step': update_step, 'model_params': model_params})
         if update_step % self.cfg.model_save_fre == 0:
             while True:
                 try: # if queue is full, wait for 0.01s
                     self._saved_model_que.put((update_step, model_params), block=False)
                     break
                 except:
-                    exec_method(self.logger, 'warning', True, "[PolicyMgr._put_model_params] saved_model_que is full!")
+                    exec_method(self.logger, 'warning', 'get', "[PolicyMgr._put_model_params] saved_model_que is full!")
                     # time.sleep(0.001)
 
     def _get_model_params(self):
         ''' get policy
         '''
-        return self._latest_model_params_dict['model_params']
+        model_params_dict = exec_method(self._latest_model_params_dict, 'get_value', 'get')
+        return model_params_dict
 
     def _save_policy(self):
         ''' async run
         '''
         while True:
             while not self._saved_model_que.empty():
                 update_step, model_params = self._saved_model_que.get()
```

### Comparing `joyrl-0.5.2/joyrl/framework/recorder.py` & `joyrl-0.6.0/joyrl/framework/recorder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-04-28 16:18:44
 LastEditor: JiangJi
-LastEditTime: 2024-01-11 13:19:23
+LastEditTime: 2024-05-30 17:48:58
 Discription: 
 '''
 import ray 
 from ray.util.queue import Queue as RayQueue
 from pathlib import Path
 import pickle
 import time
 import threading
 
-import pandas
+import pandas as pd
 from queue import Queue
 from torch.utils.tensorboard import SummaryWriter  
 from joyrl.framework.message import Msg, MsgType
 from joyrl.framework.config import MergedConfig
 from joyrl.framework.base import Moduler
 from joyrl.utils.utils import exec_method
 
 class Recorder(Moduler):
     ''' Recorder for recording training information
     '''
     def __init__(self, cfg: MergedConfig, **kwargs) -> None:
         super().__init__(cfg, **kwargs)
         self.type = kwargs.get('type', 'recorder')
         self.writter = SummaryWriter(log_dir=f"{self.cfg.tb_dir}/{self.type}")
-        self._summary_que = RayQueue(maxsize = 256) if self.use_ray else Queue(maxsize = 128)
+        self._summary_que = RayQueue(maxsize = 256)
         self._t_start() # TODO, slow down the training speed when using threading 
 
     def _t_start(self):
-        exec_method(self.logger, 'info', False, f"Start {self.type} recorder!")
+        exec_method(self.logger, 'info', 'remote', f"[Recorder._t_start] Start {self.type} recorder!")
         self._t_save_summary = threading.Thread(target=self._save_summary)
         self._t_save_summary.setDaemon(True)
         self._t_save_summary.start()
 
     def pub_msg(self, msg: Msg):
         ''' publish message
         '''
@@ -61,27 +61,27 @@
                 self._summary_que.put(summary_data_list, block = False)
                 break
             except:
                 self.logger.warning(f"[Recorder._add_summary] {self.type} summary_que is full!")
                 # time.sleep(0.001)
                 pass
 
-    def _write_tb_scalar(self, step, summary):
+    def _write_tb_scalar(self, step: int, summary: dict):
         for key, value in summary.items():
-            self.writter.add_scalar(tag = f"{self.cfg.mode.lower()}_{key}", scalar_value=value, global_step = step)
+            self.writter.add_scalar(tag = f"{self.cfg.mode.lower()}_{key}", scalar_value = value, global_step = step)
 
-    def _write_dataframe(self, step, summary):
+    def _write_dataframe(self, step: int, summary: dict):
         df_file = f"{self.cfg.res_dir}/{self.type}.csv"
         if Path(df_file).exists():
-            df = pandas.read_csv(df_file)
+            df = pd.read_csv(df_file)
         else:
-            df = pandas.DataFrame()
+            df = pd.DataFrame()
         saved_dict = {f"{self.type}_step": step}
         saved_dict.update(summary)
-        df = df.append(saved_dict, ignore_index=True)
+        df = pd.concat([df, pd.DataFrame(saved_dict, index=[0])], ignore_index = True)
         df.to_csv(df_file, index = False)
 
     def _save_summary(self):
         while True:
             while not self._summary_que.empty():
                 summary_data_list = self._summary_que.get()
                 for summary_data in summary_data_list:
```

### Comparing `joyrl-0.5.2/joyrl/framework/tester.py` & `joyrl-0.6.0/joyrl/framework/tester.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-02 15:02:30
 LastEditor: JiangJi
-LastEditTime: 2024-01-07 22:07:11
+LastEditTime: 2024-05-31 11:29:45
 Discription: 
 '''
 import time
 import copy
 import os
 import threading
 from joyrl.framework.config import MergedConfig
 from joyrl.framework.base import Moduler
+from joyrl.framework.message import Msg, MsgType
 from joyrl.utils.utils import exec_method
     
 class OnlineTester(Moduler):
     ''' Online tester
     '''
     def __init__(self, cfg : MergedConfig, *args, **kwargs) -> None:
         super().__init__(cfg, *args, **kwargs)
         self.env = copy.deepcopy(kwargs['env'])
         self.policy = copy.deepcopy(kwargs['policy'])
+        self.recorder = kwargs['recorder']
         self.seed = self.cfg.seed
         self.best_eval_reward = -float('inf')
         self.curr_test_step = -1
         self.curr_obs, self.curr_info = self.env.reset(seed = self.seed) # reset env
         self._t_start()
 
     def _t_start(self):
-        exec_method(self.logger, 'info', False, "[OnlineTester._t_start] Start online tester!")
+        exec_method(self.logger, 'info', 'remote', "[OnlineTester._t_start] Start online tester!")
         self._t_eval_policy = threading.Thread(target=self._eval_policy)
         self._t_eval_policy.setDaemon(True)
         self._t_eval_policy.start()
     
     def _check_updated_model(self):
         model_step_list = os.listdir(self.cfg.model_dir)
         model_step_list = [int(model_step) for model_step in model_step_list if model_step.isdigit()]
@@ -68,16 +70,17 @@
                             self.curr_obs, self.curr_info = self.env.reset(seed = self.seed)
                             break
                 try:
                     self.env.close()
                 except:
                     pass
                 mean_eval_reward = sum_eval_reward / self.cfg.online_eval_episode
-                exec_method(self.logger, 'info', True, f"test_step: {self.curr_test_step}, online_eval_reward: {mean_eval_reward:.3f}")
+                exec_method(self.logger, 'info', 'get', f"online_eval step: {self.curr_test_step}, online_eval_reward: {mean_eval_reward:.3f}")
+                exec_method(self.recorder, 'pub_msg', 'remote', Msg(type = MsgType.RECORDER_PUT_SUMMARY, data = [(model_step, {'online_eval_reward': mean_eval_reward})])) # put summary to stats recorder
                 # logger_info = f"test_step: {self.curr_test_step}, online_eval_reward: {mean_eval_reward:.3f}"
                 # self.logger.info.remote(logger_info) if self.use_ray else self.logger.info(logger_info)
                 if mean_eval_reward >= self.best_eval_reward:
-                    exec_method(self.logger, 'info', True, f"current test step obtain a better online_eval_reward: {mean_eval_reward:.3f}, save the best model!")
+                    exec_method(self.logger, 'info', 'get', f"current online_eval step obtain a better reward: {mean_eval_reward:.3f}, save the best model!")
                     self.policy.save_model(f"{self.cfg.model_dir}/best")
                     self.best_eval_reward = mean_eval_reward
             time.sleep(1)
```

### Comparing `joyrl-0.5.2/joyrl/framework/tracker.py` & `joyrl-0.6.0/joyrl/framework/tracker.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/run.py` & `joyrl-0.6.0/joyrl/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-22 13:16:59
 LastEditor: JiangJi
-LastEditTime: 2024-01-21 18:18:30
+LastEditTime: 2024-06-01 16:57:32
 Discription: 
 '''
 import os,copy
 import ray
 import argparse,datetime,importlib,yaml
 import gymnasium as gym
 from pathlib import Path
@@ -158,30 +158,23 @@
          # create agent
         data_handler_mod = importlib.import_module(f"joyrl.algos.{self.general_cfg.algo_name}.data_handler")
         policy = policy_mod.Policy(self.cfg) 
         if self.cfg.load_checkpoint:
             policy.load_model(f"tasks/{self.cfg.load_path}/models/{self.cfg.load_model_step}")
             policy.save_model(f"{self.cfg.model_dir}/{self.cfg.load_model_step}")
         data_handler = data_handler_mod.DataHandler(self.cfg)
+        # data_handler = ray.remote(data_handler_mod.DataHandler).options(**{'num_cpus': 0}).remote(self.cfg)
         return policy, data_handler
 
     def run(self) -> None:
+        ray.init()     
         env = self.env_config() # create single env
-        policy, data_handler = self.policy_config() # configure policy and data_handler
-        is_remote = False
-        if self.cfg.n_interactors > 1: 
-            is_remote = True
-            ray.init()                           
-        trainer = create_module(Trainer, is_remote, {'num_cpus':0}, 
-                                self.cfg,
-                                env = env,
-                                policy = policy,
-                                data_handler = data_handler,
-                                )
-        exec_method(trainer, 'run', True)
+        policy, data_handler = self.policy_config() # configure policy and data_handler                         
+        trainer = Trainer(self.cfg, name = "Trainer", env = env, policy = policy, data_handler = data_handler) # create trainer
+        trainer.run()
 
 def run(**kwargs):
     launcher = Launcher(**kwargs)
     launcher.run()
 
 if __name__ == "__main__":
     launcher = Launcher()
```

### Comparing `joyrl-0.5.2/joyrl/scripts/scripts.py` & `joyrl-0.6.0/joyrl/scripts/scripts.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/joyrl/utils/utils.py` & `joyrl-0.6.0/joyrl/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: John
 Email: johnjim0816@gmail.com
 Date: 2021-03-12 16:02:24
 LastEditor: John
-LastEditTime: 2024-01-04 23:10:57
+LastEditTime: 2024-05-30 17:48:11
 Discription: 
 Environment: 
 '''
 import os
 import math
 import copy
 import numpy as np
@@ -175,30 +175,32 @@
     if is_remote:
         kwargs.update({'use_ray': True})
         return ray.remote(class_name).options(**remote_options).remote(*args, **kwargs)
     else:
         return class_name(*args, **kwargs)
 
     
-def exec_method(instance_name, method_name, need_get, *args, **kwargs):
+def exec_method(instance_name, method_name, way: str, *args, **kwargs):
     ''' execute method of class_name, which can be remote or local
 
     Args:
         class_name (_type_): _description_
         method_name (_type_): _description_
         is_remote (bool, optional): remote or not. Defaults to False.
         need_return (bool, optional): need to return. Defaults to False.
 
     Returns:
         _type_: default None
     '''
     is_remote = isinstance(instance_name, ray.actor.ActorHandle)
     if is_remote:
-        if need_get:
+        if way == "get":
             return ray.get(getattr(instance_name, method_name).remote(*args, **kwargs))
+        elif way == "wait":
+            return ray.wait([getattr(instance_name, method_name).remote(*args, **kwargs)])
         else:
             return getattr(instance_name, method_name).remote(*args, **kwargs)
     else:
         return getattr(instance_name, method_name)(*args, **kwargs)
 
 def all_seed(seed = 1):
     ''' 设置随机种子，保证实验可复现，同时保证GPU和CPU的随机种子一致
@@ -223,23 +225,22 @@
     with open(traj_pkl, 'wb') as f:
         pickle.dump(traj, f)
 
 class Logger(object):
     ''' Logger for print log to console
     '''
     def __init__(self, log_dir, *args, **kwargs) -> None:
-        self.logger = logging.getLogger(name= "Log")
-        if kwargs.get('log_name', None) is not None: # set log name
-            self.logger.name = kwargs['log_name']
+        self.name = kwargs.get('log_name', '')
+        self.logger = logging.getLogger(name = f"Log_{self.name}")
         self.logger.setLevel(logging.INFO) # default level is INFO
         self.formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s: - %(message)s',
             datefmt='%Y-%m-%d %H:%M:%S')
         # output to file by using FileHandler
         if not self.logger.handlers: # avoid duplicate print
-            fh = logging.FileHandler(f"{log_dir}/log.txt")
+            fh = logging.FileHandler(f"{log_dir}/Log_{self.name}.txt")
             fh.setLevel(logging.DEBUG)
             fh.setFormatter(self.formatter)
             self.logger.addHandler(fh)
             ch = logging.StreamHandler()
             ch.setLevel(logging.INFO)
             ch.setFormatter(self.formatter)
             self.logger.addHandler(ch)
```

### Comparing `joyrl-0.5.2/joyrl.egg-info/PKG-INFO` & `joyrl-0.6.0/joyrl.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,57 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.5.2
+Version: 0.6.0
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ray[default]==2.6.3
+Requires-Dist: torch==2.2.1
+Requires-Dist: torchaudio==2.2.1
+Requires-Dist: torchvision==0.17.1
+Requires-Dist: gymnasium==0.29.1
+Requires-Dist: tensorboard==2.16.2
+Requires-Dist: matplotlib==3.8.4
+Requires-Dist: seaborn==0.13.2
+Requires-Dist: dill==0.3.8
+Requires-Dist: scipy==1.13.0
+Requires-Dist: pygame==2.5.2
 Provides-Extra: atari
+Requires-Dist: atari_py; extra == "atari"
+Requires-Dist: opencv-python; extra == "atari"
 Provides-Extra: mujoco
+Requires-Dist: mujoco_py; extra == "mujoco"
 Provides-Extra: pybullet
-License-File: LICENSE
+Requires-Dist: pybullet; extra == "pybullet"
 
 # JoyRL
 
 [![PyPI](https://img.shields.io/pypi/v/joyrl)](https://pypi.org/project/joyrl/)  [![GitHub issues](https://img.shields.io/github/issues/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/issues) [![GitHub stars](https://img.shields.io/github/stars/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/stargazers) [![GitHub forks](https://img.shields.io/github/forks/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/network) [![GitHub license](https://img.shields.io/github/license/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/blob/master/LICENSE)
 
 `JoyRL` is a parallel reinforcement learning library based on PyTorch and Ray. Unlike existing RL libraries, `JoyRL` is helping users to release the burden of implementing algorithms with tough details, unfriendly APIs, and etc. JoyRL is designed for users to train and test RL algorithms with **only hyperparameters configuration**, which is mush easier for beginners to learn and use. Also, JoyRL supports plenties of state-of-art RL algorithms including **RLHF(core of ChatGPT)**(See algorithms below). JoyRL provides a **modularized framework** for users as well to customize their own algorithms and environments. 
 
 ## Install
 
 ⚠️ Note that donot install JoyRL through any mirror image!!!
 
 ```bash
 # you need to install Anaconda first
-conda create -n joyrl python=3.8
+conda create -n joyrl python=3.10
 conda activate joyrl
 pip install -U joyrl
 ```
 
-Torch install:
-
-Pip install is recommended, but if you encounter network error, you can try conda install or pip install with mirrors.
+Torch GPU install:
 
 ```bash
 # pip CPU only
 pip install torch==1.10.0 torchvision==0.11.0 torchaudio==0.10.0
 # if network error, then GPU with mirror image
 pip install torch==1.10.0+cu113 torchvision==0.11.0+cu113 torchaudio==0.10.0 --extra-index-url https://download.pytorch.org/whl/cu113
 # CPU only
@@ -127,8 +140,7 @@
             <a href="https://github.com/yyysjz1997"><img width="70" height="70" src="https://github.com/yyysjz1997.png?s=40" alt="pic"></a><br>
             <a href="https://github.com/yyysjz1997">Yiyuan Yang</a> 
             <p>University of Oxford</p>
         </td>
     </tr>
   </tbody>
 </table>
-
```

### Comparing `joyrl-0.5.2/joyrl.egg-info/SOURCES.txt` & `joyrl-0.6.0/joyrl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -77,12 +77,13 @@
 joyrl/framework/learner.py
 joyrl/framework/message.py
 joyrl/framework/policy_mgr.py
 joyrl/framework/recorder.py
 joyrl/framework/tester.py
 joyrl/framework/tracker.py
 joyrl/framework/trainer.py
+joyrl/framework/utils.py
 joyrl/scripts/__init__.py
 joyrl/scripts/scripts.py
 joyrl/utils/__init__.py
 joyrl/utils/plot.py
 joyrl/utils/utils.py
```

### Comparing `joyrl-0.5.2/setup.cfg` & `joyrl-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `joyrl-0.5.2/setup.py` & `joyrl-0.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,39 @@
 #!/usr/bin/env python
 # coding=utf-8
 '''
 Author: JiangJi
 Email: johnjim0816@gmail.com
 Date: 2023-12-22 13:01:23
 LastEditor: JiangJi
-LastEditTime: 2023-12-22 14:07:48
+LastEditTime: 2024-06-01 17:01:07
 Discription: 
 '''
 import sys,os
 from setuptools import setup, find_packages
 curr_path = os.path.dirname(os.path.abspath(__file__))  # current path
 
 def get_version() -> str:
     # https://packaging.python.org/guides/single-sourcing-package-version/
     init = open(os.path.join("joyrl", "__init__.py"), "r").read().split()
     return init[init.index("__version__") + 2][1:-1]
 
 def get_install_requires() -> str:
     return [
-        "argparse==1.4.0",
-        "dill==0.3.5.1",
-        "glfw==2.5.5",
-        "gymnasium==0.28.1",
-        "imageio==2.22.4",
-        "importlib-metadata<5.0",
-        "matplotlib==3.5.3",
-        "numpy==1.24.3",
-        "pandas==1.3.5",
-        "Pillow==9.4.0",
-        "pygame==2.1.2",
-        "pyglet==2.0.0",
-        "pyyaml==6.0",
-        "ray==2.6.3",
-        "six==1.16.0",
-        "seaborn==0.12.1",
-        "setuptools==59.5.0",
-        "tensorboard==2.11.2",
+        "ray[default]==2.6.3",
+        "torch==2.2.1",
+        "torchaudio==2.2.1",
+        "torchvision==0.17.1",
+        "gymnasium==0.29.1",
+        "tensorboard==2.16.2",
+        "matplotlib==3.8.4",
+        "seaborn==0.13.2",
+        "dill==0.3.8",
+        "scipy==1.13.0",
+        "pygame==2.5.2",
     ]
 
 def get_extras_require() -> str:
     req = {
         "atari": ["atari_py", "opencv-python"],
         "mujoco": ["mujoco_py"],
         "pybullet": ["pybullet"],
```

