# Comparing `tmp/panos_upgrade_assurance-0.0.2.tar.gz` & `tmp/panos_upgrade_assurance-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panos_upgrade_assurance-0.0.2.tar", max compression
+gzip compressed data, was "panos_upgrade_assurance-0.1.0.tar", max compression
```

## Comparing `panos_upgrade_assurance-0.0.2.tar` & `panos_upgrade_assurance-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-05-31 01:35:38.966524 panos_upgrade_assurance-0.0.2/LICENSE
--rw-r--r--   0        0        0      930 2023-05-31 01:35:38.966524 panos_upgrade_assurance-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-05-31 01:35:38.970525 panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/__init__.py
--rw-r--r--   0        0        0    36412 2023-05-31 01:35:38.970525 panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/check_firewall.py
--rw-r--r--   0        0        0    34581 2023-05-31 01:35:38.970525 panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/firewall_proxy.py
--rw-r--r--   0        0        0    30971 2023-05-31 01:35:38.970525 panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/snapshot_compare.py
--rw-r--r--   0        0        0    12052 2023-05-31 01:35:38.970525 panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/utils.py
--rw-r--r--   0        0        0      932 2023-05-31 01:36:17.018704 panos_upgrade_assurance-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 panos_upgrade_assurance-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-21 08:45:29.863809 panos_upgrade_assurance-0.1.0/LICENSE
+-rw-r--r--   0        0        0      930 2023-06-21 08:45:29.863809 panos_upgrade_assurance-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 08:45:29.863809 panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/__init__.py
+-rw-r--r--   0        0        0    37984 2023-06-21 08:45:29.867810 panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/check_firewall.py
+-rw-r--r--   0        0        0     2325 2023-06-21 08:45:29.867810 panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/exceptions.py
+-rw-r--r--   0        0        0    36113 2023-06-21 08:45:29.867810 panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/firewall_proxy.py
+-rw-r--r--   0        0        0    31244 2023-06-21 08:45:29.867810 panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/snapshot_compare.py
+-rw-r--r--   0        0        0    11662 2023-06-21 08:45:29.867810 panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/utils.py
+-rw-r--r--   0        0        0     1120 2023-06-21 08:45:52.296277 panos_upgrade_assurance-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 panos_upgrade_assurance-0.1.0/PKG-INFO
```

### Comparing `panos_upgrade_assurance-0.0.2/LICENSE` & `panos_upgrade_assurance-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.0.2/README.md` & `panos_upgrade_assurance-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/check_firewall.py` & `panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/check_firewall.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,77 +8,65 @@
     ConfigParser,
     interpret_yes_no,
     CheckType,
     SnapType,
     CheckStatus,
 )
 from panos_upgrade_assurance.firewall_proxy import FirewallProxy
+from panos_upgrade_assurance import exceptions
 from panos import PanOSVersion
-from panos.errors import PanDeviceXapiError
-
-
-class ContentDBVersionInFutureException(Exception):
-    """Used when the installed Content DB version is newer than the latest available version."""
-
-    pass
-
-
-class WrongDataTypeException(Exception):
-    """Used when passed configuration does not meet the data type requirements."""
-
-    pass
-
-
-class ImageVersionNotAvailableException(Exception):
-    """Used when requested image version is not available for downloading."""
-
-    pass
-
-
-class UpdateServerConnectivityException(Exception):
-    """Used when connection to the Update Server cannot be established."""
-
-    pass
 
 
 class CheckFirewall:
     """Class responsible for running readiness checks and creating Firewall state snapshots.
 
     This class is designed to:
 
     * run one or more [`FirewallProxy`](/panos/docs/panos-upgrade-assurance/api/firewall_proxy#class-firewallproxy) class methods,
     * gather and interpret results,
     * present results.
 
     It is split into two parts responsible for:
 
     1. running readiness checks, all methods related to this functionality are prefixed with `check_`,
-    2. running state snapshots, all methods related to this functionality are prefixed with `get_`, although usually the [`FirewallProxy`](/panos/docs/panos-upgrade-assurance/api/firewall_proxy#class-firewallproxy) methods are run directly.
+    2. running state snapshots, all methods related to this functionality are prefixed with `get_`, although usually the
+        [`FirewallProxy`](/panos/docs/panos-upgrade-assurance/api/firewall_proxy#class-firewallproxy) methods are run directly.
 
-    Although it is possible to run the methods directly, the preferred way is to run them through one of the following `run` methods:
+    Although it is possible to run the methods directly, the preferred way is to run them through one of the following `run`
+        methods:
 
     * [`run_readiness_checks()`](#checkfirewallrun_readiness_checks) is responsible for running specified readiness checks,
     * [`run_snapshots()`](#checkfirewallrun_snapshots) is responsible for getting a snapshot of specified device areas.
 
     # Attributes
 
-    _snapshot_method_mapping (dict): Internal variable containing a map of all valid snapshot types mapped to the specific methods.
-
-    This mapping is used to verify the requested snapshot types and to map the snapshot with an actual method that will eventually run. Keys in this dictionary are snapshot names as defined in the [`SnapType`](/panos/docs/panos-upgrade-assurance/api/utils#class-snaptype) class, values are references to methods that will be run.
+    _snapshot_method_mapping (dict): Internal variable containing a map of all valid snapshot types mapped to the specific
+        methods.
 
-    _check_method_mapping (dict): Internal variable containing the map of all valid check types mapped to the specific methods. This mapping is used to verify requested check types and to map a check with an actual method that will be eventually run. Keys in this dictionary are check names as defined in the [`CheckType`](/panos/docs/panos-upgrade-assurance/api/utils#class-checktype) class, values are references to methods that will be run.
+        This mapping is used to verify the requested snapshot types and to map the snapshot with an actual method that
+        will eventually run. Keys in this dictionary are snapshot names as defined in the
+        [`SnapType`](/panos/docs/panos-upgrade-assurance/api/utils#class-snaptype) class, values are references to methods that
+        will be run.
+
+    _check_method_mapping (dict): Internal variable containing the map of all valid check types mapped to the specific methods.
+
+        This mapping is used to verify requested check types and to map a check with an actual method that will be eventually run.
+        Keys in this dictionary are check names as defined in the
+        [`CheckType`](/panos/docs/panos-upgrade-assurance/api/utils#class-checktype) class, values are references to methods that
+        will be run.
 
     """
 
     def __init__(self, node: FirewallProxy) -> None:
         """CheckFirewall constructor.
 
         # Parameters
 
-        node (FirewallProxy): Object representing a device against which checks and/or snapshots are run. See [`FirewallProxy`](/panos/docs/panos-upgrade-assurance/api/firewall_proxy#class-firewallproxy) class' documentation.
+        node (FirewallProxy): Object representing a device against which checks and/or snapshots are run. See
+            [`FirewallProxy`](/panos/docs/panos-upgrade-assurance/api/firewall_proxy#class-firewallproxy) class' documentation.
 
         """
         self._node = node
         self._snapshot_method_mapping = {
             SnapType.NICS: self._node.get_nics,
             SnapType.ROUTES: self._node.get_routes,
             SnapType.LICENSE: self._node.get_licenses,
@@ -99,30 +87,32 @@
             CheckType.SESSION_EXIST: self.check_critical_session,
             CheckType.ARP_ENTRY_EXIST: self.check_arp_entry,
             CheckType.IPSEC_TUNNEL_STATUS: self.check_ipsec_tunnel_status,
             CheckType.FREE_DISK_SPACE: self.check_free_disk_space,
             CheckType.MP_DP_CLOCK_SYNC: self.check_mp_dp_sync,
         }
         locale.setlocale(
-            locale.LC_ALL, "en_US"
+            locale.LC_ALL, "en_US.UTF-8"
         )  # force locale for datetime string parsing when non-English locale is set on host
 
     def check_pending_changes(self) -> CheckResult:
         """Check if there are pending changes on device.
 
         It checks two states:
 
         1. if there is full commit required on the device,
         2. if not, if there is a candidate config pending on a device.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class representing the result of the content version check:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class \
+            representing the result of the content version check:
 
-        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) if there is no pending configuration,
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) if there is no pending
+            configuration,
         * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) otherwise.
 
         """
         if self._node.is_full_commit_required():
             return CheckResult(reason="Full commit required on device.")
         else:
             if self._node.is_pending_changes():
@@ -131,51 +121,63 @@
                 return CheckResult(status=CheckStatus.SUCCESS)
 
     def check_panorama_connectivity(self) -> CheckResult:
         """Check connectivity with the Panorama service.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class representing a state of Panorama connection:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class \
+            representing a state of Panorama connection:
 
-        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when device is connected to Panorama,
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when device is connected to
+            Panorama,
         * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) otherwise,
-        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) is returned when no Panorama configuration is found.
+        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) is returned when no Panorama
+            configuration is found.
 
         """
 
         if self._node.is_panorama_configured():
             if self._node.is_panorama_connected():
                 return CheckResult(status=CheckStatus.SUCCESS)
             else:
                 return CheckResult(reason="Device not connected to Panorama.")
         else:
-            return CheckResult(
-                status=CheckStatus.ERROR, reason="Device not configured with Panorama."
-            )
+            return CheckResult(status=CheckStatus.ERROR, reason="Device not configured with Panorama.")
 
-    def check_ha_status(self, skip_config_sync: Optional[bool] = False) -> CheckResult:
+    def check_ha_status(
+        self,
+        skip_config_sync: Optional[bool] = False,
+        ignore_non_functional: Optional[bool] = False,
+    ) -> CheckResult:
         """Checks HA pair status from the perspective of the current device.
 
         Currently, only Active-Passive configuration is supported.
 
-        # Parameters:
+        # Parameters
 
-        skip_config_sync (bool, optional): (defaults to `False`) Use with caution, when set to `True` will skip checking if configuration is synchronized between nodes. Helpful when verifying a state of a partially upgraded HA pair.
+        skip_config_sync (bool, optional): (defaults to `False`) Use with caution, when set to `True` will skip checking if
+            configuration is synchronized between nodes. Helpful when verifying a state of a partially upgraded HA pair.
+        ignore_non_functional (bool, optional): (defaults to `False`) Use with caution, when set to `True` will ignore if device
+            state is `non-functional` on one of the nodes. Helpful when verifying a state of a partially upgraded HA pair with
+            vmseries plugin version mismatch.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class representing results of HA pair status inspection:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class \
+            representing results of HA pair status inspection:
 
-        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when pair is configured correctly,
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when pair is configured
+            correctly,
         * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) otherwise,
-        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) is returned when device is not a member of an HA pair or the pair is not in Active-Passive configuration.
+        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) is returned when device is not a
+            member of an HA pair or the pair is not in Active-Passive configuration.
 
         """
-        states = ("active", "passive")
+        states = ("active", "passive") if not ignore_non_functional else ("active", "passive", "non-functional")
 
         ha_config = self._node.get_ha_configuration()
         result = CheckResult()
 
         if interpret_yes_no(ha_config["enabled"]):
             ha_pair = ha_config["group"]
 
@@ -195,88 +197,111 @@
 
             elif (
                 not skip_config_sync
                 and interpret_yes_no(ha_pair["running-sync-enabled"])
                 and ha_pair["running-sync"] != "synchronized"
             ):
                 result.status = CheckStatus.ERROR
-                result.reason = (
-                    "Device configuration is not synchronized between the nodes."
-                )
+                result.reason = "Device configuration is not synchronized between the nodes."
 
             else:
                 result.status = CheckStatus.SUCCESS
         else:
             result.reason = "Device is not a member of an HA pair."
             result.status = CheckStatus.ERROR
 
         return result
 
     def check_is_ha_active(
-        self, skip_config_sync: Optional[bool] = False
+        self,
+        skip_config_sync: Optional[bool] = False,
+        ignore_non_functional: Optional[bool] = False,
     ) -> CheckResult:
         """Checks whether this is an active node of an HA pair.
 
-        Before checking the state of the current device, the [`check_ha_status()`](#checkfirewallcheck_ha_status) method is run. If this method does not end with [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus), its return value is passed as the result of [`check_is_ha_active()`](#checkfirewallcheck_is_ha_active).
+        Before checking the state of the current device, the [`check_ha_status()`](#checkfirewallcheck_ha_status) method is run.
+        If this method does not end with
+        [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus), its return value is passed as
+        the result of [`check_is_ha_active()`](#checkfirewallcheck_is_ha_active).
 
-        Detailed results matrix looks like this:
+        Detailed results matrix looks like this
 
-        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) the actual state of the device in an HA pair is checked, if the state is:
-            * active - [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) is returned,
-            * passive - [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) is returned,
-        * anything else than [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus), the [`check_ha_status()`](#checkfirewallcheck_ha_status) return value is passed as a return value of this method.
+        - [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) the actual state of the device
+            in an HA pair is checked, if the state is
+
+            - active - [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) is returned,
+            - passive - [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) is returned,
+
+
+        - anything else than [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus), the
+        [`check_ha_status()`](#checkfirewallcheck_ha_status) return value is passed as a return value of this method.
 
 
         # Parameters
 
-        skip_config_sync (bool, optional): (defaults to `False`) Use with caution, when set to `True` will skip checking if configuration is synchronized between nodes. Helpful when working with a partially upgraded HA pair.
+        skip_config_sync (bool, optional): (defaults to `False`) Use with caution, when set to `True` will skip checking if
+            configuration is synchronized between nodes. Helpful when working with a partially upgraded HA pair.
+        ignore_non_functional (bool, optional): (defaults to `False`) Use with caution, when set to `True` will ignore if device
+            state is `non-functional` on one of the nodes. Helpful when verifying a state of a partially upgraded HA pair with
+            vmseries plugin version mismatch.
 
         # Returns
 
         CheckResult: Boolean information reflecting the state of the device.
 
         """
