# Comparing `tmp/aranet4-2.1.3.tar.gz` & `tmp/aranet4-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aranet4-2.1.3.tar", last modified: Mon Oct 24 03:52:41 2022, max compression
+gzip compressed data, was "dist/aranet4-2.2.0.tar", last modified: Wed Jun 21 20:02:17 2023, max compression
```

## Comparing `aranet4-2.1.3.tar` & `aranet4-2.2.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 anrijs     (501) staff       (20)        0 2022-10-24 03:52:41.713194 aranet4-2.1.3/
--rw-r--r--   0 anrijs     (501) staff       (20)     1071 2022-10-24 03:50:02.000000 aranet4-2.1.3/LICENSE
--rw-r--r--   0 anrijs     (501) staff       (20)     6502 2022-10-24 03:52:41.713054 aranet4-2.1.3/PKG-INFO
--rw-r--r--   0 anrijs     (501) staff       (20)     6079 2022-10-24 03:50:02.000000 aranet4-2.1.3/README.md
-drwxr-xr-x   0 anrijs     (501) staff       (20)        0 2022-10-24 03:52:41.712214 aranet4-2.1.3/aranet4/
--rw-r--r--   0 anrijs     (501) staff       (20)      129 2022-10-24 03:50:56.000000 aranet4-2.1.3/aranet4/__init__.py
--rw-r--r--   0 anrijs     (501) staff       (20)     7888 2022-10-24 03:50:02.000000 aranet4-2.1.3/aranet4/aranetctl.py
--rw-r--r--   0 anrijs     (501) staff       (20)    23341 2022-10-24 03:50:02.000000 aranet4-2.1.3/aranet4/client.py
-drwxr-xr-x   0 anrijs     (501) staff       (20)        0 2022-10-24 03:52:41.712895 aranet4-2.1.3/aranet4.egg-info/
--rw-r--r--   0 anrijs     (501) staff       (20)     6502 2022-10-24 03:52:41.000000 aranet4-2.1.3/aranet4.egg-info/PKG-INFO
--rw-r--r--   0 anrijs     (501) staff       (20)      273 2022-10-24 03:52:41.000000 aranet4-2.1.3/aranet4.egg-info/SOURCES.txt
--rw-r--r--   0 anrijs     (501) staff       (20)        1 2022-10-24 03:52:41.000000 aranet4-2.1.3/aranet4.egg-info/dependency_links.txt
--rw-r--r--   0 anrijs     (501) staff       (20)       61 2022-10-24 03:52:41.000000 aranet4-2.1.3/aranet4.egg-info/entry_points.txt
--rw-r--r--   0 anrijs     (501) staff       (20)       15 2022-10-24 03:52:41.000000 aranet4-2.1.3/aranet4.egg-info/requires.txt
--rw-r--r--   0 anrijs     (501) staff       (20)        8 2022-10-24 03:52:41.000000 aranet4-2.1.3/aranet4.egg-info/top_level.txt
--rw-r--r--   0 anrijs     (501) staff       (20)       38 2022-10-24 03:52:41.713237 aranet4-2.1.3/setup.cfg
--rw-r--r--   0 anrijs     (501) staff       (20)      747 2022-10-24 03:50:48.000000 aranet4-2.1.3/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 20:02:17.000000 aranet4-2.2.0/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 20:02:17.000000 aranet4-2.2.0/aranet4.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)        8 2023-06-21 20:02:16.000000 aranet4-2.2.0/aranet4.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-21 20:02:16.000000 aranet4-2.2.0/aranet4.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)     8239 2023-06-21 20:02:16.000000 aranet4-2.2.0/aranet4.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)       61 2023-06-21 20:02:16.000000 aranet4-2.2.0/aranet4.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       15 2023-06-21 20:02:16.000000 aranet4-2.2.0/aranet4.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      265 2023-06-21 20:02:16.000000 aranet4-2.2.0/aranet4.egg-info/SOURCES.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-21 20:02:17.000000 aranet4-2.2.0/aranet4/
+-rw-r--r--   0 pi        (1000) pi        (1000)      129 2023-06-21 19:58:29.000000 aranet4-2.2.0/aranet4/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    26361 2023-06-21 19:45:41.000000 aranet4-2.2.0/aranet4/client.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     9129 2023-06-21 19:45:41.000000 aranet4-2.2.0/aranet4/aranetctl.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      759 2023-06-21 19:58:21.000000 aranet4-2.2.0/setup.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     8239 2023-06-21 20:02:17.000000 aranet4-2.2.0/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-21 20:02:17.000000 aranet4-2.2.0/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)     6079 2023-06-19 17:40:33.000000 aranet4-2.2.0/README.md
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `aranet4-2.1.3/PKG-INFO` & `aranet4-2.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: aranet4
-Version: 2.1.3
-Summary: Aranet4 Python client
-Home-page: https://github.com/Anrijs/Aranet4-Python
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Aranet4 Python client
 ## Installation
 1. Install aranet4 and its dependencies:
 ```
 pip3 install aranet4
 ```
 2. Pair Aranet4 device
@@ -225,9 +211,7 @@
     begin: int
     end: int
     incl_temperature: bool
     incl_humidity: bool
     incl_pressure: bool
     incl_co2: bool
 ```
