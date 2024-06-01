# Comparing `tmp/tapescript-0.4.1.tar.gz` & `tmp/tapescript-0.5.0.tar.gz`

## Comparing `tapescript-0.4.1.tar` & `tapescript-0.5.0.tar`

### file list

```diff
@@ -1,130 +1,132 @@
--rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 tapescript-0.4.1/changelog.md
--rw-r--r--   0        0        0    25982 2020-02-02 00:00:00.000000 tapescript-0.4.1/docs.md
--rw-r--r--   0        0        0    28025 2020-02-02 00:00:00.000000 tapescript-0.4.1/language_spec.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tapescript-0.4.1/license
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tapescript-0.4.1/requirements.txt
--rw-r--r--   0        0        0    16750 2020-02-02 00:00:00.000000 tapescript-0.4.1/script_examples.md
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/AMHL.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/__init__.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/classes.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/errors.py
--rw-r--r--   0        0        0    72141 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/functions.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/interfaces.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/notes.md
--rw-r--r--   0        0        0    50537 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/parsing.py
--rw-r--r--   0        0        0    34258 2020-02-02 00:00:00.000000 tapescript-0.4.1/tapescript/tools.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/context.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/debug.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/test_classes.py
--rw-r--r--   0        0        0    14258 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/test_e2e_eltoo.py
--rw-r--r--   0        0        0   108069 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/test_functions.py
--rw-r--r--   0        0        0    26875 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/test_parsing.py
--rw-r--r--   0        0        0    36207 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/test_tools.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/1.hex
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/1.src
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/2.hex
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/2.src
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/2_decompiled.src
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/3.hex
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/3.src
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/3_decompiled.src
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/4.hex
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/4.src
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/4_decompiled.src
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/5.hex
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/5.src
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/5_decompiled.src
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/6.hex
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/6.src
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/6_decompiled.src
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/branching_e2e.hex
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/branching_e2e.src
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/branching_e2e_decompiled.src
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_committed_script.hex
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_committed_script.src
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_committed_script_decompiled.src
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_locking_script.hex
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_locking_script.src
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_locking_script_decompiled.src
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script1.hex
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script1.src
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script1_decompiled.src
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script2.hex
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script2.src
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script2_decompiled.src
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script3.hex
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script3.src
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/cds_unlocking_script3_decompiled.src
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_committed_script.hex
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_committed_script.src
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_committed_script_decompiled.src
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_locking_script.hex
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_locking_script.src
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_locking_script_decompiled.src
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_unlocking_script1.hex
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_unlocking_script1.src
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_unlocking_script1_decompiled.src
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_unlocking_script2.hex
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_unlocking_script2.src
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/correspondent_unlocking_script2_decompiled.src
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/macros_and_variables.hex
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/macros_and_variables.src
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/macros_and_variables_decompiled.src
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_a.hex
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_a.src
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_a_decompiled.src
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_b.hex
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_b.src
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_ba.hex
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_ba.src
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_ba_decompiled.src
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_bb.hex
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_bb.src
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_committed_script_bb_decompiled.src
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_locking_script.hex
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_locking_script.src
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_a.hex
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_a.src
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_a_decompiled.src
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_ba.hex
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_ba.src
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_ba_decompiled.src
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_bb.hex
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_bb.src
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/merkleval_unlocking_script_bb_decompiled.src
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/new_if_hoist_syntax_0.4.0.hex
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/new_if_hoist_syntax_0.4.0.src
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/new_if_hoist_syntax_0.4.0_decompiled.src
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/new_ops_0.4.0.hex
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/new_ops_0.4.0.src
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/new_ops_0.4.0_decompiled.src
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/omega_e2e.hex
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/omega_e2e.src
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/omega_e2e_aliases.src
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/omega_e2e_decompiled.src
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_locking_script.hex
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_locking_script.src
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_locking_script_decompiled.src
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_unlocking_script1.hex
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_unlocking_script1.src
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_unlocking_script1_decompiled.src
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_unlocking_script2.hex
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_unlocking_script2.src
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2pk_unlocking_script2_decompiled.src
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_committed_script.hex
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_committed_script.src
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_committed_script_decompiled.src
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_locking_script.hex
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_locking_script.src
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_locking_script_decompiled.src
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_unlocking_script.hex
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_unlocking_script.src
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/p2sh_unlocking_script_decompiled.src
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/try_in_if.hex
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/try_in_if.src
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/trydef.hex
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.4.1/tests/vectors/trydef.src
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tapescript-0.4.1/.gitignore
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 tapescript-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    17806 2020-02-02 00:00:00.000000 tapescript-0.4.1/readme.md
--rw-r--r--   0        0        0    18488 2020-02-02 00:00:00.000000 tapescript-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 tapescript-0.5.0/changelog.md
+-rw-r--r--   0        0        0    41263 2020-02-02 00:00:00.000000 tapescript-0.5.0/docs.md
+-rw-r--r--   0        0        0    31927 2020-02-02 00:00:00.000000 tapescript-0.5.0/language_spec.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 tapescript-0.5.0/license
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 tapescript-0.5.0/requirements.txt
+-rw-r--r--   0        0        0    18314 2020-02-02 00:00:00.000000 tapescript-0.5.0/script_examples.md
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 tapescript-0.5.0/tapescript/AMHL.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 tapescript-0.5.0/tapescript/__init__.py
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 tapescript-0.5.0/tapescript/classes.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 tapescript-0.5.0/tapescript/errors.py
+-rw-r--r--   0        0        0    80355 2020-02-02 00:00:00.000000 tapescript-0.5.0/tapescript/functions.py
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 tapescript-0.5.0/tapescript/interfaces.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 tapescript-0.5.0/tapescript/notes.md
+-rw-r--r--   0        0        0    47762 2020-02-02 00:00:00.000000 tapescript-0.5.0/tapescript/parsing.py
+-rw-r--r--   0        0        0    46193 2020-02-02 00:00:00.000000 tapescript-0.5.0/tapescript/tools.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/context.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/debug.py
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/test_classes.py
+-rw-r--r--   0        0        0    14916 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/test_e2e_eltoo.py
+-rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/test_e2e_extensions.py
+-rw-r--r--   0        0        0   107912 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/test_functions.py
+-rw-r--r--   0        0        0    26687 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/test_parsing.py
+-rw-r--r--   0        0        0     7360 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/test_security.py
+-rw-r--r--   0        0        0    39984 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/test_tools.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/1.hex
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/1.src
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/2.hex
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/2.src
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/2_decompiled.src
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/3.hex
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/3.src
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/3_decompiled.src
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/4.hex
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/4.src
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/4_decompiled.src
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/5.hex
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/5.src
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/5_decompiled.src
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/6.hex
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/6.src
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/6_decompiled.src
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/branching_e2e.hex
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/branching_e2e.src
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/branching_e2e_decompiled.src
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/cds_committed_script.hex
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/cds_committed_script.src
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/cds_committed_script_decompiled.src
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/cds_locking_script.hex
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/cds_locking_script.src
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/cds_locking_script_decompiled.src
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/cds_unlocking_script1.hex
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/cds_unlocking_script1.src
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/cds_unlocking_script1_decompiled.src
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/cds_unlocking_script2.hex
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/cds_unlocking_script2.src
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/cds_unlocking_script2_decompiled.src
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/cds_unlocking_script3.hex
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/cds_unlocking_script3.src
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/cds_unlocking_script3_decompiled.src
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/correspondent_committed_script.hex
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/correspondent_committed_script.src
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/correspondent_committed_script_decompiled.src
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/correspondent_locking_script.hex
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/correspondent_locking_script.src
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/correspondent_locking_script_decompiled.src
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/correspondent_unlocking_script1.hex
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/correspondent_unlocking_script1.src
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/correspondent_unlocking_script1_decompiled.src
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/correspondent_unlocking_script2.hex
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/correspondent_unlocking_script2.src
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/correspondent_unlocking_script2_decompiled.src
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/macros_and_variables.hex
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/macros_and_variables.src
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/macros_and_variables_decompiled.src
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_committed_script_a.hex
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_committed_script_a.src
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_committed_script_a_decompiled.src
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_committed_script_b.hex
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_committed_script_b.src
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_committed_script_ba.hex
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_committed_script_ba.src
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_committed_script_ba_decompiled.src
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_committed_script_bb.hex
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_committed_script_bb.src
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_committed_script_bb_decompiled.src
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_locking_script.hex
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_locking_script.src
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_unlocking_script_a.hex
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_unlocking_script_a.src
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_unlocking_script_a_decompiled.src
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_unlocking_script_ba.hex
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_unlocking_script_ba.src
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_unlocking_script_ba_decompiled.src
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_unlocking_script_bb.hex
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_unlocking_script_bb.src
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/merkleval_unlocking_script_bb_decompiled.src
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/new_if_hoist_syntax_0.4.0.hex
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/new_if_hoist_syntax_0.4.0.src
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/new_if_hoist_syntax_0.4.0_decompiled.src
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/new_ops_0.4.0.hex
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/new_ops_0.4.0.src
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/new_ops_0.4.0_decompiled.src
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/omega_e2e.hex
+-rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/omega_e2e.src
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/omega_e2e_aliases.src
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/omega_e2e_decompiled.src
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2pk_locking_script.hex
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2pk_locking_script.src
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2pk_locking_script_decompiled.src
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2pk_unlocking_script1.hex
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2pk_unlocking_script1.src
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2pk_unlocking_script1_decompiled.src
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2pk_unlocking_script2.hex
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2pk_unlocking_script2.src
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2pk_unlocking_script2_decompiled.src
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2sh_committed_script.hex
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2sh_committed_script.src
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2sh_committed_script_decompiled.src
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2sh_locking_script.hex
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2sh_locking_script.src
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2sh_locking_script_decompiled.src
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2sh_unlocking_script.hex
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2sh_unlocking_script.src
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/p2sh_unlocking_script_decompiled.src
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/try_in_if.hex
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/try_in_if.src
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/trydef.hex
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 tapescript-0.5.0/tests/vectors/trydef.src
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tapescript-0.5.0/.gitignore
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tapescript-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    25365 2020-02-02 00:00:00.000000 tapescript-0.5.0/readme.md
+-rw-r--r--   0        0        0    26121 2020-02-02 00:00:00.000000 tapescript-0.5.0/PKG-INFO
```

### Comparing `tapescript-0.4.1/license` & `tapescript-0.5.0/license`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/script_examples.md` & `tapescript-0.5.0/script_examples.md`

 * *Files 6% similar despite different names*

```diff
@@ -185,69 +185,67 @@
 
 This is an example of a streamlined branching script where unexecuted branches
 remain hidden behind cryptographic commitments. Only those script branches
 included in the root commitment can be executed.
 
 ```s
 # locking script: 33 bytes #
-OP_MERKLEVAL x<hex 32 byte root sha256 hash>
+OP_MERKLEVAL x<hex 32 byte root commitment>
 
 # committed script branch A: 36 bytes #
 OP_PUSH x<hex pubkey0>
 OP_CHECK_SIG x00
 
 # unlocking script A: 139 bytes #
 OP_PUSH x<hex signature from pubkey0>
 OP_PUSH x<hex 32 byte branch B sha256 hash>
 OP_PUSH x<hex branch A script>
-OP_TRUE
 
 # committed script branch B: 33 bytes #
-OP_MERKLEVAL x<hex 32 byte branch B root sha256 hash>
+OP_MERKLEVAL x<hex 32 byte branch B root commitment>
 
 # committed script branch BA: 36 bytes #
 OP_PUSH x<hex pubkey1>
 OP_CHECK_SIG x00
 
 # unlocking script BA: 147 bytes #
 OP_PUSH x<hex signature from pubkey1>
 OP_PUSH x<hex 32 byte branch BB sha256 hash>
 OP_PUSH x<hex branch BA script>
-OP_TRUE
+
 OP_PUSH x<hex 32 byte branch A sha256 hash>
 OP_PUSH x<hex branch B script>
-OP_FALSE
 
 # committed script branch BB: 36 bytes #
 OP_PUSH x<hex pubkey2>
 OP_CHECK_SIG x00
 
 # unlocking script BB: 147 bytes #
 OP_PUSH x<hex signature from pubkey2>
 OP_PUSH x<hex 32 byte branch BA sha256 hash>
 OP_PUSH x<hex branch BB script>
-OP_FALSE
+
 OP_PUSH x<hex 32 byte branch A sha256 hash>
 OP_PUSH x<hex branch B script>
-OP_FALSE
+
 ```
 
 This functionality can be replicated with the other ops, but it will have more
-overhead since OP_MERKLEVAL is like a macro that runs a number of other ops.
+overhead since `OP_MERKLEVAL` reads the tape and runs 9 ops and 1 stack push.
 Note that 5 bytes can be shaved from the commitment scripts by using OP_SHAKE256
 with digest length 26, reducing the commitment security from 256 to 208 bits;
 this reduces the size of unlocking scripts A by 10 bytes and unlocking scripts
 BA and BB by 20 bytes. If we decreased the commitment security down to 180 bits
 using `OP_SHAKE256 d20`, this shaves an additional 6 bytes from the locking
 script, 12 bytes from unlocking script A, and 24 bytes from unlocking scripts BA
-and BB (final byte counts of 27, 174, and 232 respectively). The OP_MERKLEVAL
+and BB (final byte counts of 27, 174, and 232 respectively). The `OP_MERKLEVAL`
 option is both more secure and a more efficient branching script solution. The
 below example of this was not added as a test vector because it is strictly
-inferior to the OP_MERKLEVAL method above, and it would have been a lot of time
-and effort that I would rather put elsewhere.
+inferior to the `OP_MERKLEVAL` method above, and it would have been a lot of
+time and effort that I would rather put elsewhere.
 
 ```s
 # locking script: 38 bytes #
 OP_DUP
 OP_SHA256
 OP_PUSH x<hex 32 byte root sha256 hash>
 OP_EQUAL_VERIFY
@@ -318,20 +316,46 @@
 OP_PUSH x<hex committed script branch BB>
 OP_FALSE
 OP_PUSH x<hex committed script branch B>
 OP_FALSE
 OP_PUSH x<hex committed script root>
 ```
 
+## Important Security Note
+
+Since the v0.5.0 upgrade, `OP_MERKLEVAL` now uses a root commitment calculated
+as `xor(sha256(sha256(branch1)), sha256(sha256(branch2)))`. Validation to
+execute branch1 requires providing `sha256(branch2)`, which is then hashed and
+`xor`ed with the double sha256 of branch1; this additional hashing step is to
+prevent being able to execute arbitrary scripts since XOR is a reversible
+operation -- the extra sha256 step requires that one must find the preimage for
+a sha256 hash in order to validate the execution of arbitrary code. Without the
+step, we could do this: given some `root_commitment` and arbitrary code
+`branchA`, calculate `branchB` = `xor(root_commitment, sha256(branchA))`;
+`branchA` would then be executable by providing this calculated `branchB` value.
+With the additional hashing operation, the calculation is instead
+`branchB = sha256_preimage(xor(root_commitment, sha256(sha256(branchA))))`,
+which cannot be calculated.
+
+However, there is one case for which this construction is vulnerable: any
+symmetrical tree will have a root of all null bytes. Given some code `branchA`,
+if a tree is constructed with that branch twice, then the root commitment will
+be `xor(sha256(sha256(branchA)), sha256(sha256(branchA)))`; since anything XOR
+itself is all null bits, every symmetrical tree will share the same root, which
+means that any arbitrary code can be validated and executed against that root by
+constructing another symmetrical tree. This is proven in the
+[security](https://github.com/k98kurz/tapescript/blob/v0.5.0/tests/test_security.py)
+test file.
+
 # Example 6: eltoo-like protocol
 
 This example shows how the features of tapescript can be used to implement the
 [eltoo off-chain protocol](https://blockstream.com/eltoo.pdf) using on-chain
 primitives. This example was implemented as an e2e test
-[here](https://github.com/k98kurz/tapescript/blob/master/tests/test_e2e_eltoo.py).
+[here](https://github.com/k98kurz/tapescript/blob/v0.5.0/tests/test_e2e_eltoo.py).
 This assumes instant confirmation of transactions once broadcast for the sake of
 convenience -- the Unix timestamp based constraints can be adapted for a system
 that enforces causal ordering, e.g. a blockchain or other logical clock.
 
 ## Original proposal
 
 In the original paper, designed for Bitcoin and introducing a new sighash flag
```

### Comparing `tapescript-0.4.1/tapescript/AMHL.py` & `tapescript-0.5.0/tapescript/AMHL.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tapescript/errors.py` & `tapescript-0.5.0/tapescript/errors.py`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tapescript/interfaces.py` & `tapescript-0.5.0/tapescript/interfaces.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from typing import Protocol, runtime_checkable
 
 
 @runtime_checkable
 class TapeProtocol(Protocol):
     def read(self, size: int, move_pointer: bool = True) -> bytes:
         """Read symbols from the data."""
@@ -46,7 +47,40 @@
 class CanBeInvoked(Protocol):
     def abi(self, args: list[bytes]) -> list[bytes]|None:
         """Allow the contract to be called by OP_INVOKE. ABI=Application
             Binary Interface. Takes a list of bytes as args and returns
             either a list of bytes or None.
         """
         ...
+
+
+@runtime_checkable
+class ScriptProtocol(Protocol):
+    """Represent a script as a pairing of source and byte code."""
+    src: str
+    bytes: bytes
+
+    @classmethod
+    def from_src(cls, src: str) -> ScriptProtocol:
+        """Create an instance from tapescript source code."""
+        ...
+
+    @classmethod
+    def from_bytes(cls, code: bytes) -> ScriptProtocol:
+        """Create an instance from tapescript byte code."""
+        ...
+
+    def commitment(self) -> bytes:
+        """Return a cryptographic commitment for the Script."""
+        ...
+
+    def __bytes__(self) -> bytes:
+        """Return the tapescript byte code."""
+        ...
+
+    def __str__(self) -> str:
+        """Return the tapescript source code."""
+        ...
+
+    def __add__(self, other: ScriptProtocol) -> ScriptProtocol:
+        """Add two instances together."""
+        ...
```

### Comparing `tapescript-0.4.1/tapescript/notes.md` & `tapescript-0.5.0/tapescript/notes.md`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 - 3: when True (default True), relevant ops set cache key b'r' (nonce scalar)
 - 4: when True (default True), relevant ops set cache key b'R' (nonce point)
 - 5: when True (default True), relevant ops set cache key b't' (tweak scalar)
 - 6: when True (default True), relevant ops set cache key b'T' (tweak point)
 - 7: when True (default True), relevant ops set cache key b'RT' (nonce point * tweak point)
 - 8: when True (default True), relevant ops set cache key b'sa' (signature adapter)
 - 9: when True (default True), relevant ops set cache key b's' (signature)
+- 10: when True (default True), `OP_CHECK_TEMPLATE` will run the signature extension plugins
 
 These values can be changed by updating the `functions.flags` dict. Additional
 flags can be defined with similar syntax.
 
 ```python
 functions.flags['ts_threshold'] = 120
 functions.flags[69] = 420
```

### Comparing `tapescript-0.4.1/tapescript/parsing.py` & `tapescript-0.5.0/tapescript/parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         else:
             symbols.append(token)
 
     return symbols
 
 
 additional_opcodes = {}
+_special_symbols = ('END_IF', 'END_DEF', 'ELSE', '(',')','{','}')
 
 def define_macro(symbols: list[str], macros: dict = {}) -> int:
     """Defines a macro. Code syntax is `!= name [ args ] { statements }`.
         Returns the number by which to advance the symbol index.
     """
     yert(symbols[0] == '!=', 'macro definition must begin with !=')
     name = symbols[1].lower()
@@ -210,26 +211,26 @@
                 val = bytes(val[2:last_idx+2], 'utf-8')
             elif val[1] == "'" and "'" in val[2:]:
                 last_idx = val[2:].index("'")
                 val = bytes(val[2:last_idx+2], 'utf-8')
             else:
                 val = bytes(val[1:], 'utf-8')
 
-    if 1 < len(val) < 256:
+    if len(val) == 1:
+        ...
+    elif 1 < len(val) < 256:
         # tape syntax of OP_PUSH1 [size 0-255] [val]
         # human-readable decompiled syntax of OP_PUSH1 val
         args.append(len(val).to_bytes(1, 'big'))
     elif 255 < len(val) < 65_536:
         # tape syntax of OP_PUSH2 [size 0-65_535] [val]
         # human-readable decompiled syntax of OP_PUSH2 val
         args.append(len(val).to_bytes(2, 'big'))
-    elif 65_535 < len(val) < 4_294_967_296:
-        # tape syntax of OP_PUSH4 [size 0-4_294_967_295] [val]
-        # human-readable decompiled syntax of OP_PUSH4 val
-        args.append(len(val).to_bytes(4, 'big'))
+    else:
+        raise ValueError(f'size of value invalid for OP_PUSH: {len(val)}')
     args.append(val)
     return (symbols_to_advance, args)
 
 def _get_OP_WRITE_CACHE_args(
         opname: str, symbols: list[str], symbols_to_advance: int
     ) -> tuple[int, tuple[bytes]]:
     symbols_to_advance += 2
@@ -307,16 +308,17 @@
         symbol_index: int
     ) -> tuple[int, tuple[bytes]]:
     args = []
     val = None
 
     if opname == 'OP_PUSH1':
         # human-readable syntax of OP_PUSH1 [size] [val] or OP_PUSH1 [val]
-        if symbols[1] not in ('(',')','{','}') and symbols[1][:3] != 'OP_' and \
-            symbols[1] not in ('END_IF', 'END_DEF', 'ELSE'):
+        if (len(symbols[1]) < 3 or symbols[1][:3] != 'OP_') and \
+            symbols[1] not in opcodes_inverse and symbols[1] not in nopcodes_inverse and \
+            symbols[1] not in opcode_aliases and symbols[1] not in _special_symbols:
             symbols_to_advance += 2
             val = symbols[1]
         else:
             symbols_to_advance += 1
             val = symbols[0]
     else:
         # human-readable syntax of OP_[whatever] [key]
@@ -362,17 +364,17 @@
         symbol_index: int
     ) -> tuple[int, tuple[bytes]]:
     args = []
     val = None
 
     if opname == 'OP_PUSH2':
         # human-readable syntax of OP_PUSH2 [size] [val] or OP_PUSH2 [val]
-        if symbols[1] not in ('(',')','{','}') and symbols[1] not in opcode_aliases and \
+        if (len(symbols[1]) < 3 or symbols[1][:3] != 'OP_') and \
             symbols[1] not in opcodes_inverse and symbols[1] not in nopcodes_inverse and \
-            symbols[1] not in ('END_IF', 'END_DEF', 'ELSE'):
+            symbols[1] not in opcode_aliases and symbols[1] not in _special_symbols:
             symbols_to_advance += 2
             val = symbols[1]
         else:
             symbols_to_advance += 1
             val = symbols[0]
     else:
         # human-readable syntax of OP_[whatever] [key]
@@ -411,71 +413,14 @@
             vert(len(val) < 65_536,
                 f'x-value for OP_PUSH2 must be at most 65_535 bytes long - '
                 f'symbol {symbol_index}')
     args.append(len(val).to_bytes(2, 'big'))
     args.append(val)
     return (symbols_to_advance, args)
 
-def _get_OP_PUSH4_args(
-        opname: str, symbols: list[str], symbols_to_advance: int,
-        symbol_index: int
-    ) -> tuple[int, tuple[bytes]]:
-    args = []
-    val = None
-
-    if opname == 'OP_PUSH4':
-        # human-readable syntax of OP_PUSH4 [size] [val] or OP_PUSH4 [val]
-        if symbols[1] not in ('(',')','{','}') and symbols[1][:3] != 'OP_' and \
-            symbols[1] not in ('END_IF', 'END_DEF', 'ELSE'):
-            symbols_to_advance += 2
-            val = symbols[1]
-        else:
-            symbols_to_advance += 1
-            val = symbols[0]
-    else:
-        # human-readable syntax of OP_[whatever] [key]
-        symbols_to_advance += 1
-        val = symbols[0]
-
-    yert(val[0].lower() in ('d', 'x', 's'), \
-        f'{opname} - values for {opname} must be prefaced with d, x, or s - symbol {symbol_index}')
-
-    match val[0].lower():
-        case 's':
-            if val[1] == '"' and '"' in val[2:]:
-                last_idx = val[2:].index('"')
-                val = bytes(val[2:last_idx+2], 'utf-8')
-            elif val[1] == "'" and "'" in val[2:]:
-                last_idx = val[2:].index("'")
-                val = bytes(val[2:last_idx+2], 'utf-8')
-            else:
-                val = bytes(val[1:], 'utf-8')
-            vert(len(val) < 2**32,
-                f's-value for {opname} must be at most 4_294_967_295 bytes long - symbol {symbol_index}')
-        case 'd':
-            vert(val[1:].lstrip('+-').isnumeric(),
-                f'{opname} - value prefaced by d must be decimal int - symbol {symbol_index}')
-            if '.' in val:
-                val = int_to_bytes(int(val[1:].split('.')[0]))
-            else:
-                val = int_to_bytes(int(val[1:]))
-        case 'f':
-            vert(val[1:].lstrip('+-').replace('.','').isnumeric(),
-                f'{opname} - value prefaced by f must be decimal float; '
-                f'{val} is invalid - symbol {symbol_index}')
-            args.append((4).to_bytes(1, 'big'))
-            args.append(struct.pack('!f', float(val[1:])))
-        case 'x':
-            val = bytes.fromhex(val[1:])
-            vert(len(val) < 2**32,
-                f'x-value for {opname} must be at most 4_294_967_295 bytes long - symbol {symbol_index}')
-    args.append(len(val).to_bytes(4, 'big'))
-    args.append(val)
-    return (symbols_to_advance, args)
-
 def _get_OP_DIV_FLOAT_args(
         opname: str, symbols: list[str], symbols_to_advance: int,
         symbol_index: int
     ) -> tuple[int, tuple[bytes]]:
     args = []
     symbols_to_advance += 1
     val = symbols[0]
@@ -572,24 +517,24 @@
     ) -> tuple[int, tuple[bytes]]:
     """Get the number of symbols to advance and args for an op."""
     symbols_to_advance = 1
     args = []
 
     match opname:
         case 'OP_FALSE' | 'OP_TRUE' | 'OP_POP0' | 'OP_SIZE' | \
-            'OP_READ_CACHE_Q' | 'OP_READ_CACHE_Q_SIZE' | 'OP_DIV_INTS' | \
+            'OP_READ_CACHE_STACK' | 'OP_READ_CACHE_STACK_SIZE' | 'OP_DIV_INTS' | \
             'OP_MOD_INTS' | 'OP_DIV_FLOATS' | 'OP_MOD_FLOATS' | 'OP_DUP' | \
             'OP_SHA256' | 'OP_VERIFY' | 'OP_EQUAL' | 'OP_EQUAL_VERIFY' | \
             'OP_CHECK_TIMESTAMP' | 'OP_CHECK_TIMESTAMP_VERIFY' | \
             'OP_CHECK_EPOCH' | 'OP_CHECK_EPOCH_VERIFY' | 'OP_EVAL' | \
-            'OP_NOT' | 'OP_RETURN' | 'OP_DEPTH' | 'OP_SWAP2' | \
+            'OP_RANDOM' | 'OP_NOT' | 'OP_RETURN' | 'OP_DEPTH' | 'OP_SWAP2' | \
             'OP_CONCAT' | 'OP_CONCAT_STR' | 'OP_CHECK_TRANSFER' | 'OP_LESS' | \
             'OP_LESS_OR_EQUAL' | 'OP_FLOAT_LESS' | 'OP_FLOAT_LESS_OR_EQUAL' | \
-            'OP_INT_TO_FLOAT' | 'OP_FLOAT_TO_INT' | 'OP_SIGN_QUEUE' | \
-            'OP_CHECK_SIG_QUEUE' | 'OP_DERIVE_SCALAR' | 'OP_DERIVE_POINT' | \
+            'OP_INT_TO_FLOAT' | 'OP_FLOAT_TO_INT' | 'OP_SIGN_STACK' | \
+            'OP_CHECK_SIG_STACK' | 'OP_DERIVE_SCALAR' | 'OP_DERIVE_POINT' | \
             'OP_MAKE_ADAPTER_SIG_PUBLIC' | 'OP_MAKE_ADAPTER_SIG_PRIVATE' | \
             'OP_CHECK_ADAPTER_SIG' | 'OP_DECRYPT_ADAPTER_SIG' | 'OP_INVOKE' | \
             'OP_XOR' | 'OP_OR' | 'OP_AND':
             # ops that have no arguments on the tape
             # human-readable syntax of OP_[whatever]
             pass
         case 'OP_PUSH':
@@ -602,41 +547,38 @@
             'OP_READ_CACHE_SIZE' | 'OP_DIV_INT' | \
             'OP_MOD_INT' | 'OP_SET_FLAG' | 'OP_UNSET_FLAG' | 'OP_GET_VALUE':
             # ops that have tape arguments of form [size 0-255] [val]
             return _get_OP_PUSH1_type_args(opname, symbols, symbols_to_advance, symbol_index)
         case 'OP_PUSH0' | 'OP_POP1' | 'OP_ADD_INTS' | 'OP_SUBTRACT_INTS' | \
             'OP_MULT_INTS' | 'OP_ADD_FLOATS' | \
             'OP_SUBTRACT_FLOATS' | 'OP_ADD_POINTS' | 'OP_CALL' | \
-            'OP_COPY' | 'OP_SHAKE256' | 'OP_RANDOM' | 'OP_REVERSE' | \
+            'OP_COPY' | 'OP_SHAKE256' | 'OP_REVERSE' | \
             'OP_SPLIT' | 'OP_SPLIT_STR' | 'OP_CHECK_SIG' | 'OP_SIGN' | \
             'OP_CHECK_SIG_VERIFY' | 'OP_CLAMP_SCALAR' | 'OP_ADD_SCALARS' | \
-            'OP_SUBTRACT_SCALARS' | 'OP_SUBTRACT_POINTS' | 'OP_GET_MESSAGE':
+            'OP_SUBTRACT_SCALARS' | 'OP_SUBTRACT_POINTS' | \
+            'OP_GET_MESSAGE' | 'OP_CHECK_TEMPLATE' | 'OP_CHECK_TEMPLATE_VERIFY':
             # ops that have tape argument of form [-128 to 127]
             # human-readable syntax of OP_[whatever] [int]
             return _get_OP_PUSH0_type_args(opname, symbols, symbols_to_advance, symbol_index)
         case 'OP_PUSH2':
             # ops that have tape argument of form [0-65535] [val]
             # human-readable syntax of simply OP_PUSH2 [val]
             return _get_OP_PUSH2_args(opname, symbols, symbols_to_advance, symbol_index)
-        case 'OP_PUSH4':
-            # ops that have tape argument of form [0-4_294_967_295] [val]
-            # human-readable syntax of simply OP_PUSH4 [val]
-            return _get_OP_PUSH4_args(opname, symbols, symbols_to_advance, symbol_index)
         case 'OP_DIV_FLOAT' | 'OP_MOD_FLOAT':
             # ops that have tape argument of form [4-byte float]
             # human-readable syntax of OP_[DIV|MOD]_FLOAT [val]
             return _get_OP_DIV_FLOAT_args(opname, symbols, symbols_to_advance, symbol_index)
         case 'OP_SWAP':
             # ops that have tape arguments of form [0-255] [0-255]
             # human-readable syntax of OP_SWAP [idx1] [idx2]
             return _get_OP_SWAP_type_args(opname, symbols, symbols_to_advance, symbol_index)
         case 'OP_CHECK_MULTISIG' | 'OP_CHECK_MULTISIG_VERIFY':
             return _get_OP_CHECK_MULTISIG_args(opname, symbols, symbols_to_advance, symbol_index)
-        case 'OP_MERKLEVAL':
-            # op has tape argument of form [val]
+        case 'OP_MERKLEVAL' | 'OP_TAPROOT':
+            # op has tape argument of form [32-byte val]
             return _get_OP_MERKLEVAL_args(opname, symbols, symbols_to_advance, symbol_index)
         case _:
             if opname[:3] == 'NOP':
                 return _get_nopcode_args(opname, symbols, symbols_to_advance, symbol_index)
             return _get_additional_opcode_args(opname, symbols, symbols_to_advance, symbol_index)
 
     return (symbols_to_advance, tuple(args))
@@ -1005,16 +947,14 @@
         if current_symbol in ('OP_PUSH', 'PUSH'):
             if len(args) < 2:
                 parts.append(opcodes_inverse['OP_PUSH0'][0].to_bytes(1, 'big'))
             elif len(args[0]) == 1:
                 parts.append(opcodes_inverse['OP_PUSH1'][0].to_bytes(1, 'big'))
             elif len(args[0]) == 2:
                 parts.append(opcodes_inverse['OP_PUSH2'][0].to_bytes(1, 'big'))
-            elif len(args[0]) == 4:
-                parts.append(opcodes_inverse['OP_PUSH4'][0].to_bytes(1, 'big'))
         elif current_symbol[:3] == 'NOP':
             parts.append(nopcodes_inverse[current_symbol][0].to_bytes(1, 'big'))
         else:
             parts.append(opcodes_inverse[current_symbol][0].to_bytes(1, 'big'))
         parts.append(b''.join(args))
     return (advance, parts)
 
@@ -1119,24 +1059,24 @@
                 loop_len = int.from_bytes(tape.read(2), 'big')
                 lop_body = tape.read(loop_len)
                 loop_lines = decompile_script(lop_body, indent+1)
                 add_line('OP_LOOP {')
                 code_lines.extend(loop_lines)
                 add_line('}')
             case 'OP_FALSE' | 'OP_TRUE' | 'OP_POP0' | 'OP_SIZE' | \
-                'OP_READ_CACHE_Q' | 'OP_READ_CACHE_Q_SIZE' | 'OP_DIV_INTS' | \
+                'OP_READ_CACHE_STACK' | 'OP_READ_CACHE_STACK_SIZE' | 'OP_DIV_INTS' | \
                 'OP_MOD_INTS' | 'OP_DIV_FLOATS' | 'OP_MOD_FLOATS' | 'OP_DUP' | \
                 'OP_SHA256' | 'OP_VERIFY' | 'OP_EQUAL' | 'OP_EQUAL_VERIFY' | \
                 'OP_CHECK_TIMESTAMP' | 'OP_CHECK_TIMESTAMP_VERIFY' | \
                 'OP_CHECK_EPOCH' | 'OP_CHECK_EPOCH_VERIFY' | 'OP_EVAL' | \
-                'OP_NOT' | 'OP_RETURN' | 'OP_DEPTH' | 'OP_SWAP2' | \
+                'OP_RANDOM' | 'OP_NOT' | 'OP_RETURN' | 'OP_DEPTH' | 'OP_SWAP2' | \
                 'OP_CONCAT' | 'OP_CONCAT_STR' | 'OP_CHECK_TRANSFER' | \
                 'OP_LESS' | 'OP_LESS_OR_EQUAL' | 'OP_FLOAT_LESS' | \
                 'OP_FLOAT_LESS_OR_EQUAL' | 'OP_INT_TO_FLOAT' | \
-                'OP_FLOAT_TO_INT' | 'OP_SIGN_QUEUE' | 'OP_CHECK_SIG_QUEUE' | \
+                'OP_FLOAT_TO_INT' | 'OP_SIGN_STACK' | 'OP_CHECK_SIG_STACK' | \
                 'OP_DERIVE_SCALAR' | 'OP_DERIVE_POINT' | \
                 'OP_MAKE_ADAPTER_SIG_PUBLIC' | 'OP_MAKE_ADAPTER_SIG_PRIVATE' | \
                 'OP_CHECK_ADAPTER_SIG' | 'OP_DECRYPT_ADAPTER_SIG' | 'OP_XOR' | \
                 'OP_INVOKE' | 'OP_OR' | 'OP_AND':
                 # ops that have no arguments on the tape
                 # human-readable syntax of OP_[whatever]
                 add_line(op_name)
@@ -1161,38 +1101,33 @@
                 size = tape.read(1)[0]
                 val = tape.read(size)
                 count = tape.read(1)[0]
                 add_line(f'{op_name} x{val.hex()} d{count}')
             case 'OP_PUSH0' | 'OP_POP1' | 'OP_ADD_INTS' | 'OP_SUBTRACT_INTS' | \
                 'OP_MULT_INTS' | 'OP_ADD_FLOATS' | \
                 'OP_SUBTRACT_FLOATS' | 'OP_ADD_POINTS' | 'OP_CALL' | \
-                'OP_COPY' | 'OP_SHAKE256' | 'OP_RANDOM' | 'OP_REVERSE' | \
+                'OP_COPY' | 'OP_SHAKE256' | 'OP_REVERSE' | \
                 'OP_SPLIT' | 'OP_SPLIT_STR' | 'OP_CLAMP_SCALAR' | \
                 'OP_ADD_SCALARS' | 'OP_SUBTRACT_SCALARS' | 'OP_SUBTRACT_POINTS':
                 # ops that have tape argument of form [0-255]
                 # human-readable syntax of OP_[whatever] [int]
                 val = bytes_to_int(tape.read(1))
                 add_line(f'{op_name} d{val}')
-            case 'OP_CHECK_SIG' | 'OP_CHECK_SIG_VERIFY' | 'OP_SIGN' | 'OP_GET_MESSAGE':
+            case 'OP_CHECK_SIG' | 'OP_CHECK_SIG_VERIFY' | 'OP_SIGN' | \
+                'OP_GET_MESSAGE' | 'OP_CHECK_TEMPLATE' | 'OP_CHECK_TEMPLATE_VERIFY':
                 # ops that have tape argument of form x[00-ff]
                 # human-readable syntax of OP_[whatever] x[00-ff]
                 val = tape.read(1)
                 add_line(f'{op_name} x{val.hex()}')
             case 'OP_PUSH2':
                 # ops that have tape argument of form [0-65535] [val]
                 # human-readable syntax of simply OP_PUSH2 [val]
                 size = bytes_to_int(tape.read(2))
                 val = tape.read(size)
                 add_line(f'{op_name} d{size} x{val.hex()}')
-            case 'OP_PUSH4':
-                # ops that have tape argument of form [0-4_294_967_295] [val]
-                # human-readable syntax of simply OP_PUSH4 [val]
-                size = bytes_to_int(tape.read(4))
-                val = tape.read(size)
-                add_line(f'{op_name} d{size} x{val.hex()}')
             case 'OP_DIV_FLOAT' | 'OP_MOD_FLOAT':
                 # ops that have tape argument of form [4-byte float]
                 # human-readable syntax of OP_[DIV|MOD]_FLOAT [val]
                 val = tape.read(4)
                 add_line(f'{op_name} x{val.hex()}')
             case 'OP_SWAP':
                 # ops that have tape arguments of form [0-255] [0-255]
@@ -1203,18 +1138,18 @@
             case 'OP_CHECK_MULTISIG' | 'OP_CHECK_MULTISIG_VERIFY':
                 # ops that have tape arguments of form [0-255] [0-255]
                 # human-readable syntax of OP_SWAP [idx1] [idx2]
                 flag = tape.read(1).hex()
                 idx1 = tape.read(1)[0]
                 idx2 = tape.read(1)[0]
                 add_line(f'{op_name} x{flag} d{idx1} d{idx2}')
-            case 'OP_MERKLEVAL':
+            case 'OP_MERKLEVAL' | 'OP_TAPROOT':
                 # op has tape argument of form [32-byte val]
                 digest = tape.read(32)
-                add_line(f'OP_MERKLEVAL x{digest.hex()}')
+                add_line(f'{op_name} x{digest.hex()}')
             case _:
                 if op_name[:3] == 'NOP':
                     val = tape.read(1)[0]
                     add_line(f'{op_name} d{val}')
                 else:
                     lines = additional_opcodes[op_name][1](op_name, tape)
                     add_lines(lines)
```

### Comparing `tapescript-0.4.1/tapescript/tools.py` & `tapescript-0.5.0/tapescript/tools.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from .AMHL import AMHL
 from .classes import Tape
 from .errors import tert, vert, yert
 from .parsing import (
     compile_script,
     decompile_script,
     add_opcode_parsing_handlers,
@@ -20,88 +21,255 @@
     add_contract_interface,
     remove_contract_interface,
     clamp_scalar,
     derive_key_from_seed,
     derive_point_from_scalar,
     aggregate_points,
     aggregate_scalars,
-    H_big,
-    H_small,
+    sign_with_scalar,
+    xor,
 )
+from .interfaces import ScriptProtocol
+from dataclasses import dataclass, field
 from hashlib import sha256, shake_256
 from sys import argv
 from time import time
 from typing import Callable
 import nacl.bindings
 import json
+import struct
 
 
-def _combine_two(branch_a: str, branch_b: str) -> list[str]:
-    """Takes two script branches, hashes them, and returns a root script
-        using OP_MERKLEVAL and two unlocking scripts that execute the
-        supplied branches after the locking script executes.
-    """
-    compiled_a = compile_script(branch_a)
-    compiled_b = compile_script(branch_b)
-    hash_a = sha256(compiled_a).digest()
-    hash_b = sha256(compiled_b).digest()
-    root = sha256(hash_a + hash_b).digest()
-
-    root_script = f'OP_MERKLEVAL x{root.hex()}\n'
-    script_a = f'OP_PUSH x{hash_b.hex()}\nOP_PUSH x{compiled_a.hex()}\nOP_TRUE\n'
-    script_b = f'OP_PUSH x{hash_a.hex()}\nOP_PUSH x{compiled_b.hex()}\nOP_FALSE\n'
-
-    return [root_script, script_a, script_b]
-
-def _format_scripts(levels: list) -> tuple[str, list[str]]:
-    """Turns a list of script levels into a top-level locking script and
-        the unlocking scripts for each branch.
-    """
-    locking_script = levels[0][0]
-    branches = [levels[0][1]]
-    partial = levels[0][2]
-
-    for i in range(1, len(levels)):
-        branches.append(levels[i][1] + partial)
-        partial = levels[i][2] + partial
-
-    branches.append(partial)
-
-    return (locking_script, branches)
-
-def create_merklized_script(branches: list[str], levels: list = None) -> tuple[str, list[str]]:
-    """Produces a Merklized, branching script structure with a branch on
-        the left at every level. Returns a tuple of root script and list
-        of branch execution scripts.
-    """
-    tert(type(branches) in (list, tuple), 'branches must be list or tuple of str')
-    for branch in branches:
-        tert(type(branch) is str, 'branches must be list or tuple of str')
-        vert(len(branch) > 0, 'branches must not be empty')
-    vert(len(branches) >= 1, 'must be at least 1 branch')
-
-    if len(branches) == 1:
-        branches.append('OP_FALSE') # filler branch
-    levels = levels or []
-
-    # combine final 2 branches
-    scripts = _combine_two(branches[-2], branches[-1])
-    levels.append(scripts)
-    remaining_branches = [*branches[:-2], scripts[0]]
-
-    if len(remaining_branches) == 1:
-        levels.reverse()
-        return _format_scripts(levels)
+@dataclass
+class Script:
+    """Represent a script as a pairing of source and byte code."""
+    src: str = field()
+    bytes: bytes = field()
+
+    @classmethod
+    def from_src(cls, src: str) -> Script:
+        """Create an instance from tapescript source code."""
+        return cls(src, compile_script(src))
+
+    @classmethod
+    def from_bytes(cls, code: bytes) -> Script:
+        """Create an instance from tapescript byte code."""
+        return cls('\n'.join(decompile_script(code)), code)
+
+    def commitment(self) -> bytes:
+        """Return a cryptographic commitment for the Script."""
+        return sha256(self.bytes).digest()
+
+    def __bytes__(self) -> bytes:
+        """Return the tapescript byte code."""
+        return self.bytes
+
+    def __str__(self) -> str:
+        """Return the tapescript source code."""
+        return self.src
+
+    def __add__(self, other: Script) -> Script:
+        """Add two instances together."""
+        tert(isinstance(other, Script), 'cannot add Script to non-Script')
+        return Script(f'{self.src}\n{other.src}', self.bytes + other.bytes)
+
+
+@dataclass
+class ScriptLeaf:
+    """A leaf in a Merklized script tree."""
+    hash: bytes = field()
+    script: Script|None = field(default=None)
+    parent: ScriptNode = field(default=None)
+
+    @classmethod
+    def from_script(cls, script: Script) -> ScriptLeaf:
+        """Create an instance from a Script object."""
+        return cls(script.commitment(), script)
+
+    @classmethod
+    def from_src(cls, src: str) -> ScriptLeaf:
+        """Create an instance from the source code."""
+        return cls.from_script(Script.from_src(src))
+
+    @classmethod
+    def from_code(cls, code: bytes) -> ScriptLeaf:
+        """Create an instance from the byte code."""
+        return cls.from_script(Script.from_bytes(code))
+
+    def commitment(self) -> bytes:
+        """Return the cryptographic commitment for the leaf."""
+        return self.hash
+
+    def unlocking_script(self) -> Script:
+        """Calculate an unlocking script recursively, traveling up the
+            parents. Returns a Script with the source and byte codes.
+        """
+        vert(self.parent is not None,
+             'leaf must be part of a tree to generate an unlocking script')
+        other = self.parent.right if self.parent.left is self else self.parent.left
+        commitment = other.commitment()
+        src = f'push x{commitment.hex()}\npush x{self.script.bytes.hex()}'
+        script = Script.from_src(src)
+
+        previous = self.parent.unlocking_script()
+        return Script(f'{script.src}\n{previous.src}', script.bytes + previous.bytes)
+
+    def pack(self) -> bytes:
+        """Serialize the instance to bytes."""
+        return self.script.bytes
+
+    @classmethod
+    def unpack(cls, serialized: bytes) -> ScriptLeaf:
+        """Deserialize an instance from bytes."""
+        return cls.from_code(serialized)
+
+
+class ScriptNode:
+    """A node in a Merklized script tree."""
+    left: ScriptLeaf|ScriptNode
+    right: ScriptLeaf|ScriptNode
+    parent: ScriptNode
+
+    def __init__(self, left: ScriptLeaf|ScriptNode, right: ScriptLeaf|ScriptNode) -> None:
+        """Initialize the instance."""
+        left.parent = self
+        right.parent = self
+        self.left = left
+        self.right = right
+        self.parent = None
+
+    def root(self) -> bytes:
+        """Calculate and return the local root between the two branches."""
+        return xor(
+            sha256(self.left.commitment()).digest(),
+            sha256(self.right.commitment()).digest()
+        )
+
+    def locking_script(self) -> Script:
+        """Calculates the locking script for the node. Returns a tuple
+            with the source and byte codes.
+        """
+        return Script.from_src(f'OP_MERKLEVAL x{self.root().hex()}')
+
+    def commitment(self) -> bytes:
+        """Calculates the commitment to execute this ScriptNode and
+            returns as bytes.
+        """
+        return self.locking_script().commitment()
+
+    def unlocking_script(self) -> Script:
+        """Calculates a recursive unlocking script for the node. Returns
+            a Script with the source and byte codes.
+        """
+        if not self.parent:
+            return Script('', b'')
+
+        other = self.parent.right if self.parent.left is self else self.parent.left
+        commitment = other.commitment()
+        src = f'push x{commitment.hex()}\npush x{self.locking_script().bytes.hex()}'
+        script = Script.from_src(src)
+        previous = self.parent.unlocking_script()
+        return Script(f'{script.src}\n{previous.src}', script.bytes + previous.bytes)
+
+    def pack(self) -> bytes:
+        """Serialize the script tree to bytes."""
+        left = self.left.pack()
+        right = self.right.pack()
+        return struct.pack(
+            f'!cH{len(left)}scH{len(right)}s',
+            b'L' if isinstance(self.left, ScriptLeaf) else b'N',
+            len(left),
+            left,
+            b'L' if isinstance(self.right, ScriptLeaf) else b'N',
+            len(right),
+            right,
+        )
+
+    @classmethod
+    def unpack(cls, data: bytes) -> ScriptNode:
+        """Deserialize a script tree from bytes."""
+        left_type, left_len, data = struct.unpack(f'!cH{len(data)-3}s', data)
+        left_data, right_type, right_len, data = struct.unpack(
+            f'!{left_len}scH{len(data)-3-left_len}s',
+            data
+        )
+        right_data = data
+        if len(data) > right_len:
+            right_data, data = struct.unpack(f'!{right_len}s{len(data)-right_len}s', data)
+
+        left = ScriptLeaf.unpack(left_data) if left_type == b'L' else ScriptNode.unpack(left_data)
+        right = ScriptLeaf.unpack(right_data) if right_type == b'L' else ScriptNode.unpack(right_data)
+        return cls(left, right)
+
+def create_script_tree_prioritized(
+        leaves: list[str|ScriptProtocol], tree: ScriptNode = None) -> ScriptNode:
+    """Construct a script tree from the leaves using a ScriptLeaf for
+        each leaf script, combining the last two into a ScriptNode and
+        then recursively combining a ScriptLeaf for the last of the
+        remaining script leaves with the previously generated ScriptNode
+        until all leaves have been included, priorizing the lower index
+        leaf scripts with smaller unlocking script sizes.
+    """
+    tert(type(leaves) in (list, tuple), 'leaves must be list or tuple of str')
+    for leaf in leaves:
+        tert(type(leaf) is str or isinstance(leaf, ScriptProtocol),
+             'leaves must be list or tuple of str|ScriptProtocol')
+        vert(len(str(leaf)) > 0, 'leaves must not be empty')
+    vert(len(leaves) >= 1, 'must be at least 1 leaf')
+
+    for i in range(len(leaves)):
+        if type(leaves[i]) is str:
+            leaves[i] = Script.from_src(leaves[i])
+
+    if tree:
+        node = ScriptNode(
+            ScriptLeaf.from_script(leaves.pop()),
+            tree
+        )
+        if len(leaves):
+            return create_script_tree_prioritized(leaves, node)
+        return node
+
+    if len(leaves) == 1:
+        leaves.append(Script.from_src('false')) # filler branch
+
+    # combine final 2 leaves
+    node = ScriptNode(
+        right=ScriptLeaf.from_script(leaves.pop()),
+        left=ScriptLeaf.from_script(leaves.pop())
+    )
 
-    return create_merklized_script(remaining_branches, levels)
+    if len(leaves):
+        return create_script_tree_prioritized(leaves, node)
+    return node
+
+def create_merklized_script_prioritized(
+        leaves: list[str|ScriptProtocol]) -> tuple[Script, list[Script]]:
+    """Produces a Merklized, branching script structure with one leaf
+        and one node at every level except for the last node, which is
+        balanced. Returns a tuple of root locking script and list of
+        unlocking scripts. The tree is unbalanced; execution is
+        optimized for earlier branches (lower index leaf scripts), and
+        execution is linearly worse for each subsequent branch.
+    """
+    tree = create_script_tree_prioritized(leaves)
+    lock = tree.locking_script()
+    scripts = [tree.left.unlocking_script()]
+    while type(tree.right) is ScriptNode:
+        tree = tree.right
+        scripts.append(tree.left.unlocking_script())
+    scripts.append(tree.right.unlocking_script())
+    return (lock, scripts)
 
 def _format_docstring(docstring: str) -> str:
     """Takes a docstring, tokenizes it, and returns a str formatted to
         80 chars or fewer per line without splitting tokens.
     """
+    if not docstring:
+        return ""
     def make_line(tokens: list[str]) -> tuple[str, list[str]]:
         line = ''
         while len(tokens) and len(line) + len(tokens[0]) <= 80:
             line += tokens[0] + ' '
             tokens = tokens[1:]
         return (line[:-1], tokens)
 
@@ -110,15 +278,15 @@
 
     while len(tokens):
         line, tokens = make_line(tokens)
         lines.append(line)
 
     return '\n'.join(lines)
 
-def _format_function_doc(function: Callable) -> str:
+def _format_function_doc(function: Callable, extra_indent: int = 0) -> str:
     """Documents a function with header hashtags, annotations, and
         docstring.
     """
     docstring = _format_docstring(function.__doc__)
     name = function.__name__ or 'None'
 
     annotations = [
@@ -132,35 +300,43 @@
         annotations[i+offset] += f' = {defaults[i]}'
     annotations = ', '.join(annotations) or ''
 
     return_annotation = function.__annotations__['return'] or 'unseen_return_value'
     if hasattr(return_annotation, '__name__'):
         return_annotation = return_annotation.__name__
 
-    val = '\n\n## `'
-    val += name
-    val += '('
-    val += annotations
-    val += '): -> '
-    val += return_annotation
-    val += f'`\n\n{docstring}'
+    val = f'\n\n##{"".join(["#" for _ in range(extra_indent)])} `{name}'
+    val += f'({annotations}): -> {return_annotation}`'
+    val += f'\n\n{docstring}'
     return val
 
+def _format_class_doc(cls: type) -> str:
+    """Documents a class. Imports from autodox because I did not want to
+        replicate code, but it is not ordinarily called during package
+        use, so autodox is not considered a main dependency.
+    """
+    if 'dox_a_class' not in dir():
+        from autodox import dox_a_class
+    return dox_a_class(cls, {'header_level': 1})
+
 def _get_op_aliases() -> dict[str, list[str]]:
     """Find and return all aliases for all ops."""
     aliases = {
         opname: []
         for opname in opcodes_inverse
     }
     for alias in opcode_aliases:
         aliases[opcode_aliases[alias]].append(alias)
     return aliases
 
 def generate_docs() -> list[str]:
-    """Generates the docs file using annotations and docstrings."""
+    """Generates the docs file using annotations and docstrings.
+        Requires the autodox library, which is included in the optional
+        "docs" dependencies.
+    """
     data = {}
     aliases = _get_op_aliases()
     alias_lists = {
         opname: 'Aliases:\n- ' + '\n- '.join(aliases[opname])
         for opname in aliases
     }
 
@@ -183,15 +359,15 @@
     nop_doc = f"Codes in {nop_code_snippet}\n" + nop_doc
 
     paragraphs = [
         '# OPs\n\n'
         'Each `OP_` function has an alias that excludes the `OP_` prefix.\n\n'
         'All `OP_` functions have the following signature:\n\n'
         '```python\n'
-        'def OP_WHATEVER(tape: Tape, queue: LifoQueue, cache: dict) -> None:\n'
+        'def OP_WHATEVER(tape: Tape, stack: Stack, cache: dict) -> None:\n'
         '    ...\n```\n\n'
         'All OPs advance the Tape pointer by the amount they read.\n'
     ]
 
     for number in data:
         line = f'\n## {data[number][0]} - {number} - x{number.to_bytes(1, "big").hex().upper()}\n\n'
         docstring = _format_docstring(data[number][1])
@@ -209,18 +385,48 @@
     paragraphs.append(_format_function_doc(remove_contract))
     paragraphs.append(_format_function_doc(add_contract_interface))
     paragraphs.append(_format_function_doc(remove_contract_interface))
     paragraphs.append('\n\n# Parsing functions')
     paragraphs.append(_format_function_doc(compile_script))
     paragraphs.append(_format_function_doc(decompile_script))
     paragraphs.append(_format_function_doc(add_opcode_parsing_handlers))
-    paragraphs.append('\n\n# Tools')
-    paragraphs.append(_format_function_doc(create_merklized_script))
-    paragraphs.append(_format_function_doc(generate_docs))
-    paragraphs.append(_format_function_doc(add_soft_fork) + '\n\n')
+    paragraphs.append('\n\n# Tools\n\n')
+    paragraphs.append(_format_class_doc(Script))
+    paragraphs.append(_format_class_doc(ScriptLeaf))
+    paragraphs.append(_format_class_doc(ScriptNode))
+    paragraphs.append(_format_function_doc(create_script_tree_prioritized))
+    paragraphs.append(_format_function_doc(create_merklized_script_prioritized))
+    paragraphs.append(_format_function_doc(make_adapter_lock_pub))
+    paragraphs.append(_format_function_doc(make_adapter_lock_prv))
+    paragraphs.append(_format_function_doc(make_single_sig_lock))
+    paragraphs.append(_format_function_doc(make_single_sig_lock2))
+    paragraphs.append(_format_function_doc(make_single_sig_witness))
+    paragraphs.append(_format_function_doc(make_single_sig_witness2))
+    paragraphs.append(_format_function_doc(make_multisig_lock))
+    paragraphs.append(_format_function_doc(make_adapter_locks_pub))
+    paragraphs.append(_format_function_doc(make_adapter_decrypt))
+    paragraphs.append(_format_function_doc(decrypt_adapter))
+    paragraphs.append(_format_function_doc(make_adapter_locks_prv))
+    paragraphs.append(_format_function_doc(make_adapter_witness))
+    paragraphs.append(_format_function_doc(make_delegate_key_lock))
+    paragraphs.append(_format_function_doc(make_delegate_key_cert_sig))
+    paragraphs.append(_format_function_doc(make_delegate_key_unlock))
+    paragraphs.append(_format_function_doc(make_htlc_sha256_lock))
+    paragraphs.append(_format_function_doc(make_htlc_shake256_lock))
+    paragraphs.append(_format_function_doc(make_htlc_witness))
+    paragraphs.append(_format_function_doc(make_htlc2_sha256_lock))
+    paragraphs.append(_format_function_doc(make_htlc2_shake256_lock))
+    paragraphs.append(_format_function_doc(make_htlc2_witness))
+    paragraphs.append(_format_function_doc(make_ptlc_lock))
+    paragraphs.append(_format_function_doc(make_ptlc_witness))
+    paragraphs.append(_format_function_doc(make_ptlc_refund_witness))
+    paragraphs.append(_format_function_doc(setup_amhl))
+    paragraphs.append(_format_function_doc(release_left_amhl_lock))
+    paragraphs.append(_format_function_doc(add_soft_fork))
+    paragraphs.append(_format_function_doc(generate_docs) + '\n\n')
 
     with open('tapescript/notes.md', 'r') as f:
         paragraphs.append(f.read())
 
     return paragraphs
 
 def add_soft_fork(code: int, name: str, op: Callable) -> None:
@@ -253,19 +459,19 @@
         val = tape.read(1)[0]
         return [f'{opname} d{val}']
 
     add_opcode(code, name, op)
     add_opcode_parsing_handlers(name, compiler_handler, decompiler_handler)
 
 def make_adapter_lock_pub(
-        pubkey: bytes, tweak_point: bytes, sigflags: str = '00') -> str:
+        pubkey: bytes, tweak_point: bytes, sigflags: str = '00') -> Script:
     """Make an adapter locking script that verifies a sig adapter,
         decrypts it, and then verifies the decrypted signature.
     """
-    return f'''
+    return Script.from_src(f'''
         # required push by unlocking script: tweak scalar t #
         # required push by unlocking script: signature adapter sa #
         # required push by unlocking script: nonce point R #
         @= R 1
         @= sa 1
         @= t 1
 
@@ -279,178 +485,180 @@
         # decrypt adapter sig #
         @sa @R @t decrypt_adapter_sig
         concat
 
         # check sig #
         push x{pubkey.hex()}
         check_sig x{sigflags}
-    '''
+    ''')
 
 def make_adapter_lock_prv(
-        pubkey: bytes, tweak: bytes, sigflags: str = '00') -> str:
+        pubkey: bytes, tweak: bytes, sigflags: str = '00') -> Script:
     """Make an adapter locking script that verifies a sig adapter,
         decrypts it, and then verifies the decrypted signature.
     """
     t = clamp_scalar(tweak)
     T = derive_point_from_scalar(t)
     return make_adapter_lock_pub(pubkey, T, sigflags)
 
-def make_single_sig_lock(pubkey: bytes, sigflags: str = '00') -> str:
+def make_single_sig_lock(pubkey: bytes, sigflags: str = '00') -> Script:
     """Make a locking script that requires a valid signature from a
         single key to unlock. Returns tapescript source code.
     """
-    return f'push x{pubkey.hex()} check_sig x{sigflags}'
+    return Script.from_src(f'push x{pubkey.hex()} check_sig x{sigflags}')
 
-def make_single_sig_lock2(pubkey: bytes, sigflags: str = '00') -> str:
+def make_single_sig_lock2(pubkey: bytes, sigflags: str = '00') -> Script:
     """Make a locking script that requires a valid signature from a
         single key to unlock. Returns tapescript source code. Saves 8
         bytes in locking script at expense of an additional 33 bytes in
         the witness.
     """
-    return f'''
+    return Script.from_src(f'''
         dup shake256 d20
         push x{shake_256(pubkey).digest(20).hex()}
         equal_verify
         check_sig x{sigflags}
-    '''
+    ''')
 
 def make_single_sig_witness(
-        prvkey: bytes, sigfields: dict[str, bytes], sigflags: str = '00') -> str:
+        prvkey: bytes, sigfields: dict[str, bytes], sigflags: str = '00') -> Script:
     """Make an unlocking script that validates for a single sig locking
         script by signing the sigfields. Returns tapescript source code.
     """
-    _, queue, _ = run_script(
+    _, stack, _ = run_script(
         compile_script(f'push x{prvkey.hex()} sign x{sigflags}'),
         {**sigfields}
     )
-    sig = queue.get(False)
-    return f'push x{sig.hex()}'
+    sig = stack.get()
+    return Script.from_src(f'push x{sig.hex()}')
 
 def make_single_sig_witness2(
-        prvkey: bytes, sigfields: dict[str, bytes], sigflags: str = '00') -> str:
+        prvkey: bytes, sigfields: dict[str, bytes], sigflags: str = '00') -> Script:
     """Make an unlocking script that validates for a single sig locking
         script by signing the sigfields. Returns tapescript source code.
         33 bytes larger witness than make_single_sig_witness to save 8
         bytes in the locking script.
     """
-    _, queue, _ = run_script(
+    _, stack, _ = run_script(
         compile_script(f'''
             push x{prvkey.hex()}
             dup derive_scalar derive_point
             swap2 sign x{sigflags}
         '''),
         {**sigfields}
     )
-    sig = queue.get(False)
-    pubkey = queue.get(False)
-    return f'push x{sig.hex()} push x{pubkey.hex()}'
+    sig = stack.get()
+    pubkey = stack.get()
+    return Script.from_src(f'push x{sig.hex()} push x{pubkey.hex()}')
 
 def make_multisig_lock(
-        pubkeys: list[bytes], quorum_size: int, sigflags: str = '00') -> str:
+        pubkeys: list[bytes], quorum_size: int, sigflags: str = '00') -> Script:
     """Make a locking script that requires quorum_size valid signatures
         from unique keys within the pubkeys list. Returns tapescript
         source code. Can be unlocked by joining the results of
         quorum_size calls to make_single_sig_witness by different key
         holders.
     """
     src = ''
     for pk in pubkeys:
         src += f'push x{pk.hex()}\n'
     src += f'check_multisig x{sigflags} d{quorum_size} d{len(pubkeys)}'
-    return src
+    return Script.from_src(src)
 
 def make_adapter_locks_pub(
-        pubkey: bytes, tweak_point: bytes, sigflags: str = '00') -> tuple[str]:
+        pubkey: bytes, tweak_point: bytes, sigflags: str = '00') -> tuple[Script, Script]:
     """Make adapter locking scripts using a public key and a tweak
-        scalar. Returns the source for 2 tapescripts: one that checks if
-        a sig adapter is valid, and one that verifies the decrypted
-        signature.
+        scalar. Returns 2 Scripts: one that checks if a sig adapter is
+        valid, and one that verifies the decrypted signature.
     """
-    script1 = f'''
+    script1 = Script.from_src(f'''
         # required push by unlocking script: signature adapter sa #
         # required push by unlocking script: nonce point R #
         get_message x{sigflags}
         push x{tweak_point.hex()}
         push x{pubkey.hex()}
         check_adapter_sig
-    '''
-    script2 = f'''
+    ''')
+    script2 = Script.from_src(f'''
         # required push by unlocking script: decrypted signature #
-        {make_single_sig_lock(pubkey, sigflags)}
-    '''
+        {make_single_sig_lock(pubkey, sigflags).src}
+    ''')
     return (script1, script2)
 
-def make_adapter_decrypt(tweak: bytes) -> str:
+def make_adapter_decrypt(tweak: bytes) -> Script:
     """Make adapter decryption script."""
     t = clamp_scalar(tweak)
-    return f'''
+    return Script.from_src(f'''
         push x{t.hex()}
         decrypt_adapter_sig
-    '''
+    ''')
 
-def decrypt_adapter(adapter_witness: bytes, tweak: bytes) -> bytes:
+def decrypt_adapter(adapter_witness: bytes|ScriptProtocol, tweak: bytes) -> bytes:
     """Decrypt an adapter signature, returning the decrypted signature."""
-    _, queue, _ = run_script(
+    tert(type(adapter_witness) is bytes or isinstance(adapter_witness, ScriptProtocol),
+         'adapter_witness must be bytes or ScriptProtocol')
+    adapter_witness = bytes(adapter_witness)
+    _, stack, _ = run_script(
         adapter_witness +
-        compile_script(make_adapter_decrypt(tweak))
+        make_adapter_decrypt(tweak).bytes
     )
-    RT = queue.get(False)
-    s = queue.get(False)
+    s = stack.get()
+    RT = stack.get()
     return RT + s
 
 def make_adapter_locks_prv(
-        pubkey: bytes, tweak: bytes, sigflags: str = '00') -> tuple[str]:
+        pubkey: bytes, tweak: bytes, sigflags: str = '00') -> tuple[Script, Script, Script]:
     """Make adapter locking scripts using a public key and a tweak
         scalar. Returns the source for 3 tapescripts: one that checks if
         a sig adapter is valid, one that decrypts the signature, and one
         that verifies the decrypted signature.
     """
     t = clamp_scalar(tweak)
     T = derive_point_from_scalar(t)
     script1, script3 = make_adapter_locks_pub(pubkey, T, sigflags)
     script2 = make_adapter_decrypt(tweak)
     return (script1, script2, script3)
 
 def make_adapter_witness(
         prvkey: bytes, tweak_point: bytes, sigfields: dict,
-        sigflags: str = '00') -> str:
+        sigflags: str = '00') -> Script:
     """Make an adapter signature witness using a private key and a tweak
         point. Returns tapescript src code.
     """
     assert 'sigfield1' in sigfields or 'sigfield2' in sigfields or \
         'sigfield3' in sigfields or 'sigfield4' in sigfields or \
         'sigfield5' in sigfields or 'sigfield6' in sigfields or \
         'sigfield7' in sigfields or 'sigfield8' in sigfields, \
         'at least one sigfield[1-8] must be included'
 
-    _, queue, _ = run_script(
+    _, stack, _ = run_script(
         compile_script(f'''
             push x{prvkey.hex()}
             get_message x{sigflags}
             push x{tweak_point.hex()}
             make_adapter_sig_public
         '''),
         {**sigfields}
     )
-    sa = queue.get(False)
-    R = queue.get(False)
+    sa = stack.get()
+    R = stack.get()
 
-    return f'''
+    return Script.from_src(f'''
         push x{sa.hex()}
         push x{R.hex()}
-    '''
+    ''')
 
-def make_delegate_key_lock(root_pubkey: bytes, sigflags: str = '00') -> str:
+def make_delegate_key_lock(root_pubkey: bytes, sigflags: str = '00') -> Script:
     """Takes a root_pubkey and returns the tapescript source for a
         locking script that is unlocked with a signature from the
         delegate key, the delegated public key, and a certificate from
         the root key committing to the delegate public key and validity
         time constraints.
     """
-    return f'''
+    return Script.from_src(f'''
         # required push: signature from delegate key #
         # required push: delegate public key #
         # required push: delegation begin ts #
         # required push: delegation expiry ts #
         # required push: signature from root key #
         @= crt 1
         @= exp 1
@@ -458,153 +666,159 @@
         @= dpk 1
 
         # prove the timestamp is within the cert bounds #
         @exp val s"timestamp" less verify
         val s"timestamp" @bgn less verify
 
         # cert form: delegate key + begin ts + expiry #
-        @exp @bgn concat @dpk concat
-        @crt push x{root_pubkey.hex()} check_sig_queue verify
+        @crt
+        @dpk @bgn concat @exp concat
+        push x{root_pubkey.hex()} check_sig_stack verify
 
         @dpk check_sig x{sigflags}
-    '''
+    ''')
 
 def make_delegate_key_cert_sig(
         root_skey: bytes, delegate_pubkey: bytes, begin_ts: int, end_ts: int
     ) -> bytes:
     """Returns a signature for a key delegation cert."""
-    _, queue, _ = run_script(compile_script(f'''
-        push d{end_ts} push d{begin_ts} concat
-        push x{delegate_pubkey.hex()} concat
-        push x{root_skey.hex()} sign_queue
+    # cert form: delegate key + begin ts + expiry #
+    _, stack, _ = run_script(compile_script(f'''
+        push x{delegate_pubkey.hex()}
+        push d{begin_ts} concat
+        push d{end_ts} concat
+        push x{root_skey.hex()} sign_stack
     '''))
-    assert queue.qsize() == 1
-    return queue.get(False)
+    assert len(stack) == 1
+    return stack.get()
 
 def make_delegate_key_unlock(
         prvkey: bytes, pubkey: bytes, begin_ts: int, end_ts: int,
         cert_sig: bytes, sigfields: dict, sigflags: str = '00'
-    ) -> str:
-    _, queue, _ = run_script(
+    ) -> Script:
+    """Returns an unlocking script including a signature from the
+        delegate key as well as the delegation certificate.
+    """
+    _, stack, _ = run_script(
         compile_script(f'push x{prvkey.hex()} sign x{sigflags}'),
         sigfields
     )
-    assert queue.qsize() == 1
-    sig = queue.get(False)
-    return f'''
+    assert len(stack) == 1
+    sig = stack.get()
+    return Script.from_src(f'''
         push x{sig.hex()}
         push x{pubkey.hex()}
         push d{begin_ts}
         push d{end_ts}
         push x{cert_sig.hex()}
-    '''
+    ''')
 
 def make_htlc_sha256_lock(
         receiver_pubkey: bytes, preimage: bytes, refund_pubkey: bytes,
-        timeout: int = 60*60*24, sigflags: str = '00') -> str:
+        timeout: int = 60*60*24, sigflags: str = '00') -> Script:
     """Returns an HTLC that can be unlocked either with the preimage and
         a signature matching receiver_pubkey or with a signature
         matching the refund_pubkey after the timeout has expired.
         Suitable only for systems with guaranteed causal ordering and
         non-repudiation of transactions.
     """
-    return f'''
+    return Script.from_src(f'''
         sha256
         push x{sha256(preimage).digest().hex()}
         equal
         if {{
             push x{receiver_pubkey.hex()}
         }} else {{
             push d{int(time())+timeout}
             check_timestamp_verify
             push x{refund_pubkey.hex()}
         }}
         check_sig x{sigflags}
-    '''
+    ''')
 
 def make_htlc_shake256_lock(
         receiver_pubkey: bytes, preimage: bytes, refund_pubkey: bytes,
-        hash_size: int = 20, timeout: int = 60*60*24, sigflags: str = '00') -> str:
+        hash_size: int = 20, timeout: int = 60*60*24, sigflags: str = '00') -> Script:
     """Returns an HTLC that can be unlocked either with the preimage and
         a signature matching receiver_pubkey or with a signature
         matching the refund_pubkey after the timeout has expired.
         Suitable only for systems with guaranteed causal ordering and
         non-repudiation of transactions. Using a hash_size of 20 saves
         11 bytes compared to the sha256 version with a 96 bit reduction
         in security (remaining 160 bits) for the hash lock.
     """
-    return f'''
+    return Script.from_src(f'''
         shake256 d{hash_size}
         push x{shake_256(preimage).digest(20).hex()}
         equal
         if {{
             push x{receiver_pubkey.hex()}
         }} else {{
             push d{int(time())+timeout}
             check_timestamp_verify
             push x{refund_pubkey.hex()}
         }}
         check_sig x{sigflags}
-    '''
+    ''')
 
 def make_htlc_witness(
         prvkey: bytes, preimage: bytes, sigfields: dict, sigflags: str = '00'
-    ) -> str:
+    ) -> Script:
     """Returns the tapescript source for a witness to unlock either the
         hash lock or the time lock path of an HTLC, depending upon
         whether or not the preimage matches.
     """
-    _, queue, _ = run_script(
+    _, stack, _ = run_script(
         compile_script(f'push x{prvkey.hex()} sign x{sigflags}'),
         {**sigfields}
     )
-    sig = queue.get(False)
-    return f'''
+    sig = stack.get()
+    return Script.from_src(f'''
         push x{sig.hex()}
         push x{preimage.hex()}
-    '''
+    ''')
 
 def make_htlc2_sha256_lock(
         receiver_pubkey: bytes, preimage: bytes, refund_pubkey: bytes,
-        timeout: int = 60*60*24, sigflags: str = '00') -> str:
+        timeout: int = 60*60*24, sigflags: str = '00') -> Script:
     """Returns an HTLC that can be unlocked either with the preimage and
         a signature matching receiver_pubkey or with a signature
         matching the refund_pubkey after the timeout has expired.
         Suitable only for systems with guaranteed causal ordering and
         non-repudiation of transactions. This version is optimized for
         smaller locking script size (-18 bytes) at the expense of larger
         witnesses (+33 bytes) for larger overall txn size (+15 bytes).
         Which to use will depend upon the intended use case: for public
         blockchains where all nodes must hold a UTXO set in memory and
         can trim witness data after consensus, the lock script size
         reduction is significant and useful; for other use cases, in
         particular systems where witness data cannot be trimmed, the
         other version is more appropriate.
     """
-    return f'''
+    return Script.from_src(f'''
         sha256
         push x{sha256(preimage).digest().hex()}
         equal
         if {{
             dup shake256 d20
             push x{shake_256(receiver_pubkey).digest(20).hex()}
         }} else {{
             push d{int(time())+timeout}
             check_timestamp_verify
             dup shake256 d20
             push x{shake_256(refund_pubkey).digest(20).hex()}
         }}
         equal_verify
         check_sig x{sigflags}
-    '''
+    ''')
 
 def make_htlc2_shake256_lock(
         receiver_pubkey: bytes, preimage: bytes, refund_pubkey: bytes,
         hash_size: int = 20, timeout: int = 60*60*24, sigflags: str = '00'
-    ) -> str:
+    ) -> Script:
     """Returns an HTLC that can be unlocked either with the preimage and
         a signature matching receiver_pubkey or with a signature
         matching the refund_pubkey after the timeout has expired.
         Suitable only for systems with guaranteed causal ordering and
         non-repudiation of transactions. Using a hash_size of 20 saves
         11 bytes compared to the sha256 version with a 96 bit reduction
         in security (remaining 160 bits) for the hash lock. This version
@@ -613,119 +827,164 @@
         size (+15 bytes). Which to use will depend upon the intended use
         case: for public blockchains where all nodes must hold a UTXO
         set in memory and can trim witness data after consensus, the
         lock script size reduction is significant and useful; for other
         use cases, in particular systems where witness data cannot be
         trimmed, the other version is more appropriate.
     """
-    return f'''
+    return Script.from_src(f'''
         shake256 d{hash_size}
         push x{shake_256(preimage).digest(20).hex()}
         equal
         if {{
             dup shake256 d20
             push x{shake_256(receiver_pubkey).digest(20).hex()}
         }} else {{
             push d{int(time())+timeout}
             check_timestamp_verify
             dup shake256 d20
             push x{shake_256(refund_pubkey).digest(20).hex()}
         }}
         equal_verify
         check_sig x{sigflags}
-    '''
+    ''')
 
 def make_htlc2_witness(
         prvkey: bytes, preimage: bytes, sigfields: dict, sigflags: str = '00'
-    ) -> str:
+    ) -> Script:
     """Returns the tapescript source for a witness to unlock either the
         hash lock or the time lock path of an HTLC, depending upon
         whether or not the preimage matches. This version is optimized
         for smaller locking script size (-18 bytes) at the expense of
         larger witnesses (+33 bytes) for larger overall txn size (+15
         bytes). Which to use will depend upon the intended use case: for
         public blockchains where all nodes must hold a UTXO set in
         memory and can trim witness data after consensus, the lock
         script size reduction is significant and useful; for other use
         cases, in particular systems where witness data cannot be
         trimmed, the other version is more appropriate.
     """
-    _, queue, _ = run_script(
+    _, stack, _ = run_script(
         compile_script(f'''
             push x{prvkey.hex()}
             dup derive_scalar derive_point
             swap2 sign x{sigflags}
         '''),
         {**sigfields}
     )
-    sig = queue.get(False)
-    pubkey = queue.get(False)
-    return f'''
+    sig = stack.get()
+    pubkey = stack.get()
+    return Script.from_src(f'''
         push x{sig.hex()}
         push x{pubkey.hex()}
         push x{preimage.hex()}
-    '''
+    ''')
 
 def make_ptlc_lock(
         receiver_pubkey: bytes, refund_pubkey: bytes, tweak_point: bytes = None,
-        timeout: int = 60*60*24, sigflags: str = '00') -> str:
+        timeout: int = 60*60*24, sigflags: str = '00') -> Script:
     """Returns the tapescript source for a Point Time Locked Contract
         that can be unlcoked with either a signature matching the
         receiver_pubkey or with a signature matching the refund_pubkey
         after the timeout has expired. Suitable only for systems with
         guaranteed causal ordering and non-repudiation of transactions.
         If a tweak_point is passed, use tweak_point+receiver_pubkey as
         the point lock.
     """
     if type(tweak_point) is bytes:
         receiver_pubkey = aggregate_points([receiver_pubkey, tweak_point])
-    return f'''
+    return Script.from_src(f'''
         if {{
             push x{receiver_pubkey.hex()}
         }} else {{
             push d{int(time())+timeout}
             check_timestamp_verify
             push x{refund_pubkey.hex()}
         }}
         check_sig x{sigflags}
-    '''
+    ''')
 
 def make_ptlc_witness(
         prvkey: bytes, sigfields: dict, tweak_scalar: bytes = None,
-        sigflags: str = '00') -> str:
+        sigflags: str = '00') -> Script:
     '''Returns the tapescript source for a PTLC witness unlocking the
         main branch. If a tweak_scalar is passed, add tweak_scalar to x
         within signature generation to unlock the point corresponding to
         derive_point(tweak_scalar)+derive_point(x).
     '''
     if tweak_scalar:
         # create signature manually
-        _, queue, _ = run_script(compile_script(f'get_message x{sigflags}'), {**sigfields})
-        m = queue.get(False)
+        _, stack, _ = run_script(compile_script(f'get_message x{sigflags}'), {**sigfields})
+        m = stack.get()
         x = aggregate_scalars([derive_key_from_seed(prvkey), tweak_scalar])
-        X = nacl.bindings.crypto_scalarmult_ed25519_base_noclamp(x) # G^x
-        r = clamp_scalar(H_small(H_big(prvkey)[32:], m))
-        R = nacl.bindings.crypto_scalarmult_ed25519_base_noclamp(r) # G^r
-        c = clamp_scalar(H_small(R, X, m)) # clamp(H(R || X || m))
-        s = nacl.bindings.crypto_core_ed25519_scalar_add(
-            r, nacl.bindings.crypto_core_ed25519_scalar_mul(c, x)
-        )
-        return f'push x{R.hex() + s.hex()}{sigflags} true'
-    return f'{make_single_sig_witness(prvkey, sigfields, sigflags)} true'
+        sig = sign_with_scalar(x, m)
+        return Script.from_src(f'push x{sig.hex()}{sigflags} true')
+    return Script.from_src(f'{make_single_sig_witness(prvkey, sigfields, sigflags).src} true')
 
-def make_ptlc_refund_witness(prvkey: bytes, sigfields: dict, sigflags: str = '00') -> str:
+def make_ptlc_refund_witness(
+        prvkey: bytes, sigfields: dict, sigflags: str = '00') -> Script:
     '''Returns the tapescript source for a PTLC witness unlcoking the
         time locked refund branch.
     '''
-    return f'{make_single_sig_witness(prvkey, sigfields, sigflags)} false'
+    return Script.from_src(f'{make_single_sig_witness(prvkey, sigfields, sigflags).src} false')
+
+def make_taproot_lock(
+        pubkey: bytes, script: Script = None, script_commitment: bytes = None
+    ) -> Script:
+    """Returns a tapescript Script for a taproot locking script that can
+        either be unlocked with a signature that validates using the
+        taproot root commitment as a public key or by supplying both the
+        committed script and the committed public key to execute the
+        committed script.
+    """
+    tert(isinstance(script, Script) or type(script_commitment) is bytes,
+         'must supply either committed_script or script_commitment')
+    script_commitment = script_commitment or script.commitment()
+    vert(len(script_commitment) == 32, 'script_commitment must be 32 bytes')
+    X = derive_point_from_scalar(clamp_scalar(sha256(pubkey + script_commitment).digest()))
+    root = aggregate_points((pubkey, X))
+    return Script.from_src(f'taproot x{root.hex()}')
+
+def make_taproot_witness_keyspend(
+        prvkey: bytes, sigfields: dict, committed_script: Script = None,
+        script_commitment: bytes = None, sigflags: str = '00') -> Script:
+    """Returns a tapescript Script witness for a taproot keyspend."""
+    tert(type(prvkey) is bytes, 'prvkey must be the 32 byte prvkey seed')
+    vert(len(prvkey) == 32, 'prvkey must be the 32 byte prvkey seed')
+    tert(isinstance(sigfields, dict), 'must supply sigfields dict')
+    tert(isinstance(committed_script, Script) or type(script_commitment) is bytes,
+         'must supply either committed_script or script_commitment')
+    vert(sigflags != 'ff', 'cannot use sigflag xFF; must sign at least 1 sigfield')
+
+    script_commitment = script_commitment or committed_script.commitment()
+    x = derive_key_from_seed(prvkey)
+    X = derive_point_from_scalar(x)
+    t = clamp_scalar(sha256(X + script_commitment).digest())
+    _, stack, _ = run_script(Script.from_src(f'msg x{sigflags}'), sigfields)
+    message = stack.get()
+    sig = sign_with_scalar(aggregate_scalars((x, t)), message)
+
+    if sigflags != '00':
+        return Script.from_src(f'@= trsf [ x{sigflags} ] push x{sig.hex()}{sigflags}')
+    return Script.from_src(f'push x{sig.hex()}')
+
+def make_taproot_witness_scriptspend(
+        pubkey: bytes, committed_script: Script) -> Script:
+    """Returns a tapescript Script witness for a taproot scriptspend,
+        i.e. a witness that causes the committed script to be executed.
+    """
+    tert(type(pubkey) is bytes, 'pubkey must be the 32 byte committed pubkey')
+    vert(len(pubkey) == 32, 'pubkey must be the 32 byte committed pubkey')
+    tert(isinstance(committed_script, ScriptProtocol), 'committed_script must be ScriptProtocol')
+    return Script.from_src(f'push x{committed_script.bytes.hex()} push x{pubkey.hex()}')
 
 def setup_amhl(
         seed: bytes, pubkeys: tuple[bytes]|list[bytes], sigflags: str = '00',
         refund_pubkeys: dict[bytes] = None, timeout: int = 60*60*24
-    ) -> dict[bytes|str, bytes|tuple[str|bytes]]:
+    ) -> dict[bytes|str, bytes|tuple[Script|bytes, ...]]:
     """Sets up an annoymous multi-hop lock for a sorted list of pubkeys.
         Returns a dict mapping each public key to a tuple containing the
         tuple of scripts returned by make_adapter_locks_pub and the
         tweak point for the hop, and mapping the key 'key' to the first
         tweak scalar needed to unlock the last hop in the AMHL and begin
         the cascade back to the funding source. The order of pubkeys
         must start with the originator and end with the correspondent
@@ -749,20 +1008,23 @@
         if type(refund_pubkeys) is dict and pk in refund_pubkeys:
             result[pk][1] = make_ptlc_lock(
                 pk, refund_pubkeys[pk], timeout=timeout, sigflags=sigflags)
         result[pk] = tuple(result[pk])
     result['key'] = AMHL.setup_for(setup, n)[-1]
     return result
 
-def release_left_amhl_lock(adapter_witness: bytes, signature: bytes, y: bytes) -> bytes:
+def release_left_amhl_lock(
+        adapter_witness: bytes|ScriptProtocol, signature: bytes, y: bytes) -> bytes:
     """Release the next lock using an adapter witness and a decrypted
         signature from right lock. Returns the tweak scalar used to
         decrypt the left adapter signature.
     """
-    tert(type(adapter_witness) is bytes, 'adapter_witness must be bytes of len 66')
+    tert(type(adapter_witness) is bytes or isinstance(adapter_witness, ScriptProtocol),
+         'adapter_witness must be bytes or ScriptProtocol of bytes len 66')
+    adapter_witness = bytes(adapter_witness)
     vert(len(adapter_witness) == 68, 'adapter_witness must be bytes of len 68')
     tert(type(signature) is bytes, 'signature must be bytes of len 64 or 65')
     vert(len(signature) == 64, 'signature must be bytes of len 64')
     sa = adapter_witness[2:34]
     s = signature[32:]
     t = nacl.bindings.crypto_core_ed25519_scalar_sub(s, sa) # s = sa + t
     return AMHL.release(t, y)
@@ -772,15 +1034,15 @@
     name = argv[0]
     return '\n'.join([
         f'Usage: {name} [method] [options]',
         '\tcompile src_file bin_file -- compiles the source code into bytecode '
         'and writes it to bin_file',
         '\tdecompile bin_file -- decompiles the bytecode and outputs to stdout',
         '\trun bin_file [cache_file] -- runs tapescript bytecode and prints the '
-        'resulting cache and queue',
+        'resulting cache and stack',
         '\tauth bin_file [cache_file] -- runs tapescript bytecode as auth script'
         ' and prints true if it was successful or false otherwise\n',
         'The optional cache_file parameter must be a json file with the '
         'following format:',
         '{', '\t"type:name": [type, value]', '}\n',
         'The type must be one of "string", "str", "number", "bytes". All bytes '
         'values must be hexadecimal strings. For example:',
@@ -852,25 +1114,25 @@
         case 'run':
             _clert(len(argv) >= 3, 'Must supply bin_file parameter.')
             bin_fname, script, cache = argv[2], b'', {}
             with open(bin_fname, 'rb') as f:
                 script = f.read()
             if len(argv) > 3:
                 cache = _parse_cache_json(argv[3])
-            _, queue, cache = run_script(script, cache)
+            _, stack, cache = run_script(script, cache)
             items = []
-            while queue.qsize():
-                items.append(queue.get(False).hex())
+            while len(stack):
+                items.append(stack.get().hex())
             items.reverse()
             cache = {
                 (f'bytes:{k.hex()}' if type(k) is bytes else k):
                 f'bytes:{v.hex()}' if type(v) is bytes else v
                 for k, v in cache.items()
             }
-            print(f'queue:\n' + '\n'.join(items))
+            print(f'stack:\n' + '\n'.join(items))
             print(f'cache:\n{cache}')
         case 'auth':
             _clert(len(argv) >= 3, 'Must supply bin_file parameter.')
             bin_fname, script, cache = argv[2], b'', {}
             with open(bin_fname, 'rb') as f:
                 script = f.read()
             if len(argv) > 3:
```

### Comparing `tapescript-0.4.1/tests/test_e2e_eltoo.py` & `tapescript-0.5.0/tests/test_e2e_eltoo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from context import functions, parsing
+from context import functions, tools
 from dataclasses import dataclass, field
 from hashlib import sha256
 from nacl.signing import SigningKey, VerifyKey
 from time import time
 import struct
 import unittest
 
@@ -11,42 +11,49 @@
 '''Example implementation of the eltoo protocol. The primary deviation
     from Example 6 from script_examples.md is that UTXOs are simply
     serialized rather than referenced via txn_id and index in the
     witness data creation and verification -- as written, Example 6
     requires looking up the UTXO data before creating or verifying any
     witness data. I did not want to implement an entire blockchain for
     this test and was interested only in the eltoo mechanism itself.
+
+    The Eltoo proposed OP_CHECKSEQUENCEVERIFY is simulated by putting
+    the state integer into sigfield3 and comparing in the locking script
+    with OP_LESS OP_VERIFY. For channel updates, inputs are encoded in
+    sigfield1 and excluded from signature checks using sigflag of 0x01.
+    For channel closures (i.e. time lock branch), a sigflag of 0x00 is
+    used to require signature commitment to the whole transaction.
 '''
 
 
 @dataclass
 class UTXO:
-    lock: bytes = field(default=b'\x01')
+    lock: tools.Script = field(default_factory=lambda: tools.Script.from_src('true'))
     amount: int = field(default=0)
     spent: bool = field(default=False)
     txn: Txn|None = field(default=None)
 
     def pack(self) -> bytes:
         return struct.pack(
-            f'!{len(self.lock)}sh?',
-            self.lock,
+            f'!{len(self.lock.bytes)}sH?',
+            self.lock.bytes,
             self.amount,
             self.spent
         )
 
     @classmethod
     def unpack(cls, data: bytes) -> UTXO:
-        lock, amount, spent = struct.unpack(f'!{len(data)-3}sh?', data)
-        return cls(lock=lock,amount=amount,spent=spent)
+        lock, amount, spent = struct.unpack(f'!{len(data)-3}sH?', data)
+        return cls(lock=tools.Script.from_bytes(lock),amount=amount,spent=spent)
 
 @dataclass
 class Entry:
     inputs: list[UTXO] = field(default_factory=list)
     outputs: list[UTXO] = field(default_factory=list)
-    witnesses: list[bytes] = field(default_factory=list)
+    witnesses: list[tools.Script] = field(default_factory=list)
 
     def pack_inputs(self) -> bytes:
         inputs = b''
         for i in self.inputs:
             i = i.pack()
             inputs = inputs + struct.pack(f'!h{len(i)}s', i)
         return inputs
@@ -57,63 +64,63 @@
             o = o.pack()
             outputs = outputs + struct.pack(f'!h{len(o)}s', o)
         return outputs
 
     def pack_witnesses(self) -> bytes:
         witnesses = b''
         for w in self.witnesses:
-            witnesses += struct.pack(f'!h{len(w)}s', w)
+            witnesses += struct.pack(f'!h{len(w.bytes)}s', w.bytes)
         return witnesses
 
     def pack(self) -> bytes:
         inputs = self.pack_inputs()
         outputs = self.pack_outputs()
         witnesses = self.pack_witnesses()
         return struct.pack(
-            f'!hhh{len(inputs)}s{len(outputs)}s{len(witnesses)}s',
+            f'!HHH{len(inputs)}s{len(outputs)}s{len(witnesses)}s',
             len(inputs),
             len(outputs),
             len(witnesses),
             inputs,
             outputs,
             witnesses,
         )
 
     def pack_without_witnesses(self) -> bytes:
         inputs = self.pack_inputs()
         outputs = self.pack_outputs()
         return struct.pack(
-            f'!hh{len(inputs)}s{len(outputs)}s',
+            f'!HH{len(inputs)}s{len(outputs)}s',
             len(inputs),
             len(outputs),
             inputs,
             outputs,
         )
 
     def id(self) -> bytes:
         return sha256(self.pack_without_witnesses()).digest()
 
     @classmethod
     def unpack(cls, data: bytes) -> Entry:
-        ilen, olen, wlen, data = struct.unpack(f'!hhh{len(data)-6}s', data)
+        ilen, olen, wlen, data = struct.unpack(f'!HHH{len(data)-6}s', data)
         idata, odata, wdata = struct.unpack(f'!{ilen}s{olen}s{wlen}s', data)
         inputs = []
         while len(idata):
-            ilen, idata = struct.unpack(f'!h{len(idata)-2}s', idata)
+            ilen, idata = struct.unpack(f'!H{len(idata)-2}s', idata)
             inputs.append(UTXO.unpack(idata[:ilen]))
             idata = idata[ilen:]
         outputs = []
         while len(odata):
-            olen, odata = struct.unpack(f'!h{len(odata)-2}s', odata)
+            olen, odata = struct.unpack(f'!H{len(odata)-2}s', odata)
             outputs.append(UTXO.unpack(odata[:olen]))
             odata = odata[olen:]
         witnesses = []
         while len(wdata):
-            wlen, wdata = struct.unpack(f'!h{len(wdata)-2}s', wdata)
-            witnesses.append(wdata[:wlen])
+            wlen, wdata = struct.unpack(f'!H{len(wdata)-2}s', wdata)
+            witnesses.append(tools.Script.from_bytes(wdata[:wlen]))
             wdata = wdata[wlen:]
         return cls(inputs=inputs, outputs=outputs, witnesses=witnesses)
 
 @dataclass
 class Txn:
     sequence: int = field()
     timestamp: int = field(default_factory=lambda: int(time()))
@@ -129,15 +136,15 @@
             self.sequence,
             self.timestamp,
             entries,
         )
 
     def entries_root(self) -> bytes:
         """Get the root hash for all entries."""
-        return sha256(b''.join([e.id() for e in self.entries])).digest()
+        return sha256(b''.join(sorted([e.id() for e in self.entries]))).digest()
 
     def id(self) -> bytes:
         return sha256(struct.pack(
             f'!ii32s',
             self.sequence,
             self.timestamp,
             self.entries_root(),
@@ -150,23 +157,23 @@
         while len(edata):
             elen, edata = struct.unpack(f'!h{len(edata)}s', edata)
             entries.append(Entry.unpack(edata[:elen]))
             edata = edata[elen:]
         return cls(sequence=sequence, timestamp=timestamp, entries=entries)
 
 
-def eltoo_setup_lock(pubkeyA: bytes, pubkeyB: bytes) -> bytes:
-    return parsing.compile_script(f'''
+def eltoo_setup_lock(pubkeyA: bytes, pubkeyB: bytes) -> tools.Script:
+    return tools.Script.from_src(f'''
         PUSH x{bytes(pubkeyA).hex()}
         PUSH x{bytes(pubkeyB).hex()}
         CHECK_MULTISIG x00 d2 d2
     ''')
 
-def eltoo_update_lock(pubkeyA: bytes, pubkeyB: bytes, state: int) -> bytes:
-    return parsing.compile_script(f'''
+def eltoo_update_lock(pubkeyA: bytes, pubkeyB: bytes, state: int) -> tools.Script:
+    return tools.Script.from_src(f'''
         if {"{"}
             val s"sigfield4"
             # 2 second delay is all I'm willing to wait in a test #
             val s"input_ts" push d2 add_ints d2
             less verify
             val s"time"
             val s"sigfield4"
@@ -182,18 +189,18 @@
             push x{bytes(pubkeyB).hex()}
             check_multisig x01 d2 d2
         {"}"}
     ''')
 
 def eltoo_witness(
         prvkeyA: SigningKey, prvkeyB: SigningKey, message: bytes,
-        sigflag: str = '') -> bytes:
+        sigflag: str = '') -> tools.Script:
     sigA = prvkeyA.sign(message).signature
     sigB = prvkeyB.sign(message).signature
-    return parsing.compile_script(f'''
+    return tools.Script.from_src(f'''
         push x{sigB.hex()}{sigflag}
         push x{sigA.hex()}{sigflag}
     ''')
 
 def validate_txn(txn: Txn) -> bool:
     for entry in txn.entries:
         input_ts = max([
@@ -208,16 +215,16 @@
                 {
                     'sigfield1': b''.join([
                         n.pack() for n in entry.inputs
                     ]),
                     'sigfield2': b''.join([
                         o.pack() for o in entry.outputs
                     ]),
-                    'sigfield3': functions.int_to_bytes(txn.sequence),
-                    'sigfield4': functions.int_to_bytes(txn.timestamp),
+                    'sigfield3': functions.uint_to_bytes(txn.sequence),
+                    'sigfield4': functions.uint_to_bytes(txn.timestamp),
                     'time': int(time()),
                     'input_ts': input_ts,
                 }
             ):
                 return False
         input_sum = sum([i.amount for i in entry.inputs])
         output_sum = sum([o.amount for o in entry.outputs])
@@ -239,46 +246,46 @@
         self.pubkeyB = self.prvkeyB.verify_key
         return super().setUp()
 
     def test_auto_validate(self):
         genesis_utxo = UTXO(amount=10)
         genesis_entry = Entry([], [genesis_utxo])
         genesis_txn = Txn(0, entries=[genesis_entry])
-        genesis_entry.txn = genesis_txn
+        genesis_utxo.txn = genesis_txn
 
-        burn_utxo = UTXO(b'\x00', amount=10)
-        burn_entry = Entry([genesis_utxo], [burn_utxo], [b''])
+        burn_utxo = UTXO(tools.Script.from_src('false'), amount=10)
+        burn_entry = Entry([genesis_utxo], [burn_utxo], [tools.Script('', b'')])
         burn_txn = Txn(1, entries=[burn_entry])
         assert validate_txn(burn_txn)
 
     def test_single_sig(self):
-        genesis_utxo = UTXO(parsing.compile_script(f'''
+        genesis_utxo = UTXO(tools.Script.from_src(f'''
             push x{bytes(self.pubkeyA).hex()}
             check_sig x00
         '''), 100)
         spend_utxo = UTXO(amount=5)
         ts = int(time())
         sig = self.prvkeyA.sign(
             genesis_utxo.pack() + spend_utxo.pack() +
             b'\x01' + functions.int_to_bytes(ts)
         ).signature
         spend_entry = Entry([genesis_utxo], [spend_utxo], [
-            parsing.compile_script(f'push x{sig.hex()}')
+            tools.Script.from_src(f'push x{sig.hex()}')
         ])
         spend_txn = Txn(1, ts, [spend_entry])
         assert validate_txn(spend_txn)
 
     def test_eltoo_e2e(self):
         """A proof-of-concept eltoo implementation."""
-        op_false, op_true = b'\x00', b'\x01'
-        settle_A_lock = parsing.compile_script(f'''
+        op_false, op_true = tools.Script.from_src('false'), tools.Script.from_src('true')
+        settle_A_lock = tools.Script.from_src(f'''
             push x{bytes(self.pubkeyA).hex()}
             check_sig x00
         ''')
-        settle_B_lock = parsing.compile_script(f'''
+        settle_B_lock = tools.Script.from_src(f'''
             push x{bytes(self.pubkeyB).hex()}
             check_sig x00
         ''')
         setup_lock = eltoo_setup_lock(self.pubkeyA, self.pubkeyB)
         setup_utxo = UTXO(setup_lock, 100)
         state = 0
```

### Comparing `tapescript-0.4.1/tests/test_functions.py` & `tapescript-0.5.0/tests/test_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from context import classes, errors, functions, interfaces
 from hashlib import sha256, shake_256
 from nacl.signing import SigningKey
-from queue import LifoQueue
 from random import randint
 from secrets import token_bytes
 from time import time
 from typing import Protocol, runtime_checkable
 import nacl.bindings
 import unittest
 
@@ -33,28 +32,33 @@
     def does_thing(self):
         ...
 
 class DoesThing:
     def does_thing(self):
         ...
 
+def merkleval_root(commitment1: bytes, commitment2: bytes) -> bytes:
+    return functions.xor(
+        sha256(commitment1).digest(),
+        sha256(commitment2).digest(),
+    )
 
 class TestFunctions(unittest.TestCase):
     tape: classes.Tape
-    queue: LifoQueue
+    stack: classes.Stack
     cache: dict
     original_opcodes: dict
     original_nopcodes: dict
     original_opcodes_inverse: dict
     original_nopcodes_inverse: dict
     original_contract_interfaces: dict
 
     def setUp(self) -> None:
         self.tape = classes.Tape(b'')
-        self.queue = LifoQueue()
+        self.stack = classes.Stack()
         self.cache = {}
         self.original_opcodes = {**functions.opcodes}
         self.original_opcodes_inverse = {**functions.opcodes_inverse}
         self.original_nopcodes = {**functions.nopcodes}
         self.original_nopcodes_inverse = {**functions.nopcodes_inverse}
         self.original_contract_interfaces = {**functions._contract_interfaces}
         return super().setUp()
@@ -131,1761 +135,1771 @@
         assert str(e.exception) == 'number must be float'
 
     def test_float_to_bytes_returns_bytes(self):
         number = functions.float_to_bytes(123.0394)
         assert type(number) is bytes
 
     # ops
-    def test_OP_FALSE_puts_null_byte_onto_queue(self):
-        assert self.queue.empty()
+    def test_OP_FALSE_puts_null_byte_onto_stack(self):
+        assert self.stack.empty()
         assert not len(self.cache.keys())
-        functions.OP_FALSE(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
+        functions.OP_FALSE(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
         assert not len(self.cache.keys())
-        assert self.queue.get() == b'\x00'
+        assert self.stack.get() == b'\x00'
 
-    def test_OP_TRUE_puts_nonnull_byte_onto_queue(self):
-        assert self.queue.empty()
+    def test_OP_TRUE_puts_nonnull_byte_onto_stack(self):
+        assert self.stack.empty()
         assert not len(self.cache.keys())
-        functions.OP_TRUE(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
+        functions.OP_TRUE(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
         assert not len(self.cache.keys())
-        assert functions.bytes_to_bool(self.queue.get())
+        assert functions.bytes_to_bool(self.stack.get())
 
-    def test_OP_PUSH0_puts_next_byte_from_tape_onto_queue(self):
+    def test_OP_PUSH0_puts_next_byte_from_tape_onto_stack(self):
         self.tape = classes.Tape(b'123')
-        assert self.queue.empty()
+        assert self.stack.empty()
         assert not len(self.cache.keys())
-        functions.OP_PUSH0(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
+        functions.OP_PUSH0(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
         assert not len(self.cache.keys())
-        assert self.queue.get() == b'1'
+        assert self.stack.get() == b'1'
 
-    def test_OP_PUSH1_reads_next_byte_as_uint_and_puts_that_many_from_tape_onto_queue(self):
+    def test_OP_PUSH1_reads_next_byte_as_uint_and_puts_that_many_from_tape_onto_stack(self):
         self.tape = classes.Tape(functions.int_to_bytes(11) + b'hello world')
-        assert self.queue.empty()
+        assert self.stack.empty()
         assert not len(self.cache.keys())
-        functions.OP_PUSH1(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
+        functions.OP_PUSH1(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
         assert not len(self.cache.keys())
-        assert self.queue.get() == b'hello world'
+        assert self.stack.get() == b'hello world'
 
-    def test_OP_PUSH2_reads_next_2_bytes_as_uint_and_puts_that_many_from_tape_onto_queue(self):
+    def test_OP_PUSH2_reads_next_2_bytes_as_uint_and_puts_that_many_from_tape_onto_stack(self):
         self.tape = classes.Tape(b'\x00' + functions.int_to_bytes(11) + b'hello world')
-        assert self.queue.empty()
+        assert self.stack.empty()
         assert not len(self.cache.keys())
-        functions.OP_PUSH2(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
+        functions.OP_PUSH2(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
         assert not len(self.cache.keys())
-        assert self.queue.get() == b'hello world'
+        assert self.stack.get() == b'hello world'
 
-    def test_OP_PUSH4_reads_next_4_bytes_as_uint_and_puts_that_many_from_tape_onto_queue(self):
-        self.tape = classes.Tape(b'\x00\x00\x00' + functions.int_to_bytes(11) + b'hello world')
-        assert self.queue.empty()
+    def test_OP_POP0_moves_one_item_from_stack_into_cache(self):
+        self.stack.put(b'1234')
+        assert not self.stack.empty()
         assert not len(self.cache.keys())
-        functions.OP_PUSH4(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        assert not len(self.cache.keys())
-        assert self.queue.get() == b'hello world'
-
-    def test_OP_POP0_moves_one_item_from_queue_into_cache(self):
-        self.queue.put(b'1234')
-        assert not self.queue.empty()
-        assert not len(self.cache.keys())
-        functions.OP_POP0(self.tape, self.queue, self.cache)
-        assert self.queue.empty()
+        functions.OP_POP0(self.tape, self.stack, self.cache)
+        assert self.stack.empty()
         assert len(self.cache.keys())
         assert b'P' in self.cache
         assert self.cache[b'P'] == [b'1234']
 
-    def test_OP_POP1_reads_uint_from_tape_then_puts_that_many_items_from_queue_to_cache(self):
-        assert self.queue.empty()
-        self.queue.put(b'12')
-        self.queue.put(b'34')
+    def test_OP_POP1_reads_uint_from_tape_then_puts_that_many_items_from_stack_to_cache(self):
+        assert self.stack.empty()
+        self.stack.put(b'12')
+        self.stack.put(b'34')
         self.tape = classes.Tape(functions.int_to_bytes(2))
-        assert not self.queue.empty()
+        assert not self.stack.empty()
         assert b'P' not in self.cache
-        functions.OP_POP1(self.tape, self.queue, self.cache)
-        assert self.queue.empty()
+        functions.OP_POP1(self.tape, self.stack, self.cache)
+        assert self.stack.empty()
         assert b'P' in self.cache
         assert self.cache[b'P'] == [b'34', b'12']
 
     def test_OP_POP1_interprets_negative_ints_as_positive(self):
-        assert self.queue.empty()
+        assert self.stack.empty()
         for i in range(136):
-            self.queue.put(functions.int_to_bytes(i))
+            self.stack.put(functions.int_to_bytes(i))
         self.tape = classes.Tape(functions.int_to_bytes(-120))
-        functions.OP_POP1(self.tape, self.queue, self.cache)
-        assert self.queue.empty()
+        functions.OP_POP1(self.tape, self.stack, self.cache)
+        assert self.stack.empty()
         assert b'P' in self.cache
         assert len(self.cache[b'P']) == 136
 
-    def test_OP_SIZE_pulls_item_from_queue_and_puts_its_length_onto_queue(self):
-        assert self.queue.empty()
-        self.queue.put(b'123')
-        functions.OP_SIZE(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+    def test_OP_SIZE_pulls_item_from_stack_and_puts_its_length_onto_stack(self):
+        assert self.stack.empty()
+        self.stack.put(b'123')
+        functions.OP_SIZE(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        item = self.stack.get()
         assert item == functions.int_to_bytes(3)
 
-    def test_OP_WRITE_CACHE_reads_cache_key_and_int_from_tape_and_moves_from_queue_to_cache(self):
+    def test_OP_WRITE_CACHE_reads_cache_key_and_int_from_tape_and_moves_from_stack_to_cache(self):
         self.tape = classes.Tape(
             functions.int_to_bytes(4) +
             b'test' +
             functions.int_to_bytes(2)
         )
-        assert self.queue.empty()
+        assert self.stack.empty()
         assert not len(self.cache.keys())
-        self.queue.put(b'1')
-        self.queue.put(b'2')
-        functions.OP_WRITE_CACHE(self.tape, self.queue, self.cache)
-        assert self.queue.empty()
+        self.stack.put(b'1')
+        self.stack.put(b'2')
+        functions.OP_WRITE_CACHE(self.tape, self.stack, self.cache)
+        assert self.stack.empty()
         assert b'test' in self.cache
         assert self.cache[b'test'] == [b'2', b'1']
 
-    def test_OP_READ_CACHE_reads_cache_key_from_tape_and_moves_values_from_cache_to_queue(self):
+    def test_OP_READ_CACHE_reads_cache_key_from_tape_and_moves_values_from_cache_to_stack(self):
         self.cache[b'test'] = [b'2', b'1']
         self.tape = classes.Tape(functions.int_to_bytes(4) + b'test')
-        assert self.queue.empty()
-        functions.OP_READ_CACHE(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
+        assert self.stack.empty()
+        functions.OP_READ_CACHE(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
         assert self.cache[b'test'] == [b'2', b'1']
-        items = [self.queue.get(False), self.queue.get(False)]
+        items = [self.stack.get(), self.stack.get()]
         assert items == [b'1', b'2']
 
     def test_OP_READ_CACHE_raises_ScriptExecutionError_for_missing_cache_key(self):
         self.tape = classes.Tape(functions.int_to_bytes(4) + b'test')
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_READ_CACHE(self.tape, self.queue, self.cache)
+            functions.OP_READ_CACHE(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_READ_CACHE key not in cache'
 
-    def test_OP_READ_CACHE_SIZE_reads_cache_key_from_tape_and_puts_size_of_cache_on_queue(self):
+    def test_OP_READ_CACHE_SIZE_reads_cache_key_from_tape_and_puts_size_of_cache_on_stack(self):
         self.cache[b'test'] = [b'2', b'1']
         self.tape = classes.Tape(functions.int_to_bytes(4) + b'test')
-        assert self.queue.empty()
-        functions.OP_READ_CACHE_SIZE(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
+        assert self.stack.empty()
+        functions.OP_READ_CACHE_SIZE(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
         assert self.cache[b'test'] == [b'2', b'1']
-        item = self.queue.get(False)
-        assert self.queue.empty()
+        item = self.stack.get()
+        assert self.stack.empty()
         assert item == functions.int_to_bytes(2)
 
-    def test_OP_READ_CACHE_Q_reads_cache_key_from_queue_and_moves_items_from_cache_to_queue(self):
+    def test_OP_READ_CACHE_STACK_reads_cache_key_from_stack_and_moves_items_from_cache_to_stack(self):
         self.cache[b'test'] = [b'2', b'1']
-        assert self.queue.empty()
-        self.queue.put(b'test')
-        functions.OP_READ_CACHE_Q(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
+        assert self.stack.empty()
+        self.stack.put(b'test')
+        functions.OP_READ_CACHE_STACK(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
         assert self.cache[b'test'] == [b'2', b'1']
-        items = [self.queue.get(False), self.queue.get(False)]
-        assert self.queue.empty()
+        items = [self.stack.get(), self.stack.get()]
+        assert self.stack.empty()
         assert items == [b'1', b'2']
 
-    def test_OP_READ_CACHE_Q_raises_ScriptExecutionError_for_missing_cache_key(self):
-        self.queue.put(b'test')
+    def test_OP_READ_CACHE_STACK_raises_ScriptExecutionError_for_missing_cache_key(self):
+        self.stack.put(b'test')
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_READ_CACHE_Q(self.tape, self.queue, self.cache)
-        assert str(e.exception) == 'OP_READ_CACHE_Q key not in cache'
+            functions.OP_READ_CACHE_STACK(self.tape, self.stack, self.cache)
+        assert str(e.exception) == 'OP_READ_CACHE_STACK key not in cache'
 
-    def test_OP_READ_CACHE_Q_SIZE_reads_cache_key_from_queue_and_puts_size_of_cache_on_queue(self):
+    def test_OP_READ_CACHE_STACK_SIZE_reads_cache_key_from_stack_and_puts_size_of_cache_on_stack(self):
         self.cache[b'test'] = [b'2', b'1']
-        assert self.queue.empty()
-        self.queue.put(b'test')
-        functions.OP_READ_CACHE_Q_SIZE(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
+        assert self.stack.empty()
+        self.stack.put(b'test')
+        functions.OP_READ_CACHE_STACK_SIZE(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
         assert self.cache[b'test'] == [b'2', b'1']
-        item = self.queue.get(False)
-        assert self.queue.empty()
+        item = self.stack.get()
+        assert self.stack.empty()
         assert item == functions.int_to_bytes(2)
 
-    def test_OP_ADD_INTS_reads_uint_from_tape_pulls_that_many_ints_from_queue_and_puts_sum_on_queue(self):
+    def test_OP_ADD_INTS_reads_uint_from_tape_pulls_that_many_ints_from_stack_and_puts_sum_on_stack(self):
         self.tape = classes.Tape(functions.int_to_bytes(3))
-        assert self.queue.empty()
-        self.queue.put(functions.int_to_bytes(2))
-        self.queue.put(functions.int_to_bytes(5))
-        self.queue.put(functions.int_to_bytes(-3))
-        functions.OP_ADD_INTS(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        item = self.queue.get(False)
-        assert self.queue.empty()
+        assert self.stack.empty()
+        self.stack.put(functions.int_to_bytes(2))
+        self.stack.put(functions.int_to_bytes(5))
+        self.stack.put(functions.int_to_bytes(-3))
+        functions.OP_ADD_INTS(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        item = self.stack.get()
+        assert self.stack.empty()
         assert not self.cache
         assert functions.bytes_to_int(item) == 4
 
-    def test_OP_SUBTRACT_INTS_reads_uint_from_tape_pulls_that_many_ints_from_queue_and_puts_difference_on_queue(self):
+    def test_OP_SUBTRACT_INTS_reads_uint_from_tape_pulls_that_many_ints_from_stack_and_puts_difference_on_stack(self):
         self.tape = classes.Tape(functions.int_to_bytes(3))
-        assert self.queue.empty()
-        self.queue.put(functions.int_to_bytes(-3))
-        self.queue.put(functions.int_to_bytes(2))
-        self.queue.put(functions.int_to_bytes(5))
-        functions.OP_SUBTRACT_INTS(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        item = self.queue.get(False)
-        assert self.queue.empty()
+        assert self.stack.empty()
+        self.stack.put(functions.int_to_bytes(-3))
+        self.stack.put(functions.int_to_bytes(2))
+        self.stack.put(functions.int_to_bytes(5))
+        functions.OP_SUBTRACT_INTS(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        item = self.stack.get()
+        assert self.stack.empty()
         assert not self.cache
         assert functions.bytes_to_int(item) == 6
 
-    def test_OP_MULT_INTS_reads_uint_from_tape_pulls_that_many_ints_from_queue_and_puts_product_on_queue(self):
+    def test_OP_MULT_INTS_reads_uint_from_tape_pulls_that_many_ints_from_stack_and_puts_product_on_stack(self):
         self.tape = classes.Tape(functions.int_to_bytes(4))
-        assert self.queue.empty()
-        self.queue.put(functions.int_to_bytes(3))
-        self.queue.put(functions.int_to_bytes(2))
-        self.queue.put(functions.int_to_bytes(-2))
-        self.queue.put(functions.int_to_bytes(5))
-        functions.OP_MULT_INTS(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        item = self.queue.get(False)
-        assert self.queue.empty()
+        assert self.stack.empty()
+        self.stack.put(functions.int_to_bytes(3))
+        self.stack.put(functions.int_to_bytes(2))
+        self.stack.put(functions.int_to_bytes(-2))
+        self.stack.put(functions.int_to_bytes(5))
+        functions.OP_MULT_INTS(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        item = self.stack.get()
+        assert self.stack.empty()
         assert not self.cache
         assert functions.bytes_to_int(item) == -60
 
-    def test_OP_DIV_INT_pulls_int_from_queue_reads_signed_int_from_tape_and_puts_quotient_on_queue(self):
+    def test_OP_DIV_INT_pulls_int_from_stack_reads_signed_int_from_tape_and_puts_quotient_on_stack(self):
         self.tape = classes.Tape(functions.int_to_bytes(1) + functions.int_to_bytes(-2))
-        assert self.queue.empty()
-        self.queue.put(functions.int_to_bytes(-60))
-        functions.OP_DIV_INT(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        item = self.queue.get(False)
-        assert self.queue.empty()
+        assert self.stack.empty()
+        self.stack.put(functions.int_to_bytes(-60))
+        functions.OP_DIV_INT(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        item = self.stack.get()
+        assert self.stack.empty()
         assert not self.cache
         assert functions.bytes_to_int(item) == 30
 
-    def test_OP_DIV_INTS_pulls_two_ints_from_queue_and_puts_quotient_on_queue(self):
-        assert self.queue.empty()
-        self.queue.put(functions.int_to_bytes(12))
-        self.queue.put(functions.int_to_bytes(-132))
-        functions.OP_DIV_INTS(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        item = self.queue.get(False)
-        assert self.queue.empty()
+    def test_OP_DIV_INTS_pulls_two_ints_from_stack_and_puts_quotient_on_stack(self):
+        assert self.stack.empty()
+        divisor = 12
+        dividend = -132
+        self.stack.put(functions.int_to_bytes(divisor))
+        self.stack.put(functions.int_to_bytes(dividend))
+        functions.OP_DIV_INTS(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        item = self.stack.get()
+        assert self.stack.empty()
         assert not self.cache
-        assert functions.bytes_to_int(item) == -11
+        assert functions.bytes_to_int(item) == dividend / divisor
 
-    def test_OP_MOD_INT_reads_uint_from_tape_pulls_int_from_queue_and_puts_modulus_on_queue(self):
-        assert self.queue.empty()
-        self.tape = classes.Tape(functions.int_to_bytes(1) + functions.int_to_bytes(17))
-        self.queue.put(functions.int_to_bytes(1258))
-        functions.OP_MOD_INT(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        item = self.queue.get(False)
-        assert self.queue.empty()
+    def test_OP_MOD_INT_reads_uint_from_tape_pulls_int_from_stack_and_puts_modulus_on_stack(self):
+        assert self.stack.empty()
+        self.tape = classes.Tape(functions.uint_to_bytes(1) + functions.int_to_bytes(17))
+        self.stack.put(functions.int_to_bytes(1258))
+        functions.OP_MOD_INT(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        item = self.stack.get()
+        assert self.stack.empty()
         assert not self.cache
         assert functions.bytes_to_int(item) == (1258%17)
 
-    def test_OP_MOD_INT_pulls_two_ints_from_queue_and_puts_modulus_on_queue(self):
-        assert self.queue.empty()
-        self.queue.put(functions.int_to_bytes(17))
-        self.queue.put(functions.int_to_bytes(1258))
-        functions.OP_MOD_INTS(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        item = self.queue.get(False)
-        assert self.queue.empty()
+    def test_OP_MOD_INTS_pulls_two_ints_from_stack_and_puts_modulus_on_stack(self):
+        assert self.stack.empty()
+        dividend = 1258
+        divisor = 17
+        self.stack.put(functions.int_to_bytes(divisor))
+        self.stack.put(functions.int_to_bytes(dividend))
+        functions.OP_MOD_INTS(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        item = self.stack.get()
+        assert self.stack.empty()
         assert not self.cache
-        assert functions.bytes_to_int(item) == (1258%17)
+        assert functions.bytes_to_int(item) == (dividend%divisor)
 
-    def test_OP_ADD_FLOATS_reads_uint_from_tape_pulls_that_many_floats_from_queue_put_sum_on_queue(self):
-        assert self.queue.empty()
+    def test_OP_ADD_FLOATS_reads_uint_from_tape_pulls_that_many_floats_from_stack_put_sum_on_stack(self):
+        assert self.stack.empty()
         self.tape = classes.Tape(functions.int_to_bytes(3))
-        self.queue.put(functions.float_to_bytes(0.01))
-        self.queue.put(functions.float_to_bytes(0.1))
-        self.queue.put(functions.float_to_bytes(1.0))
-
-        expected = functions.bytes_to_float(functions.float_to_bytes(0.01))
-        expected += functions.bytes_to_float(functions.float_to_bytes(0.1))
-        expected += functions.bytes_to_float(functions.float_to_bytes(1.0))
+        floats = [
+            functions.float_to_bytes(0.01),
+            functions.float_to_bytes(0.1),
+            functions.float_to_bytes(1.0)
+        ]
+        self.stack.put(floats[0])
+        self.stack.put(floats[1])
+        self.stack.put(floats[2])
+
+        expected = functions.bytes_to_float(floats[0])
+        expected += functions.bytes_to_float(floats[1])
+        expected += functions.bytes_to_float(floats[2])
 
-        functions.OP_ADD_FLOATS(self.tape, self.queue, self.cache)
+        functions.OP_ADD_FLOATS(self.tape, self.stack, self.cache)
         assert not self.cache
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+        assert not self.stack.empty()
+        item = self.stack.get()
         item = functions.bytes_to_float(item)
-        assert self.queue.empty()
+        assert self.stack.empty()
         assert str(item)[:5] == str(expected)[:5]
 
     def test_OP_ADD_FLOATS_raises_errors_for_invalid_floats(self):
         self.tape = classes.Tape(functions.int_to_bytes(2))
-        assert self.queue.empty()
-        self.queue.put(functions.float_to_bytes(0.01)+b'000')
-        self.queue.put(functions.float_to_bytes(0.1))
+        assert self.stack.empty()
+        self.stack.put(functions.float_to_bytes(0.01)+b'000')
+        self.stack.put(functions.float_to_bytes(0.1))
         with self.assertRaises(TypeError) as e:
-            functions.OP_ADD_FLOATS(self.tape, self.queue, self.cache)
+            functions.OP_ADD_FLOATS(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_ADD_FLOATS malformed float'
 
         self.tape = classes.Tape(functions.int_to_bytes(2))
-        self.queue.put(functions.float_to_bytes(float('NaN')))
-        self.queue.put(functions.float_to_bytes(0.1))
+        self.stack.put(functions.float_to_bytes(float('NaN')))
+        self.stack.put(functions.float_to_bytes(0.1))
         with self.assertRaises(ValueError) as e:
-            functions.OP_ADD_FLOATS(self.tape, self.queue, self.cache)
+            functions.OP_ADD_FLOATS(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_ADD_FLOATS nan encountered'
 
-    def test_OP_SUBTRACT_FLOATS_reads_uint_from_tape_pulls_that_many_floats_from_queue_put_difference_on_queue(self):
-        assert self.queue.empty()
+    def test_OP_SUBTRACT_FLOATS_reads_uint_from_tape_pulls_that_many_floats_from_stack_put_difference_on_stack(self):
+        assert self.stack.empty()
+        minuend = functions.float_to_bytes(1.0)
+        subtrahend1 = functions.float_to_bytes(0.01)
+        subtrahend2 = functions.float_to_bytes(0.1)
         self.tape = classes.Tape(functions.int_to_bytes(3))
-        self.queue.put(functions.float_to_bytes(0.01))
-        self.queue.put(functions.float_to_bytes(0.1))
-        self.queue.put(functions.float_to_bytes(1.0))
-
-        expected = functions.bytes_to_float(functions.float_to_bytes(1.0))
-        expected -= functions.bytes_to_float(functions.float_to_bytes(0.01))
-        expected -= functions.bytes_to_float(functions.float_to_bytes(0.1))
+        self.stack.put(subtrahend1)
+        self.stack.put(subtrahend2)
+        self.stack.put(minuend)
+
+        expected = functions.bytes_to_float(minuend)
+        expected -= functions.bytes_to_float(subtrahend1)
+        expected -= functions.bytes_to_float(subtrahend2)
 
-        functions.OP_SUBTRACT_FLOATS(self.tape, self.queue, self.cache)
+        functions.OP_SUBTRACT_FLOATS(self.tape, self.stack, self.cache)
         assert not self.cache
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+        assert not self.stack.empty()
+        item = self.stack.get()
         item = functions.bytes_to_float(item)
-        assert self.queue.empty()
+        assert self.stack.empty()
         assert str(item)[:5] == str(expected)[:5]
 
     def test_OP_SUBTRACT_FLOATS_raises_errors_for_invalid_floats(self):
         self.tape = classes.Tape(functions.int_to_bytes(2))
-        self.queue.put(functions.float_to_bytes(0.01)+b'000')
-        self.queue.put(functions.float_to_bytes(0.1))
+        self.stack.put(functions.float_to_bytes(0.01)+b'000')
+        self.stack.put(functions.float_to_bytes(0.1))
         with self.assertRaises(TypeError) as e:
-            functions.OP_SUBTRACT_FLOATS(self.tape, self.queue, self.cache)
+            functions.OP_SUBTRACT_FLOATS(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_SUBTRACT_FLOATS malformed float'
 
         self.tape = classes.Tape(functions.int_to_bytes(2))
-        self.queue.put(functions.float_to_bytes(float('NaN')))
-        self.queue.put(functions.float_to_bytes(0.1))
+        self.stack.put(functions.float_to_bytes(float('NaN')))
+        self.stack.put(functions.float_to_bytes(0.1))
         with self.assertRaises(ValueError) as e:
-            functions.OP_SUBTRACT_FLOATS(self.tape, self.queue, self.cache)
+            functions.OP_SUBTRACT_FLOATS(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_SUBTRACT_FLOATS nan encountered'
 
-    def test_OP_DIV_FLOAT_reads_float_from_tape_pulls_float_from_queue_put_quotient_on_queue(self):
-        assert self.queue.empty()
-        self.tape = classes.Tape(functions.float_to_bytes(0.01))
-        self.queue.put(functions.float_to_bytes(0.1))
+    def test_OP_DIV_FLOAT_reads_float_from_tape_pulls_float_from_stack_put_quotient_on_stack(self):
+        assert self.stack.empty()
+        dividend = functions.float_to_bytes(0.1)
+        divisor = functions.float_to_bytes(0.01)
+        self.tape = classes.Tape(divisor)
+        self.stack.put(dividend)
 
-        expected = functions.bytes_to_float(functions.float_to_bytes(0.1))
-        expected /= functions.bytes_to_float(functions.float_to_bytes(0.01))
+        expected = functions.bytes_to_float(dividend)
+        expected /= functions.bytes_to_float(divisor)
 
-        functions.OP_DIV_FLOAT(self.tape, self.queue, self.cache)
+        functions.OP_DIV_FLOAT(self.tape, self.stack, self.cache)
         assert not self.cache
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+        assert not self.stack.empty()
+        item = self.stack.get()
         item = functions.bytes_to_float(item)
-        assert self.queue.empty()
-        assert (item-expected)/expected < 0.000001
+        assert self.stack.empty()
+        error_ratio = abs(item-expected)/expected
+        assert error_ratio < 0.000001, f'error ratio: {error_ratio}'
 
     def test_OP_DIV_FLOAT_raises_errors_for_invalid_float(self):
         self.tape = classes.Tape(functions.float_to_bytes(0.01))
-        self.queue.put(functions.float_to_bytes(0.1) + b'xx')
+        self.stack.put(functions.float_to_bytes(0.1) + b'xx')
         with self.assertRaises(TypeError) as e:
-            functions.OP_DIV_FLOAT(self.tape, self.queue, self.cache)
+            functions.OP_DIV_FLOAT(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_DIV_FLOAT malformed float'
 
         self.tape = classes.Tape(functions.float_to_bytes(float('NaN')))
-        self.queue.put(functions.float_to_bytes(0.1))
+        self.stack.put(functions.float_to_bytes(0.1))
         with self.assertRaises(ValueError) as e:
-            functions.OP_DIV_FLOAT(self.tape, self.queue, self.cache)
+            functions.OP_DIV_FLOAT(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_DIV_FLOAT nan encountered'
 
-    def test_OP_DIV_FLOATS_pulls_two_floats_from_queue_put_quotient_on_queue(self):
-        assert self.queue.empty()
-        self.queue.put(functions.float_to_bytes(0.01))
-        self.queue.put(functions.float_to_bytes(0.1))
+    def test_OP_DIV_FLOATS_pulls_two_floats_from_stack_put_quotient_on_stack(self):
+        assert self.stack.empty()
+        dividend = functions.float_to_bytes(0.1)
+        divisor = functions.float_to_bytes(0.01)
+        self.stack.put(divisor)
+        self.stack.put(dividend)
 
-        expected = functions.bytes_to_float(functions.float_to_bytes(0.1))
-        expected /= functions.bytes_to_float(functions.float_to_bytes(0.01))
+        expected = functions.bytes_to_float(dividend)
+        expected /= functions.bytes_to_float(divisor)
 
-        functions.OP_DIV_FLOATS(self.tape, self.queue, self.cache)
+        functions.OP_DIV_FLOATS(self.tape, self.stack, self.cache)
         assert not self.cache
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+        assert not self.stack.empty()
+        item = self.stack.get()
         item = functions.bytes_to_float(item)
-        assert self.queue.empty()
-        assert (item-expected)/expected < 0.000001
+        assert self.stack.empty()
+        # assert item == expected
+        error_ratio = abs(item-expected)/expected
+        assert error_ratio < 0.000001, f'error ratio: {error_ratio}'
 
     def test_OP_DIV_FLOATS_raises_errors_for_invalid_floats(self):
-        self.queue.put(functions.float_to_bytes(0.01)+b'1212')
+        self.stack.put(functions.float_to_bytes(0.01)+b'1212')
         with self.assertRaises(TypeError) as e:
-            functions.OP_DIV_FLOATS(self.tape, self.queue, self.cache)
+            functions.OP_DIV_FLOATS(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_DIV_FLOATS malformed float'
 
-        self.queue.put(functions.float_to_bytes(0.1))
-        self.queue.put(functions.float_to_bytes(0.01)+b'1212')
+        self.stack.put(functions.float_to_bytes(0.1))
+        self.stack.put(functions.float_to_bytes(0.01)+b'1212')
         with self.assertRaises(TypeError) as e:
-            functions.OP_DIV_FLOATS(self.tape, self.queue, self.cache)
+            functions.OP_DIV_FLOATS(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_DIV_FLOATS malformed float'
 
-        self.queue.put(functions.float_to_bytes(float('NaN')))
-        self.queue.put(functions.float_to_bytes(0.1))
+        self.stack.put(functions.float_to_bytes(float('NaN')))
+        self.stack.put(functions.float_to_bytes(0.1))
         with self.assertRaises(ValueError) as e:
-            functions.OP_DIV_FLOATS(self.tape, self.queue, self.cache)
+            functions.OP_DIV_FLOATS(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_DIV_FLOATS nan encountered'
 
-    def test_OP_MOD_FLOAT_reads_float_from_tape_pulls_float_from_queue_put_modulus_on_queue(self):
-        assert self.queue.empty()
-        self.tape = classes.Tape(functions.float_to_bytes(13.0))
-        self.queue.put(functions.float_to_bytes(131.1))
+    def test_OP_MOD_FLOAT_reads_float_from_tape_pulls_float_from_stack_put_modulus_on_stack(self):
+        assert self.stack.empty()
+        divisor = functions.float_to_bytes(13.0)
+        dividend = functions.float_to_bytes(131.1)
+        self.tape = classes.Tape(divisor)
+        self.stack.put(dividend)
 
-        expected = functions.bytes_to_float(functions.float_to_bytes(131.1))
-        expected = expected % functions.bytes_to_float(functions.float_to_bytes(13.0))
+        expected = functions.bytes_to_float(dividend)
+        expected = expected % functions.bytes_to_float(divisor)
 
-        functions.OP_MOD_FLOAT(self.tape, self.queue, self.cache)
+        functions.OP_MOD_FLOAT(self.tape, self.stack, self.cache)
         assert not self.cache
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+        assert not self.stack.empty()
+        item = self.stack.get()
         item = functions.bytes_to_float(item)
-        assert self.queue.empty()
-        assert (item-expected)/expected < 0.000001
+        assert self.stack.empty()
+        assert item == expected
+        # assert abs(item-expected)/expected < 0.000001
 
     def test_OP_MOD_FLOAT_raises_errors_for_invalid_floats(self):
         self.tape = classes.Tape(functions.float_to_bytes(1.1))
-        self.queue.put(functions.float_to_bytes(0.1) + b'12')
+        self.stack.put(functions.float_to_bytes(0.1) + b'12')
         with self.assertRaises(TypeError) as e:
-            functions.OP_MOD_FLOAT(self.tape, self.queue, self.cache)
+            functions.OP_MOD_FLOAT(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_MOD_FLOAT malformed float'
 
         self.tape = classes.Tape(functions.float_to_bytes(float('NaN')))
-        self.queue.put(functions.float_to_bytes(0.1))
+        self.stack.put(functions.float_to_bytes(0.1))
         with self.assertRaises(ValueError) as e:
-            functions.OP_MOD_FLOAT(self.tape, self.queue, self.cache)
+            functions.OP_MOD_FLOAT(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_MOD_FLOAT nan encountered'
 
-    def test_OP_MOD_FLOATS_pulls_two_floats_from_queue_put_modulus_on_queue(self):
-        assert self.queue.empty()
-        self.queue.put(functions.float_to_bytes(131.1))
-        self.queue.put(functions.float_to_bytes(13.0))
+    def test_OP_MOD_FLOATS_pulls_two_floats_from_stack_put_modulus_on_stack(self):
+        assert self.stack.empty()
+        divisor = functions.float_to_bytes(13.0)
+        dividend = functions.float_to_bytes(131.1)
+        self.stack.put(divisor)
+        self.stack.put(dividend)
 
-        expected = functions.bytes_to_float(functions.float_to_bytes(131.1))
-        expected = expected % functions.bytes_to_float(functions.float_to_bytes(13.0))
+        expected = functions.bytes_to_float(divisor)
+        expected = expected % functions.bytes_to_float(dividend)
 
-        functions.OP_MOD_FLOATS(self.tape, self.queue, self.cache)
+        functions.OP_MOD_FLOATS(self.tape, self.stack, self.cache)
         assert not self.cache
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+        assert not self.stack.empty()
+        item = self.stack.get()
         item = functions.bytes_to_float(item)
-        assert self.queue.empty()
-        assert (item-expected)/expected < 0.000001
+        assert self.stack.empty()
+        assert item == expected
+        # assert abs(item-expected)/expected < 0.000001
 
     def test_OP_MOD_FLOATS_raises_errors_for_invalid_floats(self):
-        self.queue.put(functions.float_to_bytes(0.1) + b'x')
+        self.stack.put(functions.float_to_bytes(0.1) + b'x')
         with self.assertRaises(TypeError) as e:
-            functions.OP_MOD_FLOATS(self.tape, self.queue, self.cache)
+            functions.OP_MOD_FLOATS(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_MOD_FLOATS malformed float'
 
-        self.queue.put(functions.float_to_bytes(0.1))
-        self.queue.put(functions.float_to_bytes(0.1) + b'x')
+        self.stack.put(functions.float_to_bytes(0.1))
+        self.stack.put(functions.float_to_bytes(0.1) + b'x')
         with self.assertRaises(TypeError) as e:
-            functions.OP_MOD_FLOATS(self.tape, self.queue, self.cache)
+            functions.OP_MOD_FLOATS(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_MOD_FLOATS malformed float'
 
-        self.queue.put(functions.float_to_bytes(0.1))
-        self.queue.put(functions.float_to_bytes(float('NaN')))
+        self.stack.put(functions.float_to_bytes(0.1))
+        self.stack.put(functions.float_to_bytes(float('NaN')))
         with self.assertRaises(ValueError) as e:
-            functions.OP_MOD_FLOATS(self.tape, self.queue, self.cache)
+            functions.OP_MOD_FLOATS(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_MOD_FLOATS nan encountered'
 
-    def test_OP_ADD_POINTS_reads_uint_from_tape_pulls_that_many_points_from_queue_puts_sum_on_queue(self):
-        assert self.queue.empty()
+    def test_OP_ADD_POINTS_reads_uint_from_tape_pulls_that_many_points_from_stack_puts_sum_on_stack(self):
+        assert self.stack.empty()
         self.tape = classes.Tape(functions.int_to_bytes(2))
         point1 = bytes(SigningKey(token_bytes(32)).verify_key)
         point2 = bytes(SigningKey(token_bytes(32)).verify_key)
         expected = nacl.bindings.crypto_core_ed25519_add(point1, point2)
-        self.queue.put(point1)
-        self.queue.put(point2)
-        functions.OP_ADD_POINTS(self.tape, self.queue, self.cache)
+        self.stack.put(point1)
+        self.stack.put(point2)
+        functions.OP_ADD_POINTS(self.tape, self.stack, self.cache)
         assert not self.cache
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+        assert not self.stack.empty()
+        item = self.stack.get()
         assert item == bytes(expected)
 
     def test_OP_ADD_POINTS_raises_errors_for_invalid_points(self):
         self.tape = classes.Tape(b'\x02')
-        self.queue.put(12323)
-        with self.assertRaises(TypeError) as e:
-            functions.OP_ADD_POINTS(self.tape, self.queue, self.cache)
-        assert str(e.exception) == 'OP_ADD_POINTS non-point value encountered'
-
-        self.tape = classes.Tape(b'\x02')
-        self.queue.put(b''.join([b'\xff' for _ in range(32)]))
-        self.queue.put(b''.join([b'\xff' for _ in range(32)]))
+        self.stack.put(b''.join([b'\xff' for _ in range(32)]))
+        self.stack.put(b''.join([b'\xff' for _ in range(32)]))
         with self.assertRaises(ValueError) as e:
-            functions.OP_ADD_POINTS(self.tape, self.queue, self.cache)
+            functions.OP_ADD_POINTS(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_ADD_POINTS invalid point encountered'
 
-    def test_OP_COPY_reads_uint_from_tape_and_copies_top_queue_value_that_many_times(self):
-        assert self.queue.empty()
+    def test_OP_COPY_reads_uint_from_tape_and_copies_top_stack_value_that_many_times(self):
+        assert self.stack.empty()
         n_copies = randint(1, 255)
-        self.queue.put(b'1')
+        self.stack.put(b'1')
         self.tape = classes.Tape(n_copies.to_bytes(1, 'big'))
-        functions.OP_COPY(self.tape, self.queue, self.cache)
+        functions.OP_COPY(self.tape, self.stack, self.cache)
         expected = n_copies + 1
         observed = 0
-        while not self.queue.empty():
+        while not self.stack.empty():
             observed += 1
-            assert self.queue.get(False) == b'1'
+            assert self.stack.get() == b'1'
         assert observed == expected
 
-    def test_OP_DUP_duplicates_top_queue_item(self):
-        assert self.queue.empty()
-        self.queue.put(b'1')
-        functions.OP_DUP(self.tape, self.queue, self.cache)
-        assert self.queue.get(False) == b'1'
-        assert self.queue.get(False) == b'1'
-        assert self.queue.empty()
+    def test_OP_DUP_duplicates_top_stack_item(self):
+        assert self.stack.empty()
+        self.stack.put(b'1')
+        functions.OP_DUP(self.tape, self.stack, self.cache)
+        assert self.stack.get() == b'1'
+        assert self.stack.get() == b'1'
+        assert self.stack.empty()
 
-    def test_OP_SHA256_pulls_value_from_queue_and_puts_its_sha256_on_queue(self):
-        assert self.queue.empty()
+    def test_OP_SHA256_pulls_value_from_stack_and_puts_its_sha256_on_stack(self):
+        assert self.stack.empty()
         preimage = b'123232'
-        self.queue.put(preimage)
-        functions.OP_SHA256(self.tape, self.queue, self.cache)
+        self.stack.put(preimage)
+        functions.OP_SHA256(self.tape, self.stack, self.cache)
         expected = sha256(preimage).digest()
-        assert self.queue.get(False) == expected
-        assert self.queue.empty()
+        assert self.stack.get() == expected
+        assert self.stack.empty()
 
-    def test_OP_SHAKE256_reads_uint_from_tape_pulls_value_from_queue_and_puts_its_shake256_on_queue(self):
-        assert self.queue.empty()
+    def test_OP_SHAKE256_reads_uint_from_tape_pulls_value_from_stack_and_puts_its_shake256_on_stack(self):
+        assert self.stack.empty()
         self.tape = classes.Tape((20).to_bytes(1, 'big'))
         preimage = b'123232'
-        self.queue.put(preimage)
-        functions.OP_SHAKE256(self.tape, self.queue, self.cache)
+        self.stack.put(preimage)
+        functions.OP_SHAKE256(self.tape, self.stack, self.cache)
         expected = shake_256(preimage).digest(20)
-        assert self.queue.get(False) == expected
-        assert self.queue.empty()
+        assert self.stack.get() == expected
+        assert self.stack.empty()
 
-    def test_OP_VERIFY_raises_error_only_if_top_queue_item_is_not_true(self):
-        self.queue.put(b'\x00')
+    def test_OP_VERIFY_raises_error_only_if_top_stack_item_is_not_true(self):
+        self.stack.put(b'\x00')
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_VERIFY(self.tape, self.queue, self.cache)
+            functions.OP_VERIFY(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_VERIFY check failed'
 
-        self.queue.put(b'\x01')
-        functions.OP_VERIFY(self.tape, self.queue, self.cache)
-        self.queue.put(b'12323')
-        functions.OP_VERIFY(self.tape, self.queue, self.cache)
-
-    def test_OP_EQUAL_compares_two_values_from_queue_and_puts_bool_on_queue(self):
-        self.queue.put(b'123')
-        self.queue.put(b'123')
-        functions.OP_EQUAL(self.tape, self.queue, self.cache)
-        assert self.queue.get(False) == b'\xff'
-
-        self.queue.put(b'321')
-        self.queue.put(b'123')
-        functions.OP_EQUAL(self.tape, self.queue, self.cache)
-        assert self.queue.get(False) == b'\x00'
+        self.stack.put(b'\x01')
+        functions.OP_VERIFY(self.tape, self.stack, self.cache)
+        self.stack.put(b'12323')
+        functions.OP_VERIFY(self.tape, self.stack, self.cache)
+
+    def test_OP_EQUAL_compares_two_values_from_stack_and_puts_bool_on_stack(self):
+        self.stack.put(b'123')
+        self.stack.put(b'123')
+        functions.OP_EQUAL(self.tape, self.stack, self.cache)
+        assert self.stack.get() == b'\xff'
+
+        self.stack.put(b'321')
+        self.stack.put(b'123')
+        functions.OP_EQUAL(self.tape, self.stack, self.cache)
+        assert self.stack.get() == b'\x00'
 
     def test_OP_EQUAL_VERIFY_runs_OP_EQUAL_then_OP_VERIFY(self):
-        assert self.queue.empty()
-        self.queue.put(b'123')
-        self.queue.put(b'123')
-        functions.OP_EQUAL_VERIFY(self.tape, self.queue, self.cache)
-        assert self.queue.empty()
+        assert self.stack.empty()
+        self.stack.put(b'123')
+        self.stack.put(b'123')
+        functions.OP_EQUAL_VERIFY(self.tape, self.stack, self.cache)
+        assert self.stack.empty()
 
-        self.queue.put(b'321')
-        self.queue.put(b'123')
+        self.stack.put(b'321')
+        self.stack.put(b'123')
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_EQUAL_VERIFY(self.tape, self.queue, self.cache)
+            functions.OP_EQUAL_VERIFY(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_VERIFY check failed'
-        assert self.queue.empty()
+        assert self.stack.empty()
 
-    def test_OP_CHECK_SIG_pulls_VerifyKey_and_signature_from_queue_and_checks_against_cache(self):
+    def test_OP_CHECK_SIG_pulls_VerifyKey_and_signature_from_stack_and_checks_against_cache(self):
         body = b'hello world'
         skey = SigningKey(token_bytes(32))
         vkey = skey.verify_key
         smsg = skey.sign(body)
         sig = smsg[:64]
         self.tape = classes.Tape(b'\x00')
-        assert self.queue.empty()
-        self.queue.put(sig)
-        self.queue.put(bytes(vkey))
+        assert self.stack.empty()
+        self.stack.put(sig)
+        self.stack.put(bytes(vkey))
         self.cache['sigfield1'] = body
-        functions.OP_CHECK_SIG(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        assert self.queue.get(False) == b'\xff'
-        assert self.queue.empty()
+        functions.OP_CHECK_SIG(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        assert self.stack.get() == b'\xff'
+        assert self.stack.empty()
 
     def test_OP_CHECK_SIG_sigflag_omits_sigfields(self):
         field1 = b'hello'
         field3 = b' '
         field8 = b'world'
         body = field1 + field3 + field8
         sigflag = 0b00000001 | 0b00000100 | 0b10000000
         sigflag = (~sigflag) & 255
         self.tape = classes.Tape(sigflag.to_bytes(1, 'big'))
         skey = SigningKey(token_bytes(32))
         vkey = skey.verify_key
         smsg = skey.sign(body)
         sig = smsg[:64] + sigflag.to_bytes(1, 'big')
-        assert self.queue.empty()
-        self.queue.put(sig)
-        self.queue.put(bytes(vkey))
+        assert self.stack.empty()
+        self.stack.put(sig)
+        self.stack.put(bytes(vkey))
         self.cache['sigfield1'] = field1
         self.cache['sigfield2'] = b'should be ignored'
         self.cache['sigfield3'] = field3
         self.cache['sigfield4'] = b'should be ignored'
         self.cache['sigfield5'] = b'should be ignored'
         self.cache['sigfield6'] = b'should be ignored'
         self.cache['sigfield7'] = b'should be ignored'
         self.cache['sigfield8'] = field8
-        functions.OP_CHECK_SIG(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        assert self.queue.get(False) == b'\xff'
-        assert self.queue.empty()
+        functions.OP_CHECK_SIG(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        assert self.stack.get() == b'\xff'
+        assert self.stack.empty()
 
     def test_OP_CHECK_SIG_errors_on_invalid_vkey_or_sig(self):
         self.tape = classes.Tape(b'\x00')
-        self.queue.put(b''.join(b'\xff' for _ in range(64)))
-        self.queue.put(b'not a valid vkey')
+        self.stack.put(b''.join(b'\xff' for _ in range(64)))
+        self.stack.put(b'not a valid vkey')
         with self.assertRaises(ValueError) as e:
-            functions.OP_CHECK_SIG(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_SIG(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_CHECK_SIG invalid vkey encountered'
 
         self.tape = classes.Tape(b'\x00')
-        self.queue.put(b'not a valid sig')
-        self.queue.put(b''.join(b'\xff' for _ in range(32)))
+        self.stack.put(b'not a valid sig')
+        self.stack.put(b''.join(b'\xff' for _ in range(32)))
         with self.assertRaises(ValueError) as e:
-            functions.OP_CHECK_SIG(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_SIG(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_CHECK_SIG invalid sig encountered'
 
     def test_OP_CHECK_SIG_errors_on_disallowed_sigflag(self):
         field1 = b'hello'
         body = field1
         allowed_sigflags = 0b00000100 | 0b10000000
         allowed_sigflags = (~allowed_sigflags) & 255
         self.tape = classes.Tape(allowed_sigflags.to_bytes(1, 'big'))
         attempted_sigflags = 0b10000000
         attempted_sigflags = (~attempted_sigflags) & 255
         skey = SigningKey(token_bytes(32))
         vkey = skey.verify_key
         smsg = skey.sign(body)
         sig = smsg[:64] + attempted_sigflags.to_bytes(1, 'big')
-        assert self.queue.empty()
-        self.queue.put(sig)
-        self.queue.put(bytes(vkey))
+        assert self.stack.empty()
+        self.stack.put(sig)
+        self.stack.put(bytes(vkey))
 
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_SIG(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_SIG(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'disallowed sigflag'
-        assert self.queue.empty()
+        assert self.stack.empty()
 
     def test_OP_CHECK_SIG_VERIFY_runs_OP_CHECK_SIG_then_OP_VERIFY(self):
         body = b'hello world'
         skey = SigningKey(token_bytes(32))
         vkey = skey.verify_key
         smsg = skey.sign(body)
         sig = smsg[:64]
         self.tape = classes.Tape(b'\x00')
-        assert self.queue.empty()
-        self.queue.put(sig)
-        self.queue.put(bytes(vkey))
+        assert self.stack.empty()
+        self.stack.put(sig)
+        self.stack.put(bytes(vkey))
         self.cache['sigfield1'] = body
-        functions.OP_CHECK_SIG_VERIFY(self.tape, self.queue, self.cache)
-        assert self.queue.empty()
+        functions.OP_CHECK_SIG_VERIFY(self.tape, self.stack, self.cache)
+        assert self.stack.empty()
 
         sig = smsg[:64]
         self.tape = classes.Tape(b'\x00')
-        assert self.queue.empty()
-        self.queue.put(sig)
-        self.queue.put(bytes(vkey))
+        assert self.stack.empty()
+        self.stack.put(sig)
+        self.stack.put(bytes(vkey))
         self.cache['sigfield1'] = b'not body'
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_SIG_VERIFY(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_SIG_VERIFY(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_VERIFY check failed'
-        assert self.queue.empty()
+        assert self.stack.empty()
 
     def test_OP_CHECK_TIMESTAMP_raises_error_for_invalid_constraint(self):
-        assert self.queue.empty()
-        self.queue.put(b'')
+        assert self.stack.empty()
+        self.stack.put(b'')
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_TIMESTAMP(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_TIMESTAMP(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_CHECK_TIMESTAMP malformed constraint encountered'
 
     def test_OP_CHECKTIMESTAMP_raises_errors_for_invalid_cache_timestamp(self):
-        assert self.queue.empty()
-        self.queue.put(b'xxxx')
+        assert self.stack.empty()
+        self.stack.put(b'xxxx')
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_TIMESTAMP(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_TIMESTAMP(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_CHECK_TIMESTAMP cache missing timestamp'
 
-        assert self.queue.empty()
-        self.queue.put(b'xxxx')
+        assert self.stack.empty()
+        self.stack.put(b'xxxx')
         self.cache['timestamp'] = 'not an int'
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_TIMESTAMP(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_TIMESTAMP(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_CHECK_TIMESTAMP malformed cache timestamp'
 
     def test_OP_CHECKTIMESTAMP_raises_errors_for_invalid_ts_threshold_tape_flag(self):
-        assert self.queue.empty()
-        self.queue.put(b'xxxx')
+        assert self.stack.empty()
+        self.stack.put(b'xxxx')
         self.cache['timestamp'] = 3
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_TIMESTAMP(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_TIMESTAMP(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_CHECK_TIMESTAMP missing ts_threshold flag'
 
-        assert self.queue.empty()
-        self.queue.put(b'xxxx')
+        assert self.stack.empty()
+        self.stack.put(b'xxxx')
         self.cache['timestamp'] = 3
         self.tape.flags['ts_threshold'] = 'not an int'
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_TIMESTAMP(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_TIMESTAMP(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_CHECK_TIMESTAMP malformed ts_threshold flag'
 
-    def test_OP_CHECK_TIMESTAMP_compares_top_queue_int_to_cache_timestamp(self):
-        assert self.queue.empty()
+    def test_OP_CHECK_TIMESTAMP_compares_top_stack_int_to_cache_timestamp(self):
+        assert self.stack.empty()
         self.tape.flags['ts_threshold'] = 10
         self.cache['timestamp'] = int(time())
-        self.queue.put(int(time()).to_bytes(4, 'big'))
-        functions.OP_CHECK_TIMESTAMP(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        assert self.queue.get(False) == b'\xff'
+        self.stack.put(int(time()).to_bytes(4, 'big'))
+        functions.OP_CHECK_TIMESTAMP(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        assert self.stack.get() == b'\xff'
 
-        assert self.queue.empty()
+        assert self.stack.empty()
         self.cache['timestamp'] = int(time())-1
-        self.queue.put(int(time()).to_bytes(4, 'big'))
-        functions.OP_CHECK_TIMESTAMP(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+        self.stack.put(int(time()).to_bytes(4, 'big'))
+        functions.OP_CHECK_TIMESTAMP(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        item = self.stack.get()
         assert item == b'\x00'
 
-        assert self.queue.empty()
+        assert self.stack.empty()
         self.cache['timestamp'] = int(time())+12
-        self.queue.put(int(time()).to_bytes(4, 'big'))
-        functions.OP_CHECK_TIMESTAMP(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+        self.stack.put(int(time()).to_bytes(4, 'big'))
+        functions.OP_CHECK_TIMESTAMP(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        item = self.stack.get()
         assert item == b'\x00'
 
-        assert self.queue.empty()
+        assert self.stack.empty()
         self.tape.flags['ts_threshold'] = 100
         self.cache['timestamp'] = int(time())+12
-        self.queue.put(int(time()).to_bytes(4, 'big'))
-        functions.OP_CHECK_TIMESTAMP(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+        self.stack.put(int(time()).to_bytes(4, 'big'))
+        functions.OP_CHECK_TIMESTAMP(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        item = self.stack.get()
         assert item == b'\xff'
 
     def test_OP_CHECK_TIMESTAMP_VERIFY_runs_OP_CHECK_TIMESTAMP_then_OP_VERIFY(self):
-        assert self.queue.empty()
+        assert self.stack.empty()
         self.tape = classes.Tape(b'', flags={'ts_threshold': 10})
         self.cache['timestamp'] = int(time())
-        self.queue.put(int(time()).to_bytes(4, 'big'))
-        functions.OP_CHECK_TIMESTAMP_VERIFY(self.tape, self.queue, self.cache)
-        assert self.queue.empty()
+        self.stack.put(int(time()).to_bytes(4, 'big'))
+        functions.OP_CHECK_TIMESTAMP_VERIFY(self.tape, self.stack, self.cache)
+        assert self.stack.empty()
 
-        assert self.queue.empty()
+        assert self.stack.empty()
         self.cache['timestamp'] = int(time())-1
-        self.queue.put(int(time()).to_bytes(4, 'big'))
+        self.stack.put(int(time()).to_bytes(4, 'big'))
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_TIMESTAMP_VERIFY(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_TIMESTAMP_VERIFY(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_VERIFY check failed'
-        assert self.queue.empty()
+        assert self.stack.empty()
 
-        assert self.queue.empty()
+        assert self.stack.empty()
         self.cache['timestamp'] = int(time())+12
-        self.queue.put(int(time()).to_bytes(4, 'big'))
+        self.stack.put(int(time()).to_bytes(4, 'big'))
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_TIMESTAMP_VERIFY(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_TIMESTAMP_VERIFY(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_VERIFY check failed'
-        assert self.queue.empty()
+        assert self.stack.empty()
 
     def test_OP_CHECK_EPOCH_raises_error_for_invalid_constraint(self):
-        assert self.queue.empty()
-        self.queue.put(b'')
+        assert self.stack.empty()
+        self.stack.put(b'')
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_EPOCH(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_EPOCH(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_CHECK_EPOCH malformed constraint encountered'
 
     def test_OP_CHECK_EPOCH_raises_errors_for_invalid_epoch_threshold_tape_flag(self):
-        assert self.queue.empty()
-        self.queue.put(b'x')
+        assert self.stack.empty()
+        self.stack.put(b'x')
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_EPOCH(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_EPOCH(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_CHECK_EPOCH missing epoch_threshold flag'
 
-        assert self.queue.empty()
-        self.queue.put(b'x')
+        assert self.stack.empty()
+        self.stack.put(b'x')
         self.tape.flags['epoch_threshold'] = 'not an int'
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_EPOCH(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_EPOCH(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_CHECK_EPOCH malformed epoch_threshold flag'
 
-        assert self.queue.empty()
-        self.queue.put(b'x')
+        assert self.stack.empty()
+        self.stack.put(b'x')
         self.tape.flags['epoch_threshold'] = -1
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_EPOCH(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_EPOCH(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_CHECK_EPOCH malformed epoch_threshold flag'
 
     def test_OP_CHCECK_EPOCH_compares_current_time_to_constraint(self):
-        assert self.queue.empty()
+        assert self.stack.empty()
         self.tape.flags['epoch_threshold'] = 0
-        self.queue.put(int(time()-10).to_bytes(4, 'big'))
-        functions.OP_CHECK_EPOCH(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        assert self.queue.get(False) == b'\xff'
-
-        assert self.queue.empty()
-        self.queue.put(int(time()+10).to_bytes(4, 'big'))
-        functions.OP_CHECK_EPOCH(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+        self.stack.put(int(time()-10).to_bytes(4, 'big'))
+        functions.OP_CHECK_EPOCH(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        assert self.stack.get() == b'\xff'
+
+        assert self.stack.empty()
+        self.stack.put(int(time()+10).to_bytes(4, 'big'))
+        functions.OP_CHECK_EPOCH(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        item = self.stack.get()
         assert item == b'\x00'
 
-        assert self.queue.empty()
+        assert self.stack.empty()
         self.tape.flags['epoch_threshold'] = 100
-        self.queue.put(int(time()+10).to_bytes(4, 'big'))
-        functions.OP_CHECK_EPOCH(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+        self.stack.put(int(time()+10).to_bytes(4, 'big'))
+        functions.OP_CHECK_EPOCH(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        item = self.stack.get()
         assert item == b'\xff'
 
     def test_OP_CHECK_EPOCH_VERIFY_runs_OP_CHECK_EPOCH_then_OP_VERIFY(self):
-        assert self.queue.empty()
+        assert self.stack.empty()
         self.tape.flags['epoch_threshold'] = 0
-        self.queue.put(int(time()-10).to_bytes(4, 'big'))
-        functions.OP_CHECK_EPOCH_VERIFY(self.tape, self.queue, self.cache)
-        assert self.queue.empty()
+        self.stack.put(int(time()-10).to_bytes(4, 'big'))
+        functions.OP_CHECK_EPOCH_VERIFY(self.tape, self.stack, self.cache)
+        assert self.stack.empty()
 
-        assert self.queue.empty()
-        self.queue.put(int(time()+10).to_bytes(4, 'big'))
+        assert self.stack.empty()
+        self.stack.put(int(time()+10).to_bytes(4, 'big'))
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_EPOCH_VERIFY(self.tape, self.queue, self.cache)
-        assert self.queue.empty()
+            functions.OP_CHECK_EPOCH_VERIFY(self.tape, self.stack, self.cache)
+        assert self.stack.empty()
 
-        assert self.queue.empty()
+        assert self.stack.empty()
         self.tape.flags['epoch_threshold'] = 100
-        self.queue.put(int(time()+10).to_bytes(4, 'big'))
-        functions.OP_CHECK_EPOCH_VERIFY(self.tape, self.queue, self.cache)
-        assert self.queue.empty()
+        self.stack.put(int(time()+10).to_bytes(4, 'big'))
+        functions.OP_CHECK_EPOCH_VERIFY(self.tape, self.stack, self.cache)
+        assert self.stack.empty()
 
     def test_OP_DEF_creates_subtape_definition(self):
-        assert self.queue.empty()
+        assert self.stack.empty()
         self.tape = classes.Tape(b'\x00\x00\x0bhello world')
         assert not self.tape.definitions
-        functions.OP_DEF(self.tape, self.queue, self.cache)
+        functions.OP_DEF(self.tape, self.stack, self.cache)
         assert b'\x00' in self.tape.definitions
         assert isinstance(self.tape.definitions[b'\x00'], classes.Tape)
         assert self.tape.definitions[b'\x00'].data == b'hello world'
-        assert self.queue.empty()
+        assert self.stack.empty()
 
-    def test_OP_NOT_inverts_bool_value_of_top_queue_value(self):
-        assert self.queue.empty()
-        self.queue.put(b'\xFF')
-        functions.OP_NOT(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        assert self.queue.get(False) == b'\x00'
-
-        assert self.queue.empty()
-        self.queue.put(b'\x00')
-        functions.OP_NOT(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        assert self.queue.get(False) == b'\xFF'
-        assert self.queue.empty()
-
-    def test_OP_NOT_inverts_bytestring_on_top_of_queue(self):
-        self.queue.put(b'\xf0\x0f')
-        functions.OP_NOT(self.tape, self.queue, self.cache)
-        assert self.queue.get(False) == b'\x0f\xf0'
+    def test_OP_NOT_inverts_bool_value_of_top_stack_value(self):
+        assert self.stack.empty()
+        self.stack.put(b'\xFF')
+        functions.OP_NOT(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        assert self.stack.get() == b'\x00'
+
+        assert self.stack.empty()
+        self.stack.put(b'\x00')
+        functions.OP_NOT(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        assert self.stack.get() == b'\xFF'
+        assert self.stack.empty()
+
+    def test_OP_NOT_inverts_bytestring_on_top_of_stack(self):
+        self.stack.put(b'\xf0\x0f')
+        functions.OP_NOT(self.tape, self.stack, self.cache)
+        assert self.stack.get() == b'\x0f\xf0'
 
         data = token_bytes(4)
-        self.queue.put(data)
-        functions.OP_DUP(self.tape, self.queue, self.cache)
-        functions.OP_NOT(self.tape, self.queue, self.cache)
-        functions.OP_XOR(self.tape, self.queue, self.cache)
-        assert self.queue.get(False) == b'\xff\xff\xff\xff'
+        self.stack.put(data)
+        functions.OP_DUP(self.tape, self.stack, self.cache)
+        functions.OP_NOT(self.tape, self.stack, self.cache)
+        functions.OP_XOR(self.tape, self.stack, self.cache)
+        assert self.stack.get() == b'\xff\xff\xff\xff'
 
-    def test_OP_RANDOM_puts_random_bytes_on_queue(self):
-        assert self.queue.empty()
+    def test_OP_RANDOM_puts_random_bytes_on_stack(self):
+        assert self.stack.empty()
         n_bytes = randint(1, 250)
-        self.tape = classes.Tape(n_bytes.to_bytes(1, 'big'))
-        functions.OP_RANDOM(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+        self.stack.put(functions.int_to_bytes(n_bytes))
+        self.tape = classes.Tape(b'')
+        functions.OP_RANDOM(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        item = self.stack.get()
         assert type(item) is bytes
         assert len(item) == n_bytes
-        assert self.queue.empty()
+        assert self.stack.empty()
 
     def test_OP_RETURN_advances_tape_pointer_to_end(self):
         self.tape = classes.Tape(b'asdkjhk123')
         assert self.tape.pointer == 0
-        functions.OP_RETURN(self.tape, self.queue, self.cache)
+        functions.OP_RETURN(self.tape, self.stack, self.cache)
         assert self.tape.pointer == len(self.tape.data)
         with self.assertRaises(errors.ScriptExecutionError) as e:
             self.tape.read(1)
 
     def test_OP_SET_FLAG_raises_error_for_unrecognized_flag(self):
         self.tape = classes.Tape(b'\x03abc')
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_SET_FLAG(self.tape, self.queue, self.cache)
+            functions.OP_SET_FLAG(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_SET_FLAG unrecognized flag'
 
     def test_OP_SET_FLAG_sets_tape_flag_to_default_value(self):
         original_flags = functions.flags
         functions.flags = {**original_flags, b'dummy_flag': 1}
         self.tape = classes.Tape(b'\x0adummy_flag')
         assert b'dummy_flag' not in self.tape.flags
-        functions.OP_SET_FLAG(self.tape, self.queue, self.cache)
+        functions.OP_SET_FLAG(self.tape, self.stack, self.cache)
         assert b'dummy_flag' in self.tape.flags
         functions.flags = original_flags
 
     def test_OP_UNSET_FLAG_unsets_tape_flag(self):
         self.tape = classes.Tape(b'\x0adummy_flag')
         self.tape.flags[b'dummy_flag'] = 1
         assert b'dummy_flag' in self.tape.flags
-        functions.OP_UNSET_FLAG(self.tape, self.queue, self.cache)
+        functions.OP_UNSET_FLAG(self.tape, self.stack, self.cache)
         assert b'dummy_flag' not in self.tape.flags
 
-    def test_OP_DEPTH_puts_queue_size_onto_queue(self):
-        assert self.queue.empty()
-        self.queue.put(b'123')
-        self.queue.put(b'321')
-        self.queue.put(b'asd')
-        functions.OP_DEPTH(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+    def test_OP_DEPTH_puts_stack_size_onto_stack(self):
+        assert self.stack.empty()
+        self.stack.put(b'123')
+        self.stack.put(b'321')
+        self.stack.put(b'asd')
+        functions.OP_DEPTH(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        item = self.stack.get()
         assert functions.bytes_to_int(item) == 3
         items = []
-        while not self.queue.empty():
-            items.append(self.queue.get(False))
+        while not self.stack.empty():
+            items.append(self.stack.get())
         assert items == [b'asd', b'321', b'123']
 
-    def test_OP_SWAP_swaps_order_of_queue_items_given_indices_from_tape(self):
-        assert self.queue.empty()
+    def test_OP_SWAP_swaps_order_of_stack_items_given_indices_from_tape(self):
+        assert self.stack.empty()
         self.tape = classes.Tape(b'\x00\x02')
-        self.queue.put(b'bottom')
-        self.queue.put(b'middle')
-        self.queue.put(b'top')
-        functions.OP_SWAP(self.tape, self.queue, self.cache)
+        self.stack.put(b'bottom')
+        self.stack.put(b'middle')
+        self.stack.put(b'top')
+        functions.OP_SWAP(self.tape, self.stack, self.cache)
         items = []
-        while not self.queue.empty():
-            items.append(self.queue.get(False))
+        while not self.stack.empty():
+            items.append(self.stack.get())
         assert items == [b'bottom', b'middle', b'top']
 
-        self.queue = LifoQueue()
+        self.stack = classes.Stack()
         self.tape = classes.Tape(b'\x00\x01')
-        self.queue.put(b'bottom')
-        self.queue.put(b'middle')
-        self.queue.put(b'top')
-        functions.OP_SWAP(self.tape, self.queue, self.cache)
+        self.stack.put(b'bottom')
+        self.stack.put(b'middle')
+        self.stack.put(b'top')
+        functions.OP_SWAP(self.tape, self.stack, self.cache)
         items = []
-        while not self.queue.empty():
-            items.append(self.queue.get(False))
+        while not self.stack.empty():
+            items.append(self.stack.get())
         assert items == [b'middle', b'top', b'bottom']
 
-    def test_OP_SWAP_raises_ScriptExecutionError_for_queue_depth_overflow(self):
-        self.queue.put(b'sds')
+    def test_OP_SWAP_raises_ScriptExecutionError_for_stack_depth_overflow(self):
+        self.stack.put(b'sds')
         self.tape = classes.Tape(b'\x00\xff')
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_SWAP(self.tape, self.queue, self.cache)
-        assert str(e.exception) == 'OP_SWAP queue size exceeded by index'
+            functions.OP_SWAP(self.tape, self.stack, self.cache)
+        assert str(e.exception) == 'OP_SWAP stack size exceeded by index'
 
         self.tape = classes.Tape(b'\xff\x00')
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_SWAP(self.tape, self.queue, self.cache)
-        assert str(e.exception) == 'OP_SWAP queue size exceeded by index'
+            functions.OP_SWAP(self.tape, self.stack, self.cache)
+        assert str(e.exception) == 'OP_SWAP stack size exceeded by index'
 
-    def test_OP_SWAP2_swaps_top_two_queue_items(self):
-        self.queue.put(b'second')
-        self.queue.put(b'first')
-        functions.OP_SWAP2(self.tape, self.queue, self.cache)
-        assert self.queue.get(False) == b'second'
-        assert self.queue.get(False) == b'first'
-
-    def test_OP_REVERSE_reads_uint_from_tape_and_reverses_order_of_that_many_queue_items(self):
-        assert self.queue.empty()
-        self.queue.put(4)
-        self.queue.put(3)
-        self.queue.put(2)
-        self.queue.put(1)
+    def test_OP_SWAP2_swaps_top_two_stack_items(self):
+        self.stack.put(b'second')
+        self.stack.put(b'first')
+        functions.OP_SWAP2(self.tape, self.stack, self.cache)
+        assert self.stack.get() == b'second'
+        assert self.stack.get() == b'first'
+
+    def test_OP_REVERSE_reads_uint_from_tape_and_reverses_order_of_that_many_stack_items(self):
+        assert self.stack.empty()
+        self.stack.put(b'4')
+        self.stack.put(b'3')
+        self.stack.put(b'2')
+        self.stack.put(b'1')
         self.tape = classes.Tape(b'\x03')
-        functions.OP_REVERSE(self.tape, self.queue, self.cache)
-        items = []
-        while not self.queue.empty():
-            items.append(self.queue.get(False))
-        assert items == [3,2,1,4]
+        functions.OP_REVERSE(self.tape, self.stack, self.cache)
+        assert self.stack.list() == [b'4',b'1',b'2',b'3'], self.stack.list()
 
-    def test_OP_REVERSE_raises_ScriptExecutionError_for_queue_depth_overflow(self):
-        self.queue.put(b'sds')
+    def test_OP_REVERSE_raises_ScriptExecutionError_for_stack_depth_overflow(self):
+        self.stack.put(b'sds')
         self.tape = classes.Tape(b'\xff')
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_REVERSE(self.tape, self.queue, self.cache)
-        assert str(e.exception) == 'OP_REVERSE queue size exceeded'
+            functions.OP_REVERSE(self.tape, self.stack, self.cache)
+        assert str(e.exception) == 'OP_REVERSE stack size exceeded'
 
-    def test_OP_CONCAT_concatenates_top_two_items_from_queue(self):
-        self.queue.put(b'123')
-        self.queue.put(b'321')
-        functions.OP_CONCAT(self.tape, self.queue, self.cache)
-        assert self.queue.get(False) == b'321123'
-        assert self.queue.empty()
+    def test_OP_CONCAT_concatenates_top_two_items_from_stack(self):
+        self.stack.put(b'321')
+        self.stack.put(b'123')
+        functions.OP_CONCAT(self.tape, self.stack, self.cache)
+        assert self.stack.get() == b'321123'
+        assert self.stack.empty()
 
-    def test_OP_SPLIT_splits_top_queue_item_at_uint_index_read_from_tape(self):
+    def test_OP_SPLIT_splits_top_stack_item_at_uint_index_read_from_tape(self):
         self.tape = classes.Tape(b'\x02')
-        self.queue.put(b'12345')
-        functions.OP_SPLIT(self.tape, self.queue, self.cache)
-        assert self.queue.get(False) == b'345'
-        assert self.queue.get(False) == b'12'
+        self.stack.put(b'12345')
+        functions.OP_SPLIT(self.tape, self.stack, self.cache)
+        assert self.stack.get() == b'345'
+        assert self.stack.get() == b'12'
 
     def test_OP_SPLIT_raises_ScriptExecutionError_for_length_index_overflow(self):
-        self.queue.put(b'sds')
+        self.stack.put(b'sds')
         self.tape = classes.Tape(b'\xff')
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_SPLIT(self.tape, self.queue, self.cache)
+            functions.OP_SPLIT(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_SPLIT item len exceeded by index'
 
-    def test_OP_CONCAT_STR_concatenates_top_two_utf8_str_items_from_queue(self):
-        self.queue.put(bytes('123', 'utf-8'))
-        self.queue.put(bytes('abc', 'utf-8'))
-        functions.OP_CONCAT_STR(self.tape, self.queue, self.cache)
-        item = self.queue.get(False)
+    def test_OP_SPLIT_and_OP_CONCAT_are_inverse_functions(self):
+        first = b'123'
+        second = b'abc'
+        self.stack.put(first)
+        self.stack.put(second)
+        functions.OP_CONCAT(self.tape, self.stack, self.cache)
+        functions.OP_SPLIT(classes.Tape(b'\x03'), self.stack, self.cache)
+        assert self.stack.get() == second
+        assert self.stack.get() == first
+
+    def test_OP_CONCAT_STR_concatenates_top_two_utf8_str_items_from_stack(self):
+        self.stack.put(bytes('abc', 'utf-8'))
+        self.stack.put(bytes('123', 'utf-8'))
+        functions.OP_CONCAT_STR(self.tape, self.stack, self.cache)
+        item = self.stack.get()
         assert str(item, 'utf-8') == 'abc123'
-        assert self.queue.empty()
+        assert self.stack.empty()
 
-    def test_OP_SPLIT_STR_splits_top_queue_utf8_str_at_uint_index_read_from_tape(self):
+    def test_OP_SPLIT_STR_splits_top_stack_utf8_str_at_uint_index_read_from_tape(self):
         self.tape = classes.Tape(b'\x02')
-        self.queue.put(bytes('12345', 'utf-8'))
-        functions.OP_SPLIT_STR(self.tape, self.queue, self.cache)
-        assert str(self.queue.get(False), 'utf-8') == '345'
-        assert str(self.queue.get(False), 'utf-8') == '12'
+        self.stack.put(bytes('12345', 'utf-8'))
+        functions.OP_SPLIT_STR(self.tape, self.stack, self.cache)
+        assert str(self.stack.get(), 'utf-8') == '345'
+        assert str(self.stack.get(), 'utf-8') == '12'
 
     def test_OP_SPLIT_STR_raises_ScriptExecutionError_for_str_length_overflow(self):
-        self.queue.put(b'sds')
+        self.stack.put(b'sds')
         self.tape = classes.Tape(b'\xff')
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_SPLIT_STR(self.tape, self.queue, self.cache)
+            functions.OP_SPLIT_STR(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_SPLIT_STR item len exceeded by index'
 
-    def test_NOP_reads_int_from_tape_and_pulls_that_many_items_from_queue(self):
-        assert self.queue.empty()
-        self.queue.put(1)
-        self.queue.put(2)
-        self.queue.put(3)
+    def test_NOP_reads_int_from_tape_and_pulls_that_many_items_from_stack(self):
+        assert self.stack.empty()
+        self.stack.put(b'1')
+        self.stack.put(b'2')
+        self.stack.put(b'3')
         self.tape = classes.Tape(functions.int_to_bytes(2))
-        functions.NOP(self.tape, self.queue, self.cache)
-        assert self.queue.get(False) == 1
-        assert self.queue.empty()
+        functions.NOP(self.tape, self.stack, self.cache)
+        assert self.stack.get() == b'1'
+        assert self.stack.empty()
 
     def test_NOP_raises_ScriptExecutionError_for_negative_count(self):
         self.tape = classes.Tape(functions.int_to_bytes(-2))
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.NOP(self.tape, self.queue, self.cache)
+            functions.NOP(self.tape, self.stack, self.cache)
 
     def test_OP_CHECK_TRANSFER_errors_on_missing_or_invalid_contract_or_params(self):
         def setup_transfer():
             self.tape = classes.Tape(b'\x01')
-            self.queue.put(b'txn_proof')
-            self.queue.put(b'source')
-            self.queue.put(b'\x01')
-            self.queue.put(b'destination')
-            self.queue.put(b'constraint')
-            self.queue.put(b'amount')
-            self.queue.put(b'contractid')
+            self.stack.put(b'txn_proof')
+            self.stack.put(b'source')
+            self.stack.put(b'\x01')
+            self.stack.put(b'destination')
+            self.stack.put(b'constraint')
+            self.stack.put(b'amount')
+            self.stack.put(b'contractid')
 
         setup_transfer()
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_TRANSFER(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_TRANSFER(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_CHECK_TRANSFER missing contract'
 
         setup_transfer()
         self.tape.contracts[b'contractid'] = InvalidContract(10)
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_TRANSFER(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_TRANSFER(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'contract must implement the CanCheckTransfer interface'
 
     def test_OP_CHECK_TRANSFER_works(self):
         def setup_transfer():
             self.tape = classes.Tape(b'\x00')
-            self.queue.put(b'txn_proof')
-            self.queue.put(b'source')
-            self.queue.put((1).to_bytes(1, 'big'))
-            self.queue.put(b'destination')
-            self.queue.put(b'constraint')
-            self.queue.put((10).to_bytes(1, 'big')) # amount
-            self.queue.put(b'contractid')
+            self.stack.put(b'txn_proof')
+            self.stack.put(b'source')
+            self.stack.put((1).to_bytes(1, 'big'))
+            self.stack.put(b'destination')
+            self.stack.put(b'constraint')
+            self.stack.put((10).to_bytes(1, 'big')) # amount
+            self.stack.put(b'contractid')
 
         amount = 10
         setup_transfer()
         self.tape.contracts[b'contractid'] = ValidContract(amount)
-        functions.OP_CHECK_TRANSFER(self.tape, self.queue, self.cache)
-        assert self.queue.get(False) == b'\xff'
-        assert self.queue.empty()
+        functions.OP_CHECK_TRANSFER(self.tape, self.stack, self.cache)
+        assert self.stack.get() == b'\xff'
+        assert self.stack.empty()
 
         amount = 9
         setup_transfer()
         self.tape.contracts[b'contractid'] = ValidContract(amount)
-        functions.OP_CHECK_TRANSFER(self.tape, self.queue, self.cache)
-        assert self.queue.get(False) == b'\x00'
-        assert self.queue.empty()
+        functions.OP_CHECK_TRANSFER(self.tape, self.stack, self.cache)
+        assert self.stack.get() == b'\x00'
+        assert self.stack.empty()
 
         amount = 11
         setup_transfer()
         self.tape.contracts[b'contractid'] = ValidContract(amount)
-        functions.OP_CHECK_TRANSFER(self.tape, self.queue, self.cache)
-        assert self.queue.get(False) == b'\xff'
-        assert self.queue.empty()
+        functions.OP_CHECK_TRANSFER(self.tape, self.stack, self.cache)
+        assert self.stack.get() == b'\xff'
+        assert self.stack.empty()
 
     def test_OP_CALL_reads_uint_from_tape_and_runs_that_definition(self):
         self.tape = classes.Tape(b'\x00')
         self.tape.definitions[b'\x00'] = classes.Tape(b'\x01')
-        assert self.queue.empty()
-        functions.OP_CALL(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        assert self.queue.get(False) == b'\xff'
+        assert self.stack.empty()
+        functions.OP_CALL(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        assert self.stack.get() == b'\xff'
 
     def test_OP_CALL_raises_ScriptExecutionError_when_callstack_limit_exceeded(self):
         self.tape.callstack_limit = -1
         self.tape.callstack_count = 1
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CALL(self.tape, self.queue, self.cache)
+            functions.OP_CALL(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'callstack limit exceeded'
 
     def test_OP_CALL_does_not_reset_definition_pointer(self):
         self.tape = classes.Tape(b'\x00')
         subtape = classes.Tape(b'\x2b\x00\x03\x00\x2a\x00\x02\x03')
         self.tape.definitions[b'\x00'] = subtape
         subtape.definitions = self.tape.definitions
-        assert self.queue.empty()
-        self.queue.put(b'\x01', False)
-        functions.OP_CALL(self.tape, self.queue, self.cache)
+        assert self.stack.empty()
+        self.stack.put(b'\x01')
+        functions.OP_CALL(self.tape, self.stack, self.cache)
         assert self.tape.definitions[b'\x00'].pointer == 0
-        assert self.queue.qsize() == 2
-        assert self.queue.get(False) == b'\x03'
-        assert self.queue.get(False) == b'\x03'
+        assert len(self.stack) == 2
+        assert self.stack.get() == b'\x03'
+        assert self.stack.get() == b'\x03'
 
-    def test_OP_IF_reads_2uint_length_from_tape_pulls_top_queue_bool_and_executes_if_true(self):
+    def test_OP_IF_reads_2uint_length_from_tape_pulls_top_stack_bool_and_executes_if_true(self):
         length = b'\x00\x02'
         op_push0 = b'\x02'
         self.tape = classes.Tape(length + op_push0 + b'X')
-        assert self.queue.empty()
-        self.queue.put(b'\x01')
-        functions.OP_IF(self.tape, self.queue, self.cache)
+        assert self.stack.empty()
+        self.stack.put(b'\x01')
+        functions.OP_IF(self.tape, self.stack, self.cache)
         assert self.tape.has_terminated()
-        assert self.queue.get(False) == b'X'
-        assert self.queue.empty()
+        assert self.stack.get() == b'X'
+        assert self.stack.empty()
 
         length = b'\x00\x02'
         op_push0 = b'\x02'
         self.tape = classes.Tape(length + op_push0 + b'X')
-        assert self.queue.empty()
-        self.queue.put(b'\x00')
-        functions.OP_IF(self.tape, self.queue, self.cache)
+        assert self.stack.empty()
+        self.stack.put(b'\x00')
+        functions.OP_IF(self.tape, self.stack, self.cache)
         assert self.tape.has_terminated()
-        assert self.queue.empty()
+        assert self.stack.empty()
 
-    def test_OP_IF_ELSE_reads_2_definitions_from_tape_and_executes_first_one_if_top_queue_value(self):
+    def test_OP_IF_ELSE_reads_2_definitions_from_tape_and_executes_first_one_if_top_stack_value(self):
         length = b'\x00\x02'
         if_def = b'\x02Y'
         else_def = b'\x02N'
         self.tape = classes.Tape(length + if_def + length + else_def)
-        assert self.queue.empty()
-        self.queue.put(b'\x01')
-        functions.OP_IF_ELSE(self.tape, self.queue, self.cache)
+        assert self.stack.empty()
+        self.stack.put(b'\x01')
+        functions.OP_IF_ELSE(self.tape, self.stack, self.cache)
         assert self.tape.has_terminated()
-        assert self.queue.get(False) == b'Y'
-        assert self.queue.empty()
+        assert self.stack.get() == b'Y'
+        assert self.stack.empty()
 
         self.tape = classes.Tape(length + if_def + length + else_def)
-        assert self.queue.empty()
-        self.queue.put(b'\x00')
-        functions.OP_IF_ELSE(self.tape, self.queue, self.cache)
+        assert self.stack.empty()
+        self.stack.put(b'\x00')
+        functions.OP_IF_ELSE(self.tape, self.stack, self.cache)
         assert self.tape.has_terminated()
-        assert self.queue.get(False) == b'N'
-        assert self.queue.empty()
+        assert self.stack.get() == b'N'
+        assert self.stack.empty()
 
     def test_OP_TRY_EXCEPT_reads_2_definitions_from_tape_executes_properly(self):
         try_len = b'\x00\x02'
         except_len = b'\x00\x01'
         try_def = b'\x00\x20'
         except_def = b'\x01'
         self.tape = classes.Tape(try_len + try_def + except_len + except_def)
-        assert self.queue.empty()
+        assert self.stack.empty()
         assert b'E' not in self.cache
-        functions.OP_TRY_EXCEPT(self.tape, self.queue, self.cache)
+        functions.OP_TRY_EXCEPT(self.tape, self.stack, self.cache)
         assert self.tape.has_terminated()
         assert b'E' in self.cache
         assert len(self.cache[b'E']) == 1
         exname, exstr = str(self.cache[b'E'][0], 'utf-8').split('|')
         assert exname == 'ScriptExecutionError'
         assert exstr == 'OP_VERIFY check failed'
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+        assert not self.stack.empty()
+        item = self.stack.get()
         assert functions.bytes_to_bool(item)
 
-    def test_OP_EVAL_pulls_value_from_queue_and_runs_as_script(self):
+    def test_OP_EVAL_pulls_value_from_stack_and_runs_as_script(self):
         code = b'\x02F'
-        assert self.queue.empty()
-        self.queue.put(code)
-        functions.OP_EVAL(self.tape, self.queue, self.cache)
+        assert self.stack.empty()
+        self.stack.put(code)
+        functions.OP_EVAL(self.tape, self.stack, self.cache)
         assert self.tape.has_terminated()
-        assert not self.queue.empty()
-        assert self.queue.get(False) == b'F'
-        assert self.queue.empty()
+        assert not self.stack.empty()
+        assert self.stack.get() == b'F'
+        assert self.stack.empty()
 
     def test_OP_EVAL_raises_ScriptExecutionError_if_disallow_OP_EVAL_flag_set(self):
         self.tape.flags['disallow_OP_EVAL'] = True
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_EVAL(self.tape, self.queue, self.cache)
+            functions.OP_EVAL(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_EVAL disallowed'
 
     def test_OP_EVAL_raises_ValueError_for_empty_script(self):
-        self.queue.put(b'')
+        self.stack.put(b'')
         with self.assertRaises(ValueError) as e:
-            functions.OP_EVAL(self.tape, self.queue, self.cache)
+            functions.OP_EVAL(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_EVAL encountered empty script'
 
     def test_OP_MERKLEVAL_single_branch(self):
         committed_branch_a = b'\x02A'
         committed_branch_b = b'\x02B'
         commitment_a = sha256(committed_branch_a).digest()
         commitment_b = sha256(committed_branch_b).digest()
-        commitment_root = sha256(commitment_a + commitment_b).digest()
-        self.queue.put(commitment_b)
-        self.queue.put(committed_branch_a)
-        self.queue.put(b'\xff')
+        commitment_root = merkleval_root(commitment_a, commitment_b)
+        self.stack.put(commitment_b)
+        self.stack.put(committed_branch_a)
         self.tape = classes.Tape(commitment_root)
-        functions.OP_MERKLEVAL(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        assert self.queue.get(False) == b'A'
-        assert self.queue.empty()
-
-        self.queue.put(commitment_a)
-        self.queue.put(committed_branch_b)
-        self.queue.put(b'\x00')
+        functions.OP_MERKLEVAL(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        assert self.stack.get() == b'A'
+        assert self.stack.empty()
+
+        self.stack.put(commitment_a)
+        self.stack.put(committed_branch_b)
         self.tape = classes.Tape(commitment_root)
-        functions.OP_MERKLEVAL(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        assert self.queue.get(False) == b'B'
-        assert self.queue.empty()
+        functions.OP_MERKLEVAL(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        assert self.stack.get() == b'B'
+        assert self.stack.empty()
 
     def test_OP_MERKLEVAL_double_branch(self):
         committed_branch_a = b'\x02A'
         committed_branch_ba = b'\x03\x02BA'
         committed_branch_bb = b'\x03\x02BB'
         commitment_a = sha256(committed_branch_a).digest()
         commitment_ba = sha256(committed_branch_ba).digest()
         commitment_bb = sha256(committed_branch_bb).digest()
-        commitment_b_root = sha256(commitment_ba + commitment_bb).digest()
+        commitment_b_root = merkleval_root(commitment_ba, commitment_bb)
         committed_branch_b_root = b'\x3c' + commitment_b_root
         commitment_b = sha256(committed_branch_b_root).digest()
 
-        commitment_root = sha256(commitment_a + commitment_b).digest()
-        self.queue.put(commitment_b)
-        self.queue.put(committed_branch_a)
-        self.queue.put(b'\xff')
+        commitment_root = merkleval_root(commitment_a, commitment_b)
+        self.stack.put(commitment_b)
+        self.stack.put(committed_branch_a)
         self.tape = classes.Tape(commitment_root)
-        functions.OP_MERKLEVAL(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        assert self.queue.get(False) == b'A'
-        assert self.queue.empty()
-
-        self.queue.put(commitment_bb)
-        self.queue.put(committed_branch_ba)
-        self.queue.put(b'\xff')
-        self.queue.put(commitment_a)
-        self.queue.put(committed_branch_b_root)
-        self.queue.put(b'\x00')
+        functions.OP_MERKLEVAL(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        assert self.stack.get() == b'A'
+        assert self.stack.empty()
+
+        self.stack.put(commitment_bb)
+        self.stack.put(committed_branch_ba)
+        self.stack.put(commitment_a)
+        self.stack.put(committed_branch_b_root)
         self.tape = classes.Tape(commitment_root)
-        functions.OP_MERKLEVAL(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        assert self.queue.get(False) == b'BA'
-        assert self.queue.empty()
-
-        self.queue.put(commitment_ba)
-        self.queue.put(committed_branch_bb)
-        self.queue.put(b'\x00')
-        self.queue.put(commitment_a)
-        self.queue.put(committed_branch_b_root)
-        self.queue.put(b'\x00')
+        functions.OP_MERKLEVAL(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        assert self.stack.get() == b'BA'
+        assert self.stack.empty()
+
+        self.stack.put(commitment_ba)
+        self.stack.put(committed_branch_bb)
+        self.stack.put(commitment_a)
+        self.stack.put(committed_branch_b_root)
         self.tape = classes.Tape(commitment_root)
-        functions.OP_MERKLEVAL(self.tape, self.queue, self.cache)
-        assert not self.queue.empty()
-        assert self.queue.get(False) == b'BB'
-        assert self.queue.empty()
+        functions.OP_MERKLEVAL(self.tape, self.stack, self.cache)
+        assert not self.stack.empty()
+        assert self.stack.get() == b'BB'
+        assert self.stack.empty()
 
     def test_OP_MERKLEVAL_raises_error_on_mismatching_hash(self):
         committed_branch_a = b'\x02A'
         committed_branch_b = b'\x02B'
         commitment_a = sha256(committed_branch_a).digest()
         commitment_b = sha256(committed_branch_b).digest()
-        commitment_root = sha256(commitment_a + commitment_b).digest()
-        self.queue.put(commitment_b)
-        self.queue.put(committed_branch_a + b'uncommitted code')
-        self.queue.put(b'\xff')
+        commitment_root = merkleval_root(commitment_a, commitment_b)
+        self.stack.put(commitment_b)
+        self.stack.put(committed_branch_a + b'uncommitted code')
         self.tape = classes.Tape(commitment_root)
 
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_MERKLEVAL(self.tape, self.queue, self.cache)
+            functions.OP_MERKLEVAL(self.tape, self.stack, self.cache)
         assert str(e.exception) == 'OP_VERIFY check failed'
 
-    def test_OP_LESS_pulls_two_ints_from_queue_and_places_bool_on_queue(self):
+    def test_OP_LESS_pulls_two_ints_from_stack_and_places_bool_on_stack(self):
         val1 = functions.int_to_bytes(123)
         val2 = functions.int_to_bytes(321)
-        self.queue.put(val1)
-        self.queue.put(val2)
-        functions.OP_LESS(self.tape, self.queue, self.cache)
-        assert self.queue._qsize() == 1
-        result = self.queue.get(False)
+        self.stack.put(val1)
+        self.stack.put(val2)
+        functions.OP_LESS(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        result = self.stack.get()
         assert result == b'\x00'
 
-        self.queue.put(val1)
-        self.queue.put(val1)
-        functions.OP_LESS(self.tape, self.queue, self.cache)
-        assert self.queue._qsize() == 1
-        result = self.queue.get(False)
+        self.stack.put(val1)
+        self.stack.put(val1)
+        functions.OP_LESS(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        result = self.stack.get()
         assert result == b'\x00'
 
-        self.queue.put(val2)
-        self.queue.put(val1)
-        functions.OP_LESS(self.tape, self.queue, self.cache)
-        assert self.queue._qsize() == 1
-        result = self.queue.get(False)
+        self.stack.put(val2)
+        self.stack.put(val1)
+        functions.OP_LESS(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        result = self.stack.get()
         assert result == b'\xff'
 
-    def test_OP_LESS_OR_EQUAL_pulls_two_ints_from_queue_and_places_bool_on_queue(self):
+    def test_OP_LESS_OR_EQUAL_pulls_two_ints_from_stack_and_places_bool_on_stack(self):
         val1 = functions.int_to_bytes(123)
         val2 = functions.int_to_bytes(321)
-        self.queue.put(val1)
-        self.queue.put(val2)
-        functions.OP_LESS_OR_EQUAL(self.tape, self.queue, self.cache)
-        assert self.queue._qsize() == 1
-        result = self.queue.get(False)
+        self.stack.put(val1)
+        self.stack.put(val2)
+        functions.OP_LESS_OR_EQUAL(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        result = self.stack.get()
         assert result == b'\x00'
 
-        self.queue.put(val1)
-        self.queue.put(val1)
-        functions.OP_LESS_OR_EQUAL(self.tape, self.queue, self.cache)
-        assert self.queue._qsize() == 1
-        result = self.queue.get(False)
+        self.stack.put(val1)
+        self.stack.put(val1)
+        functions.OP_LESS_OR_EQUAL(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        result = self.stack.get()
         assert result == b'\xff'
 
-        self.queue.put(val2)
-        self.queue.put(val1)
-        functions.OP_LESS_OR_EQUAL(self.tape, self.queue, self.cache)
-        assert self.queue._qsize() == 1
-        result = self.queue.get(False)
+        self.stack.put(val2)
+        self.stack.put(val1)
+        functions.OP_LESS_OR_EQUAL(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        result = self.stack.get()
         assert result == b'\xff'
 
-    def test_OP_GET_VALUE_pulls_str_from_tape_and_puts_cache_vals_onto_queue(self):
+    def test_OP_GET_VALUE_pulls_str_from_tape_and_puts_cache_vals_onto_stack(self):
         key = bytes('test', 'utf-8')
         self.cache['test'] = 123
         self.tape.data = functions.int_to_bytes(len(key)) + key
-        functions.OP_GET_VALUE(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
+        functions.OP_GET_VALUE(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
         assert self.tape.has_terminated()
-        result = self.queue.get(False)
+        result = self.stack.get()
         assert result == functions.int_to_bytes(123)
 
         self.cache['test'] = [123, 12.34, 'abc', b'ac']
-        assert self.queue.qsize() == 0
+        assert len(self.stack) == 0
         self.tape.reset_pointer()
-        functions.OP_GET_VALUE(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 4
+        functions.OP_GET_VALUE(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 4
         result = [
-            self.queue.get(False),
-            self.queue.get(False),
-            self.queue.get(False),
-            self.queue.get(False),
+            self.stack.get(),
+            self.stack.get(),
+            self.stack.get(),
+            self.stack.get(),
         ]
         assert result[0] == b'ac'
         assert result[1] == bytes('abc', 'utf-8')
         assert result[2] == functions.float_to_bytes(12.34)
         assert result[3] == functions.int_to_bytes(123)
 
-    def test_OP_FLOAT_LESS_pulls_two_floats_from_queue_and_places_bool_on_queue(self):
+    def test_OP_FLOAT_LESS_pulls_two_floats_from_stack_and_places_bool_on_stack(self):
         val1 = functions.float_to_bytes(123.0)
         val2 = functions.float_to_bytes(321.0)
-        self.queue.put(val1)
-        self.queue.put(val2)
-        functions.OP_FLOAT_LESS(self.tape, self.queue, self.cache)
-        assert self.queue._qsize() == 1
-        result = self.queue.get(False)
+        self.stack.put(val1)
+        self.stack.put(val2)
+        functions.OP_FLOAT_LESS(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        result = self.stack.get()
         assert result == b'\x00'
 
-        self.queue.put(val1)
-        self.queue.put(val1)
-        functions.OP_FLOAT_LESS(self.tape, self.queue, self.cache)
-        assert self.queue._qsize() == 1
-        result = self.queue.get(False)
+        self.stack.put(val1)
+        self.stack.put(val1)
+        functions.OP_FLOAT_LESS(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        result = self.stack.get()
         assert result == b'\x00'
 
-        self.queue.put(val2)
-        self.queue.put(val1)
-        functions.OP_FLOAT_LESS(self.tape, self.queue, self.cache)
-        assert self.queue._qsize() == 1
-        result = self.queue.get(False)
+        self.stack.put(val2)
+        self.stack.put(val1)
+        functions.OP_FLOAT_LESS(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        result = self.stack.get()
         assert result == b'\xff'
 
-    def test_OP_FLOAT_LESS_OR_EQUAL_pulls_two_floats_from_queue_and_places_bool_on_queue(self):
+    def test_OP_FLOAT_LESS_OR_EQUAL_pulls_two_floats_from_stack_and_places_bool_on_stack(self):
         val1 = functions.float_to_bytes(123.0)
         val2 = functions.float_to_bytes(321.0)
-        self.queue.put(val1)
-        self.queue.put(val2)
-        functions.OP_FLOAT_LESS_OR_EQUAL(self.tape, self.queue, self.cache)
-        assert self.queue._qsize() == 1
-        result = self.queue.get(False)
+        self.stack.put(val1)
+        self.stack.put(val2)
+        functions.OP_FLOAT_LESS_OR_EQUAL(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        result = self.stack.get()
         assert result == b'\x00'
 
-        self.queue.put(val1)
-        self.queue.put(val1)
-        functions.OP_FLOAT_LESS_OR_EQUAL(self.tape, self.queue, self.cache)
-        assert self.queue._qsize() == 1
-        result = self.queue.get(False)
+        self.stack.put(val1)
+        self.stack.put(val1)
+        functions.OP_FLOAT_LESS_OR_EQUAL(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        result = self.stack.get()
         assert result == b'\xff'
 
-        self.queue.put(val2)
-        self.queue.put(val1)
-        functions.OP_FLOAT_LESS_OR_EQUAL(self.tape, self.queue, self.cache)
-        assert self.queue._qsize() == 1
-        result = self.queue.get(False)
+        self.stack.put(val2)
+        self.stack.put(val1)
+        functions.OP_FLOAT_LESS_OR_EQUAL(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        result = self.stack.get()
         assert result == b'\xff'
 
     def test_OP_INT_TO_FLOAT_works_correctly(self):
         val = functions.int_to_bytes(123)
-        self.queue.put(val)
-        functions.OP_INT_TO_FLOAT(self.tape, self.queue, self.cache)
-        result = self.queue.get(False)
+        self.stack.put(val)
+        functions.OP_INT_TO_FLOAT(self.tape, self.stack, self.cache)
+        result = self.stack.get()
         assert result == functions.float_to_bytes(123 * 1.0)
 
     def test_OP_FLOAT_TO_INT_works_correctly(self):
         val = functions.float_to_bytes(123.1)
-        self.queue.put(val)
-        functions.OP_FLOAT_TO_INT(self.tape, self.queue, self.cache)
-        result = self.queue.get(False)
+        self.stack.put(val)
+        functions.OP_FLOAT_TO_INT(self.tape, self.stack, self.cache)
+        result = self.stack.get()
         assert result == functions.int_to_bytes(123)
 
     def test_OP_LOOP_raises_error_for_too_many_executions(self):
         self.tape.data = b'\x00\x00'
-        self.queue.put(b'\x01')
+        self.stack.put(b'\x01')
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_LOOP(self.tape, self.queue, self.cache)
+            functions.OP_LOOP(self.tape, self.stack, self.cache)
         assert 'OP_LOOP limit exceeded' in str(e.exception)
 
-    def test_OP_LOOP_executes_for_true_top_queue_value(self):
+    def test_OP_LOOP_executes_for_true_top_stack_value(self):
         self.tape.data = b'\x00\x01\x00'
-        self.queue.put(b'\x01')
-        assert self.queue.qsize() == 1
-        functions.OP_LOOP(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 2
+        self.stack.put(b'\x01')
+        assert len(self.stack) == 1
+        functions.OP_LOOP(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 2
 
-    def test_OP_LOOP_skips_execution_for_false_top_queue_value(self):
+    def test_OP_LOOP_skips_execution_for_false_top_stack_value(self):
         self.tape.data = b'\x00\x01\x00'
-        self.queue.put(b'\x00')
-        assert self.queue.qsize() == 1
-        functions.OP_LOOP(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
+        self.stack.put(b'\x00')
+        assert len(self.stack) == 1
+        functions.OP_LOOP(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
 
-    def test_OP_CHECK_MULTISIG_pulls_m_sigs_from_queue_then_n_vkeys_and_verifies(self):
+    def test_OP_CHECK_MULTISIG_pulls_m_sigs_from_stack_then_n_vkeys_and_verifies(self):
         # 3-of-3
         self.tape.data = b'\x00\x03\x03'
         msg = b'hi I am a protocol value that is signed'
         self.cache['sigfield1'] = msg
         skeys = [
             SigningKey(token_bytes(32)),
             SigningKey(token_bytes(32)),
             SigningKey(token_bytes(32)),
         ]
         vkeys = [skey.verify_key for skey in skeys]
         sigs = [skey.sign(msg).signature for skey in skeys]
-        [self.queue.put(bytes(sig)) for sig in sigs]
-        [self.queue.put(bytes(vkey)) for vkey in vkeys]
-        functions.OP_CHECK_MULTISIG(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        assert functions.bytes_to_bool(self.queue.get(False))
+        [self.stack.put(bytes(sig)) for sig in sigs]
+        [self.stack.put(bytes(vkey)) for vkey in vkeys]
+        functions.OP_CHECK_MULTISIG(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        assert functions.bytes_to_bool(self.stack.get())
 
         # 2-of-3
         self.tape = classes.Tape(b'\x00\x02\x03')
-        [self.queue.put(bytes(sig)) for sig in sigs[:2]]
-        [self.queue.put(bytes(vkey)) for vkey in vkeys]
-        functions.OP_CHECK_MULTISIG(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        assert functions.bytes_to_bool(self.queue.get(False))
+        [self.stack.put(bytes(sig)) for sig in sigs[:2]]
+        [self.stack.put(bytes(vkey)) for vkey in vkeys]
+        functions.OP_CHECK_MULTISIG(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        assert functions.bytes_to_bool(self.stack.get())
 
-    def test_OP_CHECK_MULTISIG_puts_false_onto_queue_for_reused_sig(self):
+    def test_OP_CHECK_MULTISIG_puts_false_onto_stack_for_reused_sig(self):
         # 3-of-3
         self.tape.data = b'\x00\x03\x03'
         msg = b'hi I am a protocol value that is signed'
         self.cache['sigfield1'] = msg
         skeys = [
             SigningKey(token_bytes(32)),
             SigningKey(token_bytes(32)),
             SigningKey(token_bytes(32)),
         ]
         vkeys = [skey.verify_key for skey in skeys]
         sigs = [skey.sign(msg).signature for skey in skeys]
-        [self.queue.put(bytes(sigs[0])) for _ in sigs]
-        [self.queue.put(bytes(vkey)) for vkey in vkeys]
-        functions.OP_CHECK_MULTISIG(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        assert not functions.bytes_to_bool(self.queue.get(False))
+        [self.stack.put(bytes(sigs[0])) for _ in sigs]
+        [self.stack.put(bytes(vkey)) for vkey in vkeys]
+        functions.OP_CHECK_MULTISIG(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        assert not functions.bytes_to_bool(self.stack.get())
 
-    def test_OP_CHECK_MULTISIG_puts_false_onto_queue_for_sig_using_wrong_key(self):
+    def test_OP_CHECK_MULTISIG_puts_false_onto_stack_for_sig_using_wrong_key(self):
         # 2-of-2
         self.tape.data = b'\x00\x02\x02'
         msg = b'hi I am a protocol value that is signed'
         self.cache['sigfield1'] = msg
         skeys = [
             SigningKey(token_bytes(32)),
             SigningKey(token_bytes(32)),
             SigningKey(token_bytes(32)),
         ]
         vkeys = [skey.verify_key for skey in skeys]
         sigs = [skey.sign(msg).signature for skey in skeys]
-        [self.queue.put(bytes(sig)) for sig in sigs[1:]]
-        [self.queue.put(bytes(vkey)) for vkey in vkeys[:2]]
-        functions.OP_CHECK_MULTISIG(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        assert not functions.bytes_to_bool(self.queue.get(False))
+        [self.stack.put(bytes(sig)) for sig in sigs[1:]]
+        [self.stack.put(bytes(vkey)) for vkey in vkeys[:2]]
+        functions.OP_CHECK_MULTISIG(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        assert not functions.bytes_to_bool(self.stack.get())
 
     def test_OP_CHECK_MULTISIG_VERIFY_executes_without_error_for_good_paths(self):
         # 3-of-3
         self.tape.data = b'\x00\x03\x03'
         msg = b'hi I am a protocol value that is signed'
         self.cache['sigfield1'] = msg
         skeys = [
             SigningKey(token_bytes(32)),
             SigningKey(token_bytes(32)),
             SigningKey(token_bytes(32)),
         ]
         vkeys = [skey.verify_key for skey in skeys]
         sigs = [skey.sign(msg).signature for skey in skeys]
-        [self.queue.put(bytes(sig)) for sig in sigs]
-        [self.queue.put(bytes(vkey)) for vkey in vkeys]
-        functions.OP_CHECK_MULTISIG_VERIFY(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 0
+        [self.stack.put(bytes(sig)) for sig in sigs]
+        [self.stack.put(bytes(vkey)) for vkey in vkeys]
+        functions.OP_CHECK_MULTISIG_VERIFY(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 0
 
         # 2-of-3
         self.tape = classes.Tape(b'\x00\x02\x03')
-        [self.queue.put(bytes(sig)) for sig in sigs[:2]]
-        [self.queue.put(bytes(vkey)) for vkey in vkeys]
-        functions.OP_CHECK_MULTISIG_VERIFY(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 0
+        [self.stack.put(bytes(sig)) for sig in sigs[:2]]
+        [self.stack.put(bytes(vkey)) for vkey in vkeys]
+        functions.OP_CHECK_MULTISIG_VERIFY(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 0
 
     def test_OP_CHECK_MULTISIG_VERIFY_raises_error_for_reused_sig(self):
         # 3-of-3
         self.tape.data = b'\x00\x03\x03'
         msg = b'hi I am a protocol value that is signed'
         self.cache['sigfield1'] = msg
         skeys = [
             SigningKey(token_bytes(32)),
             SigningKey(token_bytes(32)),
             SigningKey(token_bytes(32)),
         ]
         vkeys = [skey.verify_key for skey in skeys]
         sigs = [skey.sign(msg).signature for skey in skeys]
-        [self.queue.put(bytes(sigs[0])) for _ in sigs]
-        [self.queue.put(bytes(vkey)) for vkey in vkeys]
+        [self.stack.put(bytes(sigs[0])) for _ in sigs]
+        [self.stack.put(bytes(vkey)) for vkey in vkeys]
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_MULTISIG_VERIFY(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 0
+            functions.OP_CHECK_MULTISIG_VERIFY(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 0
 
     def test_OP_CHECK_MULTISIG_VERIFY_raises_error_for_sig_using_wrong_key(self):
         # 2-of-2
         self.tape.data = b'\x00\x02\x02'
         msg = b'hi I am a protocol value that is signed'
         self.cache['sigfield1'] = msg
         skeys = [
             SigningKey(token_bytes(32)),
             SigningKey(token_bytes(32)),
             SigningKey(token_bytes(32)),
         ]
         vkeys = [skey.verify_key for skey in skeys]
         sigs = [skey.sign(msg).signature for skey in skeys]
-        [self.queue.put(bytes(sig)) for sig in sigs[1:]]
-        [self.queue.put(bytes(vkey)) for vkey in vkeys[:2]]
+        [self.stack.put(bytes(sig)) for sig in sigs[1:]]
+        [self.stack.put(bytes(vkey)) for vkey in vkeys[:2]]
         with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.OP_CHECK_MULTISIG_VERIFY(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 0
+            functions.OP_CHECK_MULTISIG_VERIFY(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 0
 
     def test_OP_SIGN_creates_valid_signatures(self):
         seed = token_bytes(32)
         self.tape.data = b'\x02'
-        self.queue.put(seed)
+        self.stack.put(seed)
         self.cache['sigfield1'] = b'hello'
         self.cache['sigfield2'] = b'excluded by sigflag'
         self.cache['sigfield3'] = b'world'
-        functions.OP_SIGN(self.tape, self.queue, self.cache)
-        sig = self.queue.get(False)
-        assert self.queue.qsize() == 0
+        functions.OP_SIGN(self.tape, self.stack, self.cache)
+        sig = self.stack.get()
+        assert len(self.stack) == 0
         assert len(sig) == nacl.bindings.crypto_sign_BYTES + 1, 'invalid signature'
 
-        self.queue.put(sig)
-        self.queue.put(bytes(SigningKey(seed).verify_key))
+        self.stack.put(sig)
+        self.stack.put(bytes(SigningKey(seed).verify_key))
         self.tape.reset()
-        functions.OP_CHECK_SIG(self.tape, self.queue, self.cache)
-        result = self.queue.get(False)
-        assert self.queue.qsize() == 0
+        functions.OP_CHECK_SIG(self.tape, self.stack, self.cache)
+        result = self.stack.get()
+        assert len(self.stack) == 0
         assert result == b'\xff'
 
     def test_OP_SIGN_raises_error_for_invalid_key(self):
         seed = b'not a valid key length'
         self.tape.data = b'\x00'
-        self.queue.put(seed)
+        self.stack.put(seed)
         self.cache['sigfield1'] = b'test'
         with self.assertRaises(ValueError) as e:
-            functions.OP_SIGN(self.tape, self.queue, self.cache)
+            functions.OP_SIGN(self.tape, self.stack, self.cache)
         assert 'invalid' in str(e.exception)
 
-    def test_OP_SIGN_QUEUE_signs_message_from_queue_using_skey_seed_from_queue(self):
+    def test_OP_SIGN_STACK_signs_message_from_stack_using_skey_seed_from_stack(self):
         seed = token_bytes(nacl.bindings.crypto_sign_SEEDBYTES)
         msg = b'hello world'
-        self.queue.put(msg)
-        self.queue.put(seed)
-        functions.OP_SIGN_QUEUE(self.tape, self.queue, self.cache)
-        sig = self.queue.get(False)
+        self.stack.put(msg)
+        self.stack.put(seed)
+        functions.OP_SIGN_STACK(self.tape, self.stack, self.cache)
+        sig = self.stack.get()
         assert len(sig) == nacl.bindings.crypto_sign_BYTES
         SigningKey(seed).verify_key.verify(msg, sig)
 
-    def test_OP_CHECK_SIG_QUEUE_raises_correct_errors(self):
+    def test_OP_CHECK_SIG_STACK_raises_correct_errors(self):
         seed = token_bytes(nacl.bindings.crypto_sign_SEEDBYTES)
         msg = b'hello world'
         skey = SigningKey(seed)
         sig = skey.sign(msg).signature
 
-        self.queue.put(msg)
-        self.queue.put(sig)
-        self.queue.put(bytes(skey.verify_key)[:-1])
+        self.stack.put(sig)
+        self.stack.put(msg)
+        self.stack.put(bytes(skey.verify_key)[:-1])
         with self.assertRaises(ValueError) as e:
-            functions.OP_CHECK_SIG_QUEUE(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_SIG_STACK(self.tape, self.stack, self.cache)
         assert 'invalid vkey' in str(e.exception)
 
-        self.queue.put(msg)
-        self.queue.put(sig[:-1])
-        self.queue.put(bytes(skey.verify_key))
+        self.stack.put(sig[:-1])
+        self.stack.put(msg)
+        self.stack.put(bytes(skey.verify_key))
         with self.assertRaises(ValueError) as e:
-            functions.OP_CHECK_SIG_QUEUE(self.tape, self.queue, self.cache)
+            functions.OP_CHECK_SIG_STACK(self.tape, self.stack, self.cache)
         assert 'invalid sig' in str(e.exception)
 
-    def test_OP_CHECK_SIG_QUEUE_puts_correct_bool_onto_queue(self):
+    def test_OP_CHECK_SIG_STACK_puts_correct_bool_onto_stack(self):
         seed = token_bytes(nacl.bindings.crypto_sign_SEEDBYTES)
         msg = b'hello world'
         skey = SigningKey(seed)
         sig = skey.sign(msg).signature
 
-        self.queue.put(msg)
-        self.queue.put(sig)
-        self.queue.put(bytes(skey.verify_key))
-        functions.OP_CHECK_SIG_QUEUE(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        assert self.queue.get(False) == b'\xff'
-
-        self.queue.put(msg)
-        self.queue.put(sig[1:] + sig[:1])
-        self.queue.put(bytes(skey.verify_key))
-        functions.OP_CHECK_SIG_QUEUE(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        assert self.queue.get(False) == b'\x00'
+        self.stack.put(sig)
+        self.stack.put(msg)
+        self.stack.put(bytes(skey.verify_key))
+        functions.OP_CHECK_SIG_STACK(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        assert self.stack.get() == b'\xff'
+
+        self.stack.put(sig[1:] + sig[:1])
+        self.stack.put(msg)
+        self.stack.put(bytes(skey.verify_key))
+        functions.OP_CHECK_SIG_STACK(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        assert self.stack.get() == b'\x00'
 
     def test_OP_INVOKE_e2e(self):
         contract_id = b'abcdef'
         class ABIContract:
             def abi(self, args: list[bytes]) -> list[bytes]:
                 return [b''.join(args)]
-        self.queue.put(b'world')
-        self.queue.put(b'hello')
-        self.queue.put(b'\x02')
-        self.queue.put(contract_id)
+        self.stack.put(b'world')
+        self.stack.put(b'hello')
+        self.stack.put(b'\x02')
+        self.stack.put(contract_id)
         self.tape.contracts[contract_id] = ABIContract()
-        functions.OP_INVOKE(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        assert self.queue.get(False) == b'helloworld'
+        functions.OP_INVOKE(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        assert self.stack.get() == b'helloworld'
 
-    def test_OP_XOR_takes_two_values_and_puts_XOR_of_them_onto_queue(self):
+    def test_OP_XOR_takes_two_values_and_puts_XOR_of_them_onto_stack(self):
         item1 = b'hello'
         item2 = b'world'
         expected = []
         for i in range(len(item1)):
             expected.append(item1[i] ^ item2[i])
         expected = bytes(expected)
-        self.queue.put(item1)
-        self.queue.put(item2)
-        functions.OP_XOR(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        observed = self.queue.get(False)
+        self.stack.put(item1)
+        self.stack.put(item2)
+        functions.OP_XOR(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        observed = self.stack.get()
         assert expected == observed, \
             f'expected {expected.hex()}, observed {observed.hex()}'
 
-    def test_OP_OR_takes_two_values_and_puts_OR_of_them_onto_queue(self):
+    def test_OP_OR_takes_two_values_and_puts_OR_of_them_onto_stack(self):
         item1 = b'\xf0'
         item2 = b'\x01'
         expected = b'\xf1'
-        self.queue.put(item1)
-        self.queue.put(item2)
-        functions.OP_OR(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        observed = self.queue.get(False)
+        self.stack.put(item1)
+        self.stack.put(item2)
+        functions.OP_OR(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        observed = self.stack.get()
         assert expected == observed, \
             f'expected {expected.hex()}, observed {observed.hex()}'
 
-    def test_OP_AND_takes_two_values_and_puts_AND_of_them_onto_queue(self):
+    def test_OP_AND_takes_two_values_and_puts_AND_of_them_onto_stack(self):
         item1 = b'\xf0'
         item2 = b'\x01'
         expected = b'\x00'
-        self.queue.put(item1)
-        self.queue.put(item2)
-        functions.OP_AND(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        observed = self.queue.get(False)
+        self.stack.put(item1)
+        self.stack.put(item2)
+        functions.OP_AND(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        observed = self.stack.get()
         assert expected == observed, \
             f'expected {expected.hex()}, observed {observed.hex()}'
 
     def test_OP_DERIVE_SCALAR_creates_32_byte_value_from_seed(self):
-        self.queue.put(b'yellow submarine')
-        functions.OP_DERIVE_SCALAR(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        result = self.queue.get(False)
+        self.stack.put(b'yellow submarine')
+        functions.OP_DERIVE_SCALAR(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        result = self.stack.get()
         assert len(result) == 32
 
     def test_OP_CLAMP_SCALAR_clamps_32_bytes_to_ed25519_scalar(self):
         seed = token_bytes(32)
-        self.queue.put(seed)
+        self.stack.put(seed)
         self.tape.data = b'\x00'
-        functions.OP_CLAMP_SCALAR(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        x1 = self.queue.get(False)
+        functions.OP_CLAMP_SCALAR(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        x1 = self.stack.get()
         assert len(x1) == 32
         assert not (x1[31] & 0b10000000)
 
         self.tape = classes.Tape(b'\x01')
-        self.queue.put(seed)
-        functions.OP_CLAMP_SCALAR(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        x2 = self.queue.get(False)
+        self.stack.put(seed)
+        functions.OP_CLAMP_SCALAR(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        x2 = self.stack.get()
         assert len(x2) == 32
         assert not (x2[31] & 0b10000000)
         assert not (x2[0] & 0b00000111)
         assert (x2[31] & 0b01000000)
 
     def test_OP_CLAMP_SCALAR_raises_ValueError_for_invalid_seed_size(self):
         seed = token_bytes(token_bytes(1)[0] % 32) # 31 random bytes
-        self.queue.put(seed)
+        self.stack.put(seed)
         self.tape.data = b'\x00'
         with self.assertRaises(ValueError) as e:
-            functions.OP_CLAMP_SCALAR(self.tape, self.queue, self.cache)
+            functions.OP_CLAMP_SCALAR(self.tape, self.stack, self.cache)
 
-    def test_OP_DERIVE_POINT_replaces_scalar_with_point_on_queue_and_sets_cache(self):
+    def test_OP_DERIVE_POINT_replaces_scalar_with_point_on_stack_and_sets_cache(self):
         seed = token_bytes(32)
         x = functions.derive_key_from_seed(seed)
-        self.queue.put(x)
+        self.stack.put(x)
         assert b'X' not in self.cache
         functions.set_tape_flags(self.tape)
-        functions.OP_DERIVE_POINT(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
+        functions.OP_DERIVE_POINT(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
         assert b'X' in self.cache
-        X = self.queue.get(False)
+        X = self.stack.get()
         assert X != x
 
     def test_OP_DERIVE_POINT_works_with_CHECK_SIG(self):
         # basically proves it generates a public key
         seed = token_bytes(32)
         x = functions.derive_key_from_seed(seed)
         m = b'hello world'
-        self.queue.put(x)
-        functions.OP_DERIVE_POINT(self.tape, self.queue, self.cache)
-        X = self.queue.get(False)
+        self.stack.put(x)
+        functions.OP_DERIVE_POINT(self.tape, self.stack, self.cache)
+        X = self.stack.get()
         sig = SigningKey(seed).sign(m).signature
 
         self.tape = classes.Tape(b'\x00')
-        self.queue.put(m)
-        self.queue.put(sig)
-        self.queue.put(X)
-        functions.OP_CHECK_SIG_QUEUE(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        assert self.queue.get(False) == b'\xff'
+        self.stack.put(sig)
+        self.stack.put(m)
+        self.stack.put(X)
+        functions.OP_CHECK_SIG_STACK(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        assert self.stack.get() == b'\xff'
 
     def test_OP_SUBTRACT_POINTS_and_OP_SUBTRACT_SCALARS_work_properly(self):
         seed1 = token_bytes(32)
         seed2 = token_bytes(32)
         x1 = functions.derive_key_from_seed(seed1)
         x2 = functions.derive_key_from_seed(seed2)
         x3 = functions.aggregate_scalars([x1, x2])
@@ -1895,175 +1909,235 @@
         X2 = functions.derive_point_from_scalar(x2)
         X3_1 = functions.aggregate_points([X1, X2])
         X3_2 = functions.derive_point_from_scalar(x3)
         assert X3_1 == X3_2
         assert X3_1 not in (X1, X2)
 
         self.tape.data = b'\x02'
-        self.queue.put(x2)
-        self.queue.put(x3)
-        functions.OP_SUBTRACT_SCALARS(self.tape, self.queue, self.cache)
-        x = self.queue.get(False)
+        self.stack.put(x2)
+        self.stack.put(x3)
+        functions.OP_SUBTRACT_SCALARS(self.tape, self.stack, self.cache)
+        x = self.stack.get()
         X = functions.derive_point_from_scalar(x)
         assert X == X1
 
         self.tape.reset()
-        self.queue.put(X2)
-        self.queue.put(X3_1)
-        functions.OP_SUBTRACT_POINTS(self.tape, self.queue, self.cache)
-        X = self.queue.get(False)
+        self.stack.put(X2)
+        self.stack.put(X3_1)
+        functions.OP_SUBTRACT_POINTS(self.tape, self.stack, self.cache)
+        X = self.stack.get()
         assert X == X1
 
-    def test_OP_MAKE_ADAPTER_SIG_PUBLIC_takes_3_from_and_puts_2_on_queue(self):
+    def test_OP_MAKE_ADAPTER_SIG_PUBLIC_takes_3_from_and_puts_2_on_stack(self):
         seed = token_bytes(32)
         T = functions.derive_point_from_scalar(
             functions.derive_key_from_seed(token_bytes(32))
         )
         m = b'hello world'
-        self.queue.put(seed)
-        self.queue.put(m)
-        self.queue.put(T)
+        self.stack.put(seed)
+        self.stack.put(m)
+        self.stack.put(T)
         functions.set_tape_flags(self.tape)
-        functions.OP_MAKE_ADAPTER_SIG_PUBLIC(self.tape, self.queue, self.cache)
+        functions.OP_MAKE_ADAPTER_SIG_PUBLIC(self.tape, self.stack, self.cache)
         assert b'T' in self.cache
         assert b'R' in self.cache
         assert b'sa' in self.cache
-        assert self.queue.qsize() == 2
-        sa = self.queue.get(False)
-        R = self.queue.get(False)
+        assert len(self.stack) == 2
+        sa = self.stack.get()
+        R = self.stack.get()
         assert len(sa) == 32 and sa not in (seed, T, m)
         assert len(R) == 32 and R not in (seed, T, m)
 
-    def test_OP_MAKE_ADAPTER_SIG_PRIVATE_takes_3_from_and_puts_3_on_queue(self):
+    def test_OP_MAKE_ADAPTER_SIG_PRIVATE_takes_3_from_and_puts_3_on_stack(self):
         seed1 = token_bytes(32)
         seed2 = token_bytes(32)
         m = b'hello world'
-        self.queue.put(m)
-        self.queue.put(seed2)
-        self.queue.put(seed1)
+        self.stack.put(m)
+        self.stack.put(seed2)
+        self.stack.put(seed1)
         functions.set_tape_flags(self.tape)
-        functions.OP_MAKE_ADAPTER_SIG_PRIVATE(self.tape, self.queue, self.cache)
+        functions.OP_MAKE_ADAPTER_SIG_PRIVATE(self.tape, self.stack, self.cache)
         assert b't' in self.cache
         assert b'T' in self.cache
         assert b'R' in self.cache
         assert b'sa' in self.cache
-        assert self.queue.qsize() == 3
-        sa = self.queue.get(False)
-        R = self.queue.get(False)
-        T = self.queue.get(False)
+        assert len(self.stack) == 3
+        sa = self.stack.get()
+        R = self.stack.get()
+        T = self.stack.get()
         assert len(sa) == 32 and sa not in (seed1, seed2, m)
         assert len(T) == 32 and T not in (seed1, seed2, m)
         assert len(R) == 32 and R not in (seed1, seed2, m)
 
-    def test_OP_CHECK_ADAPTER_SIG_takes_5_from_and_puts_1_on_queue(self):
+    def test_OP_CHECK_ADAPTER_SIG_takes_5_from_and_puts_1_on_stack(self):
         R = functions.derive_point_from_scalar(
             functions.derive_key_from_seed(token_bytes(32))
         )
         T = functions.derive_point_from_scalar(
             functions.derive_key_from_seed(token_bytes(32))
         )
         # sa = functions.clamp_scalar(token_bytes(32))
         sa = token_bytes(32)
         m = b'hello world'
         X = functions.derive_point_from_scalar(
             functions.derive_key_from_seed(token_bytes(32))
         )
-        self.queue.put(sa)
-        self.queue.put(R)
-        self.queue.put(m)
-        self.queue.put(T)
-        self.queue.put(X)
-        functions.OP_CHECK_ADAPTER_SIG(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        assert self.queue.get(False) == b'\x00'
+        self.stack.put(sa)
+        self.stack.put(R)
+        self.stack.put(m)
+        self.stack.put(T)
+        self.stack.put(X)
+        functions.OP_CHECK_ADAPTER_SIG(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        assert self.stack.get() == b'\x00'
 
     def test_OP_MAKE_ADAPTER_SIG_and_OP_VALIDATE_ADAPTER_SIG_e2e(self):
         seed = token_bytes(32)
         T = functions.derive_point_from_scalar(
             functions.derive_key_from_seed(token_bytes(32))
         )
         X = bytes(SigningKey(seed).verify_key)
         m = b'hello world'
-        self.queue.put(seed)
-        self.queue.put(m)
-        self.queue.put(T)
-        functions.OP_MAKE_ADAPTER_SIG_PUBLIC(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 2
-        sa = self.queue.get(False)
-        R = self.queue.get(False)
+        self.stack.put(seed)
+        self.stack.put(m)
+        self.stack.put(T)
+        functions.OP_MAKE_ADAPTER_SIG_PUBLIC(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 2
+        sa = self.stack.get()
+        R = self.stack.get()
 
         # positive case
-        self.queue.put(sa)
-        self.queue.put(R)
-        self.queue.put(m)
-        self.queue.put(T)
-        self.queue.put(X)
-        functions.OP_CHECK_ADAPTER_SIG(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        assert self.queue.get(False) == b'\xff'
+        self.stack.put(sa)
+        self.stack.put(R)
+        self.stack.put(m)
+        self.stack.put(T)
+        self.stack.put(X)
+        functions.OP_CHECK_ADAPTER_SIG(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        assert self.stack.get() == b'\xff'
 
         # negative case
-        self.queue.put(sa)
-        self.queue.put(R)
-        self.queue.put(m + b'qws')
-        self.queue.put(T)
-        self.queue.put(X)
-        functions.OP_CHECK_ADAPTER_SIG(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        assert self.queue.get(False) == b'\x00'
+        self.stack.put(sa)
+        self.stack.put(R)
+        self.stack.put(m + b'qws')
+        self.stack.put(T)
+        self.stack.put(X)
+        functions.OP_CHECK_ADAPTER_SIG(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        assert self.stack.get() == b'\x00'
 
     def test_OP_MAKE_ADAPTER_SIG_and_OP_DECRYPT_ADAPTER_SIG_e2e(self):
         seed1 = token_bytes(32)
         seed2 = token_bytes(32)
         t = functions.clamp_scalar(seed2)
         T = functions.derive_point_from_scalar(t)
         X = bytes(SigningKey(seed1).verify_key)
         m = b'hello world'
-        self.queue.put(seed1)
-        self.queue.put(m)
-        self.queue.put(T)
+        self.stack.put(seed1)
+        self.stack.put(m)
+        self.stack.put(T)
         functions.set_tape_flags(self.tape)
-        functions.OP_MAKE_ADAPTER_SIG_PUBLIC(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 2
-        sa = self.queue.get(False)
-        R = self.queue.get(False)
-
-        self.queue.put(sa)
-        self.queue.put(R)
-        self.queue.put(seed2)
-        functions.OP_DECRYPT_ADAPTER_SIG(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 2
+        functions.OP_MAKE_ADAPTER_SIG_PUBLIC(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 2
+        sa = self.stack.get()
+        R = self.stack.get()
+
+        self.stack.put(sa)
+        self.stack.put(R)
+        self.stack.put(seed2)
+        functions.OP_DECRYPT_ADAPTER_SIG(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 2
         assert b's' in self.cache
         assert b'RT' in self.cache
-        RT = self.queue.get(False)
-        s = self.queue.get(False)
+        s = self.stack.get()
+        RT = self.stack.get()
 
         # check signature
         self.cache['sigfield1'] = m
         self.tape = classes.Tape(b'\x00')
         functions.set_tape_flags(self.tape)
-        self.queue.put(RT + s)
-        self.queue.put(X)
-        functions.OP_CHECK_SIG(self.tape, self.queue, self.cache)
-        assert self.queue.qsize() == 1
-        assert self.queue.get(False) == b'\xff'
-
-    # cryptographic proofs
-    def test_ed25519_maths_meet_homomorphic_one_way_condition(self):
-        """Test if Ed25519 meets the homomorphic one way condition."""
-        x1 = functions.clamp_scalar(token_bytes(32))
-        x2 = functions.clamp_scalar(token_bytes(32))
-        y1 = nacl.bindings.crypto_scalarmult_ed25519_base_noclamp(x1) # G^x1
-        y2 = nacl.bindings.crypto_scalarmult_ed25519_base_noclamp(x2) # G^x2
-
-        # test
-        y3_1 = nacl.bindings.crypto_core_ed25519_add(y1, y2) # G^x1 * G^x2
-        x3 = nacl.bindings.crypto_core_ed25519_scalar_add(x1, x2) # x1 + x2
-        y3_2 = nacl.bindings.crypto_scalarmult_ed25519_base_noclamp(x3) # G^(x1+x2)
-        assert y3_1 == y3_2 # G^x1 * G^x2 = G^(x1+x2) where * denotes group operator
+        self.stack.put(RT + s)
+        self.stack.put(X)
+        functions.OP_CHECK_SIG(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        assert self.stack.get() == b'\xff'
+
+    def test_OP_CHECK_TEMPLATE(self):
+        self.tape.data = b'\x01'
+        template = b'hello world'
+        self.stack.put(template)
+        self.cache = {'sigfield1': template}
+
+        functions.OP_CHECK_TEMPLATE(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        assert self.stack.get() == b'\xff'
+
+        self.tape.reset_pointer()
+        template = b'something else'
+        self.stack.put(template)
+
+        functions.OP_CHECK_TEMPLATE(self.tape, self.stack, self.cache)
+        assert len(self.stack) == 1
+        assert self.stack.get() == b'\x00'
+
+    def test_OP_TAPROOT(self):
+        # get keypair
+        seed = token_bytes(32)
+        skey = functions.derive_key_from_seed(seed)
+        pubk = functions.derive_point_from_scalar(skey)
+
+        # setup script
+        # script_src = 'push d1 less'
+        script_bin = b'\x01'
+        script_hash = sha256(pubk + sha256(script_bin).digest()).digest()
+        script_scalar = functions.clamp_scalar(script_hash)
+        script_point = functions.derive_point_from_scalar(script_scalar)
+
+        # combine pubk and script point
+        root = functions.aggregate_points([pubk, script_point])
+
+        tape = classes.Tape(root)
+        stack = classes.Stack()
+        cache = {'sigfield1': b'nope ', 'sigfield2': b'hello world'}
+
+        # create message and signature
+        message = cache['sigfield2']
+        sig = functions.sign_with_scalar(functions.aggregate_scalars([skey, script_scalar]), message)
+
+        # test unlock1 (key spend): should result in True value
+        tape.reset_pointer()
+        cache[b'trsf'] = [b'\x01']
+        assert len(stack) == 0
+        stack.put(sig + b'\x01')
+        functions.OP_TAPROOT(tape, stack, cache)
+        assert len(stack) == 1
+        assert stack.get() == b'\xff'
+
+        # test malformed unlock1: should result in False value
+        tape.reset_pointer()
+        stack.put(bytes(reversed(sig)))
+        functions.OP_TAPROOT(tape, stack, cache)
+        assert len(stack) == 1
+        assert stack.get() == b'\x00'
+
+        # test unlock2 (committed script): should result in True value
+        tape.reset_pointer()
+        stack.put(script_bin)
+        stack.put(pubk)
+        functions.OP_TAPROOT(tape, stack, cache)
+        assert len(stack) == 1
+        assert stack.get() == b'\xff'
+
+        # test malformed unlock2: should result in False value
+        tape.reset_pointer()
+        stack.put(script_bin + b'\x01')
+        stack.put(pubk)
+        functions.OP_TAPROOT(tape, stack, cache)
+        assert len(stack) == 1
+        assert stack.get() == b'\x00'
 
     # values
     def test_opcodes_is_dict_mapping_ints_to_tuple_str_function(self):
         assert isinstance(functions.opcodes, dict)
         for key, value in functions.opcodes.items():
             assert type(key) is int
             assert type(value) is tuple
@@ -2098,132 +2172,105 @@
             assert type(value[0]) is int
             assert callable(value[1])
 
     # code running functions
     def test_run_tape_executes_ops_until_tape_has_terminated(self):
         code = bytes.fromhex('990099009900990099009900')
         self.tape = classes.Tape(code)
-        assert self.queue.empty()
+        assert self.stack.empty()
         assert not self.cache
-        functions.run_tape(self.tape, self.queue, self.cache)
+        functions.run_tape(self.tape, self.stack, self.cache)
         assert self.tape.has_terminated()
-        assert self.queue.empty()
+        assert self.stack.empty()
 
         code = bytes.fromhex('290000000202012a00')
         self.tape = classes.Tape(code)
-        assert self.queue.empty()
+        assert self.stack.empty()
         assert not self.cache
-        functions.run_tape(self.tape, self.queue, self.cache)
+        functions.run_tape(self.tape, self.stack, self.cache)
         assert self.tape.has_terminated()
-        assert not self.queue.empty()
-        item = self.queue.get(False)
+        assert not self.stack.empty()
+        item = self.stack.get()
         assert item == b'\xff'
-        item = self.queue.get(False)
+        item = self.stack.get()
         assert item == b'\x02'
 
-    def test_run_script_returns_tuple_of_tape_queue_and_cache(self):
+    def test_run_script_returns_tuple_of_tape_stack_and_cache(self):
         code = bytes.fromhex('990099009900990099009900')
         result = functions.run_script(code)
         assert isinstance(result, tuple)
         assert len(result) == 3
         assert isinstance(result[0], classes.Tape)
-        assert isinstance(result[1], LifoQueue)
+        assert isinstance(result[1], classes.Stack)
         assert isinstance(result[2], dict)
         assert result[0].has_terminated()
 
-    def test_run_auth_script_returns_True_only_if_queue_has_single_True_value(self):
+    def test_run_auth_script_returns_True_only_if_stack_has_single_True_value(self):
         assert functions.run_auth_script(b'\x00') == False
         assert functions.run_auth_script(b'\x00\x20') == False
         assert functions.run_auth_script(b'\x01') == True
         assert functions.run_auth_script(b'\x01\x01') == False
 
-    def test_infinite_recursion_results_in_callstack_limit_exceeded_error(self):
-        with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.run_script(b'\x29\x00\x00\x02\x2a\x00\x2a\x00')
-        assert str(e.exception) == 'callstack limit exceeded'
-
     def test_OP_RETURN_exits_local_context_and_returns_to_outer_context(self):
-        # return from def before adding int false to queue
+        # return from def before adding int false to stack
         code = b'\x29\x00\x00\x02\x30\x00\x2a\x00\x01'
-        tape, queue, _ = functions.run_script(code)
+        tape, stack, _ = functions.run_script(code)
         assert tape.has_terminated()
-        assert queue.get(False) == b'\xff'
-        assert queue.empty()
+        assert stack.get() == b'\xff'
+        assert stack.empty()
 
-        # return from def after adding int false to queue
+        # return from def after adding int false to stack
         code = b'\x29\x00\x00\x02\x00\x30\x2a\x00\x01'
-        tape, queue, _ = functions.run_script(code)
+        tape, stack, _ = functions.run_script(code)
         assert tape.has_terminated()
-        assert queue.get(False) == b'\xff'
-        assert queue.get(False) == b'\x00'
-        assert queue.empty()
+        assert stack.get() == b'\xff'
+        assert stack.get() == b'\x00'
+        assert stack.empty()
 
     def test_OP_RETURN_within_OP_IF_exits_outer_context(self):
-        # return from def within OP_IF before adding int false to queue
+        # return from def within OP_IF before adding int false to stack
         code = b'\x29\x00\x00\x06\x2b\x00\x02\x30\x00\x01\x01\x2a\x00\x02\x02'
-        tape, queue, _ = functions.run_script(code)
+        tape, stack, _ = functions.run_script(code)
         assert tape.has_terminated()
-        assert queue.get(False) == b'\x02'
-        assert queue.empty()
+        assert stack.get() == b'\x02'
+        assert stack.empty()
 
     def test_OP_RETURN_within_OP_IF_ELSE_exits_outer_context(self):
-        # return from def within OP_IF before adding int false to queue
+        # return from def within OP_IF before adding int false to stack
         code = b'\x29\x00\x00\x08\x2c\x00\x02\x30\x00\x00\x00\x01\x01\x2a\x00\x02\x02'
-        tape, queue, _ = functions.run_script(code)
+        tape, stack, _ = functions.run_script(code)
         assert tape.has_terminated()
-        assert queue.get(False) == b'\x02'
-        assert queue.empty()
+        assert stack.get() == b'\x02'
+        assert stack.empty()
 
     def test_OP_RETURN_within_OP_TRY_EXCEPT_exits_outer_context(self):
-        # return from def within OP_TRY_EXCEPT before adding int false to queue
+        # return from def within OP_TRY_EXCEPT before adding int false to stack
         code = b'\x29\x00\x00\x07\x3d\x00\x01\x30\x00\x00\x01\x2a\x00\x02\x02'
-        tape, queue, _ = functions.run_script(code)
+        tape, stack, _ = functions.run_script(code)
         assert tape.has_terminated()
-        assert queue.get(False) == b'\x02'
-        assert queue.empty()
+        assert stack.get() == b'\x02'
+        assert stack.empty()
 
     def test_OP_RETURN_within_OP_EVAL_does_not_exit_outer_context(self):
-        # do not return from def within OP_EVAL before adding \xff to queue
+        # do not return from def within OP_EVAL before adding \xff to stack
         code = b'\x29\x00\x00\x05' + b'\x02\x30\x2d\x02\xff' + b'\x2a\x00'
-        tape, queue, _ = functions.run_script(code)
+        tape, stack, _ = functions.run_script(code)
         assert tape.has_terminated()
-        assert queue.get(False) == b'\xff'
-        assert queue.empty()
+        assert stack.get() == b'\xff'
+        assert stack.empty()
 
     def test_OP_RETURN_within_OP_EVAL_exits_outer_context_when_eval_return_flag_set(self):
-        # return from def within OP_EVAL before adding \xff to queue
+        # return from def within OP_EVAL before adding \xff to stack
         code = b'\x29\x00\x00\x05' + b'\x02\x30\x2d\x02\xff' + b'\x2a\x00'
-        tape, queue, _ = functions.run_script(code, additional_flags={'eval_return':True})
+        tape, stack, _ = functions.run_script(code, additional_flags={'eval_return':True})
         assert tape.has_terminated()
-        assert queue.empty()
-
-    def test_OP_LOOP_and_recursive_OP_CALL_raises_callstack_limit_error(self):
-        """
-            OP_DEF 0 {
-                OP_LOOP {
-                    OP_CALL 0
-                }
-            }
-            OP_TRUE
-            OP_CALL 0
-        """
-        defbody = functions.opcodes_inverse['OP_LOOP'][0].to_bytes(1, 'big') + \
-            b'\x00\x02' + functions.opcodes_inverse['OP_CALL'][0].to_bytes(1, 'big') + \
-            b'\x00'
-        self.tape = classes.Tape(
-            functions.opcodes_inverse['OP_DEF'][0].to_bytes(1, 'big') +
-            b'\x00' + len(defbody).to_bytes(2, 'big') + defbody + b'\x01' +
-            functions.opcodes_inverse['OP_CALL'][0].to_bytes(1, 'big') + b'\x00'
-        )
-        with self.assertRaises(errors.ScriptExecutionError) as e:
-            functions.run_tape(self.tape, self.queue, self.cache)
-        assert 'callstack limit' in str(e.exception)
+        assert stack.empty()
 
     def test_add_opcode_raises_errors_for_invalid_input(self):
-        function = lambda tape, queue, cache: queue.put('nonsense')
+        function = lambda tape, stack, cache: stack.put('nonsense')
         with self.assertRaises(TypeError) as e:
             functions.add_opcode('not an int', '', function)
         assert str(e.exception) == 'code must be int'
         with self.assertRaises(TypeError) as e:
             functions.add_opcode(255, b'not str', function)
         assert str(e.exception) == 'name must be str'
         with self.assertRaises(TypeError) as e:
@@ -2236,26 +2283,26 @@
             functions.add_opcode(256, 'name', function)
         assert str(e.exception) == 'code must be <256'
         with self.assertRaises(ValueError) as e:
             functions.add_opcode(255, 'name', function)
         assert str(e.exception) == 'name must start with OP_'
 
     def test_add_opcode_adds_function_e2e(self):
-        self.queue.put('123')
-        functions.run_tape(classes.Tape(b'\xff\x01'), self.queue, {})
-        assert self.queue.empty()
+        self.stack.put(b'123')
+        functions.run_tape(classes.Tape(b'\xff\x01'), self.stack, {})
+        assert self.stack.empty()
 
-        functions.add_opcode(255, 'OP_NONSENSE', lambda tape, queue, cache: queue.put('nonsense'))
+        functions.add_opcode(255, 'OP_NONSENSE', lambda tape, stack, cache: stack.put(b'nonsense'))
         assert self.original_opcodes != functions.opcodes
         assert self.original_opcodes_inverse != functions.opcodes_inverse
 
-        tape, queue, cache = functions.run_script(b'\xff\x01')
-        assert not queue.empty()
-        assert queue.get(False) == b'\xff'
-        assert queue.get(False) == 'nonsense'
+        tape, stack, cache = functions.run_script(b'\xff\x01')
+        assert not stack.empty()
+        assert stack.get() == b'\xff'
+        assert stack.get() == b'nonsense'
 
     def test_add_contract_raises_error_on_invalid_contract(self):
         assert b'123' not in functions._contracts
         with self.assertRaises(errors.ScriptExecutionError) as e:
             functions.add_contract(b'123', InvalidContract(1))
         assert str(e.exception) == 'contract does not fulfill at least one interface'
         assert b'123' not in functions._contracts
@@ -2272,15 +2319,15 @@
         assert b'123' in functions._contracts
         functions.remove_contract(b'123')
         assert b'123' not in functions._contracts
 
     def test_added_contracts_added_to_executing_scripts(self):
         contract = ValidContract(10)
         functions.add_contract(b'123', contract)
-        tape, queue, cache = functions.run_script(b'\x00')
+        tape, stack, cache = functions.run_script(b'\x00')
         assert b'123' in tape.contracts
         assert tape.contracts[b'123'] is contract
 
     def test_add_contract_interface_raises_TypeError_for_invalid_interface(self):
         with self.assertRaises(TypeError) as e:
             functions.add_contract_interface({})
         assert str(e.exception) == 'interface must be a Protocol'
@@ -2329,28 +2376,28 @@
             locking_script = bytes.fromhex(hexdata)
             locking_script = locking_script.replace(old_ts, ts_bytes)
 
         with open('tests/vectors/p2pk_unlocking_script1.hex', 'r') as f:
             hexdata = ''.join(f.read().split())
             unlocking_script1 = bytes.fromhex(hexdata)
             script = unlocking_script1 + locking_script
-            tape, queue, _ = functions.run_script(script, cache_vals)
+            tape, stack, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
-            assert not queue.empty()
-            item = queue.get(False)
+            assert not stack.empty()
+            item = stack.get()
             assert item == b'\xff'
 
         with open('tests/vectors/p2pk_unlocking_script2.hex', 'r') as f:
             hexdata = ''.join(f.read().split())
             unlocking_script2 = bytes.fromhex(hexdata)
             script = unlocking_script2 + locking_script
-            tape, queue, _ = functions.run_script(script, cache_vals)
+            tape, stack, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
-            assert not queue.empty()
-            item = queue.get(False)
+            assert not stack.empty()
+            item = stack.get()
             assert item == b'\xff'
 
     def test_p2sh_e2e(self):
         message = b'spending bitcoinz or something'
         original_flags = {**functions.flags}
         # disable additional time check
         functions.flags['ts_threshold'] = 0
@@ -2364,18 +2411,18 @@
             hexdata = ''.join(f.read().split())
             locking_script = bytes.fromhex(hexdata)
 
         with open('tests/vectors/p2sh_unlocking_script.hex', 'r') as f:
             hexdata = ''.join(f.read().split())
             unlocking_script = bytes.fromhex(hexdata)
             script = unlocking_script + locking_script
-            tape, queue, _ = functions.run_script(script, cache_vals)
+            tape, stack, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
-            assert not queue.empty()
-            item = queue.get(False)
+            assert not stack.empty()
+            item = stack.get()
             assert item == b'\xff'
 
         functions.flags = original_flags
 
     def test_cds_e2e(self):
         original_flags = {**functions.flags}
         # disable additional time check
@@ -2456,28 +2503,28 @@
             hexdata = ''.join(f.read().split())
             locking_script = bytes.fromhex(hexdata)
 
         with open('tests/vectors/correspondent_unlocking_script1.hex', 'r') as f:
             hexdata = ''.join(f.read().split())
             unlocking_script = bytes.fromhex(hexdata)
             script = unlocking_script + locking_script
-            tape, queue, _ = functions.run_script(script, cache_vals)
+            tape, stack, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
-            assert not queue.empty()
-            item = queue.get(False)
+            assert not stack.empty()
+            item = stack.get()
             assert item == b'\xff'
 
         with open('tests/vectors/correspondent_unlocking_script2.hex', 'r') as f:
             hexdata = ''.join(f.read().split())
             unlocking_script = bytes.fromhex(hexdata)
             script = unlocking_script + locking_script
-            tape, queue, _ = functions.run_script(script, cache_vals)
+            tape, stack, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
-            assert not queue.empty()
-            item = queue.get(False)
+            assert not stack.empty()
+            item = stack.get()
             assert item == b'\xff'
 
         functions.flags = original_flags
 
     def test_merkleval_e2e(self):
         message = b'spending some coinz'
         original_flags = {**functions.flags}
@@ -2493,38 +2540,38 @@
             hexdata = ''.join(f.read().split())
             locking_script = bytes.fromhex(hexdata)
 
         with open('tests/vectors/merkleval_unlocking_script_a.hex', 'r') as f:
             hexdata = ''.join(f.read().split())
             unlocking_script = bytes.fromhex(hexdata)
             script = unlocking_script + locking_script
-            tape, queue, _ = functions.run_script(script, cache_vals)
+            tape, stack, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
-            assert not queue.empty()
-            item = queue.get(False)
+            assert not stack.empty()
+            item = stack.get()
             assert item == b'\xff'
 
         with open('tests/vectors/merkleval_unlocking_script_ba.hex', 'r') as f:
             hexdata = ''.join(f.read().split())
             unlocking_script = bytes.fromhex(hexdata)
             script = unlocking_script + locking_script
-            tape, queue, _ = functions.run_script(script, cache_vals)
+            tape, stack, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
-            assert not queue.empty()
-            item = queue.get(False)
+            assert not stack.empty()
+            item = stack.get()
             assert item == b'\xff'
 
         with open('tests/vectors/merkleval_unlocking_script_bb.hex', 'r') as f:
             hexdata = ''.join(f.read().split())
             unlocking_script = bytes.fromhex(hexdata)
             script = unlocking_script + locking_script
-            tape, queue, _ = functions.run_script(script, cache_vals)
+            tape, stack, _ = functions.run_script(script, cache_vals)
             assert tape.has_terminated()
-            assert not queue.empty()
-            item = queue.get(False)
+            assert not stack.empty()
+            item = stack.get()
             assert item == b'\xff'
 
         functions.flags = original_flags
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tapescript-0.4.1/tests/test_parsing.py` & `tapescript-0.5.0/tests/test_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,22 +131,14 @@
         assert 'values for OP_PUSH2 must be prefaced with' in str(e.exception)
 
         with self.assertRaises(ValueError) as e:
             parsing.compile_script('OP_DEF 0 { OP_PUSH2 dnotnumeric }')
         assert 'value prefaced by d must be decimal int' in str(e.exception)
 
         with self.assertRaises(errors.SyntaxError) as e:
-            parsing.compile_script('OP_DEF 0 { OP_PUSH4 asd }')
-        assert 'values for OP_PUSH4 must be prefaced with' in str(e.exception)
-
-        with self.assertRaises(ValueError) as e:
-            parsing.compile_script('OP_DEF 0 { OP_PUSH4 dnotnumeric }')
-        assert 'value prefaced by d must be decimal int' in str(e.exception)
-
-        with self.assertRaises(errors.SyntaxError) as e:
             parsing.compile_script('OP_DEF 0 { OP_DIV_FLOAT asd }')
         assert 'numeric args must be prefaced with' in str(e.exception)
 
         with self.assertRaises(ValueError) as e:
             parsing.compile_script('OP_DEF 0 { OP_DIV_FLOAT fnotnumeric }')
         assert 'value prefaced by' in str(e.exception)
         assert 'must be decimal float' in str(e.exception)
@@ -227,37 +219,37 @@
             'branching_e2e.src': 'branching_e2e.hex',
             'trydef.src': 'trydef.hex',
             'try_in_if.src': 'try_in_if.hex',
             'macros_and_variables.src': 'macros_and_variables.hex',
             'new_ops_0.4.0.src': 'new_ops_0.4.0.hex',
             'new_if_hoist_syntax_0.4.0.src': 'new_if_hoist_syntax_0.4.0.hex',
         }
-        vectors = {}
-        names = {}
+        vectors = []
         errors = []
 
         for src_fname, hex_fname in vector_files.items():
             with open(f'tests/vectors/{src_fname}', 'r') as fsrc:
                 with open(f'tests/vectors/{hex_fname}', 'r') as fhex:
                     src = fsrc.read()
                     hex = ''.join(fhex.read().split())
-                    vectors[src] = hex
-                    names[hex] = src_fname
+                    vectors.append((src, hex, src_fname))
 
-        for src, hex in vectors.items():
+        for vector in vectors:
+            src, hex, name = vector
             expected = hex
-            current = names[hex]
+            if name == 'omega_e2e.src':
+                ...
             try:
                 observed = parsing.compile_script(src).hex()
             except BaseException as e:
-                errors.append(f"test_compile_script_e2e_vector: error with {current}: {e}")
+                errors.append(f"test_compile_script_e2e_vector: error with {name}: {e}")
                 continue
             if expected != observed:
                 # just to make it easier to step through the broken test vectors
-                print(f"{names[hex]} compilation failed")
+                print(f"{name} compilation failed")
                 observed = parsing.compile_script(src).hex()
                 print(expected)
                 print(observed)
                 diff = ''
                 if len(observed) > len(expected):
                     for i in range(len(observed)):
                         if i >= len(expected):
@@ -275,18 +267,21 @@
                 else:
                     print(
                         self.bytes_xor(
                             bytes.fromhex(expected),
                             bytes.fromhex(observed)
                         ).hex()
                     )
-            assert expected == observed
+            assert expected == observed, \
+                f'{name}\nobserved\n{observed}\n\nexpected\n{expected}' + \
+                f'\n\ndiff\n' + \
+                self.bytes_xor(bytes.fromhex(expected), bytes.fromhex(observed)).hex()
 
         assert len(errors) == 0, f'errors encountered: {errors}'
-        print(f'{len(vectors.items())} vectors tested for compile_script')
+        print(f'{len(vectors)} vectors tested for compile_script')
 
     def test_decompile_script_returns_list_of_str(self):
         code = parsing.decompile_script(b'\x00')
         assert type(code) is list
         assert code == ['OP_FALSE']
 
     def test_decompile_script_e2e_vectors(self):
@@ -544,17 +539,18 @@
 
         result = bytearray(len(first))
         for i in range(len(first)):
             result[i] = first[i] ^ second[i]
 
         return bytes(result)
 
-    def line_diff(self, first: str, second: str) -> None:
+    def line_diff(self, first: str, second: str) -> str:
         diff = ''
         if len(first) > len(second):
             for i in range(len(first)):
                 if i >= len(second):
                     diff += first[i]
+        return diff
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tapescript-0.4.1/tests/test_tools.py` & `tapescript-0.5.0/tests/test_tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-from context import classes
-from context import errors
-from context import functions
-from context import parsing
-from context import tools
+from context import classes, errors, functions, parsing, tools
+from hashlib import sha256
 from nacl.signing import SigningKey, VerifyKey
-from queue import LifoQueue
 from secrets import token_bytes
 from time import time
 import nacl.bindings
 import unittest
 
 
 class TestTools(unittest.TestCase):
@@ -60,117 +56,182 @@
 
         opnames = [name for name in parsing.additional_opcodes]
         for opname in opnames:
             del parsing.additional_opcodes[opname]
 
         return super().tearDown()
 
-    def test_create_merklized_script_returns_tuple_of_str_and_list(self):
-        result = tools.create_merklized_script(['OP_PUSH d123'])
+    def test_Script_class_e2e(self):
+        src1, src2 = '', ''
+        code1, code2 = b'', b''
+        decompiled1, decompiled2 = '', ''
+
+        # get test vectors
+        with open('tests/vectors/4.src', 'r') as f:
+            src1 = f.read()
+        with open('tests/vectors/4_decompiled.src', 'r') as f:
+            decompiled1 = f.read()
+        with open('tests/vectors/4.hex', 'r') as f:
+            code1 = bytes.fromhex(''.join(f.read().split()))
+        with open('tests/vectors/5.src', 'r') as f:
+            src2 = f.read()
+        with open('tests/vectors/5_decompiled.src', 'r') as f:
+            decompiled2 = f.read()
+        with open('tests/vectors/5.hex', 'r') as f:
+            code2 = bytes.fromhex(''.join(f.read().split()))
+
+        # create scripts from src vectors
+        script1 = tools.Script.from_src(src1)
+        script2 = tools.Script.from_src(src2)
+
+        # test compilation was correct
+        assert script1.bytes == code1
+        assert script2.bytes == code2
+
+        # test addition
+        script3 = script1 + script2
+        assert script1.src in script3.src
+        assert script2.src in script3.src
+        assert script3.bytes == script1.bytes + script2.bytes
+
+        # create scripts from bytes vectors
+        script1 = tools.Script.from_bytes(code1)
+        script2 = tools.Script.from_bytes(code2)
+
+        # test decompilation was correct
+        assert script1.src == decompiled1, f'{script1.src=}\n\n{decompiled1=}'
+        assert script2.src == decompiled2, f'{script2.src=}\n\n{decompiled2=}'
+
+    def test_merklized_script_tree_classes_e2e(self):
+        tree = tools.ScriptNode(
+            tools.ScriptNode(
+                tools.ScriptLeaf.from_src('push s"hello world"'),
+                tools.ScriptLeaf.from_src('true'),
+            ),
+            tools.ScriptNode(
+                tools.ScriptLeaf.from_src('push s"hello world"'),
+                tools.ScriptLeaf.from_src('true'),
+            )
+        )
+
+        unlock = tree.right.right.unlocking_script()
+        assert type(unlock) is tools.Script
+
+        lock = tree.locking_script()
+        assert type(lock) is tools.Script
+        assert functions.run_auth_script(unlock.bytes + lock.bytes)
+
+        packed = tree.pack()
+        unpacked = tools.ScriptNode.unpack(packed)
+        assert unpacked.locking_script().bytes == lock.bytes
+
+    def test_create_merklized_script_prioritized_returns_tuple_of_Script_and_list_of_Scripts(self):
+        result = tools.create_merklized_script_prioritized(['OP_PUSH d123'])
         assert type(result) is tuple
         assert len(result) == 2
 
         # locking script
-        assert type(result[0]) is str
-        parts = result[0].split()
+        assert type(result[0]) is tools.Script
+        parts = result[0].src.split()
         assert len(parts) == 2
         assert parts[0] == 'OP_MERKLEVAL'
         assert parts[1][0] == 'x'
         assert len(parts[1]) == 65
 
         # unlocking scripts
         assert type(result[1]) is list
         assert len(result[1]) == 2 # given branch + filler
         for unlocking_script in result[1]:
-            assert type(unlocking_script) is str
+            assert type(unlocking_script) is tools.Script
 
-    def test_create_merklized_script_1_branch_e2e(self):
-        result = tools.create_merklized_script(['OP_PUSH d123'])
-        locking_script = parsing.compile_script(result[0])
-        unlocking_script = parsing.compile_script(result[1][0])
+    def test_create_merklized_script_prioritized_1_branch_e2e(self):
+        lock, unlocks = tools.create_merklized_script_prioritized(['OP_PUSH d123'])
+        locking_script = lock.bytes
+        unlocking_script = unlocks[0].bytes
 
-        tape, queue, cache = functions.run_script(unlocking_script + locking_script)
+        tape, stack, cache = functions.run_script(unlocking_script + locking_script)
         assert tape.has_terminated()
-        assert not queue.empty()
-        assert int.from_bytes(queue.get(False), 'big') == 123
-        assert queue.empty()
-
-    def test_create_merklized_script_2_branches_e2e(self):
-        result = tools.create_merklized_script(['OP_PUSH d123', 'OP_PUSH x0123'])
-        locking_script = parsing.compile_script(result[0])
-        unlocking_scripts = [parsing.compile_script(s) for s in result[1]]
+        assert not stack.empty()
+        item = stack.get()
+        assert int.from_bytes(item, 'big') == 123, item.hex()
+        assert stack.empty()
+
+    def test_create_merklized_script_prioritized_2_branches_e2e(self):
+        lock, unlocks = tools.create_merklized_script_prioritized(['OP_PUSH d123', 'OP_PUSH x0123'])
+        locking_script = lock.bytes
+        unlocking_scripts = [s.bytes for s in unlocks]
         assert len(unlocking_scripts) == 2
 
-        tape, queue, cache = functions.run_script(unlocking_scripts[0] + locking_script)
+        tape, stack, cache = functions.run_script(unlocking_scripts[0] + locking_script)
         assert tape.has_terminated()
-        assert not queue.empty()
-        assert int.from_bytes(queue.get(False), 'big') == 123
-        assert queue.empty()
+        assert not stack.empty()
+        assert int.from_bytes(stack.get(), 'big') == 123
+        assert stack.empty()
 
-        tape, queue, cache = functions.run_script(unlocking_scripts[1] + locking_script)
+        tape, stack, cache = functions.run_script(unlocking_scripts[1] + locking_script)
         assert tape.has_terminated()
-        assert not queue.empty()
-        assert queue.get(False) == b'\x01\x23'
-        assert queue.empty()
+        assert not stack.empty()
+        assert stack.get() == b'\x01\x23'
+        assert stack.empty()
 
-    def test_create_merklized_script_3_branches_e2e(self):
-        result = tools.create_merklized_script([
+    def test_create_merklized_script_prioritized_3_branches_e2e(self):
+        lock, unlocks = tools.create_merklized_script_prioritized([
             'OP_PUSH d123', 'OP_PUSH x0123', 'OP_PUSH s"hello world"'
         ])
-        locking_script = parsing.compile_script(result[0])
-        unlocking_scripts = [parsing.compile_script(s) for s in result[1]]
+        locking_script = lock.bytes
+        unlocking_scripts = [s.bytes for s in unlocks]
         assert len(unlocking_scripts) == 3
 
-        tape, queue, cache = functions.run_script(unlocking_scripts[0] + locking_script)
+        tape, stack, cache = functions.run_script(unlocking_scripts[0] + locking_script)
         assert tape.has_terminated()
-        assert not queue.empty()
-        assert int.from_bytes(queue.get(False), 'big') == 123
-        assert queue.empty()
+        assert not stack.empty()
+        assert int.from_bytes(stack.get(), 'big') == 123
+        assert stack.empty()
 
-        tape, queue, cache = functions.run_script(unlocking_scripts[1] + locking_script)
+        tape, stack, cache = functions.run_script(unlocking_scripts[1] + locking_script)
         assert tape.has_terminated()
-        assert not queue.empty()
-        assert queue.get(False) == b'\x01\x23'
-        assert queue.empty()
+        assert not stack.empty()
+        assert stack.get() == b'\x01\x23'
+        assert stack.empty()
 
-        tape, queue, cache = functions.run_script(unlocking_scripts[2] + locking_script)
+        tape, stack, cache = functions.run_script(unlocking_scripts[2] + locking_script)
         assert tape.has_terminated()
-        assert not queue.empty()
-        assert str(queue.get(False), 'utf-8') == 'hello world'
-        assert queue.empty()
+        assert not stack.empty()
+        assert str(stack.get(), 'utf-8') == 'hello world'
+        assert stack.empty()
 
-    def test_create_merklized_script_20_branches_e2e(self):
+    def test_create_merklized_script_prioritized_20_branches_e2e(self):
         scripts = [f'OP_PUSH d{i}' for i in range(20)]
-        result = tools.create_merklized_script(scripts)
-        locking_script = parsing.compile_script(result[0])
-        unlocking_scripts = [parsing.compile_script(s) for s in result[1]]
+        lock, unlocks = tools.create_merklized_script_prioritized(scripts)
+        locking_script = lock.bytes
+        unlocking_scripts = [s.bytes for s in unlocks]
         assert len(unlocking_scripts) == 20
 
         for i in range(20):
-            tape, queue, cache = functions.run_script(unlocking_scripts[i] + locking_script)
+            tape, stack, cache = functions.run_script(unlocking_scripts[i] + locking_script)
             assert tape.has_terminated()
-            assert not queue.empty()
-            assert int.from_bytes(queue.get(False), 'big') == i
-            assert queue.empty()
+            assert not stack.empty()
+            assert int.from_bytes(stack.get(), 'big') == i
+            assert stack.empty()
 
     def test_add_soft_fork_e2e(self):
         locking_script_old_src = 'NOP255 d3 OP_TRUE'
         locking_script_new_src = 'OP_CHECK_ALL_EQUAL_VERIFY d3 OP_TRUE'
         good_unlocking_script_src = 'OP_PUSH x0123 OP_PUSH x0123 OP_PUSH x0123'
         bad_unlocking_script_src = 'OP_PUSH x0123 OP_PUSH x0123 OP_PUSH x3210'
 
-        def OP_CHECK_ALL_EQUAL_VERIFY(tape: classes.Tape, queue: LifoQueue, cache: dict) -> None:
+        def OP_CHECK_ALL_EQUAL_VERIFY(tape: classes.Tape, stack: classes.Stack, cache: dict) -> None:
             """Replacement for NOP255: read the next bytes as uint count, take
-                that many items from queue, run checks, and raise an error if
+                that many items from stack, run checks, and raise an error if
                 any checks fail.
             """
             count = tape.read(1)[0]
             items = []
             for i in range(count):
-                items.append(queue.get(False))
+                items.append(stack.get())
 
             compare = items.pop()
             while len(items):
                 if items.pop() != compare:
                     raise errors.ScriptExecutionError('not all the same')
 
         locking_script_old = parsing.compile_script(locking_script_old_src)
@@ -192,42 +253,42 @@
 
     def test_add_soft_fork_merklized_script_e2e(self):
         locking_script_old_src = 'NOP255 d3 OP_TRUE'
         locking_script_new_src = 'OP_CHECK_ALL_EQUAL_VERIFY d3 OP_TRUE'
         good_unlocking_script_src = 'OP_PUSH x0123 OP_PUSH x0123 OP_PUSH x0123'
         bad_unlocking_script_src = 'OP_PUSH x0123 OP_PUSH x0123 OP_PUSH x3210'
 
-        def OP_CHECK_ALL_EQUAL_VERIFY(tape: classes.Tape, queue: LifoQueue, cache: dict) -> None:
+        def OP_CHECK_ALL_EQUAL_VERIFY(tape: classes.Tape, stack: classes.Stack, cache: dict) -> None:
             """Replacement for NOP255: read the next bytes as uint count, take
-                that many items from queue, run checks, and raise an error if
+                that many items from stack, run checks, and raise an error if
                 any checks fail.
             """
             count = tape.read(1)[0]
             items = []
             for i in range(count):
-                items.append(queue.get(False))
+                items.append(stack.get())
 
             compare = items.pop()
             while len(items):
                 if items.pop() != compare:
                     raise errors.ScriptExecutionError('not all the same')
 
         locking_script_old = parsing.compile_script(locking_script_old_src)
 
         # before soft fork activation
         good_scripts = [good_unlocking_script_src for i in range(20)]
         bad_scripts = [bad_unlocking_script_src for i in range(20)]
 
-        result = tools.create_merklized_script(good_scripts)
-        good_locking_script = parsing.compile_script(result[0])
-        good_unlocking_scripts = [parsing.compile_script(s) for s in result[1]]
-
-        result = tools.create_merklized_script(bad_scripts)
-        bad_locking_script = parsing.compile_script(result[0])
-        bad_unlocking_scripts = [parsing.compile_script(s) for s in result[1]]
+        result = tools.create_merklized_script_prioritized(good_scripts)
+        good_locking_script = result[0].bytes
+        good_unlocking_scripts = [s.bytes for s in result[1]]
+
+        result = tools.create_merklized_script_prioritized(bad_scripts)
+        bad_locking_script = result[0].bytes
+        bad_unlocking_scripts = [s.bytes for s in result[1]]
 
         for i in range(20):
             branch = good_unlocking_scripts[i] + good_locking_script + locking_script_old
             assert functions.run_auth_script(branch)
             branch = bad_unlocking_scripts[i] + bad_locking_script + locking_script_old
             assert functions.run_auth_script(branch)
 
@@ -237,77 +298,76 @@
         # after soft fork activation
         locking_script_new = parsing.compile_script(locking_script_new_src)
         assert locking_script_new == locking_script_old
 
         good_scripts = [good_unlocking_script_src for i in range(20)]
         bad_scripts = [bad_unlocking_script_src for i in range(20)]
 
-        result = tools.create_merklized_script(good_scripts)
-        good_locking_script = parsing.compile_script(result[0])
-        good_unlocking_scripts = [parsing.compile_script(s) for s in result[1]]
-
-        result = tools.create_merklized_script(bad_scripts)
-        bad_locking_script = parsing.compile_script(result[0])
-        bad_unlocking_scripts = [parsing.compile_script(s) for s in result[1]]
+        result = tools.create_merklized_script_prioritized(good_scripts)
+        good_locking_script = result[0].bytes
+        good_unlocking_scripts = [s.bytes for s in result[1]]
+
+        result = tools.create_merklized_script_prioritized(bad_scripts)
+        bad_locking_script = result[0].bytes
+        bad_unlocking_scripts = [s.bytes for s in result[1]]
 
         for i in range(20):
             branch = good_unlocking_scripts[i] + good_locking_script + locking_script_old
             assert functions.run_auth_script(branch)
             branch = bad_unlocking_scripts[i] + bad_locking_script + locking_script_old
             assert not functions.run_auth_script(branch)
 
     def test_make_adapter_locks_prv_and_make_adapter_witness_e2e(self):
         # setup lock and decrypt scripts
         tweak = token_bytes(32)
         scripts = tools.make_adapter_locks_prv(bytes(self.pubkeyA), tweak)
-        assert type(scripts) in (list, tuple) and len(scripts) == 3
-        script1_src, script2_src, script3_src = scripts
-        verify_adapter_lock = parsing.compile_script(script1_src)
-        decrypt_adapter_script = parsing.compile_script(script2_src)
-        check_sig_lock = parsing.compile_script(script3_src)
+        assert type(scripts) is tuple and len(scripts) == 3
+        script1, script2, script3 = scripts
+        verify_adapter_lock = script1.bytes
+        decrypt_adapter_script = script2.bytes
+        check_sig_lock = script3.bytes
         # make_adapter_locks_prv calls make_adapter_locks_pub and
         # make_adapter_decrypt under the hood, so this counts as testing both
 
         # setup adapter witness
         sigfields = {
             'sigfield1': b'hello world',
             'sigfield2': b'pay Bob 2 btc pls',
         }
         tweak_point = functions.derive_point_from_scalar(
             functions.clamp_scalar(tweak)
         )
-        witness_src = tools.make_adapter_witness(
+        witness = tools.make_adapter_witness(
             bytes(self.prvkeyA),
             tweak_point,
             sigfields
-        )
-        witness = tools.compile_script(witness_src)
+        ).bytes
 
         # run witness script
-        _, queue, _ = functions.run_script(witness, sigfields)
-        assert queue.qsize() == 2
-        R = queue.get(False)
-        sa = queue.get(False)
+        _, stack, _ = functions.run_script(witness, sigfields)
+        assert len(stack) == 2
+        R = stack.get()
+        sa = stack.get()
         assert nacl.bindings.crypto_core_ed25519_is_valid_point(R)
         assert len(sa) == 32
 
         # verify adapter witness with adapter verification script
         assert functions.run_auth_script(
             witness + verify_adapter_lock,
             sigfields
         )
 
         # decrypt signature from witness
-        _, queue, _ = functions.run_script(
+        _, stack, _ = functions.run_script(
             witness + decrypt_adapter_script,
             sigfields
         )
-        assert queue.qsize() == 2
-        RT = queue.get(False)
-        s = queue.get(False)
+        assert len(stack) == 2
+        s = stack.get()
+        RT = stack.get()
 
         # decrypt method 2
         assert tools.decrypt_adapter(witness, tweak) == RT + s
 
         # check the signature with the check_sig auth script
         assert functions.run_auth_script(
             parsing.compile_script(f'push x{(RT+s).hex()}') + check_sig_lock,
@@ -321,15 +381,15 @@
             sigfields
         )
 
     def test_make_adapter_lock_prv_and_make_adapter_witness_e2e(self):
         # setup lock and decrypt scripts
         tweak = token_bytes(32)
         script = tools.make_adapter_lock_prv(bytes(self.pubkeyA), tweak)
-        lock = parsing.compile_script(script)
+        lock = script.bytes
         # make_adapter_lock_prv calls make_adapter_lock_pub under the hood,
         # so this counts as testing both
 
         # setup adapter witness
         sigfields = {
             'sigfield1': b'hello world',
             'sigfield2': b'pay Bob 2 btc pls',
@@ -341,307 +401,367 @@
             bytes(self.prvkeyA),
             tweak_point,
             {**sigfields}
         )
         witness = tools.compile_script(f'push x{tweak.hex()} {witness_src}')
 
         # run witness script
-        _, queue, _ = functions.run_script(witness, {**sigfields})
-        assert queue.qsize() == 3
-        R = queue.get(False)
-        sa = queue.get(False)
-        t = queue.get(False)
+        _, stack, _ = functions.run_script(witness, {**sigfields})
+        assert len(stack) == 3
+        R = stack.get()
+        sa = stack.get()
+        t = stack.get()
         assert nacl.bindings.crypto_core_ed25519_is_valid_point(R)
         assert len(sa) == 32
         assert t == tweak
 
         # run combined auth script
         assert functions.run_auth_script(
             witness + lock,
             {**sigfields}
         )
 
+    def test_double_tweak_adapters_e2e(self):
+        t1 = functions.clamp_scalar(token_bytes(32))
+        t2 = functions.clamp_scalar(token_bytes(32))
+        T1 = functions.derive_point_from_scalar(t1)
+        T2 = functions.derive_point_from_scalar(t2)
+        tt = functions.aggregate_scalars([t1, t2])
+        TT = functions.aggregate_points([T1, T2])
+        assert TT == functions.derive_point_from_scalar(tt)
+
+        scripts1 = tools.make_adapter_locks_pub(bytes(self.pubkeyA), TT)
+        scripts2 = tools.make_adapter_locks_pub(bytes(self.pubkeyB), TT)
+
+        verify_adapter_1 = scripts1[0].bytes
+        verify_signature_1 = scripts1[1].bytes
+        verify_adapter_2 = scripts2[0].bytes
+        verify_signature_2 = scripts2[1].bytes
+
+        sigfields = {'sigfield1': b'we both get what we want'}
+        adapter_witness1 = tools.make_adapter_witness(bytes(self.prvkeyA), TT, sigfields).bytes
+        adapter_witness2 = tools.make_adapter_witness(bytes(self.prvkeyB), TT, sigfields).bytes
+
+        # verify adapters
+        assert functions.run_auth_script(adapter_witness1 + verify_adapter_1, sigfields)
+        assert functions.run_auth_script(adapter_witness2 + verify_adapter_2, sigfields)
+
+        # decrypt signatures
+        sig1 = tools.decrypt_adapter(adapter_witness1, tt)
+        sig2 = tools.decrypt_adapter(adapter_witness2, tt)
+
+        # verify signatures
+        assert functions.run_auth_script(
+            parsing.compile_script(f'push x{sig1.hex()}') + verify_signature_1,
+            sigfields
+        )
+        assert functions.run_auth_script(
+            parsing.compile_script(f'push x{sig2.hex()}') + verify_signature_2,
+            sigfields
+        )
+
     def test_make_single_sig_lock_and_make_single_sig_witness_e2e(self):
         # make lock
         sigfields = {'sigfield1': b'hello world'}
-        lock_src = tools.make_single_sig_lock(bytes(self.pubkeyA))
-        lock = parsing.compile_script(lock_src)
+        lock = tools.make_single_sig_lock(bytes(self.pubkeyA)).bytes
 
         # make witness
-        unlock_src = tools.make_single_sig_witness(bytes(self.prvkeyA), {**sigfields})
-        unlock = parsing.compile_script(unlock_src)
+        unlock = tools.make_single_sig_witness(bytes(self.prvkeyA), {**sigfields}).bytes
 
         # run e2e
         assert functions.run_auth_script(unlock + lock, {**sigfields})
 
     def test_make_single_sig_lock2_and_make_single_sig_witness2_e2e(self):
         # make lock
         sigfields = {'sigfield1': b'hello world'}
-        lock_src = tools.make_single_sig_lock2(bytes(self.pubkeyA))
-        lock = parsing.compile_script(lock_src)
+        lock = tools.make_single_sig_lock2(bytes(self.pubkeyA))
 
         # make witness
-        unlock_src = tools.make_single_sig_witness2(bytes(self.prvkeyA), {**sigfields})
-        unlock = parsing.compile_script(unlock_src)
+        unlock = tools.make_single_sig_witness2(bytes(self.prvkeyA), {**sigfields})
 
         # run e2e
-        assert functions.run_auth_script(unlock + lock, {**sigfields})
+        assert functions.run_auth_script(unlock.bytes + lock.bytes, {**sigfields})
 
     def test_make_multi_sig_lock_and_make_single_sig_witness_e2e(self):
         # make lock
         sigfields = {'sigfield1': b'hello world'}
-        lock_src = tools.make_multisig_lock(
-            [bytes(self.pubkeyA), bytes(self.pubkeyB)], 2, 'f0')
-        lock = parsing.compile_script(lock_src)
+        lock = tools.make_multisig_lock(
+            [bytes(self.pubkeyA), bytes(self.pubkeyB)], 2, 'f0'
+        )
 
         # make witness
-        unlock_src1 = tools.make_single_sig_witness(bytes(self.prvkeyA), {**sigfields}, 'f0')
-        unlock_src2 = tools.make_single_sig_witness(bytes(self.prvkeyB), {**sigfields}, 'f0')
-        unlock = parsing.compile_script(unlock_src1) + parsing.compile_script(unlock_src2)
+        unlock1 = tools.make_single_sig_witness(bytes(self.prvkeyA), {**sigfields}, 'f0')
+        unlock2 = tools.make_single_sig_witness(bytes(self.prvkeyB), {**sigfields}, 'f0')
+        unlock = unlock1.bytes + unlock2.bytes
 
         # run e2e
-        assert functions.run_auth_script(unlock + lock, {**sigfields})
+        assert functions.run_auth_script(unlock + lock.bytes, {**sigfields})
 
     def test_make_delegate_key_lock_e2e(self):
-        lock_src = tools.make_delegate_key_lock(bytes(self.pubkeyA))
-        lock = parsing.compile_script(lock_src)
+        lock = tools.make_delegate_key_lock(bytes(self.pubkeyA))
 
         begin_ts = int(time()) - 120
         end_ts = int(time()) + 120
         cert_sig = tools.make_delegate_key_cert_sig(
             bytes(self.prvkeyA), bytes(self.pubkeyB), begin_ts, end_ts
         )
         assert type(cert_sig) is bytes
         assert len(cert_sig) == 64
 
         cache = {'sigfield1': b'hello world'}
 
-        unlock_src = tools.make_delegate_key_unlock(
+        unlock = tools.make_delegate_key_unlock(
             bytes(self.prvkeyB), bytes(self.pubkeyB), begin_ts, end_ts,
             cert_sig, cache
         )
-        unlock = parsing.compile_script(unlock_src)
 
         # run e2e
-        assert functions.run_auth_script(unlock + lock, cache)
+        assert functions.run_auth_script(unlock.bytes + lock.bytes, cache)
 
     def test_make_htlc_sha256_lock_e2e(self):
         preimage = token_bytes(16)
         sigfields = {'sigfield1': b'hello world'}
         # NB: ts_threshold is 60, preventing timestamps >60s into future from verifying
         timeout = 30
-        lock_src = tools.make_htlc_sha256_lock(
+        lock = tools.make_htlc_sha256_lock(
             receiver_pubkey=bytes(self.pubkeyB),
             preimage=preimage,
             refund_pubkey=bytes(self.pubkeyA),
             timeout=timeout
         )
-        lock = parsing.compile_script(lock_src)
 
-        hash_unlock_src = tools.make_htlc_witness(
+        hash_unlock = tools.make_htlc_witness(
             prvkey=bytes(self.prvkeyB),
             preimage=preimage,
             sigfields=sigfields
         )
-        hash_unlock = parsing.compile_script(hash_unlock_src)
-        refund_unlock_src = tools.make_htlc_witness(
+        refund_unlock = tools.make_htlc_witness(
             bytes(self.prvkeyA), b'refund', sigfields
         )
-        refund_unlock = parsing.compile_script(refund_unlock_src)
 
         # test that the refund will not work yet
-        assert not functions.run_auth_script(refund_unlock + lock, sigfields)
+        assert not functions.run_auth_script(refund_unlock.bytes + lock.bytes, sigfields)
 
         # test that the main path works
-        assert functions.run_auth_script(hash_unlock + lock, sigfields)
+        assert functions.run_auth_script(hash_unlock.bytes + lock.bytes, sigfields)
 
         # test that the refund will work if the timestamp is past the timeout
         assert functions.run_auth_script(
-            refund_unlock + lock,
+            refund_unlock.bytes + lock.bytes,
             {**sigfields, 'timestamp': int(time()) + timeout + 1}
         )
 
     def test_make_htlc_shake256_lock_e2e(self):
         preimage = token_bytes(16)
         sigfields = {'sigfield1': b'hello world'}
         # NB: ts_threshold is 60, preventing timestamps >60s into future from verifying
         timeout = 30
-        lock_src = tools.make_htlc_shake256_lock(
+        lock = tools.make_htlc_shake256_lock(
             receiver_pubkey=bytes(self.pubkeyB),
             preimage=preimage,
             refund_pubkey=bytes(self.pubkeyA),
             timeout=timeout
         )
-        lock = parsing.compile_script(lock_src)
 
-        hash_unlock_src = tools.make_htlc_witness(
+        hash_unlock = tools.make_htlc_witness(
             prvkey=bytes(self.prvkeyB),
             preimage=preimage,
             sigfields=sigfields
         )
-        hash_unlock = parsing.compile_script(hash_unlock_src)
-        refund_unlock_src = tools.make_htlc_witness(
+        refund_unlock = tools.make_htlc_witness(
             bytes(self.prvkeyA), b'refund', sigfields
         )
-        refund_unlock = parsing.compile_script(refund_unlock_src)
 
         # test that the refund will not work yet
-        assert not functions.run_auth_script(refund_unlock + lock, sigfields)
+        assert not functions.run_auth_script(refund_unlock.bytes + lock.bytes, sigfields)
 
         # test that the main path works
-        assert functions.run_auth_script(hash_unlock + lock, sigfields)
+        assert functions.run_auth_script(hash_unlock.bytes + lock.bytes, sigfields)
 
         # test that the refund will work if the timestamp is past the timeout
         assert functions.run_auth_script(
-            refund_unlock + lock,
+            refund_unlock.bytes + lock.bytes,
             {**sigfields, 'timestamp': int(time()) + timeout + 1}
         )
 
     def test_make_htlc2_sha256_lock_e2e(self):
         preimage = token_bytes(16)
         sigfields = {'sigfield1': b'hello world'}
         # NB: ts_threshold is 60, preventing timestamps >60s into future from verifying
         timeout = 30
-        lock_src = tools.make_htlc2_sha256_lock(
+        lock = tools.make_htlc2_sha256_lock(
             receiver_pubkey=bytes(self.pubkeyB),
             preimage=preimage,
             refund_pubkey=bytes(self.pubkeyA),
             timeout=timeout
         )
-        lock = parsing.compile_script(lock_src)
 
-        hash_unlock_src = tools.make_htlc2_witness(
+        hash_unlock = tools.make_htlc2_witness(
             prvkey=bytes(self.prvkeyB),
             preimage=preimage,
             sigfields=sigfields
         )
-        hash_unlock = parsing.compile_script(hash_unlock_src)
-        refund_unlock_src = tools.make_htlc2_witness(
+        refund_unlock = tools.make_htlc2_witness(
             bytes(self.prvkeyA), b'refund', sigfields
         )
-        refund_unlock = parsing.compile_script(refund_unlock_src)
 
         # test that the refund will not work yet
-        assert not functions.run_auth_script(refund_unlock + lock, sigfields)
+        assert not functions.run_auth_script(refund_unlock.bytes + lock.bytes, sigfields)
 
         # test that the main path works
-        assert functions.run_auth_script(hash_unlock + lock, sigfields)
+        assert functions.run_auth_script(hash_unlock.bytes + lock.bytes, sigfields)
 
         # test that the refund will work if the timestamp is past the timeout
         assert functions.run_auth_script(
-            refund_unlock + lock,
+            refund_unlock.bytes + lock.bytes,
             {**sigfields, 'timestamp': int(time()) + timeout + 1}
         )
 
     def test_make_htlc2_shake256_lock_e2e(self):
         preimage = token_bytes(16)
         sigfields = {'sigfield1': b'hello world'}
         # NB: ts_threshold is 60, preventing timestamps >60s into future from verifying
         timeout = 30
-        lock_src = tools.make_htlc2_shake256_lock(
+        lock = tools.make_htlc2_shake256_lock(
             receiver_pubkey=bytes(self.pubkeyB),
             preimage=preimage,
             refund_pubkey=bytes(self.pubkeyA),
             timeout=timeout
         )
-        lock = parsing.compile_script(lock_src)
 
-        hash_unlock_src = tools.make_htlc2_witness(
+        hash_unlock = tools.make_htlc2_witness(
             prvkey=bytes(self.prvkeyB),
             preimage=preimage,
             sigfields=sigfields
         )
-        hash_unlock = parsing.compile_script(hash_unlock_src)
-        refund_unlock_src = tools.make_htlc2_witness(
+        refund_unlock = tools.make_htlc2_witness(
             bytes(self.prvkeyA), b'refund', sigfields
         )
-        refund_unlock = parsing.compile_script(refund_unlock_src)
 
         # test that the refund will not work yet
-        assert not functions.run_auth_script(refund_unlock + lock, sigfields)
+        assert not functions.run_auth_script(refund_unlock.bytes + lock.bytes, sigfields)
 
         # test that the main path works
-        assert functions.run_auth_script(hash_unlock + lock, sigfields)
+        assert functions.run_auth_script(hash_unlock.bytes + lock.bytes, sigfields)
 
         # test that the refund will work if the timestamp is past the timeout
         assert functions.run_auth_script(
-            refund_unlock + lock,
+            refund_unlock.bytes + lock.bytes,
             {**sigfields, 'timestamp': int(time()) + timeout + 1}
         )
 
     def test_make_ptlc_lock_e2e(self):
         sigfields = {'sigfield1': b'hello world'}
         # NB: ts_threshold is 60, preventing timestamps >60s into future from verifying
         timeout = 30
-        lock_src = tools.make_ptlc_lock(
+        lock = tools.make_ptlc_lock(
             receiver_pubkey=bytes(self.pubkeyB),
             refund_pubkey=bytes(self.pubkeyA),
             timeout=timeout
         )
-        lock = parsing.compile_script(lock_src)
 
-        unlock_src = tools.make_ptlc_witness(
+        unlock = tools.make_ptlc_witness(
             prvkey=bytes(self.prvkeyB),
             sigfields=sigfields
         )
-        unlock = parsing.compile_script(unlock_src)
-        refund_unlock_src = tools.make_ptlc_refund_witness(
+        refund_unlock = tools.make_ptlc_refund_witness(
             bytes(self.prvkeyA), sigfields
         )
-        refund_unlock = parsing.compile_script(refund_unlock_src)
 
         # test that the refund will not work yet
-        assert not functions.run_auth_script(refund_unlock + lock, sigfields)
+        assert not functions.run_auth_script(refund_unlock.bytes + lock.bytes, sigfields)
 
         # test that the main path works
-        assert functions.run_auth_script(unlock + lock, sigfields)
+        assert functions.run_auth_script(unlock.bytes + lock.bytes, sigfields)
 
         # test that the refund will work if the timestamp is past the timeout
         assert functions.run_auth_script(
-            refund_unlock + lock,
+            refund_unlock.bytes + lock.bytes,
             {**sigfields, 'timestamp': int(time()) + timeout + 1}
         )
 
     def test_make_ptlc_lock_with_tweak_e2e(self):
         tweak_scalar = functions.clamp_scalar(token_bytes(32), True)
         tweak_point = functions.derive_point_from_scalar(tweak_scalar)
         sigfields = {'sigfield1': b'hello world'}
         # NB: ts_threshold is 60, preventing timestamps >60s into future from verifying
         timeout = 30
-        lock_src = tools.make_ptlc_lock(
+        lock = tools.make_ptlc_lock(
             receiver_pubkey=bytes(self.pubkeyB),
             refund_pubkey=bytes(self.pubkeyA),
             tweak_point=tweak_point,
             timeout=timeout,
         )
-        lock = parsing.compile_script(lock_src)
 
-        unlock_src = tools.make_ptlc_witness(
+        unlock = tools.make_ptlc_witness(
             prvkey=bytes(self.prvkeyB),
             sigfields=sigfields,
             tweak_scalar=tweak_scalar,
         )
-        unlock = parsing.compile_script(unlock_src)
-        refund_unlock_src = tools.make_ptlc_refund_witness(
+        refund_unlock = tools.make_ptlc_refund_witness(
             bytes(self.prvkeyA), sigfields
         )
-        refund_unlock = parsing.compile_script(refund_unlock_src)
 
         # test that the refund will not work yet
-        assert not functions.run_auth_script(refund_unlock + lock, sigfields)
+        assert not functions.run_auth_script(refund_unlock.bytes + lock.bytes, sigfields)
 
         # test that the main path works
-        assert functions.run_auth_script(unlock + lock, sigfields)
+        assert functions.run_auth_script(unlock.bytes + lock.bytes, sigfields)
 
         # test that the refund will work if the timestamp is past the timeout
         assert functions.run_auth_script(
-            refund_unlock + lock,
+            refund_unlock.bytes + lock.bytes,
             {**sigfields, 'timestamp': int(time()) + timeout + 1}
         )
 
+    def test_make_taproot_lock_and_witnesses_e2e(self):
+        sigfields = {'sigfield1': b'hello ', 'sigfield2': b'world'}
+        script = tools.Script.from_src('true')
+        x = functions.derive_key_from_seed(bytes(self.prvkeyA))
+        X = bytes(self.pubkeyA)
+        t = functions.clamp_scalar(sha256(X + script.commitment()).digest())
+        T = functions.derive_point_from_scalar(t)
+        root = functions.aggregate_points((X, T))
+        sig = functions.sign_with_scalar(
+            functions.aggregate_scalars([x, t]),
+            b'hello world'
+        )
+
+        lock = tools.make_taproot_lock(X, script)
+        assert lock.src == f'taproot x{root.hex()}'
+
+        unlock1 = tools.make_taproot_witness_keyspend(
+            bytes(self.prvkeyA),
+            sigfields,
+            script
+        )
+        assert unlock1.src == f'push x{sig.hex()}', \
+            f'\nexpected push x{sig.hex()}\nobserved {unlock1.src}'
+
+        unlock2 = tools.make_taproot_witness_scriptspend(X, script)
+        assert unlock2.src == f'push x{script.bytes.hex()} push x{X.hex()}'
+
+        assert functions.run_auth_script(unlock1 + lock, sigfields)
+        assert functions.run_auth_script(unlock2 + lock, sigfields)
+
+        sig = functions.sign_with_scalar(
+            functions.aggregate_scalars((x, t)),
+            b'world'
+        )
+
+        unlock1 = tools.make_taproot_witness_keyspend(
+            bytes(self.prvkeyA),
+            sigfields,
+            script,
+            sigflags='01'
+        )
+        assert unlock1.src == f'@= trsf [ x01 ] push x{sig.hex()}01', \
+            f'\nexpected @= trsf [ x01 ] push x{sig.hex()}01\nobserved {unlock1.src}'
+        assert functions.run_auth_script(unlock1 + lock, sigfields)
+
     def test_AMHL_primitive(self):
         """Test for setup, locking, and release of an Anonymous Multi-
             Hop Lock using the homomorphic one-way ability of ed25519.
         """
         # first run the initial setup for 5 payers (4 intermediate)
         n = 5
         s = tools.AMHL.setup(n)
@@ -678,59 +798,55 @@
         assert 'key' in amhl
         sigfields = [
             {'sigfield1': b'pay Bob 1.2'},
             {'sigfield1': b'pay Carla 1.1'},
             {'sigfield1': b'pay Dave 1.0'},
         ]
 
-        adapter_witnesses_sources = [
+        adapter_witnesses = [
             tools.make_adapter_witness(prvkeys[i], amhl[pubkeys[i]][2], sigfields[i])
             for i in range(len(prvkeys))
         ]
-        adapter_witnesses = [
-            parsing.compile_script(ws)
-            for ws in adapter_witnesses_sources
-        ]
 
         # validate adapter witnesses
         for i in range(len(adapter_witnesses)):
             assert functions.run_auth_script(
-                adapter_witnesses[i] + parsing.compile_script(amhl[pubkeys[i]][0]),
+                adapter_witnesses[i].bytes + amhl[pubkeys[i]][0].bytes,
                 sigfields[i]
             )
 
         Alice = {
             'outbound_txn': {
                 'sigfields': sigfields[0],
                 'adapter_lock': amhl[pubkeys[0]][0],
-                'adapter_witness': adapter_witnesses[0],
-                'locking_script': parsing.compile_script(amhl[pubkeys[0]][1]),
+                'adapter_witness': adapter_witnesses[0].bytes,
+                'locking_script': amhl[pubkeys[0]][1].bytes,
             },
             'tweak_point': amhl[pubkeys[0]][2],
             'scalar': amhl[pubkeys[0]][3],
         }
 
         Bob = {
             'outbound_txn': {
                 'sigfields': sigfields[1],
                 'adapter_lock': amhl[pubkeys[1]][0],
-                'adapter_witness': adapter_witnesses[1],
-                'locking_script': parsing.compile_script(amhl[pubkeys[1]][1]),
+                'adapter_witness': adapter_witnesses[1].bytes,
+                'locking_script': amhl[pubkeys[1]][1].bytes,
             },
             'inbound_txn': Alice['outbound_txn'],
             'tweak_point': amhl[pubkeys[1]][2],
             'scalar': amhl[pubkeys[1]][3],
         }
 
         Carla = {
             'outbound_txn': {
                 'sigfields': sigfields[2],
                 'adapter_lock': amhl[pubkeys[2]][0],
-                'adapter_witness': adapter_witnesses[2],
-                'locking_script': parsing.compile_script(amhl[pubkeys[2]][1]),
+                'adapter_witness': adapter_witnesses[2].bytes,
+                'locking_script': amhl[pubkeys[2]][1].bytes,
             },
             'inbound_txn': Bob['outbound_txn'],
             'tweak_point': amhl[pubkeys[2]][2],
             'scalar': amhl[pubkeys[2]][3],
         }
 
         Dave = {
@@ -798,63 +914,59 @@
         ]
         refund_sigfields = [
             {'sigfield1': b'Alice takes back her 1.2 after timeout'},
             {'sigfield1': b'Bob takes back his 1.1 after timeout'},
             {'sigfield1': b'Carla takes back her 1.0 after timeout'},
         ]
 
-        adapter_witnesses_sources = [
+        adapter_witnesses = [
             tools.make_adapter_witness(prvkeys[i], amhl[pubkeys[i]][2], sigfields[i])
             for i in range(len(prvkeys))
         ]
-        adapter_witnesses = [
-            parsing.compile_script(ws)
-            for ws in adapter_witnesses_sources
-        ]
 
         # validate adapter witnesses
         for i in range(len(adapter_witnesses)):
             assert functions.run_auth_script(
-                adapter_witnesses[i] + parsing.compile_script(amhl[pubkeys[i]][0]),
+                adapter_witnesses[i].bytes + amhl[pubkeys[i]][0].bytes,
                 sigfields[i]
             )
 
         Alice = {
             'outbound_txn': {
                 'sigfields': sigfields[0],
                 'adapter_lock': amhl[pubkeys[0]][0],
-                'adapter_witness': adapter_witnesses[0],
-                'locking_script': parsing.compile_script(amhl[pubkeys[0]][1]),
+                'adapter_witness': adapter_witnesses[0].bytes,
+                'locking_script': amhl[pubkeys[0]][1].bytes,
             },
             'prvkey': prvkeys[0],
             'pubkey': pubkeys[0],
             'tweak_point': amhl[pubkeys[0]][2],
             'scalar': amhl[pubkeys[0]][3],
         }
 
         Bob = {
             'outbound_txn': {
                 'sigfields': sigfields[1],
                 'adapter_lock': amhl[pubkeys[1]][0],
-                'adapter_witness': adapter_witnesses[1],
-                'locking_script': parsing.compile_script(amhl[pubkeys[1]][1]),
+                'adapter_witness': adapter_witnesses[1].bytes,
+                'locking_script': amhl[pubkeys[1]][1].bytes,
             },
             'prvkey': prvkeys[1],
             'pubkey': pubkeys[1],
             'inbound_txn': Alice['outbound_txn'],
             'tweak_point': amhl[pubkeys[1]][2],
             'scalar': amhl[pubkeys[1]][3],
         }
 
         Carla = {
             'outbound_txn': {
                 'sigfields': sigfields[2],
                 'adapter_lock': amhl[pubkeys[2]][0],
-                'adapter_witness': adapter_witnesses[2],
-                'locking_script': parsing.compile_script(amhl[pubkeys[2]][1]),
+                'adapter_witness': adapter_witnesses[2].bytes,
+                'locking_script': amhl[pubkeys[2]][1].bytes,
             },
             'prvkey': prvkeys[2],
             'pubkey': pubkeys[2],
             'inbound_txn': Bob['outbound_txn'],
             'tweak_point': amhl[pubkeys[2]][2],
             'scalar': amhl[pubkeys[2]][3],
         }
@@ -895,18 +1007,18 @@
         Bob['inbound_txn']['witness'] = parsing.compile_script(f'push x{sigA.hex()} true')
         assert functions.run_auth_script(
             Bob['inbound_txn']['witness'] + Bob['inbound_txn']['locking_script'],
             Bob['inbound_txn']['sigfields']
         )
 
         # go into the future to prove a refund txn works
-        refund_witness = parsing.compile_script(tools.make_ptlc_refund_witness(
+        refund_witness = tools.make_ptlc_refund_witness(
             Alice['prvkey'], refund_sigfields[0]
-        ))
+        )
         assert functions.run_auth_script(
-            refund_witness + Alice['outbound_txn']['locking_script'],
+            refund_witness.bytes + Alice['outbound_txn']['locking_script'],
             {**refund_sigfields[0], 'timestamp': int(time())+11}
         )
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `tapescript-0.4.1/tests/vectors/cds_committed_script.hex` & `tapescript-0.5.0/tests/vectors/cds_committed_script.hex`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/cds_committed_script.src` & `tapescript-0.5.0/tests/vectors/cds_committed_script.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/cds_committed_script_decompiled.src` & `tapescript-0.5.0/tests/vectors/cds_committed_script_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/cds_unlocking_script1.hex` & `tapescript-0.5.0/tests/vectors/cds_unlocking_script1.hex`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/cds_unlocking_script1.src` & `tapescript-0.5.0/tests/vectors/cds_unlocking_script1.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/cds_unlocking_script1_decompiled.src` & `tapescript-0.5.0/tests/vectors/cds_unlocking_script1_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/cds_unlocking_script2.hex` & `tapescript-0.5.0/tests/vectors/cds_unlocking_script2.hex`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/cds_unlocking_script2.src` & `tapescript-0.5.0/tests/vectors/cds_unlocking_script2.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/cds_unlocking_script2_decompiled.src` & `tapescript-0.5.0/tests/vectors/cds_unlocking_script2_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/cds_unlocking_script3.hex` & `tapescript-0.5.0/tests/vectors/cds_unlocking_script3.hex`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/cds_unlocking_script3.src` & `tapescript-0.5.0/tests/vectors/cds_unlocking_script3.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/cds_unlocking_script3_decompiled.src` & `tapescript-0.5.0/tests/vectors/cds_unlocking_script3_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/correspondent_unlocking_script2.src` & `tapescript-0.5.0/tests/vectors/correspondent_unlocking_script2.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/correspondent_unlocking_script2_decompiled.src` & `tapescript-0.5.0/tests/vectors/correspondent_unlocking_script2_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/macros_and_variables.src` & `tapescript-0.5.0/tests/vectors/macros_and_variables.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/macros_and_variables_decompiled.src` & `tapescript-0.5.0/tests/vectors/macros_and_variables_decompiled.src`

 * *Files identical despite different names*

### Comparing `tapescript-0.4.1/tests/vectors/new_ops_0.4.0_decompiled.src` & `tapescript-0.5.0/tests/vectors/new_ops_0.4.0_decompiled.src`

 * *Files 22% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 OP_LOOP {
     OP_PUSH0 d1
     OP_SUBTRACT_INTS d2
 }
 OP_CHECK_MULTISIG x00 d2 d2
 OP_CHECK_MULTISIG_VERIFY x00 d2 d3
 OP_SIGN xdd
-OP_SIGN_QUEUE
-OP_CHECK_SIG_QUEUE
+OP_SIGN_STACK
+OP_CHECK_SIG_STACK
 OP_DERIVE_SCALAR
 OP_CLAMP_SCALAR d1
 OP_ADD_SCALARS d3
 OP_SUBTRACT_SCALARS d2
 OP_DERIVE_POINT
 OP_SUBTRACT_POINTS d4
 OP_MAKE_ADAPTER_SIG_PUBLIC
```

### Comparing `tapescript-0.4.1/tests/vectors/omega_e2e.hex` & `tapescript-0.5.0/tests/vectors/omega_e2e.hex`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 2900 0004
     2b 0001
         06
 
-2901 0026
+2901 0023
     2c 0005
-        0200
-        030122
-    001c
+        02 00
+        0301 22
+    0019
         040004 feedbeef
-        0500000010 79656c6c6f77207375626d6172696e65
+        0310 79656c6c6f77207375626d6172696e65
 
 2902 0017
     2c 0009
         2c 0002
             2a00
         0002
             2a01
@@ -73,15 +73,15 @@
 24 33
 25
 26
 27
 28
 2d
 2e
-2f 20
+2f
 30
 31 04 feedbeef
 32 04 feedbeef
 33
 34 0c 15
 35
 36 0c
@@ -125,17 +125,18 @@
 52
 53
 54
 55
 56
 57
 58
+05 00
 59 00
-5a 01
-5b 01
+5a 00
+5b b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9
 5c 01
 5d 01
 5e 01
 5f 01
 60 01
 61 01
 62 01
```

### Comparing `tapescript-0.4.1/tests/vectors/omega_e2e.src` & `tapescript-0.5.0/tests/vectors/omega_e2e.src`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     OP_IF {
         # comment within if #
         OP_PUSH0 d0
         OP_PUSH1 x22
     } ELSE {
         # comment within else #
         OP_PUSH2 xfeedbeef
-        OP_PUSH4 s"yellow submarine"
+        OP_PUSH s"yellow submarine"
     }
 }
 
 
 OP_DEF 2 {
     OP_IF {
         OP_IF {
@@ -67,16 +67,16 @@
 OP_CALL d0
 OP_TRUE
 OP_CALL d1
 OP_SIZE
 OP_WRITE_CACHE s"size" d1
 OP_READ_CACHE s"size"
 OP_READ_CACHE_SIZE s"size"
-OP_READ_CACHE_Q
-OP_READ_CACHE_Q_SIZE
+OP_READ_CACHE_STACK
+OP_READ_CACHE_STACK_SIZE
 OP_ADD_INTS d12
 OP_SUBTRACT_INTS d21
 OP_MULT_INTS d2
 OP_DIV_INT d-10
 OP_DIV_INTS
 OP_MOD_INT d10
 OP_MOD_INTS
@@ -98,15 +98,15 @@
 OP_CHECK_SIG_VERIFY x33
 OP_CHECK_TIMESTAMP
 OP_CHECK_TIMESTAMP_VERIFY
 OP_CHECK_EPOCH
 OP_CHECK_EPOCH_VERIFY
 OP_EVAL
 OP_NOT
-OP_RANDOM d32
+OP_RANDOM
 OP_RETURN
 OP_SET_FLAG xfeedbeef
 OP_UNSET_FLAG xfeedbeef
 OP_DEPTH
 OP_SWAP d12 d21
 OP_SWAP2
 OP_REVERSE d12
@@ -139,16 +139,16 @@
     # comment within loop #
     OP_PUSH d1
     OP_SUBTRACT_INTS d2
 }
 OP_CHECK_MULTISIG x00 d2 d2
 OP_CHECK_MULTISIG_VERIFY x00 d2 d3
 OP_SIGN x00
-OP_SIGN_QUEUE
-OP_CHECK_SIG_QUEUE
+OP_SIGN_STACK
+OP_CHECK_SIG_STACK
 OP_DERIVE_SCALAR
 OP_CLAMP_SCALAR d1
 OP_ADD_SCALARS d3
 OP_SUBTRACT_SCALARS d2
 OP_DERIVE_POINT
 OP_SUBTRACT_POINTS d4
 OP_MAKE_ADAPTER_SIG_PUBLIC
@@ -156,16 +156,17 @@
 OP_CHECK_ADAPTER_SIG
 OP_DECRYPT_ADAPTER_SIG
 OP_INVOKE
 OP_XOR
 OP_OR
 OP_AND
 OP_GET_MESSAGE x00
-NOP90 d1
-NOP91 d1
+OP_CHECK_TEMPLATE x00
+OP_CHECK_TEMPLATE_VERIFY x00
+OP_TAPROOT xb94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9
 NOP92 d1
 NOP93 d1
 NOP94 d1
 NOP95 d1
 NOP96 d1
 NOP97 d1
 NOP98 d1
```

### Comparing `tapescript-0.4.1/tests/vectors/omega_e2e_aliases.src` & `tapescript-0.5.0/tests/vectors/omega_e2e_aliases.src`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     if {
         # comment within if #
         push0 d0
         push1 x22
     } else {
         # comment within else #
         push2 xfeedbeef
-        push4 s"yellow submarine"
+        push1 s"yellow submarine"
     }
 }
 
 
 def 2 {
     if {
         if {
@@ -65,24 +65,24 @@
 false
 call d0
 true
 call d1
 size
 write_cache s"size" d1
 read_cache s"size"
-rcs s"size"
-rcq
-rcqs
-add_ints d12
-subtract_ints d21
-mult_ints d2
+rcz s"size"
+rcs
+rcsz
+add d12
+sub d21
+mult d2
 div_int d-10
-div_ints
+div
 mod_int d10
-mod_ints
+mod
 add_floats d2
 subf d2
 div_float x3c4985f0
 div_floats
 mod_float x3c4985f0
 mod_floats
 add_points d3
@@ -91,31 +91,31 @@
 sha256
 shake256 d20
 verify
 equal
 equal_verify
 check_sig x22
 csv x33
-check_timestamp
-ctv
+cts
+ctsv
 check_epoch
 cev
 eval
 not
-random d32
+random
 return
 set_flag xfeedbeef
 unset_flag xfeedbeef
 depth
 swap d12 d21
 swap2
 reverse d12
-concat
+cat
 split d12
-concat_str
+cats
 split_str d21
 check_transfer
 merkleval xfeedbeeffeedbeeffeedbeeffeedbeeffeedbeeffeedbeeffeedbeeffeedbeef
 try {
     # comment within try #
     false
     verify
@@ -138,16 +138,16 @@
     # comment within loop #
     push d1
     subtract_ints d2
 }
 cms x00 d2 d2
 cmsv x00 d2 d3
 sign x00
-sign_queue
-csq
+sign_stack
+css
 derive_scalar
 clamp_scalar d1
 add_scalars d3
 subtract_scalars d2
 derive_point
 subtract_points d4
 masu
@@ -155,16 +155,17 @@
 cas
 das
 invoke
 xor
 or
 and
 msg x00
-nop90 d1
-nop91 d1
+ct x00
+ctv x00
+tr xb94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9
 nop92 d1
 nop93 d1
 nop94 d1
 nop95 d1
 nop96 d1
 nop97 d1
 nop98 d1
```

### Comparing `tapescript-0.4.1/tests/vectors/omega_e2e_decompiled.src` & `tapescript-0.5.0/tests/vectors/omega_e2e_decompiled.src`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 }
 OP_DEF 1 {
     OP_IF {
         OP_PUSH0 d0
         OP_PUSH1 d1 x22
     } ELSE {
         OP_PUSH2 d4 xfeedbeef
-        OP_PUSH4 d16 x79656c6c6f77207375626d6172696e65
+        OP_PUSH1 d16 x79656c6c6f77207375626d6172696e65
     }
 }
 OP_DEF 2 {
     OP_IF {
         OP_IF {
             OP_CALL d0
         } ELSE {
@@ -52,16 +52,16 @@
 OP_CALL d0
 OP_TRUE
 OP_CALL d1
 OP_SIZE
 OP_WRITE_CACHE x73697a65 d1
 OP_READ_CACHE x73697a65
 OP_READ_CACHE_SIZE x73697a65
-OP_READ_CACHE_Q
-OP_READ_CACHE_Q_SIZE
+OP_READ_CACHE_STACK
+OP_READ_CACHE_STACK_SIZE
 OP_ADD_INTS d12
 OP_SUBTRACT_INTS d21
 OP_MULT_INTS d2
 OP_DIV_INT d-10
 OP_DIV_INTS
 OP_MOD_INT d10
 OP_MOD_INTS
@@ -83,15 +83,15 @@
 OP_CHECK_SIG_VERIFY x33
 OP_CHECK_TIMESTAMP
 OP_CHECK_TIMESTAMP_VERIFY
 OP_CHECK_EPOCH
 OP_CHECK_EPOCH_VERIFY
 OP_EVAL
 OP_NOT
-OP_RANDOM d32
+OP_RANDOM
 OP_RETURN
 OP_SET_FLAG xfeedbeef
 OP_UNSET_FLAG xfeedbeef
 OP_DEPTH
 OP_SWAP d12 d21
 OP_SWAP2
 OP_REVERSE d12
@@ -121,16 +121,16 @@
 OP_LOOP {
     OP_PUSH0 d1
     OP_SUBTRACT_INTS d2
 }
 OP_CHECK_MULTISIG x00 d2 d2
 OP_CHECK_MULTISIG_VERIFY x00 d2 d3
 OP_SIGN x00
-OP_SIGN_QUEUE
-OP_CHECK_SIG_QUEUE
+OP_SIGN_STACK
+OP_CHECK_SIG_STACK
 OP_DERIVE_SCALAR
 OP_CLAMP_SCALAR d1
 OP_ADD_SCALARS d3
 OP_SUBTRACT_SCALARS d2
 OP_DERIVE_POINT
 OP_SUBTRACT_POINTS d4
 OP_MAKE_ADAPTER_SIG_PUBLIC
@@ -138,16 +138,17 @@
 OP_CHECK_ADAPTER_SIG
 OP_DECRYPT_ADAPTER_SIG
 OP_INVOKE
 OP_XOR
 OP_OR
 OP_AND
 OP_GET_MESSAGE x00
-NOP90 d1
-NOP91 d1
+OP_CHECK_TEMPLATE x00
+OP_CHECK_TEMPLATE_VERIFY x00
+OP_TAPROOT xb94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9
 NOP92 d1
 NOP93 d1
 NOP94 d1
 NOP95 d1
 NOP96 d1
 NOP97 d1
 NOP98 d1
```

### Comparing `tapescript-0.4.1/pyproject.toml` & `tapescript-0.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tapescript"
-version = "0.4.1"
+version = "0.5.0"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 dependencies = [
   "PyNaCl>=1.5.0"
 ]
-description = "Scripting system for use in distributed systems"
+description = "Bytecode VM for embedding ACL in distributed systems"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: ISC License (ISCL)",
   "Operating System :: OS Independent",
@@ -25,7 +25,12 @@
 
 [project.urls]
 "Homepage" = "https://github.com/k98kurz/tapescript"
 "Bug Tracker" = "https://github.com/k98kurz/tapescript/issues"
 
 [project.scripts]
 tapescript = "tapescript.tools:run_cli"
+
+[project.optional-dependencies]
+docs = [
+  "autodox >= 0.1.16"
+]
```

### Comparing `tapescript-0.4.1/readme.md` & `tapescript-0.5.0/readme.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Tapescript
 
 Simple DSL and VM loosely inspired by Bitcoin script but also hopefully more
 useful for other applications. The idea is to programmatically ensure access
-controls in a distributed system using cryptography.
+controls in a distributed system using cryptography. Unlike Java or WASM VMs,
+many op codes do complex things rather than simple/primitive ones, e.g.
+`OP_MERKLEVAL` and `OP_CHECK_MULTISIG`.
 
 ## Status
 
 - [x] OPs
 - [x] Interpreter functions and classes
 - [x] Byte-code compiler
 - [x] Decompiler
@@ -20,15 +22,16 @@
 - [x] Package published
 - [x] Added try...except
 - [x] Aliases without `OP_` prefix
 - [x] Macros and variables
 - [x] Loops
 - [x] HTLCs, AMHLs, adapter signatures, delegated key scripts
 - [x] Simple CLI: compile, decompile, run, and auth
-- [ ] Rewrite `OP_MERKLEVAL` and tools to use root=xor(hash(hash(branch)), hash(hash(branch)))
+- [x] Document plugin system
+- [x] Rewrite `OP_MERKLEVAL` and tools to use root=xor(hash(hash(branchA)), hash(hash(branchB)))
 
 ## Usage
 
 ### Installation
 
 ```bash
 pip install tapescript
@@ -42,59 +45,80 @@
 
 ### CLI
 
 As of version 0.4.0, a simple CLI has been included with the following features:
 - `compile src_file bin_file` -- compiles the human-readable source into bytecode
 - `decompile bin_file` -- decompiles bytecode to human-readable source
 - `run bin_file [cache_file]` -- runs Tapescript bytecode and prints the cache
-and queue
+and stack
 - `auth bin_file [cache_file]` -- runs the Tapescript bytecode as an auth script
 and prints "true" if it succeeded and "false" otherwise
 
 Passing the optional `cache_file` parameter will set specific cache values after
 parsing the `cache_file`, which must adhere to a specific format. The intent of
 this CLI is to make it easy to experiment and/or debug Tapescript scripts. Run
 the command `tapescript` to get the help text.
 
+Note that the CLI does not currently include support for soft-forks, contracts,
+or plugins.
+
 ### Write, compile, decompile
 
 See the
-[langauge_spec.md](https://github.com/k98kurz/tapescript/blob/master/language_spec.md)
-and [docs.md](https://github.com/k98kurz/tapescript/blob/master/docs.md) files
+[langauge_spec.md](https://github.com/k98kurz/tapescript/blob/v0.5.0/language_spec.md)
+and [docs.md](https://github.com/k98kurz/tapescript/blob/v0.5.0/docs.md) files
 for syntax and operation specifics.
 
 Once you have a script written, use the `compile_script(code: str) -> bytes`
-function to turn it into the byte code that the interpreter runs. Note that each
-`OP_` function has an alias that excludes the `OP_` prefix; e.g. `OP_PUSH d1`
-can also be written `PUSH d1`. Op names are not case-sensitive, and several ops
-have additional aliases. Variable and macro names are case-sensitive.
+function to turn it into the byte code that the interpreter runs. Alternatvely,
+there is a `Script` class that can be initialized with either the source code or
+the byte code with `Script.from_src` and `Script.from_bytes`, respectively, and
+it will automatically compile source code to byte code or decompile byte code to
+source code; `Script` instances can also be added together with a simple +, e.g.
+`script = unlocking_script + locking_script`. The script running functions can
+accept either a `Script` object or the byte code.
+
+Note that each `OP_` function has an alias that excludes the `OP_` prefix; e.g.
+`OP_PUSH d1` can also be written `PUSH d1`. Op names are not case-sensitive, and
+several ops have additional aliases. Variable and macro names are case-sensitive.
 
 The following functions are also available for VM-compatible serialization:
 - `bytes_to_int`
 - `int_to_bytes`
 - `uint_to_bytes`
 - `bytes_to_bool`
 - `bytes_to_float`
 - `float_to_bytes`
 
-And these functions are available for convenience:
+And these functions are available for convenience and cryptography:
+- `clamp_scalar`
+- `H_big`
+- `H_small`
+- `derive_key_from_seed`
+- `derive_point_from_scalar`
+- `aggregate_points`
+- `aggregate_scalars`
+- `sign_with_scalar`
+- `not_bytes`
 - `xor`
+- `and_bytes`
+- `or_bytes`
 - `bytes_are_same`
 
 #### Variables and Macros
 
 Version 0.3.0 and 0.3.1 added a sort of variable and macro system to the
-compiler.
+compiler. Full documentation can be found in the language spec file.
 
 Variable assignment uses two possible syntaxes: `@= varname [vals]` or
-`@= varname count`; the first pushes the values onto the queue then calls
+`@= varname count`; the first pushes the values onto the stack then calls
 `OP_WRITE_CACHE` to store those values in the cache at the `varname` key, while
 the second instead just calls `OP_WRITE_CACHE` and takes `count` items from the
 queue. Using `@varname` calls `OP_READ_CACHE` and places the values held at the
-`varname` cache key onto the queue.
+`varname` cache key onto the stack.
 
 Macros allow use of string interpolation in the compiler: use the syntax
 `!= macroname [ arg1 arg2 ... ] { statements }` to define a macro and
 `!macroname [ arg1 arg2 ... ]` to call the macro. The compiler will replace the
 macro call with the `statements` after substituting the args before compilation.
 
 #### Merklized scripts
@@ -123,14 +147,70 @@
 compiled and used as the locking condition. A signature would be prepended to
 the unlocking script with an `OP_PUSH x<hex signature> `, and this would then be
 compiled to become the unlocking bytes. Then concatenate the locking script to
 the unlocking script (i.e. script = unlock + lock) and run through the
 `run_auth_script` function, which will return a `True` if it executed
 successfully and `False` otherwise.
 
+Tools are included for making merklized scripts:
+- `ScriptLeaf` and `ScriptNode` classes
+- `create_script_tree_prioritized(...) -> ScriptNode`
+- `create_merklized_script_prioritized(...) -> tuple[Script, list[Script]]`,
+which uses `create_script_tree_prioritized` under the hood
+
+The two functions accept a list of leaf scripts and produce an unbalanced tree
+that priotizes efficient execution of lowest index scripts at the expense of
+linearly increasing unlocking script size for higher index scripts. There are
+not currently any functions for producing a balanced tree, but the included
+`ScriptLeaf` and `ScriptNode` classes can be used to make any arbitrary tree:
+
+```python
+from tapescript import ScriptLeaf, ScriptNode
+
+# get some scripts from somewhere
+sources = get_five_script_sources()
+
+tree = ScriptNode(
+    ScriptNode(
+        ScriptLeaf.from_src(sources[0]),
+        ScriptNode(
+            ScriptLeaf.from_src(sources[1]),
+            ScriptLeaf.from_src(sources[2]),
+        )
+    ),
+    ScriptNode(
+        ScriptLeaf.from_src(sources[3]),
+        ScriptLeaf.from_src(sources[4]),
+    )
+)
+```
+
+#### Taproot scripts
+
+The basic Taproot concept is to take a sha256 hash of a script as a commitment,
+clamp it to the ed25519 scalar field, derive a point from it, and add that point
+to a public key to create the root commitment, which itself functions both as a
+commitment to the script and as a public key. Signatures can be made that
+validate against the root, or the committed script can be executed by supplying
+both the script and the original public key. The script execution path (aka
+script-spend) verifies that the script and public key combine to form the root,
+then it executes the committed script if verification succeeded and otherwise
+removes the script and places `x00` (`False`) onto the stack. The signature path
+(aka key-spend) instead validates the supplied signature against the root as a
+public key.
+
+Signatures are created using the original private key and the script commitment
+by adding the script commitment (clamped to the scalar field) to the scalar
+derived from the private key, then using that in place of the private key scalar.
+
+Tools are included for using taproot:
+- `make_taproot_lock`
+- `make_taproot_witness_keyspend`
+- `make_taproot_witness_scriptspend`
+
 #### Hash Time Locked Contracts and Point Time Locked Contracts
 
 Tapescript includes tools for generating locking scripts and unlocking scripts/
 witnesses for HTLCs and PTLCs:
 - `make_htlc_sha256_lock`
 - `make_htlc_sha256_witness`
 - `make_htlc_shake256_lock`
@@ -214,48 +294,48 @@
 beyond the scope of this project.
 
 These may be changed or more ops/tools added in the future as the technology is
 tested in specific applications.
 
 ### Run a script
 
-Run a script by compiling it to byte code (if it wasn't already) and run with
-either `run_script(script: bytes, cache_vals: dict = {}, contracts: dict = {})`
-or `run_auth_script(script: bytes, cache_vals: dict = {}, contracts: dict = {})`.
+Run a script by compiling the source to byte code or creating a `Script` object
+and run with either
+`run_script(script: bytes|Script, cache_vals: dict = {}, contracts: dict = {})`
+or `run_auth_script(script: bytes|Script, cache_vals: dict = {}, contracts: dict = {})`.
 The `run_script` function returns `tuple` of length 3 containing a `Tape`, a
 `LifoQueue`, and the final state of the `cache` dict. The `run_auth_script`
 instead returns a bool that is `True` if the script ran without error and
-resulted in a single `0x01` value on the queue; otherwise it returns `False`.
+resulted in a single `0x01` value on the stack; otherwise it returns `False`.
 
 In the case where a signature is expected to be validated, the message parts for
 the signature must be passed in via the `cache_vals` dict at keys `sigfield[1-8]`.
 In the case where `OP_CHECK_TRANSFER` or `OP_INVOKE` might be called, the
 contracts must be passed in via the `contracts` dict. See the
-[check_transfer](https://github.com/k98kurz/tapescript/blob/master/language_spec.md#op_check_transfer)
+[check_transfer](https://github.com/k98kurz/tapescript/blob/v0.5.0/language_spec.md#op_check_transfer)
 and
-[INVOKE](https://github.com/k98kurz/tapescript/blob/master/language_spec.md#op_invoke)
-section in the language_spec.md file for more informaiton about these two ops.
+[invoke](https://github.com/k98kurz/tapescript/blob/v0.5.0/language_spec.md#op_invoke)
+sections in the language_spec.md file for more informaiton about these two ops.
 
 #### Changing flags
 
 The interpreter flags can be changed by changing the `functions.flags` dict.
 
 #### Adding ops
 
 The ops can be updated via a plugin system.
 
 ```py
-from queue import LifoQueue
-from tapescript import Tape, add_opcode, add_opcode_parsing_handlers
+from tapescript import Stack, Tape, add_opcode, add_opcode_parsing_handlers
 
 
-def OP_SOME_NONSENSE(tape: Tape, queue: LifoQueue, cache: dict) -> None:
+def OP_SOME_NONSENSE(tape: Tape, stack: Stack, cache: dict) -> None:
     count = tape.read(1)[0]
     for _ in range(count):
-        queue.put(b'some nonsense')
+        stack.put(b'some nonsense')
 
 def OP_SOME_NONSENSE_compiler(opname: str, symbols: list[str],
         symbols_to_advance: int, symbol_index: int):
     symbols_to_advance += 1
     if symbols[0][0] != 'd':
         raise SyntaxError(f'{opname} - int argument must begin with d - {symbol_index}')
     val = int(symbols[0][1:]).to_bytes(1, 'big')
@@ -272,14 +352,68 @@
 add_opcode_parsing_handlers(
     'OP_SOME_NONSENSE',
     OP_SOME_NONSENSE_compiler,
     OP_SOME_NONSENSE_decompiler
 )
 ```
 
+#### Adding an alias
+
+If you want to use a new alias for an op code, you can create this alias using
+the `add_alias` function. Valid aliases are alpha-numeric and may contain
+underscores. This function will raise a `TypeError` for non-str args and a
+`ValueError` if the alias contains invalid chars or is already in use.
+
+### Plugins
+
+There is a simple plugin system available for modifying execution behavior when
+calling certain ops. Existing uses are documented below, but this system may be
+used for future extensions when such use cases arise.
+
+The basic functions for interacting with the plugin system are the following:
+- `add_plugin(scope: str, plugin: Callable[[Tape, Stack, dict], Any]) -> None`
+- `remove_plugin(scope: str, plugin: Callable[[Tape, Stack, dict], Any]) -> None`
+- `reset_plugins(scope: str) -> None`
+
+Additionally, plugins can be supplied in a dict format to `run_script` or
+`run_auth_script`, but this will overwrite any plugins previously added for any
+scope included in the injected `plugins` argument.
+
+#### Signature Extensions
+
+The signature extension system executes all plugins under the
+"signature_extensions" scope at the beginning of these ops:
+- `OP_GET_MESSAGE`
+- `OP_CHECK_SIG`
+- `OP_CHECK_SIG_VERIFY`
+- `OP_CHECK_MULTISIG`
+- `OP_CHECK_MULTISIG_VERIFY`
+- `OP_SIGN`
+- `OP_CHECK_TEMPLATE` if tape.flags[10] is set to True, which is the default
+- `OP_CHECK_TEMPLATE_VERIFY` if tape.flags[10] is set to True, which is the default
+
+The functions registered as signature extension plugins should modify the
+sigfields in the cache, but they are free to do anything with the runtime data.
+Signature extension plugins can be managed using the following functions:
+- `add_signature_extension(plugin: Callable[[Tape, Stack, dict], None]) -> None`
+- `remove_signature_extension(plugin: Callable[[Tape, Stack, dict], None]) -> None`
+- `reset_signature_extensions() -> None`
+- `run_sig_extensions(tape: Tape, stack: Stack, cache: dict) -> None`
+
+#### Check Template
+
+`OP_CHECK_TEMPLATE` and `OP_CHECK_TEMPLATE_VERIFY` will run the plugins in the
+"check_template" scope when checking each sigfield against the appropriate
+template. This execution is different from the signature extension system: the
+args passed into this plugin execution call are not the runtime data but rather
+limited to just the two items in question and the cache; also, the return values
+are collected, and if any return value is True, then the check passes. If there
+are no plugins, `OP_CHECK_TEMPLATE/VERIFY` will instead do a strict equality
+check.
+
 ### Contracts
 
 The interpreter includes a system for including contracts for greater
 extensibility. For example, the bundled `CanCheckTransfer` interface is used
 to check that contracts can be used with the `OP_CHECK_TRANSFER` operation, and
 the `CanBeInvoked` interface is used to check that contracts can be used with
 the `OP_INVOKE` operation. To add an interface for checking loaded contracts,
@@ -317,43 +451,68 @@
 If a signature is passed to a signature checker that uses a disallowed sigflag,
 a `ScriptExecutionError` will be raised.
 
 These also apply to the `OP_CHECK_MULTI_SIG` and `OP_CHECK_MULTI_SIG_VERIFY`
 operations. See the language spec and docs files for more detailed information
 about how `CMS` and `CMSV` work.
 
+#### Signature Extension Plugins
+
+As of 0.4.2, the following OPs can be slightly modified with a plugin system:
+`CHECK_SIG`, `CHECK_MULTISIG`, `SIGN`, and `GET_MESSAGE`. Signature extension
+plugins can be managed with the following functions:
+- `add_signature_extension(plugin: Callable[[Tape, Stack, dict], None])`
+- `remove_signature_extension(plugin: Callable[[Tape, Stack, dict], None])`
+- `reset_signature_extensions()`
+
+Additionally, plugins can be injected when calling `run_script` or
+`run_auth_script` the same way as contracts. The underlying plugin system uses
+string scopes, and the signature extension plugins have the scope of
+"signature_extensions". For example:
+
+```python
+t, q, c = run_script(script, plugins={
+    'signature_extensions': [some_plugin_function]
+})
+```
+
+Plugin functions must take a Tape, Stack, and dict (i.e. the runtime data)
+as arguments, and they must do all of their work on them. (Technically, they
+are procedures with side-effects.) For signature extension, the sigfields in the
+dict cache are the most likely target for alteration.
+
 ### Soft Forks
 
 A soft fork is a protocol upgrade such that all scripts written under the new
 protocol also validate under the old version -- older versions do not break when
 encountering use of the new feature. Tapescript was designed with soft-fork
 support in mind, and the helper function `add_soft_fork` is included to
 streamline the process and reduce the use of boilerplate.
 
 To enable a soft fork, a NOP code must be replaced with an op that reads the
-next byte as a signed int, pulls that many values from the queue, runs any
+next byte as a signed int, pulls that many values from the stack, runs any
 checks on the data, and raises an error in case any check fails. This maintains
 the behavior of the original NOP such that any nodes that did not activate the
 soft fork will not have any errors parsing scripts using the new OP.
 
 Example soft fork:
 
 ```python
 from tapescript import (
     Tape,
+    Stack,
     ScriptExecutionError,
     add_soft_fork,
     bytes_to_int,
 )
-from queue import LifoQueue
 
 
-def OP_CHECK_ALL_EQUAL_VERIFY(tape: Tape, queue: LifoQueue, cache: dict) -> None:
+def OP_CHECK_ALL_EQUAL_VERIFY(tape: Tape, stack: Stack, cache: dict) -> None:
     """Replacement for NOP255: read the next byte an int count, take
-        that many items from queue, run checks, and raise an error if
+        that many items from stack, run checks, and raise an error if
         any check fails.
     """
     count = bytes_to_int(tape.read(1))
     assert count >= 0
     items = []
     for i in range(count):
         items.append(queue.get(False))
@@ -414,32 +573,44 @@
 ```
 
 For windows, replace `source venv/bin/activate` with `source venv/Scripts/activate`.
 
 Then run the test suite with the following:
 
 ```bash
-find tests -name test_*.py -exec {} \;
+find tests -name test_*.py -print -exec {} \;
 ```
 
 or
 
 ```bash
-python test/test_classes.py
-python test/test_functions.py
-python test/test_parsing.py
-python test/test_tools.py
-python test/test_e2e_eltoo.py
+python tests/test_classes.py
+python tests/test_functions.py
+python tests/test_parsing.py
+python tests/test_security.py
+python tests/test_tools.py
+python tests/test_e2e_eltoo.py
+python tests/test_e2e_sigext.py
 ```
 
-There are currently 225 tests and 106 test vectors used for validating the
+There are currently 239 tests and 104 test vectors used for validating the ops,
 compiler, decompiler, and script running functions. This includes 3 tests for a
-proof-of-concept implementation of the eltoo payment channel protocol, a test
-proving the one-way homomorphic quality of ed25519, and e2e tests combining the
-anonymous multi-hop lock (AMHL) system with adapter signatures.
+proof-of-concept implementation of the eltoo payment channel protocol, and e2e
+tests combining the anonymous multi-hop lock (AMHL) system with adapter
+signatures, as well as tests for the contract system, signature extension
+plugins, hard-forks, and the soft-fork system. There are an additional 7
+security tests, including a test proving the one-way homomorphic quality of
+ed25519 and a test proving that all symmetric script trees share the same root.
+
+## Contributing
+
+Check out the [Pycelium discord server](https://discord.gg/b2QFEJDX69). If you
+experience a problem, please discuss it on the Discord server. All suggestions
+for improvement are also welcome, and the best place for that is also Discord.
+If you experience a bug and do not use Discord, open an issue on Github.
 
 ## ISC License
 
 Copyright (c) 2024 Jonathan Voss
 
 Permission to use, copy, modify, and/or distribute this software
 for any purpose with or without fee is hereby granted, provided
```

### Comparing `tapescript-0.4.1/PKG-INFO` & `tapescript-0.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.3
 Name: tapescript
-Version: 0.4.1
-Summary: Scripting system for use in distributed systems
+Version: 0.5.0
+Summary: Bytecode VM for embedding ACL in distributed systems
 Project-URL: Homepage, https://github.com/k98kurz/tapescript
 Project-URL: Bug Tracker, https://github.com/k98kurz/tapescript/issues
 Author-email: k98kurz <k98kurz@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Other Scripting Engines
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.10
 Requires-Dist: pynacl>=1.5.0
+Provides-Extra: docs
+Requires-Dist: autodox>=0.1.16; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # Tapescript
 
 Simple DSL and VM loosely inspired by Bitcoin script but also hopefully more
 useful for other applications. The idea is to programmatically ensure access
-controls in a distributed system using cryptography.
+controls in a distributed system using cryptography. Unlike Java or WASM VMs,
+many op codes do complex things rather than simple/primitive ones, e.g.
+`OP_MERKLEVAL` and `OP_CHECK_MULTISIG`.
 
 ## Status
 
 - [x] OPs
 - [x] Interpreter functions and classes
 - [x] Byte-code compiler
 - [x] Decompiler
@@ -37,15 +41,16 @@
 - [x] Package published
 - [x] Added try...except
 - [x] Aliases without `OP_` prefix
 - [x] Macros and variables
 - [x] Loops
 - [x] HTLCs, AMHLs, adapter signatures, delegated key scripts
 - [x] Simple CLI: compile, decompile, run, and auth
-- [ ] Rewrite `OP_MERKLEVAL` and tools to use root=xor(hash(hash(branch)), hash(hash(branch)))
+- [x] Document plugin system
+- [x] Rewrite `OP_MERKLEVAL` and tools to use root=xor(hash(hash(branchA)), hash(hash(branchB)))
 
 ## Usage
 
 ### Installation
 
 ```bash
 pip install tapescript
@@ -59,59 +64,80 @@
 
 ### CLI
 
 As of version 0.4.0, a simple CLI has been included with the following features:
 - `compile src_file bin_file` -- compiles the human-readable source into bytecode
 - `decompile bin_file` -- decompiles bytecode to human-readable source
 - `run bin_file [cache_file]` -- runs Tapescript bytecode and prints the cache
-and queue
+and stack
 - `auth bin_file [cache_file]` -- runs the Tapescript bytecode as an auth script
 and prints "true" if it succeeded and "false" otherwise
 
 Passing the optional `cache_file` parameter will set specific cache values after
 parsing the `cache_file`, which must adhere to a specific format. The intent of
 this CLI is to make it easy to experiment and/or debug Tapescript scripts. Run
 the command `tapescript` to get the help text.
 
+Note that the CLI does not currently include support for soft-forks, contracts,
+or plugins.
+
 ### Write, compile, decompile
 
 See the
-[langauge_spec.md](https://github.com/k98kurz/tapescript/blob/master/language_spec.md)
-and [docs.md](https://github.com/k98kurz/tapescript/blob/master/docs.md) files
+[langauge_spec.md](https://github.com/k98kurz/tapescript/blob/v0.5.0/language_spec.md)
+and [docs.md](https://github.com/k98kurz/tapescript/blob/v0.5.0/docs.md) files
 for syntax and operation specifics.
 
 Once you have a script written, use the `compile_script(code: str) -> bytes`
-function to turn it into the byte code that the interpreter runs. Note that each
-`OP_` function has an alias that excludes the `OP_` prefix; e.g. `OP_PUSH d1`
-can also be written `PUSH d1`. Op names are not case-sensitive, and several ops
-have additional aliases. Variable and macro names are case-sensitive.
+function to turn it into the byte code that the interpreter runs. Alternatvely,
+there is a `Script` class that can be initialized with either the source code or
+the byte code with `Script.from_src` and `Script.from_bytes`, respectively, and
+it will automatically compile source code to byte code or decompile byte code to
+source code; `Script` instances can also be added together with a simple +, e.g.
+`script = unlocking_script + locking_script`. The script running functions can
+accept either a `Script` object or the byte code.
+
+Note that each `OP_` function has an alias that excludes the `OP_` prefix; e.g.
+`OP_PUSH d1` can also be written `PUSH d1`. Op names are not case-sensitive, and
+several ops have additional aliases. Variable and macro names are case-sensitive.
 
 The following functions are also available for VM-compatible serialization:
 - `bytes_to_int`
 - `int_to_bytes`
 - `uint_to_bytes`
 - `bytes_to_bool`
 - `bytes_to_float`
 - `float_to_bytes`
 
-And these functions are available for convenience:
+And these functions are available for convenience and cryptography:
+- `clamp_scalar`
+- `H_big`
+- `H_small`
+- `derive_key_from_seed`
+- `derive_point_from_scalar`
+- `aggregate_points`
+- `aggregate_scalars`
+- `sign_with_scalar`
+- `not_bytes`
 - `xor`
+- `and_bytes`
+- `or_bytes`
 - `bytes_are_same`
 
 #### Variables and Macros
 
 Version 0.3.0 and 0.3.1 added a sort of variable and macro system to the
-compiler.
+compiler. Full documentation can be found in the language spec file.
 
 Variable assignment uses two possible syntaxes: `@= varname [vals]` or
-`@= varname count`; the first pushes the values onto the queue then calls
+`@= varname count`; the first pushes the values onto the stack then calls
 `OP_WRITE_CACHE` to store those values in the cache at the `varname` key, while
 the second instead just calls `OP_WRITE_CACHE` and takes `count` items from the
 queue. Using `@varname` calls `OP_READ_CACHE` and places the values held at the
-`varname` cache key onto the queue.
+`varname` cache key onto the stack.
 
 Macros allow use of string interpolation in the compiler: use the syntax
 `!= macroname [ arg1 arg2 ... ] { statements }` to define a macro and
 `!macroname [ arg1 arg2 ... ]` to call the macro. The compiler will replace the
 macro call with the `statements` after substituting the args before compilation.
 
 #### Merklized scripts
@@ -140,14 +166,70 @@
 compiled and used as the locking condition. A signature would be prepended to
 the unlocking script with an `OP_PUSH x<hex signature> `, and this would then be
 compiled to become the unlocking bytes. Then concatenate the locking script to
 the unlocking script (i.e. script = unlock + lock) and run through the
 `run_auth_script` function, which will return a `True` if it executed
 successfully and `False` otherwise.
 
+Tools are included for making merklized scripts:
+- `ScriptLeaf` and `ScriptNode` classes
+- `create_script_tree_prioritized(...) -> ScriptNode`
+- `create_merklized_script_prioritized(...) -> tuple[Script, list[Script]]`,
+which uses `create_script_tree_prioritized` under the hood
+
+The two functions accept a list of leaf scripts and produce an unbalanced tree
+that priotizes efficient execution of lowest index scripts at the expense of
+linearly increasing unlocking script size for higher index scripts. There are
+not currently any functions for producing a balanced tree, but the included
+`ScriptLeaf` and `ScriptNode` classes can be used to make any arbitrary tree:
+
+```python
+from tapescript import ScriptLeaf, ScriptNode
+
+# get some scripts from somewhere
+sources = get_five_script_sources()
+
+tree = ScriptNode(
+    ScriptNode(
+        ScriptLeaf.from_src(sources[0]),
+        ScriptNode(
+            ScriptLeaf.from_src(sources[1]),
+            ScriptLeaf.from_src(sources[2]),
+        )
+    ),
+    ScriptNode(
+        ScriptLeaf.from_src(sources[3]),
+        ScriptLeaf.from_src(sources[4]),
+    )
+)
+```
+
+#### Taproot scripts
+
+The basic Taproot concept is to take a sha256 hash of a script as a commitment,
+clamp it to the ed25519 scalar field, derive a point from it, and add that point
+to a public key to create the root commitment, which itself functions both as a
+commitment to the script and as a public key. Signatures can be made that
+validate against the root, or the committed script can be executed by supplying
+both the script and the original public key. The script execution path (aka
+script-spend) verifies that the script and public key combine to form the root,
+then it executes the committed script if verification succeeded and otherwise
+removes the script and places `x00` (`False`) onto the stack. The signature path
+(aka key-spend) instead validates the supplied signature against the root as a
+public key.
+
+Signatures are created using the original private key and the script commitment
+by adding the script commitment (clamped to the scalar field) to the scalar
+derived from the private key, then using that in place of the private key scalar.
+
+Tools are included for using taproot:
+- `make_taproot_lock`
+- `make_taproot_witness_keyspend`
+- `make_taproot_witness_scriptspend`
+
 #### Hash Time Locked Contracts and Point Time Locked Contracts
 
 Tapescript includes tools for generating locking scripts and unlocking scripts/
 witnesses for HTLCs and PTLCs:
 - `make_htlc_sha256_lock`
 - `make_htlc_sha256_witness`
 - `make_htlc_shake256_lock`
@@ -231,48 +313,48 @@
 beyond the scope of this project.
 
 These may be changed or more ops/tools added in the future as the technology is
 tested in specific applications.
 
 ### Run a script
 
-Run a script by compiling it to byte code (if it wasn't already) and run with
-either `run_script(script: bytes, cache_vals: dict = {}, contracts: dict = {})`
-or `run_auth_script(script: bytes, cache_vals: dict = {}, contracts: dict = {})`.
+Run a script by compiling the source to byte code or creating a `Script` object
+and run with either
+`run_script(script: bytes|Script, cache_vals: dict = {}, contracts: dict = {})`
+or `run_auth_script(script: bytes|Script, cache_vals: dict = {}, contracts: dict = {})`.
 The `run_script` function returns `tuple` of length 3 containing a `Tape`, a
 `LifoQueue`, and the final state of the `cache` dict. The `run_auth_script`
 instead returns a bool that is `True` if the script ran without error and
-resulted in a single `0x01` value on the queue; otherwise it returns `False`.
+resulted in a single `0x01` value on the stack; otherwise it returns `False`.
 
 In the case where a signature is expected to be validated, the message parts for
 the signature must be passed in via the `cache_vals` dict at keys `sigfield[1-8]`.
 In the case where `OP_CHECK_TRANSFER` or `OP_INVOKE` might be called, the
 contracts must be passed in via the `contracts` dict. See the
-[check_transfer](https://github.com/k98kurz/tapescript/blob/master/language_spec.md#op_check_transfer)
+[check_transfer](https://github.com/k98kurz/tapescript/blob/v0.5.0/language_spec.md#op_check_transfer)
 and
-[INVOKE](https://github.com/k98kurz/tapescript/blob/master/language_spec.md#op_invoke)
-section in the language_spec.md file for more informaiton about these two ops.
+[invoke](https://github.com/k98kurz/tapescript/blob/v0.5.0/language_spec.md#op_invoke)
+sections in the language_spec.md file for more informaiton about these two ops.
 
 #### Changing flags
 
 The interpreter flags can be changed by changing the `functions.flags` dict.
 
 #### Adding ops
 
 The ops can be updated via a plugin system.
 
 ```py
-from queue import LifoQueue
-from tapescript import Tape, add_opcode, add_opcode_parsing_handlers
+from tapescript import Stack, Tape, add_opcode, add_opcode_parsing_handlers
 
 
-def OP_SOME_NONSENSE(tape: Tape, queue: LifoQueue, cache: dict) -> None:
+def OP_SOME_NONSENSE(tape: Tape, stack: Stack, cache: dict) -> None:
     count = tape.read(1)[0]
     for _ in range(count):
-        queue.put(b'some nonsense')
+        stack.put(b'some nonsense')
 
 def OP_SOME_NONSENSE_compiler(opname: str, symbols: list[str],
         symbols_to_advance: int, symbol_index: int):
     symbols_to_advance += 1
     if symbols[0][0] != 'd':
         raise SyntaxError(f'{opname} - int argument must begin with d - {symbol_index}')
     val = int(symbols[0][1:]).to_bytes(1, 'big')
@@ -289,14 +371,68 @@
 add_opcode_parsing_handlers(
     'OP_SOME_NONSENSE',
     OP_SOME_NONSENSE_compiler,
     OP_SOME_NONSENSE_decompiler
 )
 ```
 
+#### Adding an alias
+
+If you want to use a new alias for an op code, you can create this alias using
+the `add_alias` function. Valid aliases are alpha-numeric and may contain
+underscores. This function will raise a `TypeError` for non-str args and a
+`ValueError` if the alias contains invalid chars or is already in use.
+
+### Plugins
+
+There is a simple plugin system available for modifying execution behavior when
+calling certain ops. Existing uses are documented below, but this system may be
+used for future extensions when such use cases arise.
+
+The basic functions for interacting with the plugin system are the following:
+- `add_plugin(scope: str, plugin: Callable[[Tape, Stack, dict], Any]) -> None`
+- `remove_plugin(scope: str, plugin: Callable[[Tape, Stack, dict], Any]) -> None`
+- `reset_plugins(scope: str) -> None`
+
+Additionally, plugins can be supplied in a dict format to `run_script` or
+`run_auth_script`, but this will overwrite any plugins previously added for any
+scope included in the injected `plugins` argument.
+
+#### Signature Extensions
+
+The signature extension system executes all plugins under the
+"signature_extensions" scope at the beginning of these ops:
+- `OP_GET_MESSAGE`
+- `OP_CHECK_SIG`
+- `OP_CHECK_SIG_VERIFY`
+- `OP_CHECK_MULTISIG`
+- `OP_CHECK_MULTISIG_VERIFY`
+- `OP_SIGN`
+- `OP_CHECK_TEMPLATE` if tape.flags[10] is set to True, which is the default
+- `OP_CHECK_TEMPLATE_VERIFY` if tape.flags[10] is set to True, which is the default
+
+The functions registered as signature extension plugins should modify the
+sigfields in the cache, but they are free to do anything with the runtime data.
+Signature extension plugins can be managed using the following functions:
+- `add_signature_extension(plugin: Callable[[Tape, Stack, dict], None]) -> None`
+- `remove_signature_extension(plugin: Callable[[Tape, Stack, dict], None]) -> None`
+- `reset_signature_extensions() -> None`
+- `run_sig_extensions(tape: Tape, stack: Stack, cache: dict) -> None`
+
+#### Check Template
+
+`OP_CHECK_TEMPLATE` and `OP_CHECK_TEMPLATE_VERIFY` will run the plugins in the
+"check_template" scope when checking each sigfield against the appropriate
+template. This execution is different from the signature extension system: the
+args passed into this plugin execution call are not the runtime data but rather
+limited to just the two items in question and the cache; also, the return values
+are collected, and if any return value is True, then the check passes. If there
+are no plugins, `OP_CHECK_TEMPLATE/VERIFY` will instead do a strict equality
+check.
+
 ### Contracts
 
 The interpreter includes a system for including contracts for greater
 extensibility. For example, the bundled `CanCheckTransfer` interface is used
 to check that contracts can be used with the `OP_CHECK_TRANSFER` operation, and
 the `CanBeInvoked` interface is used to check that contracts can be used with
 the `OP_INVOKE` operation. To add an interface for checking loaded contracts,
@@ -334,43 +470,68 @@
 If a signature is passed to a signature checker that uses a disallowed sigflag,
 a `ScriptExecutionError` will be raised.
 
 These also apply to the `OP_CHECK_MULTI_SIG` and `OP_CHECK_MULTI_SIG_VERIFY`
 operations. See the language spec and docs files for more detailed information
 about how `CMS` and `CMSV` work.
 
+#### Signature Extension Plugins
+
+As of 0.4.2, the following OPs can be slightly modified with a plugin system:
+`CHECK_SIG`, `CHECK_MULTISIG`, `SIGN`, and `GET_MESSAGE`. Signature extension
+plugins can be managed with the following functions:
+- `add_signature_extension(plugin: Callable[[Tape, Stack, dict], None])`
+- `remove_signature_extension(plugin: Callable[[Tape, Stack, dict], None])`
+- `reset_signature_extensions()`
+
+Additionally, plugins can be injected when calling `run_script` or
+`run_auth_script` the same way as contracts. The underlying plugin system uses
+string scopes, and the signature extension plugins have the scope of
+"signature_extensions". For example:
+
+```python
+t, q, c = run_script(script, plugins={
+    'signature_extensions': [some_plugin_function]
+})
+```
+
+Plugin functions must take a Tape, Stack, and dict (i.e. the runtime data)
+as arguments, and they must do all of their work on them. (Technically, they
+are procedures with side-effects.) For signature extension, the sigfields in the
+dict cache are the most likely target for alteration.
+
 ### Soft Forks
 
 A soft fork is a protocol upgrade such that all scripts written under the new
 protocol also validate under the old version -- older versions do not break when
 encountering use of the new feature. Tapescript was designed with soft-fork
 support in mind, and the helper function `add_soft_fork` is included to
 streamline the process and reduce the use of boilerplate.
 
 To enable a soft fork, a NOP code must be replaced with an op that reads the
-next byte as a signed int, pulls that many values from the queue, runs any
+next byte as a signed int, pulls that many values from the stack, runs any
 checks on the data, and raises an error in case any check fails. This maintains
 the behavior of the original NOP such that any nodes that did not activate the
 soft fork will not have any errors parsing scripts using the new OP.
 
 Example soft fork:
 
 ```python
 from tapescript import (
     Tape,
+    Stack,
     ScriptExecutionError,
     add_soft_fork,
     bytes_to_int,
 )
-from queue import LifoQueue
 
 
-def OP_CHECK_ALL_EQUAL_VERIFY(tape: Tape, queue: LifoQueue, cache: dict) -> None:
+def OP_CHECK_ALL_EQUAL_VERIFY(tape: Tape, stack: Stack, cache: dict) -> None:
     """Replacement for NOP255: read the next byte an int count, take
-        that many items from queue, run checks, and raise an error if
+        that many items from stack, run checks, and raise an error if
         any check fails.
     """
     count = bytes_to_int(tape.read(1))
     assert count >= 0
     items = []
     for i in range(count):
         items.append(queue.get(False))
@@ -431,32 +592,44 @@
 ```
 
 For windows, replace `source venv/bin/activate` with `source venv/Scripts/activate`.
 
 Then run the test suite with the following:
 
 ```bash
-find tests -name test_*.py -exec {} \;
+find tests -name test_*.py -print -exec {} \;
 ```
 
 or
 
 ```bash
-python test/test_classes.py
-python test/test_functions.py
-python test/test_parsing.py
-python test/test_tools.py
-python test/test_e2e_eltoo.py
+python tests/test_classes.py
+python tests/test_functions.py
+python tests/test_parsing.py
+python tests/test_security.py
+python tests/test_tools.py
+python tests/test_e2e_eltoo.py
+python tests/test_e2e_sigext.py
 ```
 
-There are currently 225 tests and 106 test vectors used for validating the
+There are currently 239 tests and 104 test vectors used for validating the ops,
 compiler, decompiler, and script running functions. This includes 3 tests for a
-proof-of-concept implementation of the eltoo payment channel protocol, a test
-proving the one-way homomorphic quality of ed25519, and e2e tests combining the
-anonymous multi-hop lock (AMHL) system with adapter signatures.
+proof-of-concept implementation of the eltoo payment channel protocol, and e2e
+tests combining the anonymous multi-hop lock (AMHL) system with adapter
+signatures, as well as tests for the contract system, signature extension
+plugins, hard-forks, and the soft-fork system. There are an additional 7
+security tests, including a test proving the one-way homomorphic quality of
+ed25519 and a test proving that all symmetric script trees share the same root.
+
+## Contributing
+
+Check out the [Pycelium discord server](https://discord.gg/b2QFEJDX69). If you
+experience a problem, please discuss it on the Discord server. All suggestions
+for improvement are also welcome, and the best place for that is also Discord.
+If you experience a bug and do not use Discord, open an issue on Github.
 
 ## ISC License
 
 Copyright (c) 2024 Jonathan Voss
 
 Permission to use, copy, modify, and/or distribute this software
 for any purpose with or without fee is hereby granted, provided
```

