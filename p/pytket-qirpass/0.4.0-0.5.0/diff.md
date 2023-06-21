# Comparing `tmp/pytket-qirpass-0.4.0.tar.gz` & `tmp/pytket_qirpass-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket-qirpass-0.4.0.tar", last modified: Mon Mar 13 16:02:54 2023, max compression
+gzip compressed data, was "pytket_qirpass-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytket-qirpass-0.4.0.tar` & `pytket_qirpass-0.5.0.tar`

### file list

```diff
@@ -1,269 +1,269 @@
--rw-r--r--   0        0        0       19 2023-03-09 10:42:35.005904 pytket-qirpass-0.4.0/.gitignore
--rw-r--r--   0        0        0      330 2023-03-10 13:40:31.842135 pytket-qirpass-0.4.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    10173 2023-03-08 10:23:31.476023 pytket-qirpass-0.4.0/LICENSE
--rw-r--r--   0        0        0     1003 2023-03-10 13:40:02.929911 pytket-qirpass-0.4.0/README.md
--rw-r--r--   0        0        0      551 2023-03-13 08:20:23.015295 pytket-qirpass-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      111 2023-03-13 16:01:59.676815 pytket-qirpass-0.4.0/src/pytket_qirpass/__init__.py
--rw-r--r--   0        0        0    10720 2023-03-13 15:48:37.563827 pytket-qirpass-0.4.0/src/pytket_qirpass/apply_qirpass.py
--rw-r--r--   0        0        0       22 2023-03-10 09:23:19.543436 pytket-qirpass-0.4.0/test/__init__.py
--rw-r--r--   0        0        0     2129 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/ClassicalCircuit.ll
--rw-r--r--   0        0        0     1384 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/ClassicalReg2ConstCircuit.ll
--rw-r--r--   0        0        0      196 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/GenerateAnd.ll
--rw-r--r--   0        0        0      218 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/GenerateOr.ll
--rw-r--r--   0        0        0      219 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/GenerateXorAsBitNegation.ll
--rw-r--r--   0        0        0      241 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/GenerateXorOr.ll
--rw-r--r--   0        0        0     1540 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/NestedConditionalsCircuit.ll
--rw-r--r--   0        0        0     6629 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/RUSLoopXX-1.ll
--rw-r--r--   0        0        0      413 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/ReadResult.ll
--rw-r--r--   0        0        0     1580 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/RebasedCircuit.ll
--rw-r--r--   0        0        0     6621 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/RoundTripDiamondConditional.ll
--rw-r--r--   0        0        0     2249 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/RoundTripSimpleChain.ll
--rw-r--r--   0        0        0      291 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/RtBoolRecordOutput.ll
--rw-r--r--   0        0        0      297 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/RtIntRecordOutput.ll
--rw-r--r--   0        0        0      329 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/RtResultRecordOutput.ll
--rw-r--r--   0        0        0     1841 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/SimpleConditionalCircuit.ll
--rw-r--r--   0        0        0     3299 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/SimpleGroverBaseProfile.ll
--rw-r--r--   0        0        0     4600 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/SimpleGroverSample.BaseProfile.ll
--rw-r--r--   0        0        0     2893 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/SimpleGroverSampleOptimised.ll
--rw-r--r--   0        0        0      693 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/TestBellCircuit.ll
--rw-r--r--   0        0        0      786 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/WASM.ll
--rw-r--r--   0        0        0      325 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/WASM_noinputs.ll
--rw-r--r--   0        0        0      205 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/add_only.ll
--rw-r--r--   0        0        0      205 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/and_only.ll
--rw-r--r--   0        0        0     1362 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/classical_and_controlflow.ll
--rw-r--r--   0        0        0     4226 2023-03-10 09:23:19.551436 pytket-qirpass-0.4.0/test/qir/batch_1/collapse_jump_instr.ll
--rw-r--r--   0        0        0     2986 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/collapse_jump_left.ll
--rw-r--r--   0        0        0     2986 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/collapse_jump_right.ll
--rw-r--r--   0        0        0     5447 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/collapse_nested_jump_instr.ll
--rw-r--r--   0        0        0     3041 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/collapse_simple_instr_chain.ll
--rw-r--r--   0        0        0      399 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/cx_only.ll
--rw-r--r--   0        0        0      206 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/div_only.ll
--rw-r--r--   0        0        0      208 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/eq_only.ll
--rw-r--r--   0        0        0      339 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/h_only.ll
--rw-r--r--   0        0        0      207 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/lshr_only.ll
--rw-r--r--   0        0        0      388 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/measure_only.ll
--rw-r--r--   0        0        0      205 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/mul_only.ll
--rw-r--r--   0        0        0      205 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/neg_only.ll
--rw-r--r--   0        0        0      209 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/neq_only.ll
--rw-r--r--   0        0        0    17188 2023-03-10 11:49:24.286731 pytket-qirpass-0.4.0/test/qir/batch_1/nested_conditionals-new.ll
--rw-r--r--   0        0        0     9545 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/nested_conditionals.ll
--rw-r--r--   0        0        0     3303 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/nested_conditionals_crossed.ll
--rw-r--r--   0        0        0     3183 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/nested_conditionals_else.ll
--rw-r--r--   0        0        0     3183 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/nested_conditionals_then.ll
--rw-r--r--   0        0        0      228 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/not_supported.ll
--rw-r--r--   0        0        0     6225 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/one_conditional.ll
--rw-r--r--   0        0        0     6225 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/one_conditional_diamond.ll
--rw-r--r--   0        0        0     6225 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/one_conditional_diamond_opposite.ll
--rw-r--r--   0        0        0     5335 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/one_conditional_else.ll
--rw-r--r--   0        0        0     5335 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/one_conditional_if.ll
--rw-r--r--   0        0        0     5118 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/one_conditional_then.ll
--rw-r--r--   0        0        0      203 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/or_only.ll
--rw-r--r--   0        0        0      413 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/phasedx_only.ll
--rw-r--r--   0        0        0      404 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/purely_classical.ll
--rw-r--r--   0        0        0      347 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/reset_only.ll
--rw-r--r--   0        0        0      376 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/rx_only.ll
--rw-r--r--   0        0        0      376 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/rz_only.ll
--rw-r--r--   0        0        0      390 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/select.ll
--rw-r--r--   0        0        0      654 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/select_and_controlflow.ll
--rw-r--r--   0        0        0      205 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/shl_only.ll
--rw-r--r--   0        0        0      205 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/sub_only.ll
--rw-r--r--   0        0        0      339 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/t_only.ll
--rw-r--r--   0        0        0      337 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/tadj_only.ll
--rw-r--r--   0        0        0     2180 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/tagged_rt_functions.ll
--rw-r--r--   0        0        0     5046 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/teleportchain_baseprofile.ll
--rw-r--r--   0        0        0      210 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/uge_only.ll
--rw-r--r--   0        0        0      210 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/ugt_only.ll
--rw-r--r--   0        0        0      210 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/ule_only.ll
--rw-r--r--   0        0        0      210 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/ult_only.ll
--rw-r--r--   0        0        0     1725 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/untagged_rt_functions.ll
--rw-r--r--   0        0        0     1195 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/wasm_and_controlflow.ll
--rw-r--r--   0        0        0      322 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/wasm_only_test.ll
--rw-r--r--   0        0        0      339 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/x_only.ll
--rw-r--r--   0        0        0      205 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/xor_only.ll
--rw-r--r--   0        0        0      339 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/y_only.ll
--rw-r--r--   0        0        0      339 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/z_only.ll
--rw-r--r--   0        0        0      355 2023-03-10 09:23:19.555436 pytket-qirpass-0.4.0/test/qir/batch_1/zext.ll
--rw-r--r--   0        0        0     5810 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/1_PauliX_PauliX_.ll
--rw-r--r--   0        0        0    11396 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/2_PauliX_PauliX_.ll
--rw-r--r--   0        0        0    22634 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/3_PauliX_PauliX_.ll
--rw-r--r--   0        0        0    45178 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/4_PauliX_PauliX_.ll
--rw-r--r--   0        0        0     8802 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/ArithmeticOps.TargetedAlt_.ll
--rw-r--r--   0        0        0    50533 2023-03-10 16:19:55.250645 pytket-qirpass-0.4.0/test/qir/batch_2/Distillation.ll
--rw-r--r--   0        0        0    50533 2023-03-10 16:19:54.270638 pytket-qirpass-0.4.0/test/qir/batch_2/Distillation_other.ll
--rw-r--r--   0        0        0    12636 2023-03-10 16:19:56.430653 pytket-qirpass-0.4.0/test/qir/batch_2/Distillation_small.ll
--rw-r--r--   0        0        0    55800 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/IntegerComparison.TargetedAlt_.ll
--rw-r--r--   0        0        0    55800 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/IntegerComparison.Targeted_.ll
--rw-r--r--   0        0        0   122649 2023-03-10 16:19:55.342646 pytket-qirpass-0.4.0/test/qir/batch_2/LogicalRb-BaseProfile.opt.ll
--rw-r--r--   0        0        0    19828 2023-03-10 16:19:55.462646 pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-3X.ll
--rw-r--r--   0        0        0    32978 2023-03-10 16:19:53.238630 pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-5X.ll
--rw-r--r--   0        0        0    39601 2023-03-10 16:19:53.642633 pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-6X.ll
--rw-r--r--   0        0        0    46254 2023-03-10 16:19:57.538661 pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-7X.ll
--rw-r--r--   0        0        0    17459 2023-03-10 16:20:32.826920 pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-NoInline.10X.ll
--rw-r--r--   0        0        0    59833 2023-03-10 09:23:19.559436 pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.10X.ll
--rw-r--r--   0        0        0    26141 2023-03-10 16:19:56.562654 pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.3.ll
--rw-r--r--   0        0        0    18595 2023-03-10 09:23:19.559436 pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.3X.ll
--rw-r--r--   0        0        0    36248 2023-03-10 16:19:54.498639 pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.6X.ll
--rw-r--r--   0        0        0    48028 2023-03-10 16:19:56.342653 pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.8Y.ll
--rw-r--r--   0        0        0    53944 2023-03-10 16:19:57.438661 pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.9X.ll
--rw-r--r--   0        0        0    70809 2023-03-10 16:19:55.998650 pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.opt.ll
--rw-r--r--   0        0        0    65494 2023-03-10 09:23:19.563436 pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-Grouping.10X.ll
--rw-r--r--   0        0        0    20485 2023-03-10 09:23:19.563436 pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-Grouping.3Y.ll
--rw-r--r--   0        0        0    71671 2023-03-10 16:20:40.342975 pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation.BaseProfile-4X.ll
--rw-r--r--   0        0        0     6766 2023-03-10 09:23:19.563436 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop1.ll
--rw-r--r--   0        0        0    40822 2023-03-10 09:23:19.563436 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop10.ll
--rw-r--r--   0        0        0    44073 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop10_.ll
--rw-r--r--   0        0        0     6766 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop1_.ll
--rw-r--r--   0        0        0     9961 2023-03-10 09:23:19.563436 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop2.ll
--rw-r--r--   0        0        0     9961 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop2_.ll
--rw-r--r--   0        0        0    13980 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop3_.ll
--rw-r--r--   0        0        0    17677 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop4_.ll
--rw-r--r--   0        0        0    21373 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop5_.ll
--rw-r--r--   0        0        0    25071 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop6_.ll
--rw-r--r--   0        0        0    28771 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop7_.ll
--rw-r--r--   0        0        0    32479 2023-03-10 09:23:19.623437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop8_.ll
--rw-r--r--   0        0        0    36197 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop9_.ll
--rw-r--r--   0        0        0    40324 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-10_.ll
--rw-r--r--   0        0        0     7116 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-1_.ll
--rw-r--r--   0        0        0    10697 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-2_.ll
--rw-r--r--   0        0        0    14716 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-3_.ll
--rw-r--r--   0        0        0    18413 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-4_.ll
--rw-r--r--   0        0        0    22109 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-5_.ll
--rw-r--r--   0        0        0    25807 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-6_.ll
--rw-r--r--   0        0        0    29507 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-7_.ll
--rw-r--r--   0        0        0    33215 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-8_.ll
--rw-r--r--   0        0        0    36933 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-9_.ll
--rw-r--r--   0        0        0    38602 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-10_.ll
--rw-r--r--   0        0        0     6461 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-1_.ll
--rw-r--r--   0        0        0     9885 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-2_.ll
--rw-r--r--   0        0        0    13749 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-3_.ll
--rw-r--r--   0        0        0    17291 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-4_.ll
--rw-r--r--   0        0        0    20834 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-5_.ll
--rw-r--r--   0        0        0    24375 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-6_.ll
--rw-r--r--   0        0        0    27920 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-7_.ll
--rw-r--r--   0        0        0    31473 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-8_.ll
--rw-r--r--   0        0        0    35036 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-9_.ll
--rw-r--r--   0        0        0    16264 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/RandomWalkPE1.baseProfile.ll
--rw-r--r--   0        0        0     3452 2023-03-10 16:19:55.138644 pytket-qirpass-0.4.0/test/qir/batch_2/SimpleGroverBaseProfile.ll
--rw-r--r--   0        0        0     3922 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/SimpleGroverGrouped.ll
--rw-r--r--   0        0        0     4419 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/SimpleGroverSample.BaseProfile.ll
--rw-r--r--   0        0        0    10195 2023-03-10 16:20:48.275033 pytket-qirpass-0.4.0/test/qir/batch_2/SimpleGroverSample.O1.ll
--rw-r--r--   0        0        0   184385 2023-03-10 16:20:51.671058 pytket-qirpass-0.4.0/test/qir/batch_2/SimpleGroverSample.ll
--rw-r--r--   0        0        0   729811 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/XX_recursion_limit8.ll
--rw-r--r--   0        0        0      277 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/add_only.ll
--rw-r--r--   0        0        0      277 2023-03-10 16:19:53.302631 pytket-qirpass-0.4.0/test/qir/batch_2/and_only.ll
--rw-r--r--   0        0        0      332 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/bad_div.ll
--rw-r--r--   0        0        0     2072 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/bool_tag.ll
--rw-r--r--   0        0        0      685 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/classical_flow.ll
--rw-r--r--   0        0        0      613 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/classical_flow2.ll
--rw-r--r--   0        0        0      795 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/classical_flow3.ll
--rw-r--r--   0        0        0      795 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/classical_flow4.ll
--rw-r--r--   0        0        0      971 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/classical_flow5.ll
--rw-r--r--   0        0        0      971 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/classical_flow6.ll
--rw-r--r--   0        0        0      428 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/comparison_instrs.ll
--rw-r--r--   0        0        0      975 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/cond_ops.ll
--rw-r--r--   0        0        0     6747 2023-03-10 16:19:56.226652 pytket-qirpass-0.4.0/test/qir/batch_2/conditional-test-3.ll
--rw-r--r--   0        0        0     5770 2023-03-10 16:19:57.650662 pytket-qirpass-0.4.0/test/qir/batch_2/conditional_test.ll
--rw-r--r--   0        0        0     5932 2023-03-10 16:19:53.858635 pytket-qirpass-0.4.0/test/qir/batch_2/conditional_test_2.ll
--rw-r--r--   0        0        0     8760 2023-03-10 16:19:57.222659 pytket-qirpass-0.4.0/test/qir/batch_2/conditional_test_3.ll
--rw-r--r--   0        0        0     8760 2023-03-10 16:19:55.550647 pytket-qirpass-0.4.0/test/qir/batch_2/conditional_test_4.ll
--rw-r--r--   0        0        0     2506 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/control_flow_complex.baseProfile.ll
--rw-r--r--   0        0        0     2276 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/control_flow_long.baseProfile.ll
--rw-r--r--   0        0        0     3048 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/control_flow_nested.baseProfile.ll
--rw-r--r--   0        0        0     3819 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/control_flow_short.baseProfile.ll
--rw-r--r--   0        0        0      446 2023-03-10 09:23:19.567436 pytket-qirpass-0.4.0/test/qir/batch_2/cx_only.ll
--rw-r--r--   0        0        0      281 2023-03-10 16:19:54.182637 pytket-qirpass-0.4.0/test/qir/batch_2/eq_only.ll
--rw-r--r--   0        0        0     4644 2023-03-10 16:19:56.794656 pytket-qirpass-0.4.0/test/qir/batch_2/fallthrough_simple.ll
--rw-r--r--   0        0        0     6958 2023-03-10 09:23:19.571436 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_5qb.ll
--rw-r--r--   0        0        0    18595 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_5qb_.ll
--rw-r--r--   0        0        0   448873 2023-03-10 09:23:19.571436 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test.ll
--rw-r--r--   0        0        0     2612 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_.ll
--rw-r--r--   0        0        0   896353 2023-03-10 09:23:19.571436 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_10k.ll
--rw-r--r--   0        0        0   448873 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_10k_.ll
--rw-r--r--   0        0        0   503842 2023-03-10 09:23:19.571436 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_10qb.ll
--rw-r--r--   0        0        0     6958 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_10qb_.ll
--rw-r--r--   0        0        0  1130427 2023-03-10 09:23:19.575436 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_10qb_10k.ll
--rw-r--r--   0        0        0   503842 2023-03-10 09:23:19.627437 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_10qb_10k_.ll
--rw-r--r--   0        0        0  1342733 2023-03-10 09:23:19.579436 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_15k.ll
--rw-r--r--   0        0        0   896353 2023-03-10 09:23:19.631437 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_15k_.ll
--rw-r--r--   0        0        0  1799516 2023-03-10 09:23:19.583436 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_20k.ll
--rw-r--r--   0        0        0  1342733 2023-03-10 09:23:19.631437 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_20k_.ll
--rw-r--r--   0        0        0  2267488 2023-03-10 09:23:19.587436 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_25k.ll
--rw-r--r--   0        0        0  1799516 2023-03-10 09:23:19.635437 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_25k_.ll
--rw-r--r--   0        0        0  4533587 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_50k.ll
--rw-r--r--   0        0        0      282 2023-03-10 16:19:56.114651 pytket-qirpass-0.4.0/test/qir/batch_2/ge_only.ll
--rw-r--r--   0        0        0     3322 2023-03-10 09:23:19.635437 pytket-qirpass-0.4.0/test/qir/batch_2/ghz_fail_.ll
--rw-r--r--   0        0        0      282 2023-03-10 16:19:56.890657 pytket-qirpass-0.4.0/test/qir/batch_2/gt_only.ll
--rw-r--r--   0        0        0      386 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/h_only.ll
--rw-r--r--   0        0        0      341 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/int_record_out.ll
--rw-r--r--   0        0        0      559 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/int_result_with_tag.ll
--rw-r--r--   0        0        0     1847 2023-03-10 09:23:19.635437 pytket-qirpass-0.4.0/test/qir/batch_2/int_tag_alt_.ll
--rw-r--r--   0        0        0    12077 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/iqpe.ll
--rw-r--r--   0        0        0    12077 2023-03-10 09:23:19.635437 pytket-qirpass-0.4.0/test/qir/batch_2/iqpe_.ll
--rw-r--r--   0        0        0      282 2023-03-10 16:19:54.610640 pytket-qirpass-0.4.0/test/qir/batch_2/le_only.ll
--rw-r--r--   0        0        0     7399 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/loopRecursion.baseProfile.ll
--rw-r--r--   0        0        0      279 2023-03-10 16:19:53.966635 pytket-qirpass-0.4.0/test/qir/batch_2/lshr_only.ll
--rw-r--r--   0        0        0      282 2023-03-10 16:19:57.102658 pytket-qirpass-0.4.0/test/qir/batch_2/lt_only.ll
--rw-r--r--   0        0        0     2612 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/many_gates.baseProfile.ll
--rw-r--r--   0        0        0     1024 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/many_ops.ll
--rw-r--r--   0        0        0      419 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/measure_only.ll
--rw-r--r--   0        0        0      693 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/measure_result.ll
--rw-r--r--   0        0        0     2269 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/most_features.ll
--rw-r--r--   0        0        0     1348 2023-03-10 09:23:19.635437 pytket-qirpass-0.4.0/test/qir/batch_2/most_features_.ll
--rw-r--r--   0        0        0      277 2023-03-10 16:19:54.390638 pytket-qirpass-0.4.0/test/qir/batch_2/mul_only.ll
--rw-r--r--   0        0        0      618 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/multi_arith.ll
--rw-r--r--   0        0        0    13223 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/mutables_ops_branches.baseProfile.ll
--rw-r--r--   0        0        0     1578 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/native_gates.ll
--rw-r--r--   0        0        0      281 2023-03-10 16:19:55.890649 pytket-qirpass-0.4.0/test/qir/batch_2/ne_only.ll
--rw-r--r--   0        0        0      887 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/negative_arith.ll
--rw-r--r--   0        0        0    10035 2023-03-10 09:23:19.595436 pytket-qirpass-0.4.0/test/qir/batch_2/nested_conditions.ll
--rw-r--r--   0        0        0     1237 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/no-ops.ll
--rw-r--r--   0        0        0      370 2023-03-10 16:19:55.034643 pytket-qirpass-0.4.0/test/qir/batch_2/no_entry.ll
--rw-r--r--   0        0        0      315 2023-03-10 16:19:54.930642 pytket-qirpass-0.4.0/test/qir/batch_2/no_qubits.ll
--rw-r--r--   0        0        0      316 2023-03-10 16:19:54.826642 pytket-qirpass-0.4.0/test/qir/batch_2/no_results.ll
--rw-r--r--   0        0        0      361 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/null_tag.ll
--rw-r--r--   0        0        0     5770 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/one_conditional.ll
--rw-r--r--   0        0        0      276 2023-03-10 16:19:55.670648 pytket-qirpass-0.4.0/test/qir/batch_2/or_only.ll
--rw-r--r--   0        0        0      684 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_1.ll
--rw-r--r--   0        0        0      727 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_2.ll
--rw-r--r--   0        0        0      902 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_3.ll
--rw-r--r--   0        0        0      902 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_4.ll
--rw-r--r--   0        0        0      902 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_5.ll
--rw-r--r--   0        0        0     1259 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_6.ll
--rw-r--r--   0        0        0     1259 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_7.ll
--rw-r--r--   0        0        0     1259 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_8.ll
--rw-r--r--   0        0        0     1217 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/qir_hybrid.ll
--rw-r--r--   0        0        0      394 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/reset_only.ll
--rw-r--r--   0        0        0     1892 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/result_tag.ll
--rw-r--r--   0        0        0     1708 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/result_tag_alt.ll
--rw-r--r--   0        0        0     1713 2023-03-10 09:23:19.635437 pytket-qirpass-0.4.0/test/qir/batch_2/result_tag_alt_.ll
--rw-r--r--   0        0        0      529 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/result_with_constant_args.ll
--rw-r--r--   0        0        0      423 2023-03-10 16:19:57.742663 pytket-qirpass-0.4.0/test/qir/batch_2/rx_only.ll
--rw-r--r--   0        0        0      423 2023-03-10 16:19:53.534632 pytket-qirpass-0.4.0/test/qir/batch_2/rz_only.ll
--rw-r--r--   0        0        0      553 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/select-nested-const-cond.ll
--rw-r--r--   0        0        0      661 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/select-nested.ll
--rw-r--r--   0        0        0      443 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/select.ll
--rw-r--r--   0        0        0      995 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/sequential_flow_1.ll
--rw-r--r--   0        0        0      992 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/sequential_flow_2.ll
--rw-r--r--   0        0        0      498 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/sge.ll
--rw-r--r--   0        0        0      498 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/sgt.ll
--rw-r--r--   0        0        0      277 2023-03-10 16:19:57.314660 pytket-qirpass-0.4.0/test/qir/batch_2/shl_only.ll
--rw-r--r--   0        0        0      498 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/sle.ll
--rw-r--r--   0        0        0      498 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/slt.ll
--rw-r--r--   0        0        0      277 2023-03-10 16:19:53.750634 pytket-qirpass-0.4.0/test/qir/batch_2/sub_only.ll
--rw-r--r--   0        0        0      386 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/t_only.ll
--rw-r--r--   0        0        0      384 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/tadj_only.ll
--rw-r--r--   0        0        0      761 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/tagged_duplicates.ll
--rw-r--r--   0        0        0      761 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/tagged_result_control_flow.ll
--rw-r--r--   0        0        0      559 2023-03-10 09:23:19.635437 pytket-qirpass-0.4.0/test/qir/batch_2/tagged_result_control_flow_.ll
--rw-r--r--   0        0        0     9157 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/teleport-chain-grouping.ll
--rw-r--r--   0        0        0     6421 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/teleportchain.BaseProfile.ll
--rw-r--r--   0        0        0      278 2023-03-10 16:19:56.654655 pytket-qirpass-0.4.0/test/qir/batch_2/udiv_only.ll
--rw-r--r--   0        0        0      386 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/x_only.ll
--rw-r--r--   0        0        0      277 2023-03-10 16:19:57.010658 pytket-qirpass-0.4.0/test/qir/batch_2/xor_only.ll
--rw-r--r--   0        0        0      386 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/y_only.ll
--rw-r--r--   0        0        0      386 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/z_only.ll
--rw-r--r--   0        0        0      431 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/zext-reg.ll
--rw-r--r--   0        0        0      456 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/zext-use.ll
--rw-r--r--   0        0        0      412 2023-03-10 09:23:19.599436 pytket-qirpass-0.4.0/test/qir/batch_2/zext.ll
--rw-r--r--   0        0        0     8335 2023-03-13 15:52:59.001383 pytket-qirpass-0.4.0/test/test_qirpass.py
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 pytket-qirpass-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-03-09 10:42:35.005904 pytket_qirpass-0.5.0/.gitignore
+-rw-r--r--   0        0        0      330 2023-03-10 13:40:31.842135 pytket_qirpass-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    10173 2023-03-08 10:23:31.476023 pytket_qirpass-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1003 2023-03-10 13:40:02.929911 pytket_qirpass-0.5.0/README.md
+-rw-r--r--   0        0        0      553 2023-06-20 16:19:26.334825 pytket_qirpass-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-06-21 06:44:08.289647 pytket_qirpass-0.5.0/src/pytket_qirpass/__init__.py
+-rw-r--r--   0        0        0    10924 2023-06-20 19:45:58.502999 pytket_qirpass-0.5.0/src/pytket_qirpass/apply_qirpass.py
+-rw-r--r--   0        0        0       22 2023-03-10 09:23:19.543436 pytket_qirpass-0.5.0/test/__init__.py
+-rw-r--r--   0        0        0     2129 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/ClassicalCircuit.ll
+-rw-r--r--   0        0        0     1384 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/ClassicalReg2ConstCircuit.ll
+-rw-r--r--   0        0        0      196 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/GenerateAnd.ll
+-rw-r--r--   0        0        0      218 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/GenerateOr.ll
+-rw-r--r--   0        0        0      219 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/GenerateXorAsBitNegation.ll
+-rw-r--r--   0        0        0      241 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/GenerateXorOr.ll
+-rw-r--r--   0        0        0     1540 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/NestedConditionalsCircuit.ll
+-rw-r--r--   0        0        0     6629 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/RUSLoopXX-1.ll
+-rw-r--r--   0        0        0      413 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/ReadResult.ll
+-rw-r--r--   0        0        0     1580 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/RebasedCircuit.ll
+-rw-r--r--   0        0        0     6621 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/RoundTripDiamondConditional.ll
+-rw-r--r--   0        0        0     2249 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/RoundTripSimpleChain.ll
+-rw-r--r--   0        0        0      291 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/RtBoolRecordOutput.ll
+-rw-r--r--   0        0        0      297 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/RtIntRecordOutput.ll
+-rw-r--r--   0        0        0      329 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/RtResultRecordOutput.ll
+-rw-r--r--   0        0        0     1841 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/SimpleConditionalCircuit.ll
+-rw-r--r--   0        0        0     3299 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/SimpleGroverBaseProfile.ll
+-rw-r--r--   0        0        0     4600 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/SimpleGroverSample.BaseProfile.ll
+-rw-r--r--   0        0        0     2893 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/SimpleGroverSampleOptimised.ll
+-rw-r--r--   0        0        0      693 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/TestBellCircuit.ll
+-rw-r--r--   0        0        0      786 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/WASM.ll
+-rw-r--r--   0        0        0      325 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/WASM_noinputs.ll
+-rw-r--r--   0        0        0      205 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/add_only.ll
+-rw-r--r--   0        0        0      205 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/and_only.ll
+-rw-r--r--   0        0        0     1362 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/classical_and_controlflow.ll
+-rw-r--r--   0        0        0     4226 2023-03-10 09:23:19.551436 pytket_qirpass-0.5.0/test/qir/batch_1/collapse_jump_instr.ll
+-rw-r--r--   0        0        0     2986 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/collapse_jump_left.ll
+-rw-r--r--   0        0        0     2986 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/collapse_jump_right.ll
+-rw-r--r--   0        0        0     5447 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/collapse_nested_jump_instr.ll
+-rw-r--r--   0        0        0     3041 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/collapse_simple_instr_chain.ll
+-rw-r--r--   0        0        0      399 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/cx_only.ll
+-rw-r--r--   0        0        0      206 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/div_only.ll
+-rw-r--r--   0        0        0      208 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/eq_only.ll
+-rw-r--r--   0        0        0      339 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/h_only.ll
+-rw-r--r--   0        0        0      207 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/lshr_only.ll
+-rw-r--r--   0        0        0      388 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/measure_only.ll
+-rw-r--r--   0        0        0      205 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/mul_only.ll
+-rw-r--r--   0        0        0      205 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/neg_only.ll
+-rw-r--r--   0        0        0      209 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/neq_only.ll
+-rw-r--r--   0        0        0    17188 2023-03-10 11:49:24.286731 pytket_qirpass-0.5.0/test/qir/batch_1/nested_conditionals-new.ll
+-rw-r--r--   0        0        0     9545 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/nested_conditionals.ll
+-rw-r--r--   0        0        0     3303 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/nested_conditionals_crossed.ll
+-rw-r--r--   0        0        0     3183 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/nested_conditionals_else.ll
+-rw-r--r--   0        0        0     3183 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/nested_conditionals_then.ll
+-rw-r--r--   0        0        0      228 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/not_supported.ll
+-rw-r--r--   0        0        0     6225 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/one_conditional.ll
+-rw-r--r--   0        0        0     6225 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/one_conditional_diamond.ll
+-rw-r--r--   0        0        0     6225 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/one_conditional_diamond_opposite.ll
+-rw-r--r--   0        0        0     5335 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/one_conditional_else.ll
+-rw-r--r--   0        0        0     5335 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/one_conditional_if.ll
+-rw-r--r--   0        0        0     5118 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/one_conditional_then.ll
+-rw-r--r--   0        0        0      203 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/or_only.ll
+-rw-r--r--   0        0        0      413 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/phasedx_only.ll
+-rw-r--r--   0        0        0      404 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/purely_classical.ll
+-rw-r--r--   0        0        0      347 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/reset_only.ll
+-rw-r--r--   0        0        0      376 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/rx_only.ll
+-rw-r--r--   0        0        0      376 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/rz_only.ll
+-rw-r--r--   0        0        0      390 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/select.ll
+-rw-r--r--   0        0        0      654 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/select_and_controlflow.ll
+-rw-r--r--   0        0        0      205 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/shl_only.ll
+-rw-r--r--   0        0        0      205 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/sub_only.ll
+-rw-r--r--   0        0        0      339 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/t_only.ll
+-rw-r--r--   0        0        0      337 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/tadj_only.ll
+-rw-r--r--   0        0        0     2180 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/tagged_rt_functions.ll
+-rw-r--r--   0        0        0     5046 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/teleportchain_baseprofile.ll
+-rw-r--r--   0        0        0      210 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/uge_only.ll
+-rw-r--r--   0        0        0      210 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/ugt_only.ll
+-rw-r--r--   0        0        0      210 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/ule_only.ll
+-rw-r--r--   0        0        0      210 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/ult_only.ll
+-rw-r--r--   0        0        0     1725 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/untagged_rt_functions.ll
+-rw-r--r--   0        0        0     1195 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/wasm_and_controlflow.ll
+-rw-r--r--   0        0        0      322 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/wasm_only_test.ll
+-rw-r--r--   0        0        0      339 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/x_only.ll
+-rw-r--r--   0        0        0      205 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/xor_only.ll
+-rw-r--r--   0        0        0      339 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/y_only.ll
+-rw-r--r--   0        0        0      339 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/z_only.ll
+-rw-r--r--   0        0        0      355 2023-03-10 09:23:19.555436 pytket_qirpass-0.5.0/test/qir/batch_1/zext.ll
+-rw-r--r--   0        0        0     5810 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/1_PauliX_PauliX_.ll
+-rw-r--r--   0        0        0    11396 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/2_PauliX_PauliX_.ll
+-rw-r--r--   0        0        0    22634 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/3_PauliX_PauliX_.ll
+-rw-r--r--   0        0        0    45178 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/4_PauliX_PauliX_.ll
+-rw-r--r--   0        0        0     8802 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/ArithmeticOps.TargetedAlt_.ll
+-rw-r--r--   0        0        0    50533 2023-03-10 16:19:55.250645 pytket_qirpass-0.5.0/test/qir/batch_2/Distillation.ll
+-rw-r--r--   0        0        0    50533 2023-03-10 16:19:54.270638 pytket_qirpass-0.5.0/test/qir/batch_2/Distillation_other.ll
+-rw-r--r--   0        0        0    12636 2023-03-10 16:19:56.430653 pytket_qirpass-0.5.0/test/qir/batch_2/Distillation_small.ll
+-rw-r--r--   0        0        0    55800 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/IntegerComparison.TargetedAlt_.ll
+-rw-r--r--   0        0        0    55800 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/IntegerComparison.Targeted_.ll
+-rw-r--r--   0        0        0   122649 2023-03-10 16:19:55.342646 pytket_qirpass-0.5.0/test/qir/batch_2/LogicalRb-BaseProfile.opt.ll
+-rw-r--r--   0        0        0    19828 2023-03-10 16:19:55.462646 pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-3X.ll
+-rw-r--r--   0        0        0    32978 2023-03-10 16:19:53.238630 pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-5X.ll
+-rw-r--r--   0        0        0    39601 2023-03-10 16:19:53.642633 pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-6X.ll
+-rw-r--r--   0        0        0    46254 2023-03-10 16:19:57.538661 pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-7X.ll
+-rw-r--r--   0        0        0    17459 2023-03-10 16:20:32.826920 pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-NoInline.10X.ll
+-rw-r--r--   0        0        0    59833 2023-03-10 09:23:19.559436 pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.10X.ll
+-rw-r--r--   0        0        0    26141 2023-03-10 16:19:56.562654 pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.3.ll
+-rw-r--r--   0        0        0    18595 2023-03-10 09:23:19.559436 pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.3X.ll
+-rw-r--r--   0        0        0    36248 2023-03-10 16:19:54.498639 pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.6X.ll
+-rw-r--r--   0        0        0    48028 2023-03-10 16:19:56.342653 pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.8Y.ll
+-rw-r--r--   0        0        0    53944 2023-03-10 16:19:57.438661 pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.9X.ll
+-rw-r--r--   0        0        0    70809 2023-03-10 16:19:55.998650 pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.opt.ll
+-rw-r--r--   0        0        0    65494 2023-03-10 09:23:19.563436 pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-Grouping.10X.ll
+-rw-r--r--   0        0        0    20485 2023-03-10 09:23:19.563436 pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-Grouping.3Y.ll
+-rw-r--r--   0        0        0    71671 2023-03-10 16:20:40.342975 pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation.BaseProfile-4X.ll
+-rw-r--r--   0        0        0     6766 2023-03-10 09:23:19.563436 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop1.ll
+-rw-r--r--   0        0        0    40822 2023-03-10 09:23:19.563436 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop10.ll
+-rw-r--r--   0        0        0    44073 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop10_.ll
+-rw-r--r--   0        0        0     6766 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop1_.ll
+-rw-r--r--   0        0        0     9961 2023-03-10 09:23:19.563436 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop2.ll
+-rw-r--r--   0        0        0     9961 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop2_.ll
+-rw-r--r--   0        0        0    13980 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop3_.ll
+-rw-r--r--   0        0        0    17677 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop4_.ll
+-rw-r--r--   0        0        0    21373 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop5_.ll
+-rw-r--r--   0        0        0    25071 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop6_.ll
+-rw-r--r--   0        0        0    28771 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop7_.ll
+-rw-r--r--   0        0        0    32479 2023-03-10 09:23:19.623437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop8_.ll
+-rw-r--r--   0        0        0    36197 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop9_.ll
+-rw-r--r--   0        0        0    40324 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-10_.ll
+-rw-r--r--   0        0        0     7116 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-1_.ll
+-rw-r--r--   0        0        0    10697 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-2_.ll
+-rw-r--r--   0        0        0    14716 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-3_.ll
+-rw-r--r--   0        0        0    18413 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-4_.ll
+-rw-r--r--   0        0        0    22109 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-5_.ll
+-rw-r--r--   0        0        0    25807 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-6_.ll
+-rw-r--r--   0        0        0    29507 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-7_.ll
+-rw-r--r--   0        0        0    33215 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-8_.ll
+-rw-r--r--   0        0        0    36933 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-9_.ll
+-rw-r--r--   0        0        0    38602 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-10_.ll
+-rw-r--r--   0        0        0     6461 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-1_.ll
+-rw-r--r--   0        0        0     9885 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-2_.ll
+-rw-r--r--   0        0        0    13749 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-3_.ll
+-rw-r--r--   0        0        0    17291 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-4_.ll
+-rw-r--r--   0        0        0    20834 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-5_.ll
+-rw-r--r--   0        0        0    24375 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-6_.ll
+-rw-r--r--   0        0        0    27920 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-7_.ll
+-rw-r--r--   0        0        0    31473 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-8_.ll
+-rw-r--r--   0        0        0    35036 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-9_.ll
+-rw-r--r--   0        0        0    16264 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/RandomWalkPE1.baseProfile.ll
+-rw-r--r--   0        0        0     3452 2023-03-10 16:19:55.138644 pytket_qirpass-0.5.0/test/qir/batch_2/SimpleGroverBaseProfile.ll
+-rw-r--r--   0        0        0     3922 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/SimpleGroverGrouped.ll
+-rw-r--r--   0        0        0     4419 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/SimpleGroverSample.BaseProfile.ll
+-rw-r--r--   0        0        0    10195 2023-03-10 16:20:48.275033 pytket_qirpass-0.5.0/test/qir/batch_2/SimpleGroverSample.O1.ll
+-rw-r--r--   0        0        0   184385 2023-03-10 16:20:51.671058 pytket_qirpass-0.5.0/test/qir/batch_2/SimpleGroverSample.ll
+-rw-r--r--   0        0        0   729811 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/XX_recursion_limit8.ll
+-rw-r--r--   0        0        0      277 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/add_only.ll
+-rw-r--r--   0        0        0      277 2023-03-10 16:19:53.302631 pytket_qirpass-0.5.0/test/qir/batch_2/and_only.ll
+-rw-r--r--   0        0        0      332 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/bad_div.ll
+-rw-r--r--   0        0        0     2072 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/bool_tag.ll
+-rw-r--r--   0        0        0      685 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/classical_flow.ll
+-rw-r--r--   0        0        0      613 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/classical_flow2.ll
+-rw-r--r--   0        0        0      795 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/classical_flow3.ll
+-rw-r--r--   0        0        0      795 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/classical_flow4.ll
+-rw-r--r--   0        0        0      971 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/classical_flow5.ll
+-rw-r--r--   0        0        0      971 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/classical_flow6.ll
+-rw-r--r--   0        0        0      428 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/comparison_instrs.ll
+-rw-r--r--   0        0        0      975 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/cond_ops.ll
+-rw-r--r--   0        0        0     6747 2023-03-10 16:19:56.226652 pytket_qirpass-0.5.0/test/qir/batch_2/conditional-test-3.ll
+-rw-r--r--   0        0        0     5770 2023-03-10 16:19:57.650662 pytket_qirpass-0.5.0/test/qir/batch_2/conditional_test.ll
+-rw-r--r--   0        0        0     5932 2023-03-10 16:19:53.858635 pytket_qirpass-0.5.0/test/qir/batch_2/conditional_test_2.ll
+-rw-r--r--   0        0        0     8760 2023-03-10 16:19:57.222659 pytket_qirpass-0.5.0/test/qir/batch_2/conditional_test_3.ll
+-rw-r--r--   0        0        0     8760 2023-03-10 16:19:55.550647 pytket_qirpass-0.5.0/test/qir/batch_2/conditional_test_4.ll
+-rw-r--r--   0        0        0     2506 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/control_flow_complex.baseProfile.ll
+-rw-r--r--   0        0        0     2276 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/control_flow_long.baseProfile.ll
+-rw-r--r--   0        0        0     3048 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/control_flow_nested.baseProfile.ll
+-rw-r--r--   0        0        0     3819 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/control_flow_short.baseProfile.ll
+-rw-r--r--   0        0        0      446 2023-03-10 09:23:19.567436 pytket_qirpass-0.5.0/test/qir/batch_2/cx_only.ll
+-rw-r--r--   0        0        0      281 2023-03-10 16:19:54.182637 pytket_qirpass-0.5.0/test/qir/batch_2/eq_only.ll
+-rw-r--r--   0        0        0     4644 2023-03-10 16:19:56.794656 pytket_qirpass-0.5.0/test/qir/batch_2/fallthrough_simple.ll
+-rw-r--r--   0        0        0     6958 2023-03-10 09:23:19.571436 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_5qb.ll
+-rw-r--r--   0        0        0    18595 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_5qb_.ll
+-rw-r--r--   0        0        0   448873 2023-03-10 09:23:19.571436 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test.ll
+-rw-r--r--   0        0        0     2612 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_.ll
+-rw-r--r--   0        0        0   896353 2023-03-10 09:23:19.571436 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_10k.ll
+-rw-r--r--   0        0        0   448873 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_10k_.ll
+-rw-r--r--   0        0        0   503842 2023-03-10 09:23:19.571436 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_10qb.ll
+-rw-r--r--   0        0        0     6958 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_10qb_.ll
+-rw-r--r--   0        0        0  1130427 2023-03-10 09:23:19.575436 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_10qb_10k.ll
+-rw-r--r--   0        0        0   503842 2023-03-10 09:23:19.627437 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_10qb_10k_.ll
+-rw-r--r--   0        0        0  1342733 2023-03-10 09:23:19.579436 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_15k.ll
+-rw-r--r--   0        0        0   896353 2023-03-10 09:23:19.631437 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_15k_.ll
+-rw-r--r--   0        0        0  1799516 2023-03-10 09:23:19.583436 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_20k.ll
+-rw-r--r--   0        0        0  1342733 2023-03-10 09:23:19.631437 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_20k_.ll
+-rw-r--r--   0        0        0  2267488 2023-03-10 09:23:19.587436 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_25k.ll
+-rw-r--r--   0        0        0  1799516 2023-03-10 09:23:19.635437 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_25k_.ll
+-rw-r--r--   0        0        0  4533587 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_50k.ll
+-rw-r--r--   0        0        0      282 2023-03-10 16:19:56.114651 pytket_qirpass-0.5.0/test/qir/batch_2/ge_only.ll
+-rw-r--r--   0        0        0     3322 2023-03-10 09:23:19.635437 pytket_qirpass-0.5.0/test/qir/batch_2/ghz_fail_.ll
+-rw-r--r--   0        0        0      282 2023-03-10 16:19:56.890657 pytket_qirpass-0.5.0/test/qir/batch_2/gt_only.ll
+-rw-r--r--   0        0        0      386 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/h_only.ll
+-rw-r--r--   0        0        0      341 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/int_record_out.ll
+-rw-r--r--   0        0        0      559 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/int_result_with_tag.ll
+-rw-r--r--   0        0        0     1847 2023-03-10 09:23:19.635437 pytket_qirpass-0.5.0/test/qir/batch_2/int_tag_alt_.ll
+-rw-r--r--   0        0        0    12077 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/iqpe.ll
+-rw-r--r--   0        0        0    12077 2023-03-10 09:23:19.635437 pytket_qirpass-0.5.0/test/qir/batch_2/iqpe_.ll
+-rw-r--r--   0        0        0      282 2023-03-10 16:19:54.610640 pytket_qirpass-0.5.0/test/qir/batch_2/le_only.ll
+-rw-r--r--   0        0        0     7399 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/loopRecursion.baseProfile.ll
+-rw-r--r--   0        0        0      279 2023-03-10 16:19:53.966635 pytket_qirpass-0.5.0/test/qir/batch_2/lshr_only.ll
+-rw-r--r--   0        0        0      282 2023-03-10 16:19:57.102658 pytket_qirpass-0.5.0/test/qir/batch_2/lt_only.ll
+-rw-r--r--   0        0        0     2612 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/many_gates.baseProfile.ll
+-rw-r--r--   0        0        0     1024 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/many_ops.ll
+-rw-r--r--   0        0        0      419 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/measure_only.ll
+-rw-r--r--   0        0        0      693 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/measure_result.ll
+-rw-r--r--   0        0        0     2269 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/most_features.ll
+-rw-r--r--   0        0        0     1348 2023-03-10 09:23:19.635437 pytket_qirpass-0.5.0/test/qir/batch_2/most_features_.ll
+-rw-r--r--   0        0        0      277 2023-03-10 16:19:54.390638 pytket_qirpass-0.5.0/test/qir/batch_2/mul_only.ll
+-rw-r--r--   0        0        0      618 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/multi_arith.ll
+-rw-r--r--   0        0        0    13223 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/mutables_ops_branches.baseProfile.ll
+-rw-r--r--   0        0        0     1578 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/native_gates.ll
+-rw-r--r--   0        0        0      281 2023-03-10 16:19:55.890649 pytket_qirpass-0.5.0/test/qir/batch_2/ne_only.ll
+-rw-r--r--   0        0        0      887 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/negative_arith.ll
+-rw-r--r--   0        0        0    10035 2023-03-10 09:23:19.595436 pytket_qirpass-0.5.0/test/qir/batch_2/nested_conditions.ll
+-rw-r--r--   0        0        0     1237 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/no-ops.ll
+-rw-r--r--   0        0        0      370 2023-03-10 16:19:55.034643 pytket_qirpass-0.5.0/test/qir/batch_2/no_entry.ll
+-rw-r--r--   0        0        0      315 2023-03-10 16:19:54.930642 pytket_qirpass-0.5.0/test/qir/batch_2/no_qubits.ll
+-rw-r--r--   0        0        0      316 2023-03-10 16:19:54.826642 pytket_qirpass-0.5.0/test/qir/batch_2/no_results.ll
+-rw-r--r--   0        0        0      361 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/null_tag.ll
+-rw-r--r--   0        0        0     5770 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/one_conditional.ll
+-rw-r--r--   0        0        0      276 2023-03-10 16:19:55.670648 pytket_qirpass-0.5.0/test/qir/batch_2/or_only.ll
+-rw-r--r--   0        0        0      684 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_1.ll
+-rw-r--r--   0        0        0      727 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_2.ll
+-rw-r--r--   0        0        0      902 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_3.ll
+-rw-r--r--   0        0        0      902 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_4.ll
+-rw-r--r--   0        0        0      902 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_5.ll
+-rw-r--r--   0        0        0     1259 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_6.ll
+-rw-r--r--   0        0        0     1259 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_7.ll
+-rw-r--r--   0        0        0     1259 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_8.ll
+-rw-r--r--   0        0        0     1217 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/qir_hybrid.ll
+-rw-r--r--   0        0        0      394 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/reset_only.ll
+-rw-r--r--   0        0        0     1892 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/result_tag.ll
+-rw-r--r--   0        0        0     1708 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/result_tag_alt.ll
+-rw-r--r--   0        0        0     1713 2023-03-10 09:23:19.635437 pytket_qirpass-0.5.0/test/qir/batch_2/result_tag_alt_.ll
+-rw-r--r--   0        0        0      529 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/result_with_constant_args.ll
+-rw-r--r--   0        0        0      423 2023-03-10 16:19:57.742663 pytket_qirpass-0.5.0/test/qir/batch_2/rx_only.ll
+-rw-r--r--   0        0        0      423 2023-03-10 16:19:53.534632 pytket_qirpass-0.5.0/test/qir/batch_2/rz_only.ll
+-rw-r--r--   0        0        0      553 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/select-nested-const-cond.ll
+-rw-r--r--   0        0        0      661 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/select-nested.ll
+-rw-r--r--   0        0        0      443 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/select.ll
+-rw-r--r--   0        0        0      995 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/sequential_flow_1.ll
+-rw-r--r--   0        0        0      992 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/sequential_flow_2.ll
+-rw-r--r--   0        0        0      498 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/sge.ll
+-rw-r--r--   0        0        0      498 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/sgt.ll
+-rw-r--r--   0        0        0      277 2023-03-10 16:19:57.314660 pytket_qirpass-0.5.0/test/qir/batch_2/shl_only.ll
+-rw-r--r--   0        0        0      498 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/sle.ll
+-rw-r--r--   0        0        0      498 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/slt.ll
+-rw-r--r--   0        0        0      277 2023-03-10 16:19:53.750634 pytket_qirpass-0.5.0/test/qir/batch_2/sub_only.ll
+-rw-r--r--   0        0        0      386 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/t_only.ll
+-rw-r--r--   0        0        0      384 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/tadj_only.ll
+-rw-r--r--   0        0        0      761 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/tagged_duplicates.ll
+-rw-r--r--   0        0        0      761 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/tagged_result_control_flow.ll
+-rw-r--r--   0        0        0      559 2023-03-10 09:23:19.635437 pytket_qirpass-0.5.0/test/qir/batch_2/tagged_result_control_flow_.ll
+-rw-r--r--   0        0        0     9157 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/teleport-chain-grouping.ll
+-rw-r--r--   0        0        0     6421 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/teleportchain.BaseProfile.ll
+-rw-r--r--   0        0        0      278 2023-03-10 16:19:56.654655 pytket_qirpass-0.5.0/test/qir/batch_2/udiv_only.ll
+-rw-r--r--   0        0        0      386 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/x_only.ll
+-rw-r--r--   0        0        0      277 2023-03-10 16:19:57.010658 pytket_qirpass-0.5.0/test/qir/batch_2/xor_only.ll
+-rw-r--r--   0        0        0      386 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/y_only.ll
+-rw-r--r--   0        0        0      386 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/z_only.ll
+-rw-r--r--   0        0        0      431 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/zext-reg.ll
+-rw-r--r--   0        0        0      456 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/zext-use.ll
+-rw-r--r--   0        0        0      412 2023-03-10 09:23:19.599436 pytket_qirpass-0.5.0/test/qir/batch_2/zext.ll
+-rw-r--r--   0        0        0     8604 2023-06-20 19:48:04.047690 pytket_qirpass-0.5.0/test/test_qirpass.py
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 pytket_qirpass-0.5.0/PKG-INFO
```

