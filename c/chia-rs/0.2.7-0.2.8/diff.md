# Comparing `tmp/chia_rs-0.2.7.tar.gz` & `tmp/chia_rs-0.2.8.tar.gz`

## Comparing `chia_rs-0.2.7.tar` & `chia_rs-0.2.8.tar`

### file list

```diff
@@ -1,137 +1,138 @@
--rw-r--r--   0        0        0      458 1970-01-01 00:00:00.000000 chia_rs-0.2.7/local_dependencies/chia_py_streamable_macro/Cargo.toml
--rw-r--r--   0     1001      123     9330 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia_py_streamable_macro/src/lib.rs
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 chia_rs-0.2.7/local_dependencies/clvm-utils/Cargo.toml
--rw-r--r--   0     1001      123      155 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/clvm-utils/README.md
--rw-r--r--   0     1001      123       36 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/clvm-utils/src/lib.rs
--rw-r--r--   0     1001      123     2918 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/clvm-utils/src/tree_hash.rs
--rw-r--r--   0     1001      123     6300 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/clvm-utils/src/uncurry.rs
--rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 chia_rs-0.2.7/local_dependencies/chia_streamable_macro/Cargo.toml
--rw-r--r--   0     1001      123     4715 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia_streamable_macro/src/lib.rs
--rw-r--r--   0        0        0      781 1970-01-01 00:00:00.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/Cargo.toml
--rw-r--r--   0     1001      123      722 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/bls.rs
--rw-r--r--   0     1001      123     5474 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/bytes.rs
--rw-r--r--   0     1001      123     1386 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/chia_error.rs
--rw-r--r--   0     1001      123     4701 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/chia_protocol.rs
--rw-r--r--   0     1001      123      862 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/classgroup.rs
--rw-r--r--   0     1001      123     1809 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/coin.rs
--rw-r--r--   0     1001      123      556 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/coin_spend.rs
--rw-r--r--   0     1001      123      540 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/coin_state.rs
--rw-r--r--   0     1001      123      743 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/end_of_sub_slot_bundle.rs
--rw-r--r--   0     1001      123      871 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/fee_estimate.rs
--rw-r--r--   0     1001      123     2316 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/foliage.rs
--rw-r--r--   0     1001      123     3679 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/from_json_dict.rs
--rw-r--r--   0     1001      123     1497 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/fullblock.rs
--rw-r--r--   0     1001      123     1388 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/header_block.rs
--rw-r--r--   0     1001      123     1288 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/lib.rs
--rw-r--r--   0     1001      123      810 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/message_struct.rs
--rw-r--r--   0     1001      123      540 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/pool_target.rs
--rw-r--r--   0     1001      123     1624 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/program.rs
--rw-r--r--   0     1001      123      679 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/proof_of_space.rs
--rw-r--r--   0     1001      123     1527 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/reward_chain_block.rs
--rw-r--r--   0     1001      123     1788 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/slots.rs
--rw-r--r--   0     1001      123      569 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/spend_bundle.rs
--rw-r--r--   0     1001      123    20212 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/streamable.rs
--rw-r--r--   0     1001      123     2217 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/to_json_dict.rs
--rw-r--r--   0     1001      123      679 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/vdf.rs
--rw-r--r--   0     1001      123     4016 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/wallet_protocol.rs
--rw-r--r--   0     1001      123     1225 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia-protocol/src/weight_proof.rs
--rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 chia_rs-0.2.7/local_dependencies/chia/Cargo.toml
--rw-r--r--   0     1001      123      224 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/.cargo/config
--rw-r--r--   0     1001      123      290 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/.github/workflows/audit-check.yml
--rw-r--r--   0     1001      123     3050 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/.github/workflows/benchmark.yml
--rw-r--r--   0     1001      123     2843 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/.github/workflows/build-crate-and-npm.yml
--rw-r--r--   0     1001      123    13503 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/.github/workflows/build-test.yml
--rw-r--r--   0     1001      123       19 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/.gitignore
--rw-r--r--   0     1001      123    11357 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/LICENSE
--rw-r--r--   0     1001      123      192 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/README.md
--rw-r--r--   0     1001      123      142 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/cl/README.md
--rw-r--r--   0     1001      123     4603 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/cl/deserialize_w_backrefs.cl
--rw-r--r--   0     1001      123     4474 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/docs/implementation-notes.md
--rw-r--r--   0     1001      123      882 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/examples/README.md
--rw-r--r--   0     1001      123    48843 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/examples/block-1519806.bin
--rw-r--r--   0     1001      123      299 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/examples/dump.py
--rw-r--r--   0     1001      123     1592 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/examples/streaming-patch.diff
--rw-r--r--   0     1001      123       93 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/mypy.ini
--rw-r--r--   0     1001      123      261 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/allocator.rs
--rw-r--r--   0     1001      123     1817 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/compression/compressor.rs
--rw-r--r--   0     1001      123      858 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/compression/deserialize_w_backrefs.bin
--rw-r--r--   0     1001      123       20 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/compression/mod.rs
--rw-r--r--   0     1001      123     3120 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/fuzzing_utils.rs
--rw-r--r--   0     1001      123     3042 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/gen/coin_id.rs
--rw-r--r--   0     1001      123     4493 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/gen/condition_sanitizers.rs
--rw-r--r--   0     1001      123   129755 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/gen/conditions.rs
--rw-r--r--   0     1001      123      972 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/gen/flags.rs
--rw-r--r--   0     1001      123     6447 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/gen/get_puzzle_and_solution.rs
--rw-r--r--   0     1001      123      221 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/gen/mod.rs
--rw-r--r--   0     1001      123     7075 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/gen/opcodes.rs
--rw-r--r--   0     1001      123     2475 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/gen/run_block_generator.rs
--rw-r--r--   0     1001      123     2159 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/gen/run_puzzle.rs
--rw-r--r--   0     1001      123     2916 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/gen/sanitize_int.rs
--rw-r--r--   0     1001      123     5743 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/gen/validation_error.rs
--rw-r--r--   0     1001      123     4972 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/generator_rom.rs
--rw-r--r--   0     1001      123      136 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/lib.rs
--rw-r--r--   0     1001      123    22862 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/src/merkle_set.rs
--rwxr-xr-x   0     1001      123     8264 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generate-programs.py
--rw-r--r--   0     1001      123     1143 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/assert-puzzle-announce-fail.clvm
--rw-r--r--   0     1001      123    21116 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/block-834752.clvm
--rw-r--r--   0     1001      123    25761 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/block-834752.hex
--rw-r--r--   0     1001      123    99972 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/block-834760.clvm
--rw-r--r--   0     1001      123    22001 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/block-834761.clvm
--rw-r--r--   0     1001      123    59172 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/block-834765.clvm
--rw-r--r--   0     1001      123   105717 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/block-834766.clvm
--rw-r--r--   0     1001      123    83316 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/block-834768.clvm
--rw-r--r--   0     1001      123      577 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/create-coin-different-amounts.clvm
--rw-r--r--   0     1001      123      267 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/create-coin-hint-duplicate-outputs.clvm
--rw-r--r--   0     1001      123      685 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/create-coin-hint.clvm
--rw-r--r--   0     1001      123      699 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/create-coin-hint2.clvm
--rw-r--r--   0     1001      123      456 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/deep-recursion-plus.clvm
--rw-r--r--   0     1001      123      382 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/double-spend.clvm
--rw-r--r--   0     1001      123      501 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/duplicate-coin-announce.clvm
--rw-r--r--   0     1001      123      263 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/duplicate-create-coin.clvm
--rw-r--r--   0     1001      123      448 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/duplicate-height-absolute-div.clvm
--rw-r--r--   0     1001      123      429 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/duplicate-height-absolute-substr-tail.clvm
--rw-r--r--   0     1001      123      422 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/duplicate-height-absolute-substr.clvm
--rw-r--r--   0     1001      123      391 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/duplicate-height-absolute.clvm
--rw-r--r--   0     1001      123      391 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/duplicate-height-relative.clvm
--rw-r--r--   0     1001      123      196 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/duplicate-outputs.clvm
--rw-r--r--   0     1001      123      391 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/duplicate-reserve-fee.clvm
--rw-r--r--   0     1001      123      391 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/duplicate-seconds-absolute.clvm
--rw-r--r--   0     1001      123      392 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/duplicate-seconds-relative.clvm
--rw-r--r--   0     1001      123      380 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/height-absolute-ladder.clvm
--rw-r--r--   0     1001      123      104 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/infinite-recursion1.clvm
--rw-r--r--   0     1001      123       92 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/infinite-recursion2.clvm
--rw-r--r--   0     1001      123     1458 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/infinite-recursion3.clvm
--rw-r--r--   0     1001      123      160 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/infinite-recursion4.clvm
--rw-r--r--   0     1001      123      100 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/invalid-conditions.clvm
--rw-r--r--   0     1001      123     1339 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/just-puzzle-announce.clvm
--rw-r--r--   0     1001      123   590571 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/many-create-coin.clvm
--rw-r--r--   0     1001      123      597 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/many-large-ints-negative.clvm
--rw-r--r--   0     1001      123      416 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/many-large-ints.clvm
--rw-r--r--   0     1001      123      500 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/max-height.clvm
--rw-r--r--   0     1001      123      349 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/multiple-reserve-fee.clvm
--rw-r--r--   0     1001      123      400 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/negative-reserve-fee.clvm
--rw-r--r--   0     1001      123      160 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/recursion-pairs.clvm
--rw-r--r--   0     1001      123      343 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/generators/unknown-condition.clvm
--rwxr-xr-x   0     1001      123     3042 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/run-programs.py
--rwxr-xr-x   0     1001      123     1569 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/run.py
--rwxr-xr-x   0     1001      123     3789 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/run_gen.py
--rwxr-xr-x   0     1001      123     3497 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/test-generators.py
--rw-r--r--   0     1001      123    11060 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/test_coin.py
--rw-r--r--   0     1001      123      878 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/test_run_block_generator.py
--rw-r--r--   0     1001      123     5068 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/test_run_puzzle.py
--rw-r--r--   0     1001      123    10725 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/test_streamable.py
--rw-r--r--   0     1001      123     1050 2023-04-24 16:19:39.000000 chia_rs-0.2.7/local_dependencies/chia/tests/test_tree_hash.py
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 chia_rs-0.2.7/Cargo.toml
--rw-r--r--   0     1001      123       77 2023-04-24 16:19:39.000000 chia_rs-0.2.7/README.md
--rw-r--r--   0     1001      123    68299 2023-04-24 16:19:39.000000 chia_rs-0.2.7/chia_rs.pyi
--rw-r--r--   0     1001      123     7396 2023-04-24 16:19:39.000000 chia_rs-0.2.7/generate_type_stubs.py
--rw-r--r--   0     1001      123        0 2023-04-24 16:19:39.000000 chia_rs-0.2.7/py.typed
--rw-r--r--   0     1001      123      112 2023-04-24 16:19:39.000000 chia_rs-0.2.7/pyproject.toml
--rw-r--r--   0     1001      123      615 2023-04-24 16:19:39.000000 chia_rs-0.2.7/src/adapt_response.rs
--rw-r--r--   0     1001      123     8865 2023-04-24 16:19:39.000000 chia_rs-0.2.7/src/api.rs
--rw-r--r--   0     1001      123      641 2023-04-24 16:19:39.000000 chia_rs-0.2.7/src/compression.rs
--rw-r--r--   0     1001      123      175 2023-04-24 16:19:39.000000 chia_rs-0.2.7/src/lib.rs
--rw-r--r--   0     1001      123     6946 2023-04-24 16:19:39.000000 chia_rs-0.2.7/src/run_generator.rs
--rw-r--r--   0     1001      123     2644 2023-04-24 16:19:39.000000 chia_rs-0.2.7/src/run_program.rs
--rw-r--r--   0     1001      123    14442 2023-04-24 16:20:42.000000 chia_rs-0.2.7/Cargo.lock
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 chia_rs-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 chia_rs-0.2.8/local_dependencies/clvm-utils/Cargo.toml
+-rw-r--r--   0     1001      123      155 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/clvm-utils/README.md
+-rw-r--r--   0     1001      123       36 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/clvm-utils/src/lib.rs
+-rw-r--r--   0     1001      123     2914 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/clvm-utils/src/tree_hash.rs
+-rw-r--r--   0     1001      123     6491 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/clvm-utils/src/uncurry.rs
+-rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 chia_rs-0.2.8/local_dependencies/chia/Cargo.toml
+-rw-r--r--   0     1001      123      224 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/.cargo/config
+-rw-r--r--   0     1001      123      290 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/.github/workflows/audit-check.yml
+-rw-r--r--   0     1001      123     3050 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/.github/workflows/benchmark.yml
+-rw-r--r--   0     1001      123     2843 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/.github/workflows/build-crate-and-npm.yml
+-rw-r--r--   0     1001      123    15546 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/.github/workflows/build-test.yml
+-rw-r--r--   0     1001      123       19 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/.gitignore
+-rw-r--r--   0     1001      123    11357 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/LICENSE
+-rw-r--r--   0     1001      123      192 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/README.md
+-rw-r--r--   0     1001      123      142 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/cl/README.md
+-rw-r--r--   0     1001      123     4603 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/cl/deserialize_w_backrefs.cl
+-rw-r--r--   0     1001      123     4474 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/docs/implementation-notes.md
+-rw-r--r--   0     1001      123      882 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/examples/README.md
+-rw-r--r--   0     1001      123    48843 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/examples/block-1519806.bin
+-rw-r--r--   0     1001      123      299 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/examples/dump.py
+-rw-r--r--   0     1001      123     1592 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/examples/streaming-patch.diff
+-rw-r--r--   0     1001      123     2184 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/assert-puzzle-announce-fail.txt
+-rw-r--r--   0     1001      123    12107 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834752-compressed.txt
+-rw-r--r--   0     1001      123    28444 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834752.txt
+-rw-r--r--   0     1001      123   132615 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834760.txt
+-rw-r--r--   0     1001      123    26930 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834761.txt
+-rw-r--r--   0     1001      123    74748 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834765.txt
+-rw-r--r--   0     1001      123   124696 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834766.txt
+-rw-r--r--   0     1001      123   104382 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834768.txt
+-rw-r--r--   0     1001      123      665 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/create-coin-different-amounts.txt
+-rw-r--r--   0     1001      123      425 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/create-coin-hint-duplicate-outputs.txt
+-rw-r--r--   0     1001      123      808 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/create-coin-hint.txt
+-rw-r--r--   0     1001      123      832 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/create-coin-hint2.txt
+-rw-r--r--   0     1001      123      554 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/deep-recursion-plus.txt
+-rw-r--r--   0     1001      123      413 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/double-spend.txt
+-rw-r--r--   0     1001      123      631 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-coin-announce.txt
+-rw-r--r--   0     1001      123      405 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-create-coin.txt
+-rw-r--r--   0     1001      123      556 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-height-absolute-div.txt
+-rw-r--r--   0     1001      123      601 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-height-absolute-substr-tail.txt
+-rw-r--r--   0     1001      123      589 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-height-absolute-substr.txt
+-rw-r--r--   0     1001      123      556 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-height-absolute.txt
+-rw-r--r--   0     1001      123      556 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-height-relative.txt
+-rw-r--r--   0     1001      123      281 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-outputs.txt
+-rw-r--r--   0     1001      123      556 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-reserve-fee.txt
+-rw-r--r--   0     1001      123      556 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-seconds-absolute.txt
+-rw-r--r--   0     1001      123      557 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/duplicate-seconds-relative.txt
+-rw-r--r--   0     1001      123      546 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/height-absolute-ladder.txt
+-rw-r--r--   0     1001      123      171 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/infinite-recursion1.txt
+-rw-r--r--   0     1001      123      155 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/infinite-recursion2.txt
+-rw-r--r--   0     1001      123     1431 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/infinite-recursion3.txt
+-rw-r--r--   0     1001      123      219 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/infinite-recursion4.txt
+-rw-r--r--   0     1001      123      110 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/invalid-conditions.txt
+-rw-r--r--   0     1001      123     2380 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/just-puzzle-announce.txt
+-rw-r--r--   0     1001      123   590784 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/many-create-coin.txt
+-rw-r--r--   0     1001      123      796 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/many-large-ints-negative.txt
+-rw-r--r--   0     1001      123      612 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/many-large-ints.txt
+-rw-r--r--   0     1001      123      559 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/max-height.txt
+-rw-r--r--   0     1001      123      373 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/multiple-reserve-fee.txt
+-rw-r--r--   0     1001      123      598 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/negative-reserve-fee.txt
+-rw-r--r--   0     1001      123      273 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/recursion-pairs.txt
+-rw-r--r--   0     1001      123      367 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/generator-tests/unknown-condition.txt
+-rw-r--r--   0     1001      123       93 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/mypy.ini
+-rw-r--r--   0     1001      123      412 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/allocator.rs
+-rw-r--r--   0     1001      123     1713 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/compression/compressor.rs
+-rw-r--r--   0     1001      123      858 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/compression/deserialize_w_backrefs.bin
+-rw-r--r--   0     1001      123       20 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/compression/mod.rs
+-rw-r--r--   0     1001      123     3120 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/fuzzing_utils.rs
+-rw-r--r--   0     1001      123     3042 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/coin_id.rs
+-rw-r--r--   0     1001      123     4493 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/condition_sanitizers.rs
+-rw-r--r--   0     1001      123   140900 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/conditions.rs
+-rw-r--r--   0     1001      123     2233 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/flags.rs
+-rw-r--r--   0     1001      123     6447 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/get_puzzle_and_solution.rs
+-rw-r--r--   0     1001      123      256 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/mod.rs
+-rw-r--r--   0     1001      123    10135 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/opcodes.rs
+-rw-r--r--   0     1001      123     2650 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/run_block_generator.rs
+-rw-r--r--   0     1001      123     2352 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/run_puzzle.rs
+-rw-r--r--   0     1001      123     2916 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/sanitize_int.rs
+-rw-r--r--   0     1001      123     7440 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/test_generators.rs
+-rw-r--r--   0     1001      123     5987 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/gen/validation_error.rs
+-rw-r--r--   0     1001      123     1990 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/generator_rom.rs
+-rw-r--r--   0     1001      123      136 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/lib.rs
+-rw-r--r--   0     1001      123    22862 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/src/merkle_set.rs
+-rwxr-xr-x   0     1001      123     8264 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/generate-programs.py
+-rwxr-xr-x   0     1001      123     3042 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/run-programs.py
+-rwxr-xr-x   0     1001      123     1569 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/run.py
+-rwxr-xr-x   0     1001      123     3563 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/run_gen.py
+-rwxr-xr-x   0     1001      123     3014 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/test-generators.py
+-rw-r--r--   0     1001      123    11060 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/test_coin.py
+-rw-r--r--   0     1001      123      803 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/test_run_block_generator.py
+-rw-r--r--   0     1001      123     5587 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/test_run_puzzle.py
+-rw-r--r--   0     1001      123    10725 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/test_streamable.py
+-rw-r--r--   0     1001      123     1050 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia/tests/test_tree_hash.py
+-rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/Cargo.toml
+-rw-r--r--   0     1001      123      722 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/bls.rs
+-rw-r--r--   0     1001      123     5474 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/bytes.rs
+-rw-r--r--   0     1001      123     1386 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/chia_error.rs
+-rw-r--r--   0     1001      123     4701 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/chia_protocol.rs
+-rw-r--r--   0     1001      123      862 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/classgroup.rs
+-rw-r--r--   0     1001      123     1809 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/coin.rs
+-rw-r--r--   0     1001      123      556 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/coin_spend.rs
+-rw-r--r--   0     1001      123      540 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/coin_state.rs
+-rw-r--r--   0     1001      123      743 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/end_of_sub_slot_bundle.rs
+-rw-r--r--   0     1001      123      871 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/fee_estimate.rs
+-rw-r--r--   0     1001      123     2316 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/foliage.rs
+-rw-r--r--   0     1001      123     3679 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/from_json_dict.rs
+-rw-r--r--   0     1001      123     1497 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/fullblock.rs
+-rw-r--r--   0     1001      123     1388 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/header_block.rs
+-rw-r--r--   0     1001      123     1288 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/lib.rs
+-rw-r--r--   0     1001      123      810 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/message_struct.rs
+-rw-r--r--   0     1001      123      540 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/pool_target.rs
+-rw-r--r--   0     1001      123     1624 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/program.rs
+-rw-r--r--   0     1001      123      679 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/proof_of_space.rs
+-rw-r--r--   0     1001      123     1527 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/reward_chain_block.rs
+-rw-r--r--   0     1001      123     1788 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/slots.rs
+-rw-r--r--   0     1001      123      569 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/spend_bundle.rs
+-rw-r--r--   0     1001      123    20212 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/streamable.rs
+-rw-r--r--   0     1001      123     2217 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/to_json_dict.rs
+-rw-r--r--   0     1001      123      679 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/vdf.rs
+-rw-r--r--   0     1001      123     4016 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/wallet_protocol.rs
+-rw-r--r--   0     1001      123     1225 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia-protocol/src/weight_proof.rs
+-rw-r--r--   0        0        0      458 1970-01-01 00:00:00.000000 chia_rs-0.2.8/local_dependencies/chia_py_streamable_macro/Cargo.toml
+-rw-r--r--   0     1001      123     9330 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia_py_streamable_macro/src/lib.rs
+-rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 chia_rs-0.2.8/local_dependencies/chia_streamable_macro/Cargo.toml
+-rw-r--r--   0     1001      123     4715 2023-06-21 16:36:00.000000 chia_rs-0.2.8/local_dependencies/chia_streamable_macro/src/lib.rs
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 chia_rs-0.2.8/Cargo.toml
+-rw-r--r--   0     1001      123       77 2023-06-21 16:36:00.000000 chia_rs-0.2.8/README.md
+-rw-r--r--   0     1001      123    68548 2023-06-21 16:36:00.000000 chia_rs-0.2.8/chia_rs.pyi
+-rw-r--r--   0     1001      123     7645 2023-06-21 16:36:00.000000 chia_rs-0.2.8/generate_type_stubs.py
+-rw-r--r--   0     1001      123        0 2023-06-21 16:36:00.000000 chia_rs-0.2.8/py.typed
+-rw-r--r--   0     1001      123      112 2023-06-21 16:36:00.000000 chia_rs-0.2.8/pyproject.toml
+-rw-r--r--   0     1001      123      559 2023-06-21 16:36:00.000000 chia_rs-0.2.8/src/adapt_response.rs
+-rw-r--r--   0     1001      123     9671 2023-06-21 16:36:00.000000 chia_rs-0.2.8/src/api.rs
+-rw-r--r--   0     1001      123      641 2023-06-21 16:36:00.000000 chia_rs-0.2.8/src/compression.rs
+-rw-r--r--   0     1001      123      175 2023-06-21 16:36:00.000000 chia_rs-0.2.8/src/lib.rs
+-rw-r--r--   0     1001      123     6961 2023-06-21 16:36:00.000000 chia_rs-0.2.8/src/run_generator.rs
+-rw-r--r--   0     1001      123     2843 2023-06-21 16:36:00.000000 chia_rs-0.2.8/src/run_program.rs
+-rw-r--r--   0     1001      123    22607 2023-06-21 16:36:09.000000 chia_rs-0.2.8/Cargo.lock
+-rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 chia_rs-0.2.8/PKG-INFO
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia_py_streamable_macro/src/lib.rs` & `chia_rs-0.2.8/local_dependencies/chia_py_streamable_macro/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/clvm-utils/src/tree_hash.rs` & `chia_rs-0.2.8/local_dependencies/clvm-utils/src/tree_hash.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 pub fn tree_hash(a: &Allocator, node: NodePtr) -> [u8; 32] {
     let mut hashes: Vec<[u8; 32]> = vec![];
     let mut ops = vec![TreeOp::SExp(node)];
 
     while !ops.is_empty() {
         match ops.pop().unwrap() {
             TreeOp::SExp(node) => match a.sexp(node) {
-                SExp::Atom(atom) => {
+                SExp::Atom() => {
                     let mut sha256 = Sha256::new();
                     sha256.update([1_u8]);
-                    sha256.update(a.buf(&atom));
+                    sha256.update(a.atom(node));
                     hashes.push(sha256.finalize().into())
                 }
                 SExp::Pair(left, right) => {
                     ops.push(TreeOp::Cons);
                     ops.push(TreeOp::SExp(left));
                     ops.push(TreeOp::SExp(right));
                 }
```

### Comparing `chia_rs-0.2.7/local_dependencies/clvm-utils/src/uncurry.rs` & `chia_rs-0.2.8/local_dependencies/clvm-utils/src/uncurry.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,78 @@
-use clvmr::allocator::{Allocator, NodePtr};
-use clvmr::node::Node;
+use clvmr::allocator::{Allocator, NodePtr, SExp};
+use clvmr::op_utils::nullp;
 
