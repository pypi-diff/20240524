# Comparing `tmp/quantum_pecos-0.6.0.dev2.tar.gz` & `tmp/quantum_pecos-0.6.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantum_pecos-0.6.0.dev2.tar", last modified: Mon May 20 17:24:01 2024, max compression
+gzip compressed data, was "quantum_pecos-0.6.0.dev3.tar", last modified: Fri May 24 16:22:22 2024, max compression
```

## Comparing `quantum_pecos-0.6.0.dev2.tar` & `quantum_pecos-0.6.0.dev3.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.268051 quantum_pecos-0.6.0.dev2/
--rw-rw-rw-   0        0        0    11560 2024-02-18 00:34:34.000000 quantum_pecos-0.6.0.dev2/LICENSE
--rw-rw-rw-   0        0        0      136 2024-02-18 00:34:34.000000 quantum_pecos-0.6.0.dev2/MANIFEST.in
--rw-rw-rw-   0        0        0      463 2024-02-18 00:34:34.000000 quantum_pecos-0.6.0.dev2/NOTICE
--rw-rw-rw-   0        0        0    20885 2024-05-20 17:24:01.267551 quantum_pecos-0.6.0.dev2/PKG-INFO
--rw-rw-rw-   0        0        0     5198 2024-03-10 03:52:18.000000 quantum_pecos-0.6.0.dev2/README.md
--rw-rw-rw-   0        0        0     3267 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.095383 quantum_pecos-0.6.0.dev2/python/
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.099883 quantum_pecos-0.6.0.dev2/python/pecos/
--rw-rw-rw-   0        0        0     1907 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.102387 quantum_pecos-0.6.0.dev2/python/pecos/circuit_converters/
--rw-rw-rw-   0        0        0      942 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuit_converters/__init__.py
--rw-rw-rw-   0        0        0     9739 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuit_converters/checks2circuit.py
--rw-rw-rw-   0        0        0     5302 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuit_converters/std2chs.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.105888 quantum_pecos-0.6.0.dev2/python/pecos/circuits/
--rw-rw-rw-   0        0        0      911 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.112391 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/
--rw-rw-rw-   0        0        0      671 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/__init__.py
--rw-rw-rw-   0        0        0     1437 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/conditionals.py
--rw-rw-rw-   0        0        0     1708 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/cops.py
--rw-rw-rw-   0        0        0     1086 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/fund.py
--rw-rw-rw-   0        0        0     1225 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/hyqc.py
--rw-rw-rw-   0        0        0     2830 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/int.py
--rw-rw-rw-   0        0        0     1302 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/misc_stmts.py
--rw-rw-rw-   0        0        0     5680 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/qops.py
--rw-rw-rw-   0        0        0     1513 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/qubits.py
--rw-rw-rw-   0        0        0     1200 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/vars.py
--rw-rw-rw-   0        0        0     5033 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/logical_circuit.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.119896 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/
--rw-rw-rw-   0        0        0     1028 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/__init__.py
--rw-rw-rw-   0        0        0      852 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/barrier.py
--rw-rw-rw-   0        0        0     1070 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/block.py
--rw-rw-rw-   0        0        0     2283 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/conditionals.py
--rw-rw-rw-   0        0        0     2020 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/expr.py
--rw-rw-rw-   0        0        0      935 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/func.py
--rw-rw-rw-   0        0        0     6986 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/gates.py
--rw-rw-rw-   0        0        0     1592 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/misc.py
--rw-rw-rw-   0        0        0     5616 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/qasm.py
--rw-rw-rw-   0        0        0     1252 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/std_gates.py
--rw-rw-rw-   0        0        0     2312 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/vars.py
--rw-rw-rw-   0        0        0     9989 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/qc2phir.py
--rw-rw-rw-   0        0        0    14990 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/circuits/quantum_circuit.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.121973 quantum_pecos-0.6.0.dev2/python/pecos/classical_interpreters/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/classical_interpreters/__init__.py
--rw-rw-rw-   0        0        0     1513 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/classical_interpreters/classical_interpreter_abc.py
--rw-rw-rw-   0        0        0    12692 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/classical_interpreters/phir_classical_interpreter.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.122900 quantum_pecos-0.6.0.dev2/python/pecos/decoders/
--rw-rw-rw-   0        0        0      872 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/decoders/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.124399 quantum_pecos-0.6.0.dev2/python/pecos/decoders/dummy_decoder/
--rw-rw-rw-   0        0        0      794 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/decoders/dummy_decoder/__init__.py
--rw-rw-rw-   0        0        0     1171 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/decoders/dummy_decoder/dummy_decoder.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.126399 quantum_pecos-0.6.0.dev2/python/pecos/decoders/mwpm2d/
--rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/decoders/mwpm2d/__init__.py
--rw-rw-rw-   0        0        0     5211 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/decoders/mwpm2d/mwpm2d.py
--rw-rw-rw-   0        0        0    17301 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/decoders/mwpm2d/precomputing.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.128899 quantum_pecos-0.6.0.dev2/python/pecos/engines/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.130900 quantum_pecos-0.6.0.dev2/python/pecos/engines/circuit_runners/
--rw-rw-rw-   0        0        0      885 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/circuit_runners/__init__.py
--rw-rw-rw-   0        0        0     3508 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/circuit_runners/standard.py
--rw-rw-rw-   0        0        0     2385 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/circuit_runners/timing_runner.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.135404 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/__init__.py
--rw-rw-rw-   0        0        0     8608 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/binarray.py
--rw-rw-rw-   0        0        0     5391 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/binarray2.py
--rw-rw-rw-   0        0        0     7544 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/classical.py
--rw-rw-rw-   0        0        0     1738 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/cvm.py
--rw-rw-rw-   0        0        0     1661 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/sim_func.py
--rw-rw-rw-   0        0        0     4353 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.138404 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/__init__.py
--rw-rw-rw-   0        0        0     1654 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/pywasm.py
--rw-rw-rw-   0        0        0     1180 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/pywasm3.py
--rw-rw-rw-   0        0        0     2728 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/wasmer.py
--rw-rw-rw-   0        0        0     1634 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/wasmtime.py
--rw-rw-rw-   0        0        0     7574 2024-04-29 19:48:00.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/hybrid_engine.py
--rw-rw-rw-   0        0        0     4968 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/hybrid_engine_multiprocessing.py
--rw-rw-rw-   0        0        0     8562 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/engines/hybrid_engine_old.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.144908 quantum_pecos-0.6.0.dev2/python/pecos/error_models/
--rw-rw-rw-   0        0        0     1109 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/__init__.py
--rw-rw-rw-   0        0        0     1849 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/class_errors_circuit.py
--rw-rw-rw-   0        0        0     5704 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/depolarizing_error_model.py
--rw-rw-rw-   0        0        0     5604 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/error_depolar.py
--rw-rw-rw-   0        0        0     1768 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/error_model.py
--rw-rw-rw-   0        0        0     1368 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/error_model_abc.py
--rw-rw-rw-   0        0        0     1035 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/fake_error_model.py
--rw-rw-rw-   0        0        0     5851 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/generic_error_model.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.151908 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/__init__.py
--rw-rw-rw-   0        0        0      958 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_initz_bitflip.py
--rw-rw-rw-   0        0        0     1435 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_initz_bitflip_leakage.py
--rw-rw-rw-   0        0        0     1450 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_meas_bitflip.py
--rw-rw-rw-   0        0        0     1621 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_meas_bitflip_leakage.py
--rw-rw-rw-   0        0        0     1196 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_sq_bitflip.py
--rw-rw-rw-   0        0        0     1488 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_sq_depolarizing.py
--rw-rw-rw-   0        0        0     1958 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_sq_depolarizing_leakage.py
--rw-rw-rw-   0        0        0     1761 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_tq_depolarizing.py
--rw-rw-rw-   0        0        0     2490 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_tq_depolarizing_leakage.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.157913 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/__init__.py
--rw-rw-rw-   0        0        0     2546 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/gate_groups.py
--rw-rw-rw-   0        0        0     1385 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/init_noise.py
--rw-rw-rw-   0        0        0     1593 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/meas_noise.py
--rw-rw-rw-   0        0        0     1337 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/memory_noise.py
--rw-rw-rw-   0        0        0     1207 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/sq_noise.py
--rw-rw-rw-   0        0        0     2943 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/tq_noise.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.161914 quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/
--rw-rw-rw-   0        0        0      791 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/__init__.py
--rw-rw-rw-   0        0        0     7653 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/depolar_gen.py
--rw-rw-rw-   0        0        0     5732 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/gatewise_gen.py
--rw-rw-rw-   0        0        0     6255 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/xerror_gen.py
--rw-rw-rw-   0        0        0     7322 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/xzerror_gen.py
--rw-rw-rw-   0        0        0     6255 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/zerror_gen.py
--rw-rw-rw-   0        0        0    11841 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/parent_class_error_gen.py
--rw-rw-rw-   0        0        0     5100 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/error_models/simple_depolarizing_error_model.py
--rw-rw-rw-   0        0        0     1026 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.166419 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/__init__.py
--rw-rw-rw-   0        0        0     1304 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/foreign_object_abc.py
--rw-rw-rw-   0        0        0     2466 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/object_pool.py
--rw-rw-rw-   0        0        0     1168 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/python.py
--rw-rw-rw-   0        0        0      527 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/wasm_execution_timer_thread.py
--rw-rw-rw-   0        0        0     3837 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/wasmer.py
--rw-rw-rw-   0        0        0     5054 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/wasmtime.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.168418 quantum_pecos-0.6.0.dev2/python/pecos/machines/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/machines/__init__.py
--rw-rw-rw-   0        0        0     2356 2024-04-29 19:48:00.000000 quantum_pecos-0.6.0.dev2/python/pecos/machines/generic_machine.py
--rw-rw-rw-   0        0        0     1591 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/machines/machine_abc.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.173419 quantum_pecos-0.6.0.dev2/python/pecos/misc/
--rw-rw-rw-   0        0        0      840 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/__init__.py
--rw-rw-rw-   0        0        0     2240 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/commute.py
--rw-rw-rw-   0        0        0      838 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/errors.py
--rw-rw-rw-   0        0        0     1681 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/gate_groups.py
--rw-rw-rw-   0        0        0    10545 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/stabilizer_funcs.py
--rw-rw-rw-   0        0        0     1992 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/std_output.py
--rw-rw-rw-   0        0        0     3552 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/symbol_library.py
--rw-rw-rw-   0        0        0     7419 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/misc/threshold_curve.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.175423 quantum_pecos-0.6.0.dev2/python/pecos/op_processors/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/op_processors/__init__.py
--rw-rw-rw-   0        0        0     2266 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/op_processors/generic_op_processor.py
--rw-rw-rw-   0        0        0     1132 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/op_processors/op_processor_abc.py
--rw-rw-rw-   0        0        0        0 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.179423 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/
--rw-rw-rw-   0        0        0     1147 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.182923 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/
--rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/__init__.py
--rw-rw-rw-   0        0        0     7774 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/circuit_implementation1.py
--rw-rw-rw-   0        0        0     7702 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/color_488.py
--rw-rw-rw-   0        0        0     3276 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/gates.py
--rw-rw-rw-   0        0        0     8975 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/instructions.py
--rw-rw-rw-   0        0        0     3576 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/gate_parent_class.py
--rw-rw-rw-   0        0        0     2262 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/helper_functions.py
--rw-rw-rw-   0        0        0     3845 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/instruction_parent_class.py
--rw-rw-rw-   0        0        0     7751 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/plot.py
--rw-rw-rw-   0        0        0     8065 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/qecc_parent_class.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.185928 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/
--rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/__init__.py
--rw-rw-rw-   0        0        0     3276 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/gates.py
--rw-rw-rw-   0        0        0    11245 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/instructions.py
--rw-rw-rw-   0        0        0     9623 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/surface_4444.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.188428 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/
--rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/__init__.py
--rw-rw-rw-   0        0        0     3276 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/gates.py
--rw-rw-rw-   0        0        0    19744 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/instructions.py
--rw-rw-rw-   0        0        0    10241 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/surface_medial_4444.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.188928 quantum_pecos-0.6.0.dev2/python/pecos/reps/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.194428 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/
--rw-rw-rw-   0        0        0      675 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/__init__.py
--rw-rw-rw-   0        0        0     1844 2024-04-29 19:48:00.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/block_types.py
--rw-rw-rw-   0        0        0     1961 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/data_types.py
--rw-rw-rw-   0        0        0      236 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/instr_type.py
--rw-rw-rw-   0        0        0     1104 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/list_types.py
--rw-rw-rw-   0        0        0     1103 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/name_resolver.py
--rw-rw-rw-   0        0        0     3167 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/op_types.py
--rw-rw-rw-   0        0        0    10789 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/pypmir.py
--rw-rw-rw-   0        0        0      812 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/types.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.198434 quantum_pecos-0.6.0.dev2/python/pecos/simulators/
--rw-rw-rw-   0        0        0     1878 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.201435 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/
--rw-rw-rw-   0        0        0      692 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/__init__.py
--rw-rw-rw-   0        0        0     1661 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/bindings.py
--rw-rw-rw-   0        0        0     1196 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/gates.py
--rw-rw-rw-   0        0        0     1773 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/state.py
--rw-rw-rw-   0        0        0     2185 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/compile_cython.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.202934 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/
--rw-rw-rw-   0        0        0      698 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/__init__.py
--rw-rw-rw-   0        0        0      776 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuconn.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.203434 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/
--rw-rw-rw-   0        0        0      692 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.204934 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/
--rw-rw-rw-   0        0        0      624 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/__init__.py
--rw-rw-rw-   0        0        0     4489 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/test_python_bindings.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.208938 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/
--rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/__init__.py
--rw-rw-rw-   0        0        0     2010 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/bindings.py
--rw-rw-rw-   0        0        0     1046 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_init.py
--rw-rw-rw-   0        0        0      785 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_meas.py
--rw-rw-rw-   0        0        0     3562 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_sq.py
--rw-rw-rw-   0        0        0     1200 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_tq.py
--rw-rw-rw-   0        0        0     1874 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/state.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.213939 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/
--rw-rw-rw-   0        0        0      698 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/__init__.py
--rw-rw-rw-   0        0        0     1769 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/bindings.py
--rw-rw-rw-   0        0        0     1046 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_init.py
--rw-rw-rw-   0        0        0     1867 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_meas.py
--rw-rw-rw-   0        0        0     9594 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_one_qubit.py
--rw-rw-rw-   0        0        0    12354 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_two_qubit.py
--rw-rw-rw-   0        0        0     3719 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/state.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.214939 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/
--rw-rw-rw-   0        0        0      857 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/__init__.py
--rw-rw-rw-   0        0        0     2191 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.215438 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/src/
--rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/src/__init__.py
--rw-rw-rw-   0        0        0     6362 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/src/logical_sign.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.218021 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/
--rw-rw-rw-   0        0        0      857 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/__init__.py
--rw-rw-rw-   0        0        0     1983 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.219527 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/src/
--rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/src/__init__.py
--rw-rw-rw-   0        0        0     6090 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/src/logical_sign.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.221031 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/
--rw-rw-rw-   0        0        0      857 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/__init__.py
--rw-rw-rw-   0        0        0     1983 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.222531 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/src/
--rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/src/__init__.py
--rw-rw-rw-   0        0        0     6090 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/src/logical_sign.py
--rw-rw-rw-   0        0        0     2736 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/gate_syms.py
--rw-rw-rw-   0        0        0     2691 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/parent_sim_classes.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.228036 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/
--rw-rw-rw-   0        0        0      710 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/__init__.py
--rw-rw-rw-   0        0        0     2945 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/bindings.py
--rw-rw-rw-   0        0        0      881 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_init.py
--rw-rw-rw-   0        0        0     2985 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_meas.py
--rw-rw-rw-   0        0        0    14031 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_one_qubit.py
--rw-rw-rw-   0        0        0     7900 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_two_qubit.py
--rw-rw-rw-   0        0        0     1738 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/logical_sign.py
--rw-rw-rw-   0        0        0     9712 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/state.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.234536 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/
--rw-rw-rw-   0        0        0      859 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/__init__.py
--rw-rw-rw-   0        0        0     4891 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/bindings.py
--rw-rw-rw-   0        0        0     2213 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_init.py
--rw-rw-rw-   0        0        0     2631 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_meas.py
--rw-rw-rw-   0        0        0     6819 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_one_qubit.py
--rw-rw-rw-   0        0        0     4884 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_two_qubit.py
--rw-rw-rw-   0        0        0     1205 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/helper.py
--rw-rw-rw-   0        0        0     2379 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/logical_sign.py
--rw-rw-rw-   0        0        0     4977 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/state.py
--rw-rw-rw-   0        0        0     2885 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/quantum_simulator.py
--rw-rw-rw-   0        0        0     1409 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sim_class_types.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.240541 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/
--rw-rw-rw-   0        0        0     1933 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/__init__.py
--rw-rw-rw-   0        0        0     2909 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/bindings.py
--rw-rw-rw-   0        0        0     3225 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_init.py
--rw-rw-rw-   0        0        0    11606 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_meas.py
--rw-rw-rw-   0        0        0    33702 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_one_qubit.py
--rw-rw-rw-   0        0        0    15954 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_two_qubit.py
--rw-rw-rw-   0        0        0     8070 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/logical_sign.py
--rw-rw-rw-   0        0        0     5143 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/refactor.py
--rw-rw-rw-   0        0        0    17202 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/state.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.246541 quantum_pecos-0.6.0.dev2/python/pecos/slr/
--rw-rw-rw-   0        0        0     1170 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/__init__.py
--rw-rw-rw-   0        0        0     2062 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/block.py
--rw-rw-rw-   0        0        0     2688 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/cond_block.py
--rw-rw-rw-   0        0        0     3124 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/cops.py
--rw-rw-rw-   0        0        0      799 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/fund.py
--rw-rw-rw-   0        0        0     3541 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/misc.py
--rw-rw-rw-   0        0        0     1883 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/slr.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.247041 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/
--rw-rw-rw-   0        0        0        0 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.254046 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/
--rw-rw-rw-   0        0        0      903 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/__init__.py
--rw-rw-rw-   0        0        0      794 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/cliffords_tq.py
--rw-rw-rw-   0        0        0     1664 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/face_rots.py
--rw-rw-rw-   0        0        0      126 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/hadamards.py
--rw-rw-rw-   0        0        0     4539 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/metaclasses.py
--rw-rw-rw-   0        0        0      297 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/misc.py
--rw-rw-rw-   0        0        0     1272 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/paulis.py
--rw-rw-rw-   0        0        0      870 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/projective.py
--rw-rw-rw-   0        0        0      381 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/rots.py
--rw-rw-rw-   0        0        0      603 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/sqrt_paulis.py
--rw-rw-rw-   0        0        0      878 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/util.py
--rw-rw-rw-   0        0        0     3530 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/slr/vars.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.262051 quantum_pecos-0.6.0.dev2/python/pecos/tools/
--rw-rw-rw-   0        0        0     1319 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/__init__.py
--rw-rw-rw-   0        0        0     6558 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/fault_tolerance_checking.py
--rw-rw-rw-   0        0        0    13635 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/fault_tolerance_checks.py
--rw-rw-rw-   0        0        0     5829 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/find_cliffs.py
--rw-rw-rw-   0        0        0     3384 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/logic_circuit_speed.py
--rw-rw-rw-   0        0        0     7186 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/pseudo_threshold_tools.py
--rw-rw-rw-   0        0        0     3630 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/random_circuit_speed.py
--rw-rw-rw-   0        0        0    32511 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/stabilizer_verification.py
--rw-rw-rw-   0        0        0    17415 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/threshold_tools.py
--rw-rw-rw-   0        0        0     1465 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/tool_anticommute.py
--rw-rw-rw-   0        0        0     6963 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/tools/tool_collection.py
--rw-rw-rw-   0        0        0     3802 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev2/python/pecos/typed_list.py
-drwxrwxrwx   0        0        0        0 2024-05-20 17:24:01.266051 quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/
--rw-rw-rw-   0        0        0    20885 2024-05-20 17:24:01.000000 quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11045 2024-05-20 17:24:01.000000 quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 17:24:01.000000 quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-15 23:26:47.000000 quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      487 2024-05-20 17:24:01.000000 quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-20 17:24:01.000000 quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      741 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 17:24:01.268051 quantum_pecos-0.6.0.dev2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.706280 quantum_pecos-0.6.0.dev3/
+-rw-rw-rw-   0        0        0    11560 2024-02-18 00:34:34.000000 quantum_pecos-0.6.0.dev3/LICENSE
+-rw-rw-rw-   0        0        0      136 2024-02-18 00:34:34.000000 quantum_pecos-0.6.0.dev3/MANIFEST.in
+-rw-rw-rw-   0        0        0      463 2024-02-18 00:34:34.000000 quantum_pecos-0.6.0.dev3/NOTICE
+-rw-rw-rw-   0        0        0    20937 2024-05-24 16:22:22.706280 quantum_pecos-0.6.0.dev3/PKG-INFO
+-rw-rw-rw-   0        0        0     5198 2024-03-10 03:52:18.000000 quantum_pecos-0.6.0.dev3/README.md
+-rw-rw-rw-   0        0        0     3294 2024-05-24 16:16:18.000000 quantum_pecos-0.6.0.dev3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.556133 quantum_pecos-0.6.0.dev3/python/
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.560640 quantum_pecos-0.6.0.dev3/python/pecos/
+-rw-rw-rw-   0        0        0     1907 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev3/python/pecos/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.563145 quantum_pecos-0.6.0.dev3/python/pecos/circuit_converters/
+-rw-rw-rw-   0        0        0      942 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuit_converters/__init__.py
+-rw-rw-rw-   0        0        0     9739 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuit_converters/checks2circuit.py
+-rw-rw-rw-   0        0        0     5302 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuit_converters/std2chs.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.565145 quantum_pecos-0.6.0.dev3/python/pecos/circuits/
+-rw-rw-rw-   0        0        0      911 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.571150 quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/
+-rw-rw-rw-   0        0        0      671 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/__init__.py
+-rw-rw-rw-   0        0        0     1437 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/conditionals.py
+-rw-rw-rw-   0        0        0     1708 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/cops.py
+-rw-rw-rw-   0        0        0     1086 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/fund.py
+-rw-rw-rw-   0        0        0     1225 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/hyqc.py
+-rw-rw-rw-   0        0        0     2830 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/int.py
+-rw-rw-rw-   0        0        0     1302 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/misc_stmts.py
+-rw-rw-rw-   0        0        0     5680 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/qops.py
+-rw-rw-rw-   0        0        0     1513 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/qubits.py
+-rw-rw-rw-   0        0        0     1200 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/vars.py
+-rw-rw-rw-   0        0        0     5033 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/logical_circuit.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.577655 quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/
+-rw-rw-rw-   0        0        0     1028 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/__init__.py
+-rw-rw-rw-   0        0        0      852 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/barrier.py
+-rw-rw-rw-   0        0        0     1070 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/block.py
+-rw-rw-rw-   0        0        0     2283 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/conditionals.py
+-rw-rw-rw-   0        0        0     2020 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/expr.py
+-rw-rw-rw-   0        0        0      935 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/func.py
+-rw-rw-rw-   0        0        0     6986 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/gates.py
+-rw-rw-rw-   0        0        0     1592 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/misc.py
+-rw-rw-rw-   0        0        0     5616 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/qasm.py
+-rw-rw-rw-   0        0        0     1252 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/std_gates.py
+-rw-rw-rw-   0        0        0     2312 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/vars.py
+-rw-rw-rw-   0        0        0     9989 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/qc2phir.py
+-rw-rw-rw-   0        0        0    14990 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/circuits/quantum_circuit.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.579656 quantum_pecos-0.6.0.dev3/python/pecos/classical_interpreters/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/classical_interpreters/__init__.py
+-rw-rw-rw-   0        0        0     1513 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/classical_interpreters/classical_interpreter_abc.py
+-rw-rw-rw-   0        0        0    12692 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev3/python/pecos/classical_interpreters/phir_classical_interpreter.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.580155 quantum_pecos-0.6.0.dev3/python/pecos/decoders/
+-rw-rw-rw-   0        0        0      872 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/decoders/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.581157 quantum_pecos-0.6.0.dev3/python/pecos/decoders/dummy_decoder/
+-rw-rw-rw-   0        0        0      794 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/decoders/dummy_decoder/__init__.py
+-rw-rw-rw-   0        0        0     1171 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/decoders/dummy_decoder/dummy_decoder.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.583166 quantum_pecos-0.6.0.dev3/python/pecos/decoders/mwpm2d/
+-rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/decoders/mwpm2d/__init__.py
+-rw-rw-rw-   0        0        0     5211 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/decoders/mwpm2d/mwpm2d.py
+-rw-rw-rw-   0        0        0    17301 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/decoders/mwpm2d/precomputing.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.585665 quantum_pecos-0.6.0.dev3/python/pecos/engines/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.587165 quantum_pecos-0.6.0.dev3/python/pecos/engines/circuit_runners/
+-rw-rw-rw-   0        0        0      885 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/circuit_runners/__init__.py
+-rw-rw-rw-   0        0        0     3508 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/circuit_runners/standard.py
+-rw-rw-rw-   0        0        0     2385 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/circuit_runners/timing_runner.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.590665 quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/__init__.py
+-rw-rw-rw-   0        0        0     8608 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/binarray.py
+-rw-rw-rw-   0        0        0     5391 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/binarray2.py
+-rw-rw-rw-   0        0        0     7544 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/classical.py
+-rw-rw-rw-   0        0        0     1738 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/cvm.py
+-rw-rw-rw-   0        0        0     1661 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/sim_func.py
+-rw-rw-rw-   0        0        0     4353 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/wasm.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.593674 quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/wasm_vms/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/wasm_vms/__init__.py
+-rw-rw-rw-   0        0        0     1654 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/wasm_vms/pywasm.py
+-rw-rw-rw-   0        0        0     1180 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/wasm_vms/pywasm3.py
+-rw-rw-rw-   0        0        0     2728 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/wasm_vms/wasmer.py
+-rw-rw-rw-   0        0        0     1634 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/wasm_vms/wasmtime.py
+-rw-rw-rw-   0        0        0     7574 2024-04-29 19:48:00.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/hybrid_engine.py
+-rw-rw-rw-   0        0        0     4968 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/hybrid_engine_multiprocessing.py
+-rw-rw-rw-   0        0        0     8562 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev3/python/pecos/engines/hybrid_engine_old.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.599675 quantum_pecos-0.6.0.dev3/python/pecos/error_models/
+-rw-rw-rw-   0        0        0     1109 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/__init__.py
+-rw-rw-rw-   0        0        0     1849 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/class_errors_circuit.py
+-rw-rw-rw-   0        0        0     5704 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/depolarizing_error_model.py
+-rw-rw-rw-   0        0        0     5604 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/error_depolar.py
+-rw-rw-rw-   0        0        0     1768 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/error_model.py
+-rw-rw-rw-   0        0        0     1368 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/error_model_abc.py
+-rw-rw-rw-   0        0        0     1035 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/fake_error_model.py
+-rw-rw-rw-   0        0        0     5851 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/generic_error_model.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.605184 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/__init__.py
+-rw-rw-rw-   0        0        0      958 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_initz_bitflip.py
+-rw-rw-rw-   0        0        0     1435 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_initz_bitflip_leakage.py
+-rw-rw-rw-   0        0        0     1450 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_meas_bitflip.py
+-rw-rw-rw-   0        0        0     1621 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_meas_bitflip_leakage.py
+-rw-rw-rw-   0        0        0     1196 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_sq_bitflip.py
+-rw-rw-rw-   0        0        0     1488 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_sq_depolarizing.py
+-rw-rw-rw-   0        0        0     1958 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_sq_depolarizing_leakage.py
+-rw-rw-rw-   0        0        0     1761 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_tq_depolarizing.py
+-rw-rw-rw-   0        0        0     2490 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_tq_depolarizing_leakage.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.609184 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl_old/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl_old/__init__.py
+-rw-rw-rw-   0        0        0     2546 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl_old/gate_groups.py
+-rw-rw-rw-   0        0        0     1385 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl_old/init_noise.py
+-rw-rw-rw-   0        0        0     1593 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl_old/meas_noise.py
+-rw-rw-rw-   0        0        0     1337 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl_old/memory_noise.py
+-rw-rw-rw-   0        0        0     1207 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl_old/sq_noise.py
+-rw-rw-rw-   0        0        0     2943 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl_old/tq_noise.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.612687 quantum_pecos-0.6.0.dev3/python/pecos/error_models/old/
+-rw-rw-rw-   0        0        0      791 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/old/__init__.py
+-rw-rw-rw-   0        0        0     7653 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/old/depolar_gen.py
+-rw-rw-rw-   0        0        0     5732 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/old/gatewise_gen.py
+-rw-rw-rw-   0        0        0     6255 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/old/xerror_gen.py
+-rw-rw-rw-   0        0        0     7322 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/old/xzerror_gen.py
+-rw-rw-rw-   0        0        0     6255 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/old/zerror_gen.py
+-rw-rw-rw-   0        0        0    11841 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/parent_class_error_gen.py
+-rw-rw-rw-   0        0        0     5100 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/error_models/simple_depolarizing_error_model.py
+-rw-rw-rw-   0        0        0     1026 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev3/python/pecos/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.616694 quantum_pecos-0.6.0.dev3/python/pecos/foreign_objects/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/foreign_objects/__init__.py
+-rw-rw-rw-   0        0        0     1304 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/foreign_objects/foreign_object_abc.py
+-rw-rw-rw-   0        0        0     2466 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/foreign_objects/object_pool.py
+-rw-rw-rw-   0        0        0     1168 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/foreign_objects/python.py
+-rw-rw-rw-   0        0        0      527 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev3/python/pecos/foreign_objects/wasm_execution_timer_thread.py
+-rw-rw-rw-   0        0        0     3837 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev3/python/pecos/foreign_objects/wasmer.py
+-rw-rw-rw-   0        0        0     5054 2024-05-15 17:56:54.000000 quantum_pecos-0.6.0.dev3/python/pecos/foreign_objects/wasmtime.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.618194 quantum_pecos-0.6.0.dev3/python/pecos/machines/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/machines/__init__.py
+-rw-rw-rw-   0        0        0     2356 2024-04-29 19:48:00.000000 quantum_pecos-0.6.0.dev3/python/pecos/machines/generic_machine.py
+-rw-rw-rw-   0        0        0     1591 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/machines/machine_abc.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.622194 quantum_pecos-0.6.0.dev3/python/pecos/misc/
+-rw-rw-rw-   0        0        0      840 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/misc/__init__.py
+-rw-rw-rw-   0        0        0     2240 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/misc/commute.py
+-rw-rw-rw-   0        0        0      838 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/misc/errors.py
+-rw-rw-rw-   0        0        0     1681 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/misc/gate_groups.py
+-rw-rw-rw-   0        0        0    10545 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/misc/stabilizer_funcs.py
+-rw-rw-rw-   0        0        0     1992 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/misc/std_output.py
+-rw-rw-rw-   0        0        0     3552 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/misc/symbol_library.py
+-rw-rw-rw-   0        0        0     7419 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/misc/threshold_curve.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.624703 quantum_pecos-0.6.0.dev3/python/pecos/op_processors/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/op_processors/__init__.py
+-rw-rw-rw-   0        0        0     2266 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/op_processors/generic_op_processor.py
+-rw-rw-rw-   0        0        0     1132 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/op_processors/op_processor_abc.py
+-rw-rw-rw-   0        0        0        0 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.628206 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/
+-rw-rw-rw-   0        0        0     1147 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.631207 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/color_488/
+-rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/color_488/__init__.py
+-rw-rw-rw-   0        0        0     7774 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/color_488/circuit_implementation1.py
+-rw-rw-rw-   0        0        0     7702 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/color_488/color_488.py
+-rw-rw-rw-   0        0        0     3276 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/color_488/gates.py
+-rw-rw-rw-   0        0        0     8975 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/color_488/instructions.py
+-rw-rw-rw-   0        0        0     3576 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/gate_parent_class.py
+-rw-rw-rw-   0        0        0     2262 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/helper_functions.py
+-rw-rw-rw-   0        0        0     3845 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/instruction_parent_class.py
+-rw-rw-rw-   0        0        0     7751 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/plot.py
+-rw-rw-rw-   0        0        0     8065 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/qecc_parent_class.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.633708 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_4444/
+-rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_4444/__init__.py
+-rw-rw-rw-   0        0        0     3276 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_4444/gates.py
+-rw-rw-rw-   0        0        0    11245 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_4444/instructions.py
+-rw-rw-rw-   0        0        0     9623 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_4444/surface_4444.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.636219 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_medial_4444/
+-rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_medial_4444/__init__.py
+-rw-rw-rw-   0        0        0     3276 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_medial_4444/gates.py
+-rw-rw-rw-   0        0        0    19744 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_medial_4444/instructions.py
+-rw-rw-rw-   0        0        0    10241 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_medial_4444/surface_medial_4444.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.636718 quantum_pecos-0.6.0.dev3/python/pecos/reps/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/reps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.642218 quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/
+-rw-rw-rw-   0        0        0      675 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/__init__.py
+-rw-rw-rw-   0        0        0     1844 2024-04-29 19:48:00.000000 quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/block_types.py
+-rw-rw-rw-   0        0        0     1961 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/data_types.py
+-rw-rw-rw-   0        0        0      236 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/instr_type.py
+-rw-rw-rw-   0        0        0     1104 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/list_types.py
+-rw-rw-rw-   0        0        0     1103 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/name_resolver.py
+-rw-rw-rw-   0        0        0     3167 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/op_types.py
+-rw-rw-rw-   0        0        0    10789 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/pypmir.py
+-rw-rw-rw-   0        0        0      812 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/types.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.646231 quantum_pecos-0.6.0.dev3/python/pecos/simulators/
+-rw-rw-rw-   0        0        0     1878 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.648231 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cointoss/
+-rw-rw-rw-   0        0        0      692 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cointoss/__init__.py
+-rw-rw-rw-   0        0        0     1661 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cointoss/bindings.py
+-rw-rw-rw-   0        0        0     1196 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cointoss/gates.py
+-rw-rw-rw-   0        0        0     1773 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cointoss/state.py
+-rw-rw-rw-   0        0        0     2185 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/compile_cython.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.649231 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/
+-rw-rw-rw-   0        0        0      698 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/cuconn.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.649731 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/
+-rw-rw-rw-   0        0        0      692 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.651731 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/
+-rw-rw-rw-   0        0        0      624 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/__init__.py
+-rw-rw-rw-   0        0        0     4489 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/test_python_bindings.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.655236 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/custatevec/
+-rw-rw-rw-   0        0        0      588 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/custatevec/__init__.py
+-rw-rw-rw-   0        0        0     2010 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/custatevec/bindings.py
+-rw-rw-rw-   0        0        0     1046 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/custatevec/gates_init.py
+-rw-rw-rw-   0        0        0      785 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/custatevec/gates_meas.py
+-rw-rw-rw-   0        0        0     3562 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/custatevec/gates_sq.py
+-rw-rw-rw-   0        0        0     1200 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/custatevec/gates_tq.py
+-rw-rw-rw-   0        0        0     1874 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/custatevec/state.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.659742 quantum_pecos-0.6.0.dev3/python/pecos/simulators/custatevec/
+-rw-rw-rw-   0        0        0      698 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/custatevec/__init__.py
+-rw-rw-rw-   0        0        0     2203 2024-05-24 15:55:50.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/custatevec/bindings.py
+-rw-rw-rw-   0        0        0     1361 2024-05-24 15:55:50.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/custatevec/gates_init.py
+-rw-rw-rw-   0        0        0     1871 2024-05-24 15:55:50.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/custatevec/gates_meas.py
+-rw-rw-rw-   0        0        0     9620 2024-05-24 15:55:50.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/custatevec/gates_one_qubit.py
+-rw-rw-rw-   0        0        0    12442 2024-05-24 15:55:50.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/custatevec/gates_two_qubit.py
+-rw-rw-rw-   0        0        0     4128 2024-05-24 15:55:50.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/custatevec/state.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.660741 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim/
+-rw-rw-rw-   0        0        0      857 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim/__init__.py
+-rw-rw-rw-   0        0        0     2191 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.662242 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim/src/
+-rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim/src/__init__.py
+-rw-rw-rw-   0        0        0     6362 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim/src/logical_sign.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.663241 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_col/
+-rw-rw-rw-   0        0        0      857 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_col/__init__.py
+-rw-rw-rw-   0        0        0     1983 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_col/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.664241 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_col/src/
+-rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_col/src/__init__.py
+-rw-rw-rw-   0        0        0     6090 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_col/src/logical_sign.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.665746 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_row/
+-rw-rw-rw-   0        0        0      857 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_row/__init__.py
+-rw-rw-rw-   0        0        0     1983 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_row/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.666748 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_row/src/
+-rw-rw-rw-   0        0        0      752 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_row/src/__init__.py
+-rw-rw-rw-   0        0        0     6090 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_row/src/logical_sign.py
+-rw-rw-rw-   0        0        0     2736 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/gate_syms.py
+-rw-rw-rw-   0        0        0     2691 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/parent_sim_classes.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.671751 quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/
+-rw-rw-rw-   0        0        0      710 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/__init__.py
+-rw-rw-rw-   0        0        0     2945 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/bindings.py
+-rw-rw-rw-   0        0        0      881 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/gates_init.py
+-rw-rw-rw-   0        0        0     2985 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/gates_meas.py
+-rw-rw-rw-   0        0        0    14031 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/gates_one_qubit.py
+-rw-rw-rw-   0        0        0     7900 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/gates_two_qubit.py
+-rw-rw-rw-   0        0        0     1738 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/logical_sign.py
+-rw-rw-rw-   0        0        0     9712 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/state.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.676255 quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/
+-rw-rw-rw-   0        0        0      859 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/__init__.py
+-rw-rw-rw-   0        0        0     4891 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/bindings.py
+-rw-rw-rw-   0        0        0     2213 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/gates_init.py
+-rw-rw-rw-   0        0        0     2631 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/gates_meas.py
+-rw-rw-rw-   0        0        0     6819 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/gates_one_qubit.py
+-rw-rw-rw-   0        0        0     4884 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/gates_two_qubit.py
+-rw-rw-rw-   0        0        0     1205 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/helper.py
+-rw-rw-rw-   0        0        0     2379 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/logical_sign.py
+-rw-rw-rw-   0        0        0     4977 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/state.py
+-rw-rw-rw-   0        0        0     2885 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/quantum_simulator.py
+-rw-rw-rw-   0        0        0     1409 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/sim_class_types.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.682259 quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/
+-rw-rw-rw-   0        0        0     1933 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/__init__.py
+-rw-rw-rw-   0        0        0     2909 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/bindings.py
+-rw-rw-rw-   0        0        0     3225 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/cmd_init.py
+-rw-rw-rw-   0        0        0    11606 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/cmd_meas.py
+-rw-rw-rw-   0        0        0    33702 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/cmd_one_qubit.py
+-rw-rw-rw-   0        0        0    15954 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/cmd_two_qubit.py
+-rw-rw-rw-   0        0        0     8070 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/logical_sign.py
+-rw-rw-rw-   0        0        0     5143 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/refactor.py
+-rw-rw-rw-   0        0        0    17202 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/state.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.686766 quantum_pecos-0.6.0.dev3/python/pecos/slr/
+-rw-rw-rw-   0        0        0     1170 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/__init__.py
+-rw-rw-rw-   0        0        0     2062 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/block.py
+-rw-rw-rw-   0        0        0     2688 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/cond_block.py
+-rw-rw-rw-   0        0        0     3124 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/cops.py
+-rw-rw-rw-   0        0        0      799 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/fund.py
+-rw-rw-rw-   0        0        0     3541 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/misc.py
+-rw-rw-rw-   0        0        0     1883 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/slr.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.687769 quantum_pecos-0.6.0.dev3/python/pecos/slr/std/
+-rw-rw-rw-   0        0        0        0 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/std/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.693271 quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/
+-rw-rw-rw-   0        0        0      903 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/__init__.py
+-rw-rw-rw-   0        0        0      794 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/cliffords_tq.py
+-rw-rw-rw-   0        0        0     1664 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/face_rots.py
+-rw-rw-rw-   0        0        0      126 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/hadamards.py
+-rw-rw-rw-   0        0        0     4539 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/metaclasses.py
+-rw-rw-rw-   0        0        0      297 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/misc.py
+-rw-rw-rw-   0        0        0     1272 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/paulis.py
+-rw-rw-rw-   0        0        0      870 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/projective.py
+-rw-rw-rw-   0        0        0      381 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/rots.py
+-rw-rw-rw-   0        0        0      603 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/sqrt_paulis.py
+-rw-rw-rw-   0        0        0      878 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/util.py
+-rw-rw-rw-   0        0        0     3530 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/slr/vars.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.699780 quantum_pecos-0.6.0.dev3/python/pecos/tools/
+-rw-rw-rw-   0        0        0     1319 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/tools/__init__.py
+-rw-rw-rw-   0        0        0     6558 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/tools/fault_tolerance_checking.py
+-rw-rw-rw-   0        0        0    13635 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/tools/fault_tolerance_checks.py
+-rw-rw-rw-   0        0        0     5829 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/tools/find_cliffs.py
+-rw-rw-rw-   0        0        0     3384 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/tools/logic_circuit_speed.py
+-rw-rw-rw-   0        0        0     7186 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/tools/pseudo_threshold_tools.py
+-rw-rw-rw-   0        0        0     3630 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/tools/random_circuit_speed.py
+-rw-rw-rw-   0        0        0    32511 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/tools/stabilizer_verification.py
+-rw-rw-rw-   0        0        0    17415 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/tools/threshold_tools.py
+-rw-rw-rw-   0        0        0     1465 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/tools/tool_anticommute.py
+-rw-rw-rw-   0        0        0     6963 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/tools/tool_collection.py
+-rw-rw-rw-   0        0        0     3802 2024-03-15 23:25:09.000000 quantum_pecos-0.6.0.dev3/python/pecos/typed_list.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:22:22.704280 quantum_pecos-0.6.0.dev3/python/quantum_pecos.egg-info/
+-rw-rw-rw-   0        0        0    20937 2024-05-24 16:22:22.000000 quantum_pecos-0.6.0.dev3/python/quantum_pecos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11045 2024-05-24 16:22:22.000000 quantum_pecos-0.6.0.dev3/python/quantum_pecos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 16:22:22.000000 quantum_pecos-0.6.0.dev3/python/quantum_pecos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-15 23:26:47.000000 quantum_pecos-0.6.0.dev3/python/quantum_pecos.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      506 2024-05-24 16:22:22.000000 quantum_pecos-0.6.0.dev3/python/quantum_pecos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-24 16:22:22.000000 quantum_pecos-0.6.0.dev3/python/quantum_pecos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      741 2024-05-20 17:19:14.000000 quantum_pecos-0.6.0.dev3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 16:22:22.706280 quantum_pecos-0.6.0.dev3/setup.cfg
```

### Comparing `quantum_pecos-0.6.0.dev2/LICENSE` & `quantum_pecos-0.6.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/PKG-INFO` & `quantum_pecos-0.6.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum-pecos
-Version: 0.6.0.dev2
+Version: 0.6.0.dev3
 Summary: PECOS is a library/framework for the evaluation, study, and design of QEC protocols. It also provides the ability to study and evaluate the performance advanced hybrid quantum/classical compute execution models for NISQ algorithms and beyond.
 Author: The PECOS Developers
 Maintainer-email: Ciaran Ryan-Anderson <ciaran.ryan-anderson@quantinuum.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -230,15 +230,16 @@
 Requires-Dist: networkx<3.0,>=2.1.0
 Requires-Dist: matplotlib<4.0,>=2.2.0
 Provides-Extra: simulators
 Requires-Dist: cython; extra == "simulators"
 Requires-Dist: pybind11<3.0,>=2.2.3; extra == "simulators"
 Requires-Dist: projectq<0.9.0,>=0.5.0; extra == "simulators"
 Provides-Extra: cuda
