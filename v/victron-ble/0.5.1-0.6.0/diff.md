# Comparing `tmp/victron_ble-0.5.1.tar.gz` & `tmp/victron_ble-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "victron_ble-0.5.1.tar", last modified: Sun Mar  5 05:54:40 2023, max compression
+gzip compressed data, was "victron_ble-0.6.0.tar", last modified: Wed Jun 21 00:59:44 2023, max compression
```

## Comparing `victron_ble-0.5.1.tar` & `victron_ble-0.6.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 05:54:40.976067 victron_ble-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-05 05:54:30.000000 victron_ble-0.5.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-05 05:54:30.000000 victron_ble-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-05 05:54:30.000000 victron_ble-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-03-05 05:54:40.976067 victron_ble-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-03-05 05:54:30.000000 victron_ble-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 05:54:40.976067 victron_ble-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-05 05:54:30.000000 victron_ble-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 05:54:40.972067 victron_ble-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 05:54:30.000000 victron_ble-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-05 05:54:30.000000 victron_ble-0.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-05 05:54:30.000000 victron_ble-0.5.1/tests/test_battery_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-05 05:54:30.000000 victron_ble-0.5.1/tests/test_battery_sense.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-05 05:54:30.000000 victron_ble-0.5.1/tests/test_dc_energy_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-05 05:54:30.000000 victron_ble-0.5.1/tests/test_dcdc_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-05 05:54:30.000000 victron_ble-0.5.1/tests/test_device_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-05 05:54:30.000000 victron_ble-0.5.1/tests/test_solar_charger.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-05 05:54:30.000000 victron_ble-0.5.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 05:54:40.972067 victron_ble-0.5.1/victron_ble/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-05 05:54:30.000000 victron_ble-0.5.1/victron_ble/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 05:54:30.000000 victron_ble-0.5.1/victron_ble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-03-05 05:54:30.000000 victron_ble-0.5.1/victron_ble/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 05:54:40.976067 victron_ble-0.5.1/victron_ble/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-05 05:54:30.000000 victron_ble-0.5.1/victron_ble/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-03-05 05:54:30.000000 victron_ble-0.5.1/victron_ble/devices/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-03-05 05:54:30.000000 victron_ble-0.5.1/victron_ble/devices/battery_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-05 05:54:30.000000 victron_ble-0.5.1/victron_ble/devices/battery_sense.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-03-05 05:54:30.000000 victron_ble-0.5.1/victron_ble/devices/dc_energy_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-05 05:54:30.000000 victron_ble-0.5.1/victron_ble/devices/dcdc_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-03-05 05:54:30.000000 victron_ble-0.5.1/victron_ble/devices/solar_charger.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-05 05:54:30.000000 victron_ble-0.5.1/victron_ble/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-03-05 05:54:30.000000 victron_ble-0.5.1/victron_ble/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 05:54:40.972067 victron_ble-0.5.1/victron_ble.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-03-05 05:54:40.000000 victron_ble-0.5.1/victron_ble.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-05 05:54:40.000000 victron_ble-0.5.1/victron_ble.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 05:54:40.000000 victron_ble-0.5.1/victron_ble.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-05 05:54:40.000000 victron_ble-0.5.1/victron_ble.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-05 05:54:40.000000 victron_ble-0.5.1/victron_ble.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-05 05:54:40.000000 victron_ble-0.5.1/victron_ble.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:59:44.768318 victron_ble-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-21 00:59:30.000000 victron_ble-0.6.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-21 00:59:30.000000 victron_ble-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 00:59:30.000000 victron_ble-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-21 00:59:44.768318 victron_ble-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-06-21 00:59:30.000000 victron_ble-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 00:59:44.768318 victron_ble-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-21 00:59:30.000000 victron_ble-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:59:44.768318 victron_ble-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 00:59:30.000000 victron_ble-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-21 00:59:30.000000 victron_ble-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-21 00:59:30.000000 victron_ble-0.6.0/tests/test_battery_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-21 00:59:30.000000 victron_ble-0.6.0/tests/test_battery_sense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-21 00:59:30.000000 victron_ble-0.6.0/tests/test_dc_energy_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-21 00:59:30.000000 victron_ble-0.6.0/tests/test_dcdc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-21 00:59:30.000000 victron_ble-0.6.0/tests/test_device_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-21 00:59:30.000000 victron_ble-0.6.0/tests/test_solar_charger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-21 00:59:30.000000 victron_ble-0.6.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-21 00:59:30.000000 victron_ble-0.6.0/tests/test_vebus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:59:44.768318 victron_ble-0.6.0/victron_ble/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 00:59:30.000000 victron_ble-0.6.0/victron_ble/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 00:59:30.000000 victron_ble-0.6.0/victron_ble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-21 00:59:30.000000 victron_ble-0.6.0/victron_ble/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:59:44.768318 victron_ble-0.6.0/victron_ble/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-21 00:59:30.000000 victron_ble-0.6.0/victron_ble/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-06-21 00:59:30.000000 victron_ble-0.6.0/victron_ble/devices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-21 00:59:30.000000 victron_ble-0.6.0/victron_ble/devices/battery_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-21 00:59:30.000000 victron_ble-0.6.0/victron_ble/devices/battery_sense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-21 00:59:30.000000 victron_ble-0.6.0/victron_ble/devices/dc_energy_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-21 00:59:30.000000 victron_ble-0.6.0/victron_ble/devices/dcdc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-21 00:59:30.000000 victron_ble-0.6.0/victron_ble/devices/solar_charger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-06-21 00:59:30.000000 victron_ble-0.6.0/victron_ble/devices/vebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-21 00:59:30.000000 victron_ble-0.6.0/victron_ble/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-21 00:59:30.000000 victron_ble-0.6.0/victron_ble/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:59:44.768318 victron_ble-0.6.0/victron_ble.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-21 00:59:44.000000 victron_ble-0.6.0/victron_ble.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-21 00:59:44.000000 victron_ble-0.6.0/victron_ble.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:59:44.000000 victron_ble-0.6.0/victron_ble.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 00:59:44.000000 victron_ble-0.6.0/victron_ble.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-21 00:59:44.000000 victron_ble-0.6.0/victron_ble.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 00:59:44.000000 victron_ble-0.6.0/victron_ble.egg-info/top_level.txt
```

### Comparing `victron_ble-0.5.1/HISTORY.md` & `victron_ble-0.6.0/HISTORY.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+0.6.0 (2023)
+------------------
+- Add VEBus support
+- Improve readme 
+
 0.5.1 (2023)
 ------------------
 - Fix DC/DC output voltage when off
 
 0.5.0 (2023)
 ------------------
 - Add DC/DC charger support