-fn unwrap3(node: Node) -> Option<(Node, Node, Node)> {
-    let mut i = node;
-    let n1 = i.next()?;
-    let n2 = i.next()?;
-    let n3 = i.next()?;
-    if i.next().is_some() {
-        return None;
+fn destructure<const N: usize>(a: &Allocator, mut node: NodePtr) -> Option<[NodePtr; N]> {
+    let mut counter = 0;
+    let mut ret: [NodePtr; N] = [0; N];
+    while let Some((first, rest)) = a.next(node) {
+        node = rest;
+        if counter == N {
+            return None;
+        }
+        ret[counter] = first;
+        counter += 1;
+    }
+    if counter != N {
+        None
+    } else {
+        Some(ret)
     }
-    Some((n1, n2, n3))
 }
 
-fn check(n: &Node, atom: &[u8]) -> Option<()> {
-    if n.atom()? == atom {
-        Some(())
-    } else {
-        None
+fn check(a: &Allocator, n: NodePtr, atom: &[u8]) -> Option<()> {
+    match a.sexp(n) {
+        SExp::Atom() => {
+            if a.atom(n) == atom {
+                Some(())
+            } else {
+                None
+            }
+        }
+        _ => None,
     }
 }
 
-fn unwrap_quote(node: Node) -> Option<Node> {
-    let p = node.pair()?;
-    check(&p.0, &[1_u8])?;
-    Some(p.1)
+fn unwrap_quote(a: &Allocator, n: NodePtr) -> Option<NodePtr> {
+    match a.sexp(n) {
+        SExp::Pair(first, rest) => {
+            check(a, first, &[1_u8])?;
+            Some(rest)
+        }
+        _ => None,
+    }
 }
 
 // matches
 // (2 (1 . self) rest)
 // returning (self, rest)
-fn match_wrapper(node: Node) -> Option<(Node, Node)> {
-    let (ev, quoted_inner, args_list) = unwrap3(node)?;
-    check(&ev, &[2_u8])?;
-    let inner = unwrap_quote(quoted_inner)?;
+fn match_wrapper(a: &Allocator, node: NodePtr) -> Option<(NodePtr, NodePtr)> {
+    let [ev, quoted_inner, args_list] = destructure::<3>(a, node)?;
+    check(a, ev, &[2_u8])?;
+    let inner = unwrap_quote(a, quoted_inner)?;
     Some((inner, args_list))
 }
 
 // returns the inner puzzle and the list of arguments, or Err, in case the node
 // is not conforming to the standard curry format
 pub fn uncurry(a: &Allocator, node: NodePtr) -> Option<(NodePtr, Vec<NodePtr>)> {
     let mut ret_args = Vec::<NodePtr>::new();
 
-    let n = Node::new(a, node);
-    let (inner, args) = match_wrapper(n)?;
+    let (inner, mut args) = match_wrapper(a, node)?;
 
-    let mut rest = args;
-    while rest.pair().is_some() {
+    while !nullp(a, args) {
         // match
         // (4 (1 . <arg>) <rest>)
-        let (cons, quoted_arg, r) = unwrap3(rest.clone())?;
-        rest = r;
-        let arg = unwrap_quote(quoted_arg)?;
-        check(&cons, &[4_u8])?;
-        ret_args.push(arg.node);
+        let [cons, quoted_arg, r] = destructure::<3>(a, args)?;
+        args = r;
+        let arg = unwrap_quote(a, quoted_arg)?;
+        check(a, cons, &[4_u8])?;
+        ret_args.push(arg);
     }
-    Some((inner.node, ret_args))
+    Some((inner, ret_args))
 }
 
 // ==== tests ===
 
 #[test]
 fn simple_uncurry() {
     let mut a = Allocator::new();
@@ -100,70 +114,66 @@
     let quote = a.one();
     let foobar = a.new_atom(b"foobar").unwrap();
     let quoted_foobar = a.new_pair(quote, foobar).unwrap();
     let double_quoted_foobar = a.new_pair(quote, quoted_foobar).unwrap();
     let invalid_quote = a.new_pair(a.null(), foobar).unwrap();
 
     // positive tests
+    assert_eq!(unwrap_quote(&a, quoted_foobar).unwrap(), foobar);
+    assert_eq!(unwrap_quote(&a, quoted_foobar).unwrap(), foobar);
     assert_eq!(
-        unwrap_quote(Node::new(&a, quoted_foobar)).unwrap().node,
-        foobar
-    );
-    assert_eq!(
-        unwrap_quote(Node::new(&a, double_quoted_foobar))
-            .unwrap()
-            .node,
+        unwrap_quote(&a, double_quoted_foobar).unwrap(),
         quoted_foobar
     );
 
     // negative tests
-    assert!(unwrap_quote(Node::new(&a, foobar)).is_none());
-    assert!(unwrap_quote(Node::new(&a, invalid_quote)).is_none());
-    assert!(unwrap_quote(Node::new(&a, a.null())).is_none());
+    assert!(unwrap_quote(&a, foobar).is_none());
+    assert!(unwrap_quote(&a, invalid_quote).is_none());
+    assert!(unwrap_quote(&a, a.null()).is_none());
 }
 
 #[test]
 fn test_check() {
     let mut a = Allocator::new();
     let quote = a.one();
     let foobar = a.new_atom(b"foobar").unwrap();
     let quoted_foobar = a.new_pair(quote, foobar).unwrap();
 
-    assert!(check(&Node::new(&a, quote), &[1_u8]).is_some());
-    assert!(check(&Node::new(&a, foobar), b"foobar").is_some());
+    assert!(check(&a, quote, &[1_u8]).is_some());
+    assert!(check(&a, foobar, b"foobar").is_some());
 
     // the wrong atom value
-    assert!(check(&Node::new(&a, foobar), &[1_u8]).is_none());
-    assert!(check(&Node::new(&a, quote), b"foobar").is_none());
+    assert!(check(&a, foobar, &[1_u8]).is_none());
+    assert!(check(&a, quote, b"foobar").is_none());
 
     // pairs alwaus fail
-    assert!(check(&Node::new(&a, quoted_foobar), b"foobar").is_none());
-    assert!(check(&Node::new(&a, quoted_foobar), &[1_u8]).is_none());
+    assert!(check(&a, quoted_foobar, b"foobar").is_none());
+    assert!(check(&a, quoted_foobar, &[1_u8]).is_none());
 }
 
 #[test]
-fn test_unwrap3() {
+fn test_destructure() {
     let mut a = Allocator::new();
     let foobar = a.new_atom(b"foobar").unwrap();
     let list1 = a.new_pair(foobar, a.null()).unwrap();
     let list2 = a.new_pair(foobar, list1).unwrap();
     let list3 = a.new_pair(foobar, list2).unwrap();
     let list4 = a.new_pair(foobar, list3).unwrap();
 
     // negative tests
-    assert!(unwrap3(Node::new(&a, foobar)).is_none());
-    assert!(unwrap3(Node::new(&a, list1)).is_none());
-    assert!(unwrap3(Node::new(&a, list2)).is_none());
-    assert!(unwrap3(Node::new(&a, list4)).is_none());
+    assert!(destructure::<3>(&a, foobar).is_none());
+    assert!(destructure::<3>(&a, list1).is_none());
+    assert!(destructure::<3>(&a, list2).is_none());
+    assert!(destructure::<3>(&a, list4).is_none());
 
     // positive test
-    let foobar_tuple = unwrap3(Node::new(&a, list3)).unwrap();
-    assert!(foobar_tuple.0.node == foobar);
-    assert!(foobar_tuple.1.node == foobar);
-    assert!(foobar_tuple.2.node == foobar);
+    let foobar_array = destructure::<3>(&a, list3).unwrap();
+    assert!(foobar_array[0] == foobar);
+    assert!(foobar_array[1] == foobar);
+    assert!(foobar_array[2] == foobar);
 }
 
 #[test]
 fn test_match_wrapper() {
     let mut a = Allocator::new();
     let apply = a.new_atom(&[2_u8]).unwrap();
     let rest = a.new_atom(b"args").unwrap();
@@ -174,21 +184,21 @@
     let input1 = a.new_pair(quoted_inner, input2).unwrap();
     let input = a.new_pair(apply, input1).unwrap();
     let invalid_input = a.new_pair(a.one(), input1).unwrap();
     let long_input = a.new_pair(apply, input).unwrap();
 
     // input: (2 (1 . self) rest)
     // returns: (self, rest)
-    let matched = match_wrapper(Node::new(&a, input)).unwrap();
-    assert!(matched.0.node == inner);
-    assert!(matched.1.node == rest);
+    let matched = match_wrapper(&a, input).unwrap();
+    assert!(matched.0 == inner);
+    assert!(matched.1 == rest);
 
     // negative tests
-    assert!(match_wrapper(Node::new(&a, long_input)).is_none());
-    assert!(match_wrapper(Node::new(&a, invalid_input)).is_none());
-    assert!(match_wrapper(Node::new(&a, quoted_inner)).is_none());
-    assert!(match_wrapper(Node::new(&a, apply)).is_none());
-    assert!(match_wrapper(Node::new(&a, rest)).is_none());
-    assert!(match_wrapper(Node::new(&a, inner)).is_none());
-    assert!(match_wrapper(Node::new(&a, input2)).is_none());
-    assert!(match_wrapper(Node::new(&a, input1)).is_none());
+    assert!(match_wrapper(&a, long_input).is_none());
+    assert!(match_wrapper(&a, invalid_input).is_none());
+    assert!(match_wrapper(&a, quoted_inner).is_none());
+    assert!(match_wrapper(&a, apply).is_none());
+    assert!(match_wrapper(&a, rest).is_none());
+    assert!(match_wrapper(&a, inner).is_none());
+    assert!(match_wrapper(&a, input2).is_none());
+    assert!(match_wrapper(&a, input1).is_none());
 }
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia_streamable_macro/src/lib.rs` & `chia_rs-0.2.8/local_dependencies/chia_streamable_macro/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/Cargo.toml` & `chia_rs-0.2.8/local_dependencies/chia-protocol/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 repository = "https://github.com/Chia-Network/chia_rs/chia-protocol/"
 
 [features]
 py-bindings = ["dep:pyo3", "dep:chia_py_streamable_macro"]
 
 [dependencies]
 pyo3 = { version = "=0.15.1", features = ["extension-module", "multiple-pymethods"], optional = true }
-sha2 = "=0.10.2"
+sha2 = "=0.9.9"
 hex = "=0.4.3"
 chia_streamable_macro = { version = "=0.2.4", path = "../chia_streamable_macro" }
 chia_py_streamable_macro = { path = "../chia_py_streamable_macro", version = "=0.1.3", optional = true }
-clvmr = "=0.2.4"
+clvmr = "=0.2.6"
 
 [lib]
 crate-type = ["rlib"]
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/bls.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/bls.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/bytes.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/bytes.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/chia_error.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/chia_error.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/chia_protocol.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/chia_protocol.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/classgroup.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/classgroup.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/coin.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/coin.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/coin_spend.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/coin_spend.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/coin_state.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/coin_state.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/end_of_sub_slot_bundle.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/end_of_sub_slot_bundle.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/fee_estimate.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/fee_estimate.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/foliage.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/foliage.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/from_json_dict.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/from_json_dict.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/fullblock.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/fullblock.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/header_block.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/header_block.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/lib.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/message_struct.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/message_struct.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/pool_target.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/pool_target.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/program.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/program.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/proof_of_space.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/proof_of_space.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/reward_chain_block.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/reward_chain_block.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/slots.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/slots.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/spend_bundle.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/spend_bundle.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/streamable.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/streamable.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/to_json_dict.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/to_json_dict.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/vdf.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/vdf.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/wallet_protocol.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/wallet_protocol.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia-protocol/src/weight_proof.rs` & `chia_rs-0.2.8/local_dependencies/chia-protocol/src/weight_proof.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/Cargo.toml` & `chia_rs-0.2.8/local_dependencies/chia/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 # "cargo test" and "cargo bench"
 [workspace]
 members = ["wasm", "chia_streamable_macro", "chia-bls", "clvm-utils", "chia-protocol", "chia_py_streamable_macro", "chia-tools"]
 exclude = ["wheel"]
 
 [package]
 name = "chia"
-version = "0.2.7"
+version = "0.2.8"
 edition = "2021"
 license = "Apache-2.0"
 description = "Utility functions and types used by the Chia blockchain full node"
 authors = ["Richard Kiss <him@richardkiss.com>", "Arvid Norberg <arvid@chia.net>"]
 homepage = "https://github.com/Chia-Network/chia_rs/"
 repository = "https://github.com/Chia-Network/chia_rs/"
 
 [features]
 py-bindings = ["dep:pyo3"]
 
 [dependencies]
-clvmr = "=0.2.4"
+clvmr = "=0.2.6"
 hex = "=0.4.3"
 pyo3 = { version = "=0.15.1", features = ["extension-module"], optional = true }
 clvm-utils = { version = "=0.2.7", path = "../clvm-utils" }
 chia-protocol = { version = "=0.2.7", path = "../chia-protocol" }
+hex-literal = "=0.4.1"
 
 [lib]
 name = "chia"
 crate-type = ["rlib"]
 
 [profile.release]
 lto = true
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia/.github/workflows/benchmark.yml` & `chia_rs-0.2.8/local_dependencies/chia/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/.github/workflows/build-crate-and-npm.yml` & `chia_rs-0.2.8/local_dependencies/chia/.github/workflows/build-crate-and-npm.yml`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/.github/workflows/build-test.yml` & `chia_rs-0.2.8/local_dependencies/chia/.github/workflows/build-test.yml`

 * *Files 3% similar despite different names*

```diff
@@ -164,16 +164,16 @@
         python${{ matrix.python.major-dot-minor }} -m venv venv
         . venv/bin/activate
         maturin build -i python --release -m wheel/Cargo.toml
 
     - name: Build Linux with maturin on Python ${{ matrix.python }}
       if: matrix.os.matrix == 'ubuntu'
       run: |
-        podman run --rm=true \
-          -v ${{ github.workspace }}:/ws:rw --workdir=/ws \
+        docker run --rm \
+          -v ${{ github.workspace }}:/ws --workdir=/ws \
           ${{ matrix.python.by-arch[matrix.arch.matrix].docker-url }} \
           bash -exc '\
             curl -L https://sh.rustup.rs > rustup-init.sh && \
             sh rustup-init.sh -y && \
             yum -y install openssl-devel && \
             source $HOME/.cargo/env && \
             rustup target add ${{ matrix.python.by-arch[matrix.arch.matrix].rustup-target }} && \
@@ -295,29 +295,38 @@
       - name: Install rust
         uses: actions-rs/toolchain@v1
         with:
             toolchain: nightly
             components: rustfmt, clippy
             override: true
       - name: fmt
-        run: cargo fmt --all -- --files-with-diff --check
+        run: |
+            cargo fmt --all -- --files-with-diff --check
+            cd wheel
+            cargo fmt -- --files-with-diff --check
+            cd ../fuzz
+            cargo fmt -- --files-with-diff --check
 
   clippy:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions-rs/toolchain@v1
         with:
           toolchain: nightly
           components: clippy
           override: true
       - uses: actions-rs/clippy-check@v1
         with:
           token: ${{ secrets.GITHUB_TOKEN }}
           args: --all-features --workspace
+      - name: wheel
+        run: |
+            cd wheel
+            cargo clippy
 
   fuzz_targets:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions-rs/toolchain@v1
         with:
@@ -349,22 +358,61 @@
   unit_tests:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [macos-latest, ubuntu-latest, windows-latest]
     name: Unit tests
     steps:
+      # the test files are read verbatim, making it problematic if git is
+      # allowed to insert \r when checking out files
+      - name: disable git autocrlf
+        run: |
+          git config --global core.autocrlf false
+
       - uses: actions/checkout@v3
         with:
           fetch-depth: 1
       - uses: actions-rs/toolchain@v1
         with:
             toolchain: stable
+      - name: Prepare for coverage
+        if: matrix.os == 'ubuntu-latest'
+        run: |
+          cargo install grcov
+          echo "RUSTFLAGS=-Cinstrument-coverage" >> "$GITHUB_ENV"
+          echo "LLVM_PROFILE_FILE=$(pwd)/target/chia_rs-%p-%m.profraw" >> "$GITHUB_ENV"
+          echo "CARGO_TARGET_DIR=$(pwd)/target" >> "$GITHUB_ENV"
       - name: cargo test
         run: cargo test --workspace
+      - name: Continue with coverage
+        if: matrix.os == 'ubuntu-latest'
+        run: |
+          sudo apt-get update
+          sudo apt-get install lcov -y
+          rustup component add llvm-tools-preview
+          python -m venv venv
+          source venv/bin/activate
+          git clone https://github.com/Chia-Network/clvm_tools.git --branch=main --single-branch
+          pip install ./clvm_tools
+          pip install colorama maturin pytest
+          maturin develop --release -m wheel/Cargo.toml
+          cd tests
+          python generate-programs.py
+          python run-programs.py || true
+          cd ..
+          pytest tests
+          grcov . --binary-path target -s . --branch --ignore-not-existing --ignore='*/.cargo/*' --ignore='tests/*' --ignore='venv/*' -o rust_cov.info
+          python -c 'with open("rust_cov.info") as f: lines = [l for l in f if not (l.startswith("DA:") and int(l.split(",")[1].strip()) >= 2**63)]; open("lcov.info", "w").writelines(lines)'
+      - name: Upload to Coveralls
+        uses: coverallsapp/github-action@v2
+        if: matrix.os == 'ubuntu-latest'
+        env:
+          COVERALLS_REPO_TOKEN: ${{ secrets.COVERALLS_REPO_TOKEN }}
+        with:
+          path-to-lcov: './lcov.info'
 
   upload:
     name: Upload to PyPI - ${{ matrix.os.name }} ${{ matrix.python.major-dot-minor }} ${{ matrix.arch.name }}
     runs-on: ${{ matrix.os.runs-on[matrix.arch.matrix] }}
     needs:
       - build-wheels
       - build-sdist
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia/LICENSE` & `chia_rs-0.2.8/local_dependencies/chia/LICENSE`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/cl/deserialize_w_backrefs.cl` & `chia_rs-0.2.8/local_dependencies/chia/cl/deserialize_w_backrefs.cl`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/docs/implementation-notes.md` & `chia_rs-0.2.8/local_dependencies/chia/docs/implementation-notes.md`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/examples/README.md` & `chia_rs-0.2.8/local_dependencies/chia/examples/README.md`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/examples/block-1519806.bin` & `chia_rs-0.2.8/local_dependencies/chia/examples/block-1519806.bin`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/examples/streaming-patch.diff` & `chia_rs-0.2.8/local_dependencies/chia/examples/streaming-patch.diff`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/src/compression/compressor.rs` & `chia_rs-0.2.8/local_dependencies/chia/src/compression/compressor.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 use clvmr::allocator::{Allocator, NodePtr};
-use clvmr::node::Node;
 use clvmr::serde::{
     node_from_bytes, node_from_bytes_backrefs, node_to_bytes, node_to_bytes_backrefs,
 };
 
 pub fn wrap_atom_with_decompression_program(
     allocator: &mut Allocator,
     node_ptr: NodePtr,
@@ -27,17 +26,13 @@
 pub fn decompress(allocator: &mut Allocator, blob: &[u8]) -> Result<NodePtr, std::io::Error> {
     node_from_bytes_backrefs(allocator, blob)
 }
 
 pub fn create_autoextracting_clvm_program(input_program: &[u8]) -> std::io::Result<Vec<u8>> {
     let mut allocator = Allocator::new();
     let node_ptr = decompress(&mut allocator, input_program)?;
-    let node = Node {
-        allocator: &allocator,
-        node: node_ptr,
-    };
-    let compressed_block = node_to_bytes_backrefs(&node).expect("can't compress");
+    let compressed_block = node_to_bytes_backrefs(&allocator, node_ptr).expect("can't compress");
     let compressed_block_as_atom = allocator.new_atom(&compressed_block)?;
     let decompression_program_ptr =
         wrap_atom_with_decompression_program(&mut allocator, compressed_block_as_atom)?;
-    node_to_bytes(&Node::new(&allocator, decompression_program_ptr))
+    node_to_bytes(&allocator, decompression_program_ptr)
 }
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia/src/compression/deserialize_w_backrefs.bin` & `chia_rs-0.2.8/local_dependencies/chia/src/compression/deserialize_w_backrefs.bin`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/src/fuzzing_utils.rs` & `chia_rs-0.2.8/local_dependencies/chia/src/fuzzing_utils.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/src/gen/coin_id.rs` & `chia_rs-0.2.8/local_dependencies/chia/src/gen/coin_id.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/src/gen/condition_sanitizers.rs` & `chia_rs-0.2.8/local_dependencies/chia/src/gen/condition_sanitizers.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/src/gen/conditions.rs` & `chia_rs-0.2.8/local_dependencies/chia/src/gen/conditions.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 use super::coin_id::compute_coin_id;
 use super::condition_sanitizers::{parse_amount, sanitize_announce_msg, sanitize_hash};
 use super::opcodes::{
-    parse_opcode, ConditionOpcode, AGG_SIG_COST, AGG_SIG_ME, AGG_SIG_UNSAFE, ALWAYS_TRUE,
-    ASSERT_BEFORE_HEIGHT_ABSOLUTE, ASSERT_BEFORE_HEIGHT_RELATIVE, ASSERT_BEFORE_SECONDS_ABSOLUTE,
-    ASSERT_BEFORE_SECONDS_RELATIVE, ASSERT_COIN_ANNOUNCEMENT, ASSERT_CONCURRENT_PUZZLE,
-    ASSERT_CONCURRENT_SPEND, ASSERT_EPHEMERAL, ASSERT_HEIGHT_ABSOLUTE, ASSERT_HEIGHT_RELATIVE,
-    ASSERT_MY_AMOUNT, ASSERT_MY_BIRTH_HEIGHT, ASSERT_MY_BIRTH_SECONDS, ASSERT_MY_COIN_ID,
-    ASSERT_MY_PARENT_ID, ASSERT_MY_PUZZLEHASH, ASSERT_PUZZLE_ANNOUNCEMENT, ASSERT_SECONDS_ABSOLUTE,
-    ASSERT_SECONDS_RELATIVE, CREATE_COIN, CREATE_COIN_ANNOUNCEMENT, CREATE_COIN_COST,
-    CREATE_PUZZLE_ANNOUNCEMENT, RESERVE_FEE,
+    compute_unknown_condition_cost, parse_opcode, ConditionOpcode, AGG_SIG_COST, AGG_SIG_ME,
+    AGG_SIG_UNSAFE, ASSERT_BEFORE_HEIGHT_ABSOLUTE, ASSERT_BEFORE_HEIGHT_RELATIVE,
+    ASSERT_BEFORE_SECONDS_ABSOLUTE, ASSERT_BEFORE_SECONDS_RELATIVE, ASSERT_COIN_ANNOUNCEMENT,
+    ASSERT_CONCURRENT_PUZZLE, ASSERT_CONCURRENT_SPEND, ASSERT_EPHEMERAL, ASSERT_HEIGHT_ABSOLUTE,
+    ASSERT_HEIGHT_RELATIVE, ASSERT_MY_AMOUNT, ASSERT_MY_BIRTH_HEIGHT, ASSERT_MY_BIRTH_SECONDS,
+    ASSERT_MY_COIN_ID, ASSERT_MY_PARENT_ID, ASSERT_MY_PUZZLEHASH, ASSERT_PUZZLE_ANNOUNCEMENT,
+    ASSERT_SECONDS_ABSOLUTE, ASSERT_SECONDS_RELATIVE, CREATE_COIN, CREATE_COIN_ANNOUNCEMENT,
+    CREATE_COIN_COST, CREATE_PUZZLE_ANNOUNCEMENT, REMARK, RESERVE_FEE, SOFTFORK,
 };
 use super::sanitize_int::{sanitize_uint, SanitizedUint};
 use super::validation_error::{first, next, rest, ErrorCode, ValidationErr};
-use crate::gen::flags::COND_ARGS_NIL;
-use crate::gen::flags::NO_RELATIVE_CONDITIONS_ON_EPHEMERAL;
-use crate::gen::flags::NO_UNKNOWN_CONDS;
-use crate::gen::flags::STRICT_ARGS_COUNT;
+use crate::gen::flags::{
+    AGG_SIG_ARGS, COND_ARGS_NIL, LIMIT_ANNOUNCES, NO_RELATIVE_CONDITIONS_ON_EPHEMERAL,
+    NO_UNKNOWN_CONDS, STRICT_ARGS_COUNT,
+};
 use crate::gen::validation_error::check_nil;
 use chia_protocol::bytes::Bytes32;
 use clvmr::allocator::{Allocator, NodePtr, SExp};
 use clvmr::cost::Cost;
 use clvmr::sha2::{Digest, Sha256};
 use std::cmp::{max, min};
 use std::collections::{HashMap, HashSet};
@@ -95,14 +95,18 @@
     AssertBeforeSecondsRelative(u64),
     AssertBeforeSecondsAbsolute(u64),
     // block height
     AssertBeforeHeightRelative(u32),
     AssertBeforeHeightAbsolute(u32),
     AssertEphemeral,
 
+    // The softfork condition is one that we don't understand, it just applies
+    // the specified cost
+    Softfork(Cost),
+
     // this means the condition is unconditionally true and can be skipped
     Skip,
     SkipRelativeCondition,
 }
 
 fn maybe_check_args_terminator(
     a: &Allocator,
@@ -127,39 +131,43 @@
             c = rest(a, c)?;
             let message = sanitize_announce_msg(a, first(a, c)?, ErrorCode::InvalidMessage)?;
             // AGG_SIG_UNSAFE takes exactly two parameters
             if (flags & COND_ARGS_NIL) != 0 {
                 // make sure there aren't more than two
                 check_nil(a, rest(a, c)?)?;
                 Ok(Condition::AggSigUnsafe(pubkey, message))
-            } else {
+            } else if (flags & AGG_SIG_ARGS) == 0 {
                 // but the argument list still doesn't need to be terminated by NIL,
                 // just any atom will do
                 match a.sexp(rest(a, c)?) {
                     SExp::Pair(_, _) => Err(ValidationErr(c, ErrorCode::InvalidCondition)),
                     _ => Ok(Condition::AggSigUnsafe(pubkey, message)),
                 }
+            } else {
+                Ok(Condition::AggSigUnsafe(pubkey, message))
             }
         }
         AGG_SIG_ME => {
             let pubkey = sanitize_hash(a, first(a, c)?, 48, ErrorCode::InvalidPubkey)?;
             c = rest(a, c)?;
             let message = sanitize_announce_msg(a, first(a, c)?, ErrorCode::InvalidMessage)?;
             // AGG_SIG_ME takes exactly two parameters
             if (flags & COND_ARGS_NIL) != 0 {
                 // make sure there aren't more than two
                 check_nil(a, rest(a, c)?)?;
                 Ok(Condition::AggSigMe(pubkey, message))
-            } else {
+            } else if (flags & AGG_SIG_ARGS) == 0 {
                 // but the argument list still doesn't need to be terminated by NIL,
                 // just any atom will do
                 match a.sexp(rest(a, c)?) {
                     SExp::Pair(_, _) => Err(ValidationErr(c, ErrorCode::InvalidCondition)),
                     _ => Ok(Condition::AggSigMe(pubkey, message)),
                 }
+            } else {
+                Ok(Condition::AggSigMe(pubkey, message))
             }
         }
         CREATE_COIN => {
             let puzzle_hash = sanitize_hash(a, first(a, c)?, 32, ErrorCode::InvalidPuzzleHash)?;
             c = rest(a, c)?;
             let node = first(a, c)?;
             let amount = match sanitize_uint(a, node, 8, ErrorCode::InvalidCoinAmount)? {
@@ -184,25 +192,48 @@
             // there was another item in the list
             if let Ok(params) = first(a, c) {
                 // the item was a cons-box, and params is the left-hand
                 // side, the list element
                 maybe_check_args_terminator(a, c, flags)?;
                 if let Ok(param) = first(a, params) {
                     // pull out the first item (param)
-                    if let SExp::Atom(b) = a.sexp(param) {
-                        if a.buf(&b).len() <= 32 {
+                    if let SExp::Atom() = a.sexp(param) {
+                        if a.atom_len(param) <= 32 {
                             return Ok(Condition::CreateCoin(puzzle_hash, amount, param));
                         }
                     }
                 }
             } else if (flags & STRICT_ARGS_COUNT) != 0 {
                 check_nil(a, c)?;
             }
             Ok(Condition::CreateCoin(puzzle_hash, amount, a.null()))
         }
+        SOFTFORK => {
+            if (flags & NO_UNKNOWN_CONDS) != 0 {
+                // We don't know of any new softforked-in conditions, so they
+                // are all unknown
+                Err(ValidationErr(c, ErrorCode::InvalidConditionOpcode))
+            } else {
+                match sanitize_uint(a, first(a, c)?, 4, ErrorCode::InvalidSoftforkCost)? {
+                    // the first argument represents the cost of the condition.
+                    // We scale it by 10000 to make the argument be a bit smaller
+                    SanitizedUint::Ok(cost) => Ok(Condition::Softfork(cost * 10000)),
+                    _ => Err(ValidationErr(c, ErrorCode::InvalidSoftforkCost)),
+                }
+            }
+        }
+        256..=65535 => {
+            // All of these conditions are unknown
+            // but they have costs (when ENABLE_SOFTFORK_CONDITION is enabled)
+            if (flags & NO_UNKNOWN_CONDS) != 0 {
+                Err(ValidationErr(c, ErrorCode::InvalidConditionOpcode))
+            } else {
+                Ok(Condition::Softfork(compute_unknown_condition_cost(op)))
+            }
+        }
         RESERVE_FEE => {
             maybe_check_args_terminator(a, c, flags)?;
             let fee = parse_amount(a, first(a, c)?, ErrorCode::ReserveFeeConditionFailed)?;
             Ok(Condition::ReserveFee(fee))
         }
         CREATE_COIN_ANNOUNCEMENT => {
             maybe_check_args_terminator(a, c, flags)?;
@@ -363,23 +394,23 @@
             let code = ErrorCode::AssertBeforeHeightAbsolute;
             match sanitize_uint(a, node, 4, code)? {
                 SanitizedUint::PositiveOverflow => Ok(Condition::Skip),
                 SanitizedUint::NegativeOverflow => Err(ValidationErr(node, code)),
                 SanitizedUint::Ok(r) => Ok(Condition::AssertBeforeHeightAbsolute(r as u32)),
             }
         }
-        ALWAYS_TRUE => {
+        REMARK => {
             // this condition is always true, we always ignore arguments
             Ok(Condition::Skip)
         }
         _ => Err(ValidationErr(c, ErrorCode::InvalidConditionOpcode)),
     }
 }
 
-#[derive(Debug)]
+#[derive(Debug, Clone)]
 pub struct NewCoin {
     pub puzzle_hash: Bytes32,
     pub amount: u64,
     // the hint is optional. When not provided, this points to null (NodePtr
     // value -1). The hint is not part of the unique identity of a coin, it's not
     // hashed when computing the coin ID
     pub hint: NodePtr,
@@ -406,15 +437,15 @@
 // nor AGG_SIG_UNSAFE
 pub const ELIGIBLE_FOR_DEDUP: u32 = 1;
 
 // If the spend bundle contained *any* relative seconds or height condition, this flag is set
 pub const HAS_RELATIVE_CONDITION: u32 = 2;
 
 // These are all the conditions related directly to a specific spend.
-#[derive(Debug)]
+#[derive(Debug, Clone)]
 pub struct Spend {
     // the parent coin ID of the coin being spent
     pub parent_id: NodePtr,
     // the amount of the coin that's being spent
     pub coin_amount: u64,
     // the puzzle hash of the p
     pub puzzle_hash: NodePtr,
@@ -531,39 +562,57 @@
     // ASSERT_BEFORE_SECONDS_RELATIVE
     // ASSERT_MY_BIRTH_SECONDS
     // ASSERT_MY_BIRTH_HEIGHT
     // each item is the index into the SpendBundleConditions::spends vector
     assert_not_ephemeral: HashSet<usize>,
 }
 
+// returns (parent-id, puzzle-hash, amount, condition-list)
 pub(crate) fn parse_single_spend(
-    ret: &mut SpendBundleConditions,
     a: &Allocator,
-    state: &mut ParseState,
     mut spend: NodePtr,
+) -> Result<(NodePtr, NodePtr, NodePtr, NodePtr), ValidationErr> {
+    let parent_id = first(a, spend)?;
+    spend = rest(a, spend)?;
+    let puzzle_hash = first(a, spend)?;
+    spend = rest(a, spend)?;
+    let amount = first(a, spend)?;
+    spend = rest(a, spend)?;
+    let cond = first(a, spend)?;
+    // the rest() here is spend_level_extr. Typically nil
+    Ok((parent_id, puzzle_hash, amount, cond))
+}
+
+#[allow(clippy::too_many_arguments)]
+pub fn process_single_spend(
+    a: &Allocator,
+    ret: &mut SpendBundleConditions,
+    state: &mut ParseState,
+    parent_id: NodePtr,
+    puzzle_hash: NodePtr,
+    amount: NodePtr,
+    conditions: NodePtr,
     flags: u32,
     max_cost: &mut Cost,
 ) -> Result<(), ValidationErr> {
-    let parent_id = sanitize_hash(a, first(a, spend)?, 32, ErrorCode::InvalidParentId)?;
-    spend = rest(a, spend)?;
-    let puzzle_hash = sanitize_hash(a, first(a, spend)?, 32, ErrorCode::InvalidPuzzleHash)?;
-    spend = rest(a, spend)?;
-    let my_amount = parse_amount(a, first(a, spend)?, ErrorCode::InvalidCoinAmount)?;
-    let cond = rest(a, spend)?;
-    let amount_buf = a.atom(first(a, spend)?);
+    let parent_id = sanitize_hash(a, parent_id, 32, ErrorCode::InvalidParentId)?;
+    let puzzle_hash = sanitize_hash(a, puzzle_hash, 32, ErrorCode::InvalidPuzzleHash)?;
+    let my_amount = parse_amount(a, amount, ErrorCode::InvalidCoinAmount)?;
+    let amount_buf = a.atom(amount);
+
     let coin_id = Arc::new(compute_coin_id(a, parent_id, puzzle_hash, amount_buf));
 
     if state
         .spent_coins
         .insert(coin_id.clone(), ret.spends.len())
         .is_some()
     {
         // if this coin ID has already been added to this set, it's a double
         // spend
-        return Err(ValidationErr(spend, ErrorCode::DoubleSpend));
+        return Err(ValidationErr(parent_id, ErrorCode::DoubleSpend));
     }
 
     state.spent_puzzles.insert(puzzle_hash);
 
     ret.removal_amount += my_amount as u128;
 
     let coin_spend = Spend {
@@ -579,36 +628,50 @@
         birth_seconds: None,
         create_coin: HashSet::new(),
         agg_sig_me: Vec::new(),
         // assume it's eligible until we see an agg-sig condition
         flags: ELIGIBLE_FOR_DEDUP,
     };
 
-    let iter = first(a, cond)?;
-    parse_conditions(a, ret, state, coin_spend, iter, flags, max_cost)
+    parse_conditions(a, ret, state, coin_spend, conditions, flags, max_cost)
 }
 
 fn assert_not_ephemeral(spend_flags: &mut u32, state: &mut ParseState, idx: usize) {
     if (*spend_flags & HAS_RELATIVE_CONDITION) != 0 {
         return;
     }
 
     state.assert_not_ephemeral.insert(idx);
     *spend_flags |= HAS_RELATIVE_CONDITION;
 }
 
+fn decrement(cnt: &mut u32, n: NodePtr) -> Result<(), ValidationErr> {
+    if *cnt == 0 {
+        Err(ValidationErr(n, ErrorCode::TooManyAnnouncements))
+    } else {
+        *cnt -= 1;
+        Ok(())
+    }
+}
+
 pub fn parse_conditions(
     a: &Allocator,
     ret: &mut SpendBundleConditions,
     state: &mut ParseState,
     mut spend: Spend,
     mut iter: NodePtr,
     flags: u32,
     max_cost: &mut Cost,
 ) -> Result<(), ValidationErr> {
+    let mut announce_countdown: u32 = if (flags & LIMIT_ANNOUNCES) != 0 {
+        1024
+    } else {
+        u32::MAX
+    };
+
     while let Some((mut c, next)) = next(a, iter)? {
         iter = next;
         let op = match parse_opcode(a, first(a, c)?, flags) {
             None => {
                 // in strict mode we don't allow unknown conditions
                 if (flags & NO_UNKNOWN_CONDS) != 0 {
                     return Err(ValidationErr(c, ErrorCode::InvalidConditionOpcode));
@@ -801,39 +864,51 @@
             }
             Condition::AssertMyPuzzlehash(hash) => {
                 if a.atom(hash) != a.atom(spend.puzzle_hash) {
                     return Err(ValidationErr(c, ErrorCode::AssertMyPuzzlehashFailed));
                 }
             }
             Condition::CreateCoinAnnouncement(msg) => {
+                decrement(&mut announce_countdown, msg)?;
                 state.announce_coin.insert((spend.coin_id.clone(), msg));
             }
             Condition::CreatePuzzleAnnouncement(msg) => {
+                decrement(&mut announce_countdown, msg)?;
                 state.announce_puzzle.insert((spend.puzzle_hash, msg));
             }
             Condition::AssertCoinAnnouncement(msg) => {
+                decrement(&mut announce_countdown, msg)?;
                 state.assert_coin.insert(msg);
             }
             Condition::AssertPuzzleAnnouncement(msg) => {
+                decrement(&mut announce_countdown, msg)?;
                 state.assert_puzzle.insert(msg);
             }
             Condition::AssertConcurrentSpend(id) => {
+                decrement(&mut announce_countdown, id)?;
                 state.assert_concurrent_spend.insert(id);
             }
             Condition::AssertConcurrentPuzzle(id) => {
+                decrement(&mut announce_countdown, id)?;
                 state.assert_concurrent_puzzle.insert(id);
             }
             Condition::AggSigMe(pk, msg) => {
                 spend.agg_sig_me.push((pk, msg));
                 spend.flags &= !ELIGIBLE_FOR_DEDUP;
             }
             Condition::AggSigUnsafe(pk, msg) => {
                 ret.agg_sig_unsafe.push((pk, msg));
                 spend.flags &= !ELIGIBLE_FOR_DEDUP;
             }
+            Condition::Softfork(cost) => {
+                if *max_cost < cost {
+                    return Err(ValidationErr(c, ErrorCode::CostExceeded));
+                }
+                *max_cost -= cost;
+            }
             Condition::SkipRelativeCondition => {
                 assert_not_ephemeral(&mut spend.flags, state, ret.spends.len());
             }
             Condition::Skip => {}
         }
     }
 
@@ -883,17 +958,42 @@
     while let Some((spend, next)) = next(a, iter)? {
         iter = next;
         // cost_left is passed in as a mutable reference and decremented by the
         // cost of the condition (if it has a cost). This let us fail as early
         // as possible if cost is exceeded
         // this function adds the spend to the passed-in ret
         // as well as updates it with any conditions
-        parse_single_spend(&mut ret, a, &mut state, spend, flags, &mut cost_left)?;
+        let (parent_id, puzzle_hash, amount, conds) = parse_single_spend(a, spend)?;
+
+        process_single_spend(
+            a,
+            &mut ret,
+            &mut state,
+            parent_id,
+            puzzle_hash,
+            amount,
+            conds,
+            flags,
+            &mut cost_left,
+        )?;
     }
 
+    validate_conditions(a, &ret, state, spends, flags)?;
+    ret.cost = max_cost - cost_left;
+
+    Ok(ret)
+}
+
+pub fn validate_conditions(
+    a: &Allocator,
+    ret: &SpendBundleConditions,
+    state: ParseState,
+    spends: NodePtr,
+    flags: u32,
+) -> Result<(), ValidationErr> {
     if ret.removal_amount < ret.addition_amount {
         // The sum of removal amounts must not be less than the sum of addition
         // amounts
         return Err(ValidationErr(spends, ErrorCode::MintingCoin));
     }
 
     if ret.removal_amount - ret.addition_amount < ret.reserve_fee as u128 {
@@ -1021,17 +1121,15 @@
         }
     }
 
     // TODO: there may be more failures that can be detected early here, for
     // example an assert-my-birth-height that's incompatible assert-height or
     // assert-before-height. Same thing for the seconds counterpart
 
-    ret.cost = max_cost - cost_left;
-
-    Ok(ret)
+    Ok(())
 }
 
 #[cfg(test)]
 fn u64_to_bytes(n: u64) -> Vec<u8> {
     let mut buf = Vec::<u8>::new();
     buf.extend_from_slice(&n.to_be_bytes());
     if (buf[0] & 0x80) != 0 {
@@ -1042,17 +1140,17 @@
         }
     }
     buf
 }
 #[cfg(test)]
 use crate::gen::flags::ENABLE_ASSERT_BEFORE;
 #[cfg(test)]
-use clvmr::node::Node;
+use crate::gen::flags::ENABLE_SOFTFORK_CONDITION;
 #[cfg(test)]
-use clvmr::number::{ptr_from_number, Number};
+use clvmr::number::Number;
 #[cfg(test)]
 use clvmr::serde::node_to_bytes;
 #[cfg(test)]
 use hex::FromHex;
 #[cfg(test)]
 use num_traits::Num;
 #[cfg(test)]
@@ -1152,15 +1250,15 @@
 // (1 (2 (3 ) means: (1 . (2 . (3 . ())))
 // and:
 
 #[cfg(test)]
 fn parse_list_impl(
     a: &mut Allocator,
     input: &str,
-    callback: &Option<fn(&mut Allocator) -> NodePtr>,
+    callback: &Option<Box<dyn Fn(&mut Allocator) -> NodePtr>>,
     subs: &HashMap<&'static str, NodePtr>,
 ) -> (NodePtr, usize) {
     // skip whitespace
     if input.starts_with(" ") {
         let (n, skip) = parse_list_impl(a, &input[1..], callback, subs);
         return (n, skip + 1);
     }
@@ -1173,37 +1271,37 @@
         (a.new_pair(first, rest).unwrap(), 1 + step1 + step2)
     } else if input.starts_with("{") {
         // substitute '{X}' tokens with our test hashes and messages
         // this keeps the test cases a lot simpler
         let var = input[1..].split_once("}").unwrap().0;
 
         let ret = match var {
-            "" => callback.unwrap()(a),
+            "" => callback.as_ref().unwrap()(a),
             _ => *subs.get(var).unwrap(),
         };
         (ret, var.len() + 2)
     } else if input.starts_with("0x") {
         let v = input.split_once(" ").unwrap().0;
 
         let buf = Vec::from_hex(v.strip_prefix("0x").unwrap()).unwrap();
         (a.new_atom(&buf).unwrap(), v.len() + 1)
     } else if input.starts_with("-") || "0123456789".contains(input.get(0..1).unwrap()) {
         let v = input.split_once(" ").unwrap().0;
         let num = Number::from_str_radix(v, 10).unwrap();
-        (ptr_from_number(a, &num).unwrap(), v.len() + 1)
+        (a.new_number(num).unwrap(), v.len() + 1)
     } else {
         panic!("atom not supported \"{}\"", input);
     }
 }
 
 #[cfg(test)]
 fn parse_list(
     a: &mut Allocator,
     input: &str,
-    callback: &Option<fn(&mut Allocator) -> NodePtr>,
+    callback: &Option<Box<dyn Fn(&mut Allocator) -> NodePtr>>,
 ) -> NodePtr {
     // all substitutions are allocated up-front in order to have them all use
     // the same atom in the CLVM structure. This is to cover cases where
     // conditions may be deduplicated based on the NodePtr value, when they
     // shouldn't be. The AggSig conditions are stored with NodePtr values, but
     // should never be deduplicated.
     let mut subs = HashMap::<&'static str, NodePtr>::new();
@@ -1267,22 +1365,22 @@
 // The callback can be used for arbitrary substitutions using {} in the input
 // string. Since the parser is recursive and simple, large structures have to be
 // constructed this way
 #[cfg(test)]
 fn cond_test_cb(
     input: &str,
     flags: u32,
-    callback: Option<fn(&mut Allocator) -> NodePtr>,
+    callback: Option<Box<dyn Fn(&mut Allocator) -> NodePtr>>,
 ) -> Result<(Allocator, SpendBundleConditions), ValidationErr> {
     let mut a = Allocator::new();
 
     println!("input: {}", input);
 
     let n = parse_list(&mut a, &input, &callback);
-    for c in node_to_bytes(&Node::new(&a, n)).unwrap() {
+    for c in node_to_bytes(&a, n).unwrap() {
         print!("{:02x}", c);
     }
     println!();
     match parse_spends(&a, n, 11000000000, flags) {
         Ok(list) => {
             for n in &list.spends {
                 println!("{:?}", n);
@@ -2497,15 +2595,15 @@
 fn test_create_coin_exceed_cost() {
     // CREATE_COIN
     // ensure that we terminate parsing conditions once they exceed the max cost
     assert_eq!(
         cond_test_cb(
             "((({h1} ({h2} (123 ({} )))",
             0,
-            Some(|a: &mut Allocator| -> NodePtr {
+            Some(Box::new(|a: &mut Allocator| -> NodePtr {
                 let mut rest: NodePtr = a.null();
 
                 for i in 0..6500 {
                     // this builds one CREATE_COIN condition
                     // borrow-rules prevent this from being succint
                     let coin = a.null();
                     let val = a.new_atom(&u64_to_bytes(i)).unwrap();
@@ -2515,15 +2613,15 @@
                     let val = a.new_atom(&u64_to_bytes(CREATE_COIN as u64)).unwrap();
                     let coin = a.new_pair(val, coin).unwrap();
 
                     // add the CREATE_COIN condition to the list (called rest)
                     rest = a.new_pair(coin, rest).unwrap();
                 }
                 rest
-            })
+            }))
         )
         .unwrap_err()
         .1,
         ErrorCode::CostExceeded
     );
 }
 
@@ -2619,15 +2717,15 @@
 fn test_agg_sig_me_exceed_cost() {
     // AGG_SIG_ME
     // ensure that we terminate parsing conditions once they exceed the max cost
     assert_eq!(
         cond_test_cb(
             "((({h1} ({h2} (123 ({} )))",
             0,
-            Some(|a: &mut Allocator| -> NodePtr {
+            Some(Box::new(|a: &mut Allocator| -> NodePtr {
                 let mut rest: NodePtr = a.null();
 
                 for _i in 0..9167 {
                     // this builds one AGG_SIG_ME condition
                     // borrow-rules prevent this from being succint
                     let aggsig = a.null();
                     let val = a.new_atom(MSG1).unwrap();
@@ -2637,15 +2735,15 @@
                     let val = a.new_atom(&u64_to_bytes(AGG_SIG_ME as u64)).unwrap();
                     let aggsig = a.new_pair(val, aggsig).unwrap();
 
                     // add the AGG_SIG_ME condition to the list (called rest)
                     rest = a.new_pair(aggsig, rest).unwrap();
                 }
                 rest
-            })
+            }))
         )
         .unwrap_err()
         .1,
         ErrorCode::CostExceeded
     );
 }
 
@@ -2690,14 +2788,64 @@
             .unwrap_err()
             .1,
         ErrorCode::InvalidCondition
     );
 }
 
 #[test]
+fn test_agg_sig_unsafe_extra_arg_allowed() {
+    // AGG_SIG_UNSAFE
+    // extra args are allowed when the AGG_SIG_ARGS flag is set
+    let (a, conds) = cond_test_flag(
+        "((({h1} ({h2} (123 (((49 ({pubkey} ({msg1} (456 )))))",
+        AGG_SIG_ARGS,
+    )
+    .unwrap();
+
+    assert_eq!(conds.cost, AGG_SIG_COST);
+    assert_eq!(conds.spends.len(), 1);
+    assert_eq!(conds.removal_amount, 123);
+    assert_eq!(conds.addition_amount, 0);
+    let spend = &conds.spends[0];
+    assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
+    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(conds.agg_sig_unsafe.len(), 1);
+    for (pk, msg) in &conds.agg_sig_unsafe {
+        assert_eq!(a.atom(*pk), PUBKEY);
+        assert_eq!(a.atom(*msg), MSG1);
+    }
+    assert_eq!(spend.flags, 0);
+}
+
+#[test]
+fn test_agg_sig_me_extra_arg_allowed() {
+    // AGG_SIG_ME
+    // extra args are allowed when the AGG_SIG_ARGS flag is set
+    let (a, conds) = cond_test_flag(
+        "((({h1} ({h2} (123 (((50 ({pubkey} ({msg1} (456 )))))",
+        AGG_SIG_ARGS,
+    )
+    .unwrap();
+
+    assert_eq!(conds.cost, AGG_SIG_COST);
+    assert_eq!(conds.spends.len(), 1);
+    assert_eq!(conds.removal_amount, 123);
+    assert_eq!(conds.addition_amount, 0);
+    let spend = &conds.spends[0];
+    assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
+    assert_eq!(a.atom(spend.puzzle_hash), H2);
+    assert_eq!(spend.agg_sig_me.len(), 1);
+    for c in &spend.agg_sig_me {
+        assert_eq!(a.atom(c.0), PUBKEY);
+        assert_eq!(a.atom(c.1), MSG1);
+    }
+    assert_eq!(spend.flags, 0);
+}
+
+#[test]
 fn test_agg_sig_unsafe_invalid_terminator() {
     // AGG_SIG_UNSAFE
     // in non-mempool mode, even an invalid terminator is allowed
     let (a, conds) =
         cond_test_flag("((({h1} ({h2} (123 (((49 ({pubkey} ({msg1} 456 ))))", 0).unwrap();
 
     assert_eq!(conds.cost, AGG_SIG_COST);
@@ -2817,15 +2965,15 @@
 fn test_agg_sig_unsafe_exceed_cost() {
     // AGG_SIG_UNSAFE
     // ensure that we terminate parsing conditions once they exceed the max cost
     assert_eq!(
         cond_test_cb(
             "((({h1} ({h2} (123 ({} )))",
             0,
-            Some(|a: &mut Allocator| -> NodePtr {
+            Some(Box::new(|a: &mut Allocator| -> NodePtr {
                 let mut rest: NodePtr = a.null();
 
                 for _i in 0..9167 {
                     // this builds one AGG_SIG_UNSAFE condition
                     // borrow-rules prevent this from being succint
                     let aggsig = a.null();
                     let val = a.new_atom(MSG1).unwrap();
@@ -2835,15 +2983,15 @@
                     let val = a.new_atom(&u64_to_bytes(AGG_SIG_UNSAFE as u64)).unwrap();
                     let aggsig = a.new_pair(val, aggsig).unwrap();
 
                     // add the AGG_SIG_UNSAFE condition to the list (called rest)
                     rest = a.new_pair(aggsig, rest).unwrap();
                 }
                 rest
-            })
+            }))
         )
         .unwrap_err()
         .1,
         ErrorCode::CostExceeded
     );
 }
 
@@ -2893,16 +3041,16 @@
             .unwrap_err()
             .1,
         ErrorCode::DoubleSpend
     );
 }
 
 #[test]
-fn test_always_true() {
-    // ALWAYS_TRUE
+fn test_remark() {
+    // REMARK
     let (a, conds) = cond_test("((({h1} ({h2} (123 (((1 )))))").unwrap();
 
     // just make sure there are no constraints
     assert_eq!(conds.agg_sig_unsafe.len(), 0);
     assert_eq!(conds.reserve_fee, 0);
     assert_eq!(conds.height_absolute, 0);
     assert_eq!(conds.seconds_absolute, 0);
@@ -2916,16 +3064,16 @@
     assert_eq!(*spend.coin_id, test_coin_id(H1, H2, 123));
     assert_eq!(a.atom(spend.puzzle_hash), H2);
     assert_eq!(spend.agg_sig_me.len(), 0);
     assert_eq!(spend.flags, ELIGIBLE_FOR_DEDUP);
 }
 
 #[test]
-fn test_always_true_with_arg() {
-    // ALWAYS_TRUE, but with one unknown argument
+fn test_remark_with_arg() {
+    // REMARK, but with one unknown argument
     // unknown arguments are expected and always allowed
     let (a, conds) = cond_test("((({h1} ({h2} (123 (((1 ( 42 )))))").unwrap();
 
     // just make sure there are no constraints
     assert_eq!(conds.agg_sig_unsafe.len(), 0);
     assert_eq!(conds.reserve_fee, 0);
     assert_eq!(conds.height_absolute, 0);
@@ -3661,7 +3809,213 @@
             );
             assert_eq!(a.atom(spend.puzzle_hash), H2);
             assert_eq!(spend.agg_sig_me.len(), 0);
             assert!((spend.flags & ELIGIBLE_FOR_DEDUP) != 0);
         }
     }
 }
+
+#[cfg(test)]
+#[rstest]
+// the scale factor is 10000
+#[case("((90 (1 )", 10000)]
+// 0 is OK (but does it make sense?)
+#[case("((90 (0 )", 0)]
+// the cost accumulates
+#[case("((90 (1 ) ((90 (2 ) ((90 (3 )", (1 + 2 + 3) * 10000)]
+// the cost can be large
+#[case("((90 (10000 )", 100000000)]
+// the upper cost limit in the test is 11000000000
+#[case("((90 (1100000 )", 11000000000)]
+// additional arguments are ignored
+#[case("((90 (1 ( 42 ( 1337 )", 10000)]
+// reserved opcodes with fixed cost
+#[case("((256 )", 100)]
+#[case("((257 )", 106)]
+#[case("((258 )", 112)]
+#[case("((259 )", 119)]
+#[case("((260 )", 127)]
+#[case("((261 )", 135)]
+#[case("((262 )", 143)]
+#[case("((263 )", 152)]
+#[case("((264 )", 162)]
+#[case("((265 )", 172)]
+#[case("((266 )", 183)]
+#[case("((504 )", 338000000)]
+#[case("((505 )", 359000000)]
+#[case("((506 )", 382000000)]
+#[case("((507 )", 406000000)]
+#[case("((508 )", 431000000)]
+#[case("((509 )", 458000000)]
+#[case("((510 )", 487000000)]
+#[case("((511 )", 517000000)]
+#[case("((512 )", 100)]
+#[case("((513 )", 106)]
+#[case("((0xff00 )", 100)]
+#[case("((0xff01 )", 106)]
+fn test_softfork_condition(#[case] conditions: &str, #[case] expected_cost: Cost) {
+    // SOFTFORK (90)
+    let (_, spends) = cond_test_flag(
+        &format!("((({{h1}} ({{h2}} (1234 ({}))))", conditions),
+        ENABLE_SOFTFORK_CONDITION,
+    )
+    .unwrap();
+    assert_eq!(spends.cost, expected_cost);
+
+    // when NO_UNKNOWN_CONDS is enabled, any SOFTFORK condition is an error
+    // (because we don't know of any yet)
+    assert_eq!(
+        cond_test_flag(
+            &format!("((({{h1}} ({{h2}} (1234 ({}))))", conditions),
+            ENABLE_SOFTFORK_CONDITION | NO_UNKNOWN_CONDS
+        )
+        .unwrap_err()
+        .1,
+        ErrorCode::InvalidConditionOpcode
+    );
+
+    // if softfork conditions aren't enabled, they are just plain unknown
+    // conditions (that don't incur a cost
+    let (_, spends) =
+        cond_test_flag(&format!("((({{h1}} ({{h2}} (1234 ({}))))", conditions), 0).unwrap();
+    assert_eq!(spends.cost, 0);
+
+    // if softfork conditions aren't enabled, but we don't allow unknown
+    // conditions (mempool mode) they fail
+    assert_eq!(
+        cond_test_flag(
+            &format!("((({{h1}} ({{h2}} (1234 ({}))))", conditions),
+            NO_UNKNOWN_CONDS
+        )
+        .unwrap_err()
+        .1,
+        ErrorCode::InvalidConditionOpcode
+    );
+}
+
+#[cfg(test)]
+#[rstest]
+// the cost argument must be positive
+#[case("((90 (-1 )", ErrorCode::InvalidSoftforkCost)]
+// the cost argument may not exceed 2^32-1
+#[case("((90 (0x0100000000 )", ErrorCode::InvalidSoftforkCost)]
+// the test has a cost limit of 11000000000
+#[case("((90 (0x00ffffffff )", ErrorCode::CostExceeded)]
+#[case("((90 )", ErrorCode::InvalidCondition)]
+fn test_softfork_condition_failures(#[case] conditions: &str, #[case] expected_err: ErrorCode) {
+    // SOFTFORK (90)
+    assert_eq!(
+        cond_test_flag(
+            &format!("((({{h1}} ({{h2}} (1234 ({}))))", conditions),
+            ENABLE_SOFTFORK_CONDITION
+        )
+        .unwrap_err()
+        .1,
+        expected_err
+    );
+}
+
+#[cfg(test)]
+#[rstest]
+#[case(CREATE_PUZZLE_ANNOUNCEMENT, 1000, LIMIT_ANNOUNCES, None)]
+#[case(
+    CREATE_PUZZLE_ANNOUNCEMENT,
+    1025,
+    LIMIT_ANNOUNCES,
+    Some(ErrorCode::TooManyAnnouncements)
+)]
+#[case(
+    ASSERT_PUZZLE_ANNOUNCEMENT,
+    1024,
+    LIMIT_ANNOUNCES,
+    Some(ErrorCode::AssertPuzzleAnnouncementFailed)
+)]
+#[case(
+    ASSERT_PUZZLE_ANNOUNCEMENT,
+    1025,
+    LIMIT_ANNOUNCES,
+    Some(ErrorCode::TooManyAnnouncements)
+)]
+#[case(CREATE_COIN_ANNOUNCEMENT, 1000, LIMIT_ANNOUNCES, None)]
+#[case(
+    CREATE_COIN_ANNOUNCEMENT,
+    1025,
+    LIMIT_ANNOUNCES,
+    Some(ErrorCode::TooManyAnnouncements)
+)]
+#[case(
+    ASSERT_COIN_ANNOUNCEMENT,
+    1024,
+    LIMIT_ANNOUNCES,
+    Some(ErrorCode::AssertCoinAnnouncementFailed)
+)]
+#[case(
+    ASSERT_COIN_ANNOUNCEMENT,
+    1025,
+    LIMIT_ANNOUNCES,
+    Some(ErrorCode::TooManyAnnouncements)
+)]
+#[case(ASSERT_CONCURRENT_SPEND, 1024, ENABLE_ASSERT_BEFORE | LIMIT_ANNOUNCES, Some(ErrorCode::AssertConcurrentSpendFailed))]
+#[case(ASSERT_CONCURRENT_SPEND, 1025, ENABLE_ASSERT_BEFORE | LIMIT_ANNOUNCES, Some(ErrorCode::TooManyAnnouncements))]
+#[case(ASSERT_CONCURRENT_PUZZLE, 1024, ENABLE_ASSERT_BEFORE | LIMIT_ANNOUNCES, Some(ErrorCode::AssertConcurrentPuzzleFailed))]
+#[case(ASSERT_CONCURRENT_PUZZLE, 1025, ENABLE_ASSERT_BEFORE | LIMIT_ANNOUNCES, Some(ErrorCode::TooManyAnnouncements))]
+#[case(CREATE_PUZZLE_ANNOUNCEMENT, 1025, 0, None)]
+#[case(
+    ASSERT_PUZZLE_ANNOUNCEMENT,
+    1025,
+    0,
+    Some(ErrorCode::AssertPuzzleAnnouncementFailed)
+)]
+#[case(CREATE_COIN_ANNOUNCEMENT, 1025, 0, None)]
+#[case(
+    ASSERT_COIN_ANNOUNCEMENT,
+    1025,
+    0,
+    Some(ErrorCode::AssertCoinAnnouncementFailed)
+)]
+#[case(
+    ASSERT_CONCURRENT_SPEND,
+    1025,
+    ENABLE_ASSERT_BEFORE,
+    Some(ErrorCode::AssertConcurrentSpendFailed)
+)]
+#[case(
+    ASSERT_CONCURRENT_PUZZLE,
+    1025,
+    ENABLE_ASSERT_BEFORE,
+    Some(ErrorCode::AssertConcurrentPuzzleFailed)
+)]
+fn test_limit_announcements(
+    #[case] cond: ConditionOpcode,
+    #[case] count: i32,
+    #[case] flags: u32,
+    #[case] expect_err: Option<ErrorCode>,
+) {
+    let r = cond_test_cb(
+        "((({h1} ({h1} (123 ({} )))",
+        flags,
+        Some(Box::new(move |a: &mut Allocator| -> NodePtr {
+            let mut rest: NodePtr = a.null();
+
+            // generate a lot of announcements
+            for _ in 0..count {
+                // this builds one condition
+                // borrow-rules prevent this from being succint
+                let ann = a.null();
+                let val = a.new_atom(H2).unwrap();
+                let ann = a.new_pair(val, ann).unwrap();
+                let val = a.new_atom(&u64_to_bytes(cond as u64)).unwrap();
+                let ann = a.new_pair(val, ann).unwrap();
+
+                // add the condition to the list
+                rest = a.new_pair(ann, rest).unwrap();
+            }
+            rest
+        })),
+    );
+
+    if expect_err.is_some() {
+        assert_eq!(r.unwrap_err().1, expect_err.unwrap());
+    } else {
+        r.unwrap();
+    }
+}
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia/src/gen/get_puzzle_and_solution.rs` & `chia_rs-0.2.8/local_dependencies/chia/src/gen/get_puzzle_and_solution.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/src/gen/opcodes.rs` & `chia_rs-0.2.8/local_dependencies/chia/src/gen/opcodes.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use crate::gen::flags::ENABLE_ASSERT_BEFORE;
+use crate::gen::flags::ENABLE_SOFTFORK_CONDITION;
 use clvmr::allocator::{Allocator, NodePtr, SExp};
 use clvmr::cost::Cost;
 
