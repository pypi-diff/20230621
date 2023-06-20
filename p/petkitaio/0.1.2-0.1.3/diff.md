# Comparing `tmp/petkitaio-0.1.2.tar.gz` & `tmp/petkitaio-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petkitaio-0.1.2.tar", last modified: Fri Jun  2 03:02:44 2023, max compression
+gzip compressed data, was "petkitaio-0.1.3.tar", last modified: Tue Jun 20 22:46:27 2023, max compression
```

## Comparing `petkitaio-0.1.2.tar` & `petkitaio-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-02 03:02:44.187123 petkitaio-0.1.2/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-06-02 02:50:52.000000 petkitaio-0.1.2/LICENSE
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     5340 2023-06-02 03:02:44.187333 petkitaio-0.1.2/PKG-INFO
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     3853 2023-06-02 02:50:52.000000 petkitaio-0.1.2/README.md
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-02 03:02:44.184608 petkitaio-0.1.2/petkitaio/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1550 2023-06-02 02:50:52.000000 petkitaio-0.1.2/petkitaio/__init__.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     8893 2023-06-02 02:50:52.000000 petkitaio-0.1.2/petkitaio/constants.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      835 2023-06-02 02:50:52.000000 petkitaio-0.1.2/petkitaio/exceptions.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1148 2023-06-02 02:50:52.000000 petkitaio-0.1.2/petkitaio/model.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)    37648 2023-06-02 02:50:52.000000 petkitaio-0.1.2/petkitaio/petkit_client.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      680 2023-06-02 02:50:52.000000 petkitaio-0.1.2/petkitaio/str_enum.py
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-02 03:02:44.186790 petkitaio-0.1.2/petkitaio.egg-info/
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     5340 2023-06-02 03:02:44.000000 petkitaio-0.1.2/petkitaio.egg-info/PKG-INFO
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      337 2023-06-02 03:02:44.000000 petkitaio-0.1.2/petkitaio.egg-info/SOURCES.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-06-02 03:02:44.000000 petkitaio-0.1.2/petkitaio.egg-info/dependency_links.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       28 2023-06-02 03:02:44.000000 petkitaio-0.1.2/petkitaio.egg-info/requires.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2023-06-02 03:02:44.000000 petkitaio-0.1.2/petkitaio.egg-info/top_level.txt
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)       38 2023-06-02 03:02:44.188002 petkitaio-0.1.2/setup.cfg
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1050 2023-06-02 02:50:52.000000 petkitaio-0.1.2/setup.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-20 22:46:27.770190 petkitaio-0.1.3/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-06-20 22:38:20.000000 petkitaio-0.1.3/LICENSE
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     5735 2023-06-20 22:46:27.770404 petkitaio-0.1.3/PKG-INFO
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     4224 2023-06-20 22:38:20.000000 petkitaio-0.1.3/README.md
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-20 22:46:27.767335 petkitaio-0.1.3/petkitaio/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1550 2023-06-20 22:38:20.000000 petkitaio-0.1.3/petkitaio/__init__.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     8993 2023-06-20 22:38:20.000000 petkitaio-0.1.3/petkitaio/constants.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      835 2023-06-20 22:38:20.000000 petkitaio-0.1.3/petkitaio/exceptions.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1204 2023-06-20 22:38:20.000000 petkitaio-0.1.3/petkitaio/model.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)    40259 2023-06-20 22:38:20.000000 petkitaio-0.1.3/petkitaio/petkit_client.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      680 2023-06-20 22:38:20.000000 petkitaio-0.1.3/petkitaio/str_enum.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-06-20 22:46:27.769733 petkitaio-0.1.3/petkitaio.egg-info/
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     5735 2023-06-20 22:46:27.000000 petkitaio-0.1.3/petkitaio.egg-info/PKG-INFO
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      337 2023-06-20 22:46:27.000000 petkitaio-0.1.3/petkitaio.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-06-20 22:46:27.000000 petkitaio-0.1.3/petkitaio.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       28 2023-06-20 22:46:27.000000 petkitaio-0.1.3/petkitaio.egg-info/requires.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2023-06-20 22:46:27.000000 petkitaio-0.1.3/petkitaio.egg-info/top_level.txt
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)       38 2023-06-20 22:46:27.770980 petkitaio-0.1.3/setup.cfg
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1050 2023-06-20 22:38:20.000000 petkitaio-0.1.3/setup.py
```

### Comparing `petkitaio-0.1.2/LICENSE` & `petkitaio-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.2/PKG-INFO` & `petkitaio-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petkitaio
-Version: 0.1.2
+Version: 0.1.3
 Summary: Asynchronous Python library for PetKit's API
 Home-page: https://github.com/RobertD502/petkitaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/petkitaio/issues
 Project-URL: Source, https://github.com/RobertD502/petkitaio/
