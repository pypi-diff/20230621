# Comparing `tmp/pykiso-0.22.1.tar.gz` & `tmp/pykiso-0.22.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykiso-0.22.1.tar", max compression
+gzip compressed data, was "pykiso-0.22.2.tar", max compression
```

## Comparing `pykiso-0.22.1.tar` & `pykiso-0.22.2.tar`

### file list

```diff
@@ -1,112 +1,120 @@
--rw-r--r--   0        0        0    14194 2023-05-26 11:45:04.349382 pykiso-0.22.1/LICENSE
--rw-r--r--   0        0        0     6028 2023-05-26 11:45:04.349382 pykiso-0.22.1/README.md
--rw-r--r--   0        0        0     4289 2023-05-26 11:45:04.542378 pykiso-0.22.1/pyproject.toml
--rw-r--r--   0        0        0     1972 2023-05-26 11:45:04.543378 pykiso-0.22.1/src/pykiso/__init__.py
--rw-r--r--   0        0        0      642 2023-05-26 11:45:04.543378 pykiso-0.22.1/src/pykiso/__main__.py
--rw-r--r--   0        0        0     9480 2023-05-26 11:45:04.543378 pykiso-0.22.1/src/pykiso/auxiliary.py
--rw-r--r--   0        0        0     7920 2023-05-26 11:45:04.543378 pykiso-0.22.1/src/pykiso/cli.py
--rw-r--r--   0        0        0    11837 2023-05-26 11:45:04.543378 pykiso-0.22.1/src/pykiso/config_parser.py
--rw-r--r--   0        0        0     5559 2023-05-26 11:45:04.543378 pykiso-0.22.1/src/pykiso/connector.py
--rw-r--r--   0        0        0     2436 2023-05-26 11:45:04.543378 pykiso-0.22.1/src/pykiso/exceptions.py
--rw-r--r--   0        0        0     4509 2023-05-26 11:45:04.544378 pykiso-0.22.1/src/pykiso/global_config.py
--rw-r--r--   0        0        0      410 2023-05-26 11:45:04.544378 pykiso-0.22.1/src/pykiso/interfaces/__init__.py
--rw-r--r--   0        0        0    13651 2023-05-26 11:45:04.544378 pykiso-0.22.1/src/pykiso/interfaces/dt_auxiliary.py
--rw-r--r--   0        0        0     8975 2023-05-26 11:45:04.544378 pykiso-0.22.1/src/pykiso/interfaces/mp_auxiliary.py
--rw-r--r--   0        0        0     4318 2023-05-26 11:45:04.544378 pykiso-0.22.1/src/pykiso/interfaces/simple_auxiliary.py
--rw-r--r--   0        0        0     8665 2023-05-26 11:45:04.544378 pykiso-0.22.1/src/pykiso/interfaces/thread_auxiliary.py
--rw-r--r--   0        0        0      516 2023-05-26 11:45:04.545378 pykiso-0.22.1/src/pykiso/lib/__init__.py
--rw-r--r--   0        0        0      552 2023-05-26 11:45:04.545378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/__init__.py
--rw-r--r--   0        0        0     8415 2023-05-26 11:45:04.545378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/acroname_auxiliary.py
--rw-r--r--   0        0        0     7916 2023-05-26 11:45:04.545378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/communication_auxiliary.py
--rw-r--r--   0        0        0    12655 2023-05-26 11:45:04.545378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/dut_auxiliary.py
--rw-r--r--   0        0        0     2014 2023-05-26 11:45:04.545378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py
--rw-r--r--   0        0        0    10145 2023-05-26 11:45:04.546378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py
--rw-r--r--   0        0        0    19216 2023-05-26 11:45:04.546378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py
--rw-r--r--   0        0        0     5029 2023-05-26 11:45:04.546378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py
--rw-r--r--   0        0        0    16676 2023-05-26 11:45:04.546378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py
--rw-r--r--   0        0        0    14219 2023-05-26 11:45:04.546378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py
--rw-r--r--   0        0        0    14149 2023-05-26 11:45:04.546378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/proxy_auxiliary.py
--rw-r--r--   0        0        0    17111 2023-05-26 11:45:04.547378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/record_auxiliary.py
--rw-r--r--   0        0        0     2645 2023-05-26 11:45:04.547378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py
--rw-r--r--   0        0        0     6511 2023-05-26 11:45:04.547378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py
--rw-r--r--   0        0        0    14146 2023-05-26 11:45:04.547378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py
--rw-r--r--   0        0        0     3889 2023-05-26 11:45:04.547378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py
--rw-r--r--   0        0        0     4288 2023-05-26 11:45:04.547378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py
--rw-r--r--   0        0        0      718 2023-05-26 11:45:04.547378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/__init__.py
--rw-r--r--   0        0        0      599 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py
--rw-r--r--   0        0        0     3913 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/odx_parser.py
--rw-r--r--   0        0        0     5299 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py
--rw-r--r--   0        0        0    12896 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py
--rw-r--r--   0        0        0     1517 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py
--rw-r--r--   0        0        0     1570 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py
--rw-r--r--   0        0        0     2664 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py
--rw-r--r--   0        0        0     1404 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py
--rw-r--r--   0        0        0    12764 2023-05-26 11:45:04.549378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py
--rw-r--r--   0        0        0    17074 2023-05-26 11:45:04.549378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/uds_server_auxiliary.py
--rw-r--r--   0        0        0    13528 2023-05-26 11:45:04.549378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/ykush_auxiliary.py
--rw-r--r--   0        0        0      548 2023-05-26 11:45:04.549378 pykiso-0.22.1/src/pykiso/lib/connectors/__init__.py
--rw-r--r--   0        0        0     3999 2023-05-26 11:45:04.549378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_example.py
--rw-r--r--   0        0        0    13274 2023-05-26 11:45:04.549378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_fdx_lauterbach.py
--rw-r--r--   0        0        0     1446 2023-05-26 11:45:04.550378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_flasher_example.py
--rw-r--r--   0        0        0     4966 2023-05-26 11:45:04.550378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_mp_proxy.py
--rw-r--r--   0        0        0    19971 2023-05-26 11:45:04.550378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_pcan_can.py
--rw-r--r--   0        0        0    11002 2023-05-26 11:45:04.550378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_process.py
--rw-r--r--   0        0        0     5697 2023-05-26 11:45:04.550378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_proxy.py
--rw-r--r--   0        0        0     2048 2023-05-26 11:45:04.550378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_raw_loopback.py
--rw-r--r--   0        0        0    14178 2023-05-26 11:45:04.551378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_rtt_segger.py
--rw-r--r--   0        0        0     5713 2023-05-26 11:45:04.551378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_serial.py
--rw-r--r--   0        0        0      538 2023-05-26 11:45:04.551378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_socket_can/__init__.py
--rw-r--r--   0        0        0     7361 2023-05-26 11:45:04.551378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py
--rw-r--r--   0        0        0     8065 2023-05-26 11:45:04.551378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py
--rw-r--r--   0        0        0     3215 2023-05-26 11:45:04.551378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_tcp_ip.py
--rw-r--r--   0        0        0     5893 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_uart.py
--rw-r--r--   0        0        0     2981 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_udp.py
--rw-r--r--   0        0        0     3425 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_udp_server.py
--rw-r--r--   0        0        0     2440 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_usb.py
--rw-r--r--   0        0        0     7302 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_vector_can.py
--rw-r--r--   0        0        0     7194 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_visa.py
--rw-r--r--   0        0        0     4085 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/flash_jlink.py
--rw-r--r--   0        0        0     8380 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/flash_lauterbach.py
--rw-r--r--   0        0        0      530 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/robot_framework/__init__.py
--rw-r--r--   0        0        0     4193 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/robot_framework/acroname_auxiliary.py
--rw-r--r--   0        0        0     2380 2023-05-26 11:45:04.553378 pykiso-0.22.1/src/pykiso/lib/robot_framework/aux_interface.py
--rw-r--r--   0        0        0     3361 2023-05-26 11:45:04.553378 pykiso-0.22.1/src/pykiso/lib/robot_framework/communication_auxiliary.py
--rw-r--r--   0        0        0     3639 2023-05-26 11:45:04.553378 pykiso-0.22.1/src/pykiso/lib/robot_framework/dut_auxiliary.py
--rw-r--r--   0        0        0    16126 2023-05-26 11:45:04.553378 pykiso-0.22.1/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py
--rw-r--r--   0        0        0     3599 2023-05-26 11:45:04.553378 pykiso-0.22.1/src/pykiso/lib/robot_framework/loader.py
--rw-r--r--   0        0        0     2321 2023-05-26 11:45:04.553378 pykiso-0.22.1/src/pykiso/lib/robot_framework/proxy_auxiliary.py
--rw-r--r--   0        0        0     6606 2023-05-26 11:45:04.553378 pykiso-0.22.1/src/pykiso/lib/robot_framework/record_auxiliary.py
--rw-r--r--   0        0        0     6840 2023-05-26 11:45:04.554378 pykiso-0.22.1/src/pykiso/lib/robot_framework/uds_auxiliary.py
--rw-r--r--   0        0        0     7770 2023-05-26 11:45:04.554378 pykiso-0.22.1/src/pykiso/logging_initializer.py
--rw-r--r--   0        0        0    11744 2023-05-26 11:45:04.554378 pykiso-0.22.1/src/pykiso/message.py
--rw-r--r--   0        0        0      410 2023-05-26 11:45:04.554378 pykiso-0.22.1/src/pykiso/test_coordinator/__init__.py
--rw-r--r--   0        0        0    12735 2023-05-26 11:45:04.554378 pykiso-0.22.1/src/pykiso/test_coordinator/test_case.py
--rw-r--r--   0        0        0    16086 2023-05-26 11:45:04.554378 pykiso-0.22.1/src/pykiso/test_coordinator/test_execution.py
--rw-r--r--   0        0        0     5480 2023-05-26 11:45:04.555378 pykiso-0.22.1/src/pykiso/test_coordinator/test_message_handler.py
--rw-r--r--   0        0        0    16859 2023-05-26 11:45:04.555378 pykiso-0.22.1/src/pykiso/test_coordinator/test_suite.py
--rw-r--r--   0        0        0      515 2023-05-26 11:45:04.556378 pykiso-0.22.1/src/pykiso/test_result/__init__.py
--rw-r--r--   0        0        0    17429 2023-05-26 11:45:04.556378 pykiso-0.22.1/src/pykiso/test_result/assert_step_report.py
--rw-r--r--   0        0        0     8391 2023-05-26 11:45:04.556378 pykiso-0.22.1/src/pykiso/test_result/multi_result.py
--rw-r--r--   0        0        0     1971 2023-05-26 11:45:04.556378 pykiso-0.22.1/src/pykiso/test_result/templates/report_template.css
--rw-r--r--   0        0        0     5812 2023-05-26 11:45:04.556378 pykiso-0.22.1/src/pykiso/test_result/templates/report_template.html.j2
--rw-r--r--   0        0        0     1624 2023-05-26 11:45:04.556378 pykiso-0.22.1/src/pykiso/test_result/templates/report_template_script.js
--rw-r--r--   0        0        0     9917 2023-05-26 11:45:04.640376 pykiso-0.22.1/src/pykiso/test_result/text_result.py
--rw-r--r--   0        0        0     5663 2023-05-26 11:45:04.640376 pykiso-0.22.1/src/pykiso/test_result/xml_result.py
--rw-r--r--   0        0        0      410 2023-05-26 11:45:04.640376 pykiso-0.22.1/src/pykiso/test_setup/__init__.py
--rw-r--r--   0        0        0     9772 2023-05-26 11:45:04.641376 pykiso-0.22.1/src/pykiso/test_setup/config_registry.py
--rw-r--r--   0        0        0    14160 2023-05-26 11:45:04.641376 pykiso-0.22.1/src/pykiso/test_setup/dynamic_loader.py
--rw-r--r--   0        0        0      410 2023-05-26 11:45:04.641376 pykiso-0.22.1/src/pykiso/tool/__init__.py
--rw-r--r--   0        0        0      410 2023-05-26 11:45:04.641376 pykiso-0.22.1/src/pykiso/tool/pykiso_to_pytest/__init__.py
--rw-r--r--   0        0        0     5577 2023-05-26 11:45:04.641376 pykiso-0.22.1/src/pykiso/tool/pykiso_to_pytest/cli.py
--rw-r--r--   0        0        0     3114 2023-05-26 11:45:04.641376 pykiso-0.22.1/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2
--rw-r--r--   0        0        0    11816 2023-05-26 11:45:04.641376 pykiso-0.22.1/src/pykiso/tool/show_tag.py
--rw-r--r--   0        0        0      410 2023-05-26 11:45:04.642376 pykiso-0.22.1/src/pykiso/tool/testrail/__init__.py
--rw-r--r--   0        0        0    12414 2023-05-26 11:45:04.642376 pykiso-0.22.1/src/pykiso/tool/testrail/api.py
--rw-r--r--   0        0        0     7728 2023-05-26 11:45:04.642376 pykiso-0.22.1/src/pykiso/tool/testrail/cli.py
--rw-r--r--   0        0        0     5195 2023-05-26 11:45:04.642376 pykiso-0.22.1/src/pykiso/tool/testrail/console.py
--rw-r--r--   0        0        0     8545 2023-05-26 11:45:04.642376 pykiso-0.22.1/src/pykiso/tool/testrail/containers.py
--rw-r--r--   0        0        0     5075 2023-05-26 11:45:04.642376 pykiso-0.22.1/src/pykiso/tool/testrail/extraction.py
--rw-r--r--   0        0        0    12851 2023-05-26 11:45:04.642376 pykiso-0.22.1/src/pykiso/tool/testrail/testrail.py
--rw-r--r--   0        0        0     1794 2023-05-26 11:45:04.643376 pykiso-0.22.1/src/pykiso/types.py
--rw-r--r--   0        0        0     9371 1970-01-01 00:00:00.000000 pykiso-0.22.1/setup.py
--rw-r--r--   0        0        0     9260 1970-01-01 00:00:00.000000 pykiso-0.22.1/PKG-INFO
+-rw-r--r--   0        0        0    14194 2023-06-21 06:36:48.823367 pykiso-0.22.2/LICENSE
+-rw-r--r--   0        0        0     6028 2023-06-21 06:36:48.824367 pykiso-0.22.2/README.md
+-rw-r--r--   0        0        0     4365 2023-06-21 06:36:49.015364 pykiso-0.22.2/pyproject.toml
+-rw-r--r--   0        0        0     1972 2023-06-21 06:36:49.015364 pykiso-0.22.2/src/pykiso/__init__.py
+-rw-r--r--   0        0        0      642 2023-06-21 06:36:49.015364 pykiso-0.22.2/src/pykiso/__main__.py
+-rw-r--r--   0        0        0     9480 2023-06-21 06:36:49.015364 pykiso-0.22.2/src/pykiso/auxiliary.py
+-rw-r--r--   0        0        0     7920 2023-06-21 06:36:49.015364 pykiso-0.22.2/src/pykiso/cli.py
+-rw-r--r--   0        0        0    11837 2023-06-21 06:36:49.015364 pykiso-0.22.2/src/pykiso/config_parser.py
+-rw-r--r--   0        0        0     5559 2023-06-21 06:36:49.016364 pykiso-0.22.2/src/pykiso/connector.py
+-rw-r--r--   0        0        0     2436 2023-06-21 06:36:49.016364 pykiso-0.22.2/src/pykiso/exceptions.py
+-rw-r--r--   0        0        0     4509 2023-06-21 06:36:49.016364 pykiso-0.22.2/src/pykiso/global_config.py
+-rw-r--r--   0        0        0      410 2023-06-21 06:36:49.016364 pykiso-0.22.2/src/pykiso/interfaces/__init__.py
+-rw-r--r--   0        0        0    13651 2023-06-21 06:36:49.016364 pykiso-0.22.2/src/pykiso/interfaces/dt_auxiliary.py
+-rw-r--r--   0        0        0     8975 2023-06-21 06:36:49.016364 pykiso-0.22.2/src/pykiso/interfaces/mp_auxiliary.py
+-rw-r--r--   0        0        0     4318 2023-06-21 06:36:49.016364 pykiso-0.22.2/src/pykiso/interfaces/simple_auxiliary.py
+-rw-r--r--   0        0        0     8665 2023-06-21 06:36:49.017364 pykiso-0.22.2/src/pykiso/interfaces/thread_auxiliary.py
+-rw-r--r--   0        0        0      516 2023-06-21 06:36:49.017364 pykiso-0.22.2/src/pykiso/lib/__init__.py
+-rw-r--r--   0        0        0      552 2023-06-21 06:36:49.017364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/__init__.py
+-rw-r--r--   0        0        0     8415 2023-06-21 06:36:49.017364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/acroname_auxiliary.py
+-rw-r--r--   0        0        0     7916 2023-06-21 06:36:49.017364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/communication_auxiliary.py
+-rw-r--r--   0        0        0    12655 2023-06-21 06:36:49.017364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/dut_auxiliary.py
+-rw-r--r--   0        0        0     2014 2023-06-21 06:36:49.017364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py
+-rw-r--r--   0        0        0    10145 2023-06-21 06:36:49.018364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py
+-rw-r--r--   0        0        0    19216 2023-06-21 06:36:49.018364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py
+-rw-r--r--   0        0        0     5029 2023-06-21 06:36:49.018364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py
+-rw-r--r--   0        0        0    16676 2023-06-21 06:36:49.018364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py
+-rw-r--r--   0        0        0    14219 2023-06-21 06:36:49.018364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py
+-rw-r--r--   0        0        0    14149 2023-06-21 06:36:49.018364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/proxy_auxiliary.py
+-rw-r--r--   0        0        0    17111 2023-06-21 06:36:49.019364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/record_auxiliary.py
+-rw-r--r--   0        0        0     2645 2023-06-21 06:36:49.019364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py
+-rw-r--r--   0        0        0     6511 2023-06-21 06:36:49.019364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py
+-rw-r--r--   0        0        0    14146 2023-06-21 06:36:49.019364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py
+-rw-r--r--   0        0        0     3889 2023-06-21 06:36:49.019364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py
+-rw-r--r--   0        0        0     4288 2023-06-21 06:36:49.019364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py
+-rw-r--r--   0        0        0      718 2023-06-21 06:36:49.020364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/__init__.py
+-rw-r--r--   0        0        0      599 2023-06-21 06:36:49.020364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py
+-rw-r--r--   0        0        0     3913 2023-06-21 06:36:49.020364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/odx_parser.py
+-rw-r--r--   0        0        0     5299 2023-06-21 06:36:49.020364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py
+-rw-r--r--   0        0        0    12896 2023-06-21 06:36:49.020364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py
+-rw-r--r--   0        0        0     1517 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py
+-rw-r--r--   0        0        0     1570 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py
+-rw-r--r--   0        0        0     2664 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py
+-rw-r--r--   0        0        0     1404 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py
+-rw-r--r--   0        0        0    12764 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py
+-rw-r--r--   0        0        0    17074 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/uds_server_auxiliary.py
+-rw-r--r--   0        0        0    13528 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/auxiliaries/ykush_auxiliary.py
+-rw-r--r--   0        0        0      548 2023-06-21 06:36:49.021364 pykiso-0.22.2/src/pykiso/lib/connectors/__init__.py
+-rw-r--r--   0        0        0     3999 2023-06-21 06:36:49.022364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_example.py
+-rw-r--r--   0        0        0    13274 2023-06-21 06:36:49.022364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_fdx_lauterbach.py
+-rw-r--r--   0        0        0     1446 2023-06-21 06:36:49.022364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_flasher_example.py
+-rw-r--r--   0        0        0     4966 2023-06-21 06:36:49.022364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_mp_proxy.py
+-rw-r--r--   0        0        0    19995 2023-06-21 06:36:49.022364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_pcan_can.py
+-rw-r--r--   0        0        0    11002 2023-06-21 06:36:49.023364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_process.py
+-rw-r--r--   0        0        0     5697 2023-06-21 06:36:49.023364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_proxy.py
+-rw-r--r--   0        0        0     2048 2023-06-21 06:36:49.023364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_raw_loopback.py
+-rw-r--r--   0        0        0    14178 2023-06-21 06:36:49.023364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_rtt_segger.py
+-rw-r--r--   0        0        0     7584 2023-06-21 06:36:49.023364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_serial.py
+-rw-r--r--   0        0        0      538 2023-06-21 06:36:49.023364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_socket_can/__init__.py
+-rw-r--r--   0        0        0     7361 2023-06-21 06:36:49.023364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py
+-rw-r--r--   0        0        0     8065 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py
+-rw-r--r--   0        0        0     3215 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_tcp_ip.py
+-rw-r--r--   0        0        0     5893 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_uart.py
+-rw-r--r--   0        0        0     2981 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_udp.py
+-rw-r--r--   0        0        0     3425 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_udp_server.py
+-rw-r--r--   0        0        0     2440 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_usb.py
+-rw-r--r--   0        0        0     7378 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_vector_can.py
+-rw-r--r--   0        0        0     7194 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/cc_visa.py
+-rw-r--r--   0        0        0     4085 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/flash_jlink.py
+-rw-r--r--   0        0        0     8380 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/connectors/flash_lauterbach.py
+-rw-r--r--   0        0        0      530 2023-06-21 06:36:49.024364 pykiso-0.22.2/src/pykiso/lib/robot_framework/__init__.py
+-rw-r--r--   0        0        0     4193 2023-06-21 06:36:49.025364 pykiso-0.22.2/src/pykiso/lib/robot_framework/acroname_auxiliary.py
+-rw-r--r--   0        0        0     2380 2023-06-21 06:36:49.025364 pykiso-0.22.2/src/pykiso/lib/robot_framework/aux_interface.py
+-rw-r--r--   0        0        0     3361 2023-06-21 06:36:49.025364 pykiso-0.22.2/src/pykiso/lib/robot_framework/communication_auxiliary.py
+-rw-r--r--   0        0        0     3639 2023-06-21 06:36:49.025364 pykiso-0.22.2/src/pykiso/lib/robot_framework/dut_auxiliary.py
+-rw-r--r--   0        0        0    16126 2023-06-21 06:36:49.025364 pykiso-0.22.2/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py
+-rw-r--r--   0        0        0     3599 2023-06-21 06:36:49.025364 pykiso-0.22.2/src/pykiso/lib/robot_framework/loader.py
+-rw-r--r--   0        0        0     2321 2023-06-21 06:36:49.025364 pykiso-0.22.2/src/pykiso/lib/robot_framework/proxy_auxiliary.py
+-rw-r--r--   0        0        0     6606 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/lib/robot_framework/record_auxiliary.py
+-rw-r--r--   0        0        0     6840 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/lib/robot_framework/uds_auxiliary.py
+-rw-r--r--   0        0        0     7770 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/logging_initializer.py
+-rw-r--r--   0        0        0    11744 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/message.py
+-rw-r--r--   0        0        0      766 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/pytest_plugin/__init__.py
+-rw-r--r--   0        0        0    12366 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/pytest_plugin/collection.py
+-rw-r--r--   0        0        0     2436 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/pytest_plugin/commandline.py
+-rw-r--r--   0        0        0     1449 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/pytest_plugin/hooks.py
+-rw-r--r--   0        0        0     2376 2023-06-21 06:36:49.026364 pykiso-0.22.2/src/pykiso/pytest_plugin/logging.py
+-rw-r--r--   0        0        0      988 2023-06-21 06:36:49.108363 pykiso-0.22.2/src/pykiso/pytest_plugin/markers.py
+-rw-r--r--   0        0        0     1503 2023-06-21 06:36:49.109362 pykiso-0.22.2/src/pykiso/pytest_plugin/reporting.py
+-rw-r--r--   0        0        0     1685 2023-06-21 06:36:49.109362 pykiso-0.22.2/src/pykiso/pytest_plugin/utils.py
+-rw-r--r--   0        0        0      410 2023-06-21 06:36:49.109362 pykiso-0.22.2/src/pykiso/test_coordinator/__init__.py
+-rw-r--r--   0        0        0    12735 2023-06-21 06:36:49.109362 pykiso-0.22.2/src/pykiso/test_coordinator/test_case.py
+-rw-r--r--   0        0        0    16129 2023-06-21 06:36:49.109362 pykiso-0.22.2/src/pykiso/test_coordinator/test_execution.py
+-rw-r--r--   0        0        0     5480 2023-06-21 06:36:49.109362 pykiso-0.22.2/src/pykiso/test_coordinator/test_message_handler.py
+-rw-r--r--   0        0        0    16859 2023-06-21 06:36:49.110362 pykiso-0.22.2/src/pykiso/test_coordinator/test_suite.py
+-rw-r--r--   0        0        0      515 2023-06-21 06:36:49.110362 pykiso-0.22.2/src/pykiso/test_result/__init__.py
+-rw-r--r--   0        0        0    17429 2023-06-21 06:36:49.110362 pykiso-0.22.2/src/pykiso/test_result/assert_step_report.py
+-rw-r--r--   0        0        0     8391 2023-06-21 06:36:49.110362 pykiso-0.22.2/src/pykiso/test_result/multi_result.py
+-rw-r--r--   0        0        0     1971 2023-06-21 06:36:49.110362 pykiso-0.22.2/src/pykiso/test_result/templates/report_template.css
+-rw-r--r--   0        0        0     6250 2023-06-21 06:36:49.110362 pykiso-0.22.2/src/pykiso/test_result/templates/report_template.html.j2
+-rw-r--r--   0        0        0     3182 2023-06-21 06:36:49.111362 pykiso-0.22.2/src/pykiso/test_result/templates/report_template_script.js
+-rw-r--r--   0        0        0     9917 2023-06-21 06:36:49.111362 pykiso-0.22.2/src/pykiso/test_result/text_result.py
+-rw-r--r--   0        0        0     5663 2023-06-21 06:36:49.111362 pykiso-0.22.2/src/pykiso/test_result/xml_result.py
+-rw-r--r--   0        0        0      410 2023-06-21 06:36:49.111362 pykiso-0.22.2/src/pykiso/test_setup/__init__.py
+-rw-r--r--   0        0        0     9799 2023-06-21 06:36:49.111362 pykiso-0.22.2/src/pykiso/test_setup/config_registry.py
+-rw-r--r--   0        0        0    14160 2023-06-21 06:36:49.111362 pykiso-0.22.2/src/pykiso/test_setup/dynamic_loader.py
+-rw-r--r--   0        0        0      410 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/__init__.py
+-rw-r--r--   0        0        0      410 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/pykiso_to_pytest/__init__.py
+-rw-r--r--   0        0        0     5577 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/pykiso_to_pytest/cli.py
+-rw-r--r--   0        0        0     3114 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2
+-rw-r--r--   0        0        0    11816 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/show_tag.py
+-rw-r--r--   0        0        0      410 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/testrail/__init__.py
+-rw-r--r--   0        0        0    12414 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/testrail/api.py
+-rw-r--r--   0        0        0     7728 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/testrail/cli.py
+-rw-r--r--   0        0        0     5195 2023-06-21 06:36:49.112362 pykiso-0.22.2/src/pykiso/tool/testrail/console.py
+-rw-r--r--   0        0        0     8545 2023-06-21 06:36:49.113362 pykiso-0.22.2/src/pykiso/tool/testrail/containers.py
+-rw-r--r--   0        0        0     5075 2023-06-21 06:36:49.113362 pykiso-0.22.2/src/pykiso/tool/testrail/extraction.py
+-rw-r--r--   0        0        0    12851 2023-06-21 06:36:49.113362 pykiso-0.22.2/src/pykiso/tool/testrail/testrail.py
+-rw-r--r--   0        0        0     1794 2023-06-21 06:36:49.113362 pykiso-0.22.2/src/pykiso/types.py
+-rw-r--r--   0        0        0     9449 1970-01-01 00:00:00.000000 pykiso-0.22.2/setup.py
+-rw-r--r--   0        0        0     9260 1970-01-01 00:00:00.000000 pykiso-0.22.2/PKG-INFO
```

### Comparing `pykiso-0.22.1/LICENSE` & `pykiso-0.22.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/README.md` & `pykiso-0.22.2/README.md`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/pyproject.toml` & `pykiso-0.22.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykiso"
-version = "0.22.1"
+version = "0.22.2"
 description = "Embedded integration testing framework."
 authors = ["Sebastian Fischer <sebastian.fischer@de.bosch.com>"]
 license = "Eclipse Public License - v 2.0"
 readme = "README.md"
 homepage = "https://pypi.org/project/pykiso/"
 repository = "https://github.com/eclipse/kiso-testing"
 documentation = "https://kiso-testing.readthedocs.io/en/latest/"
@@ -125,17 +125,20 @@
 [tool.poetry.scripts]
 pykiso = 'pykiso.cli:main'
 pykiso-tags = 'pykiso.tool.show_tag:main'
 instrument-control = 'pykiso.lib.auxiliaries.instrument_control_auxiliary.instrument_control_cli:main'
 pykitest = 'pykiso.tool.pykiso_to_pytest.cli:main'
 testrail = "pykiso.tool.testrail.cli:cli_testrail"
 
+[tool.poetry.plugins]
+pytest11 = { pytest_kiso = "pykiso.pytest_plugin" }
+
 [tool.pytest.ini_options]
 testpaths = [
-    "tests/"
+    "./tests"
 ]
 addopts = """\
     --verbose \
     --log-level=INFO \
     --cov=./src \
     --cov-report=html \
     --cov-report html:./tests/coverage_report.html \
```