-pub type ConditionOpcode = u8;
+pub type ConditionOpcode = u16;
 
 // AGG_SIG is ascii "1"
 pub const AGG_SIG_UNSAFE: ConditionOpcode = 49;
 pub const AGG_SIG_ME: ConditionOpcode = 50;
 
 // the conditions below reserve coin amounts and have to be accounted for in
 // output totals
@@ -44,124 +45,211 @@
 pub const ASSERT_BEFORE_SECONDS_ABSOLUTE: ConditionOpcode = 85;
 
 // spend is not valid if block height exceeds the specified height
 pub const ASSERT_BEFORE_HEIGHT_RELATIVE: ConditionOpcode = 86;
 pub const ASSERT_BEFORE_HEIGHT_ABSOLUTE: ConditionOpcode = 87;
 
 // no-op condition
-pub const ALWAYS_TRUE: ConditionOpcode = 1;
+pub const REMARK: ConditionOpcode = 1;
+
+// takes its cost as the first parameter, followed by future extensions
+// the cost is specified in increments of 10000, to keep the values smaller
+// This is a hard fork and is therefore only available when enabled by the
+// ENABLE_SOFTFORK_CONDITION flag
+pub const SOFTFORK: ConditionOpcode = 90;
 
 pub const CREATE_COIN_COST: Cost = 1800000;
 pub const AGG_SIG_COST: Cost = 1200000;
 