-
-
```

### Comparing `aranet4-2.1.3/README.md` & `aranet4-2.2.0/aranet4.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,217 +1,230 @@
-# Aranet4 Python client
-## Installation
-1. Install aranet4 and its dependencies:
-```
-pip3 install aranet4
-```
-2. Pair Aranet4 device
-3. Run `aranetctl` or use as library
-
-**Note:** Smart Home Integrations must be enabled in Aranet4 mobile app for full support.
-
-## aranetctl usage
-```text
-$ aranetctl -h
-usage: aranetctl [-h] [-u URL] [-r] [-s DATE] [-e DATE] [-o FILE] [-w] [-l COUNT]
-                 [--xt] [--xh] [--xp] [--xc]
-                 device_mac
-
-positional arguments:
-  device_mac            Aranet4 Bluetooth Address
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -r, --records         Fetch historical log records
-  --scan                Scan Aranet4 devices
-
-Options for current reading:
-  -u URL, --url URL     Remote url for current value push
-
-Filter History Log Records:
-  -s DATE, --start DATE
-                        Records range start (UTC time, example:
-                        2019-09-29T14:00:00
-  -e DATE, --end DATE   Records range end (UTC time, example: 2019-09-30T14:00:00
-  -o FILE, --output FILE
-                        Save records to a file
-  -w, --wait            Wait until new data point available
-  -l COUNT, --last COUNT
-                        Get <COUNT> last records
-  --xt                  Don't get temperature records
-  --xh                  Don't get humidity records
-  --xp                  Don't get pressure records
-  --xc                  Don't get co2 records
-
-```
-
-### Current Readings Example
-Usage: `aranetctl XX:XX:XX:XX:XX:XX`
-
-Output:
-```
---------------------------------------
-Connected: Aranet4 00000 | v0.3.1
-Updated 51 s ago. Intervals: 60 s
-5040 total readings
---------------------------------------
-CO2:          904 ppm
-Temperature:  19.9 C
-Humidity:     51 %
-Pressure:     997.0 hPa
-Battery:      96 %
-Status Display: GREEN
---------------------------------------
-```
-
-### Get History Example
-Write full log to screen:
-
-Usage: `aranetctl XX:XX:XX:XX:XX:XX -r`
-
-```shell
--------------------------------------------------------------
-Device Name    :        Aranet4 00000
-Device Version :               v0.3.1
--------------------------------------------------------------
- id  |        date         |  co2   | temp | hum | pressure |
--------------------------------------------------------------
-   1 | 2022-02-18T14:15:44 |    844 | 21.8 |  50 |    985.6 |
-   2 | 2022-02-18T14:20:44 |    846 | 21.8 |  50 |    985.9 |
-   3 | 2022-02-18T14:25:44 |    843 | 22.0 |  50 |    986.4 |
-   4 | 2022-02-18T14:30:44 |    881 | 22.1 |  50 |    986.4 |
-   5 | 2022-02-18T14:35:44 |    854 | 22.1 |  50 |    987.3 |
-   6 | 2022-02-18T14:40:44 |    867 | 22.2 |  50 |    987.5 |
-   7 | 2022-02-18T14:45:44 |    883 | 22.1 |  50 |    988.1 |
-   8 | 2022-02-18T14:50:44 |    921 | 22.1 |  50 |    988.6 |
-   9 | 2022-02-18T14:55:44 |    930 | 22.0 |  50 |    989.1 |
-  10 | 2022-02-18T15:00:44 |    954 | 22.0 |  50 |    989.5 |
--------------------------------------------------------------
-```
-
-Usage: `aranetctl XX:XX:XX:XX:XX:XX -r -o aranet4.csv`
-
-Output file format: `Date,CO2,Temperature,Humidity,Pressure`
-
-Output file example:
-```
-date,co2,temperature,humidity,pressure
-2022-02-18 10:05:47,1398,23.2,53,986.6
-2022-02-18 10:10:47,1155,23.1,50,986.3
-```
-
-## Usage of library
-
-### Current Readings Example
-
-```python
-import aranet4
-
-device_mac = "XX:XX:XX:XX:XX:XX"
-
-current = aranet4.client.get_current_readings(device_mac)
-
-print("co2 reading:", current.co2)
-print("Temperature:", current.temperature)
-print("Humidity:", current.humidity)
-print("Pressure:", current.pressure)
-```
-
-### Scanner Example
-Usage: `aranetctl --scan`
-
-Output:
-```
-=======================================
-  Name:     Aranet4 00000
-  Address:  XX:XX:XX:XX:XX:XX
-  RSSI:     -85 dBm
---------------------------------------
-  CO2:           662 pm
-  Temperature:   21.9 °C
-  Humidity:      48 %
-  Pressure:      1019.2 hPa
-  Battery:       34 %
-  Status disp.:  GREEN
-
-=======================================
-  Name:     Aranet4 00001
-  Address:  XX:XX:XX:XX:XX:XX
-  RSSI:     -91 dBm
-
-```
-
-**Note:** To receive current measurements, Smart Home Integrations must be enabled and firmware version must be v1.2.0 or newer.
-
-### Logged Readings Example
-
-```python
-import aranet4
-
-device_mac = "XX:XX:XX:XX:XX:XX"
-
-history = aranet4.client.get_all_records(
-    device_mac, entry_filter={"humi": False, "pres": False}
-)
-print(f"{'Date':^20} | {'CO2':^10} | {'Temperature':^10} ")
-for entry in history.value:
-    print(f"{entry.date.isoformat():^20} | {entry.co2:^10} | {entry.temperature:^10}")
-
-```
-
-## Library functions
-### get_current_readings(mac_address: str) -> client.CurrentReading
-Get current measurements from device
-Returns **CurrentReading** object:
-```python
-class CurrentReading:
-    name: str = ""
-    version: str = ""
-    temperature: float = -1
-    humidity: int = -1
-    pressure: float = -1
-    co2: int = -1
-    battery: int = -1
-    status: int = -1
-    interval: int = -1
-    ago: int = -1
-    stored: int = -1
-```
-
-### get_all_records(mac_address: str, entry_filter: dict) -> client.Record
-Get stored datapoints from device. Apply any filters if required
-
-`entry_filter` is a dictionary that can have the following values:
- - `last`: int : Get last n entries
- - `start`: datetime : Get entries after specified time
- - `end`: datetime : Get entries before specified time
- - `temp`: bool : Get temperature data points (default = True)
- - `humi`: bool : Get humidity data points (default = True)
- - `pres`: bool : Get pressure data points (default = True)
- - `co2`: bool : Get co2 data points (default = True)
-
-Returns **CurrentReading** object:
-```python
-class Record:
-    name: str
-    version: str
-    records_on_device: int
-    filter: Filter
-    value: List[RecordItem] = field(default_factory=list)
-```
-Which includes these objects:
-```python
-class RecordItem:
-    date: datetime
-    temperature: float
-    humidity: int
-    pressure: float
-    co2: int
-
-class Filter:
-    begin: int
-    end: int
-    incl_temperature: bool
-    incl_humidity: bool
-    incl_pressure: bool
-    incl_co2: bool
-```
+Metadata-Version: 2.1
+Name: aranet4
+Version: 2.2.0
+Summary: Aranet4 and Aranet2 Python client
+Home-page: https://github.com/Anrijs/Aranet4-Python
+License: UNKNOWN
+Description: # Aranet4 Python client
+        ## Installation
+        1. Install aranet4 and its dependencies:
+        ```
+        pip3 install aranet4
+        ```
+        2. Pair Aranet4 device
+        3. Run `aranetctl` or use as library
+        
+        **Note:** Smart Home Integrations must be enabled in Aranet4 mobile app for full support.
+        
+        ## aranetctl usage
+        ```text
+        $ aranetctl -h
+        usage: aranetctl [-h] [-u URL] [-r] [-s DATE] [-e DATE] [-o FILE] [-w] [-l COUNT]
+                         [--xt] [--xh] [--xp] [--xc]
+                         device_mac
+        
+        positional arguments:
+          device_mac            Aranet4 Bluetooth Address
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          -r, --records         Fetch historical log records
+          --scan                Scan Aranet4 devices
+        
+        Options for current reading:
+          -u URL, --url URL     Remote url for current value push
+        
+        Filter History Log Records:
+          -s DATE, --start DATE
+                                Records range start (UTC time, example:
+                                2019-09-29T14:00:00
+          -e DATE, --end DATE   Records range end (UTC time, example: 2019-09-30T14:00:00
+          -o FILE, --output FILE
+                                Save records to a file
+          -w, --wait            Wait until new data point available
+          -l COUNT, --last COUNT
+                                Get <COUNT> last records
+          --xt                  Don't get temperature records
+          --xh                  Don't get humidity records
+          --xp                  Don't get pressure records
+          --xc                  Don't get co2 records
+        
+        ```
+        
+        ### Current Readings Example
+        Usage: `aranetctl XX:XX:XX:XX:XX:XX`
+        
+        Output:
+        ```
+        --------------------------------------
+        Connected: Aranet4 00000 | v0.3.1
+        Updated 51 s ago. Intervals: 60 s
+        5040 total readings
+        --------------------------------------
+        CO2:          904 ppm
+        Temperature:  19.9 C
+        Humidity:     51 %
+        Pressure:     997.0 hPa
+        Battery:      96 %
+        Status Display: GREEN
+        --------------------------------------
+        ```
+        
+        ### Get History Example
+        Write full log to screen:
+        
+        Usage: `aranetctl XX:XX:XX:XX:XX:XX -r`
+        
+        ```shell
+        -------------------------------------------------------------
+        Device Name    :        Aranet4 00000
+        Device Version :               v0.3.1
+        -------------------------------------------------------------
+         id  |        date         |  co2   | temp | hum | pressure |
+        -------------------------------------------------------------
+           1 | 2022-02-18T14:15:44 |    844 | 21.8 |  50 |    985.6 |
+           2 | 2022-02-18T14:20:44 |    846 | 21.8 |  50 |    985.9 |
+           3 | 2022-02-18T14:25:44 |    843 | 22.0 |  50 |    986.4 |
+           4 | 2022-02-18T14:30:44 |    881 | 22.1 |  50 |    986.4 |
+           5 | 2022-02-18T14:35:44 |    854 | 22.1 |  50 |    987.3 |
+           6 | 2022-02-18T14:40:44 |    867 | 22.2 |  50 |    987.5 |
+           7 | 2022-02-18T14:45:44 |    883 | 22.1 |  50 |    988.1 |
+           8 | 2022-02-18T14:50:44 |    921 | 22.1 |  50 |    988.6 |
+           9 | 2022-02-18T14:55:44 |    930 | 22.0 |  50 |    989.1 |
+          10 | 2022-02-18T15:00:44 |    954 | 22.0 |  50 |    989.5 |
+        -------------------------------------------------------------
+        ```
+        
+        Usage: `aranetctl XX:XX:XX:XX:XX:XX -r -o aranet4.csv`
+        
+        Output file format: `Date,CO2,Temperature,Humidity,Pressure`
+        
+        Output file example:
+        ```
+        date,co2,temperature,humidity,pressure
+        2022-02-18 10:05:47,1398,23.2,53,986.6
+        2022-02-18 10:10:47,1155,23.1,50,986.3
+        ```
+        
+        ## Usage of library
+        
+        ### Current Readings Example
+        
+        ```python
+        import aranet4
+        
+        device_mac = "XX:XX:XX:XX:XX:XX"
+        
+        current = aranet4.client.get_current_readings(device_mac)
+        
+        print("co2 reading:", current.co2)
+        print("Temperature:", current.temperature)
+        print("Humidity:", current.humidity)
+        print("Pressure:", current.pressure)
+        ```
+        
+        ### Scanner Example
+        Usage: `aranetctl --scan`
+        
+        Output:
+        ```
+        =======================================
+          Name:     Aranet4 00000
+          Address:  XX:XX:XX:XX:XX:XX
+          RSSI:     -85 dBm
+        --------------------------------------
+          CO2:           662 pm
+          Temperature:   21.9 °C
+          Humidity:      48 %
+          Pressure:      1019.2 hPa
+          Battery:       34 %
+          Status disp.:  GREEN
+        
+        =======================================
+          Name:     Aranet4 00001
+          Address:  XX:XX:XX:XX:XX:XX
+          RSSI:     -91 dBm
+        
+        ```
+        
+        **Note:** To receive current measurements, Smart Home Integrations must be enabled and firmware version must be v1.2.0 or newer.
+        
+        ### Logged Readings Example
+        
+        ```python
+        import aranet4
+        
+        device_mac = "XX:XX:XX:XX:XX:XX"
+        
+        history = aranet4.client.get_all_records(
+            device_mac, entry_filter={"humi": False, "pres": False}
+        )
+        print(f"{'Date':^20} | {'CO2':^10} | {'Temperature':^10} ")
+        for entry in history.value:
+            print(f"{entry.date.isoformat():^20} | {entry.co2:^10} | {entry.temperature:^10}")
+        
+        ```
+        
+        ## Library functions
+        ### get_current_readings(mac_address: str) -> client.CurrentReading
+        Get current measurements from device
+        Returns **CurrentReading** object:
+        ```python
+        class CurrentReading:
+            name: str = ""
+            version: str = ""
+            temperature: float = -1
+            humidity: int = -1
+            pressure: float = -1
+            co2: int = -1
+            battery: int = -1
+            status: int = -1
+            interval: int = -1
+            ago: int = -1
+            stored: int = -1
+        ```
+        
+        ### get_all_records(mac_address: str, entry_filter: dict) -> client.Record
+        Get stored datapoints from device. Apply any filters if required
+        
+        `entry_filter` is a dictionary that can have the following values:
+         - `last`: int : Get last n entries
+         - `start`: datetime : Get entries after specified time
+         - `end`: datetime : Get entries before specified time
+         - `temp`: bool : Get temperature data points (default = True)
+         - `humi`: bool : Get humidity data points (default = True)
+         - `pres`: bool : Get pressure data points (default = True)
+         - `co2`: bool : Get co2 data points (default = True)
+        
+        Returns **CurrentReading** object:
+        ```python
+        class Record:
+            name: str
+            version: str
+            records_on_device: int
+            filter: Filter
+            value: List[RecordItem] = field(default_factory=list)
+        ```
+        Which includes these objects:
+        ```python
+        class RecordItem:
+            date: datetime
+            temperature: float
+            humidity: int
+            pressure: float
+            co2: int
+        
+        class Filter:
+            begin: int
+            end: int
+            incl_temperature: bool
+            incl_humidity: bool
+            incl_pressure: bool
+            incl_co2: bool
+        ```
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
```

### Comparing `aranet4-2.1.3/aranet4/aranetctl.py` & `aranet4-2.2.0/aranet4/aranetctl.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,30 @@
  --------------------------------------
  CO2:            {current.co2} ppm
  Temperature:    {current.temperature:.01f} \u00b0C
  Humidity:       {current.humidity} %
  Pressure:       {current.pressure:.01f} hPa
  Battery:        {current.battery} %
  Status Display: {current.status.name}