```

### Comparing `victron_ble-0.5.1/LICENSE` & `victron_ble-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `victron_ble-0.5.1/PKG-INFO` & `victron_ble-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: victron_ble
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python API to read Victron Instant Readout advertisements
 Home-page: https://github.com/keshavdv/victron-ble/
 Author: keshavdv
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
@@ -49,24 +49,40 @@
 
 To be able to decrypt the contents of the advertisement, you'll need to first fetch the per-device encryption key from the official Victron application. The method to do this will vary per platform, instructions below:
 
 #### Fetching Keys
  
 **OSX**
 
+[MacOS's bleak backend](https://bleak.readthedocs.io/en/latest/backends/macos.html) uses a bluetooth UUID address instead of the more traditional MAC address to identify bluetooth devices. This UUID address is often unique to the device scanned *and* the device being scanned such that it cannot be used to connect to the same device from another computer. 
+
+If you are going to use `victron-ble` on the same Mac computer as you have the Victron app on, follow the instructions below to retrieve the address UUID and advertisement key:
+
 1. Install the Victron app from the Mac App Store
 2. Pair with your device at least once to transfer keys
 3. Run the following from Terminal to dump the known keys (install `sqlite3` via Homebrew)
 ```bash
 ❯ sqlite3 ~/Library/Containers/com.victronenergy.victronconnect.mac/Data/Library/Application\ Support/Victron\ Energy/Victron\ Connect/d25b6546b47ebb21a04ff86a2c4fbb76.sqlite 'select address,advertisementKey from advertisementKeys inner join macAddresses on advertisementKeys.macAddress == macAddresses.macAddress'
 
 {763aeff5-1334-e64a-ab30-a0f478s20fe1}|0df4d0395b7d1a876c0c33ecb9e70dcd
 ❯
 ```
 
+If you are going to use `victron-ble` on a different non-MacOS computer than the one with the Victron app (e.g. on a Raspberry Pi), follow these instructions to obtain the bluetooth MAC address and advertisement key instead:
+
+1. Install the Victron app from the Mac App Store
+2. Pair with your device at least once to transfer keys
+3. Run the following from Terminal to dump the known keys (install `sqlite3` via Homebrew)
+```bash
+❯ sqlite3 ~/Library/Containers/com.victronenergy.victronconnect.mac/Data/Library/Application\ Support/Victron\ Energy/Victron\ Connect/d25b6546b47ebb21a04ff86a2c4fbb76.sqlite 'select macAddress,advertisementKey from advertisementKeys'
+
+a0f478020fe1|0df4d0395b7d1a876c0c33ecb9e70dcd
+❯
+```
+
 **Linux**
 
 1. Download the Victron AppImage app from the Victron website.
 2. Pair with your device at least once to transfer keys
 3. Run the following from a terminal to dump the known keys (install `sqlite3` via your package manager)
 ```bash
 ❯ sqlite3 ~/.local/share/Victron\ Energy/Victron\ Connect/d25b6546b47ebb21a04ff86a2c4fbb76.sqlite 'select address,advertisementKey from advertisementKeys inner join macAddresses on advertisementKeys.macAddress == macAddresses.macAddress'
```

### Comparing `victron_ble-0.5.1/README.md` & `victron_ble-0.6.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -39,24 +39,40 @@
 
 To be able to decrypt the contents of the advertisement, you'll need to first fetch the per-device encryption key from the official Victron application. The method to do this will vary per platform, instructions below:
 
 #### Fetching Keys
  
 **OSX**
 