-Requires-Dist: cuquantum-python>=23.6.0; extra == "cuda"
+Requires-Dist: cuquantum-python>=24.03.0; extra == "cuda"
+Requires-Dist: custatevec>=1.6.0; extra == "cuda"
 Requires-Dist: cupy>=10.4.0; extra == "cuda"
 Provides-Extra: wasmtime
 Requires-Dist: wasmtime>=13.0; extra == "wasmtime"
 Provides-Extra: wasmer
 Requires-Dist: wasmer~=1.1.0; extra == "wasmer"
 Requires-Dist: wasmer_compiler_cranelift~=1.1.0; extra == "wasmer"
 Provides-Extra: visualization
```

### Comparing `quantum_pecos-0.6.0.dev2/README.md` & `quantum_pecos-0.6.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/pyproject.toml` & `quantum_pecos-0.6.0.dev3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 [build-system]
 requires = ["setuptools>=62.6"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quantum-pecos"
-version = "0.6.0.dev2"
+version = "0.6.0.dev3"
 authors = [
     {name = "The PECOS Developers"},
 ]
 maintainers =[
     {name = "Ciaran Ryan-Anderson", email = "ciaran.ryan-anderson@quantinuum.com"},
 ]
 description = """PECOS is a library/framework for the evaluation, study, and design of QEC protocols. It also provides the ability to study and evaluate the performance advanced hybrid quantum/classical compute execution models for NISQ algorithms and beyond."""
@@ -55,15 +55,16 @@
 [project.optional-dependencies]
 simulators = [
     "cython",
     "pybind11>=2.2.3,<3.0",
     "projectq>=0.5.0,<0.9.0",
 ]
 cuda = [
-    "cuquantum-python>=23.6.0",
+    "cuquantum-python>=24.03.0",
+    "custatevec>=1.6.0",
     "cupy>=10.4.0",
 ]
 wasmtime = [
     "wasmtime>=13.0"
 ]
 wasmer = [
     "wasmer~=1.1.0",
```

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuit_converters/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuit_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuit_converters/checks2circuit.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuit_converters/checks2circuit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuit_converters/std2chs.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuit_converters/std2chs.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/conditionals.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/conditionals.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/cops.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/cops.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/fund.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/fund.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/hyqc.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/hyqc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/int.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/int.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/misc_stmts.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/misc_stmts.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/qops.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/qops.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/qubits.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/qubits.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/hyqc/vars.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/hyqc/vars.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/logical_circuit.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/logical_circuit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/barrier.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/barrier.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/block.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/block.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/conditionals.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/conditionals.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/expr.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/expr.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/func.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/func.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/gates.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/gates.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/misc.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/misc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/qasm.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/qasm.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/std_gates.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/std_gates.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qasm/vars.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/qasm/vars.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/qc2phir.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/qc2phir.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/circuits/quantum_circuit.py` & `quantum_pecos-0.6.0.dev3/python/pecos/circuits/quantum_circuit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/classical_interpreters/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/classical_interpreters/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/classical_interpreters/classical_interpreter_abc.py` & `quantum_pecos-0.6.0.dev3/python/pecos/classical_interpreters/classical_interpreter_abc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/classical_interpreters/phir_classical_interpreter.py` & `quantum_pecos-0.6.0.dev3/python/pecos/classical_interpreters/phir_classical_interpreter.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/decoders/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/decoders/dummy_decoder/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/decoders/dummy_decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/decoders/dummy_decoder/dummy_decoder.py` & `quantum_pecos-0.6.0.dev3/python/pecos/decoders/dummy_decoder/dummy_decoder.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/decoders/mwpm2d/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/decoders/mwpm2d/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/decoders/mwpm2d/mwpm2d.py` & `quantum_pecos-0.6.0.dev3/python/pecos/decoders/mwpm2d/mwpm2d.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/decoders/mwpm2d/precomputing.py` & `quantum_pecos-0.6.0.dev3/python/pecos/decoders/mwpm2d/precomputing.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/circuit_runners/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/circuit_runners/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/circuit_runners/standard.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/circuit_runners/standard.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/circuit_runners/timing_runner.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/circuit_runners/timing_runner.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/binarray.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/binarray.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/binarray2.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/binarray2.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/classical.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/classical.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/cvm.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/cvm.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/sim_func.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/sim_func.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/wasm.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/wasm_vms/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/pywasm.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/wasm_vms/pywasm.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/pywasm3.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/wasm_vms/pywasm3.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/wasmer.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/wasm_vms/wasmer.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/cvm/wasm_vms/wasmtime.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/cvm/wasm_vms/wasmtime.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/hybrid_engine.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/hybrid_engine.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/hybrid_engine_multiprocessing.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/hybrid_engine_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/engines/hybrid_engine_old.py` & `quantum_pecos-0.6.0.dev3/python/pecos/engines/hybrid_engine_old.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/class_errors_circuit.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/class_errors_circuit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/depolarizing_error_model.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/depolarizing_error_model.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/error_depolar.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/error_depolar.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/error_model.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/error_model.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/error_model_abc.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/error_model_abc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/fake_error_model.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/fake_error_model.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/generic_error_model.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/generic_error_model.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_initz_bitflip.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_initz_bitflip.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_initz_bitflip_leakage.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_initz_bitflip_leakage.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_meas_bitflip.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_meas_bitflip.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_meas_bitflip_leakage.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_meas_bitflip_leakage.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_sq_bitflip.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_sq_bitflip.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_sq_depolarizing.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_sq_depolarizing.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_sq_depolarizing_leakage.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_sq_depolarizing_leakage.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_tq_depolarizing.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_tq_depolarizing.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl/noise_tq_depolarizing_leakage.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl/noise_tq_depolarizing_leakage.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl_old/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/gate_groups.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl_old/gate_groups.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/init_noise.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl_old/init_noise.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/meas_noise.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl_old/meas_noise.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/memory_noise.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl_old/memory_noise.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/sq_noise.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl_old/sq_noise.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/noise_impl_old/tq_noise.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/noise_impl_old/tq_noise.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/old/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/depolar_gen.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/old/depolar_gen.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/gatewise_gen.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/old/gatewise_gen.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/xerror_gen.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/old/xerror_gen.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/xzerror_gen.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/old/xzerror_gen.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/old/zerror_gen.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/old/zerror_gen.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/parent_class_error_gen.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/parent_class_error_gen.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/error_models/simple_depolarizing_error_model.py` & `quantum_pecos-0.6.0.dev3/python/pecos/error_models/simple_depolarizing_error_model.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/errors.py` & `quantum_pecos-0.6.0.dev3/python/pecos/errors.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/foreign_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/foreign_object_abc.py` & `quantum_pecos-0.6.0.dev3/python/pecos/foreign_objects/foreign_object_abc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/object_pool.py` & `quantum_pecos-0.6.0.dev3/python/pecos/foreign_objects/object_pool.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/python.py` & `quantum_pecos-0.6.0.dev3/python/pecos/foreign_objects/python.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/wasm_execution_timer_thread.py` & `quantum_pecos-0.6.0.dev3/python/pecos/foreign_objects/wasm_execution_timer_thread.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/wasmer.py` & `quantum_pecos-0.6.0.dev3/python/pecos/foreign_objects/wasmer.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/foreign_objects/wasmtime.py` & `quantum_pecos-0.6.0.dev3/python/pecos/foreign_objects/wasmtime.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/machines/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/machines/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/machines/generic_machine.py` & `quantum_pecos-0.6.0.dev3/python/pecos/machines/generic_machine.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/machines/machine_abc.py` & `quantum_pecos-0.6.0.dev3/python/pecos/machines/machine_abc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/misc/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/misc/commute.py` & `quantum_pecos-0.6.0.dev3/python/pecos/misc/commute.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/misc/errors.py` & `quantum_pecos-0.6.0.dev3/python/pecos/misc/errors.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/misc/gate_groups.py` & `quantum_pecos-0.6.0.dev3/python/pecos/misc/gate_groups.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/misc/stabilizer_funcs.py` & `quantum_pecos-0.6.0.dev3/python/pecos/misc/stabilizer_funcs.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/misc/std_output.py` & `quantum_pecos-0.6.0.dev3/python/pecos/misc/std_output.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/misc/symbol_library.py` & `quantum_pecos-0.6.0.dev3/python/pecos/misc/symbol_library.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/misc/threshold_curve.py` & `quantum_pecos-0.6.0.dev3/python/pecos/misc/threshold_curve.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/op_processors/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/op_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/op_processors/generic_op_processor.py` & `quantum_pecos-0.6.0.dev3/python/pecos/op_processors/generic_op_processor.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/op_processors/op_processor_abc.py` & `quantum_pecos-0.6.0.dev3/python/pecos/op_processors/op_processor_abc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/color_488/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/circuit_implementation1.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/color_488/circuit_implementation1.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/color_488.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/color_488/color_488.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/gates.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/color_488/gates.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/color_488/instructions.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/color_488/instructions.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/gate_parent_class.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/gate_parent_class.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/helper_functions.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/helper_functions.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/instruction_parent_class.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/instruction_parent_class.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/plot.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/plot.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/qecc_parent_class.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/qecc_parent_class.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_4444/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/gates.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_4444/gates.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/instructions.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_4444/instructions.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_4444/surface_4444.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_4444/surface_4444.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_medial_4444/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/gates.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_medial_4444/gates.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/instructions.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_medial_4444/instructions.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/qeccs/surface_medial_4444/surface_medial_4444.py` & `quantum_pecos-0.6.0.dev3/python/pecos/qeccs/surface_medial_4444/surface_medial_4444.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/reps/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/reps/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/block_types.py` & `quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/block_types.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/data_types.py` & `quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/data_types.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/list_types.py` & `quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/list_types.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/name_resolver.py` & `quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/name_resolver.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/op_types.py` & `quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/op_types.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/pypmir.py` & `quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/pypmir.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/reps/pypmir/types.py` & `quantum_pecos-0.6.0.dev3/python/pecos/reps/pypmir/types.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cointoss/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/bindings.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cointoss/bindings.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/gates.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cointoss/gates.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cointoss/state.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cointoss/state.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/compile_cython.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/compile_cython.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuconn.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/cuconn.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/test_python_bindings.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/cuquantum_wrapper/test/test_python_bindings.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/custatevec/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/bindings.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/custatevec/bindings.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_init.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/custatevec/gates_init.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_meas.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/custatevec/gates_meas.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_sq.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/custatevec/gates_sq.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/gates_tq.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/custatevec/gates_tq.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cuquantum_old/custatevec/state.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cuquantum_old/custatevec/state.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/custatevec/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/bindings.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/custatevec/bindings.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,37 +7,52 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import pecos.simulators.custatevec.gates_one_qubit as one_q
 import pecos.simulators.custatevec.gates_two_qubit as two_q
-from pecos.simulators.custatevec.gates_init import init_zero
+from pecos.simulators.custatevec.gates_init import init_one, init_zero
 from pecos.simulators.custatevec.gates_meas import meas_z
 
 # Supporting gates from table:
 #   https://github.com/CQCL/phir/blob/main/spec.md#table-ii---quantum-operations
 
 gate_dict = {
     "Init": init_zero,
+    "init |0>": init_zero,
+    "init |1>": init_one,
     "Measure": meas_z,
+    "measure Z": meas_z,
+    "leak": init_zero,
+    "leak |0>": init_zero,
+    "leak |1>": init_one,
+    "unleak |0>": init_zero,
+    "unleak |1>": init_one,
     "I": one_q.identity,
     "X": one_q.X,
     "Y": one_q.Y,
     "Z": one_q.Z,
     "RX": one_q.RX,
     "RY": one_q.RY,
     "RZ": one_q.RZ,
     "R1XY": one_q.R1XY,
+    "RXY1Q": one_q.R1XY,
     "SX": one_q.SX,
     "SXdg": one_q.SXdg,
+    "SqrtX": one_q.SX,
+    "SqrtXd": one_q.SXdg,
     "SY": one_q.SY,
     "SYdg": one_q.SYdg,
+    "SqrtY": one_q.SY,
+    "SqrtYd": one_q.SYdg,
     "SZ": one_q.SZ,
     "SZdg": one_q.SZdg,
+    "SqrtZ": one_q.SZ,
+    "SqrtZd": one_q.SZdg,
     "H": one_q.H,
     "F": one_q.F,
     "Fdg": one_q.Fdg,
     "T": one_q.T,
     "Tdg": one_q.Tdg,
     "CX": two_q.CX,
     "CY": two_q.CY,
@@ -47,10 +62,11 @@
     "RZZ": two_q.RZZ,
     "R2XXYYZZ": two_q.R2XXYYZZ,
     "SXX": two_q.SXX,
     "SXXdg": two_q.SXXdg,
     "SYY": two_q.SYY,
     "SYYdg": two_q.SYYdg,
     "SZZ": two_q.SZZ,
+    "SqrtZZ": two_q.SZZ,
     "SZZdg": two_q.SZZdg,
     "SWAP": two_q.SWAP,
 }
```

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_init.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/custatevec/gates_init.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,7 +22,20 @@
         state: An instance of CuStateVec
         qubit: The index of the qubit to be initialised
     """
     result = meas_z(state, qubit)
 
     if result:
         X(state, qubit)
+
+
+def init_one(state, qubit: int, **params: Any) -> None:
+    """Initialise or reset the qubit to state |1>
+
+    Args:
+        state: An instance of CuStateVec
+        qubit: The index of the qubit to be initialised
+    """
+    result = meas_z(state, qubit)
+
+    if not result:
+        X(state, qubit)
```

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_meas.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/custatevec/gates_meas.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,18 +32,18 @@
         msg = f"Qubit {qubit} out of range."
         raise ValueError(msg)
     # CuStateVec uses smaller qubit index as least significant
     target = state.num_qubits - 1 - qubit
 
     result = cusv.measure_on_z_basis(
         handle=state.libhandle,
-        sv=state.vector.data.ptr,
+        sv=state.cupy_vector.data.ptr,
         sv_data_type=state.cuda_type,
         n_index_bits=state.num_qubits,  # Number of qubits in the statevector
         basis_bits=[target],  # The index of the qubit being measured
         n_basis_bits=1,  # Number of qubits being measured
-        rand_num=np.random.random(),  # Source of randomness for the measurement
+        randnum=np.random.random(),  # Source of randomness for the measurement
         collapse=cusv.Collapse.NORMALIZE_AND_ZERO,  # Collapse and normalise
     )
     state.stream.synchronize()
 
     return result
```

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_one_qubit.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/custatevec/gates_one_qubit.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,29 +30,29 @@
         msg = f"Qubit {qubit} out of range."
         raise ValueError(msg)
     # CuStateVec uses smaller qubit index as least significant
     target = state.num_qubits - 1 - qubit
 
     cusv.apply_matrix(
         handle=state.libhandle,
-        sv=state.vector.data.ptr,
+        sv=state.cupy_vector.data.ptr,
         sv_data_type=state.cuda_type,
         n_index_bits=state.num_qubits,
         matrix=matrix.data.ptr,
         matrix_data_type=state.cuda_type,
         layout=cusv.MatrixLayout.ROW,
         adjoint=0,  # Don't use the adjoint
         targets=[target],
         n_targets=1,
         controls=[],
         control_bit_values=[],  # No value of control bit assigned
         n_controls=0,
         compute_type=state.compute_type,
-        workspace=0,  # Let cuQuantum use the mempool we configured
-        workspace_size=0,  # Let cuQuantum use the mempool we configured
+        extra_workspace=0,  # Let cuQuantum use the mempool we configured
+        extra_workspace_size_in_bytes=0,  # Let cuQuantum use the mempool we configured
     )
     state.stream.synchronize()
 
 
 def identity(state, qubit: int, **params: Any) -> None:
     """
     Identity gate.
```

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/gates_two_qubit.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/custatevec/gates_two_qubit.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,29 +35,29 @@
         raise ValueError(msg)
     # CuStateVec uses smaller qubit index as least significant
     control = state.num_qubits - 1 - control
     target = state.num_qubits - 1 - target
 
     cusv.apply_matrix(
         handle=state.libhandle,
-        sv=state.vector.data.ptr,
+        sv=state.cupy_vector.data.ptr,
         sv_data_type=state.cuda_type,
         n_index_bits=state.num_qubits,
         matrix=matrix.data.ptr,
         matrix_data_type=state.cuda_type,
         layout=cusv.MatrixLayout.ROW,
         adjoint=0,  # Don't use the adjoint
         targets=[target],
         n_targets=1,
         controls=[control],
         control_bit_values=[],  # No value of control bit assigned
         n_controls=1,
         compute_type=state.compute_type,
-        workspace=0,  # Let cuQuantum use the mempool we configured
-        workspace_size=0,  # Let cuQuantum use the mempool we configured
+        extra_workspace=0,  # Let cuQuantum use the mempool we configured
+        extra_workspace_size_in_bytes=0,  # Let cuQuantum use the mempool we configured
     )
     state.stream.synchronize()
 
 
 def CX(state, qubits: tuple[int, int], **params: Any) -> None:
     """
     Apply controlled X gate.
@@ -138,29 +138,29 @@
         raise ValueError(msg)
     # CuStateVec uses smaller qubit index as least significant
     q0 = state.num_qubits - 1 - qubits[0]
     q1 = state.num_qubits - 1 - qubits[1]
 
     cusv.apply_matrix(
         handle=state.libhandle,
-        sv=state.vector.data.ptr,
+        sv=state.cupy_vector.data.ptr,
         sv_data_type=state.cuda_type,
         n_index_bits=state.num_qubits,
         matrix=matrix.data.ptr,
         matrix_data_type=state.cuda_type,
         layout=cusv.MatrixLayout.ROW,
         adjoint=0,  # Don't use the adjoint
         targets=[q0, q1],
         n_targets=2,
         controls=[],
         control_bit_values=[],  # No value of control bit assigned
         n_controls=0,
         compute_type=state.compute_type,
-        workspace=0,  # Let cuQuantum use the mempool we configured
-        workspace_size=0,  # Let cuQuantum use the mempool we configured
+        extra_workspace=0,  # Let cuQuantum use the mempool we configured
+        extra_workspace_size_in_bytes=0,  # Let cuQuantum use the mempool we configured
     )
     state.stream.synchronize()
 
 
 def RXX(state, qubits: tuple[int, int], angles: tuple[float], **params: Any) -> None:
     """
     Apply a rotation about XX.
@@ -214,24 +214,24 @@
     theta = angles[0]
 
     matrix = cp.asarray(
         [
             math.cos(theta / 2),
             0,
             0,
-            math.sin(theta / 2),
+            1j * math.sin(theta / 2),
             0,
             math.cos(theta / 2),
             -1j * math.sin(theta / 2),
             0,
             0,
             -1j * math.sin(theta / 2),
             math.cos(theta / 2),
             0,
-            math.sin(theta / 2),
+            1j * math.sin(theta / 2),
             0,
             0,
             math.cos(theta / 2),
         ],
         dtype=state.cp_type,
     )
     _apply_two_qubit_matrix(state, qubits, matrix)
@@ -376,23 +376,23 @@
     # CuStateVec uses smaller qubit index as least significant
     q0 = state.num_qubits - 1 - qubits[0]
     q1 = state.num_qubits - 1 - qubits[1]
 
     # Possibly faster since it may just be an internal qubit relabelling or sv reshape
     cusv.apply_generalized_permutation_matrix(
         handle=state.libhandle,
-        sv=state.vector.data.ptr,
+        sv=state.cupy_vector.data.ptr,
         sv_data_type=state.cuda_type,
         n_index_bits=state.num_qubits,
         permutation=[0, 2, 1, 3],  # Leave |00> and |11> where they are, swap the other two
         diagonals=0,  # Don't apply a diagonal gate
         diagonals_data_type=state.cuda_type,
         adjoint=0,  # Don't use the adjoint
         targets=[q0, q1],
         n_targets=2,
         controls=[],
         control_bit_values=[],  # No value of control bit assigned
         n_controls=0,
-        workspace=0,  # Let cuQuantum use the mempool we configured
-        workspace_size=0,  # Let cuQuantum use the mempool we configured
+        extra_workspace=0,  # Let cuQuantum use the mempool we configured
+        extra_workspace_size_in_bytes=0,  # Let cuQuantum use the mempool we configured
     )
     state.stream.synchronize()
```

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/custatevec/state.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/custatevec/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import random
 
 import cupy as cp
+import numpy as np
 from cuquantum import ComputeType, cudaDataType
 from cuquantum import custatevec as cusv
 
 from pecos.simulators.custatevec import bindings
 from pecos.simulators.sim_class_types import StateVector
 
 
@@ -48,16 +49,16 @@
 
         # Set data type as double precision complex numbers
         self.cp_type = cp.complex128
         self.cuda_type = cudaDataType.CUDA_C_64F  # == cp.complex128
         self.compute_type = ComputeType.COMPUTE_64F
 
         # Allocate the statevector in GPU and initialize it to |0>
-        self.vector = cp.zeros(shape=2**num_qubits, dtype=self.cp_type)
-        self.vector[0] = 1
+        self.cupy_vector = cp.zeros(shape=2**num_qubits, dtype=self.cp_type)
+        self.cupy_vector[0] = 1
 
         ####################################################
         # Set up cuStateVec library and GPU memory handles #
         ####################################################
         # All of this comes from:
         # https://github.com/NVIDIA/cuQuantum/blob/main/python/samples/custatevec/memory_handler.py
 
@@ -93,11 +94,22 @@
 
         def free(ptr, size, stream):
             cp.cuda.runtime.freeAsync(ptr, stream)
 
         mem_handler = (malloc, free, "GPU memory handler")
         cusv.set_device_mem_handler(self.libhandle, mem_handler)
 
+    def reset(self):
+        """Reset the quantum state for another run without reinitializing."""
+        # Initialize all qubits in the zero state
+        self.vector = cp.zeros(shape=2**self.num_qubits, dtype=self.cp_type)
+        self.vector[0] = 1
+        return self
+
     def __del__(self) -> None:
-        # CuPy will release GPU memory when the variable ``self.vector`` is no longer
+        # CuPy will release GPU memory when the variable ``self.cupy_vector`` is no longer
         # reachable. However, we need to manually destroy the library handle.
         cusv.destroy(self.libhandle)
+
+    @property
+    def vector(self) -> np.ndarray:
+        return self.cupy_vector.get()
```

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/setup.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/src/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim/src/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim/src/logical_sign.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim/src/logical_sign.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_col/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/setup.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_col/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/src/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_col/src/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_col/src/logical_sign.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_col/src/logical_sign.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_row/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/setup.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_row/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/src/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_row/src/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/cysparsesim_row/src/logical_sign.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/cysparsesim_row/src/logical_sign.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/gate_syms.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/gate_syms.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/parent_sim_classes.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/parent_sim_classes.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/bindings.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/bindings.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_init.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/gates_init.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_meas.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/gates_meas.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_one_qubit.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/gates_one_qubit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/gates_two_qubit.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/gates_two_qubit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/logical_sign.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/logical_sign.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/paulifaultprop/state.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/paulifaultprop/state.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/bindings.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/bindings.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_init.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/gates_init.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_meas.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/gates_meas.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_one_qubit.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/gates_one_qubit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/gates_two_qubit.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/gates_two_qubit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/helper.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/helper.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/logical_sign.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/logical_sign.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/projectq/state.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/projectq/state.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/quantum_simulator.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/quantum_simulator.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sim_class_types.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/sim_class_types.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/bindings.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/bindings.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_init.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/cmd_init.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_meas.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/cmd_meas.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_one_qubit.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/cmd_one_qubit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/cmd_two_qubit.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/cmd_two_qubit.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/logical_sign.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/logical_sign.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/refactor.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/refactor.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/simulators/sparsesim/state.py` & `quantum_pecos-0.6.0.dev3/python/pecos/simulators/sparsesim/state.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/block.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/block.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/cond_block.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/cond_block.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/cops.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/cops.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/fund.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/fund.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/misc.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/misc.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/slr.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/slr.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/cliffords_tq.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/cliffords_tq.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/face_rots.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/face_rots.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/metaclasses.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/metaclasses.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/paulis.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/paulis.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/projective.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/projective.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/std/phys/sqrt_paulis.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/std/phys/sqrt_paulis.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/util.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/util.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/slr/vars.py` & `quantum_pecos-0.6.0.dev3/python/pecos/slr/vars.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/tools/__init__.py` & `quantum_pecos-0.6.0.dev3/python/pecos/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/tools/fault_tolerance_checking.py` & `quantum_pecos-0.6.0.dev3/python/pecos/tools/fault_tolerance_checking.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/tools/fault_tolerance_checks.py` & `quantum_pecos-0.6.0.dev3/python/pecos/tools/fault_tolerance_checks.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/tools/find_cliffs.py` & `quantum_pecos-0.6.0.dev3/python/pecos/tools/find_cliffs.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/tools/logic_circuit_speed.py` & `quantum_pecos-0.6.0.dev3/python/pecos/tools/logic_circuit_speed.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/tools/pseudo_threshold_tools.py` & `quantum_pecos-0.6.0.dev3/python/pecos/tools/pseudo_threshold_tools.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/tools/random_circuit_speed.py` & `quantum_pecos-0.6.0.dev3/python/pecos/tools/random_circuit_speed.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/tools/stabilizer_verification.py` & `quantum_pecos-0.6.0.dev3/python/pecos/tools/stabilizer_verification.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/tools/threshold_tools.py` & `quantum_pecos-0.6.0.dev3/python/pecos/tools/threshold_tools.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/tools/tool_anticommute.py` & `quantum_pecos-0.6.0.dev3/python/pecos/tools/tool_anticommute.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/tools/tool_collection.py` & `quantum_pecos-0.6.0.dev3/python/pecos/tools/tool_collection.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/pecos/typed_list.py` & `quantum_pecos-0.6.0.dev3/python/pecos/typed_list.py`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/PKG-INFO` & `quantum_pecos-0.6.0.dev3/python/quantum_pecos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum-pecos
-Version: 0.6.0.dev2
+Version: 0.6.0.dev3
 Summary: PECOS is a library/framework for the evaluation, study, and design of QEC protocols. It also provides the ability to study and evaluate the performance advanced hybrid quantum/classical compute execution models for NISQ algorithms and beyond.
 Author: The PECOS Developers
 Maintainer-email: Ciaran Ryan-Anderson <ciaran.ryan-anderson@quantinuum.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -230,15 +230,16 @@
 Requires-Dist: networkx<3.0,>=2.1.0
 Requires-Dist: matplotlib<4.0,>=2.2.0
 Provides-Extra: simulators
 Requires-Dist: cython; extra == "simulators"
 Requires-Dist: pybind11<3.0,>=2.2.3; extra == "simulators"
 Requires-Dist: projectq<0.9.0,>=0.5.0; extra == "simulators"
 Provides-Extra: cuda
-Requires-Dist: cuquantum-python>=23.6.0; extra == "cuda"
+Requires-Dist: cuquantum-python>=24.03.0; extra == "cuda"
+Requires-Dist: custatevec>=1.6.0; extra == "cuda"
 Requires-Dist: cupy>=10.4.0; extra == "cuda"
 Provides-Extra: wasmtime
 Requires-Dist: wasmtime>=13.0; extra == "wasmtime"
 Provides-Extra: wasmer
 Requires-Dist: wasmer~=1.1.0; extra == "wasmer"
 Requires-Dist: wasmer_compiler_cranelift~=1.1.0; extra == "wasmer"
 Provides-Extra: visualization
```

### Comparing `quantum_pecos-0.6.0.dev2/python/quantum_pecos.egg-info/SOURCES.txt` & `quantum_pecos-0.6.0.dev3/python/quantum_pecos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantum_pecos-0.6.0.dev2/requirements.txt` & `quantum_pecos-0.6.0.dev3/requirements.txt`

 * *Files identical despite different names*