+ Age:            {current.ago}/{current.interval}
+--------------------------------------
+"""
+
+format_str_2 = """
+--------------------------------------
+ Connected: {current.name} | {current.version}
+ Updated {current.ago} s ago. Intervals: {current.interval} s
+ {current.stored} total log_size
+ --------------------------------------
+ Temperature:    {current.temperature:.01f} \u00b0C
+ Humidity:       {current.humidity} %
+ Battery:        {current.battery} %
+ Status Temp.:   {current.status_t.name}
+ Status Humid.:  {current.status_h.name}
+ Age:            {current.ago}/{current.interval}
 --------------------------------------
 """
 
 def parse_args(ctl_args):
     parser = argparse.ArgumentParser()
     parser.add_argument("device_mac", nargs='?', help="Aranet4 Bluetooth Address")
     parser.add_argument(
@@ -115,28 +131,28 @@
     print("-" * char_repeat)
     print(f"{'id': ^4} | {'date': ^25} |", end=""),
     if records.filter.incl_co2:
         print(f" {'co2':^6} |", end=""),
     if records.filter.incl_temperature:
         print(" temp |", end="")
     if records.filter.incl_humidity:
-        print(" hum |", end="")
+        print(" humid |", end="")
     if records.filter.incl_pressure:
         print(" pressure |", end="")
     print("")
     print("-" * char_repeat)
     filtered_values = records.value
     for record_id, line in enumerate(filtered_values, start=records.filter.begin):
         print(f"{record_id:>4d} | {line.date.isoformat()} |", end="")
         if records.filter.incl_co2:
             print(f" {line.co2:>6d} |", end="")
         if records.filter.incl_temperature:
             print(f" {line.temperature:>4.1f} |", end="")
         if records.filter.incl_humidity:
-            print(f" {line.humidity:>3d} |", end="")
+            print(f" {line.humidity:>3.1f} |", end="")
         if records.filter.incl_pressure:
             print(f" {line.pressure:>8.1f} |", end="")
         print("")
     print("-" * char_repeat)
 
 
 def print_scan_result(advertisement):
@@ -146,20 +162,29 @@
     print("=======================================")
     print(f"  Name:     {advertisement.device.name}")
     print(f"  Address:  {advertisement.device.address}")
     print(f"  RSSI:     {advertisement.device.rssi} dBm")
 
     if advertisement.readings:
         print("--------------------------------------")
-        print(f"  CO2:           {advertisement.readings.co2} pm")
-        print(f"  Temperature:   {advertisement.readings.temperature:.01f} \u00b0C")
-        print(f"  Humidity:      {advertisement.readings.humidity} %")
-        print(f"  Pressure:      {advertisement.readings.pressure:.01f} hPa")
-        print(f"  Battery:       {advertisement.readings.battery} %")
-        print(f"  Status disp.:  {advertisement.readings.status.name}")
+        if advertisement.readings.co2 >= 0:
+            print(f"  CO2:            {advertisement.readings.co2} pm")
+        print(f"  Temperature:    {advertisement.readings.temperature:.01f} \u00b0C")
+        print(f"  Humidity:       {advertisement.readings.humidity} %")
+        if advertisement.readings.pressure >= 0:
+            print(f"  Pressure:       {advertisement.readings.pressure:.01f} hPa")
+        print(f"  Battery:        {advertisement.readings.battery} %")
+        if advertisement.readings.status >= 0:
+            print(f"  Status Disp.:   {advertisement.readings.status.name}")
+        if advertisement.readings.status_t >= 0 and advertisement.readings.status_h >= 0:
+            print(f"  Status Temp.:   {advertisement.readings.status_t.name}")
+            print(f"  Status Humid.:  {advertisement.readings.status_h.name}")
+        print(f"  Age:            {advertisement.readings.ago}/{advertisement.readings.interval}")
+        print(f"  Counter:        {advertisement.readings.counter}")
+
     print()
 
 
 def write_csv(filename, log_data):
     """
     Output `client.Record` dataclass to csv file
     :param filename: file name