@@ -13,16 +13,19 @@
         Asynchronous Python library for PetKit's API.
         
         This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. Although support has been added for the PetKit Asia API endpoint, I have not personally tested it.
         
         ## **Currently Supported Devices**:
         - [D3 Feeder (Fresh Element Infinity)](https://www.amazon.com/PETKIT-Automatic-Stainless-Programmable-Dispenser/dp/B09JFK8BCQ)
         - [D4 Feeder (Fresh Element Solo)](https://www.amazon.com/PETKIT-Automatic-Dispenser-Compatible-Freeze-Dried/dp/B09158J9PF/)
+        - [D4s Feeder (Fresh Element Gemini)](https://www.amazon.com/PETKIT-Automatic-Combination-Dispenser-Stainless/dp/B0BF56RTQH)
         - [Mini Feeder](https://www.amazon.com/PETKIT-Automatic-Stainless-Indicator-Dispenser-2-8L/dp/B08GS1CPHH/)
+        - [W5 Water Fountain (Eversweet Solo 2)](https://www.amazon.com/PETKIT-EVERSWEET-Wireless-Visualization-Dispenser-2L/dp/B0B3RWF653)
         - [W5 Water Fountain (Eversweet 3 Pro)](https://www.amazon.com/PETKIT-Wireless-Fountain-Stainless-Dispenser/dp/B09QRH6L3M/)
+        - [W5 Water Fountain (Eversweet 5 Mini)](https://www.petkit.nl/products/eversweet-5-mini-binnen-2-weken-geleverd)
         - [T3 Litter Box (Pura X)](https://www.amazon.com/PETKIT-Self-Cleaning-Scooping-Automatic-Multiple/dp/B08T9CCP1M)
         - [T4 Litter Box (Pura MAX) with/without Pura Air](https://www.amazon.com/PETKIT-Self-Cleaning-Capacity-Multiple-Automatic/dp/B09KC7Q4YF)
         
         ## Important
         
         PetKit accounts can only be logged in on one device at a time. Using this library will result in getting signed out of the mobile app. You can avoid this by creating a secondary account and sharing devices from the main account (except water fountains). However, some device functionality is lost when using a secondary account as well as not being able to share pets between accounts.
```

### Comparing `petkitaio-0.1.2/README.md` & `petkitaio-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 Asynchronous Python library for PetKit's API.
 
 This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. Although support has been added for the PetKit Asia API endpoint, I have not personally tested it.
 
 ## **Currently Supported Devices**:
 - [D3 Feeder (Fresh Element Infinity)](https://www.amazon.com/PETKIT-Automatic-Stainless-Programmable-Dispenser/dp/B09JFK8BCQ)
 - [D4 Feeder (Fresh Element Solo)](https://www.amazon.com/PETKIT-Automatic-Dispenser-Compatible-Freeze-Dried/dp/B09158J9PF/)
+- [D4s Feeder (Fresh Element Gemini)](https://www.amazon.com/PETKIT-Automatic-Combination-Dispenser-Stainless/dp/B0BF56RTQH)
 - [Mini Feeder](https://www.amazon.com/PETKIT-Automatic-Stainless-Indicator-Dispenser-2-8L/dp/B08GS1CPHH/)
+- [W5 Water Fountain (Eversweet Solo 2)](https://www.amazon.com/PETKIT-EVERSWEET-Wireless-Visualization-Dispenser-2L/dp/B0B3RWF653)
 - [W5 Water Fountain (Eversweet 3 Pro)](https://www.amazon.com/PETKIT-Wireless-Fountain-Stainless-Dispenser/dp/B09QRH6L3M/)
+- [W5 Water Fountain (Eversweet 5 Mini)](https://www.petkit.nl/products/eversweet-5-mini-binnen-2-weken-geleverd)
 - [T3 Litter Box (Pura X)](https://www.amazon.com/PETKIT-Self-Cleaning-Scooping-Automatic-Multiple/dp/B08T9CCP1M)
 - [T4 Litter Box (Pura MAX) with/without Pura Air](https://www.amazon.com/PETKIT-Self-Cleaning-Capacity-Multiple-Automatic/dp/B09KC7Q4YF)
 
 ## Important
 
 PetKit accounts can only be logged in on one device at a time. Using this library will result in getting signed out of the mobile app. You can avoid this by creating a secondary account and sharing devices from the main account (except water fountains). However, some device functionality is lost when using a secondary account as well as not being able to share pets between accounts.
```

### Comparing `petkitaio-0.1.2/petkitaio/__init__.py` & `petkitaio-0.1.3/petkitaio/__init__.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.2/petkitaio/constants.py` & `petkitaio-0.1.3/petkitaio/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,27 +26,30 @@
     MANUAL_FEED = '/saveDailyFeed'
     MAX_ODOR_RESET = '/deodorantReset'
     MINI_DESICCANT_RESET = '/feedermini/desiccant_reset'
     MINI_MANUAL_FEED = '/feedermini/save_dailyfeed'
     MINI_SETTING = '/feedermini/update'
     PET_PROPS = '/pet/updatepetprops'
     REFRESH_HOME = '/discovery/refreshHome'
+    REPLENISHED_FOOD = '/added'
     SOUND_LIST = '/soundList'
     STATISTIC = '/statistic'
     UNIT = '/app/saveunit'
     UPDATE_SETTING = '/updateSettings'
     USER_DETAILS = '/user/details2'
     W5 = '/w5/deviceData'
 
 class FeederSetting(StrEnum):
 
     CHILD_LOCK = 'manualLock'
     DISPENSE_TONE = 'feedSound'
     DO_NOT_DISTURB = 'disturbMode'
+    FEED_TONE = 'feedTone'
     INDICATOR_LIGHT = 'lightMode'
+    MIN_EAT_DURATION = 'shortest'
     MINI_CHILD_LOCK = 'settings.manualLock'
     MINI_INDICATOR_LIGHT = 'settings.lightMode'
     SELECTED_SOUND = 'selectedSound'
     SHORTAGE_ALARM = 'foodWarn'
     SOUND_ENABLE = 'soundEnable'
     SURPLUS = 'surplus'
     SURPLUS_CONTROL = 'surplusControl'
@@ -222,15 +225,15 @@
 }
 
 SERVER_ERROR_CODES = {
     1: 'PetKit servers are busy. Please try again later.',
 }
 
 BLE_HEADER = [-6, -4, -3]
-FEEDER_LIST = ['D3', 'D4', 'FeederMini']
+FEEDER_LIST = ['D3', 'D4', 'D4s', 'FeederMini']
 LITTER_LIST = ['T3', 'T4']
 WATER_FOUNTAIN_LIST = ['W5']
 
 LB_CMD_TO_KEY = {
     LitterBoxCommand.LIGHT_ON: LitterBoxCommandKey.START,
     LitterBoxCommand.POWER: LitterBoxCommandKey.POWER,
     LitterBoxCommand.START_CLEAN: LitterBoxCommandKey.START,
```

### Comparing `petkitaio-0.1.2/petkitaio/exceptions.py` & `petkitaio-0.1.3/petkitaio/exceptions.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.2/petkitaio/model.py` & `petkitaio-0.1.3/petkitaio/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,26 +19,27 @@
 class Feeder:
     """Dataclass for PetKit Feeders."""
 
     id: int
     data: dict[str, Any]
     type: str
     sound_list: Optional[dict[int, str]] = None
+    last_manual_feed_id: Optional[str] = None
 
 @dataclass
 class LitterBox:
     """Dataclass for PetKit Litter Boxes."""
 
     id: int
     device_detail: dict[str, Any]
     device_record: dict[str, Any]
     statistics: dict[str, Any]
     type: str
     manually_paused: bool
-    manual_pause_end: datetime | None
+    manual_pause_end: Optional[datetime] = None
 
 @dataclass
 class W5Fountain:
     """Dataclass for W5 Water Fountain."""
 
     id: int
     data: dict[str, Any]
```

### Comparing `petkitaio-0.1.2/petkitaio/petkit_client.py` & `petkitaio-0.1.3/petkitaio/petkit_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         self.token: str | None = None
         self.token_expiration: datetime | None = None
         self.user_id: str | None = None
         self.has_relay: bool = False
         self.ble_sequence: int = 0
         self.manually_paused: dict[int, bool] = {}
         self.manual_pause_end: dict[int, datetime | None] = {}
+        self.last_manual_feed_id: dict[int, str | None] = {}
 
     async def get_api_server_list(self) -> None:
         """Fetches a list of all api urls categorized by region."""
 
         url = 'https://passport.petkt.com/6/account/regionservers'
 
         headers = {
@@ -199,45 +200,41 @@
         LOGGER.debug(f'Found the following PetKit devices: {devices}')
         if devices:
             for device in devices:
                 # W5 Water Fountain
                 if device['type'] in WATER_FOUNTAIN_LIST:
                     device_type: str = device['type'].lower()
                     fountain_data: dict[str, Any] = {}
-                    relay_tc: int | None = None
+                    relay_tc: int = 14
                     wf_url = f'{self.base_url}{Endpoint.W5}'
                     data = {
                         'id': device['data']['id']
                     }
 
                     if self.has_relay:
-                        ble_available: bool = False
                         main_online: bool = False
-                        fountain_tcode = str(device['data']['typeCode'])
                         ble_url = f'{self.base_url}{Endpoint.BLE_DEVICES}'
                         relay_devices = await self._post(ble_url, header, data={})
                         if relay_devices['result']:
                             ble_available = True
                             for relay_device in relay_devices['result']:
                                 if relay_device['pim'] == 1:
                                     main_online = True
                                     break
                                 else:
                                     main_online = False
 
                             if ble_available and main_online:
                                 device_details = await self._post(wf_url, header, data)
                                 mac = device_details['result']['mac']
-                                type_code = int(f'1{fountain_tcode}')
-                                relay_tc = type_code
                                 conn_url = f'{self.base_url}{Endpoint.BLE_CONNECT}'
                                 ble_data = {
                                     'bleId': device_details['result']['id'],
                                     'mac': mac,
-                                    'type': type_code
+                                    'type': relay_tc
                                 }
                                 conn_resp = await self._post(conn_url, header, ble_data)
                                 # Check to see if BLE connection was successful
                                 if conn_resp['result']['state'] != 1:
                                     LOGGER.warning(f'BLE connection to {device_details["result"]["name"]} failed. Will try again during next refresh.')
                                     fountain_data = device_details
                                 else:
@@ -281,14 +278,20 @@
                     sound_list: dict[int, str] = {}
                     feeder_url = f'{self.base_url}/{device["type"].lower()}{Endpoint.DEVICE_DETAIL}'
                     data = {
                         'id': device['data']['id']
                     }
                     feeder_data = await self._post(feeder_url, header, data)
 
+                    # Populate the last manual feeding ID for the Gemini(d4s) feeder if it exists
+                    if feeder_data['result']['id'] in self.last_manual_feed_id:
+                        last_manual_feed_id = self.last_manual_feed_id[feeder_data['result']['id']]
+                    else:
+                        last_manual_feed_id = None
+
                     if device['type'] == 'D3':
                         sound_list[-1] = 'Default'
                         sound_url = f'{self.base_url}/{device["type"].lower()}{Endpoint.SOUND_LIST}'
                         sound_data = {
                             'deviceId': device['data']['id']
                         }
                         sound_response = await self._post(sound_url, header, sound_data)
@@ -296,15 +299,16 @@
                         for sound in result:
                             sound_list[sound['id']] = sound['name']
 
                     feeders_data[feeder_data['result']['id']] = Feeder(
                         id=feeder_data['result']['id'],
                         data=feeder_data['result'],
                         type=device['type'].lower(),
-                        sound_list=sound_list
+                        sound_list=sound_list,
+                        last_manual_feed_id=last_manual_feed_id
                     )
 
                 # Litter Boxes
                 if device['type'] in LITTER_LIST:
                     ### Fetch device_detail page
                     dd_url = f'{self.base_url}/{device["type"].lower()}{Endpoint.DEVICE_DETAIL}'
                     dd_data = {
@@ -603,16 +607,14 @@
             elif command in W5_LIGHT_BRIGHTNESS:
                 if water_fountain.data['settings']['lampRingSwitch'] != 1:
                     raise PetKitError(f'{water_fountain.data["name"]} indicator light is Off. You can only change light brightness when the indicator light is On.')
                 else:
                     ble_data = await self.create_ble_data(command, water_fountain)
             # Handle all other commands
             else:
-                # Also send current light brightness in case command is to turn indicator light on/off
-#                light_brightness = water_fountain.data['settings']['lampRingBrightness']
                 ble_data = await self.create_ble_data(command, water_fountain)
             header = await self.create_header()
             conn_data = {
                 'bleId': water_fountain.data['id'],
                 'mac': water_fountain.data['mac'],
                 'type': water_fountain.ble_relay
             }
@@ -630,15 +632,15 @@
             }
             # Initiate BLE connection and poll
             await self._post(connect_url, header, conn_data)
             await self._post(poll_url, header, conn_data)
             # Ensure BLE connection is made before sending command
             await asyncio.sleep(2)
             # Send command to water fountain via BLE relay
-            send_command = await self._post(command_url, header, command_data)
+            await self._post(command_url, header, command_data)
             # Reset ble_sequence
             self.ble_sequence = 0
 
     async def call_pet(self, feeder: Feeder) -> None:
         """Call pet on D3 (Infinity) feeder."""
 
         url = f'{self.base_url}/{feeder.type}{Endpoint.CALL_PET}'
@@ -714,15 +716,15 @@
 
             if command == LitterBoxCommand.PAUSE_CLEAN:
                 self.manually_paused[litter_box.id] = True
                 ## The manual pause will end after a 10-minute wait + 1 minute to complete cleaning
                 self.manual_pause_end[litter_box.id] = datetime.now() + timedelta(seconds=660)
 
     async def check_manual_pause_expiration(self, id: int):
-        """Check to see if manual pause has expired and litter box resumed the cleanin on its own."""
+        """Check to see if manual pause has expired and litter box resumed the cleaning on its own."""
 
         current_dt = datetime.now()
         current_end = self.manual_pause_end[id]
         if (current_end - current_dt).total_seconds() <= 0:
             self.manual_pause_end[id] = None
             self.manually_paused[id] = False
 
@@ -741,14 +743,38 @@
             'amount': amount,
             'day': str(datetime.now().date()).replace('-', ''),
             'deviceId': feeder.id,
             'time': '-1'
         }
         await self._post(url, header, data)
 
+    async def dual_hopper_manual_feeding(self, feeder: Feeder, amount1: int = 0, amount2: int = 0) -> None:
+        """Dispense food manually for dual hopper Gemini feeder.
+        Allowed amount for each side ranges from 0 to 10 portions.
+        """
+
+        invalid_amount1 = (amount1 < 0) or (amount1 > 10)
+        invalid_amount2 = (amount2 < 0) or (amount2 > 10)
+        if invalid_amount1 or invalid_amount2:
+            raise PetKitError('Invalid portion amount specified. Each hopper can only take a portion value between/including 0 to 10')
+        else:
+            url = f'{self.base_url}/{feeder.type}{Endpoint.MANUAL_FEED}'
+            header = await self.create_header()
+            data = {
+                'amount1': amount1,
+                'amount2': amount2,
+                'day': str(datetime.now().date()).replace('-', ''),
+                'deviceId': feeder.id,
+                'name': '',
+                'time': '-1'
+            }
+            response = await self._post(url, header, data)
+            feeder.last_manual_feed_id = response['result']['id']
+            self.last_manual_feed_id[feeder.id] = response['result']['id']
+
     async def update_feeder_settings(self, feeder: Feeder, setting: FeederSetting, value: int) -> None:
         """Change the setting on a feeder."""
 
         if feeder.type == 'feedermini':
             url = f'{self.base_url}{Endpoint.MINI_SETTING}'
         # D3 and D4 Feeders
         else:
@@ -792,18 +818,31 @@
         await self._post(url, header, data)
 
     async def cancel_manual_feed(self, feeder: Feeder) -> None:
         """Cancel a manual feed that is currently in progress. Not available for mini feeders"""
 
         url = f'{self.base_url}/{feeder.type}{Endpoint.CANCEL_FEED}'
         header = await self.create_header()
-        data = {
-            'day': str(datetime.now().date()).replace('-', ''),
-            'deviceId': feeder.id
-        }
+        if feeder.type == 'd4s':
+            if feeder.last_manual_feed_id is None:
+                raise PetKitError('Unable to cancel manual feeding. No valid last manual feeding ID found.')
+            else:
+                data = {
+                    'day': str(datetime.now().date()).replace('-', ''),
+                    'deviceId': feeder.id,
+                    'id': feeder.last_manual_feed_id
+                }
+                self.last_manual_feed_id[feeder.id] = None
+                # Reset the last manual feed id attribute
+                feeder.last_manual_feed_id = None
+        else:
+            data = {
+                'day': str(datetime.now().date()).replace('-', ''),
+                'deviceId': feeder.id
+            }
         await self._post(url, header, data)
 
     async def reset_feeder_desiccant(self, feeder: Feeder) -> None:
         """Reset the desiccant of a single feeder."""
 
         if feeder.type == 'feedermini':
             url = f'{self.base_url}{Endpoint.MINI_DESICCANT_RESET}'
@@ -822,7 +861,25 @@
             raise PetKitError('Invalid litter box type. Only Pura Max litter boxes have N50 odor eliminators.')
         url = f'{self.base_url}/{litter_box.type}{Endpoint.MAX_ODOR_RESET}'
         header = await self.create_header()
         data = {
             'deviceId': litter_box.id
         }
         await self._post(url, header, data)
+
+    async def food_replenished(self, feeder: Feeder) -> None:
+        """Tell PetKit servers that food in the feeder has been replenished.
+        Currently only used for the D4s (Gemini) feeder.
+        If you don't send this command after adding food to the feeder containers,
+        the food state (empty/not empty) won't change until the next scheduled or manual feeding.
+        """
+
+        if feeder.type != 'd4s':
+            raise PetKitError('The food_replenished method is only used with D4s (Gemini) feeders.')
+        else:
+            url = f'{self.base_url}/{feeder.type}{Endpoint.REPLENISHED_FOOD}'
+            header = await self.create_header()
+            data = {
+                'deviceId': feeder.id,
+                'noRemind': 3
+            }
+            await self._post(url, header, data)
```

### Comparing `petkitaio-0.1.2/petkitaio/str_enum.py` & `petkitaio-0.1.3/petkitaio/str_enum.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.2/petkitaio.egg-info/PKG-INFO` & `petkitaio-0.1.3/petkitaio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petkitaio
-Version: 0.1.2
+Version: 0.1.3
 Summary: Asynchronous Python library for PetKit's API
 Home-page: https://github.com/RobertD502/petkitaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/petkitaio/issues
 Project-URL: Source, https://github.com/RobertD502/petkitaio/
@@ -13,16 +13,19 @@
         Asynchronous Python library for PetKit's API.
         
         This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. Although support has been added for the PetKit Asia API endpoint, I have not personally tested it.
         
         ## **Currently Supported Devices**:
         - [D3 Feeder (Fresh Element Infinity)](https://www.amazon.com/PETKIT-Automatic-Stainless-Programmable-Dispenser/dp/B09JFK8BCQ)
         - [D4 Feeder (Fresh Element Solo)](https://www.amazon.com/PETKIT-Automatic-Dispenser-Compatible-Freeze-Dried/dp/B09158J9PF/)
+        - [D4s Feeder (Fresh Element Gemini)](https://www.amazon.com/PETKIT-Automatic-Combination-Dispenser-Stainless/dp/B0BF56RTQH)
         - [Mini Feeder](https://www.amazon.com/PETKIT-Automatic-Stainless-Indicator-Dispenser-2-8L/dp/B08GS1CPHH/)
+        - [W5 Water Fountain (Eversweet Solo 2)](https://www.amazon.com/PETKIT-EVERSWEET-Wireless-Visualization-Dispenser-2L/dp/B0B3RWF653)
         - [W5 Water Fountain (Eversweet 3 Pro)](https://www.amazon.com/PETKIT-Wireless-Fountain-Stainless-Dispenser/dp/B09QRH6L3M/)
+        - [W5 Water Fountain (Eversweet 5 Mini)](https://www.petkit.nl/products/eversweet-5-mini-binnen-2-weken-geleverd)
         - [T3 Litter Box (Pura X)](https://www.amazon.com/PETKIT-Self-Cleaning-Scooping-Automatic-Multiple/dp/B08T9CCP1M)
         - [T4 Litter Box (Pura MAX) with/without Pura Air](https://www.amazon.com/PETKIT-Self-Cleaning-Capacity-Multiple-Automatic/dp/B09KC7Q4YF)
         
         ## Important
         
         PetKit accounts can only be logged in on one device at a time. Using this library will result in getting signed out of the mobile app. You can avoid this by creating a secondary account and sharing devices from the main account (except water fountains). However, some device functionality is lost when using a secondary account as well as not being able to share pets between accounts.
```

### Comparing `petkitaio-0.1.2/setup.py` & `petkitaio-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="petkitaio",
-    version="0.1.2",
+    version="0.1.3",
     author="Robert Drinovac",
     author_email="unlisted@gmail.com",
     description="Asynchronous Python library for PetKit's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RobertD502/petkitaio',
     keywords='petkit, eversweet 3 pro, feeder mini, d4, petkit feeder, petkit water fountain, freshelement solo, pura x, pura max, pura air',
```