-        ha_status = self.check_ha_status(skip_config_sync=skip_config_sync)
+        ha_status = self.check_ha_status(
+            skip_config_sync=skip_config_sync,
+            ignore_non_functional=ignore_non_functional,
+        )
         if ha_status:
             ha_config = self._node.get_ha_configuration()
             result = CheckResult()
             if ha_config["group"]["local-info"]["state"] == "active":
                 result.status = CheckStatus.SUCCESS
             else:
-                result.reason = (
-                    f"Node state is: {ha_config['group']['local-info']['state']}."
-                )
+                result.reason = f"Node state is: {ha_config['group']['local-info']['state']}."
             return result
         else:
             return ha_status
 
     def check_expired_licenses(self, skip_licenses: Optional[list] = []) -> CheckResult:
         """Check if any license is expired.
 
         # Parameters
 
         skip_licenses (list, optional): (defaults to `[]`) List of license names that should be skipped during the check.
 
+        # Raises
+
+        WrongDataTypeException: Raised when `skip_licenses` is not type of `list`.
+
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking \
+            value of:
 
         * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) if no license is expired,
-        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) otherwise.
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) otherwise
+        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when there is not license
+        information available in the API response.
 
         """
         if not isinstance(skip_licenses, list):
-            raise WrongDataTypeException(
-                f"The skip_licenses variable is a {type(skip_licenses)} but should be a list"
-            )
+            raise exceptions.WrongDataTypeException(f"The skip_licenses variable is a {type(skip_licenses)} but should be a list")
 
-        licenses = self._node.get_licenses()
+        result = CheckResult()
+        try:
+            licenses = self._node.get_licenses()
+        except exceptions.DeviceNotLicensedException as exp:
+            result.status = CheckStatus.ERROR
+            result.reason = str(exp)
+            return result
 
         expired_licenses = ""
-        result = CheckResult()
         for lic, value in licenses.items():
             if lic not in skip_licenses:
                 if interpret_yes_no(value["expired"]):
                     expired_licenses += f"{lic}, "
 
         if expired_licenses:
             result.reason = f"Found expired licenses:  {expired_licenses[:-2]}."
@@ -284,45 +309,48 @@
             result.status = CheckStatus.SUCCESS
 
         return result
 
     def check_active_support_license(self) -> CheckResult:
         """Check active support license with update server.
 
-        # Raises
-
-        UpdateServerConnectivityException: Thrown when a connection to an update server cannot be established during support license verification.
-
         # Returns
 
         dict: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
 
-        - [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) if the support license is not expired,
+        - [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) if the support license is not
+            expired,
         - [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) otherwise,
-        - [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when no information about the support license expiration date can be found in response from the firewall.
+        - [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when no information cannot be
+        retrieved or found in the API response.
 
         """
 
         result = CheckResult()
 
         try:
+            self._node.get_licenses()
+        except exceptions.DeviceNotLicensedException as exp:
+            result.status = CheckStatus.ERROR
+            result.reason = str(exp)
+            return result
+
+        try:
             support_license = self._node.get_support_license()
-        except PanDeviceXapiError as exc:  # raised when connectivity timeouts
-            raise UpdateServerConnectivityException(
-                "Can not reach update servers to check active support license."
-            ) from exc
+        except exceptions.UpdateServerConnectivityException:  # raised when connectivity timeouts
+            result.reason = "Can not reach update servers to check active support license."
+            result.status = CheckStatus.ERROR
+            return result
 
         if not support_license.get("support_expiry_date"):  # if None or empty string
             result.reason = "No ExpiryDate found for support license."
             result.status = CheckStatus.ERROR
             return result
 
-        dt_expiry = datetime.strptime(
-            support_license["support_expiry_date"], "%B %d, %Y"
-        )
+        dt_expiry = datetime.strptime(support_license["support_expiry_date"], "%B %d, %Y")
         dt_today = datetime.now()
 
         if dt_expiry < dt_today:
             result.reason = "Support License expired."
         else:
             result.status = CheckStatus.SUCCESS
 
@@ -336,21 +364,24 @@
     ) -> CheckResult:
         """Check if a critical session is present in the sessions table.
 
         # Parameters
 
         source (str, optional): (defaults to `None`) Source IPv4 address for the examined session.
         destination (str, optional): (defaults to `None`) Destination IPv4 address for the examined session.
-        dest_port (int, str, optional): (defaults to `None`) Destination port value. This should be an integer value, but string representations such as `"8080"` are also accepted.
+        dest_port (int, str, optional): (defaults to `None`) Destination port value. This should be an integer value, but string
+        representations such as `"8080"` are also accepted.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking \
+            value of:
 
-        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) if a session is found in the sessions table,
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) if a session is found in the
+        sessions table,
         * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) otherwise,
         * [`CheckStatus.SKIPPED`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when no config is passed,
         * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) if the session table is empty.
 
         """
 
         result = CheckResult()
@@ -385,64 +416,65 @@
         * w/o any configuration - checks if the latest version of the Content DB is installed.
         * with specific version passed - verifies if the installed Content DB is at least equal.
 
         # Parameters
 
         version (str, optional): (defaults to `None`) Target version of the content DB.
 
-        # Raises
-
-        ContentDBVersionInFutureException: If the data returned from a device is newer than the latest version available.
-
         # Returns
-        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value off:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking \
+            value off:
 
-        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when the installed Content DB met the requirements.
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when the installed Content DB
+            met the requirements.
         * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when it did not.
 
         """
         result = CheckResult()
 
-        required_version = (
-            version if version else self._node.get_latest_available_content_version()
-        )
+        try:
+            required_version = version if version else self._node.get_latest_available_content_version()
+        except exceptions.ContentDBVersionsFormatException as exp:
+            result.reason = str(exp)
+            result.status = CheckStatus.ERROR
+            return result
+
         installed_version = self._node.get_content_db_version()
 
         if required_version == installed_version:
             result.status = CheckStatus.SUCCESS
         else:
             exception_text = f"Wrong data returned from device, installed version ({installed_version}) is higher than the required_version available ({required_version})."
-            conditional_success_text = f"Installed content DB version ({installed_version}) is higher than the requested one ({required_version})."
+            conditional_success_text = (
+                f"Installed content DB version ({installed_version}) is higher than the requested one ({required_version})."
+            )
 
             # we already know that the versions are different, so as a default result we assume FAILED
             # now let's handle corner cases
-            if int(required_version.split("-")[0]) < int(
-                installed_version.split("-")[0]
-            ):
+            if int(required_version.split("-")[0]) < int(installed_version.split("-")[0]):
                 # if the passed required version is higher that the installed then we assume the test passed
                 # this is a type of a test where we look for the minimum version
                 if version:
                     result.status = CheckStatus.SUCCESS
                     result.reason = conditional_success_text
                 else:
                     # in case where no version was passed we treat this situation as an exception
                     # latest version cannot by lower than the installed one.
-                    raise ContentDBVersionInFutureException(exception_text)
-            elif int(required_version.split("-")[0]) == int(
-                installed_version.split("-")[0]
-            ):
+                    result.status = CheckStatus.ERROR
+                    result.reason = exception_text
+
+            elif int(required_version.split("-")[0]) == int(installed_version.split("-")[0]):
                 # majors the same, compare minors assuming the same logic we used for majors
-                if int(required_version.split("-")[1]) < int(
-                    installed_version.split("-")[1]
-                ):
+                if int(required_version.split("-")[1]) < int(installed_version.split("-")[1]):
                     if version:
                         result.status = CheckStatus.SUCCESS
                         result.reason = conditional_success_text
                     else:
-                        raise ContentDBVersionInFutureException(exception_text)
+                        result.status = CheckStatus.ERROR
+                        result.reason = exception_text
 
             if not result:
                 reason_suffix = (
                     f"older then the request one ({required_version})."
                     if version
                     else f"not the latest one ({required_version})."
                 )
@@ -451,19 +483,23 @@
         return result
 
     def check_ntp_synchronization(self) -> CheckResult:
         """Check synchronization with NTP server.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking \
+            value of:
 
-        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when a device is synchronized with the NTP server.
-        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when a device is not synchronized with the NTP server.
-        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when a device is not configured for NTP synchronization.
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when a device is synchronized
+            with the NTP server.
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when a device is not synchronized
+            with the NTP server.
+        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when a device is not configured
+            for NTP synchronization.
 
         """
 
         result = CheckResult()
 
         response = self._node.get_ntp_servers()
         if response["synched"] == "LOCAL":
@@ -483,27 +519,27 @@
             if synched in [v["name"] for v in response.values()]:
                 result.status = CheckStatus.SUCCESS
             else:
                 result.reason = f"NTP synchronization in unknown state: {synched}."
 
         return result
 
-    def check_arp_entry(
-        self, ip: Optional[str] = None, interface: Optional[str] = None
-    ) -> CheckResult:
+    def check_arp_entry(self, ip: Optional[str] = None, interface: Optional[str] = None) -> CheckResult:
         """Check if a given ARP entry is available in the ARP table.
 
         # Parameters
 
-        interface (str, optional): (defaults to `None`) A name of an interface we examine for the ARP entries. When skipped, all interfaces are examined.
+        interface (str, optional): (defaults to `None`) A name of an interface we examine for the ARP entries. When skipped, all
+            interfaces are examined.
         ip (str, optional): (defaults to `None`) IP address of the ARP entry we look for.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking \
+            value of:
 
         * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when the ARP entry is found.
         * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when the ARP entry is not found.
         * [`CheckStatus.SKIPPED`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when `ip` is not provided.
         * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when the ARP table is empty.
 
         """
@@ -520,44 +556,45 @@
         if not arp_table:
             result.reason = "ARP table empty."
             result.status = CheckStatus.ERROR
             return result
 
         for arp_entry in arp_table.values():
             if interface is not None:
-                found = ip == arp_entry.get("ip") and interface == arp_entry.get(
-                    "interface"
-                )
+                found = ip == arp_entry.get("ip") and interface == arp_entry.get("interface")
             else:
                 found = ip == arp_entry.get("ip")
 
             if found:
                 result.status = CheckStatus.SUCCESS
                 return result
 
         result.reason = "Entry not found in ARP table."
         return result
 
-    def check_ipsec_tunnel_status(
-        self, tunnel_name: Optional[str] = None
-    ) -> CheckResult:
+    def check_ipsec_tunnel_status(self, tunnel_name: Optional[str] = None) -> CheckResult:
         """Check if a given IPSec tunnel is in active state.
 
         # Parameters
 
         tunnel_name (str, optional): (defaults to `None`) Name of the searched IPSec tunnel.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking \
+            value of:
 
-        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when a tunnel is found and is in active state.
-        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when a tunnel is either not active or missing in the current configuration.
-        * [`CheckStatus.SKIPPED`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when `tunnel_name` is not provided.
-        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when no IPSec tunnels are configured on the device.
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when a tunnel is found and is
+            in active state.
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when a tunnel is either not
+            active or missing in the current configuration.
+        * [`CheckStatus.SKIPPED`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when `tunnel_name` is not
+            provided.
+        * [`CheckStatus.ERROR`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when no IPSec tunnels are
+            configured on the device.
 
         """
 
         result = CheckResult()
 
         if tunnel_name is None:
             result.status = CheckStatus.SKIPPED
@@ -587,92 +624,104 @@
     def check_free_disk_space(self, image_version: Optional[str] = None) -> CheckResult:
         """Check if a there is enough space on the `/opt/panrepo` volume for downloading an PanOS image.
 
         This is a check intended to be run before the actual upgrade process starts.
 
         The method operates in two modes:
 
-        * default - to be used as last resort, it will verify that the `/opt/panrepo` volume has at least 3GB free space available. This amount of free space is somewhat arbitrary and it's based maximum image sizes (path level + base image) available at the time the method was written (+ some additional error margin).
-        * specific target image - suggested mode, it will take one argument `image_version` which is the target PanOS version. For that version the actual image size (path + base image) will be calculated. Next, the available free space is verified against that image size + 10% (as an error margin).
+        * default - to be used as last resort, it will verify that the `/opt/panrepo` volume has at least 3GB free space
+            available. This amount of free space is somewhat arbitrary and it's based maximum image sizes
+            (path level + base image) available at the time the method was written (+ some additional error margin).
+        * specific target image - suggested mode, it will take one argument `image_version` which is the target PanOS version.
+            For that version the actual image size (path + base image) will be calculated. Next, the available free space
+            is verified against that image size + 10% (as an error margin).
 
         # Parameters
 
         image_version (str, optional): (defaults to `None`) Version of the target PanOS image.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking \
+            value of:
 
-        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when there is enough free space to download an image.
-        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when there is NOT enough free space, additionally the actual free space available is provided as the fail reason.
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when there is enough free
+            space to download an image.
+        * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when there is NOT enough free
+            space, additionally the actual free space available is provided as the fail reason.
 
         """
         result = CheckResult()
         minimum_free_space = ceil(3.0 * 1024)
         if image_version:
             image_sem_version = PanOSVersion(image_version)
-            available_versions = self._node.get_available_image_data()
+            try:
+                available_versions = self._node.get_available_image_data()
+            except exceptions.UpdateServerConnectivityException:
+                result.reason = "Unable to retrieve target image size most probably due to network issues or because the device is not licensed."
+                result.status = CheckStatus.ERROR
+                return result
 
             if str(image_sem_version) in available_versions:
                 requested_base_image_size = 0
-                requested_image_size = int(
-                    available_versions[str(image_sem_version)]["size"]
-                )
+                requested_image_size = int(available_versions[str(image_sem_version)]["size"])
 
                 if image_sem_version.patch != 0:
-                    base_image_version = (
-                        f"{image_sem_version.major}.{image_sem_version.minor}.0"
-                    )
+                    base_image_version = f"{image_sem_version.major}.{image_sem_version.minor}.0"
                     if base_image_version in available_versions:
-                        if not interpret_yes_no(
-                            available_versions[base_image_version]["downloaded"]
-                        ):
-                            requested_base_image_size = int(
-                                available_versions[base_image_version]["size"]
-                            )
+                        if not interpret_yes_no(available_versions[base_image_version]["downloaded"]):
+                            requested_base_image_size = int(available_versions[base_image_version]["size"])
                     else:
-                        raise ImageVersionNotAvailableException(
-                            f"Base image {base_image_version} does not exist."
-                        )
+                        result.reason = f"Base image {base_image_version} does not exist."
+                        result.status = CheckStatus.ERROR
 
-                minimum_free_space = ceil(
-                    1.1 * (requested_base_image_size + requested_image_size)
-                )
+                minimum_free_space = ceil(1.1 * (requested_base_image_size + requested_image_size))
 
             else:
-                raise ImageVersionNotAvailableException(
-                    f"Image {str(image_sem_version)} does not exist."
-                )
+                result.reason = f"Image {str(image_sem_version)} does not exist."
+                result.status = CheckStatus.ERROR
+
+        try:
+            free_space = self._node.get_disk_utilization()
+        except exceptions.WrongDiskSizeFormatException as exp:
+            result.reason = str(exp)
+            result.status = CheckStatus.ERROR
+            return result
 
-        free_space = self._node.get_disk_utilization()
         free_space_panrepo = free_space["/opt/panrepo"]
 
         if free_space_panrepo > minimum_free_space:
             result.status = CheckStatus.SUCCESS
         else:
             result.reason = f"There is not enough free space, only {str(round(free_space_panrepo/1024,1)) + 'G' if free_space_panrepo >= 1024 else str(free_space_panrepo) + 'M'}B is available."
         return result
 
     def check_mp_dp_sync(self, diff_threshold: int = 0) -> CheckResult:
         """Check if the Data and Management clocks are in sync.
 
+        # Raises
+
+        WrongDataTypeException: Raised when the `diff_threshold` is not type of `int`.
+
         # Parameters
 
         diff_threshold (int, optional): (defaults to `0`) Maximum allowable difference in seconds between both clocks.
 
         # Returns
 
-        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking value of:
+        CheckResult: Object of [`CheckResult`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkresult) class taking \
+            value of:
 
-        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when both clocks are the same or within threshold.
+        * [`CheckStatus.SUCCESS`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when both clocks are the same
+            or within threshold.
         * [`CheckStatus.FAIL`](/panos/docs/panos-upgrade-assurance/api/utils#class-checkstatus) when both clocks differ.
 
         """
         if not isinstance(diff_threshold, int):
-            raise WrongDataTypeException(
+            raise exceptions.WrongDataTypeException(
                 f"[diff_threshold] should be of type [int] but is of type [{type(diff_threshold)}]."
             )
 
         result = CheckResult()
 
         mp_clock = self._node.get_mp_clock()
         dp_clock = self._node.get_dp_clock()
@@ -695,33 +744,35 @@
         return result
 
     def get_content_db_version(self) -> Dict[str, str]:
         """Get Content DB version.
 
         # Returns
 
-        dict(str): To keep the standard of all `get` methods returning a dictionary this value is also returned as a dictionary in the following format:
+        dict(str): To keep the standard of all `get` methods returning a dictionary this value is also returned as a dictionary \
+            in the following format:
 
-        ``` yaml
+        ```python showLineNumbers
         {
             'version': 'xxxx-yyyy'
         }
         ```
 
         """
         return {"version": self._node.get_content_db_version()}
 
-    def get_ip_sec_tunnels(self) -> Dict[str, Union[str, int]]:
+    def get_ip_sec_tunnels(self) -> Dict[str, dict]:
         """Extract information about IPSEC tunnels from all tunnel data retrieved from a device.
 
         # Returns
 
-        dict: Currently configured IPSEC tunnels. The returned value is similar to the example below. It can differ though depending on the version of PanOS:
+        dict: Currently configured IPSEC tunnels. The returned value is similar to the example below. It can differ though \
+            depending on the version of PanOS:
 
-        ``` yaml
+        ```python showLineNumbers title="Example"
         {
             "tunnel_name": {
                 "peerip": "10.26.129.5",
                 "name": "tunnel_name",
                 "outer-if": "ethernet1/2",
                 "gwid": "1",
                 "localip": "0.0.0.0",
@@ -731,29 +782,31 @@
                 "owner": "1",
                 "id": "1"
             }
         }
         ```
 
         """
-        return self._node.get_tunnels()["IPSec"]
+        return self._node.get_tunnels().get("IPSec", {})
 
     def run_readiness_checks(
         self,
         checks_configuration: Optional[List[Union[str, dict]]] = None,
         report_style: bool = False,
     ) -> Union[Dict[str, dict], Dict[str, str]]:
         """Run readiness checks.
 
-        This method provides a convenient way of running readiness checks methods. For details on configuration see [readiness checks](/panos/docs/panos-upgrade-assurance/configuration-details#readiness-checks) documentation.
+        This method provides a convenient way of running readiness checks methods. For details on configuration see
+        [readiness checks](/panos/docs/panos-upgrade-assurance/configuration-details#readiness-checks) documentation.
 
         # Parameters
 
         checks_configuration (list(str,dict), optional): (defaults to `None`) List of readiness checks to run.
-        report_style (bool): (defaults to `False`) Changes the output to more descriptive. Can be used when generating a report from the checks.
+        report_style (bool): (defaults to `False`) Changes the output to more descriptive. Can be used when generating a report
+            from the checks.
 
         # Raises
 
         WrongDataTypeException: An exception is raised when the configuration is in a data type different then `str` or `dict`.
 
         # Returns
 
@@ -770,35 +823,28 @@
             if isinstance(check, dict):
                 check_type, check_config = next(iter(check.items()))
                 # check_result = self._check_method_mapping[check_type](check_config)
             elif isinstance(check, str):
                 check_type, check_config = check, {}
                 # check_result = self._check_method_mapping[check_type]()
             else:
-                raise WrongDataTypeException(
-                    f"Wrong configuration format for check: {check}."
-                )
+                raise exceptions.WrongDataTypeException(f"Wrong configuration format for check: {check}.")
 
             check_result = self._check_method_mapping[check_type](
                 **check_config
-            )  # (**) would pass dict config values as seperate parameters to method.
-            result[check_type] = (
-                str(check_result)
-                if report_style
-                else {"state": bool(check_result), "reason": str(check_result)}
-            )
+            )  # (**) would pass dict config values as separate parameters to method.
+            result[check_type] = str(check_result) if report_style else {"state": bool(check_result), "reason": str(check_result)}
 
         return result
 
-    def run_snapshots(
-        self, snapshots_config: Optional[List[Union[str, dict]]] = None
-    ) -> Dict[str, dict]:
+    def run_snapshots(self, snapshots_config: Optional[List[Union[str, dict]]] = None) -> Dict[str, dict]:
         """Run snapshots of different firewall areas states.
 
-        This method provides a convenient way of running snapshots of a device state. For details on configuration see [state snapshots](/panos/docs/panos-upgrade-assurance/configuration-details#state-snapshots) documentation.
+        This method provides a convenient way of running snapshots of a device state. For details on configuration see
+        [state snapshots](/panos/docs/panos-upgrade-assurance/configuration-details#state-snapshots) documentation.
 
         # Parameters
 
         snapshots_config (list(str), optional): (defaults to `None`) Defines snapshots of which areas will be taken.
 
         # Raises
 
@@ -813,14 +859,12 @@
         snaps_list = ConfigParser(
             valid_elements=set(self._snapshot_method_mapping.keys()),
             requested_config=snapshots_config,
         ).prepare_config()
 
         for snap_type in snaps_list:
             if not isinstance(snap_type, str):
-                raise WrongDataTypeException(
-                    f"Wrong configuration format for snapshot: {snap_type}."
-                )
+                raise exceptions.WrongDataTypeException(f"Wrong configuration format for snapshot: {snap_type}.")
 
             result[snap_type] = self._snapshot_method_mapping[snap_type]()
 
         return result
```

### Comparing `panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/firewall_proxy.py` & `panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/firewall_proxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,24 @@
 import xml.etree.ElementTree as ET
 from panos_upgrade_assurance.utils import interpret_yes_no
 from xmltodict import parse as XMLParse
 from typing import Optional, Union
 from panos.firewall import Firewall
+from pan.xapi import PanXapiError
+from panos_upgrade_assurance import exceptions
 from math import floor
 
 
-class CommandRunFailedException(Exception):
-    """Used when a command run on a device does not return the `success` status."""
-
-    pass
-
-
-class MalformedResponseException(Exception):
-    """A generic exception class used when a response does not meet the expected standards."""
-
-    pass
-
-
-class ContentDBVersionsFormatException(Exception):
-    """Used when parsing Content DB versions fail due to an unknown version format (assuming `XXXX-YYYY`)."""
-
-    pass
-
-
-class PanoramaConfigurationMissingException(Exception):
-    """Used when checking Panorama connectivity on a device that was not configured with Panorama."""
-
-    pass
-
-
-class WrongDiskSizeFormatException(Exception):
-    """Used when parsing free disk size information."""
-
-    pass
-
-
 class FirewallProxy(Firewall):
     """Class representing a Firewall.
 
-    Proxy in this class means that it is between the *high level* [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) class and a device itself.
-    Inherits the [Firewall][fw] class but adds methods to interpret XML API commands. The class constructor is also inherited from the [Firewall][fw] class.
+    Proxy in this class means that it is between the *high level*
+    [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) class and a device itself.
+    Inherits the [Firewall][fw] class but adds methods to interpret XML API commands. The class constructor is also inherited
+    from the [Firewall][fw] class.
 
     All interaction with a device are read-only. Therefore, a less privileged user can be used.
 
     All methods starting with `is_` check the state, they do not present any data besides simple `boolean`values.
 
     All methods starting with `get_` fetch data from a device by running a command and parsing the output.
     The return data type can be different depending on what kind of information is returned from a device.
@@ -56,44 +30,48 @@
         self,
         cmd: str,
         cmd_in_xml: Optional[bool] = False,
         return_xml: Optional[bool] = False,
     ) -> Union[dict, ET.Element]:
         """Execute a command on node, parse, and return response.
 
-        This is just a wrapper around the [`Firewall.op()`](https://pan-os-python.readthedocs.io/en/latest/module-firewall.html#panos.firewall.Firewall.op) method. It additionally does basic error handling and tries to extract the actual device response.
+        This is just a wrapper around the
+        [`Firewall.op()`](https://pan-os-python.readthedocs.io/en/latest/module-firewall.html#panos.firewall.Firewall.op) method.
+        It additionally does basic error handling and tries to extract the actual device
+        response.
 
         # Parameters
 
         cmd (str): The actual XML API command to be run on the device. Can be either a free form or an XML formatted command.
         cmd_in_xml (bool): (defaults to `False`) Set to `True` if the command is XML-formatted.
-        return_xml (bool): (defaults to `False`) When set to `True`, the return data is an [`XML object`](https://docs.python.org/3/library/xml.etree.elementtree.html#xml.etree.ElementTree.Element) instead of a python dictionary.
+        return_xml (bool): (defaults to `False`) When set to `True`, the return data is an \
+            [`XML object`](https://docs.python.org/3/library/xml.etree.elementtree.html#xml.etree.ElementTree.Element)
+            instead of a Python dictionary.
 
         # Raises
 
         CommandRunFailedException: An exception is raised if the command run status returned by a device is not successful.
-        MalformedResponseException: An exception is raised when a response is not parsable, no `result` element is found in the XML response.
+        MalformedResponseException: An exception is raised when a response is not parsable, no `result` element is found in the
+            XML response.
 
         # Returns
         dict, xml.etree.ElementTree.Element: The actual command output. A type is defined by the `return_xml` parameter.
 
         """
 
         raw_response = self.op(cmd, xml=False, cmd_xml=not cmd_in_xml, vsys=self.vsys)
         if raw_response.get("status") != "success":
-            raise CommandRunFailedException(f"Failed to run command: {cmd}.")
+            raise exceptions.CommandRunFailedException(f"Failed to run command: {cmd}.")
 
         resp_result = raw_response.find("result")
         if resp_result is None:
-            raise MalformedResponseException(f"No result field returned for: {cmd}")
+            raise exceptions.MalformedResponseException(f"No result field returned for: {cmd}")
 
         if not return_xml:
-            resp_result = XMLParse(
-                ET.tostring(resp_result, encoding="utf8", method="xml")
-            )["result"]
+            resp_result = XMLParse(ET.tostring(resp_result, encoding="utf8", method="xml"))["result"]
 
         return resp_result
 
     def is_pending_changes(self) -> bool:
         """Get information if there is a candidate configuration pending to be committed.
 
         The actual API command run is `check pending-changes`.
@@ -130,89 +108,85 @@
         return False if self.op_parser(cmd="show panorama-status") is None else True
 
     def is_panorama_connected(self) -> bool:
         """Get Panorama connectivity status.
 
         The actual API command run is `show panorama-status`.
 
-        An output of this command is usually a string. This method is responsible for parsing this string and trying to extract information if at least one of the Panoramas configured is connected.
-
-        Since the API response is a string (that we need to parse) this method expects a strict format. For single Panorama this is:
+        An output of this command is usually a string. This method is responsible for parsing this string and trying to extract
+        information if at least one of the Panoramas configured is connected.
 
-        ```python
+        Since the API response is a string (that we need to parse) this method expects a strict format. For single Panorama this
+        is:
 
+        ```yaml showLineNumbers title="Example - single Panorama"
             Panorama Server 1 : 1.2.3.4
                 Connected     : no
                 HA state      : disconnected
         ```
 
         For two Panoramas (HA pair for example) those are just two blocks:
 
-        ```python
-
+        ```yaml showLineNumbers title="Example - HA Panorama"
             Panorama Server 1 : 1.2.3.4
                 Connected     : no
                 HA state      : disconnected
+
             Panorama Server 2 : 5.6.7.8
                 Connected     : yes
                 HA state      : disconnected
         ```
 
         If none of this formats is met, `MalformedResponseException` exception is thrown.
 
         # Raises
 
-        PanoramaConfigurationMissingException: Exception being raised when this check is run against a device with no Panorama configured.
+        PanoramaConfigurationMissingException: Exception being raised when this check is run against a device with no Panorama
+            configured.
         MalformedResponseException: Exception being raised when response from device does not meet required format.
 
 
         # Returns
 
         bool: `True` when connection is up, `False` otherwise.
 
         """
 
         pan_status = self.op_parser(cmd="show panorama-status")
         if pan_status is None:
-            raise PanoramaConfigurationMissingException(
-                "Device not configured with Panorama."
-            )
+            raise exceptions.PanoramaConfigurationMissingException("Device not configured with Panorama.")
 
         if not isinstance(pan_status, str):
-            raise MalformedResponseException(
-                "Response from device is not type of string."
-            )
+            raise exceptions.MalformedResponseException("Response from device is not type of string.")
 
         pan_status_list = pan_status.split("\n")
         pan_status_list_length = len(pan_status_list)
 
-        if pan_status_list_length in [3, 6]:
-            for i in range(1, pan_status_list_length, 3):
-                pan_connected = interpret_yes_no(
-                    (pan_status_list[i].split(":")[1]).strip()
-                )
+        if pan_status_list_length in [3, 7]:
+            for i in range(1, pan_status_list_length, 4):
+                pan_connected = interpret_yes_no((pan_status_list[i].split(":")[1]).strip())
                 if pan_connected:
                     return True
         else:
-            raise MalformedResponseException(
+            raise exceptions.MalformedResponseException(
                 f"Panorama configuration block does not have typical structure: <{pan_status}>."
             )
 
         return False
 
     def get_ha_configuration(self) -> dict:
         """Get high-availability configuration status.
 
         The actual API command is `show high-availability state`.
 
         # Returns
 
-        dict: Information about HA pair and its status as retrieved from the current (local) device. Sample output:
+        dict: Information about HA pair and its status as retrieved from the current (local) device.
 
-        ```yaml
+        ```python showLineNumbers title="Sample output"
         {
             'enabled': 'yes',
             'group': {
                 'link-monitoring': {
                     'enabled': 'yes',
                     'failure-condition': 'any',
                     'groups': None
@@ -338,52 +312,55 @@
 
         # Raises
 
         MalformedResponseException: Exception when no `hw` entry is available in the response.
 
         # Returns
 
-        dict: Status of the configured network interfaces. Sample output:
+        dict: Status of the configured network interfaces.
 
-        ```yaml
+        ```python showLineNumbers title="Sample output"
         {
             'ethernet1/1': 'down',
             'ethernet1/2': 'down',
             'ethernet1/3': 'up'
         }
         ```
 
         """
 
         response = self.op_parser(cmd=r'show interface "hardware"')
 
         hardware = response["hw"]
         if hardware is None:
-            raise MalformedResponseException(
-                "Malformed response from device, no [hw] element present."
-            )
+            raise exceptions.MalformedResponseException("Malformed response from device, no [hw] element present.")
 
         results = {}
         entries = hardware["entry"]
         if isinstance(entries, dict):
             entries = [entries]
         for nic in entries:
             results[nic["name"]] = nic["state"]
         return results
 
     def get_licenses(self) -> dict:
         """Get device licenses.
 
         The actual API command is `request license info`.
 
+        # Raises
+
+        DeviceNotLicensedException: Exception thrown when there is no information about licenses, most probably because the
+            device is not licensed.
+
         # Returns
 
-        dict: Licenses available on a device.. Sample output:
+        dict: Licenses available on a device.
 
-        ```yaml
+        ```python showLineNumbers title="Sample output"
         {
             'AutoFocus Device License': {
                 'authcode': 'Snnnnnnn',
                 'base-license-name': 'PA-VM',
                 'description': 'AutoFocus Device License',
                 'expired': 'yes',
                 'expires': 'September 25, 2010',
@@ -404,27 +381,33 @@
         }
         ```
 
         """
         response = self.op_parser(cmd="request license info")
 
         result = {}
+
+        if response["licenses"] is None:
+            raise exceptions.DeviceNotLicensedException(
+                "Device possibly not licenced - no license information available in the API response."
+            )
+
         licenses = response["licenses"]["entry"]
         for lic in licenses if isinstance(licenses, list) else [licenses]:
             result[lic["feature"]] = dict(lic)
         return result
 
     def get_support_license(self) -> dict:
         """Get support license information from update servers.
 
         The actual API command is `request support check`.
 
         This method fetches the response in XML format:
 
-        ```xml
+        ```xml showLineNumbers
         <SupportInfoResponse>
             <Links>
             <Link>
                 <Title>Contact Us</Title>
                 <Url>https://www.paloaltonetworks.com/company/contact-us.html</Url>
             </Link>
             <Link>
@@ -443,46 +426,57 @@
             <ExpiryDate>December 31, 2023</ExpiryDate>
             <SupportLevel>Premium</SupportLevel>
             <SupportDescription>24 x 7 phone support; advanced replacement hardware service</SupportDescription>
         </Support>
         </SupportInfoResponse>
         ```
 
+        # Raises
+
+        UpdateServerConnectivityException: Raised when timeout is reached when contacting an update server.
+        PanXapiError: Re-raised when an exception is caught but does not match `UpdateServerConnectivityException`.
+
         # Returns
 
         dict: Partial information extracted from the response formatted as `dict`, it includes:
 
         - the expiry date,
         - the support level.
         """
         result = {}
-        response = self.op_parser(cmd="request support check", return_xml=True)
+        try:
+            response = self.op_parser(cmd="request support check", return_xml=True)
+        except PanXapiError as exp:
+            # This is an ugly hack to narrow down the cause of the exception to update server connectivity issues.
+            # Unfortunately the exception class is generic in this case. What is easy to identify is the message.
+            if str(exp) == "Failed to check support info due to Unknown error. Please check network connectivity and try again.":
+                raise exceptions.UpdateServerConnectivityException(str(exp)) from exp
+            else:
+                raise exp
 
-        result["support_expiry_date"] = response.findtext(
-            "./SupportInfoResponse/Support/ExpiryDate"
-        )
-        result["support_level"] = response.findtext(
-            "./SupportInfoResponse/Support/SupportLevel"
-        )
+        result["support_expiry_date"] = response.findtext("./SupportInfoResponse/Support/ExpiryDate")
+        result["support_level"] = response.findtext("./SupportInfoResponse/Support/SupportLevel")
         return result
 
     def get_routes(self) -> dict:
         """Get route table entries, either retrieved from DHCP or configured manually.
 
         The actual API command is `show routing route`.
 
-        In the returned `dict` the key is made of three route properties delimited with an underscore (`_`) in the following order:
+        In the returned `dict` the key is made of three route properties delimited with an underscore (`_`) in the following
+        order:
 
         * virtual router name,
         * destination CIDR,
         * network interface name if one is available, empty string otherwise.
 
-        The key does not provide any meaningful information, it's there only to introduce uniqueness for each entry. All properties that make a key are also available in the value of a dictionary element. Sample output:
+        The key does not provide any meaningful information, it's there only to introduce uniqueness for each entry. All
+        properties that make a key are also available in the value of a dictionary element.
 
-        ```yaml
+        ```python showLineNumbers title="Sample output"
         {
             private_0.0.0.0/0_private/i3': {
                 'age': None,
                 'destination': '0.0.0.0/0',
                 'flags': 'A S',
                 'interface': 'private/i3',
                 'metric': '10',
@@ -527,17 +521,18 @@
         The actual API command is `<show><arp><entry name = 'all'/></arp></show>`.
 
         In the returned `dict` the key is made of two properties delimited with an underscore (`_`) in the following order:
 
         * interface name,
         * IP address.
 
-        The key does not provide any meaningful information, it's there only to introduce uniqueness for each entry. All properties that make a key are also available in the value of a dictionary element. Sample output:
+        The key does not provide any meaningful information, it's there only to introduce uniqueness for each entry. All
+        properties that make a key are also available in the value of a dictionary element.
 
-        ```yaml
+        ```python showLineNumbers title="Sample output"
         {
             'ethernet1/1_10.0.2.1': {
                 'interface': 'ethernet1/1',
                 'ip': '10.0.2.1',
                 'mac': '12:34:56:78:9a:bc',
                 'port': 'ethernet1/1',
                 'status': 'c',
@@ -556,34 +551,32 @@
 
         # Returns
 
         dict: ARP table entries.
 
         """
         result = {}
-        response = self.op_parser(
-            cmd="<show><arp><entry name = 'all'/></arp></show>", cmd_in_xml=True
-        )
+        response = self.op_parser(cmd="<show><arp><entry name = 'all'/></arp></show>", cmd_in_xml=True)
 
         if response.get("entries", {}):
             arp_table = response["entries"].get("entry", [])
             for entry in arp_table if isinstance(arp_table, list) else [arp_table]:
                 result[f'{entry["interface"]}_{entry["ip"]}'] = dict(entry)
         return result
 
     def get_sessions(self) -> list:
         """Get information about currently running sessions.
 
         The actual API command run is `show session all`.
 
         # Returns
 
-        list: Information about the current sessions. Sample output:
+        list: Information about the current sessions.
 
-        ```yaml
+        ```python showLineNumbers title="Sample output"
         [
             {
                 'application': 'undecided',
                 'decrypt-mirror': 'False',
                 'dport': '80',
                 'dst': '10.0.2.11',
                 'dstnat': 'False',
@@ -624,24 +617,26 @@
         return result
 
     def get_session_stats(self) -> dict:
         """Get basic session statistics.
 
         The actual API command is `show session info`.
 
-        **NOTE**
-        This is raw output. Names of stats are the same as returned by API. No translation is made on purpose. The output of this command might vary depending on the version of PanOS.
+        :::note
+        This is raw output. Names of stats are the same as returned by API. No translation is made on purpose. The output of this
+        command might vary depending on the version of PanOS.
+        :::
 
         For meaning and available statistics, refer to the official PanOS documentation.
 
         # Returns
 
-        dict: Session stats in a form of a dictionary. Sample output:
+        dict: Session stats in a form of a dictionary.
 
-        ```yaml
+        ```python showLineNumbers title="Sample output"
         {
             'age-accel-thresh': '80',
             'age-accel-tsf': '2',
             'age-scan-ssf': '8',
             'age-scan-thresh': '80',
             'age-scan-tmo': '10',
             'cps': '0',
@@ -702,15 +697,15 @@
 
         The actual API command run is `show running tunnel flow all`.
 
         # Returns
 
         dict: Information about the configured tunnels. Sample output (with only one IPSec tunnel configured):
 
-        ```yaml
+        ```python showLineNumbers
         {
             'GlobalProtect-Gateway': {},
             'GlobalProtect-site-to-site': {},
             'IPSec': {
                 'ipsec_tunnel': {
                     'gwid': '1',
                     'id': '1',
@@ -733,76 +728,65 @@
         response = self.op_parser(cmd="show running tunnel flow all")
         result = {}
         for tunnelType, tunnelData in dict(response).items():
             if tunnelData is None:
                 result[tunnelType] = dict()
             elif not isinstance(tunnelData, str):
                 result[tunnelType] = dict()
-                for tunnel in (
-                    tunnelData["entry"]
-                    if isinstance(tunnelData["entry"], list)
-                    else [tunnelData["entry"]]
-                ):
+                for tunnel in tunnelData["entry"] if isinstance(tunnelData["entry"], list) else [tunnelData["entry"]]:
                     result[tunnelType][tunnel["name"]] = dict(tunnel)
         return result
 
     def get_latest_available_content_version(self) -> str:
         """Get the latest, downloadable content version.
 
         The actual API command run is `request content upgrade check`.
 
-        Values returned by API are not ordered. This method tries to reorder them and find the highest available Content DB version. The following assumptions are made:
+        Values returned by API are not ordered. This method tries to reorder them and find the highest available Content DB
+        version. The following assumptions are made:
 
         * versions are always increasing,
         * both components of the version string are numbers.
 
         # Raises
 
         ContentDBVersionsFormatException: An exception is thrown when the Content DB version does not match the expected format.
 
         # Returns
 
-        str: The latest available content version. Sample output:
+        str: The latest available content version.
 
-        ```python
+        ```python showLineNumbers title="Sample output"
         '8670-7824'
         ```
 
         """
         response = self.op_parser(cmd="request content upgrade check", return_xml=False)
         try:
-            content_versions = [
-                entry["version"] for entry in response["content-updates"]["entry"]
-            ]
+            content_versions = [entry["version"] for entry in response["content-updates"]["entry"]]
             majors = [int(ver.split("-")[0]) for ver in content_versions]
             majors.sort()
-            major_minors = [
-                int(ver.split("-")[1])
-                for ver in content_versions
-                if ver.startswith(f"{majors[-1]}-")
-            ]
+            major_minors = [int(ver.split("-")[1]) for ver in content_versions if ver.startswith(f"{majors[-1]}-")]
             major_minors.sort()
             latest = f"{majors[-1]}-{major_minors[-1]}"
         except Exception as exc:
-            raise ContentDBVersionsFormatException(
-                "Cannot parse list of available updates for Content DB."
-            ) from exc
+            raise exceptions.ContentDBVersionsFormatException("Cannot parse list of available updates for Content DB.") from exc
 
         return latest
 
     def get_content_db_version(self) -> str:
         """Get the currently installed Content DB version.
 
         The actual API command is `show system info`.
 
         # Returns
 
-        str: Current Content DB version. Sample output:
+        str: Current Content DB version.
 
-        ```python
+        ```python showLineNumbers title="Sample output"
         '8670-7824'
         ```
 
         """
         response = self.op_parser(cmd="show system info", return_xml=True)
         return response.findtext("./system/app-version")
 
@@ -811,23 +795,23 @@
 
         The actual API command is `show ntp`.
 
         The actual return value of this method can differ depending on whether the NTP servers are configured or not:
 
         - no NTP servers configured:
 
-            ```yaml
+            ```python showLineNumbers
             {
                 'synched': 'LOCAL'
             }
             ```
 
         - NTP servers configured:
 
-            ```yaml
+            ```python showLineNumbers
             {
                 'ntp-server-1': {
                     'authentication-type': 'none',
                     'name': '0.pool.ntp.org',
                     'reachable': 'yes',
                     'status': 'available'
                 },
@@ -841,28 +825,31 @@
             }
             ```
 
         # Returns
 
         dict: The NTP synchronization configuration.
 
-
         """
         return dict(self.op_parser(cmd="show ntp"))
 
     def get_disk_utilization(self) -> dict:
         """Get the disk utilization (in MB) and parse it to a machine readable format.
 
         The actual API command is `show system disk-space`.
 
+        # Raises
+
+        WrongDiskSizeFormatException: Raised when free text disk allocation information cannot be parsed.
+
         # Returns
 
-        dict: Disk free space in MBytes. Sample output:
+        dict: Disk free space in MBytes.
 
-        ```yaml
+        ```python showLineNumbers title="Sample output"
         {
             '/': 2867
             '/dev': 7065
             '/opt/pancfg': 14336
             '/opt/panrepo': 3276
             '/dev/shm': 1433
             '/cgroup': 7065
@@ -896,30 +883,36 @@
                 elif free_size_name == "K":
                     free_size = free_size_number / 1024
 
             elif isinstance(free_size_name, int):
                 free_size = free_size_short / 1024 / 1024
 
             else:
-                raise WrongDiskSizeFormatException("Free disk size has wrong format.")
+                raise exceptions.WrongDiskSizeFormatException("Free disk size has wrong format.")
 
             result[mount_point] = floor(free_size)
 
         return result
 
     def get_available_image_data(self) -> dict:
         """Get information on the available to download PanOS image versions.
 
         The actual API command is `request system software check`.
 
+        # Raises
+
+        UpdateServerConnectivityException: Raised when the update server is not reachable, can also mean that the device is not
+            licensed.
+        PanXapiError: Re-raised when an exception is caught but does not match `UpdateServerConnectivityException`.
+
         # Returns
 
-        dict: Detailed information on available images. Sample output:
+        dict: Detailed information on available images.
 
-        ```yaml
+        ```python showLineNumbers title="Sample output"
         {
             '11.0.1': {
                 'version': '11.0.1'
                 'filename': 'PanOS_vm-11.0.1'
                 'size': '492'
                 'size-kb': '504796'
                 'released-on': '2023/03/29 15:05:25'
@@ -944,44 +937,51 @@
             ...
         }
         ```
 
         """
         result = dict()
 
-        image_data = self.op_parser(cmd="request system software check")
+        try:
+            image_data = self.op_parser(cmd="request system software check")
+        except PanXapiError as exp:
+            if str(exp) == "Failed to check upgrade info due to Unknown error. Please check network connectivity and try again.":
+                raise exceptions.UpdateServerConnectivityException(str(exp)) from exp
+            else:
+                raise exceptions.exp
+
         images = dict(image_data["sw-updates"]["versions"])["entry"]
         for image in images if isinstance(images, list) else [images]:
             result[image["version"]] = dict(image)
 
         return result
 
     def get_mp_clock(self) -> dict:
         """Get the clock information from management plane.
 
         The actual API command is `show clock`.
 
         # Returns
 
-        dict: The clock information represented as a dictionary. Sample output:
+        dict: The clock information represented as a dictionary.
 
-        ```yaml
+        ```python showLineNumbers title="Sample output"
         {
             'time': '00:41:36',
             'tz': 'PDT',
             'day': '19',
             'month': 'Apr',
             'year': '2023',
             'day_of_week': 'Wed'
         }
         ```
 
         """
         time_string = self.op_parser(cmd="show clock")
-        time_dict = time_string.split(" ")
+        time_dict = time_string.split()
         result = {
             "time": time_dict[3],
             "tz": time_dict[4],
             "day": time_dict[2],
             "month": time_dict[1],
             "year": time_dict[5],
             "day_of_week": time_dict[0],
@@ -992,31 +992,31 @@
     def get_dp_clock(self) -> dict:
         """Get the clock information from data plane.
 
         The actual API command is `show clock more`.
 
         # Returns
 
-        dict: The clock information represented as a dictionary. Sample output:
+        dict: The clock information represented as a dictionary.
 
-        ```yaml
+        ```python showLineNumbers title="Sample output"
         {
             'time': '00:41:36',
             'tz': 'PDT',
             'day': '19',
             'month': 'Apr',
             'year': '2023',
             'day_of_week': 'Wed'
         }
         ```
 
         """
         response = self.op_parser(cmd="show clock more")
         time_string = dict(response)["member"]
-        time_dict = time_string.split(" ")
+        time_dict = time_string.split()
         result = {
             "time": time_dict[5],
             "tz": time_dict[6],
             "day": time_dict[4],
             "month": time_dict[3],
             "year": time_dict[7],
             "day_of_week": time_dict[2],
```

### Comparing `panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/snapshot_compare.py` & `panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/snapshot_compare.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,45 @@
 from typing import Optional, Union, List, Dict
 from panos_upgrade_assurance.utils import ConfigParser, SnapType
-
-
-class MissingKeyException(Exception):
-    """Used when an exception about the missing keys in a dictionary is thrown."""
-
-    pass
-
-
-class WrongDataTypeException(Exception):
-    """Used when a variable does not meet the data type requirements."""
-
-    pass
-
-
-class SnapshotSchemeMismatchException(Exception):
-    """Used when a snapshot element contains different properties in both snapshots."""
-
-    pass
+from panos_upgrade_assurance import exceptions
 
 
 class SnapshotCompare:
     """Class comparing snapshots of Firewall Nodes.
 
-    This object can be used to compare two Firewall snapshots made with the [CheckFirewall.run_snapshots()](/panos/docs/panos-upgrade-assurance/api/check_firewall#checkfirewallrun_snapshots) method and present results of this comparison.
-    Its main purpose is to compare two snapshots made with the [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) class. However, the code is generic enough to compare any two dictionaries as long as they follow the schema below:
+    This object can be used to compare two Firewall snapshots made with the
+    [`CheckFirewall.run_snapshots()`](/panos/docs/panos-upgrade-assurance/api/check_firewall#checkfirewallrun_snapshots)
+    method and present results of this comparison. Its main purpose is to compare two snapshots made with the
+    [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) class. However, the code is
+    generic enough to compare any two dictionaries as long as they follow the schema below:
 
-    ```yaml
+    ```python showLineNumbers
     {
         'root_key': {
             'key': value
         }
     }
     ```
 
     Where:
 
-    * `root_key` has to be present and mapped to a method in the `self._functions_mapping` variable in order to be recognized during a comparison.
+    * `root_key` has to be present and mapped to a method in the `self._functions_mapping` variable in order to be recognized
+    during a comparison.
     * `value` can be either of a simple type (`str`, `int`, `float`, `bool`) or a nested `dict`.
 
     # Attributes
 
     _functions_mapping (dict): Internal variable containing the map of all valid report types mapped to the specific methods.
 
-    This mapping is used to verify the requested report and to map the report to an actual method that will eventually run. Keys in this dictionary are report names as defined in the [`SnapType`](/panos/docs/panos-upgrade-assurance/api/utils#class-snaptype) class. Essentially, these are the same values that one would specify when creating a snapshot with the [CheckFirewall.run_snapshots()](/panos/docs/panos-upgrade-assurance/api/check_firewall#checkfirewallrun_snapshots) method. Values are references to the methods that will run.
+        This mapping is used to verify the requested report and to map the report to an actual method that will eventually run.
+        Keys in this dictionary are report names as defined in the
+        [`SnapType`](/panos/docs/panos-upgrade-assurance/api/utils#class-snaptype) class. Essentially, these are the same
+        values that one would specify when creating a snapshot with the
+        [`CheckFirewall.run_snapshots()`](/panos/docs/panos-upgrade-assurance/api/check_firewall#checkfirewallrun_snapshots)
+        method. Values are references to the methods that will run.
 
     """
 
     def __init__(
         self,
         left_snapshot: Dict[str, Union[str, dict]],
         right_snapshot: Dict[str, Union[str, dict]],
@@ -55,90 +47,94 @@
         """SnapshotCompare constructor.
 
         Initializes an object by storing both snapshots to be compared.
 
         # Parameters
 
         left_snapshot (dict): First snapshot dictionary to be compared, usually the older one, for example a pre-upgrade snapshot.
-        right_snapshot (dict): Second snapshot dictionary to be compared, usually the newer one, for example a post-upgrade snapshot.
+        right_snapshot (dict): Second snapshot dictionary to be compared, usually the newer one, for example a post-upgrade
+        snapshot.
 
         """
         self.left_snap = left_snapshot
         self.right_snap = right_snapshot
         self._functions_mapping = {
             SnapType.NICS: self.get_diff_and_threshold,
             SnapType.ROUTES: self.get_diff_and_threshold,
             SnapType.LICENSE: self.get_diff_and_threshold,
             SnapType.ARP_TABLE: self.get_diff_and_threshold,
             SnapType.CONTENT_VERSION: self.get_diff_and_threshold,
             SnapType.SESSION_STATS: self.get_count_change_percentage,
             SnapType.IPSEC_TUNNELS: self.get_diff_and_threshold,
         }
 
-    def compare_snapshots(
-        self, reports: Optional[List[Union[dict, str]]] = None
-    ) -> Dict[str, dict]:
+    def compare_snapshots(self, reports: Optional[List[Union[dict, str]]] = None) -> Dict[str, dict]:
         """A method that triggers the actual snapshot comparison.
 
-        This is a single point of entry to generate a comparison report. It takes both reports stored in the class object and compares areas specified in the `reports` parameter.
+        This is a single point of entry to generate a comparison report. It takes both reports stored in the class object and
+        compares areas specified in the `reports` parameter.
 
-        # Parameters
+        Refer to the [documentation on reporting](/panos/docs/panos-upgrade-assurance/configuration-details#reports) for
+        details on the currently available snapshot areas and optional parameters that can be configured for them.
 
-        reports (list, optional): A list of reports - snapshot state areas with optional configuration. This parameter follows the  [`dialect`](/panos/docs/panos-upgrade-assurance/dialect) of [`ConfigParser`](/panos/docs/panos-upgrade-assurance/api/utils#class-configparser) class.
+        # Parameters
 
-            The reports list is essentially the list of keys present in the snapshots. These keys, however, are the state areas specified when the snapshot is made with the [`CheckFirewall.run_snapshots()`](/panos/docs/panos-upgrade-assurance/api/check_firewall#checkfirewallrun_snapshots) method. This means that the reports list is basically the list of state areas. The only difference is that for reports, it is possible to specify an additional configuration. This means that the list can be specified in two ways, as `str` or `dict` (in the same manner as for [`CheckFirewall.run_readiness_checks()`](/panos/docs/panos-upgrade-assurance/api/check_firewall#checkfirewallrun_readiness_checks)).
+        reports (list, optional): A list of reports - snapshot state areas with optional configuration.
+            This parameter follows the [`dialect`](/panos/docs/panos-upgrade-assurance/dialect) of
+            [`ConfigParser`](/panos/docs/panos-upgrade-assurance/api/utils#class-configparser) class.
+
+            The reports list is essentially the list of keys present in the snapshots. These keys, however, are the state areas
+            specified when the snapshot is made with the
+            [`CheckFirewall.run_snapshots()`](/panos/docs/panos-upgrade-assurance/api/check_firewall#checkfirewallrun_snapshots)
+            method. This means that the reports list is basically the list of state areas. The only difference is that for
+            reports, it is possible to specify an additional configuration. This means that the list can be specified in two
+            ways, as `str` or `dict` (in the same manner as for
+            [`CheckFirewall.run_readiness_checks()`](/panos/docs/panos-upgrade-assurance/api/check_firewall#checkfirewallrun_readiness_checks)).
 
             For the elements specified as
 
             * `str` - the element value is the name of the report (state area),
-            * `dict` - the element contains the report name (state area) and the key value and report configuration as the element value.
-
-            Refer to the [documentation on reporting](/panos/docs/panos-upgrade-assurance/configuration-details#reports) for details on the currently available snapshot areas and optional parameters that can be configured for them.
+            * `dict` - the element contains the report name (state area) and the key value and report configuration as the
+                element value.
 
         # Raises
 
         WrongDataTypeException: An exception is raised when the configuration in a data type is different than `str` or `dict`.
 
         # Returns
 
-        dict: Result of comparison in a form of the Python dictionary. Keys in this dictionary are again state areas where values depend on the actual comparison method that was run.
+        dict: Result of comparison in a form of the Python dictionary. Keys in this dictionary are again state areas where values
+            depend on the actual comparison method that was run.
 
         """
 
         result = {}
-        reports = ConfigParser(
-            valid_elements=set(self._functions_mapping.keys()), requested_config=reports
-        ).prepare_config()
+        reports = ConfigParser(valid_elements=set(self._functions_mapping.keys()), requested_config=reports).prepare_config()
 
         for report in reports:
             if isinstance(report, dict):
                 report_type, report_config = list(report.items())[0]
                 report_config.update({"report_type": report_type})
             elif isinstance(report, str):
                 report_type = report
                 report_config = {"report_type": report_type}
             else:
-                raise WrongDataTypeException(
-                    f"Wrong configuration format for report: {report}."
-                )
+                raise exceptions.WrongDataTypeException(f"Wrong configuration format for report: {report}.")
 
             self.key_checker(self.left_snap, self.right_snap, report_type)
-            result.update(
-                {report_type: self._functions_mapping[report_type](**report_config)}
-            )
+            result.update({report_type: self._functions_mapping[report_type](**report_config)})
 
         return result
 
     @staticmethod
-    def key_checker(
-        left_dict: dict, right_dict: dict, key: Union[str, set, list]
-    ) -> None:
+    def key_checker(left_dict: dict, right_dict: dict, key: Union[str, set, list]) -> None:
         """The static method to check if a key or a list/set of keys is available in both dictionaries.
 
-        This method looks for a given key or list/set of keys in two dictionaries. Its main purpose is to assure that when comparing a key-value pair from two dictionaries, it actually exists in both.
+        This method looks for a given key or list/set of keys in two dictionaries. Its main purpose is to assure that when
+        comparing a key-value pair from two dictionaries, it actually exists in both.
 
         # Parameters
 
         left_dict (dict): 1st dictionary to verify.
         right_dict (dict): 2nd dictionary to verify.
         key (str, set, list): Key name or set/list of keys to check.
 
@@ -149,43 +145,41 @@
         """
 
         if isinstance(key, str):
             key_set = set([key])
         elif isinstance(key, (set, list)):
             key_set = set(key)
         else:
-            raise WrongDataTypeException(
-                f"The key variable is a {type(key)} but should be either: str, set or list"
-            )
+            raise exceptions.WrongDataTypeException(f"The key variable is a {type(key)} but should be either: str, set or list")
 
         left_snap_missing_key = False if key_set.issubset(left_dict.keys()) else True
         right_snap_missing_key = False if key_set.issubset(right_dict.keys()) else True
 
         if left_snap_missing_key and right_snap_missing_key:
-            raise MissingKeyException(
-                f"{key} (some elements if set/list) is missing in both snapshots"
-            )
+            raise exceptions.MissingKeyException(f"{key} (some elements if set/list) is missing in both snapshots")
         if left_snap_missing_key or right_snap_missing_key:
-            raise MissingKeyException(
+            raise exceptions.MissingKeyException(
                 f"{key} (some elements if set/list) is missing in {'left snapshot' if left_snap_missing_key else 'right snapshot'}"
             )
 
     @staticmethod
     def calculate_change_percentage(
         first_value: Union[str, int],
         second_value: Union[str, int],
         threshold: Union[str, float],
     ) -> Dict[str, Union[bool, float]]:
         """The static method to compare differences between values against a given threshold.
 
-        Values to be compared should be the `int` or `str` representation of `int`. This method is used when comparing a count of elements so a floating point value here is not expected. The threshold value, on the other hand, should be the `float` or `str` representation of `float`. This is a percentage value.
+        Values to be compared should be the `int` or `str` representation of `int`. This method is used when comparing a count of
+        elements so a floating point value here is not expected. The threshold value, on the other hand, should be the `float` or
+        `str` representation of `float`. This is a percentage value.
 
         The format of the returned value is the following:
 
-        ```yaml
+        ```python showLineNumbers
         {
             passed: bool,
             change_percentage: float,
             change_threshold: float
         }
         ```
 
@@ -201,58 +195,54 @@
 
         first_value (int, str): First value to compare.
         second_value (int, str): Second value to compare.
         threshold (float, str): Maximal difference between values given as percentage.
 
         # Raises
 
-        WrongDataTypeException: An exception is raised when the threshold value is not between `0` and `100` (typical percentage boundaries).
+        WrongDataTypeException: An exception is raised when the threshold value is not between `0` and `100` (typical percentage
+            boundaries).
 
         # Returns
 
         dict: A dictionary with the comparison results.
 
         """
         first_value = int(first_value)
         second_value = int(second_value)
         threshold = float(threshold)
 
-        result = dict(
-            passed=True, change_percentage=float(0), change_threshold=threshold
-        )
+        result = dict(passed=True, change_percentage=float(0), change_threshold=threshold)
 
         if not (first_value == 0 and second_value == 0):
             if threshold < 0 or threshold > 100:
-                raise WrongDataTypeException(
-                    "The threshold should be a percentage value between 0 and 100."
-                )
+                raise exceptions.WrongDataTypeException("The threshold should be a percentage value between 0 and 100.")
 
             result["change_percentage"] = round(
-                (
-                    abs(first_value - second_value)
-                    / (first_value if first_value >= second_value else second_value)
-                )
-                * 100,
+                (abs(first_value - second_value) / (first_value if first_value >= second_value else second_value)) * 100,
                 2,
             )
             if result["change_percentage"] > threshold:
                 result["passed"] = False
         return result
 
     @staticmethod
     def calculate_diff_on_dicts(
         left_side_to_compare: Dict[str, Union[str, dict]],
         right_side_to_compare: Dict[str, Union[str, dict]],
         properties: Optional[List[str]] = None,
     ) -> Dict[str, dict]:
         """The static method to calculate a difference between two dictionaries.
 
-        By default dictionaries are compared by going down all nested levels, to the point where key-value pairs are just strings or numbers. It is possible to configure which keys from these pairs should be compared (by default we compare all available keys). This is done using the `properties` parameter. It's a list of the bottom most level keys. For example, when comparing route tables snapshots are formatted like:
+        By default dictionaries are compared by going down all nested levels, to the point where key-value pairs are just strings
+        or numbers. It is possible to configure which keys from these pairs should be compared (by default we compare all
+        available keys). This is done using the `properties` parameter. It's a list of the bottom most level keys. For example,
+        when comparing route tables snapshots are formatted like:
 
-        ```yaml
+        ```python showLineNumbers
         {
             "routes": {
                 "default_0.0.0.0/0_ethernet1/3": {
                     "virtual-router": "default",
                     "destination": "0.0.0.0/0",
                     "nexthop": "10.26.129.129",
                     "metric": "10",
@@ -262,31 +252,49 @@
                     "route-table": "unicast"
                 },
                 ...
             }
         }
         ```
 
-        The bottom most level keys are: `virtual-router`, `destination`, `nexthop`, `metric`, `flags`, `age`, `interface`, `route-table`. This list follows [`ConfigParser`](/panos/docs/panos-upgrade-assurance/api/utils#class-configparser) [`dialect`](/panos/docs/panos-upgrade-assurance/dialect).
+        The bottom most level keys are:
+
+        - `virtual-router`,
+        - `destination`,
+        - `nexthop`,
+        - `metric`,
+        - `flags`,
+        - `age`,
+        - `interface`,
+        - `route-table`.
+
+        This list follows [`ConfigParser`](/panos/docs/panos-upgrade-assurance/api/utils#class-configparser)
+        [`dialect`](/panos/docs/panos-upgrade-assurance/dialect).
 
         The difference between dictionaries is calculated from three perspectives:
 
-        1. are there any keys missing in the 2nd (right) dictionary that are present in the 1st (left) - this is represented under the `missing` key in the results.
-        2. are there any keys in the 2nd (right) dictionary that are not present in the 1st (left) - this is represented under the `added` key in the results.
-        3. for the keys that are present in both dictionaries, are values for these keys the same or different - this is represented under the `changed` key in the results.
-
-        This is a **recursive** method. When calculating changed values, if a value for the key is `dict`, we run the method again on that dictionary - we go down one level in the nested structure. We do that to a point where the value is of the `str` type.
-        Therefore, when the final comparison results are presented, the `changed` key usually contains a nested results structure. This means it contains a dictionary with the `missing`, `added`, and `changed` keys.
-        Each comparison perspective contains the `passed` property that immediately informs if this comparison gave any results (`False`) or not (`True`).
+        1. are there any keys missing in the 2nd (right) dictionary that are present in the 1st (left) - this is represented
+        under the `missing` key in the results.
+        2. are there any keys in the 2nd (right) dictionary that are not present in the 1st (left) - this is represented under
+        the `added` key in the results.
+        3. for the keys that are present in both dictionaries, are values for these keys the same or different - this is
+        represented under the `changed` key in the results.
+
+        This is a **recursive** method. When calculating changed values, if a value for the key is `dict`, we run the method
+        again on that dictionary - we go down one level in the nested structure. We do that to a point where the value is of the
+        `str` type. Therefore, when the final comparison results are presented, the `changed` key usually contains a nested
+        results structure. This means it contains a dictionary with the `missing`, `added`, and `changed` keys.
+        Each comparison perspective contains the `passed` property that immediately informs if this comparison gave any results
+        (`False`) or not (`True`).
 
-        **Example.**
+        **Example**
 
         Let's assume we want to compare two dictionaries of the following structure:
 
-        ```python
+        ```python showLineNumbers
         left_dict = {
             'root_key1'= {
                 'key'= 'value'
             }
             'root_key2'= {
                 'key'= 'value'
             }
@@ -297,15 +305,15 @@
                 'key'= 'other_value'
             }
         }
         ```
 
         The result of this comparison would look like this:
 
-        ```json
+        ```python showLineNumbers
         {
             "missing": {
                 "passed": false,
                 "missing_keys": [
                     "root_key1"
                 ]
             },
@@ -338,27 +346,30 @@
                 }
             }
         }
         ```
 
         # Parameters
 
-        left_side_to_compare (dict): 1st dictionary to compare. When this method is triggered by [`compare_snapshots()`](#snapshotcomparecompare_snapshots), the dictionary comes from the `self.left_snap` snapshot.
-        right_side_to_compare (dict): 2nd dictionary to compare, comes from the self.right_snap snapshot. When this method is triggered by [`compare_snapshots()`](#snapshotcomparecompare_snapshots), the dictionary comes from the `self.right_snap` snapshot.
+        left_side_to_compare (dict): 1st dictionary to compare. When this method is triggered by
+            [`compare_snapshots()`](#snapshotcomparecompare_snapshots), the dictionary comes from the `self.left_snap` snapshot.
+        right_side_to_compare (dict): 2nd dictionary to compare, comes from the self.right_snap snapshot. When this method is
+            triggered by [`compare_snapshots()`](#snapshotcomparecompare_snapshots), the dictionary comes from the
+            `self.right_snap` snapshot.
         properties (list(str), optional): The list of properties used to compare two dictionaries.
 
         # Raises
 
         WrongDataTypeException: Thrown when one of the `properties` elements has a wrong data type.
 
         # Returns
 
         dict: Summary of the differences between dictionaries. The output has the following format:
 
-        ```yaml
+        ```python showLineNumbers title="Sample output"
         {
             'missing': {
                 'passed': True,
                 'missing_keys': []
             },
             'added': {
                 'passed': True,
@@ -391,23 +402,17 @@
         added = right_side_to_compare.keys() - left_side_to_compare.keys()
         if added:
             result["added"]["passed"] = False
             for key in added:
                 result["added"]["added_keys"].append(key)
 
         common_keys = left_side_to_compare.keys() & right_side_to_compare.keys()
-        at_lowest_level = (
-            True
-            if isinstance(right_side_to_compare[list(common_keys)[0]], str)
-            else False
-        )
+        at_lowest_level = True if isinstance(right_side_to_compare[list(common_keys)[0]], str) else False
         keys_to_check = (
-            ConfigParser(
-                valid_elements=set(common_keys), requested_config=properties
-            ).prepare_config()
+            ConfigParser(valid_elements=set(common_keys), requested_config=properties).prepare_config()
             if at_lowest_level
             else common_keys
         )
 
         item_changed = False
         for key in keys_to_check:
             if right_side_to_compare[key] != left_side_to_compare[key]:
@@ -425,30 +430,33 @@
                     )
 
                     SnapshotCompare.calculate_passed(nested_results)
                     if not nested_results["passed"]:
                         result["changed"]["changed_raw"][key] = nested_results
                         item_changed = True
                 else:
-                    raise WrongDataTypeException(f"Unknown value format for key {key}.")
+                    raise exceptions.WrongDataTypeException(f"Unknown value format for key {key}.")
             result["changed"]["passed"] = not item_changed
 
         return result
 
     @staticmethod
     def calculate_passed(result: Dict[str, Union[dict, str]]) -> None:
         """The static method to calculate the upper level `passed` value.
 
-        When two snapshots are compared, a dictionary that is the result of this comparison is structured as in the following [`get_diff_and_threshold()`](#snapshotcompareget_diff_and_threshold) method: each root key contains a dictionary that has a structure returned by the [`calculate_diff_on_dicts()`](#snapshotcomparecalculate_diff_on_dicts) method.
+        When two snapshots are compared, a dictionary that is the result of this comparison is structured as in the following
+        [`get_diff_and_threshold()`](#snapshotcompareget_diff_and_threshold) method: each root key contains a dictionary that has
+        a structure returned by the [`calculate_diff_on_dicts()`](#snapshotcomparecalculate_diff_on_dicts) method.
 
-        This method takes a dictionary under the root key and calculates the `passed` flag based on the all `passed` flags in that dictionary. This provides a quick way of finding out if any comparison made on data under a root key failed or not.
+        This method takes a dictionary under the root key and calculates the `passed` flag based on the all `passed` flags in
+        that dictionary. This provides a quick way of finding out if any comparison made on data under a root key failed or not.
 
-        To illustrate that, the `passed` flag added by this method is marked with an arrow:
+        To illustrate that, the `passed` flag added by this method is highlighted:
 
-        ```yaml
+        ```python showLineNumbers title="Example"
         {
             'added': {
                 'added_keys': [],
                 'passed': True
             },
             'changed': {
                 'changed_raw': {},
@@ -456,19 +464,22 @@
             },
             'missing': {
                 'missing_keys': [
                     'default_0.0.0.0/0_ethernet1/3'
                 ],
                 'passed': False
             },
-            'passed': False   <-------###
+            # highlight-next-line
+            'passed': False
         }
         ```
 
-        **NOTE** that this method operated on the passed dictionary directly.
+        :::caution
+        This method operates on the passed dictionary directly.
+        :::
 
         # Parameters
 
         result (dict): A dictionary for which the `passed` property should be calculated.
 
         """
         passed = True
@@ -482,25 +493,31 @@
         report_type: str,
         properties: Optional[List[str]] = None,
         count_change_threshold: Optional[Union[int, float]] = None,
     ) -> Optional[Dict[str, Optional[Union[bool, dict]]]]:
         """The generic snapshot comparison method.
 
         The generic method to compare two snapshots of a given type. It is meant to fit most of the comparison cases.
-        It is capable of calculating both - a difference between two snapshots and the change count in the elements against a given threshold. The 1<sup>st</sup> calculation is done by the [`calculate_diff_on_dicts()`](#snapshotcomparecalculate_diff_on_dicts) method, the 2<sup>nd</sup> - internally.
-
-        The changed elements count does not compare the count of elements in each snapshot. This value represents the number of actual changes, so elements added, missing and changed. This is compared against the number of elements in the left snapshot as this one is usually the 1st one taken and it's treated as a source of truth.
+        It is capable of calculating both - a difference between two snapshots and the change count in the elements against a
+        given threshold. The 1<sup>st</sup> calculation is done by the
+        [`calculate_diff_on_dicts()`](#snapshotcomparecalculate_diff_on_dicts) method, the 2<sup>nd</sup> - internally.
+
+        The changed elements count does not compare the count of elements in each snapshot. This value represents the number of
+        actual changes, so elements added, missing and changed. This is compared against the number of elements in the left
+        snapshot as this one is usually the 1st one taken and it's treated as a source of truth.
 
-        The changed elements count is presented as a percentage. In scenarios where the right snapshot has more elements then the left one, it can give values greater than 100%.
+        The changed elements count is presented as a percentage. In scenarios where the right snapshot has more elements then the
+        left one, it can give values greater than 100%.
 
-        This method produces a complex set of nested dictionaries. Each level contains the `passed` flag indicating if the comparison of a particular type or for a particular level failed or not, and the actual comparison results.
+        This method produces a complex set of nested dictionaries. Each level contains the `passed` flag indicating if the
+        comparison of a particular type or for a particular level failed or not, and the actual comparison results.
 
         An example for the route tables, crafted in a way that almost each level fails:
 
-        ```json
+        ```json showLineNumbers title="Example"
         {
             "added": {
                 "added_keys": [
                     "default_10.26.129.0/25_ethernet1/2",
                     "default_168.63.129.16/32_ethernet1/3"
                 ],
                 "passed": "False"
@@ -508,14 +525,15 @@
             "missing": {
                 "missing_keys": [
                     "default_0.0.0.0/0_ethernet1/3"
                 ],
                 "passed": "False"
             },
             "changed": {
+                # highlight-start
                 "changed_raw": {
                     "default_10.26.130.0/25_ethernet1/2": {
                         "added": {
                             "added_keys": [],
                             "passed": "True"
                         },
                         "missing": {
@@ -530,34 +548,39 @@
                                 }
                             },
                             "passed": "False"
                         },
                         "passed": "False"
                     }
                 },
+                # highlight-end
                 "passed": "False"
             },
             "count_change_percentage": {
                 "change_percentage": 33.33,
                 "change_threshold": 1,
                 "passed": "False"
             },
             "passed": "False"
         }
         ```
 
-        In the example above, you can also see a nested dictionary produced by the [`calculate_diff_on_dicts()`](#snapshotcomparecalculate_diff_on_dicts) method under `changed.changed_raw`.
+        In the example above, you can also see a nested dictionary produced by the
+        [`calculate_diff_on_dicts()`](#snapshotcomparecalculate_diff_on_dicts) method under `changed.changed_raw`.
 
         # Parameters
 
-        report_type (str): Name of report (type) that has to be compared. Basically this is a snapshot state area, for example `nics`, `routes`, etc.
-
-        properties (list(str), optional): (defaults to `None`) An optional list of properties to include or exclude when comparing snapshots. This parameter is passed directly to the [`calculate_diff_on_dicts()`](#snapshotcomparecalculate_diff_on_dicts) method. For details on this method parameters, see the [documentation](#snapshotcomparecalculate_diff_on_dicts) for this method.
-
-        count_change_threshold (int, float, optional): (defaults to `None`) The maximum difference between number of changed elements in each snapshot (as percentage).
+        report_type (str): Name of report (type) that has to be compared. Basically this is a snapshot state area, for example
+            `nics`, `routes`, etc.
+        properties (list(str), optional): (defaults to `None`) An optional list of properties to include or exclude when
+            comparing snapshots. This parameter is passed directly to the
+            [`calculate_diff_on_dicts()`](#snapshotcomparecalculate_diff_on_dicts) method. For details on this method parameters,
+            see the [documentation](#snapshotcomparecalculate_diff_on_dicts) for this method.
+        count_change_threshold (int, float, optional): (defaults to `None`) The maximum difference between number of changed
+            elements in each snapshot (as percentage).
 
         # Returns
 
         dict: Comparison results.
 
         """
         result = {}
@@ -567,28 +590,22 @@
             right_side_to_compare=self.right_snap[report_type],
             properties=properties,
         )
         result.update(diff)
 
         if count_change_threshold and result:
             if count_change_threshold < 0 or count_change_threshold > 100:
-                raise WrongDataTypeException(
-                    "The threshold should be a percentage value between 0 and 100."
-                )
+                raise exceptions.WrongDataTypeException("The threshold should be a percentage value between 0 and 100.")
 
             added_count = len(result["added"]["added_keys"])
             missing_count = len(result["missing"]["missing_keys"])
             changed_count = len(result["changed"]["changed_raw"])
             left_total_count = len(self.left_snap[report_type].keys())
 
-            diff = (
-                1
-                if left_total_count == 0
-                else (added_count + missing_count + changed_count) / left_total_count
-            )
+            diff = 1 if left_total_count == 0 else (added_count + missing_count + changed_count) / left_total_count
             diff_percentage = round(float(diff) * 100, 2)
 
             passed = diff_percentage <= count_change_threshold
 
             result.update(
                 {
                     "count_change_percentage": dict(
@@ -609,18 +626,20 @@
     def get_count_change_percentage(
         self,
         report_type: str,
         thresholds: Optional[List[Dict[str, Union[int, float]]]] = None,
     ) -> Optional[Dict[str, Union[bool, dict]]]:
         """Generic method to calculate the change on values and compare them against a given threshold.
 
-        In opposition to the [`get_diff_and_threshold()`](#snapshotcompareget_diff_and_threshold) method, this one does not calculate the count change but the actual difference between the numerical values.
-        A good example is a change in the session count. The snapshot for this area is a dictionary with the keys taking values of different session types and values containing the actual session count:
+        In opposition to the [`get_diff_and_threshold()`](#snapshotcompareget_diff_and_threshold) method, this one does not
+        calculate the count change but the actual difference between the numerical values.
+        A good example is a change in the session count. The snapshot for this area is a dictionary with the keys taking values
+        of different session types and values containing the actual session count:
 
-        ```yaml
+        ```python showLineNumbers title="Example"
         {
             "session_stats": {
                 "tmo-5gcdelete": "15",
                 "tmo-sctpshutdown": "60",
                 "tmo-tcp": "3600",
                 "tmo-tcpinit": "5",
                 "pps": "2",
@@ -642,32 +661,35 @@
 
         - sweeps through all the session types provided in the `thresholds` variable,
         - calculates the actual difference,
         - compares the actual difference with the threshold value (percentage) for a particular session type.
 
         It takes as parameter a list of dictionaries describing elements to compare, in a form of:
 
-        ```json
+        ```json showLineNumbers
         {
             "element_type": threshold_value
         }
         ```
 
         Where:
 
         - `element_type` is a key which value we are going to compare,
-        - `threshold_value` is a percentage value provided as either `int` or `float`. If the list is empty, the method will return `None`.
+        - `threshold_value` is a percentage value provided as either `int` or `float`. If the list is empty,
+            the method will return `None`.
 
         :::caution
-        This list **does not support** [`ConfigParser`](/panos/docs/panos-upgrade-assurance/api/utils#class-configparser) [`dialect`](/panos/docs/panos-upgrade-assurance/dialect).
+        This list **does not support** [`ConfigParser`](/panos/docs/panos-upgrade-assurance/api/utils#class-configparser)
+        [`dialect`](/panos/docs/panos-upgrade-assurance/dialect).
         :::
 
-        Below there is a sample list for the `sessions_stat` dictionary shown above that would calculate differences for the TCP and UDP sessions:
+        Below there is a sample list for the `sessions_stat` dictionary shown above that would calculate differences for the TCP
+        and UDP sessions:
 
-        ```json
+        ```json showLineNumbers
         [
             { "num-tcp": 1.5 },
             { "num-udp": 15 },
         ]
         ```
 
         # Parameters
@@ -676,17 +698,19 @@
 
         # Raises
 
         SnapshotSchemeMismatchException: Thrown when a snapshot element has a different set of properties in both snapshots.
 
         # Returns
 
-        dict: The result of difference compared against a threshold. The result for each value is in the same form as returned by the [`calculate_change_percentage()`](#snapshotcomparecalculate_change_percentage) method. For the examples above, the return value would be:
+        dict: The result of difference compared against a threshold. The result for each value is in the same form as returned \
+            by the [`calculate_change_percentage()`](#snapshotcomparecalculate_change_percentage) method. For the examples \
+            above, the return value would be:
 
-        ```yaml
+        ```python showLineNumbers title="Sample output"
         {
             'num-tcp': {
                 'change_percentage': 99.0,
                 'change_threshold': 1.5,
                 'passed': False
             },
             'num-udp': {
@@ -710,18 +734,16 @@
         requested_elements = set(next(iter(unary_dict)) for unary_dict in thresholds)
         try:
             self.key_checker(
                 self.left_snap[report_type],
                 self.right_snap[report_type],
                 requested_elements,
             )
-        except (
-            MissingKeyException
-        ) as exc:  # raised when any requested key is missing in one of the snapshots
-            raise SnapshotSchemeMismatchException(
+        except exceptions.MissingKeyException as exc:  # raised when any requested key is missing in one of the snapshots
+            raise exceptions.SnapshotSchemeMismatchException(
                 f"Snapshots have missing keys in {requested_elements} for {report_type} report."
             ) from exc
 
         elements = ConfigParser(
             valid_elements=set(self.left_snap[report_type].keys()),
             requested_config=thresholds,
         ).prepare_config()
```

### Comparing `panos_upgrade_assurance-0.0.2/panos_upgrade_assurance/utils.py` & `panos_upgrade_assurance-0.1.0/panos_upgrade_assurance/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 from dataclasses import dataclass
 from copy import deepcopy
 from typing import Optional, Union, List, Iterable
 from enum import Enum
-
-
-class UnknownParameterException(Exception):
-    """Used when one of the requested configuration parameters processed by [`ConfigParser`](#class-configparser) is not a valid parameter."""
-
-    pass
-
-
-class WrongDataTypeException(Exception):
-    """Used when a variable does not meet data type requirements."""
-
-    pass
+from panos_upgrade_assurance import exceptions
 
 
 class CheckType:
     """Class mapping check configuration strings for commonly used variables.
 
-    Readiness checks configuration passed to the [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) class is in a form of a list of strings. These strings are compared in several places to parse the configuration and set the proper checks. This class is used to avoid hardcoding these strings. It maps the actual configuration string to a variable that can be referenced in the code.
+    Readiness checks configuration passed to the
+    [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) class is in a form of a list of
+    strings. These strings are compared in several places to parse the configuration and set the proper checks. This class is
+    used to avoid hardcoding these strings. It maps the actual configuration string to a variable that can be referenced in the
+    code.
     """
 
     PANORAMA = "panorama"
     HA = "ha"
     NTP_SYNC = "ntp_sync"
     CANDIDATE_CONFIG = "candidate_config"
     EXPIRED_LICENSES = "expired_licenses"
@@ -35,31 +28,35 @@
     FREE_DISK_SPACE = "free_disk_space"
     MP_DP_CLOCK_SYNC = "planes_clock_sync"
 
 
 class SnapType:
     """Class mapping the snapshot configuration strings to the commonly used variables.
 
-    Snapshot configuration passed to the [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) class is in a form of a list of strings. These strings are compared in several places to parse the configuration and set proper snapshots.
-    This class is used to avoid hardcoding these strings. It maps the actual configuration string to a variable that can be referenced in the code.
+    Snapshot configuration passed to the
+    [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) class is in a form of a list of
+    strings. These strings are compared in several places to parse the configuration and set proper snapshots.
+    This class is used to avoid hardcoding these strings. It maps the actual configuration string to a variable that can be
+    referenced in the code.
     """
 
     NICS = "nics"
     ROUTES = "routes"
     LICENSE = "license"
     ARP_TABLE = "arp_table"
     CONTENT_VERSION = "content_version"
     SESSION_STATS = "session_stats"
     IPSEC_TUNNELS = "ip_sec_tunnels"
 
 
 class CheckStatus(Enum):
     """Class containing possible statuses for the check results.
 
-    Its main purpose is to extend the simple `True`/`False` logic in a way that would provide more details/explanation in case a check fails. It provides the following statuses:
+    Its main purpose is to extend the simple `True`/`False` logic in a way that would provide more details/explanation in case a
+    check fails. It provides the following statuses:
 
     * `SUCCESS`
     * `FAIL`
     * `ERROR`
     * `SKIPPED`
 
     """
@@ -75,15 +72,18 @@
     """Class representing the readiness check results.
 
     It provides two types of information:
 
     * `status` which represents information about the check outcome,
     * `reason` a reason behind the particular outcome, this comes in handy when a check fails.
 
-    Most of the [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) methods use this class to store the return values, but mostly internally. The [`CheckFirewall.run_readiness_checks()`](/panos/docs/panos-upgrade-assurance/api/check_firewall#checkfirewallrun_readiness_checks) method translates this class into the python primitives: `str` and `bool`.
+    Most of the [`CheckFirewall`](/panos/docs/panos-upgrade-assurance/api/check_firewall#class-checkfirewall) methods use this
+    class to store the return values, but mostly internally. The
+    [`CheckFirewall.run_readiness_checks()`](/panos/docs/panos-upgrade-assurance/api/check_firewall#checkfirewallrun_readiness_checks)
+    method translates this class into the python primitives: `str` and `bool`.
 
     # Attributes
 
     status (CheckStatus): Holds the status of a check. See [`CheckStatus`](#class-checkstatus) class for details.
     reason (str): Holds a reason explaining why a check fails. Provides no value if the check is successful.
 
     """
@@ -92,15 +92,16 @@
     reason: str = ""
 
     def __str__(self):
         """This class' string representation.
 
         # Returns
 
-        str: a string combined from the `self.status` and `self.reason` variables. Provides a human readable representation of the class. Perfect to provide a reason for a particular check outcome.
+        str: a string combined from the `self.status` and `self.reason` variables. Provides a human readable representation of
+        the class. Perfect to provide a reason for a particular check outcome.
 
         """
         return f"[{self.status.name}] {self.reason}"
 
     def __bool__(self):
         """Class' boolean representation.
 
@@ -114,92 +115,93 @@
         """
         return True if self.status == CheckStatus.SUCCESS else False
 
 
 class ConfigParser:
     """Class responsible for parsing the provided configuration.
 
-    This class is universal, meaning it parses configuration provided as the list of strings or dictionaries and verifies it against the list of valid configuration items.
-    There are no hardcoded items against which the configuration is checked. This class is used in many places in this package and it uses a specific [`dialect`](/panos/docs/panos-upgrade-assurance/dialect).
+    This class is universal, meaning it parses configuration provided as the list of strings or dictionaries and verifies it
+    against the list of valid configuration items.
+    There are no hardcoded items against which the configuration is checked. This class is used in many places in this package
+    and it uses a specific [`dialect`](/panos/docs/panos-upgrade-assurance/dialect).
 
     # Attributes
 
-    _requested_config_names (set): Contains only element names of the requested configuration. When no requested configuration is passed (implicit `'all'`), this is equal to `self.valid_elements`.
+    _requested_config_names (set): Contains only element names of the requested configuration. When no requested configuration is
+        passed (implicit `'all'`), this is equal to `self.valid_elements`.
 
     """
 
     def __init__(
         self,
         valid_elements: Iterable,
         requested_config: Optional[List[Union[str, dict]]] = None,
     ):
         """ConfigParser constructor.
 
         Introduces some initial verification logic:
 
         * `valid_elements` is converted to `set` - this way we get rid of all duplicates,
-        * if `requested_config` is `None` we immediately treat it as if `all`  was passed implicitly (see [`dialect`](/panos/docs/panos-upgrade-assurance/dialect)) - it's expanded to `valid_elements`
-        * `_requested_config_names` is introduced as `requested_config` stripped of any element configurations. Additionally, we do verification if elements of this variable match `valid_elements`. An exception is thrown if not.
+        * if `requested_config` is `None` we immediately treat it as if `all`  was passed implicitly
+            (see [`dialect`](/panos/docs/panos-upgrade-assurance/dialect)) - it's expanded to `valid_elements`
+        * `_requested_config_names` is introduced as `requested_config` stripped of any element configurations. Additionally, we
+            do verification if elements of this variable match `valid_elements`. An exception is thrown if not.
 
         # Parameters
 
         valid_elements (iterable): Valid elements against which we check the requested config.
-        requested_config (list, optional): (defaults to `None`) A list of requested configuration items with an optional configuration.
+        requested_config (list, optional): (defaults to `None`) A list of requested configuration items with an optional
+            configuration.
 
         # Raises
 
         UnknownParameterException: An exception is raised when a requested configuration element is not one of the valid elements.
 
         """
         self.valid_elements = set(valid_elements)
 
         if requested_config:  # if not None or not empty list
             self.requested_config = deepcopy(requested_config)
             self._requested_config_names = set(
-                [
-                    ConfigParser._extract_element_name(config_keyword)
-                    for config_keyword in self.requested_config
-                ]
+                [ConfigParser._extract_element_name(config_keyword) for config_keyword in self.requested_config]
             )
             for config_name in self._requested_config_names:
                 if not self._is_element_included(element=config_name):
-                    raise UnknownParameterException(
-                        f"Unknown configuration parameter passed: {config_name}."
-                    )
+                    raise exceptions.UnknownParameterException(f"Unknown configuration parameter passed: {config_name}.")
         else:
             self._requested_config_names = set(valid_elements)
             self.requested_config = list(valid_elements)  # Meaning 'all' valid tests
 
     def _is_element_included(self, element: str) -> bool:
         """Method verifying if a config element is a correct (supported) value.
 
         This method can also handle `not-elements` (see [`dialect`](/panos/docs/panos-upgrade-assurance/dialect)).
 
         # Parameters
 
-        element (str): The config element to verify. This can be a `not-element`. This parameter is verified against `self.valid_elements` `set`. Key word `'all'` is also accepted.
+        element (str): The config element to verify. This can be a `not-element`. This parameter is verified against
+            `self.valid_elements` `set`. Key word `'all'` is also accepted.
 
         # Returns
         bool: `True` if the value is correct, `False` otherwise.
 
         """
-        if element in self.valid_elements or (
-            element.startswith("!") and element[1:] in self.valid_elements
-        ):
+        if element in self.valid_elements or (element.startswith("!") and element[1:] in self.valid_elements):
             return True
         elif element == "all" and "all" in self.requested_config:
             return True
         else:
             return False
 
     @staticmethod
     def _extract_element_name(config: Union[str, dict]) -> str:
         """Method that extracts the name from a config element.
 
-        If a config element is a string, the actual config element is returned. For elements of a dictionary type, the 1<sup>st</sup> key is returned.
+        If a config element is a string, the actual config element is returned. For elements of a dictionary type, the
+        1<sup>st</sup> key is returned.
 
         # Parameters
 
         config (str, dict): A config element to provide a name for.
 
         # Raises
 
@@ -212,54 +214,45 @@
         """
         if isinstance(config, str):
             return config
         elif isinstance(config, dict):
             if len(config) == 1:
                 return list(config.keys())[0]
             else:
-                raise WrongDataTypeException(
+                raise exceptions.WrongDataTypeException(
                     "Dict provided as config definition has incorrect format, it is supposed to have only one key {key:[]}"
                 )
         else:
-            raise WrongDataTypeException("Config definition is neither string or dict")
+            raise exceptions.WrongDataTypeException("Config definition is neither string or dict")
 
     def _expand_all(self) -> None:
         """Expand key word `'all'` to  `self.valid_elements`.
 
-        During expansion, elements from `self.valid_elements` which are already available in `self.requested_config` are skipped. This way we do not introduce duplicates for elements that were provided explicitly.
+        During expansion, elements from `self.valid_elements` which are already available in `self.requested_config` are skipped.
+        This way we do not introduce duplicates for elements that were provided explicitly.
 
         This method directly operates on `self.requested_config`.
         """
-        pure_names = set(
-            [
-                (name[1:] if name.startswith("!") else name)
-                for name in self._requested_config_names
-                if name != "all"
-            ]
-        )
+        pure_names = set([(name[1:] if name.startswith("!") else name) for name in self._requested_config_names if name != "all"])
         self.requested_config.extend(list(self.valid_elements - pure_names))
         self.requested_config.remove("all")
 
     def prepare_config(self) -> List[Union[str, dict]]:
         """Parse the input config and return a machine-usable configuration.
 
-        The parsed configuration retains element types. This means that an element of a dictionary type will remain a dictionary in the parsed config.
+        The parsed configuration retains element types. This means that an element of a dictionary type will remain a dictionary
+        in the parsed config.
 
         This method handles most of the [`dialect`](/panos/docs/panos-upgrade-assurance/dialect)'s logic.
 
         # Returns
         list: The parsed configuration.
 
         """
-        if all(
-            (
-                config_name.startswith("!")
-                for config_name in self._requested_config_names
-            )
-        ):
+        if all((config_name.startswith("!") for config_name in self._requested_config_names)):
             self.requested_config.insert(0, "all")
 
         if "all" in self.requested_config:
             self._expand_all()
 
         final_configs = []
 
@@ -283,17 +276,15 @@
 
     # Returns
 
     bool: `True` for *yes*, `False` for *no*.
 
     """
     if boolstr not in ["yes", "no"]:
-        raise WrongDataTypeException(
-            f"Cannot interpret following string as boolean: {boolstr}."
-        )
+        raise exceptions.WrongDataTypeException(f"Cannot interpret following string as boolean: {boolstr}.")
 
     return True if boolstr == "yes" else False
 
 
 def printer(report: dict, indent_level: int = 0) -> None:
     """Print reports in human friendly format.
```

### Comparing `panos_upgrade_assurance-0.0.2/pyproject.toml` & `panos_upgrade_assurance-0.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "panos-upgrade-assurance"
-version = "0.0.2"
+version = "0.1.0"
 description = ""
 authors = ["Palo Alto Networks"]
 readme = "README.md"
 packages = [
     { include = "panos_upgrade_assurance" }
 ]
 classifiers = [
@@ -24,15 +24,23 @@
 xmltodict = "^0.13"
 
 [tool.poetry.group.dev.dependencies]
 pydoc-markdown = "^4.6"
 flake8 = "^6.0"
 black = "^23.3"
 bandit = "^1.7"
+Flake8-pyproject = "^1.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["docs", ".venv", ".github", "docker_image", "dist"]
 skips = ["B405"]
+
+[tool.black]
+line-length = 130
+
+[tool.flake8]
+select = ["C","E","F","W","B","D","B950"]
+ignore = ["E203","E501","W503","D203","D102","D103","D107","D400","E501"]
```

### Comparing `panos_upgrade_assurance-0.0.2/PKG-INFO` & `panos_upgrade_assurance-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panos-upgrade-assurance
-Version: 0.0.2
+Version: 0.1.0
 Summary: 
 Author: Palo Alto Networks
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