+// when ENABLE_SOFTFORK_CONDITION is enabled
+// 2-byte condition opcodes have costs according to this table:
+
+// the values `100 * (17 ** idx)/(16 ** idx)` rounded to three significant decimal figures
+
+const fn calculate_cost_table() -> [u64; 256] {
+    let (a, b) = (17, 16);
+    let mut s = [0; 256];
+    let (mut num, mut den) = (100_u64, 1_u64);
+    let max = 1 << 59;
+    let mut idx = 0;
+    while idx < 256 {
+        let v = num / den;
+        let mut power_of_ten = 1000;
+        while power_of_ten < v {
+            power_of_ten *= 10;
+        }
+        power_of_ten /= 1000;
+        s[idx] = (v / power_of_ten) * power_of_ten;
+        num *= a;
+        den *= b;
+        while num > max {
+            num >>= 5;
+            den >>= 5;
+        }
+        idx += 1;
+    }
+    s
+}
+
+const COSTS: [Cost; 256] = calculate_cost_table();
+
+pub fn compute_unknown_condition_cost(op: ConditionOpcode) -> Cost {
+    if op < 256 {
+        0
+    } else {
+        COSTS[(op & 0xff) as usize]
+    }
+}
+
 pub fn parse_opcode(a: &Allocator, op: NodePtr, flags: u32) -> Option<ConditionOpcode> {
     let buf = match a.sexp(op) {
-        SExp::Atom(_) => a.atom(op),
+        SExp::Atom() => a.atom(op),
         _ => return None,
     };
-    if buf.len() != 1 {
-        return None;
-    }
-
-    match buf[0] {
-        AGG_SIG_UNSAFE
-        | AGG_SIG_ME
-        | CREATE_COIN
-        | RESERVE_FEE
-        | CREATE_COIN_ANNOUNCEMENT
-        | ASSERT_COIN_ANNOUNCEMENT
-        | CREATE_PUZZLE_ANNOUNCEMENT
-        | ASSERT_PUZZLE_ANNOUNCEMENT
-        | ASSERT_MY_COIN_ID
-        | ASSERT_MY_PARENT_ID
-        | ASSERT_MY_PUZZLEHASH
-        | ASSERT_MY_AMOUNT
-        | ASSERT_SECONDS_RELATIVE
-        | ASSERT_SECONDS_ABSOLUTE
-        | ASSERT_HEIGHT_RELATIVE
-        | ASSERT_HEIGHT_ABSOLUTE
-        | ALWAYS_TRUE => Some(buf[0]),
-        _ => {
-            if (flags & ENABLE_ASSERT_BEFORE) != 0 {
-                match buf[0] {
-                    ASSERT_BEFORE_SECONDS_RELATIVE
-                    | ASSERT_BEFORE_SECONDS_ABSOLUTE
-                    | ASSERT_BEFORE_HEIGHT_RELATIVE
-                    | ASSERT_BEFORE_HEIGHT_ABSOLUTE
-                    | ASSERT_CONCURRENT_SPEND
-                    | ASSERT_CONCURRENT_PUZZLE
-                    | ASSERT_MY_BIRTH_SECONDS
-                    | ASSERT_MY_BIRTH_HEIGHT
-                    | ASSERT_EPHEMERAL => Some(buf[0]),
-                    _ => None,
+    if buf.len() == 2 && (flags & ENABLE_SOFTFORK_CONDITION) != 0 {
+        if buf[0] == 0 {
+            // no redundant leading zeroes
+            None
+        } else {
+            // These are 2-byte condition codes whose first byte is 1
+            Some(ConditionOpcode::from_be_bytes(buf.try_into().unwrap()))
+        }
+    } else if buf.len() == 1 {
+        let b0 = buf[0] as ConditionOpcode;
+        match b0 {
+            AGG_SIG_UNSAFE
+            | AGG_SIG_ME
+            | CREATE_COIN
+            | RESERVE_FEE
+            | CREATE_COIN_ANNOUNCEMENT
+            | ASSERT_COIN_ANNOUNCEMENT
+            | CREATE_PUZZLE_ANNOUNCEMENT
+            | ASSERT_PUZZLE_ANNOUNCEMENT
+            | ASSERT_MY_COIN_ID
+            | ASSERT_MY_PARENT_ID
+            | ASSERT_MY_PUZZLEHASH
+            | ASSERT_MY_AMOUNT
+            | ASSERT_SECONDS_RELATIVE
+            | ASSERT_SECONDS_ABSOLUTE
+            | ASSERT_HEIGHT_RELATIVE
+            | ASSERT_HEIGHT_ABSOLUTE
+            | REMARK => Some(b0),
+            _ => {
+                if (flags & ENABLE_SOFTFORK_CONDITION) != 0 && b0 == SOFTFORK {
+                    Some(b0)
+                } else if (flags & ENABLE_ASSERT_BEFORE) != 0 {
+                    match b0 {
+                        ASSERT_BEFORE_SECONDS_RELATIVE
+                        | ASSERT_BEFORE_SECONDS_ABSOLUTE
+                        | ASSERT_BEFORE_HEIGHT_RELATIVE
+                        | ASSERT_BEFORE_HEIGHT_ABSOLUTE
+                        | ASSERT_CONCURRENT_SPEND
+                        | ASSERT_CONCURRENT_PUZZLE
+                        | ASSERT_MY_BIRTH_SECONDS
+                        | ASSERT_MY_BIRTH_HEIGHT
+                        | ASSERT_EPHEMERAL => Some(b0),
+                        _ => None,
+                    }
+                } else {
+                    None
                 }
-            } else {
-                None
             }
         }
+    } else {
+        None
     }
 }
 
 #[cfg(test)]
-fn opcode_tester(a: &mut Allocator, val: &[u8]) -> Option<ConditionOpcode> {
+fn opcode_tester(a: &mut Allocator, val: &[u8], flags: u32) -> Option<ConditionOpcode> {
     let v = a.new_atom(val).unwrap();
-    parse_opcode(&a, v, 0)
-}
-
-#[cfg(test)]
-fn opcode_tester_with_assert_before(a: &mut Allocator, val: &[u8]) -> Option<ConditionOpcode> {
-    let v = a.new_atom(val).unwrap();
-    parse_opcode(&a, v, ENABLE_ASSERT_BEFORE)
+    parse_opcode(&a, v, flags)
 }
 
 #[cfg(test)]
 use rstest::rstest;
 
 #[cfg(test)]
 #[rstest]
 // leading zeros are not allowed, it makes it a different value
-#[case(&[ASSERT_HEIGHT_ABSOLUTE, 0], None, None)]
-#[case(&[0, ASSERT_HEIGHT_ABSOLUTE], None, None)]
+#[case(&[ASSERT_HEIGHT_ABSOLUTE as u8, 0, 0], None, None)]
+#[case(&[0, ASSERT_HEIGHT_ABSOLUTE as u8], None, None)]
 #[case(&[0], None, None)]
 // all condition codes
-#[case(&[AGG_SIG_UNSAFE], Some(AGG_SIG_UNSAFE), Some(AGG_SIG_UNSAFE))]
-#[case(&[AGG_SIG_ME], Some(AGG_SIG_ME), Some(AGG_SIG_ME))]
-#[case(&[CREATE_COIN], Some(CREATE_COIN), Some(CREATE_COIN))]
-#[case(&[RESERVE_FEE], Some(RESERVE_FEE), Some(RESERVE_FEE))]
-#[case(&[CREATE_COIN_ANNOUNCEMENT], Some(CREATE_COIN_ANNOUNCEMENT), Some(CREATE_COIN_ANNOUNCEMENT))]
-#[case(&[ASSERT_COIN_ANNOUNCEMENT], Some(ASSERT_COIN_ANNOUNCEMENT), Some(ASSERT_COIN_ANNOUNCEMENT))]
-#[case(&[CREATE_PUZZLE_ANNOUNCEMENT], Some(CREATE_PUZZLE_ANNOUNCEMENT), Some(CREATE_PUZZLE_ANNOUNCEMENT))]
-#[case(&[ASSERT_PUZZLE_ANNOUNCEMENT], Some(ASSERT_PUZZLE_ANNOUNCEMENT), Some(ASSERT_PUZZLE_ANNOUNCEMENT))]
-#[case(&[ASSERT_CONCURRENT_SPEND], None, Some(ASSERT_CONCURRENT_SPEND))]
-#[case(&[ASSERT_CONCURRENT_PUZZLE], None, Some(ASSERT_CONCURRENT_PUZZLE))]
-#[case(&[ASSERT_MY_COIN_ID], Some(ASSERT_MY_COIN_ID), Some(ASSERT_MY_COIN_ID))]
-#[case(&[ASSERT_MY_PARENT_ID], Some(ASSERT_MY_PARENT_ID), Some(ASSERT_MY_PARENT_ID))]
-#[case(&[ASSERT_MY_PUZZLEHASH], Some(ASSERT_MY_PUZZLEHASH), Some(ASSERT_MY_PUZZLEHASH))]
-#[case(&[ASSERT_MY_AMOUNT], Some(ASSERT_MY_AMOUNT), Some(ASSERT_MY_AMOUNT))]
-#[case(&[ASSERT_MY_BIRTH_SECONDS], None, Some(ASSERT_MY_BIRTH_SECONDS))]
-#[case(&[ASSERT_MY_BIRTH_HEIGHT], None, Some(ASSERT_MY_BIRTH_HEIGHT))]
-#[case(&[ASSERT_EPHEMERAL], None, Some(ASSERT_EPHEMERAL))]
-#[case(&[ASSERT_SECONDS_RELATIVE],Some(ASSERT_SECONDS_RELATIVE) , Some(ASSERT_SECONDS_RELATIVE))]
-#[case(&[ASSERT_SECONDS_ABSOLUTE],Some(ASSERT_SECONDS_ABSOLUTE) , Some(ASSERT_SECONDS_ABSOLUTE))]
-#[case(&[ASSERT_HEIGHT_RELATIVE], Some(ASSERT_HEIGHT_RELATIVE), Some(ASSERT_HEIGHT_RELATIVE))]
-#[case(&[ASSERT_HEIGHT_ABSOLUTE], Some(ASSERT_HEIGHT_ABSOLUTE), Some(ASSERT_HEIGHT_ABSOLUTE))]
-#[case(&[ASSERT_BEFORE_SECONDS_RELATIVE], None, Some(ASSERT_BEFORE_SECONDS_RELATIVE))]
-#[case(&[ASSERT_BEFORE_SECONDS_ABSOLUTE], None, Some(ASSERT_BEFORE_SECONDS_ABSOLUTE))]
-#[case(&[ASSERT_BEFORE_HEIGHT_RELATIVE], None, Some(ASSERT_BEFORE_HEIGHT_RELATIVE))]
-#[case(&[ASSERT_BEFORE_HEIGHT_ABSOLUTE], None, Some(ASSERT_BEFORE_HEIGHT_ABSOLUTE))]
-#[case(&[ALWAYS_TRUE], Some(ALWAYS_TRUE), Some(ALWAYS_TRUE))]
-
+#[case(&[AGG_SIG_UNSAFE as u8], Some(AGG_SIG_UNSAFE), Some(AGG_SIG_UNSAFE))]
+#[case(&[AGG_SIG_ME as u8], Some(AGG_SIG_ME), Some(AGG_SIG_ME))]
+#[case(&[CREATE_COIN as u8], Some(CREATE_COIN), Some(CREATE_COIN))]
+#[case(&[RESERVE_FEE as u8], Some(RESERVE_FEE), Some(RESERVE_FEE))]
+#[case(&[CREATE_COIN_ANNOUNCEMENT as u8], Some(CREATE_COIN_ANNOUNCEMENT), Some(CREATE_COIN_ANNOUNCEMENT))]
+#[case(&[ASSERT_COIN_ANNOUNCEMENT as u8], Some(ASSERT_COIN_ANNOUNCEMENT), Some(ASSERT_COIN_ANNOUNCEMENT))]
+#[case(&[CREATE_PUZZLE_ANNOUNCEMENT as u8], Some(CREATE_PUZZLE_ANNOUNCEMENT), Some(CREATE_PUZZLE_ANNOUNCEMENT))]
+#[case(&[ASSERT_PUZZLE_ANNOUNCEMENT as u8], Some(ASSERT_PUZZLE_ANNOUNCEMENT), Some(ASSERT_PUZZLE_ANNOUNCEMENT))]
+#[case(&[ASSERT_CONCURRENT_SPEND as u8], None, Some(ASSERT_CONCURRENT_SPEND))]
+#[case(&[ASSERT_CONCURRENT_PUZZLE as u8], None, Some(ASSERT_CONCURRENT_PUZZLE))]
+#[case(&[ASSERT_MY_COIN_ID as u8], Some(ASSERT_MY_COIN_ID), Some(ASSERT_MY_COIN_ID))]
+#[case(&[ASSERT_MY_PARENT_ID as u8], Some(ASSERT_MY_PARENT_ID), Some(ASSERT_MY_PARENT_ID))]
+#[case(&[ASSERT_MY_PUZZLEHASH as u8], Some(ASSERT_MY_PUZZLEHASH), Some(ASSERT_MY_PUZZLEHASH))]
+#[case(&[ASSERT_MY_AMOUNT as u8], Some(ASSERT_MY_AMOUNT), Some(ASSERT_MY_AMOUNT))]
+#[case(&[ASSERT_MY_BIRTH_SECONDS as u8], None, Some(ASSERT_MY_BIRTH_SECONDS))]
+#[case(&[ASSERT_MY_BIRTH_HEIGHT as u8], None, Some(ASSERT_MY_BIRTH_HEIGHT))]
+#[case(&[ASSERT_EPHEMERAL as u8], None, Some(ASSERT_EPHEMERAL))]
+#[case(&[ASSERT_SECONDS_RELATIVE as u8],Some(ASSERT_SECONDS_RELATIVE) , Some(ASSERT_SECONDS_RELATIVE))]
+#[case(&[ASSERT_SECONDS_ABSOLUTE as u8],Some(ASSERT_SECONDS_ABSOLUTE) , Some(ASSERT_SECONDS_ABSOLUTE))]
+#[case(&[ASSERT_HEIGHT_RELATIVE as u8], Some(ASSERT_HEIGHT_RELATIVE), Some(ASSERT_HEIGHT_RELATIVE))]
+#[case(&[ASSERT_HEIGHT_ABSOLUTE as u8], Some(ASSERT_HEIGHT_ABSOLUTE), Some(ASSERT_HEIGHT_ABSOLUTE))]
+#[case(&[ASSERT_BEFORE_SECONDS_RELATIVE as u8], None, Some(ASSERT_BEFORE_SECONDS_RELATIVE))]
+#[case(&[ASSERT_BEFORE_SECONDS_ABSOLUTE as u8], None, Some(ASSERT_BEFORE_SECONDS_ABSOLUTE))]
+#[case(&[ASSERT_BEFORE_HEIGHT_RELATIVE as u8], None, Some(ASSERT_BEFORE_HEIGHT_RELATIVE))]
+#[case(&[ASSERT_BEFORE_HEIGHT_ABSOLUTE as u8], None, Some(ASSERT_BEFORE_HEIGHT_ABSOLUTE))]
+#[case(&[REMARK as u8], Some(REMARK), Some(REMARK))]
 fn test_parse_opcode(
     #[case] input: &[u8],
     #[case] expected: Option<ConditionOpcode>,
     #[case] expected2: Option<ConditionOpcode>,
 ) {
     let mut a = Allocator::new();
-    assert_eq!(opcode_tester(&mut a, input), expected);
-    assert_eq!(opcode_tester_with_assert_before(&mut a, input), expected2);
+    assert_eq!(opcode_tester(&mut a, input, 0), expected);
+    assert_eq!(
+        opcode_tester(&mut a, input, ENABLE_ASSERT_BEFORE),
+        expected2
+    );
+    assert_eq!(
+        opcode_tester(&mut a, input, ENABLE_SOFTFORK_CONDITION),
+        expected
+    );
+    assert_eq!(
+        opcode_tester(
+            &mut a,
+            input,
+            ENABLE_ASSERT_BEFORE | ENABLE_SOFTFORK_CONDITION
+        ),
+        expected2
+    );
+}
+
+#[cfg(test)]
+#[rstest]
+#[case(&[AGG_SIG_UNSAFE as u8], Some(AGG_SIG_UNSAFE), Some(AGG_SIG_UNSAFE))]
+#[case(&[AGG_SIG_ME as u8], Some(AGG_SIG_ME), Some(AGG_SIG_ME))]
+#[case(&[CREATE_COIN as u8], Some(CREATE_COIN), Some(CREATE_COIN))]
+// the SOFTOFORK condition is only recognized when the flag is set
+#[case(&[SOFTFORK as u8], None, Some(SOFTFORK))]
+#[case(&[ASSERT_EPHEMERAL as u8], None, None)]
+#[case(&[ASSERT_BEFORE_SECONDS_RELATIVE as u8], None, None)]
+fn test_parse_opcode_softfork(
+    #[case] input: &[u8],
+    #[case] expected: Option<ConditionOpcode>,
+    #[case] expected2: Option<ConditionOpcode>,
+) {
+    let mut a = Allocator::new();
+    assert_eq!(opcode_tester(&mut a, input, 0), expected);
+    assert_eq!(
+        opcode_tester(&mut a, input, ENABLE_SOFTFORK_CONDITION),
+        expected2
+    );
 }
 
 #[test]
 fn test_parse_invalid_opcode() {
     // a pair is never a valid condition
     let mut a = Allocator::new();
     let v1 = a.new_atom(&[0]).unwrap();
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia/src/gen/run_block_generator.rs` & `chia_rs-0.2.8/local_dependencies/chia/src/gen/run_block_generator.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 use crate::gen::conditions::{parse_spends, SpendBundleConditions};
+use crate::gen::flags::ALLOW_BACKREFS;
 use crate::gen::validation_error::{ErrorCode, ValidationErr};
 use crate::generator_rom::{COST_PER_BYTE, GENERATOR_ROM};
 use clvmr::allocator::Allocator;
 use clvmr::chia_dialect::ChiaDialect;
 use clvmr::reduction::Reduction;
 use clvmr::run_program::run_program;
-use clvmr::serde::node_from_bytes;
+use clvmr::serde::{node_from_bytes, node_from_bytes_backrefs};
 
 // Runs the generator ROM and passes in the program (transactions generator).
 // The program is expected to return a list of spends. Each item being:
 
 // (parent-coin-id puzzle-reveal amount solution)
 
 // The puzzle-reveals are then executed with the corresponding solution being
@@ -31,15 +32,19 @@
     let byte_cost = program.len() as u64 * COST_PER_BYTE;
 
     if byte_cost >= max_cost {
         return Err(ValidationErr(a.null(), ErrorCode::CostExceeded));
     }
 
     let generator_rom = node_from_bytes(a, &GENERATOR_ROM)?;
-    let program = node_from_bytes(a, program)?;
+    let program = if (flags & ALLOW_BACKREFS) != 0 {
+        node_from_bytes_backrefs(a, program)?
+    } else {
+        node_from_bytes(a, program)?
+    };
 
     // iterate in reverse order since we're building a linked list from
     // the tail
     let mut args = a.null();
     for g in block_refs.iter().rev() {
         let ref_gen = a.new_atom(g.as_ref())?;
         args = a.new_pair(ref_gen, args)?;
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia/src/gen/run_puzzle.rs` & `chia_rs-0.2.8/local_dependencies/chia/src/gen/run_puzzle.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 use crate::gen::conditions::{
     parse_conditions, ParseState, Spend, SpendBundleConditions, ELIGIBLE_FOR_DEDUP,
 };
+use crate::gen::flags::ALLOW_BACKREFS;
 use crate::gen::validation_error::ValidationErr;
 use chia_protocol::bytes::Bytes32;
 use chia_protocol::coin::Coin;
 use clvm_utils::tree_hash::tree_hash;
 use clvmr::allocator::Allocator;
 use clvmr::chia_dialect::ChiaDialect;
 use clvmr::reduction::Reduction;
 use clvmr::run_program::run_program;
-use clvmr::serde::node_from_bytes;
+use clvmr::serde::{node_from_bytes, node_from_bytes_backrefs};
 use std::collections::HashSet;
 use std::sync::Arc;
 
 pub fn run_puzzle(
     a: &mut Allocator,
     puzzle: &[u8],
     solution: &[u8],
     parent_id: &[u8],
     amount: u64,
     max_cost: u64,
     flags: u32,
 ) -> Result<SpendBundleConditions, ValidationErr> {
-    let puzzle = node_from_bytes(a, puzzle)?;
-    let solution = node_from_bytes(a, solution)?;
+    let deserialize = if (flags & ALLOW_BACKREFS) != 0 {
+        node_from_bytes_backrefs
+    } else {
+        node_from_bytes
+    };
+    let puzzle = deserialize(a, puzzle)?;
+    let solution = deserialize(a, solution)?;
 
     let dialect = ChiaDialect::new(flags);
     let Reduction(clvm_cost, conditions) = run_program(a, &dialect, puzzle, solution, max_cost)?;
 
     let mut ret = SpendBundleConditions {
         removal_amount: amount as u128,
         ..Default::default()
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia/src/gen/sanitize_int.rs` & `chia_rs-0.2.8/local_dependencies/chia/src/gen/sanitize_int.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/src/gen/validation_error.rs` & `chia_rs-0.2.8/local_dependencies/chia/src/gen/validation_error.rs`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,17 @@
     MintingCoin,
     ImpossibleSecondsRelativeConstraints,
     ImpossibleSecondsAbsoluteConstraints,
     ImpossibleHeightRelativeConstraints,
     ImpossibleHeightAbsoluteConstraints,
     AssertEphemeralFailed,
     EphemeralRelativeCondition,
+    InvalidSoftforkCondition,
+    InvalidSoftforkCost,
+    TooManyAnnouncements,
 }
 
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
 pub struct ValidationErr(pub NodePtr, pub ErrorCode);
 
 impl From<EvalErr> for ValidationErr {
     fn from(v: EvalErr) -> Self {
@@ -122,42 +125,45 @@
             ErrorCode::ImpossibleSecondsAbsoluteConstraints => 135,
             ErrorCode::ImpossibleHeightRelativeConstraints => 136,
             ErrorCode::ImpossibleHeightAbsoluteConstraints => 137,
             ErrorCode::AssertMyBirthSecondsFailed => 138,
             ErrorCode::AssertMyBirthHeightFailed => 139,
             ErrorCode::AssertEphemeralFailed => 140,
             ErrorCode::EphemeralRelativeCondition => 141,
+            ErrorCode::InvalidSoftforkCondition => 142,
+            ErrorCode::InvalidSoftforkCost => 143,
+            ErrorCode::TooManyAnnouncements => 144,
         }
     }
 }
 
 pub fn rest(a: &Allocator, n: NodePtr) -> Result<NodePtr, ValidationErr> {
     match a.sexp(n) {
         SExp::Pair(_, right) => Ok(right),
         _ => Err(ValidationErr(n, ErrorCode::InvalidCondition)),
     }
 }
 
 pub fn next(a: &Allocator, n: NodePtr) -> Result<Option<(NodePtr, NodePtr)>, ValidationErr> {
     match a.sexp(n) {
         SExp::Pair(left, right) => Ok(Some((left, right))),
-        SExp::Atom(v) => {
+        SExp::Atom() => {
             // this is expected to be a valid list terminator
-            if v.is_empty() {
+            if a.atom_len(n) == 0 {
                 Ok(None)
             } else {
                 Err(ValidationErr(n, ErrorCode::InvalidCondition))
             }
         }
     }
 }
 
 pub fn atom(a: &Allocator, n: NodePtr, code: ErrorCode) -> Result<&[u8], ValidationErr> {
     match a.sexp(n) {
-        SExp::Atom(_) => Ok(a.atom(n)),
+        SExp::Atom() => Ok(a.atom(n)),
         _ => Err(ValidationErr(n, code)),
     }
 }
 
 pub fn check_nil(a: &Allocator, n: NodePtr) -> Result<(), ValidationErr> {
     if atom(a, n, ErrorCode::InvalidCondition)?.is_empty() {
         Ok(())
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia/src/merkle_set.rs` & `chia_rs-0.2.8/local_dependencies/chia/src/merkle_set.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/tests/generate-programs.py` & `chia_rs-0.2.8/local_dependencies/chia/tests/generate-programs.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/tests/generators/block-834752.hex` & `chia_rs-0.2.8/local_dependencies/chia/generator-tests/block-834752.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1 +1,26 @@
 ff01ffffffa022cf3c17be4e0e0e0b2e2a3f6dd1ee955528f737f0cb724247bc2e4a776cb989ffff02ffff01ff02ffff01ff02ffff03ffff18ff2fffff010180ffff01ff02ff36ffff04ff02ffff04ff05ffff04ff17ffff04ffff02ff26ffff04ff02ffff04ff0bff80808080ffff04ff2fffff04ff0bffff04ff5fff808080808080808080ffff01ff088080ff0180ffff04ffff01ffffffff4602ff3304ffff0101ff02ffff02ffff03ff05ffff01ff02ff5cffff04ff02ffff04ff0dffff04ffff0bff2cffff0bff24ff3880ffff0bff2cffff0bff2cffff0bff24ff3480ff0980ffff0bff2cff0bffff0bff24ff8080808080ff8080808080ffff010b80ff0180ff02ffff03ff0bffff01ff02ff32ffff04ff02ffff04ff05ffff04ff0bffff04ff17ffff04ffff02ff2affff04ff02ffff04ffff02ffff03ffff09ff23ff2880ffff0181b3ff8080ff0180ff80808080ff80808080808080ffff01ff02ffff03ff17ff80ffff01ff088080ff018080ff0180ffffffff0bffff0bff17ffff02ff3affff04ff02ffff04ff09ffff04ff2fffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ff5f80ff0bff81bf80ff02ffff03ffff20ffff22ff4fff178080ffff01ff02ff7effff04ff02ffff04ff6fffff04ffff04ffff02ffff03ff4fffff01ff04ff23ffff04ffff02ff3affff04ff02ffff04ff09ffff04ff53ffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ffff04ff81b3ff80808080ffff011380ff0180ffff02ff7cffff04ff02ffff04ff05ffff04ff1bffff04ffff21ff4fff1780ff80808080808080ff8080808080ffff01ff088080ff0180ffff04ffff09ffff18ff05ffff010180ffff010180ffff09ff05ffff01818f8080ff0bff2cffff0bff24ff3080ffff0bff2cffff0bff2cffff0bff24ff3480ff0580ffff0bff2cffff02ff5cffff04ff02ffff04ff07ffff04ffff0bff24ff2480ff8080808080ffff0bff24ff8080808080ffffff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff26ffff04ff02ffff04ff09ff80808080ffff02ff26ffff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff02ff5effff04ff02ffff04ff05ffff04ff0bffff04ffff02ff3affff04ff02ffff04ff09ffff04ff17ffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ffff04ff17ffff04ff2fffff04ff5fffff04ff81bfff80808080808080808080ffff04ffff04ff20ffff04ff17ff808080ffff02ff7cffff04ff02ffff04ff05ffff04ffff02ff82017fffff04ffff04ffff04ff17ff2f80ffff04ffff04ff5fff81bf80ffff04ff0bff05808080ff8202ff8080ffff01ff80808080808080ffff02ff2effff04ff02ffff04ff05ffff04ff0bffff04ffff02ffff03ff3bffff01ff02ff22ffff04ff02ffff04ff05ffff04ff17ffff04ff13ffff04ff2bffff04ff5bffff04ff5fff808080808080808080ffff01ff02ffff03ffff09ff15ffff0bff13ff1dff2b8080ffff01ff0bff15ff17ff5f80ffff01ff088080ff018080ff0180ffff04ff17ffff04ff2fffff04ff5fffff04ff81bfffff04ff82017fff8080808080808080808080ff02ffff03ff05ffff011bffff010b80ff0180ff018080ffff04ffff01ffa024e044101e57b3d8c908b8a38ad57848afd29d3eecc439dba45f4412df4954fdffa0f08eda9271f9dd1c00d9789ba0f3e4f547d66c8ad6f75edbb587b8c68d8ef5f1a0eff07522495060c066f66f32acc2a77e3a3e737aca8baea4d1a64ea4cdc13da9ffff04ffff01ff02ffff01ff02ffff01ff02ffff03ff8202ffffff01ff02ff16ffff04ff02ffff04ff05ffff04ff8204bfffff04ff8206bfffff04ff82017fffff04ffff0bffff19ff2fffff18ffff019100ffffffffffffffffffffffffffffffffff8202ff8080ff0bff82017f80ff8080808080808080ffff01ff04ffff04ff08ffff04ff17ffff04ffff02ff1effff04ff02ffff04ff82017fff80808080ff80808080ffff04ffff04ff1cffff04ff5fffff04ff8206bfff80808080ff80808080ff0180ffff04ffff01ffff32ff3d33ff3effff04ffff04ff1cffff04ff0bffff04ff17ff80808080ffff04ffff04ff1cffff04ff05ffff04ff2fff80808080ffff04ffff04ff0affff04ff5fff808080ffff04ffff04ff14ffff04ffff0bff5fffff012480ff808080ff8080808080ff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff1effff04ff02ffff04ff09ff80808080ffff02ff1effff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff018080ffff04ffff01a02f2c9ba1b2315d413a92b5f034fa03282ccba1767fd9ae7b14d942b969ed5d57ffff04ffff01a0c4a8fb8a651c5e8636c6dd67ed8c8f7a70f516f41ab73abd14dd79c7582f079affff04ffff01b08116639d853ecd6109277a9d83d3acc7e53a18d3524262ec9b99df923d22a390cbf0f632bced556dd9886bbf53f444b6ffff04ffff01a0ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000ffff04ffff01a022c0df3c66541eb57c226e12742a9f7182ceb0318cdaf5a84facb6c80bfaac1aff01808080808080ff01808080ff01ffffffa01daef44c653c413eba01d89790edfb613cb020ed0979d8447d6ed398327d0958ffa0976299e4fbb74e8732ae1ea7092ab617af435218f20912f99689d8fc69d12318ff0180ff01ffffffff70c07101022f2c9ba1b2315d413a92b5f034fa03282ccba1767fd9ae7b14d942b969ed5d578116639d853ecd6109277a9d83d3acc7e53a18d3524262ec9b99df923d22a390cbf0f632bced556dd9886bbf53f444b6010000001668747470733a2f2f6575312e706f6f6c2e73706163650000004080ff80808080ffffa0e8058c610f8f50e5e603ad136f58ff3b1f0120a76bb4985553db8bda88738ca9ffff02ffff01ff02ffff01ff02ffff03ffff18ff2fffff010180ffff01ff02ff36ffff04ff02ffff04ff05ffff04ff17ffff04ffff02ff26ffff04ff02ffff04ff0bff80808080ffff04ff2fffff04ff0bffff04ff5fff808080808080808080ffff01ff088080ff0180ffff04ffff01ffffffff4602ff3304ffff0101ff02ffff02ffff03ff05ffff01ff02ff5cffff04ff02ffff04ff0dffff04ffff0bff2cffff0bff24ff3880ffff0bff2cffff0bff2cffff0bff24ff3480ff0980ffff0bff2cff0bffff0bff24ff8080808080ff8080808080ffff010b80ff0180ff02ffff03ff0bffff01ff02ff32ffff04ff02ffff04ff05ffff04ff0bffff04ff17ffff04ffff02ff2affff04ff02ffff04ffff02ffff03ffff09ff23ff2880ffff0181b3ff8080ff0180ff80808080ff80808080808080ffff01ff02ffff03ff17ff80ffff01ff088080ff018080ff0180ffffffff0bffff0bff17ffff02ff3affff04ff02ffff04ff09ffff04ff2fffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ff5f80ff0bff81bf80ff02ffff03ffff20ffff22ff4fff178080ffff01ff02ff7effff04ff02ffff04ff6fffff04ffff04ffff02ffff03ff4fffff01ff04ff23ffff04ffff02ff3affff04ff02ffff04ff09ffff04ff53ffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ffff04ff81b3ff80808080ffff011380ff0180ffff02ff7cffff04ff02ffff04ff05ffff04ff1bffff04ffff21ff4fff1780ff80808080808080ff8080808080ffff01ff088080ff0180ffff04ffff09ffff18ff05ffff010180ffff010180ffff09ff05ffff01818f8080ff0bff2cffff0bff24ff3080ffff0bff2cffff0bff2cffff0bff24ff3480ff0580ffff0bff2cffff02ff5cffff04ff02ffff04ff07ffff04ffff0bff24ff2480ff8080808080ffff0bff24ff8080808080ffffff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff26ffff04ff02ffff04ff09ff80808080ffff02ff26ffff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff02ff5effff04ff02ffff04ff05ffff04ff0bffff04ffff02ff3affff04ff02ffff04ff09ffff04ff17ffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ffff04ff17ffff04ff2fffff04ff5fffff04ff81bfff80808080808080808080ffff04ffff04ff20ffff04ff17ff808080ffff02ff7cffff04ff02ffff04ff05ffff04ffff02ff82017fffff04ffff04ffff04ff17ff2f80ffff04ffff04ff5fff81bf80ffff04ff0bff05808080ff8202ff8080ffff01ff80808080808080ffff02ff2effff04ff02ffff04ff05ffff04ff0bffff04ffff02ffff03ff3bffff01ff02ff22ffff04ff02ffff04ff05ffff04ff17ffff04ff13ffff04ff2bffff04ff5bffff04ff5fff808080808080808080ffff01ff02ffff03ffff09ff15ffff0bff13ff1dff2b8080ffff01ff0bff15ff17ff5f80ffff01ff088080ff018080ff0180ffff04ff17ffff04ff2fffff04ff5fffff04ff81bfffff04ff82017fff8080808080808080808080ff02ffff03ff05ffff011bffff010b80ff0180ff018080ffff04ffff01ffa024e044101e57b3d8c908b8a38ad57848afd29d3eecc439dba45f4412df4954fdffa0df84418c7ba1b1a847fa23bd1101fcee22b2bd81c69d10e6d4b280f09eba2c70a0eff07522495060c066f66f32acc2a77e3a3e737aca8baea4d1a64ea4cdc13da9ffff04ffff01ff02ffff01ff02ffff01ff02ffff03ff8202ffffff01ff02ff16ffff04ff02ffff04ff05ffff04ff8204bfffff04ff8206bfffff04ff82017fffff04ffff0bffff19ff2fffff18ffff019100ffffffffffffffffffffffffffffffffff8202ff8080ff0bff82017f80ff8080808080808080ffff01ff04ffff04ff08ffff04ff17ffff04ffff02ff1effff04ff02ffff04ff82017fff80808080ff80808080ffff04ffff04ff1cffff04ff5fffff04ff8206bfff80808080ff80808080ff0180ffff04ffff01ffff32ff3d33ff3effff04ffff04ff1cffff04ff0bffff04ff17ff80808080ffff04ffff04ff1cffff04ff05ffff04ff2fff80808080ffff04ffff04ff0affff04ff5fff808080ffff04ffff04ff14ffff04ffff0bff5fffff012480ff808080ff8080808080ff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff1effff04ff02ffff04ff09ff80808080ffff02ff1effff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff018080ffff04ffff01a02f2c9ba1b2315d413a92b5f034fa03282ccba1767fd9ae7b14d942b969ed5d57ffff04ffff01a09c117e3fba164415fb868361a5c6d9c8a4551c71e5a359807cb27810b80f23bdffff04ffff01b08a505367d099210c24f1be8945a83de7db6d9396a9742c8f609aebf7ba56bbaacb038819b122741211bbc9227c903573ffff04ffff01a0ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000ffff04ffff01a0a78f9cbed5f7e1b529aa32088dcc3c53ac1df57bd0c8f4773f4c0ddae048a8edff01808080808080ff01808080ff01ffffffa0245c7e4ad426a2a6b6eb5622286d2fd8178fca04cdb9a23aeb8da08ae6d6e6c0ffa0c79f2213f98b1ac6bfa141b6724138223236e89ae456e6c6727f8709e4b28ed6ff0180ff01ffffffff70c07101022f2c9ba1b2315d413a92b5f034fa03282ccba1767fd9ae7b14d942b969ed5d578a505367d099210c24f1be8945a83de7db6d9396a9742c8f609aebf7ba56bbaacb038819b122741211bbc9227c903573010000001668747470733a2f2f6e61312e706f6f6c2e73706163650000004080ff80808080ffffa0bc334d2f6b030790debd7e4a998a38d0628b2b853fa7895db16ce14da37c441dffff02ffff01ff02ffff01ff02ffff03ffff18ff2fffff010180ffff01ff02ff36ffff04ff02ffff04ff05ffff04ff17ffff04ffff02ff26ffff04ff02ffff04ff0bff80808080ffff04ff2fffff04ff0bffff04ff5fff808080808080808080ffff01ff088080ff0180ffff04ffff01ffffffff4602ff3304ffff0101ff02ffff02ffff03ff05ffff01ff02ff5cffff04ff02ffff04ff0dffff04ffff0bff2cffff0bff24ff3880ffff0bff2cffff0bff2cffff0bff24ff3480ff0980ffff0bff2cff0bffff0bff24ff8080808080ff8080808080ffff010b80ff0180ff02ffff03ff0bffff01ff02ff32ffff04ff02ffff04ff05ffff04ff0bffff04ff17ffff04ffff02ff2affff04ff02ffff04ffff02ffff03ffff09ff23ff2880ffff0181b3ff8080ff0180ff80808080ff80808080808080ffff01ff02ffff03ff17ff80ffff01ff088080ff018080ff0180ffffffff0bffff0bff17ffff02ff3affff04ff02ffff04ff09ffff04ff2fffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ff5f80ff0bff81bf80ff02ffff03ffff20ffff22ff4fff178080ffff01ff02ff7effff04ff02ffff04ff6fffff04ffff04ffff02ffff03ff4fffff01ff04ff23ffff04ffff02ff3affff04ff02ffff04ff09ffff04ff53ffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ffff04ff81b3ff80808080ffff011380ff0180ffff02ff7cffff04ff02ffff04ff05ffff04ff1bffff04ffff21ff4fff1780ff80808080808080ff8080808080ffff01ff088080ff0180ffff04ffff09ffff18ff05ffff010180ffff010180ffff09ff05ffff01818f8080ff0bff2cffff0bff24ff3080ffff0bff2cffff0bff2cffff0bff24ff3480ff0580ffff0bff2cffff02ff5cffff04ff02ffff04ff07ffff04ffff0bff24ff2480ff8080808080ffff0bff24ff8080808080ffffff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff26ffff04ff02ffff04ff09ff80808080ffff02ff26ffff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff02ff5effff04ff02ffff04ff05ffff04ff0bffff04ffff02ff3affff04ff02ffff04ff09ffff04ff17ffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ffff04ff17ffff04ff2fffff04ff5fffff04ff81bfff80808080808080808080ffff04ffff04ff20ffff04ff17ff808080ffff02ff7cffff04ff02ffff04ff05ffff04ffff02ff82017fffff04ffff04ffff04ff17ff2f80ffff04ffff04ff5fff81bf80ffff04ff0bff05808080ff8202ff8080ffff01ff80808080808080ffff02ff2effff04ff02ffff04ff05ffff04ff0bffff04ffff02ffff03ff3bffff01ff02ff22ffff04ff02ffff04ff05ffff04ff17ffff04ff13ffff04ff2bffff04ff5bffff04ff5fff808080808080808080ffff01ff02ffff03ffff09ff15ffff0bff13ff1dff2b8080ffff01ff0bff15ff17ff5f80ffff01ff088080ff018080ff0180ffff04ff17ffff04ff2fffff04ff5fffff04ff81bfffff04ff82017fff8080808080808080808080ff02ffff03ff05ffff011bffff010b80ff0180ff018080ffff04ffff01ffa024e044101e57b3d8c908b8a38ad57848afd29d3eecc439dba45f4412df4954fdffa01a3272c823c1175f83016303bfd33823687df39736e2b7eaf9057f00671d9f97a0eff07522495060c066f66f32acc2a77e3a3e737aca8baea4d1a64ea4cdc13da9ffff04ffff01ff02ffff01ff02ffff01ff02ffff03ff8202ffffff01ff02ff16ffff04ff02ffff04ff05ffff04ff8204bfffff04ff8206bfffff04ff82017fffff04ffff0bffff19ff2fffff18ffff019100ffffffffffffffffffffffffffffffffff8202ff8080ff0bff82017f80ff8080808080808080ffff01ff04ffff04ff08ffff04ff17ffff04ffff02ff1effff04ff02ffff04ff82017fff80808080ff80808080ffff04ffff04ff1cffff04ff5fffff04ff8206bfff80808080ff80808080ff0180ffff04ffff01ffff32ff3d33ff3effff04ffff04ff1cffff04ff0bffff04ff17ff80808080ffff04ffff04ff1cffff04ff05ffff04ff2fff80808080ffff04ffff04ff0affff04ff5fff808080ffff04ffff04ff14ffff04ffff0bff5fffff012480ff808080ff8080808080ff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff1effff04ff02ffff04ff09ff80808080ffff02ff1effff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff018080ffff04ffff01a09d9c5296f00b89c2271ab4a00f249ab3a0106d8d73dd02242f3ea6357b4cde04ffff04ffff01a0e691c76d0108a7a7a44591b3784ecf4099bf5fb057173a0bb2f79fdfa2ed9fceffff04ffff01b0ab6824901d856c5a8c1664c990d1ef94a19ed7b4ab28a6b8e064f1a11e07f5e75bdb6ff8242f517534df36ae03c81da0ffff04ffff01a0ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000ffff04ffff01a0ab43e98b62a2dc33caf0b16fb5a3c037e3303fc8e177ddf437eef233c87d32f2ff01808080808080ff01808080ff01ffffffa00afb9bf9c6a13d380c9645ae07e466bf71a171ae6fe35bc3a7ac5fb5df53a937ffa0cec914e2de9e524237e7a76f3d483a9cf1674be213d4c5bf51fe28b6dab92898ff0180ff01ffffffff70c07001029d9c5296f00b89c2271ab4a00f249ab3a0106d8d73dd02242f3ea6357b4cde04ab6824901d856c5a8c1664c990d1ef94a19ed7b4ab28a6b8e064f1a11e07f5e75bdb6ff8242f517534df36ae03c81da0010000001568747470733a2f2f636869612e64706f6f6c2e63630000002080ff80808080ffffa07016fd25c14831bfe48a08cd3cd9eeb6d416436087252e1061e62cdc95cc892affff02ffff01ff02ffff01ff02ffff03ffff18ff2fffff010180ffff01ff02ff36ffff04ff02ffff04ff05ffff04ff17ffff04ffff02ff26ffff04ff02ffff04ff0bff80808080ffff04ff2fffff04ff0bffff04ff5fff808080808080808080ffff01ff088080ff0180ffff04ffff01ffffffff4602ff3304ffff0101ff02ffff02ffff03ff05ffff01ff02ff5cffff04ff02ffff04ff0dffff04ffff0bff2cffff0bff24ff3880ffff0bff2cffff0bff2cffff0bff24ff3480ff0980ffff0bff2cff0bffff0bff24ff8080808080ff8080808080ffff010b80ff0180ff02ffff03ff0bffff01ff02ff32ffff04ff02ffff04ff05ffff04ff0bffff04ff17ffff04ffff02ff2affff04ff02ffff04ffff02ffff03ffff09ff23ff2880ffff0181b3ff8080ff0180ff80808080ff80808080808080ffff01ff02ffff03ff17ff80ffff01ff088080ff018080ff0180ffffffff0bffff0bff17ffff02ff3affff04ff02ffff04ff09ffff04ff2fffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ff5f80ff0bff81bf80ff02ffff03ffff20ffff22ff4fff178080ffff01ff02ff7effff04ff02ffff04ff6fffff04ffff04ffff02ffff03ff4fffff01ff04ff23ffff04ffff02ff3affff04ff02ffff04ff09ffff04ff53ffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ffff04ff81b3ff80808080ffff011380ff0180ffff02ff7cffff04ff02ffff04ff05ffff04ff1bffff04ffff21ff4fff1780ff80808080808080ff8080808080ffff01ff088080ff0180ffff04ffff09ffff18ff05ffff010180ffff010180ffff09ff05ffff01818f8080ff0bff2cffff0bff24ff3080ffff0bff2cffff0bff2cffff0bff24ff3480ff0580ffff0bff2cffff02ff5cffff04ff02ffff04ff07ffff04ffff0bff24ff2480ff8080808080ffff0bff24ff8080808080ffffff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff26ffff04ff02ffff04ff09ff80808080ffff02ff26ffff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff02ff5effff04ff02ffff04ff05ffff04ff0bffff04ffff02ff3affff04ff02ffff04ff09ffff04ff17ffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ffff04ff17ffff04ff2fffff04ff5fffff04ff81bfff80808080808080808080ffff04ffff04ff20ffff04ff17ff808080ffff02ff7cffff04ff02ffff04ff05ffff04ffff02ff82017fffff04ffff04ffff04ff17ff2f80ffff04ffff04ff5fff81bf80ffff04ff0bff05808080ff8202ff8080ffff01ff80808080808080ffff02ff2effff04ff02ffff04ff05ffff04ff0bffff04ffff02ffff03ff3bffff01ff02ff22ffff04ff02ffff04ff05ffff04ff17ffff04ff13ffff04ff2bffff04ff5bffff04ff5fff808080808080808080ffff01ff02ffff03ffff09ff15ffff0bff13ff1dff2b8080ffff01ff0bff15ff17ff5f80ffff01ff088080ff018080ff0180ffff04ff17ffff04ff2fffff04ff5fffff04ff81bfffff04ff82017fff8080808080808080808080ff02ffff03ff05ffff011bffff010b80ff0180ff018080ffff04ffff01ffa024e044101e57b3d8c908b8a38ad57848afd29d3eecc439dba45f4412df4954fdffa0cb75e5c90f2ab4bdf1db8a420e56e9edb261b919b73a6f8756453c07d73d430fa0eff07522495060c066f66f32acc2a77e3a3e737aca8baea4d1a64ea4cdc13da9ffff04ffff01ff02ffff01ff02ffff01ff02ffff03ff82017fffff01ff04ffff04ff1cffff04ff5fff808080ffff04ffff04ff12ffff04ff8205ffffff04ff8206bfff80808080ffff04ffff04ff08ffff04ff17ffff04ffff02ff1effff04ff02ffff04ffff04ff8205ffffff04ff8202ffff808080ff80808080ff80808080ff80808080ffff01ff02ff16ffff04ff02ffff04ff05ffff04ff8204bfffff04ff8206bfffff04ff8202ffffff04ffff0bffff19ff2fffff18ffff019100ffffffffffffffffffffffffffffffffff8205ff8080ff0bff8202ff80ff808080808080808080ff0180ffff04ffff01ffff32ff3d52ffff333effff04ffff04ff12ffff04ff0bffff04ff17ff80808080ffff04ffff04ff12ffff04ff05ffff04ff2fff80808080ffff04ffff04ff1affff04ff5fff808080ffff04ffff04ff14ffff04ffff0bff5fffff012480ff808080ff8080808080ff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff1effff04ff02ffff04ff09ff80808080ffff02ff1effff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff018080ffff04ffff01a09d9c5296f00b89c2271ab4a00f249ab3a0106d8d73dd02242f3ea6357b4cde04ffff04ffff01a0a219765e3616e24fb86a7ddace966d0aacfcdb8d8b6823e9760e6b4a0469e07affff04ffff01b0afdbc8d2811665196a20931b06ffe981a2ec64aebd2d917478bf8441d77cb2b62f96194277d91983c5ca9edf0a17fdccffff04ffff01a0ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000ffff04ffff0120ff01808080808080ff01808080ff01ffffffa0b3957791c7e84aa27e759b217ef97285c3c260b0410f230679a00a346ee695b4ffa03732f9605848b5ee1fe700dd36aab3aa23110d35c0e5917676d042883330c39aff0180ff01ffff01ffffff70c0570101016127e457a90eb12296658006a7928d5acffbe3c707b705177efe504d1beae0afdbc8d2811665196a20931b06ffe981a2ec64aebd2d917478bf8441d77cb2b62f96194277d91983c5ca9edf0a17fdcc000000000080ffa062e47157eea5430b839a8fcd8390ce3c162b61acd19f94eeb97db81d7622a52e808080ffffa0b63a7ce25b1050bfd97a9e4e67fcf42ca6545eaf392a13c67307ee3614e59bc2ffff02ffff01ff02ffff01ff02ffff03ffff18ff2fffff010180ffff01ff02ff36ffff04ff02ffff04ff05ffff04ff17ffff04ffff02ff26ffff04ff02ffff04ff0bff80808080ffff04ff2fffff04ff0bffff04ff5fff808080808080808080ffff01ff088080ff0180ffff04ffff01ffffffff4602ff3304ffff0101ff02ffff02ffff03ff05ffff01ff02ff5cffff04ff02ffff04ff0dffff04ffff0bff2cffff0bff24ff3880ffff0bff2cffff0bff2cffff0bff24ff3480ff0980ffff0bff2cff0bffff0bff24ff8080808080ff8080808080ffff010b80ff0180ff02ffff03ff0bffff01ff02ff32ffff04ff02ffff04ff05ffff04ff0bffff04ff17ffff04ffff02ff2affff04ff02ffff04ffff02ffff03ffff09ff23ff2880ffff0181b3ff8080ff0180ff80808080ff80808080808080ffff01ff02ffff03ff17ff80ffff01ff088080ff018080ff0180ffffffff0bffff0bff17ffff02ff3affff04ff02ffff04ff09ffff04ff2fffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ff5f80ff0bff81bf80ff02ffff03ffff20ffff22ff4fff178080ffff01ff02ff7effff04ff02ffff04ff6fffff04ffff04ffff02ffff03ff4fffff01ff04ff23ffff04ffff02ff3affff04ff02ffff04ff09ffff04ff53ffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ffff04ff81b3ff80808080ffff011380ff0180ffff02ff7cffff04ff02ffff04ff05ffff04ff1bffff04ffff21ff4fff1780ff80808080808080ff8080808080ffff01ff088080ff0180ffff04ffff09ffff18ff05ffff010180ffff010180ffff09ff05ffff01818f8080ff0bff2cffff0bff24ff3080ffff0bff2cffff0bff2cffff0bff24ff3480ff0580ffff0bff2cffff02ff5cffff04ff02ffff04ff07ffff04ffff0bff24ff2480ff8080808080ffff0bff24ff8080808080ffffff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff26ffff04ff02ffff04ff09ff80808080ffff02ff26ffff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff02ff5effff04ff02ffff04ff05ffff04ff0bffff04ffff02ff3affff04ff02ffff04ff09ffff04ff17ffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ffff04ff17ffff04ff2fffff04ff5fffff04ff81bfff80808080808080808080ffff04ffff04ff20ffff04ff17ff808080ffff02ff7cffff04ff02ffff04ff05ffff04ffff02ff82017fffff04ffff04ffff04ff17ff2f80ffff04ffff04ff5fff81bf80ffff04ff0bff05808080ff8202ff8080ffff01ff80808080808080ffff02ff2effff04ff02ffff04ff05ffff04ff0bffff04ffff02ffff03ff3bffff01ff02ff22ffff04ff02ffff04ff05ffff04ff17ffff04ff13ffff04ff2bffff04ff5bffff04ff5fff808080808080808080ffff01ff02ffff03ffff09ff15ffff0bff13ff1dff2b8080ffff01ff0bff15ff17ff5f80ffff01ff088080ff018080ff0180ffff04ff17ffff04ff2fffff04ff5fffff04ff81bfffff04ff82017fff8080808080808080808080ff02ffff03ff05ffff011bffff010b80ff0180ff018080ffff04ffff01ffa024e044101e57b3d8c908b8a38ad57848afd29d3eecc439dba45f4412df4954fdffa05a7cdf809298a6c314bfd6ec63c6761b396fca802c0067d87de23644d17a8bb5a0eff07522495060c066f66f32acc2a77e3a3e737aca8baea4d1a64ea4cdc13da9ffff04ffff01ff02ffff01ff02ffff01ff02ffff03ff82017fffff01ff04ffff04ff1cffff04ff5fff808080ffff04ffff04ff12ffff04ff8205ffffff04ff8206bfff80808080ffff04ffff04ff08ffff04ff17ffff04ffff02ff1effff04ff02ffff04ffff04ff8205ffffff04ff8202ffff808080ff80808080ff80808080ff80808080ffff01ff02ff16ffff04ff02ffff04ff05ffff04ff8204bfffff04ff8206bfffff04ff8202ffffff04ffff0bffff19ff2fffff18ffff019100ffffffffffffffffffffffffffffffffff8205ff8080ff0bff8202ff80ff808080808080808080ff0180ffff04ffff01ffff32ff3d52ffff333effff04ffff04ff12ffff04ff0bffff04ff17ff80808080ffff04ffff04ff12ffff04ff05ffff04ff2fff80808080ffff04ffff04ff1affff04ff5fff808080ffff04ffff04ff14ffff04ffff0bff5fffff012480ff808080ff8080808080ff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff1effff04ff02ffff04ff09ff80808080ffff02ff1effff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff018080ffff04ffff01a09d9c5296f00b89c2271ab4a00f249ab3a0106d8d73dd02242f3ea6357b4cde04ffff04ffff01a06dd75452b3a13128591f83a68263fb0dc9bedfb519af3af01933782ae65dca1bffff04ffff01b08e2ab4bd0f4b65f0e6e1cc1f54fd3a953a36afc98ec25a741958bf1f19d0a416f2b39b89d4bd9870f11d6bf09030780effff04ffff01a0ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000ffff04ffff0120ff01808080808080ff01808080ff01ffffffa0f447a4cda2bd4e2c14398f96d1402e8ed0c35302b0c57f8219861d9433ba150cffa0eb4e5fc93add634ac692d2c28b0eed8dcdca399639cd7986dc6879c7a872e5f4ff0180ff01ffff01ffffff70c07701030213db9cb540a52c39071ef70acdf81796303189061b5aa0ee8098a05d5ceff58e2ab4bd0f4b65f0e6e1cc1f54fd3a953a36afc98ec25a741958bf1f19d0a416f2b39b89d4bd9870f11d6bf09030780e010000001c68747470733a2f2f7669702e746565706f6f6c2e636f6d3a393434330000002080ffa0a6322ec0a3d445a051349cf8289660b2d9686608484ecb42c135fd5bd4ea4b11808080ffffa077c52e138369b3a545a59f3daf2904197f350010676506eead7f5875f511f063ffff02ffff01ff02ffff01ff02ffff03ffff18ff2fffff010180ffff01ff02ff36ffff04ff02ffff04ff05ffff04ff17ffff04ffff02ff26ffff04ff02ffff04ff0bff80808080ffff04ff2fffff04ff0bffff04ff5fff808080808080808080ffff01ff088080ff0180ffff04ffff01ffffffff4602ff3304ffff0101ff02ffff02ffff03ff05ffff01ff02ff5cffff04ff02ffff04ff0dffff04ffff0bff2cffff0bff24ff3880ffff0bff2cffff0bff2cffff0bff24ff3480ff0980ffff0bff2cff0bffff0bff24ff8080808080ff8080808080ffff010b80ff0180ff02ffff03ff0bffff01ff02ff32ffff04ff02ffff04ff05ffff04ff0bffff04ff17ffff04ffff02ff2affff04ff02ffff04ffff02ffff03ffff09ff23ff2880ffff0181b3ff8080ff0180ff80808080ff80808080808080ffff01ff02ffff03ff17ff80ffff01ff088080ff018080ff0180ffffffff0bffff0bff17ffff02ff3affff04ff02ffff04ff09ffff04ff2fffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ff5f80ff0bff81bf80ff02ffff03ffff20ffff22ff4fff178080ffff01ff02ff7effff04ff02ffff04ff6fffff04ffff04ffff02ffff03ff4fffff01ff04ff23ffff04ffff02ff3affff04ff02ffff04ff09ffff04ff53ffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ffff04ff81b3ff80808080ffff011380ff0180ffff02ff7cffff04ff02ffff04ff05ffff04ff1bffff04ffff21ff4fff1780ff80808080808080ff8080808080ffff01ff088080ff0180ffff04ffff09ffff18ff05ffff010180ffff010180ffff09ff05ffff01818f8080ff0bff2cffff0bff24ff3080ffff0bff2cffff0bff2cffff0bff24ff3480ff0580ffff0bff2cffff02ff5cffff04ff02ffff04ff07ffff04ffff0bff24ff2480ff8080808080ffff0bff24ff8080808080ffffff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff26ffff04ff02ffff04ff09ff80808080ffff02ff26ffff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff02ff5effff04ff02ffff04ff05ffff04ff0bffff04ffff02ff3affff04ff02ffff04ff09ffff04ff17ffff04ffff02ff26ffff04ff02ffff04ff05ff80808080ff808080808080ffff04ff17ffff04ff2fffff04ff5fffff04ff81bfff80808080808080808080ffff04ffff04ff20ffff04ff17ff808080ffff02ff7cffff04ff02ffff04ff05ffff04ffff02ff82017fffff04ffff04ffff04ff17ff2f80ffff04ffff04ff5fff81bf80ffff04ff0bff05808080ff8202ff8080ffff01ff80808080808080ffff02ff2effff04ff02ffff04ff05ffff04ff0bffff04ffff02ffff03ff3bffff01ff02ff22ffff04ff02ffff04ff05ffff04ff17ffff04ff13ffff04ff2bffff04ff5bffff04ff5fff808080808080808080ffff01ff02ffff03ffff09ff15ffff0bff13ff1dff2b8080ffff01ff0bff15ff17ff5f80ffff01ff088080ff018080ff0180ffff04ff17ffff04ff2fffff04ff5fffff04ff81bfffff04ff82017fff8080808080808080808080ff02ffff03ff05ffff011bffff010b80ff0180ff018080ffff04ffff01ffa024e044101e57b3d8c908b8a38ad57848afd29d3eecc439dba45f4412df4954fdffa00485de73367a4b49eb34c7f80df3c9b70c739411d40632428e42495da7c0ba91a0eff07522495060c066f66f32acc2a77e3a3e737aca8baea4d1a64ea4cdc13da9ffff04ffff01ff02ffff01ff02ffff01ff02ffff03ff82017fffff01ff04ffff04ff1cffff04ff5fff808080ffff04ffff04ff12ffff04ff8205ffffff04ff8206bfff80808080ffff04ffff04ff08ffff04ff17ffff04ffff02ff1effff04ff02ffff04ffff04ff8205ffffff04ff8202ffff808080ff80808080ff80808080ff80808080ffff01ff02ff16ffff04ff02ffff04ff05ffff04ff8204bfffff04ff8206bfffff04ff8202ffffff04ffff0bffff19ff2fffff18ffff019100ffffffffffffffffffffffffffffffffff8205ff8080ff0bff8202ff80ff808080808080808080ff0180ffff04ffff01ffff32ff3d52ffff333effff04ffff04ff12ffff04ff0bffff04ff17ff80808080ffff04ffff04ff12ffff04ff05ffff04ff2fff80808080ffff04ffff04ff1affff04ff5fff808080ffff04ffff04ff14ffff04ffff0bff5fffff012480ff808080ff8080808080ff02ffff03ffff07ff0580ffff01ff0bffff0102ffff02ff1effff04ff02ffff04ff09ff80808080ffff02ff1effff04ff02ffff04ff0dff8080808080ffff01ff0bffff0101ff058080ff0180ff018080ffff04ffff01a09d9c5296f00b89c2271ab4a00f249ab3a0106d8d73dd02242f3ea6357b4cde04ffff04ffff01a0671ce6fd24697788441f93773e5905c1f1153ba7f5d3fbb6a4e2855a05b42731ffff04ffff01b0a5383a3b9a6c1a94a85e4f982e1fa3af2c99087e5f6df8b887d30c109f71043671683a1ae985d7d874fbe07dfa6d88b7ffff04ffff01a0ccd5bb71183532bff220ba46c268991a00000000000000000000000000000000ffff04ffff0120ff01808080808080ff01808080ff01ffffffa01dc8c9c3356a6eefee37744901b3f730c710052bd38deac264ecea45460faffeffa031460205316513dc6b11d0993462776f0994223cac2f215bf8afbeae5a0cce3fff0180ff01ffff01ffffff70c0730103e3b9adc4eb09d18d83bd56482aee566820f5afdce595b3ed095eb36c5cef9301a5383a3b9a6c1a94a85e4f982e1fa3af2c99087e5f6df8b887d30c109f71043671683a1ae985d7d874fbe07dfa6d88b7010000001868747470733a2f2f6368696170702e68706f6f6c2e636f6d0000004080ffa0fc0b1e9409ae5c3c40c50832a7aecc0b3ba4646568a00c01289c45e1f03b2b488080808080
+SPENDS:
+- coin id: 3c3412900b156403b13bb4191f1d6818619f73c97337829a4f821012b24d88eb ph: bc0e759db02410acb193d0c1c0a6841a2a821c9322570e2f23dfe220d9e6ae8f
+  ASSERT_HEIGHT_RELATIVE 32
+  CREATE_COIN: ph: 013beb3fa36f6d3f221253f7ef380e4d1197246b57b453ce32d339e9be4b2eec amount: 1
+  AGG_SIG_ME pk: afdbc8d2811665196a20931b06ffe981a2ec64aebd2d917478bf8441d77cb2b62f96194277d91983c5ca9edf0a17fdcc msg: f19e77711df9e26a0e1fda2279bd73d6dcb9afe91dafadb4c3c20b1fe441a1b3
+- coin id: 8522228562997c720038e6dca3721c36b054d766e0de80087ae9d7b4b229df29 ph: 1dc30429a17e6ee7d5b18a795da6bf838b7c87d0cf65cfb000fca5bab1ccbe19
+  CREATE_COIN: ph: c30e2a348a6a4f56fc8d4ce44cebda06f72420d68e454dd765ed40b782fca307 amount: 1
+  AGG_SIG_ME pk: 8a505367d099210c24f1be8945a83de7db6d9396a9742c8f609aebf7ba56bbaacb038819b122741211bbc9227c903573 msg: 6cbb9e5def3ed896de9651b54145afc27bcbba9c61ca853b1e3bf0e6b8a78e9a
+- coin id: a66d7b064c9fdfbcffe0755766c1a5d66899fab9f9a6cb4f93d614d676bc8292 ph: ba5089cb215c3f37dbc5718820d16d454694869e756653a516d2abb3faacd843
+  ASSERT_HEIGHT_RELATIVE 32
+  CREATE_COIN: ph: 87c64d9ef085869b1bf272816a752d093e272fa69d6840181cd48fa8eb86dcc3 amount: 1
+  AGG_SIG_ME pk: 8e2ab4bd0f4b65f0e6e1cc1f54fd3a953a36afc98ec25a741958bf1f19d0a416f2b39b89d4bd9870f11d6bf09030780e msg: 01f207c53eb38d9a0ca38981ddedf93c9d62ac0073f5706c1d513cc109206a00
+- coin id: afd297097757a8f5a3f3266933a6c29a7674c71028825562e7e4cac02b9228f6 ph: b78c1c1c0fe082b9c7f18d7e7c716b1607fd62dbdf3eef18f79e2717789ac55f
+  CREATE_COIN: ph: dca1429bcffab70d2218df91683ebe292305925337c0fffa91d5244838ffbd80 amount: 1
+  AGG_SIG_ME pk: 8116639d853ecd6109277a9d83d3acc7e53a18d3524262ec9b99df923d22a390cbf0f632bced556dd9886bbf53f444b6 msg: d497b66589f5d8bdc0631678cc488e25360d114eee51b84a3c1685771a7daa2d
+- coin id: b4fa0835dd9d595cf3d3c5e574ce081c7cca37452c4c336caaf8fbf644c5b268 ph: 0ac6539fede8c4cd50610af58f82b8cc74c774577f0a098db8ab2f42e5e90a9f
+  CREATE_COIN: ph: 948a5a1b3367d80aebc23a7ae772b140b8626f908d5b921f9980a0f01280e3c8 amount: 1
+  AGG_SIG_ME pk: ab6824901d856c5a8c1664c990d1ef94a19ed7b4ab28a6b8e064f1a11e07f5e75bdb6ff8242f517534df36ae03c81da0 msg: 38442a894ff28abb1225d3698c2e09aaea12827c9141f9e4c85267a38cec3e6f
+- coin id: ed418e8b3f49d86a0ab42343e1dc864f796026b8646c953a3bd54329a3843c1f ph: 87864b58be87e5f0fe566955088597ea0f5aafaad1ce0ed8dd02f5c84d257aa6
+  ASSERT_HEIGHT_RELATIVE 32
+  CREATE_COIN: ph: 70aea9db5a7c74a2dfa632ddac0e7cd3283c6439c1feae0417645b6392104ded amount: 1
+  AGG_SIG_ME pk: a5383a3b9a6c1a94a85e4f982e1fa3af2c99087e5f6df8b887d30c109f71043671683a1ae985d7d874fbe07dfa6d88b7 msg: 5d53d6baf98f40ce52d588135fa97fc7c6756c6fb6315298902d631548704d8c
+cost: 191803080
+removal_amount: 6
+addition_amount: 6
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia/tests/generators/create-coin-different-amounts.clvm` & `chia_rs-0.2.8/local_dependencies/chia/generator-tests/create-coin-hint2.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-(q ((0x0101010101010101010101010101010101010101010101010101010101010101 (q  (51 "abababababababababababababababab" 5) (51 "abababababababababababababababab" 4) ) 123 (() (q . ())))))
+ff01ffffffa00101010101010101010101010101010101010101010101010101010101010101ffff01ffff33ffa06162616261626162616261626162616261626162616261626162616261626162ff05ffffa03132313231323132313231323132313231323132313231323132313231323132ff8461626364ff84656667688080ffff33ffa06162616261626162616261626162616261626162616261626162616261626162ff048080ff7bffff80ffff018080808080
 SPENDS:
-- coin id: d0172c347e5e159a3dd0c4c8f47fe2e2331c946ff7596df14b64a10da0854031 ph: 549249cd4633a158169f04405ee11c74b6a6f21aa9e10b1c283ff687d4d644a0
+- coin id: 14f1e9b5377e99d2f17a56dedc70d2cbac099e732a68f4d71f6d86378c10b760 ph: 0ff60a007bf51df4cbc8e178ea6da0e38e3f5f4b76fe1820950b386de7c49a64
   CREATE_COIN: ph: 6162616261626162616261626162616261626162616261626162616261626162 amount: 4
-  CREATE_COIN: ph: 6162616261626162616261626162616261626162616261626162616261626162 amount: 5
-cost: 5252834
+  CREATE_COIN: ph: 6162616261626162616261626162616261626162616261626162616261626162 amount: 5 hint: 3132313231323132313231323132313231323132313231323132313231323132
+cost: 5841210
 removal_amount: 123
 addition_amount: 9
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia/tests/generators/many-create-coin.clvm` & `chia_rs-0.2.8/local_dependencies/chia/generator-tests/many-create-coin.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-(q ((0x0101010101010101010101010101010101010101010101010101010101010101  (a (q 2 6 (c 2 (c (q 51 "abababababababababababababababab") (c 5 ())))) (c (q (a (i 5 (q 4 9 (a 4 (c 2 (c 13 (c 11 ()))))) (q 4 11 ())) 1) 2 (i 11 (q 4 (a 4 (c 2 (c 5 (c 11 ())))) (a 6 (c 2 (c 5 (c (- 11 (q . 1)) ()))))) ()) 1) (q 6094))) 18605000 (() (q . ())))))
+ff01ffffffa00101010101010101010101010101010101010101010101010101010101010101ffff02ffff01ff02ff06ffff04ff02ffff04ffff01ff33ffa0616261626162616261626162616261626162616261626162616261626162616280ffff04ff05ff8080808080ffff04ffff01ffff02ffff03ff05ffff01ff04ff09ffff02ff04ffff04ff02ffff04ff0dffff04ff0bff808080808080ffff01ff04ff0bff808080ff0180ff02ffff03ff0bffff01ff04ffff02ff04ffff04ff02ffff04ff05ffff04ff0bff8080808080ffff02ff06ffff04ff02ffff04ff05ffff04ffff11ff0bffff010180ff808080808080ff8080ff0180ffff01ff8217ce808080ff84011be3c8ffff80ffff018080808080
 SPENDS:
 - coin id: 2a6991d3bfd05e5286e95ebdbb53978211dad6f00a2a50fc19995c1bfc933c11 ph: c69b40b3edfc197e6b6ec325d3f43f01a7c30b99d331fbc30c24a7a571d0a094
   CREATE_COIN: ph: 6162616261626162616261626162616261626162616261626162616261626162 amount: 1
   CREATE_COIN: ph: 6162616261626162616261626162616261626162616261626162616261626162 amount: 2
   CREATE_COIN: ph: 6162616261626162616261626162616261626162616261626162616261626162 amount: 3
   CREATE_COIN: ph: 6162616261626162616261626162616261626162616261626162616261626162 amount: 4
   CREATE_COIN: ph: 6162616261626162616261626162616261626162616261626162616261626162 amount: 5
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia/tests/run-programs.py` & `chia_rs-0.2.8/local_dependencies/chia/tests/run-programs.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/tests/run.py` & `chia_rs-0.2.8/local_dependencies/chia/tests/run.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/tests/run_gen.py` & `chia_rs-0.2.8/local_dependencies/chia/tests/run_gen.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 #!/usr/bin/env python3
 
 from chia_rs import run_block_generator
 from time import time
-from clvm_tools import binutils
-from clvm.serialize import atom_to_byte_iterator
 import sys
 from typing import Optional
 
-def serialize_atom(blob: bytes) -> bytes:
-    ret = bytearray()
-    for b in atom_to_byte_iterator(blob):
-        ret += b
-    return bytes(ret)
-
-
 def run_gen(fn: str, flags: int = 0, args: Optional[str] = None):
 
     # constants from the main chia blockchain:
     # https://github.com/Chia-Network/chia-blockchain/blob/main/chia/consensus/default_constants.py
     max_cost = 11000000000
     cost_per_byte = 12000
 
-    generator = binutils.assemble(open(fn, "r").read()).as_bin()
+    generator = bytes.fromhex(open(fn, "r").read().split('\n')[0])
 
     # add the block program arguments
     block_refs = []
     if args and args != "":
         with open(args, "r") as f:
             block_refs = [bytes.fromhex(f.read())]
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia/tests/test_coin.py` & `chia_rs-0.2.8/local_dependencies/chia/tests/test_coin.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/tests/test_run_block_generator.py` & `chia_rs-0.2.8/local_dependencies/chia/tests/test_run_block_generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from clvm_tools import binutils
 from chia_rs import run_block_generator
-from chia_rs import MEMPOOL_MODE, LIMIT_STACK
+from chia_rs import MEMPOOL_MODE
 import pytest
 
 def test_run_block_generator_cost() -> None:
 
-    generator = binutils.assemble(open("tests/generators/block-834768.clvm", "r").read()).as_bin()
+    generator = bytes.fromhex(open("generator-tests/block-834768.txt", "r").read().split("\n")[0])
     # the total cost of this generator is 635805370
-    err, conds = run_block_generator(generator, [], 635805370, LIMIT_STACK)
+    err, conds = run_block_generator(generator, [], 635805370, 0)
     assert err is None
     assert conds is not None
 
     # we exceed the cost limit by 1
-    err, conds = run_block_generator(generator, [], 635805370 - 1, LIMIT_STACK)
+    err, conds = run_block_generator(generator, [], 635805370 - 1, 0)
     # BLOCK_COST_EXCEEDS_MAX = 23
     assert err == 23
     assert conds is None
 
     # the byte cost alone exceeds the limit by 1
-    err, conds = run_block_generator(generator, [], len(generator) * 12000 - 1, LIMIT_STACK)
+    err, conds = run_block_generator(generator, [], len(generator) * 12000 - 1, 0)
     # BLOCK_COST_EXCEEDS_MAX = 23
     assert err == 23
     assert conds is None
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia/tests/test_run_puzzle.py` & `chia_rs-0.2.8/local_dependencies/chia/tests/test_run_puzzle.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,28 @@
-from chia_rs import run_puzzle, run_chia_program
+from chia_rs import run_puzzle, run_chia_program, ALLOW_BACKREFS
 from hashlib import sha256
 import pytest
 from run_gen import print_spend_bundle_conditions
 from clvm.SExp import SExp
 from clvm.casts import int_from_bytes
 from clvm_tools import binutils
 import os
 
-def test_block_834752() -> None:
-    block = bytes.fromhex(open(f"{os.path.dirname(__file__)}/generators/block-834752.hex").read())
-    cost, ret = run_chia_program(block, b"\xff\x80\x80", 11000000000, 0)
+@pytest.mark.parametrize("flags", [0, ALLOW_BACKREFS])
+@pytest.mark.parametrize("input_file", ["generator-tests/block-834752.txt", "generator-tests/block-834752-compressed.txt"])
+def test_block_834752(flags: int, input_file: str) -> None:
+    block = bytes.fromhex(open(input_file, "r").read().split("\n")[0])
+
+    if (flags & ALLOW_BACKREFS) == 0 and "compressed" in input_file:
+        with pytest.raises(OSError, match="bad encoding"):
+            cost, ret = run_chia_program(block, b"\xff\x80\x80", 11000000000, flags)
+        return
+    else:
+        cost, ret = run_chia_program(block, b"\xff\x80\x80", 11000000000, flags)
+
     ret = ret.pair[0]
     puzzles = []
 
     while ret.pair is not None:
         spend = ret.pair[0]
         parent = spend.pair[0].atom
         spend = spend.pair[1]
@@ -28,15 +37,15 @@
         spend = spend.pair[1]
 
         puzzles.append((parent, amount, puzzle.as_bin(), solution.as_bin()))
         ret = ret.pair[1]
 
     output = ""
     for parent, amount, puzzle, solution in puzzles:
-        conds = run_puzzle(puzzle, solution, parent, amount, 11000000000, 0)
+        conds = run_puzzle(puzzle, solution, parent, amount, 11000000000, flags)
         output += print_spend_bundle_conditions(conds)
 
     assert output == """\
 SPENDS:
 - coin id: afd297097757a8f5a3f3266933a6c29a7674c71028825562e7e4cac02b9228f6 ph: b78c1c1c0fe082b9c7f18d7e7c716b1607fd62dbdf3eef18f79e2717789ac55f
   CREATE_COIN: ph: dca1429bcffab70d2218df91683ebe292305925337c0fffa91d5244838ffbd80 amount: 1
   AGG_SIG_ME pk: 8116639d853ecd6109277a9d83d3acc7e53a18d3524262ec9b99df923d22a390cbf0f632bced556dd9886bbf53f444b6 msg: d497b66589f5d8bdc0631678cc488e25360d114eee51b84a3c1685771a7daa2d
@@ -79,32 +88,33 @@
   CREATE_COIN: ph: 70aea9db5a7c74a2dfa632ddac0e7cd3283c6439c1feae0417645b6392104ded amount: 1
   AGG_SIG_ME pk: a5383a3b9a6c1a94a85e4f982e1fa3af2c99087e5f6df8b887d30c109f71043671683a1ae985d7d874fbe07dfa6d88b7 msg: 5d53d6baf98f40ce52d588135fa97fc7c6756c6fb6315298902d631548704d8c
 cost: 3792835
 removal_amount: 1
 addition_amount: 1
 """
 
-def test_failure() -> None:
+@pytest.mark.parametrize("flags", [0, ALLOW_BACKREFS])
+def test_failure(flags: int) -> None:
 
     output = ""
     parent = b"1" * 32
     amount = 1337
     # (mod (solution) (if (= solution (q . 1)) () (x solution)))
     puzzle = binutils.assemble("(a (i (= 2 (q . 1)) () (q 8 2)) 1)").as_bin()
     solution1 = binutils.assemble("(1)").as_bin()
     solution2 = binutils.assemble("(2)").as_bin()
 
     # the puzzle expects (1)
-    conds = run_puzzle(puzzle, solution1, parent, amount, 11000000000, 0)
+    conds = run_puzzle(puzzle, solution1, parent, amount, 11000000000, flags)
     output += print_spend_bundle_conditions(conds)
     print(output)
     assert output == """\
 SPENDS:
 - coin id: 7767e945d8b73704d3ed84277b3df4572cec7d418629dc2f0325385e708c7724 ph: 51f3dbcff4ada9fe7030d6c017f243b903f9baf503e2d0590b3b78b5c2589674
 cost: 465
 removal_amount: 1337
 addition_amount: 0
 """
 
     with pytest.raises(ValueError, match="ValidationError"):
         # the puzzle does not expect (2)
-        run_puzzle(puzzle, solution2, parent, amount, 11000000000, 0)
+        run_puzzle(puzzle, solution2, parent, amount, 11000000000, flags)
```

### Comparing `chia_rs-0.2.7/local_dependencies/chia/tests/test_streamable.py` & `chia_rs-0.2.8/local_dependencies/chia/tests/test_streamable.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/local_dependencies/chia/tests/test_tree_hash.py` & `chia_rs-0.2.8/local_dependencies/chia/tests/test_tree_hash.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/Cargo.toml` & `chia_rs-0.2.8/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "chia_rs"
-version = "0.2.7"
+version = "0.2.8"
 authors = ["Richard Kiss <him@richardkiss.com>"]
 edition = "2021"
 license = "Apache-2.0"
 description = "Code useful for implementing chia consensus."
 homepage = "https://github.com/Chia-Network/chia_rs/"
 repository = "https://github.com/Chia-Network/chia_rs/"
 readme = "README.md"
@@ -13,12 +13,12 @@
 name = "chia_rs"
 crate-type = ["cdylib"]
 path = "src/lib.rs"
 
 [dependencies]
 chia = { path = "local_dependencies/chia", features = ["py-bindings"] }
 chia-protocol = { path = "local_dependencies/chia-protocol", features = ["py-bindings"]  }
-clvmr = "=0.2.4"
+clvmr = "=0.2.6"
 pyo3 = { version = "=0.15.1", features = ["extension-module", "multiple-pymethods"] }
 chia_py_streamable_macro = { version= "0.1.3", path = "local_dependencies/chia_py_streamable_macro" }
 chia_streamable_macro = { version = "0.2.4", path = "local_dependencies/chia_streamable_macro" }
 hex = "=0.4.3"
```

### Comparing `chia_rs-0.2.7/chia_rs.pyi` & `chia_rs-0.2.8/chia_rs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -21,19 +21,27 @@
 def run_puzzle(
     puzzle: bytes, solution: bytes, parent_id: bytes32, amount: int, max_cost: int, flags: int
 ) -> SpendBundleConditions: ...
 
 COND_ARGS_NIL: int = ...
 NO_UNKNOWN_CONDS: int = ...
 STRICT_ARGS_COUNT: int = ...
+LIMIT_ANNOUNCES: int = ...
+AGG_SIG_ARGS: int = ...
 LIMIT_HEAP: int = ...
-LIMIT_STACK: int = ...
 ENABLE_ASSERT_BEFORE: int = ...
+ENABLE_SOFTFORK_CONDITION: int = ...
 MEMPOOL_MODE: int = ...
 NO_RELATIVE_CONDITIONS_ON_EPHEMERAL: int = ...
+ENABLE_BLS_OPS: int = ...
+ENABLE_SECP_OPS: int = ...
+ENABLE_BLS_OPS_OUTSIDE_GUARD: int = ...
+LIMIT_OBJECTS: int = ...
+ENABLE_FIXED_DIV: int = ...
+ALLOW_BACKREFS: int = ...
 
 ELIGIBLE_FOR_DEDUP: int = ...
 
 NO_UNKNOWN_OPS: int = ...
 
 def run_chia_program(
     program: bytes, args: bytes, max_cost: int, flags: int
@@ -41,15 +49,15 @@
 
 class LazyNode:
     def pair() -> Optional[Tuple[LazyNode, LazyNode]]: ...
     def atom() -> bytes: ...
 
 def serialized_length(program: bytes) -> int: ...
 def tree_hash(program: ReadableBuffer) -> bytes32: ...
-def get_puzzle_and_solution_for_coin(program: bytes, args: bytes, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32) -> Tuple[bytes, bytes]: ...
+def get_puzzle_and_solution_for_coin(program: bytes, args: bytes, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32, flags: int) -> Tuple[bytes, bytes]: ...
 
 class Spend:
     coin_id: bytes
     puzzle_hash: bytes
     height_relative: Optional[int]
     seconds_relative: Optional[int]
     before_height_relative: Optional[int]
```

### Comparing `chia_rs-0.2.7/generate_type_stubs.py` & `chia_rs-0.2.8/generate_type_stubs.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,19 +165,27 @@
 def run_puzzle(
     puzzle: bytes, solution: bytes, parent_id: bytes32, amount: int, max_cost: int, flags: int
 ) -> SpendBundleConditions: ...
 
 COND_ARGS_NIL: int = ...
 NO_UNKNOWN_CONDS: int = ...
 STRICT_ARGS_COUNT: int = ...
+LIMIT_ANNOUNCES: int = ...
+AGG_SIG_ARGS: int = ...
 LIMIT_HEAP: int = ...
-LIMIT_STACK: int = ...
 ENABLE_ASSERT_BEFORE: int = ...
+ENABLE_SOFTFORK_CONDITION: int = ...
 MEMPOOL_MODE: int = ...
 NO_RELATIVE_CONDITIONS_ON_EPHEMERAL: int = ...
+ENABLE_BLS_OPS: int = ...
+ENABLE_SECP_OPS: int = ...
+ENABLE_BLS_OPS_OUTSIDE_GUARD: int = ...
+LIMIT_OBJECTS: int = ...
+ENABLE_FIXED_DIV: int = ...
+ALLOW_BACKREFS: int = ...
 
 ELIGIBLE_FOR_DEDUP: int = ...
 
 NO_UNKNOWN_OPS: int = ...
 
 def run_chia_program(
     program: bytes, args: bytes, max_cost: int, flags: int
@@ -185,15 +193,15 @@
 
 class LazyNode:
     def pair() -> Optional[Tuple[LazyNode, LazyNode]]: ...
     def atom() -> bytes: ...
 
 def serialized_length(program: bytes) -> int: ...
 def tree_hash(program: ReadableBuffer) -> bytes32: ...
-def get_puzzle_and_solution_for_coin(program: bytes, args: bytes, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32) -> Tuple[bytes, bytes]: ...
+def get_puzzle_and_solution_for_coin(program: bytes, args: bytes, max_cost: int, find_parent: bytes32, find_amount: int, find_ph: bytes32, flags: int) -> Tuple[bytes, bytes]: ...
 """
     )
 
     print_class(f, "Spend",
         [
             "coin_id: bytes",
             "puzzle_hash: bytes",
```

### Comparing `chia_rs-0.2.7/src/adapt_response.rs` & `chia_rs-0.2.8/src/adapt_response.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 use clvmr::allocator::Allocator;
-use clvmr::node::Node;
 use clvmr::reduction::EvalErr;
 use clvmr::serde::node_to_bytes;
 
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
 
 pub fn eval_err_to_pyresult<T>(py: Python, eval_err: EvalErr, allocator: Allocator) -> PyResult<T> {
-    let node = Node::new(&allocator, eval_err.0);
     let ctx: &PyDict = PyDict::new(py);
     let msg = eval_err.1;
     ctx.set_item("msg", msg)?;
-    if let Ok(blob) = node_to_bytes(&node) {
+    if let Ok(blob) = node_to_bytes(&allocator, eval_err.0) {
         ctx.set_item("blob", blob)?;
     }
     Err(py
         .run("raise ValueError(msg, bytes(blob).hex())", None, Some(ctx))
         .unwrap_err())
 }
```

### Comparing `chia_rs-0.2.7/src/api.rs` & `chia_rs-0.2.8/src/api.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 use crate::compression;
-use crate::run_generator::{PySpend, PySpendBundleConditions, convert_spend_bundle_conds, __pyo3_get_function_run_generator, __pyo3_get_function_run_block_generator};
+use crate::run_generator::{
+    convert_spend_bundle_conds, PySpend, PySpendBundleConditions,
+    __pyo3_get_function_run_block_generator, __pyo3_get_function_run_generator,
+};
+use chia::allocator::make_allocator;
+use chia::gen::flags::{
+    AGG_SIG_ARGS, ALLOW_BACKREFS, COND_ARGS_NIL, ENABLE_ASSERT_BEFORE, ENABLE_SOFTFORK_CONDITION,
+    LIMIT_ANNOUNCES, LIMIT_OBJECTS, MEMPOOL_MODE, NO_RELATIVE_CONDITIONS_ON_EPHEMERAL,
+    NO_UNKNOWN_CONDS, STRICT_ARGS_COUNT,
+};
 use chia::gen::run_puzzle::run_puzzle as native_run_puzzle;
-use chia::gen::flags::COND_ARGS_NIL;
-use chia::gen::flags::NO_UNKNOWN_CONDS;
-use chia::gen::flags::STRICT_ARGS_COUNT;
-use chia::gen::flags::MEMPOOL_MODE;
-use chia::gen::flags::ENABLE_ASSERT_BEFORE;
-use chia::gen::flags::NO_RELATIVE_CONDITIONS_ON_EPHEMERAL;
 use chia::merkle_set::compute_merkle_set_root as compute_merkle_root_impl;
-use chia::allocator::make_allocator;
 use chia_protocol::Bytes32;
+use chia_protocol::FullBlock;
 use chia_protocol::G1Element;
 use chia_protocol::G2Element;
-use chia_protocol::FullBlock;
 use chia_protocol::{
     ChallengeBlockInfo, ChallengeChainSubSlot, ClassgroupElement, Coin, CoinSpend, CoinState,
     CoinStateUpdate, EndOfSubSlotBundle, Foliage, FoliageTransactionBlock,
     InfusedChallengeChainSubSlot, NewPeakWallet, PoolTarget, Program, ProofOfSpace,
     PuzzleSolutionResponse, RegisterForCoinUpdates, RegisterForPhUpdates, RejectAdditionsRequest,
     RejectBlockHeaders, RejectHeaderBlocks, RejectHeaderRequest, RejectPuzzleSolution,
     RejectRemovalsRequest, RequestAdditions, RequestBlockHeader, RequestBlockHeaders,
     RequestChildren, RequestFeeEstimates, RequestHeaderBlocks, RequestPuzzleSolution,
     RequestRemovals, RequestSesInfo, RespondAdditions, RespondBlockHeader, RespondBlockHeaders,
     RespondChildren, RespondFeeEstimates, RespondHeaderBlocks, RespondPuzzleSolution,
     RespondRemovals, RespondSesInfo, RespondToCoinUpdates, RespondToPhUpdates, RewardChainBlock,
     RewardChainBlockUnfinished, RewardChainSubSlot, SendTransaction, SpendBundle,
     SubEpochChallengeSegment, SubEpochSegments, SubSlotData, SubSlotProofs, TransactionAck,
-    TransactionsInfo, VDFInfo, VDFProof
+    TransactionsInfo, VDFInfo, VDFProof,
 };
-use std::convert::TryInto;
-use clvmr::LIMIT_HEAP;
-use clvmr::LIMIT_STACK;
-use clvmr::NO_UNKNOWN_OPS;
 use clvmr::serde::tree_hash_from_stream;
+use clvmr::{
+    ENABLE_BLS_OPS, ENABLE_BLS_OPS_OUTSIDE_GUARD, ENABLE_FIXED_DIV, ENABLE_SECP_OPS, LIMIT_HEAP,
+    NO_UNKNOWN_OPS,
+};
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
 use pyo3::types::PyModule;
 use pyo3::{wrap_pyfunction, PyResult, Python};
+use std::convert::TryInto;
 
 use crate::run_program::{
     __pyo3_get_function_run_chia_program, __pyo3_get_function_serialized_length,
 };
 
 use crate::adapt_response::eval_err_to_pyresult;
 use chia::gen::get_puzzle_and_solution::get_puzzle_and_solution_for_coin as parse_puzzle_solution;
 use chia::gen::validation_error::ValidationErr;
 use clvmr::allocator::NodePtr;
-use clvmr::ChiaDialect;
 use clvmr::cost::Cost;
-use clvmr::node::Node;
 use clvmr::reduction::EvalErr;
 use clvmr::reduction::Reduction;
 use clvmr::run_program;
-use clvmr::serde::node_from_bytes;
 use clvmr::serde::node_to_bytes;
+use clvmr::serde::{node_from_bytes, node_from_bytes_backrefs, node_to_bytes_backrefs};
+use clvmr::ChiaDialect;
 
 #[pyfunction]
 pub fn compute_merkle_set_root<'p>(
     py: Python<'p>,
     values: Vec<&'p PyBytes>,
 ) -> PyResult<&'p PyBytes> {
     let mut buffer = Vec::<[u8; 32]>::with_capacity(values.len());
@@ -83,71 +85,93 @@
     py: Python<'py>,
     program: &[u8],
     args: &[u8],
     max_cost: Cost,
     find_parent: Bytes32,
     find_amount: u64,
     find_ph: Bytes32,
+    flags: u32,
 ) -> PyResult<(&'py PyBytes, &'py PyBytes)> {
     let mut allocator = make_allocator(LIMIT_HEAP);
-    let program = node_from_bytes(&mut allocator, program)?;
-    let args = node_from_bytes(&mut allocator, args)?;
-    let dialect = &ChiaDialect::new(LIMIT_STACK);
+
+    let deserialize = if (flags & ALLOW_BACKREFS) != 0 {
+        node_from_bytes_backrefs
+    } else {
+        node_from_bytes
+    };
+    let program = deserialize(&mut allocator, program)?;
+    let args = deserialize(&mut allocator, args)?;
+    let dialect = &ChiaDialect::new(flags);
 
     let r = py.allow_threads(|| -> Result<(NodePtr, NodePtr), EvalErr> {
         let Reduction(_cost, result) =
             run_program(&mut allocator, dialect, program, args, max_cost)?;
         match parse_puzzle_solution(&allocator, result, find_parent, find_amount, find_ph) {
             Err(ValidationErr(n, _)) => Err(EvalErr(n, "coin not found".to_string())),
             Ok(pair) => Ok(pair),
         }
     });
 
+    let serialize = if (flags & ALLOW_BACKREFS) != 0 {
+        node_to_bytes_backrefs
+    } else {
+        node_to_bytes
+    };
     match r {
         Err(eval_err) => eval_err_to_pyresult(py, eval_err, allocator),
-        Ok((puzzle, solution)) => {
-            Ok((
-                PyBytes::new(py, &node_to_bytes(&Node::new(&allocator, puzzle))?),
-                PyBytes::new(py, &node_to_bytes(&Node::new(&allocator, solution))?)
-            ))
-        },
+        Ok((puzzle, solution)) => Ok((
+            PyBytes::new(py, &serialize(&allocator, puzzle)?),
+            PyBytes::new(py, &serialize(&allocator, solution)?),
+        )),
     }
 }
 
 #[pyfunction]
 fn run_puzzle(
     puzzle: &[u8],
     solution: &[u8],
     parent_id: &[u8],
     amount: u64,
     max_cost: Cost,
     flags: u32,
 ) -> PyResult<PySpendBundleConditions> {
     let mut a = make_allocator(LIMIT_HEAP);
     let conds = native_run_puzzle(&mut a, puzzle, solution, parent_id, amount, max_cost, flags)?;
-    Ok(convert_spend_bundle_conds(&mut a, conds))
+    Ok(convert_spend_bundle_conds(&a, conds))
 }
 
 #[pymodule]
 pub fn chia_rs(py: Python, m: &PyModule) -> PyResult<()> {
     // generator functions
     m.add_function(wrap_pyfunction!(run_generator, m)?)?;
     m.add_function(wrap_pyfunction!(run_block_generator, m)?)?;
     m.add_function(wrap_pyfunction!(run_puzzle, m)?)?;
     m.add_class::<PySpendBundleConditions>()?;
-    m.add("ELIGIBLE_FOR_DEDUP", chia::gen::conditions::ELIGIBLE_FOR_DEDUP)?;
+    m.add(
+        "ELIGIBLE_FOR_DEDUP",
+        chia::gen::conditions::ELIGIBLE_FOR_DEDUP,
+    )?;
     m.add_class::<PySpend>()?;
 
     // clvm functions
     m.add("COND_ARGS_NIL", COND_ARGS_NIL)?;
     m.add("NO_UNKNOWN_CONDS", NO_UNKNOWN_CONDS)?;
     m.add("STRICT_ARGS_COUNT", STRICT_ARGS_COUNT)?;
+    m.add("LIMIT_ANNOUNCES", LIMIT_ANNOUNCES)?;
+    m.add("AGG_SIG_ARGS", AGG_SIG_ARGS)?;
     m.add("ENABLE_ASSERT_BEFORE", ENABLE_ASSERT_BEFORE)?;
-    m.add("NO_RELATIVE_CONDITIONS_ON_EPHEMERAL", NO_RELATIVE_CONDITIONS_ON_EPHEMERAL)?;
+    m.add("ENABLE_FIXED_DIV", ENABLE_FIXED_DIV)?;
+    m.add("ENABLE_SOFTFORK_CONDITION", ENABLE_SOFTFORK_CONDITION)?;
+    m.add(
+        "NO_RELATIVE_CONDITIONS_ON_EPHEMERAL",
+        NO_RELATIVE_CONDITIONS_ON_EPHEMERAL,
+    )?;
     m.add("MEMPOOL_MODE", MEMPOOL_MODE)?;
+    m.add("LIMIT_OBJECTS", LIMIT_OBJECTS)?;
+    m.add("ALLOW_BACKREFS", ALLOW_BACKREFS)?;
 
     // Chia classes
     m.add_class::<Coin>()?;
     m.add_class::<G1Element>()?;
     m.add_class::<G2Element>()?;
     m.add_class::<PoolTarget>()?;
     m.add_class::<ClassgroupElement>()?;
@@ -211,15 +235,18 @@
     m.add_class::<FullBlock>()?;
 
     // facilities from clvm_rs
 
     m.add_function(wrap_pyfunction!(run_chia_program, m)?)?;
     m.add("NO_UNKNOWN_OPS", NO_UNKNOWN_OPS)?;
     m.add("LIMIT_HEAP", LIMIT_HEAP)?;
-    m.add("LIMIT_STACK", LIMIT_STACK)?;
+    m.add("ENABLE_BLS_OPS", ENABLE_BLS_OPS)?;
+    m.add("ENABLE_SECP_OPS", ENABLE_SECP_OPS)?;
+    m.add("ENABLE_BLS_OPS_OUTSIDE_GUARD", ENABLE_BLS_OPS_OUTSIDE_GUARD)?;
+    m.add("LIMIT_OBJECTS", LIMIT_OBJECTS)?;
 
     m.add_function(wrap_pyfunction!(serialized_length, m)?)?;
     m.add_function(wrap_pyfunction!(compute_merkle_set_root, m)?)?;
     m.add_function(wrap_pyfunction!(tree_hash, m)?)?;
     m.add_function(wrap_pyfunction!(get_puzzle_and_solution_for_coin, m)?)?;
 
     compression::add_submodule(py, m)?;
```

### Comparing `chia_rs-0.2.7/src/compression.rs` & `chia_rs-0.2.8/src/compression.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.7/src/run_generator.rs` & `chia_rs-0.2.8/src/run_generator.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 use super::adapt_response::eval_err_to_pyresult;
 use chia_protocol::from_json_dict::FromJsonDict;
 use chia_protocol::to_json_dict::ToJsonDict;
 
+use chia::allocator::make_allocator;
 use chia::gen::conditions::{parse_spends, Spend, SpendBundleConditions};
-use chia::gen::validation_error::{ErrorCode, ValidationErr};
 use chia::gen::run_block_generator::run_block_generator as native_run_block_generator;
+use chia::gen::validation_error::{ErrorCode, ValidationErr};
 use chia_protocol::bytes::{Bytes, Bytes32, Bytes48};
-use chia::allocator::make_allocator;
 
 use clvmr::allocator::Allocator;
 use clvmr::chia_dialect::ChiaDialect;
 use clvmr::cost::Cost;
 use clvmr::reduction::{EvalErr, Reduction};
 use clvmr::run_program::run_program;
 use clvmr::serde::node_from_bytes;
@@ -91,15 +91,18 @@
         birth_seconds: spend.birth_seconds,
         create_coin,
         agg_sig_me: agg_sigs,
         flags: spend.flags,
     }
 }
 
-pub fn convert_spend_bundle_conds(a: &Allocator, sb: SpendBundleConditions) -> PySpendBundleConditions {
+pub fn convert_spend_bundle_conds(
+    a: &Allocator,
+    sb: SpendBundleConditions,
+) -> PySpendBundleConditions {
     let mut spends = Vec::<PySpend>::new();
     for s in sb.spends {
         spends.push(convert_spend(a, s));
     }
 
     let mut agg_sigs = Vec::<(Bytes48, Bytes)>::with_capacity(sb.agg_sig_unsafe.len());
     for (pk, msg) in sb.agg_sig_unsafe {
@@ -126,15 +129,15 @@
 pub fn run_generator(
     py: Python,
     program: &[u8],
     args: &[u8],
     max_cost: Cost,
     flags: u32,
 ) -> PyResult<(Option<u32>, Option<PySpendBundleConditions>)> {
-	let mut allocator = make_allocator(flags);
+    let mut allocator = make_allocator(flags);
     let program = node_from_bytes(&mut allocator, program)?;
     let args = node_from_bytes(&mut allocator, args)?;
     let dialect = &ChiaDialect::new(flags);
 
     let r = py.allow_threads(
         || -> Result<(Option<ErrorCode>, Option<SpendBundleConditions>), EvalErr> {
             let Reduction(cost, node) =
@@ -156,15 +159,15 @@
     match r {
         Ok((None, Some(spend_bundle_conds))) => {
             // everything was successful
             Ok((
                 None,
                 Some(convert_spend_bundle_conds(&allocator, spend_bundle_conds)),
             ))
-        },
+        }
         Ok((error_code, _)) => {
             // a validation error occurred
             Ok((error_code.map(|x| x.into()), None))
         }
         Err(eval_err) => eval_err_to_pyresult(py, eval_err, allocator),
     }
 }
@@ -173,28 +176,28 @@
 pub fn run_block_generator(
     _py: Python,
     program: &[u8],
     block_refs: &PyList,
     max_cost: Cost,
     flags: u32,
 ) -> PyResult<(Option<u32>, Option<PySpendBundleConditions>)> {
-	let mut allocator = make_allocator(flags);
+    let mut allocator = make_allocator(flags);
 
     let mut refs = Vec::<Vec<u8>>::new();
     for g in block_refs {
         refs.push(g.extract::<Vec<u8>>()?);
     }
 
     match native_run_block_generator(&mut allocator, program, &refs, max_cost, flags) {
         Ok(spend_bundle_conds) => {
             // everything was successful
             Ok((
                 None,
                 Some(convert_spend_bundle_conds(&allocator, spend_bundle_conds)),
             ))
-        },
+        }
         Err(ValidationErr(_, error_code)) => {
             // a validation error occurred
             Ok((Some(error_code.into()), None))
         }
     }
 }
```

### Comparing `chia_rs-0.2.7/src/run_program.rs` & `chia_rs-0.2.8/src/run_program.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 use super::adapt_response::eval_err_to_pyresult;
 use chia::allocator::make_allocator;
+use chia::gen::flags::ALLOW_BACKREFS;
 use clvmr::allocator::{Allocator, NodePtr, SExp};
 use clvmr::chia_dialect::ChiaDialect;
 use clvmr::cost::Cost;
 use clvmr::reduction::Response;
 use clvmr::run_program::run_program;
-use clvmr::serde::{node_from_bytes, serialized_length_from_bytes};
+use clvmr::serde::{node_from_bytes, node_from_bytes_backrefs, serialized_length_from_bytes};
 use pyo3::prelude::*;
 use pyo3::types::{PyBytes, PyTuple};
 use std::rc::Rc;
 
 #[pyclass(subclass, unsendable)]
 #[derive(Clone)]
 pub struct LazyNode {
@@ -39,15 +40,15 @@
             _ => Ok(None),
         }
     }
 
     #[getter(atom)]
     pub fn atom(&self, py: Python) -> Option<PyObject> {
         match &self.allocator.sexp(self.node) {
-            SExp::Atom(atom) => Some(PyBytes::new(py, self.allocator.buf(atom)).into()),
+            SExp::Atom() => Some(PyBytes::new(py, self.allocator.atom(self.node)).into()),
             _ => None,
         }
     }
 }
 
 impl LazyNode {
     pub const fn new(a: Rc<Allocator>, n: NodePtr) -> Self {
@@ -72,20 +73,24 @@
     args: &[u8],
     max_cost: Cost,
     flags: u32,
 ) -> PyResult<(Cost, LazyNode)> {
     let mut allocator = make_allocator(flags);
 
     let r: Response = (|| -> PyResult<Response> {
-        let program = node_from_bytes(&mut allocator, program)?;
-        let args = node_from_bytes(&mut allocator, args)?;
+        let deserialize = if (flags & ALLOW_BACKREFS) != 0 {
+            node_from_bytes_backrefs
+        } else {
+            node_from_bytes
+        };
+        let program = deserialize(&mut allocator, program)?;
+        let args = deserialize(&mut allocator, args)?;
         let dialect = ChiaDialect::new(flags);
 
-        Ok(py
-            .allow_threads(|| run_program(&mut allocator, &dialect, program, args, max_cost)))
+        Ok(py.allow_threads(|| run_program(&mut allocator, &dialect, program, args, max_cost)))
     })()?;
     match r {
         Ok(reduction) => {
             let val = LazyNode::new(Rc::new(allocator), reduction.1);
             Ok((reduction.0, val))
         }
         Err(eval_err) => eval_err_to_pyresult(py, eval_err, allocator),
```

### Comparing `chia_rs-0.2.7/Cargo.lock` & `chia_rs-0.2.8/Cargo.lock`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,26 @@
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "base16ct"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4c7f02d4ea65f2c1853089ffd8d2787bdbc63de2f0d29dedbcf8ccdfa0ccd4cf"
+
+[[package]]
+name = "base64ct"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitvec"
@@ -24,74 +36,91 @@
  "radium",
  "tap",
  "wyz",
 ]
 
 [[package]]
 name = "block-buffer"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4152116fd6e9dadb291ae18fc1ec3575ed6d84c29642d97890f4b4a3417297e4"
+dependencies = [
+ "generic-array",
+]
+
+[[package]]
+name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bls12_381"
-version = "0.7.0"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62250ece575fa9b22068b3a8d59586f01d426dd7785522efd97632959e71c986"
+checksum = "d7bc6d6292be3a19e6379786dac800f551e5865a5bb51ebbe3064ab80433f403"
 dependencies = [
+ "digest 0.9.0",
  "ff",
  "group",
  "pairing",
  "rand_core",
  "subtle",
 ]
 
 [[package]]
+name = "bumpalo"
+version = "3.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chia"
-version = "0.2.7"
+version = "0.2.8"
 dependencies = [
  "chia-protocol",
  "clvm-utils",
  "clvmr",
  "hex",
+ "hex-literal",
  "pyo3",
 ]
 
 [[package]]
 name = "chia-protocol"
 version = "0.2.7"
 dependencies = [
  "chia_py_streamable_macro",
  "chia_streamable_macro",
  "clvmr",
  "hex",
  "pyo3",
- "sha2",
+ "sha2 0.9.9",
 ]
 
 [[package]]
 name = "chia_py_streamable_macro"
 version = "0.1.3"
 dependencies = [
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "chia_rs"
-version = "0.2.7"
+version = "0.2.8"
 dependencies = [
  "chia",
  "chia-protocol",
  "chia_py_streamable_macro",
  "chia_streamable_macro",
  "clvmr",
  "hex",
@@ -99,49 +128,71 @@
 ]
 
 [[package]]
 name = "chia_streamable_macro"
 version = "0.2.4"
 dependencies = [
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "clvm-utils"
 version = "0.2.7"
 dependencies = [
  "clvmr",
 ]
 
 [[package]]
 name = "clvmr"
-version = "0.2.4"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93dfa322573fe20cb086a246f5d5f064d2b3c1cb7ea5b6b7687a0cbddac20bd7"
+checksum = "83afaa6d5081706f202d31ed08ddb2425c902ca968d9832429bcdf9474ca6c9f"
 dependencies = [
  "bls12_381",
+ "getrandom",
+ "group",
  "hex",
+ "k256",
  "lazy_static",
  "num-bigint",
  "num-integer",
  "num-traits",
- "sha2",
+ "p256",
+ "sha2 0.9.9",
 ]
 
 [[package]]
+name = "const-oid"
+version = "0.9.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "520fbf3c07483f94e3e3ca9d0cfd913d7718ef2483d2cfd91c0d9e91474ab913"
+
+[[package]]
 name = "cpufeatures"
-version = "0.2.7"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
+checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "crypto-bigint"
+version = "0.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cf4c2f4e1afd912bc40bfd6fed5d9dc1f288e0ba01bfcc835cc5bc3eb13efe15"
+dependencies = [
+ "generic-array",
+ "rand_core",
+ "subtle",
+ "zeroize",
+]
+
+[[package]]
 name = "crypto-common"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
@@ -154,28 +205,84 @@
 checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
 dependencies = [
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "der"
+version = "0.7.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "56acb310e15652100da43d130af8d97b509e95af61aab1c5a7939ef24337ee17"
+dependencies = [
+ "const-oid",
+ "pem-rfc7468",
+ "zeroize",
+]
+
+[[package]]
+name = "digest"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d3dd60d1080a57a05ab032377049e0591415d2b31afd7028356dbf3cc6dcb066"
+dependencies = [
+ "generic-array",
+]
+
+[[package]]
 name = "digest"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
- "block-buffer",
+ "block-buffer 0.10.4",
+ "const-oid",
  "crypto-common",
+ "subtle",
+]
+
+[[package]]
+name = "ecdsa"
+version = "0.16.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0997c976637b606099b9985693efa3581e84e41f5c11ba5255f88711058ad428"
+dependencies = [
+ "der",
+ "digest 0.10.7",
+ "elliptic-curve",
+ "rfc6979",
+ "signature",
+ "spki",
+]
+
+[[package]]
+name = "elliptic-curve"
+version = "0.13.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "968405c8fdc9b3bf4df0a6638858cc0b52462836ab6b1c87377785dd09cf1c0b"
+dependencies = [
+ "base16ct",
+ "crypto-bigint",
+ "digest 0.10.7",
+ "ff",
+ "generic-array",
+ "group",
+ "pem-rfc7468",
+ "pkcs8",
+ "rand_core",
+ "sec1",
+ "subtle",
+ "zeroize",
 ]
 
 [[package]]
 name = "ff"
-version = "0.12.1"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d013fc25338cc558c5c2cfbad646908fb23591e2404481826742b651c9af7160"
+checksum = "ded41244b729663b1e574f1b4fb731469f69f79c17667b5d776b16cda0479449"
 dependencies = [
  "bitvec",
  "rand_core",
  "subtle",
 ]
 
 [[package]]
@@ -188,45 +295,74 @@
 name = "generic-array"
 version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
+ "zeroize",
+]
+
+[[package]]
+name = "getrandom"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+dependencies = [
+ "cfg-if",
+ "js-sys",
+ "libc",
+ "wasi",
+ "wasm-bindgen",
 ]
 
 [[package]]
 name = "ghost"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e77ac7b51b8e6313251737fcef4b1c01a2ea102bde68415b62c0ee9268fec357"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "group"
-version = "0.12.1"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5dfbfb3a6cfbd390d5c9564ab283a0349b9b9fcd46a706c1eb10e0db70bfbac7"
+checksum = "f0f9ef7462f7c099f518d754361858f86d8a07af53ba9af0fe635bbccb151a63"
 dependencies = [
  "ff",
  "rand_core",
  "subtle",
 ]
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
+name = "hex-literal"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6fe2267d4ed49bc07b63801559be28c718ea06c4738b7a03c94df7386d2cde46"
+
+[[package]]
+name = "hmac"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
+dependencies = [
+ "digest 0.10.7",
+]
+
+[[package]]
 name = "indoc"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "47741a8bc60fb26eb8d6e0238bbb26d8575ff623fdc97b1a2c00c050b9684ed8"
 dependencies = [
  "indoc-impl",
  "proc-macro-hack",
@@ -273,36 +409,65 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "js-sys"
+version = "0.3.64"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
+dependencies = [
+ "wasm-bindgen",
+]
+
+[[package]]
+name = "k256"
+version = "0.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cadb76004ed8e97623117f3df85b17aaa6626ab0b0831e6573f104df16cd1bcc"
+dependencies = [
+ "cfg-if",
+ "ecdsa",
+ "elliptic-curve",
+ "once_cell",
+ "sha2 0.10.7",
+ "signature",
+]
+
+[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.142"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
+name = "log"
+version = "0.4.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
+
+[[package]]
 name = "num-bigint"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
 dependencies = [
  "autocfg",
  "num-integer",
@@ -326,23 +491,41 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+
+[[package]]
+name = "opaque-debug"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
+
+[[package]]
+name = "p256"
+version = "0.13.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c9863ad85fa8f4460f9c48cb909d38a0d689dba1f6f6988a5e3e0d31071bcd4b"
+dependencies = [
+ "ecdsa",
+ "elliptic-curve",
+ "primeorder",
+ "sha2 0.10.7",
+]
 
 [[package]]
 name = "pairing"
-version = "0.22.0"
+version = "0.23.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "135590d8bdba2b31346f9cd1fb2a912329f5135e832a4f422942eb6ead8b6b3b"
+checksum = "81fec4625e73cf41ef4bb6846cafa6d44736525f442ba45e407c4a000a13996f"
 dependencies = [
  "group",
 ]
 
 [[package]]
 name = "parking_lot"
 version = "0.11.2"
@@ -384,24 +567,52 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d95a7db200b97ef370c8e6de0088252f7e0dfff7d047a28528e47456c0fc98b6"
 dependencies = [
  "proc-macro-hack",
 ]
 
 [[package]]
+name = "pem-rfc7468"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88b39c9bfcfc231068454382784bb460aae594343fb030d46e9f50a645418412"
+dependencies = [
+ "base64ct",
+]
+
+[[package]]
+name = "pkcs8"
+version = "0.10.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f950b2377845cebe5cf8b5165cb3cc1a5e0fa5cfa3e1f7f55707d8fd82e0a7b7"
+dependencies = [
+ "der",
+ "spki",
+]
+
+[[package]]
+name = "primeorder"
+version = "0.13.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c2fcef82c0ec6eefcc179b978446c399b3cdf73c392c35604e399eee6df1ee3"
+dependencies = [
+ "elliptic-curve",
+]
+
+[[package]]
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.15.1"
@@ -449,17 +660,17 @@
  "pyo3-build-config",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -467,48 +678,108 @@
 checksum = "dc33ff2d4973d518d823d61aa239014831e521c75da58e3df4840d3f47749d09"
 
 [[package]]
 name = "rand_core"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
+dependencies = [
+ "getrandom",
+]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "rfc6979"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8dd2a808d456c4a54e300a23e9f5a67e122c3024119acbfd73e3bf664491cb2"
+dependencies = [
+ "hmac",
+ "subtle",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
+name = "sec1"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f0aec48e813d6b90b15f0b8948af3c63483992dee44c03e9930b3eebdabe046e"
+dependencies = [
+ "base16ct",
+ "der",
+ "generic-array",
+ "pkcs8",
+ "subtle",
+ "zeroize",
+]
+
+[[package]]
 name = "sha2"
-version = "0.10.2"
+version = "0.9.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4d58a1e1bf39749807d89cf2d98ac2dfa0ff1cb3faa38fbb64dd88ac8013d800"
+dependencies = [
+ "block-buffer 0.9.0",
+ "cfg-if",
+ "cpufeatures",
+ "digest 0.9.0",
+ "opaque-debug",
+]
+
+[[package]]
+name = "sha2"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "55deaec60f81eefe3cce0dc50bda92d6d8e88f2a27df7c5033b42afeb1ed2676"
+checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
 dependencies = [
  "cfg-if",
  "cpufeatures",
- "digest",
+ "digest 0.10.7",
+]
+
+[[package]]
+name = "signature"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5e1788eed21689f9cf370582dfc467ef36ed9c707f073528ddafa8d83e3b8500"
+dependencies = [
+ "digest 0.10.7",
+ "rand_core",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
+name = "spki"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d1e996ef02c474957d681f1b05213dfb0abab947b446a62d37770b23500184a"
+dependencies = [
+ "base64ct",
+ "der",
+]
+
+[[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
@@ -519,17 +790,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -542,31 +813,91 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
+name = "wasi"
+version = "0.11.0+wasi-snapshot-preview1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
+
+[[package]]
+name = "wasm-bindgen"
+version = "0.2.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+dependencies = [
+ "cfg-if",
+ "wasm-bindgen-macro",
+]
+
+[[package]]
+name = "wasm-bindgen-backend"
+version = "0.2.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+dependencies = [
+ "bumpalo",
+ "log",
+ "once_cell",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-macro"
+version = "0.2.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+dependencies = [
+ "quote",
+ "wasm-bindgen-macro-support",
+]
+
+[[package]]
+name = "wasm-bindgen-macro-support"
+version = "0.2.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.18",
+ "wasm-bindgen-backend",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-shared"
+version = "0.2.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -588,7 +919,13 @@
 name = "wyz"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
  "tap",
 ]
+
+[[package]]
+name = "zeroize"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
```