@@ -215,15 +240,15 @@
         print(f"Next data point in {secs}...", end="\r")
 
 
 def main(argv):
     args = parse_args(argv)
 
     if args.scan:
-        print("Looking for Aranet4 devices...")
+        print("Looking for Aranet devices...")
         devices = client.find_nearby(print_scan_result)
         print(f"Scan finished. Found {len(devices)}")
         return
 
     if not args.device_mac:
         print("Device address not specified")
         return
@@ -233,15 +258,16 @@
             wait_for_new_record(args.device_mac)
         records = client.get_all_records(args.device_mac, vars(args), True)
         print_records(records)
         if args.output:
             write_csv(args.output, records)
     else:
         current = client.get_current_readings(args.device_mac)
-        s = format_str.format(current=current)
+        s = format_str_2 if current.name.startswith("Aranet2") else format_str
+        s = s.format(current=current)
         print(s)
         if args.url:
             post_data(args.url, current)
 
 
 def entry_point():
     main(argv=sys.argv[1:])
```

### Comparing `aranet4-2.1.3/aranet4/client.py` & `aranet4-2.2.0/aranet4/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,22 +18,25 @@
 class Param(IntEnum):
     """Enums for the different log_size available"""
 
     TEMPERATURE = 1
     HUMIDITY = 2
     PRESSURE = 3
     CO2 = 4
+    HUMIDITY2 = 5
 
 
 class Status(IntEnum):
     """Enum for the different status colors"""
 