### Comparing `pytket-qirpass-0.4.0/LICENSE` & `pytket_qirpass-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/README.md` & `pytket_qirpass-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/pyproject.toml` & `pytket_qirpass-0.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
-requires = ["flit_core >=3.8,<4"]
+requires = ["flit_core >=3.9.0,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "pytket-qirpass"
 authors = [{name = "Alec Edgington", email = "alec.edgington@quantinuum.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 dynamic = ["version", "description"]
-dependencies = ["llvmlite >= 0.39.1,<0.40", "pytket >= 1.11.1,<2"]
+dependencies = ["llvmlite >= 0.40.0,<0.41", "pytket >= 1.16.0,<2"]
 
 [project.urls]
 Home = "https://github.com/CQCL/pytket-qirpass"
 
 [project.optional-dependencies]
 tests = ["pyqir >=0.8.0,<0.9"]
```

### Comparing `pytket-qirpass-0.4.0/src/pytket_qirpass/apply_qirpass.py` & `pytket_qirpass-0.5.0/src/pytket_qirpass/apply_qirpass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from math import pi
 import struct
-from typing import List, Set, Tuple
+from typing import List, Optional, Set, Tuple
 
 from llvmlite.binding import (
     create_context,
     parse_assembly,
     parse_bitcode,
     ModuleRef,
     ValueRef,
@@ -36,14 +36,18 @@
     "__quantum__qis__t__adj": (OpType.Tdg, "%Qubit*"),
     "__quantum__qis__x__body": (OpType.X, "%Qubit*"),
     "__quantum__qis__y__body": (OpType.Y, "%Qubit*"),
     "__quantum__qis__z__body": (OpType.Z, "%Qubit*"),
     # Additional gates:
     "__quantum__qis__phasedx__body": (OpType.PhasedX, "double, double, %Qubit*"),
     "__quantum__qis__zzmax__body": (OpType.ZZMax, "%Qubit*, %Qubit*"),
+    "__quantum__qis__rxxyyzz__body": (
+        OpType.TK2,
+        "double, double, double, %Qubit*, %Qubit*",
+    ),
 }
 
 tk_to_qir = {optype: (name, sig) for name, (optype, sig) in opdata.items()}
 
 
 def encode_double(a: float) -> str:
     assert isinstance(a, float)
@@ -213,15 +217,15 @@
 def is_entry_point(function: ValueRef) -> bool:
     assert function.is_function
     return any(b'"EntryPoint"' in attrs for attrs in function.attributes)
 
 
 def apply_qirpass(
     qir_bitcode: bytes,
-    comp_pass: BasePass,
+    comp_pass: Optional[BasePass],
     target_1q_gates: Set[OpType],
     target_2q_gates: Set[OpType],
 ) -> bytes:
     """Apply the given pass to basic blocls of the QIR.
 
     Only QIR conforming to the Quantinuum profile is accepted as input.
 
@@ -258,23 +262,24 @@
     f0 = entries[0]
     f0_attrs = list(f0.attributes)
     assert len(f0_attrs) == 1
     f0_attr = f0_attrs[0].decode("utf-8")
 
     target_gates = target_1q_gates | target_2q_gates
 
-    comp_pass = SequencePass(
+    pass_list = [] if comp_pass is None else [comp_pass]
+    pass_list.extend(
         [
-            comp_pass,
             RemoveImplicitQubitPermutation(),
             auto_rebase_pass(target_gates),
             auto_squash_pass(target_1q_gates),
             RemoveRedundancies(),
         ]
     )
+    comp_pass = SequencePass(pass_list)
 
     for function in functions:
         new_ll += "\n"
         basic_blocks = list(function.blocks)
         if len(basic_blocks) == 0:
             # This is an external declaration
             decl = str(function)
```

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/ClassicalCircuit.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/ClassicalCircuit.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/ClassicalReg2ConstCircuit.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/ClassicalReg2ConstCircuit.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/NestedConditionalsCircuit.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/NestedConditionalsCircuit.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/RUSLoopXX-1.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/RUSLoopXX-1.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/RebasedCircuit.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/RebasedCircuit.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/RoundTripDiamondConditional.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/RoundTripDiamondConditional.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/RoundTripSimpleChain.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/RoundTripSimpleChain.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/SimpleConditionalCircuit.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/SimpleConditionalCircuit.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/SimpleGroverBaseProfile.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/SimpleGroverBaseProfile.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/SimpleGroverSample.BaseProfile.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/SimpleGroverSample.BaseProfile.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/SimpleGroverSampleOptimised.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/SimpleGroverSampleOptimised.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/TestBellCircuit.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/TestBellCircuit.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/WASM.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/WASM.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/classical_and_controlflow.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/classical_and_controlflow.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/collapse_jump_instr.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/collapse_jump_instr.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/collapse_jump_left.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/collapse_jump_left.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/collapse_jump_right.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/collapse_jump_right.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/collapse_nested_jump_instr.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/collapse_nested_jump_instr.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/collapse_simple_instr_chain.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/collapse_simple_instr_chain.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/nested_conditionals-new.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/nested_conditionals-new.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/nested_conditionals.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/nested_conditionals.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/nested_conditionals_crossed.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/nested_conditionals_crossed.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/nested_conditionals_else.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/nested_conditionals_else.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/nested_conditionals_then.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/nested_conditionals_then.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/one_conditional.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/one_conditional.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/one_conditional_diamond.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/one_conditional_diamond.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/one_conditional_diamond_opposite.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/one_conditional_diamond_opposite.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/one_conditional_else.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/one_conditional_else.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/one_conditional_if.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/one_conditional_if.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/one_conditional_then.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/one_conditional_then.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/select_and_controlflow.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/select_and_controlflow.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/tagged_rt_functions.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/tagged_rt_functions.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/teleportchain_baseprofile.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/teleportchain_baseprofile.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/untagged_rt_functions.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/untagged_rt_functions.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_1/wasm_and_controlflow.ll` & `pytket_qirpass-0.5.0/test/qir/batch_1/wasm_and_controlflow.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/1_PauliX_PauliX_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/1_PauliX_PauliX_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/2_PauliX_PauliX_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/2_PauliX_PauliX_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/3_PauliX_PauliX_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/3_PauliX_PauliX_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/4_PauliX_PauliX_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/4_PauliX_PauliX_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/ArithmeticOps.TargetedAlt_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/ArithmeticOps.TargetedAlt_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/Distillation.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/Distillation.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/Distillation_other.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/Distillation_other.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/Distillation_small.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/Distillation_small.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/IntegerComparison.TargetedAlt_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/IntegerComparison.TargetedAlt_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/IntegerComparison.Targeted_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/IntegerComparison.Targeted_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/LogicalRb-BaseProfile.opt.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/LogicalRb-BaseProfile.opt.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-3X.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-3X.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-5X.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-5X.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-6X.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-6X.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-7X.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-7X.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-NoInline.10X.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile-NoInline.10X.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.10X.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.10X.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.3.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.3.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.3X.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.3X.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.6X.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.6X.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.8Y.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.8Y.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.9X.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.9X.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.opt.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-BaseProfile.opt.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-Grouping.10X.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-Grouping.10X.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation-Grouping.3Y.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation-Grouping.3Y.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/MagicStateDistillation.BaseProfile-4X.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/MagicStateDistillation.BaseProfile-4X.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop1.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop1.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop10.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop10.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop10_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop10_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop1_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop1_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop2.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop2.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop2_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop2_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop3_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop3_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop4_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop4_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop5_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop5_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop6_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop6_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop7_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop7_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop8_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop8_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoop9_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoop9_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-10_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-10_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-1_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-1_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-2_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-2_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-3_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-3_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-4_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-4_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-5_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-5_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-6_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-6_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-7_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-7_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-8_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-8_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopYY-9_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopYY-9_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-10_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-10_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-1_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-1_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-2_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-2_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-3_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-3_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-4_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-4_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-5_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-5_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-6_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-6_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-7_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-7_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-8_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-8_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RUSLoopZZ-9_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RUSLoopZZ-9_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/RandomWalkPE1.baseProfile.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/RandomWalkPE1.baseProfile.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/SimpleGroverBaseProfile.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/SimpleGroverBaseProfile.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/SimpleGroverGrouped.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/SimpleGroverGrouped.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/SimpleGroverSample.BaseProfile.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/SimpleGroverSample.BaseProfile.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/SimpleGroverSample.O1.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/SimpleGroverSample.O1.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/SimpleGroverSample.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/SimpleGroverSample.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/XX_recursion_limit8.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/XX_recursion_limit8.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/bool_tag.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/bool_tag.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/classical_flow.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/classical_flow.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/classical_flow2.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/classical_flow2.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/classical_flow3.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/classical_flow3.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/classical_flow4.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/classical_flow4.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/classical_flow5.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/classical_flow5.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/classical_flow6.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/classical_flow6.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/cond_ops.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/cond_ops.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/conditional-test-3.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/conditional-test-3.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/conditional_test.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/conditional_test.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/conditional_test_2.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/conditional_test_2.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/conditional_test_3.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/conditional_test_3.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/conditional_test_4.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/conditional_test_4.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/control_flow_complex.baseProfile.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/control_flow_complex.baseProfile.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/control_flow_long.baseProfile.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/control_flow_long.baseProfile.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/control_flow_nested.baseProfile.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/control_flow_nested.baseProfile.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/control_flow_short.baseProfile.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/control_flow_short.baseProfile.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/fallthrough_simple.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/fallthrough_simple.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_5qb.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_5qb.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_5qb_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_5qb_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_10k.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_10k.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_10k_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_10k_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_10qb.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_10qb.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_10qb_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_10qb_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_10qb_10k.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_10qb_10k.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_10qb_10k_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_10qb_10k_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_15k.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_15k.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_15k_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_15k_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_20k.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_20k.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_20k_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_20k_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_25k.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_25k.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_25k_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_25k_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/gate_stress_test_50k.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/gate_stress_test_50k.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/ghz_fail_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/ghz_fail_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/int_result_with_tag.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/int_result_with_tag.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/int_tag_alt_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/int_tag_alt_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/iqpe.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/iqpe.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/iqpe_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/iqpe_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/loopRecursion.baseProfile.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/loopRecursion.baseProfile.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/many_gates.baseProfile.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/many_gates.baseProfile.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/many_ops.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/many_ops.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/measure_result.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/measure_result.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/most_features.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/most_features.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/most_features_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/most_features_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/multi_arith.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/multi_arith.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/mutables_ops_branches.baseProfile.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/mutables_ops_branches.baseProfile.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/native_gates.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/native_gates.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/negative_arith.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/negative_arith.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/nested_conditions.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/nested_conditions.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/no-ops.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/no-ops.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/one_conditional.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/one_conditional.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_1.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_1.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_2.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_2.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_3.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_3.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_4.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_4.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_5.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_5.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_6.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_6.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_7.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_7.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/phi_test_8.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/phi_test_8.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/qir_hybrid.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/qir_hybrid.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/result_tag.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/result_tag.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/result_tag_alt.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/result_tag_alt.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/result_tag_alt_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/result_tag_alt_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/result_with_constant_args.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/result_with_constant_args.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/select-nested-const-cond.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/select-nested-const-cond.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/select-nested.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/select-nested.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/sequential_flow_1.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/sequential_flow_1.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/sequential_flow_2.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/sequential_flow_2.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/tagged_duplicates.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/tagged_duplicates.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/tagged_result_control_flow.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/tagged_result_control_flow.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/tagged_result_control_flow_.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/tagged_result_control_flow_.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/teleport-chain-grouping.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/teleport-chain-grouping.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/qir/batch_2/teleportchain.BaseProfile.ll` & `pytket_qirpass-0.5.0/test/qir/batch_2/teleportchain.BaseProfile.ll`

 * *Files identical despite different names*

### Comparing `pytket-qirpass-0.4.0/test/test_qirpass.py` & `pytket_qirpass-0.5.0/test/test_qirpass.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import unittest
 
 from pytket_qirpass import apply_qirpass
 
 from llvmlite.binding import create_context, parse_assembly, parse_bitcode, ModuleRef
 from pyqir import Context, Module
 from pytket.circuit import OpType
-from pytket.passes import FullPeepholeOptimise
+from pytket.passes import FullPeepholeOptimise, SynthesiseTK
 
 QIR_DIR = Path(__file__).parent.resolve() / "qir"
 
 
 def ll_to_module(ll: str) -> ModuleRef:
     ctx = create_context()
     module = parse_assembly(ll, context=ctx)
@@ -297,23 +297,31 @@
 def verify_with_pyqir(qir_bitcode: bytes) -> None:
     ctx = Context()
     module = Module.from_bitcode(ctx, qir_bitcode)
     module.verify()
 
 
 def check_compilation(qir_ll_in: str) -> None:
-    qir_in = ll_to_bc(qir_ll_in)
-    qir_out = apply_qirpass(
-        qir_in,
+    passes = [
+        None,
+        SynthesiseTK(),
         FullPeepholeOptimise(target_2qb_gate=OpType.TK2, allow_swaps=False),
-        {OpType.PhasedX, OpType.Rz},
+    ]
+    gatesets2q = [
         {OpType.ZZMax, OpType.ZZPhase},
-    )
-    verify_with_llvmlite(qir_out)
-    verify_with_pyqir(qir_out)
+        {OpType.ZZMax, OpType.ZZPhase, OpType.TK2},
+    ]
+    qir_in = ll_to_bc(qir_ll_in)
+    for comp_pass in passes:
+        for gateset2q in gatesets2q:
+            qir_out = apply_qirpass(
+                qir_in, comp_pass, {OpType.PhasedX, OpType.Rz}, gateset2q
+            )
+            verify_with_llvmlite(qir_out)
+            verify_with_pyqir(qir_out)
 
 
 class TestQirPass(unittest.TestCase):
     def test_qirpass(self):
         for progname in prognames_1:
             with self.subTest(msg=f"Compiling {progname}"):
                 with open(
```

### Comparing `pytket-qirpass-0.4.0/PKG-INFO` & `pytket_qirpass-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytket-qirpass
-Version: 0.4.0
+Version: 0.5.0
 Summary: Module for optimizing QIR using pytket.
 Author-email: Alec Edgington <alec.edgington@quantinuum.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: llvmlite >= 0.39.1,<0.40
-Requires-Dist: pytket >= 1.11.1,<2
+Requires-Dist: llvmlite >= 0.40.0,<0.41
+Requires-Dist: pytket >= 1.16.0,<2
 Requires-Dist: pyqir >=0.8.0,<0.9 ; extra == "tests"
 Project-URL: Home, https://github.com/CQCL/pytket-qirpass
 Provides-Extra: tests
 
 # pytket-qirpass
 
 This module provides a method to optimize QIR using pytket.
```