### Comparing `pykiso-0.22.1/src/pykiso/__init__.py` & `pykiso-0.22.2/src/pykiso/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/__main__.py` & `pykiso-0.22.2/src/pykiso/__main__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/auxiliary.py` & `pykiso-0.22.2/src/pykiso/auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/cli.py` & `pykiso-0.22.2/src/pykiso/cli.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/config_parser.py` & `pykiso-0.22.2/src/pykiso/config_parser.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/connector.py` & `pykiso-0.22.2/src/pykiso/connector.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/exceptions.py` & `pykiso-0.22.2/src/pykiso/exceptions.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/global_config.py` & `pykiso-0.22.2/src/pykiso/global_config.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/interfaces/dt_auxiliary.py` & `pykiso-0.22.2/src/pykiso/interfaces/dt_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/interfaces/mp_auxiliary.py` & `pykiso-0.22.2/src/pykiso/interfaces/mp_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/interfaces/simple_auxiliary.py` & `pykiso-0.22.2/src/pykiso/interfaces/simple_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/interfaces/thread_auxiliary.py` & `pykiso-0.22.2/src/pykiso/interfaces/thread_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/__init__.py` & `pykiso-0.22.2/src/pykiso/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/__init__.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/acroname_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/acroname_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/communication_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/communication_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/dut_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/dut_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/proxy_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/proxy_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/record_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/record_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/__init__.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/odx_parser.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/odx_parser.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/uds_server_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/udsaux/uds_server_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/auxiliaries/ykush_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/auxiliaries/ykush_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/__init__.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_example.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_example.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_fdx_lauterbach.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_fdx_lauterbach.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_flasher_example.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_flasher_example.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_mp_proxy.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_mp_proxy.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_pcan_can.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_pcan_can.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,15 @@
                 frame_id = received_msg.arbitration_id
                 payload = received_msg.data
                 timestamp = received_msg.timestamp
 
                 log.internal_debug(
                     f"received CAN Message: {frame_id}, {payload}, {timestamp}"
                 )