+    NONE = 0
     GREEN = 1
     AMBER = 2
     RED = 3
+    BLUE = 4
 
 
 @dataclass
 class Aranet4HistoryDelegate:
     """
     When collecting the historical records they are sent using BLE
     notifications. This class takes those notifications and presents them
@@ -78,36 +81,76 @@
 @dataclass
 class CurrentReading:
     """dataclass to store the information when querying the devices current settings"""
 
     name: str = ""
     version: str = ""
     temperature: float = -1
-    humidity: int = -1
+    humidity: float = -1
     pressure: float = -1
     co2: int = -1
     battery: int = -1
     status: int = -1
+    status_t: int = -1
+    status_h: int = -1
     interval: int = -1
     ago: int = -1
     stored: int = -1
+    counter: int = -1
 
     def decode(self, value: tuple):
         """Process data from current log_size and process before storing"""
         self.co2 = self._set(Param.CO2, value[0])
         self.temperature = self._set(Param.TEMPERATURE, value[1])
         self.pressure = self._set(Param.PRESSURE, value[2])
         self.humidity = self._set(Param.HUMIDITY, value[3])
         self.battery = value[4]
         self.status = Status(value[5])
         # If extended data list
         if len(value) > 6:
             self.interval = value[6]
             self.ago = value[7]
 
+    def decode2(self, value: tuple, gatt=False):
+        """Process data from current log_size and process before storing"""
+
+        # order from gatt and advertisements are different
+        if gatt:
+            self.temperature = self._set(Param.TEMPERATURE, value[4])
+            self.humidity = self._set(Param.HUMIDITY2, value[5])
+            self.battery = value[3]
+            self.status_h, self.status_t = self._decode_status_flags(value[6])
+            self.interval = value[1]
+            self.ago = value[2]
+        else:
+            self.temperature = self._set(Param.TEMPERATURE, value[1])
+            self.humidity = self._set(Param.HUMIDITY2, value[3])
+            self.battery = value[5]
+            self.status_h, self.status_t = self._decode_status_flags(value[6])
+            self.interval = value[7]
+            self.ago = value[8]
+            self.counter = value[9]
+
+    @staticmethod
+    def _decode_status_flags(status):
+        status_t = Status.GREEN
+        status_h = Status.GREEN
+
+        if status & 0b0001:
+            status_h = Status.BLUE
+        elif status & 0b0010:
+            status_h = Status.RED
+
+        if status & 0b0100:
+            status_t = Status.BLUE
+        elif status & 0b1000:
+            status_t = Status.RED
+
+        return (status_h, status_t)
+
     @staticmethod
     def _set(param: Param, value: int):
         """
         While in CO2 calibration mode Aranet4 did not take new measurements and
         stores Magic numbers in measurement history.
         Here data is converted with checking for Magic numbers.
         """
@@ -121,14 +164,17 @@
             multiplier = 0.1
         elif param == Param.TEMPERATURE:
             invalid_reading_flag = value >> 14 & 1 == 1
             multiplier = 0.05
         elif param == Param.HUMIDITY:
             invalid_reading_flag = value >> 8
             multiplier = 1
+        elif param == Param.HUMIDITY2:
+            invalid_reading_flag = value >> 15 == 1
+            multiplier = 0.1
 
         if invalid_reading_flag:
             return -1
         if isinstance(multiplier, float):
             return round(value * multiplier, 1)
         return value * multiplier
 
@@ -201,15 +247,21 @@
                 # Basic info
                 value_fmt = "<BBBHBB"
                 value = struct.unpack(value_fmt, raw_bytes[0:7])
                 mf_data.decode(value)
                 self.manufacturer_data = mf_data
 
                 # Extended info / measurements
-                if len(raw_bytes) >= 20:
+                if len(raw_bytes) >= 24 and device.name.startswith("Aranet2"):
+                    value_fmt = "<HHHHBBBHHB"
+                    value = struct.unpack(value_fmt, raw_bytes[8:24])
+                    self.readings = CurrentReading()
+                    self.readings.decode2(value)
+                    self.readings.name = device.name
+                elif len(raw_bytes) >= 20:
                     value_fmt = "<HHHBBBHH"
                     value = struct.unpack(value_fmt, raw_bytes[8:21])
                     self.readings = CurrentReading()
                     self.readings.decode(value)
                     self.readings.name = device.name
 
 
@@ -227,15 +279,15 @@
 @dataclass
 class Filter:
     """dataclass to store log filter information"""
 
     begin: int
     end: int
     incl_temperature: bool
-    incl_humidity: bool
+    incl_humidity: int
     incl_pressure: bool
     incl_co2: bool
 
 
 @dataclass
 class Record:
     name: str
@@ -272,14 +324,17 @@
     AR4_SERVICE = "0000fce0-0000-1000-8000-00805f9b34fb" # v1.2.0 and later
     GENERIC_SERVICE = "00001800-0000-1000-8000-00805f9b34fb"
     COMMON_SERVICE = "0000180a-0000-1000-8000-00805f9b34fb"
 
     # Read / Aranet service
     AR4_READ_CURRENT_READINGS = "f0cd1503-95da-4f4b-9ac8-aa55d312af0c"
     AR4_READ_CURRENT_READINGS_DET = "f0cd3001-95da-4f4b-9ac8-aa55d312af0c"
+    AR2_READ_CURRENT_READINGS = "f0cd1504-95da-4f4b-9ac8-aa55d312af0c"
+    AR2_READ_CURRENT_READINGS_A = "f0cd3003-95da-4f4b-9ac8-aa55d312af0c" # data is same as other
+    # aranet2 has different service uids. use rhose
     AR4_READ_INTERVAL = "f0cd2002-95da-4f4b-9ac8-aa55d312af0c"
     AR4_READ_SECONDS_SINCE_UPDATE = "f0cd2004-95da-4f4b-9ac8-aa55d312af0c"
     AR4_READ_TOTAL_READINGS = "f0cd2001-95da-4f4b-9ac8-aa55d312af0c"
     AR4_READ_HISTORY_READINGS_V1 = "f0cd2003-95da-4f4b-9ac8-aa55d312af0c"
     AR4_READ_HISTORY_READINGS_V2 = "f0cd2005-95da-4f4b-9ac8-aa55d312af0c"
 
     # Read / Generic servce
@@ -314,26 +369,38 @@
         """Connect to remote device"""
         await self.device.connect()
 
     async def current_readings(self, details: bool = False):
         """Extract current readings from remote device"""
         readings = CurrentReading()
 
-        if details:
-            uuid = self.AR4_READ_CURRENT_READINGS_DET
+        aranet2_char = self.device.services.get_characteristic(
+            self.AR2_READ_CURRENT_READINGS
+        )
+
+        if aranet2_char:
+            uuid = self.AR2_READ_CURRENT_READINGS
             # co2, temp, pressure, humidity, battery, status
-            value_fmt = "<HHHBBBHH"
+            value_fmt = "<HHHBHHB"
+            raw_bytes = await self.device.read_gatt_char(uuid)
+            value = struct.unpack(value_fmt, raw_bytes)
+            readings.decode2(value, True)
         else:
-            uuid = self.AR4_READ_CURRENT_READINGS
-            # co2, temp, pressure, humidity, battery, status, interval, ago
-            value_fmt = "<HHHBBB"
-
-        raw_bytes = await self.device.read_gatt_char(uuid)
-        value = struct.unpack(value_fmt, raw_bytes)
-        readings.decode(value)
+            if details:
+                uuid = self.AR4_READ_CURRENT_READINGS_DET
+                # co2, temp, pressure, humidity, battery, status
+                value_fmt = "<HHHBBBHH"
+            else:
+                uuid = self.AR4_READ_CURRENT_READINGS
+                # co2, temp, pressure, humidity, battery, status, interval, ^
+                value_fmt = "<HHHBBB"
+
+            raw_bytes = await self.device.read_gatt_char(uuid)
+            value = struct.unpack(value_fmt, raw_bytes)
+            readings.decode(value)
         return readings
 
     async def get_interval(self) -> int:
         """Get the value for how often datapoints are logged on device"""
         raw_bytes = await self.device.read_gatt_char(self.AR4_READ_INTERVAL)
         return int.from_bytes(raw_bytes, byteorder="little")
 
@@ -574,15 +641,15 @@
 async def _find_nearby(detect_callback: callable, duration: int) -> List[BLEDevice]:
     scanner = Aranet4Scanner(detect_callback)
     await scanner.start()
     await asyncio.sleep(duration)
     await scanner.stop()
     return [device
             for device in scanner.scanner.discovered_devices
-            if "Aranet4" in device.name]
+            if "Aranet4" in device.name or "Aranet2" in device.name]
 
 
 def find_nearby(detect_callback: callable, duration: int = 5) -> List[BLEDevice]:
     """
     Scans for nearby Aranet4 devices.
     Will call callback on every valid Aranet4 advertisement, including duplcates
     """
@@ -617,14 +684,20 @@
     if next_log < 10:
         print(f"Waiting {next_log} for next datapoint to be taken...")
         await asyncio.sleep(next_log)
         # there was another log so update the numbers
         last_log = await monitor.get_seconds_since_update()
         now = datetime.datetime.now(datetime.timezone.utc).replace(microsecond=0)
 
+    if dev_name.startswith("Aranet2"):
+        entry_filter["pres"] = False
+        entry_filter["co2"] = False
+        if entry_filter.get("humi", False):
+            entry_filter["humi"] = 2 #v2 humidity
+
     log_size = await monitor.get_total_readings()
     log_points = _log_times(now, log_size, interval, last_log)
     begin, end = _calc_start_end(log_points, entry_filter)
     rec_filter = Filter(
         begin,
         end,
         entry_filter.get("temp", True),
@@ -640,15 +713,19 @@
     # Read datapoint history from device
     if rec_filter.incl_temperature:
         temperature_val = await monitor.get_records(
             Param.TEMPERATURE, log_size=log_size, start=begin, end=end
         )
     else:
         temperature_val = _empty_reading(log_size)
-    if rec_filter.incl_humidity:
+    if rec_filter.incl_humidity == 2:
+        humidity_val = await monitor.get_records(
+            Param.HUMIDITY2, log_size=log_size, start=begin, end=end
+        )
+    elif rec_filter.incl_humidity:
         humidity_val = await monitor.get_records(
             Param.HUMIDITY, log_size=log_size, start=begin, end=end
         )
     else:
         humidity_val = _empty_reading(log_size)
     if rec_filter.incl_pressure:
         pressure_val = await monitor.get_records(
```

### Comparing `aranet4-2.1.3/aranet4.egg-info/PKG-INFO` & `aranet4-2.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,233 +1,230 @@
 Metadata-Version: 2.1
 Name: aranet4
-Version: 2.1.3
-Summary: Aranet4 Python client
+Version: 2.2.0
+Summary: Aranet4 and Aranet2 Python client
 Home-page: https://github.com/Anrijs/Aranet4-Python
 License: UNKNOWN
+Description: # Aranet4 Python client
+        ## Installation
+        1. Install aranet4 and its dependencies:
+        ```
+        pip3 install aranet4
+        ```
+        2. Pair Aranet4 device
+        3. Run `aranetctl` or use as library
+        
+        **Note:** Smart Home Integrations must be enabled in Aranet4 mobile app for full support.
+        
+        ## aranetctl usage
+        ```text
+        $ aranetctl -h
+        usage: aranetctl [-h] [-u URL] [-r] [-s DATE] [-e DATE] [-o FILE] [-w] [-l COUNT]
+                         [--xt] [--xh] [--xp] [--xc]
+                         device_mac
+        
+        positional arguments:
+          device_mac            Aranet4 Bluetooth Address
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          -r, --records         Fetch historical log records
+          --scan                Scan Aranet4 devices
+        
+        Options for current reading:
+          -u URL, --url URL     Remote url for current value push
+        
+        Filter History Log Records:
+          -s DATE, --start DATE
+                                Records range start (UTC time, example:
+                                2019-09-29T14:00:00
+          -e DATE, --end DATE   Records range end (UTC time, example: 2019-09-30T14:00:00
+          -o FILE, --output FILE
+                                Save records to a file
+          -w, --wait            Wait until new data point available
+          -l COUNT, --last COUNT
+                                Get <COUNT> last records
+          --xt                  Don't get temperature records
+          --xh                  Don't get humidity records
+          --xp                  Don't get pressure records
+          --xc                  Don't get co2 records
+        
+        ```
+        
+        ### Current Readings Example
+        Usage: `aranetctl XX:XX:XX:XX:XX:XX`
+        
+        Output:
+        ```
+        --------------------------------------
+        Connected: Aranet4 00000 | v0.3.1
+        Updated 51 s ago. Intervals: 60 s
+        5040 total readings
+        --------------------------------------
+        CO2:          904 ppm
+        Temperature:  19.9 C
+        Humidity:     51 %
+        Pressure:     997.0 hPa
+        Battery:      96 %
+        Status Display: GREEN
+        --------------------------------------
+        ```
+        
+        ### Get History Example
+        Write full log to screen:
+        
+        Usage: `aranetctl XX:XX:XX:XX:XX:XX -r`
+        
+        ```shell
+        -------------------------------------------------------------
+        Device Name    :        Aranet4 00000
+        Device Version :               v0.3.1
+        -------------------------------------------------------------
+         id  |        date         |  co2   | temp | hum | pressure |
+        -------------------------------------------------------------
+           1 | 2022-02-18T14:15:44 |    844 | 21.8 |  50 |    985.6 |
+           2 | 2022-02-18T14:20:44 |    846 | 21.8 |  50 |    985.9 |
+           3 | 2022-02-18T14:25:44 |    843 | 22.0 |  50 |    986.4 |
+           4 | 2022-02-18T14:30:44 |    881 | 22.1 |  50 |    986.4 |
+           5 | 2022-02-18T14:35:44 |    854 | 22.1 |  50 |    987.3 |
+           6 | 2022-02-18T14:40:44 |    867 | 22.2 |  50 |    987.5 |
+           7 | 2022-02-18T14:45:44 |    883 | 22.1 |  50 |    988.1 |
+           8 | 2022-02-18T14:50:44 |    921 | 22.1 |  50 |    988.6 |
+           9 | 2022-02-18T14:55:44 |    930 | 22.0 |  50 |    989.1 |
+          10 | 2022-02-18T15:00:44 |    954 | 22.0 |  50 |    989.5 |
+        -------------------------------------------------------------
+        ```
+        
+        Usage: `aranetctl XX:XX:XX:XX:XX:XX -r -o aranet4.csv`
+        
+        Output file format: `Date,CO2,Temperature,Humidity,Pressure`
+        
+        Output file example:
+        ```
+        date,co2,temperature,humidity,pressure
+        2022-02-18 10:05:47,1398,23.2,53,986.6
+        2022-02-18 10:10:47,1155,23.1,50,986.3
+        ```
+        
+        ## Usage of library
+        
+        ### Current Readings Example
+        
+        ```python
+        import aranet4
+        
+        device_mac = "XX:XX:XX:XX:XX:XX"
+        
+        current = aranet4.client.get_current_readings(device_mac)
+        
+        print("co2 reading:", current.co2)
+        print("Temperature:", current.temperature)
+        print("Humidity:", current.humidity)
+        print("Pressure:", current.pressure)
+        ```
+        
+        ### Scanner Example
+        Usage: `aranetctl --scan`
+        
+        Output:
+        ```
+        =======================================
+          Name:     Aranet4 00000
+          Address:  XX:XX:XX:XX:XX:XX
+          RSSI:     -85 dBm
+        --------------------------------------
+          CO2:           662 pm
+          Temperature:   21.9 °C
+          Humidity:      48 %
+          Pressure:      1019.2 hPa
+          Battery:       34 %
+          Status disp.:  GREEN
+        
+        =======================================
+          Name:     Aranet4 00001
+          Address:  XX:XX:XX:XX:XX:XX
+          RSSI:     -91 dBm
+        
+        ```
+        
+        **Note:** To receive current measurements, Smart Home Integrations must be enabled and firmware version must be v1.2.0 or newer.
+        
+        ### Logged Readings Example
+        
+        ```python
+        import aranet4
+        
+        device_mac = "XX:XX:XX:XX:XX:XX"
+        
+        history = aranet4.client.get_all_records(
+            device_mac, entry_filter={"humi": False, "pres": False}
+        )
+        print(f"{'Date':^20} | {'CO2':^10} | {'Temperature':^10} ")
+        for entry in history.value:
+            print(f"{entry.date.isoformat():^20} | {entry.co2:^10} | {entry.temperature:^10}")
+        
+        ```
+        
+        ## Library functions
+        ### get_current_readings(mac_address: str) -> client.CurrentReading
+        Get current measurements from device
+        Returns **CurrentReading** object:
+        ```python
+        class CurrentReading:
+            name: str = ""
+            version: str = ""
+            temperature: float = -1
+            humidity: int = -1
+            pressure: float = -1
+            co2: int = -1
+            battery: int = -1
+            status: int = -1
+            interval: int = -1
+            ago: int = -1
+            stored: int = -1
+        ```
+        
+        ### get_all_records(mac_address: str, entry_filter: dict) -> client.Record
+        Get stored datapoints from device. Apply any filters if required
+        
+        `entry_filter` is a dictionary that can have the following values:
+         - `last`: int : Get last n entries
+         - `start`: datetime : Get entries after specified time
+         - `end`: datetime : Get entries before specified time
+         - `temp`: bool : Get temperature data points (default = True)
+         - `humi`: bool : Get humidity data points (default = True)
+         - `pres`: bool : Get pressure data points (default = True)
+         - `co2`: bool : Get co2 data points (default = True)
+        
+        Returns **CurrentReading** object:
+        ```python
+        class Record:
+            name: str
+            version: str
+            records_on_device: int
+            filter: Filter
+            value: List[RecordItem] = field(default_factory=list)
+        ```
+        Which includes these objects:
+        ```python
+        class RecordItem:
+            date: datetime
+            temperature: float
+            humidity: int
+            pressure: float
+            co2: int
+        
+        class Filter:
+            begin: int
+            end: int
+            incl_temperature: bool
+            incl_humidity: bool
+            incl_pressure: bool
+            incl_co2: bool
+        ```
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Aranet4 Python client
-## Installation
-1. Install aranet4 and its dependencies:
-```
-pip3 install aranet4
-```
-2. Pair Aranet4 device
-3. Run `aranetctl` or use as library
-
-**Note:** Smart Home Integrations must be enabled in Aranet4 mobile app for full support.
-
-## aranetctl usage
-```text
-$ aranetctl -h
-usage: aranetctl [-h] [-u URL] [-r] [-s DATE] [-e DATE] [-o FILE] [-w] [-l COUNT]
-                 [--xt] [--xh] [--xp] [--xc]
-                 device_mac
-
-positional arguments:
-  device_mac            Aranet4 Bluetooth Address
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -r, --records         Fetch historical log records
-  --scan                Scan Aranet4 devices
-
-Options for current reading:
-  -u URL, --url URL     Remote url for current value push
-
-Filter History Log Records:
-  -s DATE, --start DATE
-                        Records range start (UTC time, example:
-                        2019-09-29T14:00:00
-  -e DATE, --end DATE   Records range end (UTC time, example: 2019-09-30T14:00:00
-  -o FILE, --output FILE
-                        Save records to a file
-  -w, --wait            Wait until new data point available
-  -l COUNT, --last COUNT
-                        Get <COUNT> last records
-  --xt                  Don't get temperature records
-  --xh                  Don't get humidity records
-  --xp                  Don't get pressure records
-  --xc                  Don't get co2 records
-
-```
-
-### Current Readings Example
-Usage: `aranetctl XX:XX:XX:XX:XX:XX`
-
-Output:
-```
---------------------------------------
-Connected: Aranet4 00000 | v0.3.1
-Updated 51 s ago. Intervals: 60 s
-5040 total readings
---------------------------------------
-CO2:          904 ppm
-Temperature:  19.9 C
-Humidity:     51 %
-Pressure:     997.0 hPa
-Battery:      96 %
-Status Display: GREEN
---------------------------------------
-```
-
-### Get History Example
-Write full log to screen:
-
-Usage: `aranetctl XX:XX:XX:XX:XX:XX -r`
-
-```shell
--------------------------------------------------------------
-Device Name    :        Aranet4 00000
-Device Version :               v0.3.1
--------------------------------------------------------------
- id  |        date         |  co2   | temp | hum | pressure |
--------------------------------------------------------------
-   1 | 2022-02-18T14:15:44 |    844 | 21.8 |  50 |    985.6 |
-   2 | 2022-02-18T14:20:44 |    846 | 21.8 |  50 |    985.9 |
-   3 | 2022-02-18T14:25:44 |    843 | 22.0 |  50 |    986.4 |
-   4 | 2022-02-18T14:30:44 |    881 | 22.1 |  50 |    986.4 |
-   5 | 2022-02-18T14:35:44 |    854 | 22.1 |  50 |    987.3 |
-   6 | 2022-02-18T14:40:44 |    867 | 22.2 |  50 |    987.5 |
-   7 | 2022-02-18T14:45:44 |    883 | 22.1 |  50 |    988.1 |
-   8 | 2022-02-18T14:50:44 |    921 | 22.1 |  50 |    988.6 |
-   9 | 2022-02-18T14:55:44 |    930 | 22.0 |  50 |    989.1 |
-  10 | 2022-02-18T15:00:44 |    954 | 22.0 |  50 |    989.5 |
--------------------------------------------------------------
-```
-
-Usage: `aranetctl XX:XX:XX:XX:XX:XX -r -o aranet4.csv`
-
-Output file format: `Date,CO2,Temperature,Humidity,Pressure`
-
-Output file example:
-```
-date,co2,temperature,humidity,pressure
-2022-02-18 10:05:47,1398,23.2,53,986.6
-2022-02-18 10:10:47,1155,23.1,50,986.3
-```
-
-## Usage of library
-
-### Current Readings Example
-
-```python
-import aranet4
-
-device_mac = "XX:XX:XX:XX:XX:XX"
-
-current = aranet4.client.get_current_readings(device_mac)
-
-print("co2 reading:", current.co2)
-print("Temperature:", current.temperature)
-print("Humidity:", current.humidity)
-print("Pressure:", current.pressure)
-```
-
-### Scanner Example
-Usage: `aranetctl --scan`
-
-Output:
-```
-=======================================
-  Name:     Aranet4 00000
-  Address:  XX:XX:XX:XX:XX:XX
-  RSSI:     -85 dBm
---------------------------------------
-  CO2:           662 pm
-  Temperature:   21.9 °C
-  Humidity:      48 %
-  Pressure:      1019.2 hPa
-  Battery:       34 %
-  Status disp.:  GREEN
-
-=======================================
-  Name:     Aranet4 00001
-  Address:  XX:XX:XX:XX:XX:XX
-  RSSI:     -91 dBm
-
-```
-
-**Note:** To receive current measurements, Smart Home Integrations must be enabled and firmware version must be v1.2.0 or newer.
-
-### Logged Readings Example
-
-```python
-import aranet4
-
-device_mac = "XX:XX:XX:XX:XX:XX"
-
-history = aranet4.client.get_all_records(
-    device_mac, entry_filter={"humi": False, "pres": False}
-)
-print(f"{'Date':^20} | {'CO2':^10} | {'Temperature':^10} ")
-for entry in history.value:
-    print(f"{entry.date.isoformat():^20} | {entry.co2:^10} | {entry.temperature:^10}")
-
-```
-
-## Library functions
-### get_current_readings(mac_address: str) -> client.CurrentReading
-Get current measurements from device
-Returns **CurrentReading** object:
-```python
-class CurrentReading:
-    name: str = ""
-    version: str = ""
-    temperature: float = -1
-    humidity: int = -1
-    pressure: float = -1
-    co2: int = -1
-    battery: int = -1
-    status: int = -1
-    interval: int = -1
-    ago: int = -1
-    stored: int = -1
-```
-
-### get_all_records(mac_address: str, entry_filter: dict) -> client.Record
-Get stored datapoints from device. Apply any filters if required
-
-`entry_filter` is a dictionary that can have the following values:
- - `last`: int : Get last n entries
- - `start`: datetime : Get entries after specified time
- - `end`: datetime : Get entries before specified time
- - `temp`: bool : Get temperature data points (default = True)
- - `humi`: bool : Get humidity data points (default = True)
- - `pres`: bool : Get pressure data points (default = True)
- - `co2`: bool : Get co2 data points (default = True)
-
-Returns **CurrentReading** object:
-```python
-class Record:
-    name: str
-    version: str
-    records_on_device: int
-    filter: Filter
-    value: List[RecordItem] = field(default_factory=list)
-```
-Which includes these objects:
-```python
-class RecordItem:
-    date: datetime
-    temperature: float
-    humidity: int
-    pressure: float
-    co2: int
-
-class Filter:
-    begin: int
-    end: int
-    incl_temperature: bool
-    incl_humidity: bool
-    incl_pressure: bool
-    incl_co2: bool
-```
-
-
```

### Comparing `aranet4-2.1.3/setup.py` & `aranet4-2.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aranet4",
-    version="2.1.3",
-    description="Aranet4 Python client",
+    version="2.2.0",
+    description="Aranet4 and Aranet2 Python client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Anrijs/Aranet4-Python",
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
```