+[MacOS's bleak backend](https://bleak.readthedocs.io/en/latest/backends/macos.html) uses a bluetooth UUID address instead of the more traditional MAC address to identify bluetooth devices. This UUID address is often unique to the device scanned *and* the device being scanned such that it cannot be used to connect to the same device from another computer. 
+
+If you are going to use `victron-ble` on the same Mac computer as you have the Victron app on, follow the instructions below to retrieve the address UUID and advertisement key:
+
 1. Install the Victron app from the Mac App Store
 2. Pair with your device at least once to transfer keys
 3. Run the following from Terminal to dump the known keys (install `sqlite3` via Homebrew)
 ```bash
 ❯ sqlite3 ~/Library/Containers/com.victronenergy.victronconnect.mac/Data/Library/Application\ Support/Victron\ Energy/Victron\ Connect/d25b6546b47ebb21a04ff86a2c4fbb76.sqlite 'select address,advertisementKey from advertisementKeys inner join macAddresses on advertisementKeys.macAddress == macAddresses.macAddress'
 
 {763aeff5-1334-e64a-ab30-a0f478s20fe1}|0df4d0395b7d1a876c0c33ecb9e70dcd
 ❯
 ```
 
+If you are going to use `victron-ble` on a different non-MacOS computer than the one with the Victron app (e.g. on a Raspberry Pi), follow these instructions to obtain the bluetooth MAC address and advertisement key instead:
+
+1. Install the Victron app from the Mac App Store
+2. Pair with your device at least once to transfer keys
+3. Run the following from Terminal to dump the known keys (install `sqlite3` via Homebrew)
+```bash
+❯ sqlite3 ~/Library/Containers/com.victronenergy.victronconnect.mac/Data/Library/Application\ Support/Victron\ Energy/Victron\ Connect/d25b6546b47ebb21a04ff86a2c4fbb76.sqlite 'select macAddress,advertisementKey from advertisementKeys'
+
+a0f478020fe1|0df4d0395b7d1a876c0c33ecb9e70dcd
+❯
+```
+
 **Linux**
 
 1. Download the Victron AppImage app from the Victron website.
 2. Pair with your device at least once to transfer keys
 3. Run the following from a terminal to dump the known keys (install `sqlite3` via your package manager)
 ```bash
 ❯ sqlite3 ~/.local/share/Victron\ Energy/Victron\ Connect/d25b6546b47ebb21a04ff86a2c4fbb76.sqlite 'select address,advertisementKey from advertisementKeys inner join macAddresses on advertisementKeys.macAddress == macAddresses.macAddress'
```

### Comparing `victron_ble-0.5.1/setup.py` & `victron_ble-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `victron_ble-0.5.1/tests/test_dc_energy_meter.py` & `victron_ble-0.6.0/tests/test_dc_energy_meter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 from victron_ble.devices.battery_monitor import AuxMode
-from victron_ble.devices.dc_energy_meter import DcEnergyMeter, MeterType
+from victron_ble.devices.dc_energy_meter import (
+    DcEnergyMeter,
+    DcEnergyMeterData,
+    MeterType,
+)
 
 
 class TestDcEnergyMeter:
-    def test_parse_data(self) -> None:
+    def test_end_to_end_parse(self) -> None:
         data = "100289a30d787fafde83ccec982199fd815286"
         actual = DcEnergyMeter("aff4d0995b7d1e176c0c33ecb9e70dcd").parse(
             bytes.fromhex(data)
         )
 
+        assert isinstance(actual, DcEnergyMeterData)
         assert actual.get_meter_type() == MeterType.FUEL_CELL
         assert actual.get_aux_mode() == AuxMode.STARTER_VOLTAGE
         assert actual.get_current() == 0.0
         assert actual.get_voltage() == 12.52
         assert actual.get_starter_voltage() == -0.01
 
         assert actual.get_alarm() == None
 
         assert actual.get_temperature() == None
         assert actual.get_model_name() == "SmartShunt 500A/50mV"
 
+    def parse_decrypted(self, decrypted: str) -> DcEnergyMeterData:
+        parsed = DcEnergyMeter(None).parse_decrypted(bytes.fromhex(decrypted))
+        return DcEnergyMeterData(None, parsed)
+
+    def test_parse(self) -> None:
+        actual = self.parse_decrypted("fdffe4040000ffff00000059a65a1c8c")
+        assert actual.get_meter_type() == MeterType.FUEL_CELL
+        assert actual.get_aux_mode() == AuxMode.STARTER_VOLTAGE
+        assert actual.get_current() == 0.0
+        assert actual.get_voltage() == 12.52
+        assert actual.get_starter_voltage() == -0.01
+        assert actual.get_alarm() == None
+        assert actual.get_temperature() == None
+
     def test_aux_starter(self) -> None:
-        data = "100289a30d787fafde83ccec982199fd815286"
-        actual = DcEnergyMeter("aff4d0995b7d1e176c0c33ecb9e70dcd").parse(
-            bytes.fromhex(data)
-        )
+        actual = self.parse_decrypted("fdffe4040000ffff00000059a65a1c8c")
         assert actual.get_starter_voltage() == -0.01
 
     def test_aux_temperature(self) -> None:
-        data = "108289a30df07faf9629bfb8c0153f431362c4"
-        actual = DcEnergyMeter("aff4d0995b7d1e176c0c33ecb9e70dcd").parse(
-            bytes.fromhex(data)
-        )
+        actual = self.parse_decrypted("fdffe4040000ffff020000ae28af8a5c")
         assert actual.get_temperature() == 382.2
```

### Comparing `victron_ble-0.5.1/tests/test_dcdc_converter.py` & `victron_ble-0.6.0/tests/test_dcdc_converter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,32 @@
-from victron_ble.devices.dcdc_converter import DcDcConverter
+from victron_ble.devices.dcdc_converter import DcDcConverter, DcDcConverterData
 from victron_ble.devices.base import OperationMode, OffReason, ChargerError
 
 
 class TestDcDcConverter:
-    def test_parse_data(self) -> None:
+    def test_end_to_end_parse(self) -> None:
         data = "1000c0a304121d64ca8d442b90bbdf6a8cba"
         actual = DcDcConverter("64ba49f1a8562e45197a8e1fe50d7658").parse(
             bytes.fromhex(data)
         )
+        assert isinstance(actual, DcDcConverterData)
 
         assert actual.get_charge_state() == OperationMode.OFF
         assert actual.get_charger_error() == ChargerError.NO_ERROR
         assert actual.get_input_voltage() == 13.15
         assert actual.get_output_voltage() == 0
         assert actual.get_off_reason() == OffReason.ENGINE_SHUTDOWN
         assert (
             actual.get_model_name() == "Orion Smart 12V|12V-18A Isolated DC-DC Charger"
         )
+
+    def parse_decrypted(self, decrypted: str) -> DcDcConverterData:
+        parsed = DcDcConverter(None).parse_decrypted(bytes.fromhex(decrypted))
+        return DcDcConverterData(None, parsed)
+
+    def test_parse(self) -> None:
+        actual = self.parse_decrypted("00002305ff7f80000000cbdd494cc5d1")
+        assert actual.get_charge_state() == OperationMode.OFF
+        assert actual.get_charger_error() == ChargerError.NO_ERROR
+        assert actual.get_input_voltage() == 13.15
+        assert actual.get_output_voltage() == 0
+        assert actual.get_off_reason() == OffReason.ENGINE_SHUTDOWN
```

### Comparing `victron_ble-0.5.1/tests/test_device_discovery.py` & `victron_ble-0.6.0/tests/test_device_discovery.py`

 * *Files identical despite different names*

### Comparing `victron_ble-0.5.1/tests/test_solar_charger.py` & `victron_ble-0.6.0/tests/test_solar_charger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,45 @@
-from victron_ble.devices.solar_charger import SolarCharger
+from victron_ble.devices.solar_charger import SolarCharger, SolarChargerData
 from victron_ble.devices.base import OperationMode
 
 
 class TestSolarChargwer:
-    def test_parse_data(self) -> None:
+    def test_end_to_end_parse(self) -> None:
         data = "100242a0016207adceb37b605d7e0ee21b24df5c"
         actual = SolarCharger("adeccb947395801a4dd45a2eaa44bf17").parse(
             bytes.fromhex(data)
         )
 
+        assert isinstance(actual, SolarChargerData)
         assert actual.get_charge_state() == OperationMode.ABSORPTION
         assert actual.get_battery_voltage() == 13.88
         assert actual.get_battery_charging_current() == 1.4
         assert actual.get_yield_today() == 30
         assert actual.get_solar_power() == 19
         assert actual.get_external_device_load() == 0.0
         assert actual.get_model_name() == "BlueSolar MPPT 75|15"
 
+    def parse_decrypted(self, decrypted: str) -> SolarChargerData:
+        parsed = SolarCharger(None).parse_decrypted(bytes.fromhex(decrypted))
+        return SolarChargerData(None, parsed)
+
+    def test_parse(self) -> None:
+        actual = self.parse_decrypted("04006c050e000300130000fe409ac069")
+        assert actual.get_charge_state() == OperationMode.ABSORPTION
+        assert actual.get_battery_voltage() == 13.88
+        assert actual.get_battery_charging_current() == 1.4
+        assert actual.get_yield_today() == 30
+        assert actual.get_solar_power() == 19
+        assert actual.get_external_device_load() == 0.0
+
     def test_bulk_charge(self) -> None:
-        data = "100242a0015939a26cc2941a491e766be8457386"
-        actual = SolarCharger("a2781bef23aecd48d6b9397350724c67").parse(
-            bytes.fromhex(data)
-        )
+        actual = self.parse_decrypted("0300f80402000200030000fe8c9a5572")
         assert actual.get_charge_state() == OperationMode.BULK
 
     def test_parse_mppt100(self) -> None:
-        data = "100249a0013a399bbb3e36d7237c7687f96e45dc"
-        actual = SolarCharger("9b3509d3d7aba706846214ca64500d0c").parse(
-            bytes.fromhex(data)
-        )
+        actual = self.parse_decrypted("0300fb09650032000901ffff31bc45ad")
         assert actual.get_battery_charging_current() == 10.1
         assert actual.get_battery_voltage() == 25.55
         assert actual.get_charge_state() == OperationMode.BULK
         assert actual.get_solar_power() == 265
         assert actual.get_yield_today() == 500
         assert actual.get_external_device_load() is None
-        assert actual.get_model_name() == "BlueSolar MPPT 100|50 rev2"
```

### Comparing `victron_ble-0.5.1/victron_ble/cli.py` & `victron_ble-0.6.0/victron_ble/cli.py`

 * *Files identical despite different names*

### Comparing `victron_ble-0.5.1/victron_ble/devices/__init__.py` & `victron_ble-0.6.0/victron_ble/devices/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 from typing import Dict, Optional, Type
 
 from construct import Int8ul, Int16ul
 
 from victron_ble.devices.base import Device, DeviceData
-from victron_ble.devices.battery_monitor import AuxMode, BatteryMonitor
-from victron_ble.devices.battery_sense import BatterySense
-from victron_ble.devices.dc_energy_meter import DcEnergyMeter
-from victron_ble.devices.dcdc_converter import DcDcConverter
-from victron_ble.devices.solar_charger import SolarCharger
+from victron_ble.devices.battery_monitor import AuxMode, BatteryMonitor, BatteryMonitorData
+from victron_ble.devices.battery_sense import BatterySense, BatterySenseData
+from victron_ble.devices.dc_energy_meter import DcEnergyMeter, DcEnergyMeterData
+from victron_ble.devices.dcdc_converter import DcDcConverter, DcDcConverterData
+from victron_ble.devices.solar_charger import SolarCharger, SolarChargerData
+from victron_ble.devices.vebus import VEBus, VEBusData
 
 __all__ = [
     "AuxMode",
     "Device",
     "DeviceData",
     "BatteryMonitor",
+    "BatteryMonitorData",
+    "BatterySense",
+    "BatterySenseData",
+    "DcDcConverter",
+    "DcDcConverterData",
     "DcEnergyMeter",
+    "DcEnergyMeterData",
     "SolarCharger",
+    "SolarChargerData",
+    "VEBus",
+    "VEBusData",
 ]
 
 # Add to this list if a device should be forced to use a particular implementation
 # instead of relying on the identifier in the advertisement
 MODEL_PARSER_OVERRIDE: Dict[int, Type[Device]] = {
     0xA3A4: BatterySense,  # Smart Battery Sense
     0xA3A5: BatterySense,  # Smart Battery Sense
@@ -53,10 +63,10 @@
     elif mode == 0xB:  # MultiRS
         pass
     elif mode == 0x5:  # SmartLithium
         pass
     elif mode == 0x1:  # SolarCharger
         return SolarCharger
     elif mode == 0xC:  # VE.Bus
-        pass
+        return VEBus
 
     return None
```

### Comparing `victron_ble-0.5.1/victron_ble/devices/base.py` & `victron_ble-0.6.0/victron_ble/devices/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import abc
 from enum import Enum
-from typing import Any, Dict
+from typing import Any, Dict, Type
 
 from construct import FixedSized, GreedyBytes, Int8sl, Int16ul, Struct
 from Crypto.Cipher import AES
 from Crypto.Util import Counter
 from Crypto.Util.Padding import pad
 
+from victron_ble.exceptions import AdvertisementKeyMismatchError
+
 
 # Sourced from VE.Direct docs
 class OperationMode(Enum):
     OFF = 0
     LOW_POWER = 1
     FAULT = 2
     BULK = 3
@@ -171,14 +173,15 @@
     SWITCHED_OFF_SWITCH = 0x00000002
     SWITCHED_OFF_REGISTER = 0x00000004
     REMOTE_INPUT = 0x00000008
     PROTECTION_ACTIVE = 0x00000010
     PAY_AS_YOU_GO_OUT_OF_CREDIT = 0x00000020
     BMS = 0x00000040
     ENGINE_SHUTDOWN = 0x00000080
+    ENGINE_SHUTDOWN_AND_INPUT_VOLTAGE_LOCKOUT = 0x00000081
     ANALYSING_INPUT_VOLTAGE = 0x00000100
 
 
 class AlarmReason(Enum):
     LOW_VOLTAGE = 1
     HIGH_VOLTAGE = 2
     LOW_SOC = 4
@@ -191,14 +194,22 @@
     DC_RIPPLE = 512
     LOW_V_AC_OUT = 1024
     HIGH_V_AC_OUT = 2048
     SHORT_CIRCUIT = 4096
     BMS_LOCKOUT = 8192
 
 
+# Sourced from Victron extra-manufacturer-data-2022-12-14.pdf
+class ACInState(Enum):
+    AC_IN_1 = 0
+    AC_IN_2 = 1
+    NOT_CONNECTED = 2
+    UNKNOWN = 3
+
+
 # Sourced from VE.Direct docs
 MODEL_ID_MAPPING = {
     0x203: "BMV-700",
     0x204: "BMV-702",
     0x205: "BMV-700H",
     0x0300: "BlueSolar MPPT 70|15",
     0xA040: "BlueSolar MPPT 75|50",
@@ -349,14 +360,15 @@
     0xA3CC: "Orion Smart 24V|48V-8.5A Isolated DC-DC Charger",
     0xA3C5: "Orion Smart 48V|12V-20A Isolated DC-DC Charger",
     0xA3CD: "Orion Smart 48V|12V-30A Isolated DC-DC Charger",
     0xA3C6: "Orion Smart 48V|24V-12A Isolated DC-DC Charger",
     0xA3CE: "Orion Smart 48V|24V-16A Isolated DC-DC Charger",
     0xA3C7: "Orion Smart 48V|48V-6A Isolated DC-DC Charger",
     0xA3CF: "Orion Smart 48V|48V-8.5A Isolated DC-DC Charger",
+    0x2780: "Victron Multiplus II 12/3000/120-50 2x120V",
 }
 
 
 class DeviceData:
     def __init__(self, model_id: int, data: Dict[str, Any]) -> None:
         self._model_id: int = model_id
         self._data: Dict[str, Any] = data
@@ -364,14 +376,16 @@
     def get_model_name(self) -> str:
         return MODEL_ID_MAPPING.get(
             self._model_id, f"<Unknown device: {self._model_id}>"
         )
 
 
 class Device(abc.ABC):
+    data_type: Type[DeviceData] = DeviceData
+
     PARSER = Struct(
         "prefix" / FixedSized(2, GreedyBytes),
         # Model ID
         "model_id" / Int16ul,
         # Packet type
         "readout_type" / Int8sl,
         # IV for encryption
@@ -384,24 +398,35 @@
 
     def get_model_id(self, data: bytes) -> int:
         return self.PARSER.parse(data).model_id
 
     def decrypt(self, data: bytes) -> bytes:
         container = self.PARSER.parse(data)
 
-        # The first byte of advertised data seems to match the first byte of the advertisement key
+        advertisement_key = bytes.fromhex(self.advertisement_key)
+
+        # The first data byte is a key check byte
+        if container.encrypted_data[0] != advertisement_key[0]:
+            raise AdvertisementKeyMismatchError("Incorrect advertisement key")
+
         ctr = Counter.new(128, initial_value=container.iv, little_endian=True)
 
         cipher = AES.new(
-            bytes.fromhex(self.advertisement_key),
+            advertisement_key,
             AES.MODE_CTR,
             counter=ctr,
         )
         return cipher.decrypt(pad(container.encrypted_data[1:], 16))
 
+    def parse(self, data: bytes) -> DeviceData:
+        decrypted = self.decrypt(data)
+        parsed = self.parse_decrypted(decrypted)
+        model = self.get_model_id(data)
+        return self.data_type(model, parsed)
+
     @abc.abstractmethod
-    def parse(self, data: bytes):
+    def parse_decrypted(self, decrypted: bytes) -> dict:
         pass
 
 
 def kelvin_to_celsius(temp_in_kelvin: float) -> float:
     return round(temp_in_kelvin - 273.15, 2)
```

### Comparing `victron_ble-0.5.1/victron_ble/devices/battery_monitor.py` & `victron_ble-0.6.0/victron_ble/devices/battery_monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Optional
+from typing import Optional, Type
 
 from construct import GreedyBytes, Int16sl, Int16ul, Int24sl, Struct
 
 from victron_ble.devices.base import AlarmReason, Device, DeviceData, kelvin_to_celsius
 
 
 class AuxMode(Enum):
@@ -75,14 +75,15 @@
         """
         Return the midpoint battery voltage in volts if the aux input is set to midpoint voltage
         """
         return self._data.get("midpoint_voltage")
 
 
 class BatteryMonitor(Device):
+    data_type: Type[DeviceData] = BatteryMonitorData
     PACKET = Struct(
         # Remaining time in minutes
         "remaining_mins" / Int16ul,
         # Voltage reading in 10mV increments
         "voltage" / Int16ul,
         # Alarm reason
         "alarm" / Int16ul,
@@ -101,16 +102,15 @@
         # The next 8 bits indicate the state of charge in 0.1% increments
         # The upper 2 bits are unknown
         "soc" / Int16ul,
         # Throw away any extra bytes
         GreedyBytes,
     )
 
-    def parse(self, data: bytes) -> BatteryMonitorData:
-        decrypted = self.decrypt(data)
+    def parse_decrypted(self, decrypted: bytes) -> dict:
         pkt = self.PACKET.parse(decrypted)
 
         aux_mode = AuxMode(pkt.current & 0b11)
 
         parsed = {
             "remaining_mins": pkt.remaining_mins,
             "aux_mode": aux_mode,
@@ -127,8 +127,8 @@
                 Int16sl.parse((pkt.aux).to_bytes(2, "little")) / 100
             )
         elif aux_mode == AuxMode.MIDPOINT_VOLTAGE:
             parsed["midpoint_voltage"] = pkt.aux / 100
         elif aux_mode == AuxMode.TEMPERATURE:
             parsed["temperature_kelvin"] = pkt.aux / 100
 
-        return BatteryMonitorData(self.get_model_id(data), parsed)
+        return parsed
```

### Comparing `victron_ble-0.5.1/victron_ble/devices/battery_sense.py` & `victron_ble-0.6.0/victron_ble/devices/battery_sense.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-from victron_ble.devices import BatteryMonitor, Device, DeviceData
+from victron_ble.devices.base import DeviceData, kelvin_to_celsius
+from victron_ble.devices.battery_monitor import BatteryMonitor
 
 
 class BatterySenseData(DeviceData):
     def get_temperature(self) -> float:
         """
         Return the temperature in Celsius
         """
-        return self._data["temperature"]
+        return kelvin_to_celsius(self._data["temperature_kelvin"])
 
     def get_voltage(self) -> float:
         """
         Return the voltage in volts
         """
         return self._data["voltage"]
 
 
-class BatterySense(Device):
-    def parse(self, data: bytes) -> BatterySenseData:
-        parsed = BatteryMonitor(self.advertisement_key).parse(data)
-
-        return BatterySenseData(
-            self.get_model_id(data),
-            {"temperature": parsed.get_temperature(), "voltage": parsed.get_voltage()},
-        )
+class BatterySense(BatteryMonitor):
+    data_type = BatterySenseData
```

### Comparing `victron_ble-0.5.1/victron_ble/devices/dc_energy_meter.py` & `victron_ble-0.6.0/victron_ble/devices/dc_energy_meter.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,16 @@
         """
         Return the starter battery voltage in volts if the aux input is set to starter battery
         """
         return self._data.get("starter_voltage")
 
 
 class DcEnergyMeter(Device):
+    data_type = DcEnergyMeterData
+
     PACKET = Struct(
         "meter_type" / Int16sl,
         # Voltage reading in 10mV increments
         "voltage" / Int16ul,
         # Alarm reason
         "alarm" / Int16ul,
         # Value of the auxillary input
@@ -88,16 +90,15 @@
         #   0 = Starter battery voltage
         #   1 = Midpoint voltage
         #   2 = Temperature
         #   3 = Disabled
         "current" / Int24sl,
     )
 
-    def parse(self, data: bytes) -> DcEnergyMeterData:
-        decrypted = self.decrypt(data)
+    def parse_decrypted(self, decrypted: bytes) -> dict:
         pkt = self.PACKET.parse(decrypted)
 
         aux_mode = AuxMode(pkt.current & 0b11)
 
         parsed = {
             "meter_type": MeterType(pkt.meter_type),
             "aux_mode": aux_mode,
@@ -110,8 +111,8 @@
             # Starter voltage is treated as signed
             parsed["starter_voltage"] = (
                 Int16sl.parse((pkt.aux).to_bytes(2, "little")) / 100
             )
         elif aux_mode == AuxMode.TEMPERATURE:
             parsed["temperature_kelvin"] = pkt.aux / 100
 
-        return DcEnergyMeterData(self.get_model_id(data), parsed)
+        return parsed
```

### Comparing `victron_ble-0.5.1/victron_ble/devices/dcdc_converter.py` & `victron_ble-0.6.0/victron_ble/devices/dcdc_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,16 @@
         """
         Return an error code stating the reason for the output to be off
         """
         return self._data["off_reason"]
 
 
 class DcDcConverter(Device):
+    data_type = DcDcConverterData
+
     PACKET = Struct(
         # Charge State:   0 - Off
         #                 3 - Bulk
         #                 4 - Absorption
         #                 5 - Float
         "device_state" / Int8ul,
         # Charger Error Code
@@ -55,22 +57,19 @@
         # Output voltage in 0.01V
         "output_voltage" / Int16sl,
         # Reason for Charger Off
         "off_reason" / Int32ul,
         GreedyBytes,
     )
 
-    def parse(self, data: bytes) -> DcDcConverterData:
-        decrypted = self.decrypt(data)
+    def parse_decrypted(self, decrypted: bytes) -> dict:
         pkt = self.PACKET.parse(decrypted)
 
-        parsed = {
+        return {
             "device_state": OperationMode(pkt.device_state),
             "charger_error": ChargerError(pkt.charger_error),
             "input_voltage": pkt.input_voltage / 100,
             "output_voltage": 0
             if pkt.output_voltage == 0x7FFF
             else pkt.output_voltage / 100,
             "off_reason": OffReason(pkt.off_reason),
         }
-
-        return DcDcConverterData(self.get_model_id(data), parsed)
```

### Comparing `victron_ble-0.5.1/victron_ble/devices/solar_charger.py` & `victron_ble-0.6.0/victron_ble/devices/solar_charger.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,14 +42,16 @@
         """
         if self._data["external_device_load"] == 0xFFFF:
             return None
         return (self._data["external_device_load"] & 0x01FF) / 10
 
 
 class SolarCharger(Device):
+    data_type = SolarChargerData
+
     PACKET = Struct(
         # Charge State:   0 - Off
         #                 3 - Bulk
         #                 4 - Absorption
         #                 5 - Float
         "charge_state" / Int8ul,
         "charger_error" / Int8ul,
@@ -61,21 +63,20 @@
         "yield_today" / Int16ul,
         # Current power from solar in 1W increments
         "solar_power" / Int16ul,
         # External device load in 0.1A increments
         "external_device_load" / Int16ul,
     )
 
-    def parse(self, data: bytes) -> SolarChargerData:
-        decrypted = self.decrypt(data)
+    def parse_decrypted(self, decrypted: bytes) -> dict:
         pkt = self.PACKET.parse(decrypted)
 
-        parsed = {
+        return {
             "charge_state": OperationMode(pkt.charge_state),
             "battery_voltage": pkt.battery_voltage / 100,
             "battery_charging_current": pkt.battery_charging_current / 10,
             "yield_today": pkt.yield_today * 10,
             "solar_power": pkt.solar_power,
-            "external_device_load": pkt.external_device_load,
+            "external_device_load": 0
+            if pkt.external_device_load == 0x1FF
+            else pkt.external_device_load,
         }
-
-        return SolarChargerData(self.get_model_id(data), parsed)
```

### Comparing `victron_ble-0.5.1/victron_ble/scanner.py` & `victron_ble-0.6.0/victron_ble/scanner.py`

 * *Files identical despite different names*

### Comparing `victron_ble-0.5.1/victron_ble.egg-info/PKG-INFO` & `victron_ble-0.6.0/victron_ble.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: victron-ble
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python API to read Victron Instant Readout advertisements
 Home-page: https://github.com/keshavdv/victron-ble/
 Author: keshavdv
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
@@ -49,24 +49,40 @@
 
 To be able to decrypt the contents of the advertisement, you'll need to first fetch the per-device encryption key from the official Victron application. The method to do this will vary per platform, instructions below:
 
 #### Fetching Keys
  
 **OSX**
 
+[MacOS's bleak backend](https://bleak.readthedocs.io/en/latest/backends/macos.html) uses a bluetooth UUID address instead of the more traditional MAC address to identify bluetooth devices. This UUID address is often unique to the device scanned *and* the device being scanned such that it cannot be used to connect to the same device from another computer. 
+
+If you are going to use `victron-ble` on the same Mac computer as you have the Victron app on, follow the instructions below to retrieve the address UUID and advertisement key:
+
 1. Install the Victron app from the Mac App Store
 2. Pair with your device at least once to transfer keys
 3. Run the following from Terminal to dump the known keys (install `sqlite3` via Homebrew)
 ```bash
 ❯ sqlite3 ~/Library/Containers/com.victronenergy.victronconnect.mac/Data/Library/Application\ Support/Victron\ Energy/Victron\ Connect/d25b6546b47ebb21a04ff86a2c4fbb76.sqlite 'select address,advertisementKey from advertisementKeys inner join macAddresses on advertisementKeys.macAddress == macAddresses.macAddress'
 
 {763aeff5-1334-e64a-ab30-a0f478s20fe1}|0df4d0395b7d1a876c0c33ecb9e70dcd
 ❯
 ```
 
+If you are going to use `victron-ble` on a different non-MacOS computer than the one with the Victron app (e.g. on a Raspberry Pi), follow these instructions to obtain the bluetooth MAC address and advertisement key instead:
+
+1. Install the Victron app from the Mac App Store
+2. Pair with your device at least once to transfer keys
+3. Run the following from Terminal to dump the known keys (install `sqlite3` via Homebrew)
+```bash
+❯ sqlite3 ~/Library/Containers/com.victronenergy.victronconnect.mac/Data/Library/Application\ Support/Victron\ Energy/Victron\ Connect/d25b6546b47ebb21a04ff86a2c4fbb76.sqlite 'select macAddress,advertisementKey from advertisementKeys'
+
+a0f478020fe1|0df4d0395b7d1a876c0c33ecb9e70dcd
+❯
+```
+
 **Linux**
 
 1. Download the Victron AppImage app from the Victron website.
 2. Pair with your device at least once to transfer keys
 3. Run the following from a terminal to dump the known keys (install `sqlite3` via your package manager)
 ```bash
 ❯ sqlite3 ~/.local/share/Victron\ Energy/Victron\ Connect/d25b6546b47ebb21a04ff86a2c4fbb76.sqlite 'select address,advertisementKey from advertisementKeys inner join macAddresses on advertisementKeys.macAddress == macAddresses.macAddress'
```

### Comparing `victron_ble-0.5.1/victron_ble.egg-info/SOURCES.txt` & `victron_ble-0.6.0/victron_ble.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 tests/test_battery_monitor.py
 tests/test_battery_sense.py
 tests/test_dc_energy_meter.py
 tests/test_dcdc_converter.py
 tests/test_device_discovery.py
 tests/test_solar_charger.py
 tests/test_utils.py
+tests/test_vebus.py
 victron_ble/VERSION
 victron_ble/__init__.py
 victron_ble/cli.py
 victron_ble/exceptions.py
 victron_ble/scanner.py
 victron_ble.egg-info/PKG-INFO
 victron_ble.egg-info/SOURCES.txt
@@ -25,8 +26,9 @@
 victron_ble.egg-info/top_level.txt
 victron_ble/devices/__init__.py
 victron_ble/devices/base.py
 victron_ble/devices/battery_monitor.py
 victron_ble/devices/battery_sense.py
 victron_ble/devices/dc_energy_meter.py
 victron_ble/devices/dcdc_converter.py
-victron_ble/devices/solar_charger.py
+victron_ble/devices/solar_charger.py
+victron_ble/devices/vebus.py
```