-                return {"msg": payload, "remote_id": frame_id}
+                return {"msg": payload, "remote_id": frame_id, "timestamp": timestamp}
             else:
                 return {"msg": None}
         except can.CanError as can_error:
             log.internal_debug(f"encountered can error: {can_error}")
             return {"msg": None}
         except Exception:
             log.exception(f"encountered error while receiving message via {self}")
```

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_process.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_process.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_proxy.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_proxy.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_raw_loopback.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_raw_loopback.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_rtt_segger.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_rtt_segger.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_serial.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_serial.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,25 +15,29 @@
 
 :synopsis: Serial communication channel
 
 .. currentmodule:: cc_serial
 
 """
 
-
+import logging
+import sys
+import time
 from enum import Enum, IntEnum
-from typing import ByteString, Dict, Optional, Union
+from typing import ByteString, Dict, List, Optional, Union
 
 try:
     import serial
+    import serial.tools.list_ports
 except ImportError as e:
     raise ImportError(
         f"{e.name} dependency missing, consider installing pykiso with 'pip install pykiso[serial]'"
     )
 
+log = logging.getLogger(__name__)
 
 from pykiso import Message, connector
 
 MessageType = Union[Message, bytes]
 
 
 class ByteSize(IntEnum):
@@ -58,15 +62,17 @@
 
 
 class CCSerial(connector.CChannel):
     """Connector for serial devices"""
 
     def __init__(
         self,
-        port: str,
+        port: Optional[str] = None,
+        vid: Optional[int] = None,
+        pid: Optional[int] = None,
         baudrate: int = 9600,
         bytesize: ByteSize = ByteSize.EIGHT_BITS,
         parity: Parity = Parity.PARITY_NONE,
         stopbits: StopBits = StopBits.STOPBITS_ONE,
         timeout: Optional[float] = None,
         xonxoff: bool = False,
         rtscts: bool = False,
@@ -115,15 +121,60 @@
             write_timeout=write_timeout,
             dsrdtr=dsrdtr,
             inter_byte_timeout=inter_byte_timeout,
             exclusive=exclusive,
         )
 
         self.current_write_timeout = write_timeout
-        self.serial.port = port
+        self.serial.port = self._get_port(port=port, vid=vid, pid=pid)
+
+    @staticmethod
+    def _find_device(vid: int, pid: int) -> str:
+        """Return the device which matches pid and vid.
+
+        :param vid: vendor id
+        :param pid: product id
+
+        :return: com port for the found device. I.e. "COM4" or "/dev/tty1"
+        """
+
+        attached_com_devices = serial.tools.list_ports.comports()
+        found_devices = [
+            port for port in attached_com_devices if port.pid == pid and port.vid == vid
+        ]
+        if not found_devices:
+            raise ConnectionError(
+                f"Failed to detect connected USB device with IDs {vid:04X}:{pid:04x}."
+            )
+
+        found_devices = [
+            port.name if not sys.platform.startswith("win") else port.device
+            for port in found_devices
+        ]
+        if len(found_devices) > 1:
+            log.internal_warning(
+                f"Found multiple devices, {found_devices}, with matching IDs {vid:04X}:{pid:04x}. Select first device {found_devices[0]}."
+            )
+        return found_devices[0]
+
+    def _get_port(self, port: str, vid: int, pid: int) -> str:
+        """Returns com port depending on the given port argument.
+        If port set to auto, the device will be searched for,
+        using the pid and vid, else the port argument will be returned.
+
+        :param port: port  I.e. "COM4" or "/dev/tty1"
+        :param vid: vendor id
+        :param pid: product id
+
+        :return: com ports of given or found device. I.e. "COM4" or "/dev/tty1"
+        """
+        if port is None:
+            return CCSerial._find_device(vid=vid, pid=pid)
+        else:
+            return port
 
     def _cc_open(self) -> None:
         """Open serial port"""
         self.serial.open()
 
     def _cc_close(self) -> None:
         """Close serial port"""
```

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_socket_can/__init__.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_socket_can/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_tcp_ip.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_tcp_ip.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_uart.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_uart.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_udp.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_udp.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_udp_server.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_udp_server.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_usb.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_usb.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_vector_can.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_vector_can.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,17 +160,19 @@
         """
         try:  # Catch bus errors & rcv.data errors when no messages where received
             received_msg = self.bus.recv(timeout=timeout or self.timeout)
 
             if received_msg is not None:
                 frame_id = received_msg.arbitration_id
                 payload = received_msg.data
+                timestamp = received_msg.timestamp
+
                 log.internal_debug(f"received CAN Message: {frame_id}, {payload}")
 
-                return {"msg": payload, "remote_id": frame_id}
+                return {"msg": payload, "remote_id": frame_id, "timestamp": timestamp}
             else:
                 return {"msg": None}
         except BaseException:
             log.exception(f"encountered error while receiving message via {self}")
             return {"msg": None}
```

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/cc_visa.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/cc_visa.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/flash_jlink.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/flash_jlink.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/connectors/flash_lauterbach.py` & `pykiso-0.22.2/src/pykiso/lib/connectors/flash_lauterbach.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/robot_framework/__init__.py` & `pykiso-0.22.2/src/pykiso/lib/robot_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/robot_framework/acroname_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/robot_framework/acroname_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/robot_framework/aux_interface.py` & `pykiso-0.22.2/src/pykiso/lib/robot_framework/aux_interface.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/robot_framework/communication_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/robot_framework/communication_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/robot_framework/dut_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/robot_framework/dut_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/robot_framework/loader.py` & `pykiso-0.22.2/src/pykiso/lib/robot_framework/loader.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/robot_framework/proxy_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/robot_framework/proxy_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/robot_framework/record_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/robot_framework/record_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/lib/robot_framework/uds_auxiliary.py` & `pykiso-0.22.2/src/pykiso/lib/robot_framework/uds_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/logging_initializer.py` & `pykiso-0.22.2/src/pykiso/logging_initializer.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/message.py` & `pykiso-0.22.2/src/pykiso/message.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/test_coordinator/test_case.py` & `pykiso-0.22.2/src/pykiso/test_coordinator/test_case.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/test_coordinator/test_execution.py` & `pykiso-0.22.2/src/pykiso/test_coordinator/test_execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,24 +29,25 @@
 from typing import TYPE_CHECKING
 from unittest.loader import VALID_MODULE_NAME
 
 from pykiso.test_result.multi_result import MultiTestResult
 
 if TYPE_CHECKING:
     from .test_case import BasicTest
+    from ..types import ConfigDict, SuiteConfig
 
 import enum
 import logging
 import re
 import time
 import unittest
 from collections import OrderedDict, namedtuple
 from fnmatch import fnmatch
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Dict, List, Optional
 
 import xmlrunner
 
 import pykiso
 
 from ..exceptions import (
     AuxiliaryCreationError,
@@ -76,17 +77,15 @@
     ONE_OR_MORE_TESTS_FAILED = 1
     ONE_OR_MORE_TESTS_RAISED_UNEXPECTED_EXCEPTION = 2
     ONE_OR_MORE_TESTS_FAILED_AND_RAISED_UNEXPECTED_EXCEPTION = 3
     AUXILIARY_CREATION_FAILED = 4
     BAD_CLI_USAGE = 5
 
 
-def create_test_suite(
-    test_suite_dict: Dict[str, Union[str, int]]
-) -> test_suite.BasicTestSuite:
+def create_test_suite(test_suite_dict: SuiteConfig) -> test_suite.BasicTestSuite:
     """create a test suite based on the config dict
 
     :param test_suite_dict: dict created from config with keys 'suite_dir',
         'test_filter_pattern', 'test_suite_id'
     """
     return test_suite.BasicTestSuite(
         test_suite_dict["suite_dir"],
@@ -143,38 +142,40 @@
     def set_skipped(test_case: BasicTest) -> BasicTest:
         """Set testcase to skipped.
 
         :param test_case: testcase to be skipped
         :return: the skipped testcase as a new instance of the provided
             TestCase subclass.
         """
-        skipped_test_cls = unittest.skip(test_case._skip_msg)(test_case.__class__)
-        return skipped_test_cls()
+        if should_skip(test_case):
+            skipped_test_cls = unittest.skip(test_case._skip_msg)(test_case.__class__)
+            return skipped_test_cls()
+        return test_case
 
     # collect and reformat all CLI and test case tag names
     usr_tags = format_tag_names(usr_tags)
 
     all_test_tags = []
     for tc in test_suite.flatten(all_tests_to_run):
         if getattr(tc, "tag", None) is None:
             continue
         tc.tag = format_tag_names(tc.tag)
         all_test_tags.extend(tc.tag.keys())
 
+    # skip the tests according to the provided CLI tags and the defined test tags
+    list(map(set_skipped, test_suite.flatten(all_tests_to_run)))
+
     # verify that each provided tag name is defined in at least one test case
     all_test_tags = set(all_test_tags)
     for tag_name in usr_tags:
         if tag_name not in all_test_tags:
             raise NameError(
-                f"Provided tag {tag_name!r} is not defined in any testcase."
+                f"Provided tag {tag_name!r} is not defined in any testcase.", tag_name
             )
 
-    # skip the tests according to the provided CLI tags and the defined test tags
-    list(map(set_skipped, filter(should_skip, test_suite.flatten(all_tests_to_run))))
-
 
 def apply_test_case_filter(
     all_tests_to_run: unittest.TestSuite,
     test_class_pattern: str,
     test_case_pattern: str,
 ) -> unittest.TestSuite:
     """Apply a filter to run only test cases which matches given expression
@@ -289,17 +290,17 @@
     file_paths = list(path.glob(pattern))
     for file in file_paths:
         if not VALID_MODULE_NAME.match(file.name):
             raise InvalidTestModuleName(file.name)
 
 
 def collect_test_suites(
-    config_test_suite_list: List[Dict[str, Union[str, int]]],
+    config_test_suite_list: List[SuiteConfig],
     test_filter_pattern: Optional[str] = None,
-) -> List[Optional[test_suite.BasicTestSuite]]:
+) -> List[test_suite.BasicTestSuite]:
     """Collect and load all test suites defined in the test configuration.
 
     :param config_test_suite_list: list of dictionaries from the configuration
         file corresponding each to one test suite.
     :param test_filter_pattern: optional filter pattern to overwrite
         the one defined in the test suite configuration.
 
@@ -335,15 +336,15 @@
     log.critical(
         "Non recoverable error occurred during test execution, aborting test session."
     )
     os.kill(os.getpid(), ExitCode.ONE_OR_MORE_TESTS_RAISED_UNEXPECTED_EXCEPTION)
 
 
 def execute(
-    config: Dict[str, Any],
+    config: ConfigDict,
     report_type: str = "text",
     report_name: str = "",
     user_tags: Optional[Dict[str, List[str]]] = None,
     step_report: Optional[Path] = None,
     pattern_inject: Optional[str] = None,
     failfast: bool = False,
 ) -> int:
```

### Comparing `pykiso-0.22.1/src/pykiso/test_coordinator/test_message_handler.py` & `pykiso-0.22.2/src/pykiso/test_coordinator/test_message_handler.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/test_coordinator/test_suite.py` & `pykiso-0.22.2/src/pykiso/test_coordinator/test_suite.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/test_result/__init__.py` & `pykiso-0.22.2/src/pykiso/test_result/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/test_result/assert_step_report.py` & `pykiso-0.22.2/src/pykiso/test_result/assert_step_report.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/test_result/multi_result.py` & `pykiso-0.22.2/src/pykiso/test_result/multi_result.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/test_result/templates/report_template.css` & `pykiso-0.22.2/src/pykiso/test_result/templates/report_template.css`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/test_result/templates/report_template.html.j2` & `pykiso-0.22.2/src/pykiso/test_result/templates/report_template.html.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 <!DOCTYPE html>
 <html>
 <body>
     <div class="navbar-header" style = " background-color: rgb(255, 255, 255); margin:0; padding:0;">
         <img src = "https://github.com/eclipse/kiso-testing/raw/master/docs/images/pykiso_logo.png" alt = "Pykiso report" width="15%" height="15%">
     </div>
+    <div class="button-container">
+        <button id="failButton">Toggle failed tests</button>
+        <button id="allButton">Toggle all tests</button>
+    </div>
     {# For each TestClass -#}
     {% for class_name, class_content in ALL_STEP_REPORT.items() -%}
         <hr>
-        <div class="col-12 text-left">
+        {% if class_content["succeed"] -%}
+                <details class="hide-marker col-12 text-left">
+        {% else -%}
+                <details open class="hide-marker col-12 text-left failed-test-details">
+        {%- endif %}
             {# Add Title and description -#}
-            <h2>ITF Test Report for:  <a href="{{class_content["file_path"]}}">{{class_name}}</a>
+            <summary style="list-style: none;"><h2>ITF Test Report for:  <a href="{{class_content["file_path"]}}">{{class_name}}</a>
             {% if class_content["succeed"] -%}
                 -> [<span style="color:green;">Success</span>]
             {% else -%}
                 -> [<span style="color:red;">Fail</span>]
             {%- endif %}
-            </h2>
+            </h2></summary>
             <h3>Test Description:</h3>
             <p>{{class_content["description"] | replace("\n", "<br/>\n") }}</p>
             <h3>Date, Time, Software versions:</h3>
             <p>
             {# Add additional information from header key -#}
             {% for data in [class_content["time_result"], class_content["header"]] -%}
                 {% for key, value in data.items() -%}
                     <u>{{key}}</u>: {{value}}</br>
                 {%- endfor %}
             {%- endfor %}
             </p>
             {#- For each test (setUp, run, tearDown) -#}
             {% for test_name, test_content in class_content["test_list"].items() %}
                 {% set test_success = is_test_success(test_content) -%}
-                <details {% if not test_success %}open{% endif %}><summary><h3>{{test_name}}
+                <details {% if not test_success %}open class="failed-test-details"{% endif %}><summary><h3>{{test_name}}
                 {% if test_success -%}<span style="color:green;">Success</span>
                 {% else %}<span style="color:red;">Fail</span>
                 {%- endif %}</h3></summary>
                 <p>{{test_content["description"] | replace("\n", "<br/>\n") }}</p>
                 <table>
                     <thead>
                         <tr>
@@ -89,15 +97,16 @@
                         {% for error in test_content.get("unexpected_errors") -%}
                             <pre>{{error}}</pre>
                         {%- endfor %}
 
                 {%- endif %}
                 </details>
             {%- endfor %}
-        </div>
+
+        </details>
     {%- endfor %}
 </body>
 </html>
 
 <style type="text/css">
 {% include "templates/report_template.css" %}
 </style>
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
 [Pykiso report]
+Toggle failed tests Toggle all tests
 {# For each TestClass -#} {% for class_name, class_content in
 ALL_STEP_REPORT.items() -%}
 ===============================================================================
-{# Add Title and description -#}
+{% if class_content["succeed"] -%}  {% else -%}  {%- endif %} {# Add Title and
+description -#}
 ***** ITF Test Report for: ]}}">{{class_name}} {% if class_content["succeed"] -
 %} -> [Success] {% else -%} -> [Fail] {%- endif %} *****
 **** Test Description: ****
 {{class_content["description"] | replace("\n", "
 \n") }}
 **** Date, Time, Software versions: ****
 {# Add additional information from header key -#} {% for data in [class_content
 ["time_result"], class_content["header"]] -%} {% for key, value in data.items()
 -%} {{key}}: {{value}} {%- endfor %} {%- endfor %}
 {#- For each test (setUp, run, tearDown) -#} {% for test_name, test_content in
 class_content["test_list"].items() %} {% set test_success = is_test_success
 (test_content) -%}
-% if not test_success %}open{% endif %}>
+% if not test_success %}open class="failed-test-details"{% endif %}>
 **** {{test_name}} {% if test_success -%}Success {% else %}Fail {%- endif %}
 ****
 {{test_content["description"] | replace("\n", "
 \n") }}
 Step           {{column_name}}
 {{loop.index}}
 {% if test_content.get("unexpected_errors") -%} Unexpected errors happened :
  {% for error in test_content.get("unexpected_errors") -%}
 {{error}}
-{%- endfor %} {%- endif %}  {%- endfor %}
-{%- endfor %}
+{%- endfor %} {%- endif %}  {%- endfor %}  {%- endfor %}
```

### Comparing `pykiso-0.22.1/src/pykiso/test_result/text_result.py` & `pykiso-0.22.2/src/pykiso/test_result/text_result.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/test_result/xml_result.py` & `pykiso-0.22.2/src/pykiso/test_result/xml_result.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/test_setup/config_registry.py` & `pykiso-0.22.2/src/pykiso/test_setup/config_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,15 @@
 
     @classmethod
     def delete_aux_con(cls) -> None:
         """Deregister the import hooks, close all running threads,
         delete all instances.
         """
         cls._linker.uninstall()
+        cls._linker = None
 
     @classmethod
     def get_all_auxes(cls) -> Dict[AuxiliaryAlias, AuxiliaryCommon]:
         """Return all auxiliaires instances and alias
 
         :return: dictionary with alias as keys and instances as values
         """
```

### Comparing `pykiso-0.22.1/src/pykiso/test_setup/dynamic_loader.py` & `pykiso-0.22.2/src/pykiso/test_setup/dynamic_loader.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/tool/pykiso_to_pytest/cli.py` & `pykiso-0.22.2/src/pykiso/tool/pykiso_to_pytest/cli.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2` & `pykiso-0.22.2/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/tool/show_tag.py` & `pykiso-0.22.2/src/pykiso/tool/show_tag.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/tool/testrail/api.py` & `pykiso-0.22.2/src/pykiso/tool/testrail/api.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/tool/testrail/cli.py` & `pykiso-0.22.2/src/pykiso/tool/testrail/cli.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/tool/testrail/console.py` & `pykiso-0.22.2/src/pykiso/tool/testrail/console.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/tool/testrail/containers.py` & `pykiso-0.22.2/src/pykiso/tool/testrail/containers.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/tool/testrail/extraction.py` & `pykiso-0.22.2/src/pykiso/tool/testrail/extraction.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/tool/testrail/testrail.py` & `pykiso-0.22.2/src/pykiso/tool/testrail/testrail.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/src/pykiso/types.py` & `pykiso-0.22.2/src/pykiso/types.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.1/setup.py` & `pykiso-0.22.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
  'pykiso.lib.auxiliaries.instrument_control_auxiliary',
  'pykiso.lib.auxiliaries.simulated_auxiliary',
  'pykiso.lib.auxiliaries.udsaux',
  'pykiso.lib.auxiliaries.udsaux.common',
  'pykiso.lib.connectors',
  'pykiso.lib.connectors.cc_socket_can',
  'pykiso.lib.robot_framework',
+ 'pykiso.pytest_plugin',
  'pykiso.test_coordinator',
  'pykiso.test_result',
  'pykiso.test_setup',
  'pykiso.tool',
  'pykiso.tool.pykiso_to_pytest',
  'pykiso.tool.testrail']
 
@@ -68,19 +69,20 @@
 
 entry_points = \
 {'console_scripts': ['instrument-control = '
                      'pykiso.lib.auxiliaries.instrument_control_auxiliary.instrument_control_cli:main',
                      'pykiso = pykiso.cli:main',
                      'pykiso-tags = pykiso.tool.show_tag:main',
                      'pykitest = pykiso.tool.pykiso_to_pytest.cli:main',
-                     'testrail = pykiso.tool.testrail.cli:cli_testrail']}
+                     'testrail = pykiso.tool.testrail.cli:cli_testrail'],
+ 'pytest11': ['pytest_kiso = pykiso.pytest_plugin']}
 
 setup_kwargs = {
     'name': 'pykiso',
-    'version': '0.22.1',
+    'version': '0.22.2',
     'description': 'Embedded integration testing framework.',
     'long_description': '[![License](https://img.shields.io/badge/Licence-Eclipse%20Public%20License%202.0-lightgrey)](https://opensource.org/licenses/EPL-2.0)\n[![Platforms](https://img.shields.io/badge/Platforms-win64%20linux64%20osx64-lightgrey)]()\n[![Supported python version](https://img.shields.io/pypi/pyversions/pykiso)]()\n[![Build status](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)\n[![Documentation Status](https://readthedocs.org/projects/kiso-testing/badge/?version=latest)](https://kiso-testing.readthedocs.io/en/latest/?badge=latest)\n[![Test results](https://img.shields.io/jenkins/tests?compact_message&failed_label=failed&jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F&passed_label=passed&skipped_label=skipped)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)\n[![codecov](https://codecov.io/gh/eclipse/kiso-testing/branch/master/graph/badge.svg?token=IBKQ700ABS)](https://codecov.io/gh/eclipse/kiso-testing)\n[![CodeFactor](https://www.codefactor.io/repository/github/eclipse/kiso-testing/badge)](https://www.codefactor.io/repository/github/eclipse/kiso-testing)\n[![Last commit](https://img.shields.io/github/last-commit/eclipse/kiso-testing)]()\n[![Commits since latest version](https://img.shields.io/github/commits-since/eclipse/kiso-testing/latest/master)]()\n\n# PyKiso\n\n![Optional Text](./docs/images/pykiso_logo.png)\n\n## Introduction ##\n\n**pykiso** is an integration test framework. With it, it is possible to write\n* Whitebox integration tests directly on my target device\n* Graybox integration tests to make sure the communication-link with my target device is working as expected\n* Blackbox integration tests to make sure my external device interfaces are working as expected\n\nThe project will contain:\n* The core python framework (this repository)\n* Framework plugins that are generic enough to be integrated as "native" (this repository)\n* Additional "testApps" for different targets platforms (e.g. stm32, ...) or languages (C, C++, ...) . It could be pure SW or also HW (other repositories)\n\n## Link to Eclipse Project\nhttps://projects.eclipse.org/projects/iot.kiso-testing\n\n## Requirements ##\n\n* Python 3.7+\n* pip/poetry (used to get the rest of the requirements)\n\n## Install ##\n\n```bash\npip install pykiso # Core framework\npip install pykiso[plugins] # For installing all plugins\npip install pykiso[all] # For installing all what we have to offer\n```\n\n[Poetry](https://python-poetry.org/) is more appropriate for developers as it automatically creates virtual environments.\n\n```bash\ncd kiso-testing\npoetry install --all-extras\npoetry shell\n```\n\n### Pre-Commit\n\nTo improve code-quality, a configuration of [pre-commit](https://pre-commit.com/) hooks are available.\nThe following pre-commit hooks are used:\n\n- black\n- flake8\n- isort\n- trailing-whitespace\n- end-of-file-fixer\n- check-docstring-first\n- check-json\n- check-added-large-files\n- check-yaml\n- debug-statements\n\nIf you don\'t have pre-commit installed, you can get it using pip:\n\n```bash\npip install pre-commit\n```\n\nStart using the hooks with\n\n```bash\npre-commit install\n```\n\n## Commit message convention\n\nCommits are sorted into multiple categories based on keywords that can occur at any position as part of the commit message.\n[Category] Keywords\n* [BREAKING CHANGES] BREAKING CHANGE\n* [Features] feat:\n* [Fixes] fix:\n* [Docs] docs:\n* [Styles] style:\n* [Refactors] refactor!:\n* [Performances] perf:\n* [Tests] test:\n* [Build] build:\n* [Ci] ci:\nEach commit is considered only once according to the order of the categories listed above. Merge commits are ignored.\n\nThe tool commitizen can help you to create commits which follows these standards.\n```bash\n# if not yet installed:\npip install -U commitizen==2.20.4\n# helps you to create a commit:\ncz commit\n# or use equivalent short variant:\ncz c\n```\n\n## Generate Changelog\n\nAfter you installed the dev dependencies from the pipfile you are able to\nautogenerate the Changelog.\n\n```bash\ninvoke changelog\n```\n\n## Usage ##\n\nOnce installed the application is bound to `pykiso`, it can be called with the following arguments:\n\n```bash\nUsage: pykiso [OPTIONS]\n\n  Embedded Integration Test Framework - CLI Entry Point.\n\n  TAG Filters: any additional option to be passed to the test as tag through\n  the pykiso call. Multiple values must be separated with a comma.\n\n  For example: pykiso -c your_config.yaml --branch-level dev,master --variant\n  delta\n\nOptions:\n  -c, --test-configuration-file FILE\n                                  path to the test configuration file (in YAML\n                                  format)  [required]\n  -l, --log-path PATH             path to log-file or folder. If not set will\n                                  log to STDOUT\n  --log-level [DEBUG|INFO|WARNING|ERROR]\n                                  set the verbosity of the logging\n  --junit                         enables the generation of a junit report\n  --text                          default, test results are only displayed in\n                                  the console\n  --step-report PATH              generate the step report at the specified\n                                  path\n  --failfast                      stop the test run on the first error or\n                                  failure\n  -v, --verbose                   activate the internal framework logs\n  -p, --pattern TEXT              test filter pattern, e.g. \'test_suite_1.py\'\n                                  or \'test_*.py\'. Or even more granularly\n                                  \'test_suite_1.py::test_class::test_name\'\n  --version                       Show the version and exit.\n  -h, --help                      Show this message and exit.\n```\n\nSuitable config files are available in the `examples` folder.\n\n### Demo using example config ##\n\n```bash\ninvoke run\n```\n\n### Running the Tests ##\n\n```bash\ninvoke test\n```\n\nor\n\n```bash\npytest\n```\n',
     'author': 'Sebastian Fischer',
     'author_email': 'sebastian.fischer@de.bosch.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pypi.org/project/pykiso/',
```

### Comparing `pykiso-0.22.1/PKG-INFO` & `pykiso-0.22.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykiso
-Version: 0.22.1
+Version: 0.22.2
 Summary: Embedded integration testing framework.
 Home-page: https://pypi.org/project/pykiso/
 License: Eclipse Public License - v 2.0
 Keywords: testing,integration testing,framework,testing framework
 Author: Sebastian Fischer
 Author-email: sebastian.fischer@de.bosch.com
 Requires-Python: >=3.7,<4.0
```

