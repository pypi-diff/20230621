# Comparing `tmp/tcia_utils-1.5.tar.gz` & `tmp/tcia_utils-1.5.1.tar.gz`

## Comparing `tcia_utils-1.5.tar` & `tcia_utils-1.5.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.5/src/tcia_utils/__init__.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 tcia_utils-1.5/src/tcia_utils/datacite.py
--rw-r--r--   0        0        0    58523 2020-02-02 00:00:00.000000 tcia_utils-1.5/src/tcia_utils/nbia.py
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tcia_utils-1.5/src/tcia_utils/pathdb.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.5/LICENSE
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 tcia_utils-1.5/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 tcia_utils-1.5/pyproject.toml
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 tcia_utils-1.5/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/src/tcia_utils/__init__.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/src/tcia_utils/datacite.py
+-rw-r--r--   0        0        0    67874 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/src/tcia_utils/nbia.py
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/src/tcia_utils/pathdb.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/LICENSE
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/README.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 tcia_utils-1.5.1/PKG-INFO
```

### Comparing `tcia_utils-1.5/src/tcia_utils/datacite.py` & `tcia_utils-1.5.1/src/tcia_utils/datacite.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.5/src/tcia_utils/nbia.py` & `tcia_utils-1.5.1/src/tcia_utils/nbia.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,37 +21,49 @@
 
 _log = logging.getLogger(__name__)
 logging.basicConfig(
     format='%(asctime)s:%(levelname)s:%(message)s'
     , level=logging.INFO
 )
 
+# Used by functions that accept parameters used in GUI Simple Search
+# e.g. getSimpleSearchWithModalityAndBodyPartPaged()
 class Criteria(Enum):
     Collection = "CollectionCriteria"
     Species = "SpeciesCriteria"
     ImageModality = "ImageModalityCriteria"
     BodyPart = "AnatomicalSiteCriteria"
     Manufacturer = "ManufacturerCriteria"
     DateRange = "DateRangeCriteria"
     Patient = "PatientCriteria"
     NumStudies = "MinNumberOfStudiesCriteria"
     ModalityAnded = "ModalityAndedSearchCriteria"
 
+# Used by getSimpleSearchWithModalityAndBodyPartPaged() to transform
+#   species codes into human readable terms
 NPEXSpecies = {
     "human": 337915000
     , "mouse": 447612001
     , "dog": 448771007
 }
 
-####### setApiUrl()
-# Called by other functions to select base URL
-# Checks for valid security tokens where needed
 
 def setApiUrl(endpoint, api_url):
-
+    """
+    setApiUrl() is used by most other functions to select the correct base URL
+    and is generally not something that needs to be called directly in your code.  
+    
+    It assists with:
+        1. verifying you are calling a supported endpoint
+        2. selecting the correct base URL for Search vs Advanced APIs
+        3. selecting the correct base URL for regular collections vs NLST
+        4. ensuring you have a valid security token where necessary
+    
+    Learn more about the NBIA APIs at https://wiki.cancerimagingarchive.net/x/ZoATBg
+    """
     global searchEndpoints, advancedEndpoints
 
     # create valid endpoint lists
     searchEndpoints = ["getCollectionValues", "getBodyPartValues", "getModalityValues",
                         "getPatient", "getPatientStudy", "getSeries", "getManufacturerValues",
                         "getSOPInstanceUIDs", "getSeriesMetaData", "getContentsByName",
                        "getImage", "getSingleImage", "getPatientByCollectionAndModality",
@@ -130,139 +142,150 @@
                     "Remove the api_url parameter unless you are querying the National Lung Screening Trial collection.\n"
                     'Use api_url = "nlst" to query the National Lung Screening Trial collection.'
                 )
                 raise StopExecution
 
         return base_url
 
-####### getToken()
-# Retrieves security token to access APIs that require authorization
-# Provides interactive prompts for user/pw if they're not specified as parameters
-# Use getToken() for querying restricted collections with "Search API"
-# Use getToken(api_url = "nlst") for "Advanced API" queries of National Lung Screening Trial
-# Sets expiration time for tokens (2 hours from creation)
-
 def getToken(user = "", pw = "", api_url = ""): 
+    """
+    getToken() accepts user and pw parameters to create a token to access APIs that require authorization.
+    Access tokens expire 2 hours after creation, and can be refreshed with refreshToken().
+    Interactive prompts are provided for user/pw if they're not specified as parameters.
+    "Advanced APIs" can be accessed anonymously using the nbia_guest account with a blank password.
+    The api_url = "nlst" parameter is only necessary for "Advanced API" queries since it's a public collection.
+    """
+    global token_exp_time, nlst_token_exp_time, api_call_headers, nlst_api_call_headers, refresh_token, nlst_refresh_token
 
-    global token_exp_time, nlst_token_exp_time, api_call_headers, nlst_api_call_headers, refresh_token
-
-    # token URLs
+    # assumes nbia_guest account for Advanced API on NLST server (all public data)
     if api_url == "nlst":
         token_url = "https://nlst.cancerimagingarchive.net/nbia-api/oauth/token"
+        userName = "nbia_guest"
+        passWord = ""        
+    # specify user/pw unless nbia_guest is being used for accessing Advanced API anonymously
     else:
         token_url = "https://nbia.cancerimagingarchive.net/nbia-api/oauth/token"
 
-    # set user name and password
-    if user == "":
-        print("Enter User: ")
-        userName = input()
-    else:
-        userName = user
-    if pw == "" and user != "nbia_guest":
-        passWord = getpass.getpass(prompt = 'Enter Password: ')
-    else:
-        passWord = pw
+        if user == "":
+            print("Enter User: ")
+            userName = input()
+        else:
+            userName = user
+        # if user is nbia_guest, we leave password blank for anonymous access
+        if pw == "" and user != "nbia_guest":
+            passWord = getpass.getpass(prompt = 'Enter Password: ')
+        else:
+            passWord = pw
 
-    # create API token
+    # request API token
     try:
         params = {
         'client_id': 'nbiaRestAPIClient',
         'client_secret' : 'ItsBetweenUAndMe',
         'grant_type': 'password',
         'username' : userName,
         'password': passWord
         }
         
         data = requests.post(token_url, data = params)
         data.raise_for_status()
         access_token = data.json()["access_token"]
-        refresh_token = data.json()["refresh_token"]
         expires_in = data.json()["expires_in"]
-        # track expiration status/time (2 hours from creation)
+        # track expiration status/time
         current_time = datetime.now()
         if api_url == "nlst":
             nlst_token_exp_time = current_time + timedelta(seconds=expires_in)
             nlst_api_call_headers = {'Authorization': 'Bearer ' + access_token}
+            nlst_refresh_token = data.json()["refresh_token"]
             _log.info(f'Success - Token saved to nlst_api_call_headers variable and expires at {nlst_token_exp_time}')
         else:
-            token_exp_time = current_time + timedelta(seconds=expires_in)
+            token_exp_time = current_time + timedelta(seconds=expires_in)            
             api_call_headers = {'Authorization': 'Bearer ' + access_token}
+            refresh_token = data.json()["refresh_token"]
             _log.info(f'Success - Token saved to api_call_headers variable and expires at {token_exp_time}')
     # handle errors
     except requests.exceptions.HTTPError as errh:
         _log.error(f"HTTP Error: {data.status_code} -- Double check your user name and password.")
     except requests.exceptions.ConnectionError as errc:
         _log.error(f"Connection Error: {data.status_code}")
     except requests.exceptions.Timeout as errt:
         _log.error(f"Timeout Error: {data.status_code}")
     except requests.exceptions.RequestException as err:
         _log.error(f"Request Error: {data.status_code}")
 
-####### refreshToken()
-# Refreshes security token to extend access time for APIs that require authorization
-# Must first use getToken() to create a token
-
-def refreshToken(api_url = ""): 
-
+def refreshToken(api_url = ""):
+    """
+    refreshToken() refreshes security tokens to extend access time for APIs that require authorization.
+    It attempts to verify that a refresh token exists and recommends using getToken() to create a new token if needed.
+    This function is called as needed by setApiUrl() and is generally not something that needs to be called directly in your code.    
+    """
     global token_exp_time, nlst_token_exp_time, api_call_headers, nlst_api_call_headers
-
-    try:
-        refresh_token
-    except NameError:
-        _log.error("Error refreshing token for accessing the Restricted API. Create one using getToken().")
-        raise StopExecution
-    else:
-
-        # token URLs
-        if api_url == "nlst":
+   
+    # token URLs
+    if api_url == "nlst":
+        try:
+            token = nlst_refresh_token
+        except NameError:
+            _log.warning(f"No NLST refresh token found. Creating a new token...")
+            getToken(api_url = "nlst")
+            raise StopExecution
+        else:
             token_url = "https://nlst.cancerimagingarchive.net/nbia-api/oauth/token"
+    
+    else:
+        try:
+            token = refresh_token
+        except NameError:
+            _log.error("Error refreshing token for accessing the Restricted API. Create one using getToken().")
+            raise StopExecution
         else:
             token_url = "https://nbia.cancerimagingarchive.net/nbia-api/oauth/token"
 
-        # refresh token request
-        try:
-            params = {
-            'client_id': 'nbiaRestAPIClient',
-            'client_secret' : 'ItsBetweenUAndMe',
-            'grant_type': 'refresh_token',
-            'refresh_token' : refresh_token,
-            }
-            
-            # obtain new access token
-            data = requests.post(token_url, data = params)
-            data.raise_for_status()
-            access_token = data.json()["access_token"]
-            expires_in = data.json()["expires_in"]
-            # track expiration status/time (2 hours from creation)
-            current_time = datetime.now()
-            if api_url == "nlst":
-                nlst_token_exp_time = current_time + timedelta(seconds=expires_in)
-                nlst_api_call_headers = {'Authorization': 'Bearer ' + access_token}
-                _log.info(f'Success - Token refreshed to nlst_api_call_headers variable and expires at {nlst_token_exp_time}')
-            else:
-                token_exp_time = current_time + timedelta(seconds=expires_in)
-                api_call_headers = {'Authorization': 'Bearer ' + access_token}
-                _log.info(f'Success - Token refreshed to api_call_headers variable and expires at {token_exp_time}')
-        # handle errors
-        except requests.exceptions.HTTPError as errh:
-            _log.error(f"HTTP Error: {data.status_code} -- Double check your user name and password.")
-        except requests.exceptions.ConnectionError as errc:
-            _log.error(f"Connection Error: {data.status_code}")
-        except requests.exceptions.Timeout as errt:
-            _log.error(f"Timeout Error: {data.status_code}")
-        except requests.exceptions.RequestException as err:
-            _log.error(f"Request Error: {data.status_code}")
+    # refresh token request
+    try:
+        params = {
+        'client_id': 'nbiaRestAPIClient',
+        'client_secret' : 'ItsBetweenUAndMe',
+        'grant_type': 'refresh_token',
+        'refresh_token' : token,
+        }
+        
+        # obtain new access token
+        data = requests.post(token_url, data = params)
+        data.raise_for_status()
+        access_token = data.json()["access_token"]
+        expires_in = data.json()["expires_in"]
+        # track expiration status/time (2 hours from creation)
+        current_time = datetime.now()
+        if api_url == "nlst":
+            nlst_token_exp_time = current_time + timedelta(seconds=expires_in)
+            nlst_api_call_headers = {'Authorization': 'Bearer ' + access_token}
+            _log.info(f'Success - Token refreshed to nlst_api_call_headers variable and expires at {nlst_token_exp_time}')
+        else:
+            token_exp_time = current_time + timedelta(seconds=expires_in)
+            api_call_headers = {'Authorization': 'Bearer ' + access_token}
+            _log.info(f'Success - Token refreshed to api_call_headers variable and expires at {token_exp_time}')
+    # handle errors
+    except requests.exceptions.HTTPError as errh:
+        _log.error(f"HTTP Error: {data.status_code} -- Double check your user name and password.")
+    except requests.exceptions.ConnectionError as errc:
+        _log.error(f"Connection Error: {data.status_code}")
+    except requests.exceptions.Timeout as errt:
+        _log.error(f"Timeout Error: {data.status_code}")
+    except requests.exceptions.RequestException as err:
+        _log.error(f"Request Error: {data.status_code}")
             
-####### logoutToken()
-# Logs out of a security token for APIs that require authorization
-# Must first use getToken() to create a token
-
 def logoutToken(api_url = ""): 
-
-    global token_exp_time, nlst_token_exp_time, api_call_headers, nlst_api_call_headers, refresh_token
+    """
+    logoutToken() logs out security tokens used for APIs that require authorization.
+    Variables holding access token information are also deleted by this operation.
+    The api_url parameter can be used to specify whether your token was for the main server (leave empty) or NLST.
+    Use getToken() to create a new token if needed.
+    """
+    global token_exp_time, nlst_token_exp_time, api_call_headers, nlst_api_call_headers, refresh_token, nlst_refresh_token
 
     # determine which server the token was created on
     if api_url == "nlst" and 'nlst_api_call_headers' in globals():
         url = "https://nlst.cancerimagingarchive.net/nbia-api/logout"
         api_call_headers = nlst_api_call_headers
     elif api_url != "nlst" and 'api_call_headers' in globals():
         url = "https://services.cancerimagingarchive.net/nbia-api/logout"
@@ -271,33 +294,41 @@
         raise StopExecution
 
     try:
         _log.info(f'Logging out of... {url}')
         data = requests.get(url, headers = api_call_headers)
         _log.info(f'{data.text}')
         # remove variables holding token details
-        del token_exp_time, nlst_token_exp_time, api_call_headers, nlst_api_call_headers, refresh_token
+        if api_url == "nlst":
+            del nlst_token_exp_time, nlst_api_call_headers, nlst_refresh_token
+        else:
+            del token_exp_time, api_call_headers, refresh_token
 
     # handle errors
     except requests.exceptions.HTTPError as errh:
         _log.error(f"HTTP Error: {data.status_code} -- Double check your user name and password.")
     except requests.exceptions.ConnectionError as errc:
         _log.error(f"Connection Error: {data.status_code}")
     except requests.exceptions.Timeout as errt:
         _log.error(f"Timeout Error: {data.status_code}")
     except requests.exceptions.RequestException as err:
         _log.error(f"Request Error: {data.status_code}")
 
-####### makeCredentialFile()
-# Create a credential file to use with NBIA Data Retriever
-# Provides interactive prompts for user/pw if they're not specified as parameters
-# Documentation at https://wiki.cancerimagingarchive.net/x/2QKPBQ
-
 def makeCredentialFile(user = "", pw = ""):
-
+    """
+    Creates a credential file to use with NBIA Data Retriever. 
+    Interactive prompts are provided for user/pw if they're not specified as parameters.
+    The credential file is a text file that passes the user's credentials in the following format:
+        userName = YourUserName
+        passWord = YourPassword
+        Both parameters are case-sensitive.
+    Additional documentation:
+        https://wiki.cancerimagingarchive.net/x/2QKPBQ 
+        https://github.com/kirbyju/TCIA_Notebooks/blob/main/TCIA_Linux_Data_Retriever_App.ipynb
+    """
     # set user name and password
     if user == "":
         print("Enter User: ")
         userName = input()
     else:
         userName = user
     if pw == "":
@@ -313,15 +344,19 @@
 
 ####### queryData()
 # Called by query functions that use requests.get()
 # Provides error handling for requests.get()
 # Formats output as JSON by default with options for "df" (dataframe) and "csv"
 
 def queryData(endpoint, options, api_url, format):
-
+    """
+    queryData() is called by many other query functions and is generally not something that needs to be called directly in your code.
+    It provides uses setApiURL() to set a base URL and addresses error handling for HTTP status and empty search results.
+    Formats output as JSON by default with options for "df" (dataframe) and "csv"
+    """
     # get base URL
     base_url = setApiUrl(endpoint, api_url)
     # display full URL with endpoint & parameters
     url = base_url + endpoint
     _log.info(f'Calling... {url} with parameters {options}')
     # get the data
     try:
@@ -359,35 +394,39 @@
         _log.error(errc)
     except requests.exceptions.Timeout as errt:
         _log.error(errt)
     except requests.exceptions.RequestException as err:
         _log.error(err)
     
 
-####### getCollections function
-# Gets a list of collections from a specified api_url
-
 def getCollections(api_url = "",
                    format = ""):
-
+    """
+    Optional: api_url, format
+    Gets a list of collections from a specified api_url
+    """
     endpoint = "getCollectionValues"
     options = {}
 
     data = queryData(endpoint, options, api_url, format)
     return data
 
 ####### getBodyPart function
 # Gets Body Part Examined metadata from a specified api_url
 # Allows filtering by collection and modality
 
 def getBodyPart(collection = "",
                 modality = "",
                 api_url = "",
                 format = ""):
-
+    """
+    Optional: api_url, format
+    Gets Body Part Examined metadata from a specified api_url
+    Allows filtering by collection and modality
+    """
     endpoint = "getBodyPartValues"
 
     # create options dict to construct URL
     options = {}
 
     if collection:
         options['Collection'] = collection
@@ -401,15 +440,19 @@
 # Gets Modalities metadata from a specified api_url
 # Allows filtering by collection and bodyPart
 
 def getModality(collection = "",
                 bodyPart = "",
                 api_url = "",
                 format = ""):
-
+    """
+    Optional: api_url, format
+    Gets Modalities metadata from a specified api_url
+    Allows filtering by collection and bodyPart
+    """
     endpoint = "getModalityValues"
 
     # create options dict to construct URL
     options = {}
 
     if collection:
         options['Collection'] = collection
@@ -422,15 +465,19 @@
 ####### getPatient function
 # Gets Patient metadata from a specified api_url
 # Allows filtering by collection
 
 def getPatient(collection = "",
                api_url = "",
                format = ""):
-
+    """
+    Optional: api_url, format
+    Gets Patient metadata from a specified api_url
+    Allows filtering by collection
+    """
     endpoint = "getPatient"
 
     # create options dict to construct URL
     options = {}
 
     if collection:
         options['Collection'] = collection
@@ -443,15 +490,19 @@
 # Requires specifying collection and modality
 # Returns a list of patient IDs
 
 def getPatientByCollectionAndModality(collection,
                                       modality,
                                       api_url = "",
                                       format = ""):
-
+    """
+    Optional: api_url, format
+    Gets Patient IDs from a specified api_url
+    Returns a list of patient IDs
+    """
     endpoint = "getPatientByCollectionAndModality"
 
     # create options dict to construct URL
     options = {}
     options['Collection'] = collection
     options['Modality'] = modality
 
@@ -463,15 +514,19 @@
 # Requires specifying collection and date
 # Date format is YYYY/MM/DD
 
 def getNewPatientsInCollection(collection,
                                date,
                                api_url = "",
                                format = ""):
-
+    """
+    Optional: api_url, format
+    Gets "new" patient metadata from a specified api_url
+    The date format is YYYY/MM/DD
+    """
     endpoint = "NewPatientsInCollection"
 
     # create options dict to construct URL
     options = {}
     options['Collection'] = collection
     options['Date'] = date
 
@@ -484,15 +539,18 @@
 # Optional filters for patientId and studyUid
 
 def getStudy(collection,
              patientId = "",
              studyUid = "",
              api_url = "",
              format = ""):
-
+    """
+    Optional: patientId, studyUid, api_url, format
+    Gets Study (visit/timepoint) metadata from a specified api_url
+    """
     endpoint = "getPatientStudy"
 
     # create options dict to construct URL
     options = {}
     options['Collection'] = collection
 
     if patientId:
@@ -509,15 +567,19 @@
 # Date format is YYYY/MM/DD
 
 def getNewStudiesInPatient(collection,
                            patientId,
                            date,
                            api_url = "",
                            format = ""):
-
+    """
+    Optional: api_url, format
+    Gets "new" patient metadata from a specified api_url
+    The date format is YYYY/MM/DD
+    """
     endpoint = "NewStudiesInPatientCollection"
 
     # create options dict to construct URL
     options = {}
     options['Collection'] = collection
     options['PatientID'] = patientId
     options['Date'] = date
@@ -536,15 +598,20 @@
               seriesUid = "",
               modality = "",
               bodyPart = "",
               manufacturer = "",
               manufacturerModel = "",
               api_url = "",
               format = ""):
-
+    """
+    All parameters are optional.
+    Gets Series (scan) metadata from a specified api_url
+    Allows filtering by collection, patient ID, study UID, series UID, modality, body part, manufacturer & model
+    Note: Since the output of this function can be very long, it is advisable to save the output to a variable and only display a portion of it at a time when the output format is JSON.
+    """
     endpoint = "getSeries"
 
     # create options dict to construct URL
     options = {}
 
     if collection:
         options['Collection'] = collection
@@ -572,15 +639,20 @@
 # Date format is YYYY/MM/DD
 # NOTE: NBIA API expects MM/DD/YYYY (unlike any other API endpoint!)
 #        so we'll convert from YYYY/MM/DD so tcia-utils is consistent
 
 def getUpdatedSeries(date,
                      api_url = "",
                      format = ""):
-
+    """
+    Optional: api_url, format
+    Gets "new" series metadata from a specified api_url
+    The date format is YYYY/MM/DD
+    NOTE: Unlike other API endpoints, this function expects MM/DD/YYYY, we'll convert from YYYY/MM/DD so tcia-utils is consistent
+    """
     endpoint = "getUpdatedSeries"
 
     # convert to NBIA's expected date format
     nbiaDate = datetime.strptime(date, "%Y/%m/%d").strftime("%m/%d/%Y")
 
     # create options dict to construct URL
     options = {}
@@ -593,15 +665,19 @@
 # Gets Series (scan) metadata from a specified api_url
 # Requires a specific Series Instance UID as input
 # Output includes DOI and license details that are not in getSeries()
 
 def getSeriesMetadata(seriesUid,
                       api_url = "",
                       format = ""):
-
+    """
+    Optional: api_url, format
+    Gets Series (scan) metadata from a specified api_url
+    Output includes DOI and license details that are not in the getSeries() function
+    """
     endpoint = "getSeriesMetaData"
 
     # create options dict to construct URL
     options = {}
     options['SeriesInstanceUID'] = seriesUid
 
     data = queryData(endpoint, options, api_url, format)
@@ -610,15 +686,18 @@
 ####### getSeriesSize function
 # Gets the file count and disk size of a series/scan
 # Requires Series Instance UID as input
 
 def getSeriesSize(seriesUid,
                   api_url = "",
                   format = ""):
-
+    """
+    Optional: api_url, format
+    Gets the file count and disk size of a series/scan
+    """
     endpoint = "getSeriesSize"
 
     # create options dict to construct URL
     options = {}
     options['SeriesInstanceUID'] = seriesUid
 
     data = queryData(endpoint, options, api_url, format)
@@ -627,15 +706,18 @@
 ####### getSopInstanceUids function
 # Gets SOP Instance UIDs from a specific series/scan
 # Requires a specific Series Instance UID as input
 
 def getSopInstanceUids(seriesUid,
                        api_url = "",
                        format = ""):
-
+    """
+    Optional: api_url, format
+    Gets SOP Instance UIDs from a specific series/scan
+    """
     endpoint = "getSOPInstanceUIDs"
 
     # create options dict to construct URL
     options = {}
     options['SeriesInstanceUID'] = seriesUid
 
     data = queryData(endpoint, options, api_url, format)
@@ -646,15 +728,19 @@
 # Allows filtering by collection, body part & modality
 
 def getManufacturer(collection = "",
                     modality = "",
                     bodyPart = "",
                     api_url = "",
                     format = ""):
-
+    """
+    All parameters are optional.
+    Gets manufacturer metadata from a specified api_url
+    Allows filtering by collection, body part & modality
+    """
     endpoint = "getManufacturerValues"
 
     # create options dict to construct URL
     options = {}
 
     if collection:
         options['Collection'] = collection
@@ -673,15 +759,20 @@
 # The "name" parameter is part of the URL that generates.
 # E.g https://nbia.cancerimagingarchive.net/nbia-search/?saved-cart=nbia-49121659384603347
 #  has a cart "name" of "nbia-49121659384603347".
 
 def getSharedCart(name,
                   api_url = "",
                   format = ""):
-
+    """
+    Optional: api_url, format
+    Gets "Shared Cart" (scan) metadata from a specified api_url
+    First use https://nbia.cancerimagingarchive.net/nbia-search/ to create a cart, then add data to your basket, then click "Share" > "Share my cart".
+    The "name" parameter is part of the URL that generates. E.g https://nbia.cancerimagingarchive.net/nbia-search/?saved-cart=nbia-49121659384603347 has a cart "name" of "nbia-49121659384603347".
+    """
     endpoint = "getContentsByName"
 
     # create options dict to construct URL
     options = {}
     options['name'] = name
 
     data = queryData(endpoint, options, api_url, format)
@@ -703,15 +794,26 @@
                    number = 0,
                    path = "",
                    hash = "",
                    api_url = "",
                    input_type = "",
                    format = "",
                    csv_filename = ""):
-
+    """
+    Ingests a set of seriesUids and downloads them
+    By default, series_data expects JSON containing "SeriesInstanceUID" elements.
+    Set number = n to download the first n series if you don't want the full dataset.
+    Set hash = "y" if you'd like to retrieve MD5 hash values for each image.
+    Saves to tciaDownload folder in current directory if no path is specified
+    Set input_type = "list" to pass a list of Series UIDs instead of JSON.
+    Set input_type = "manifest" to pass the path of a *.TCIA manifest file as series_data.
+    Format can be set to "df" or "csv" to return series metadata.
+    Setting a csv_filename will create the csv even if format isn't specified.
+    The metadata includes info about series that have previously been downloaded.
+    """
     endpoint = "getImage"
     seriesUID = ''
     success = 0
     failed = 0
     previous = 0
 
     # Prep a dataframe for later
@@ -834,15 +936,15 @@
 ####### downloadImage function
 # Ingests a seriesUids and SopInstanceUid and downloads the image
 
 def downloadImage(seriesUID,
                   sopUID,
                   path = "",
                   api_url = ""):
-
+    """Ingests a seriesUids and SopInstanceUid and downloads the image"""
     endpoint = "getSingleImage"
     success = 0
     failed = 0
     previous = 0
 
     # get base URL
     base_url = setApiUrl(endpoint, api_url)
@@ -900,40 +1002,51 @@
 ##########################
 # Advanced API Endpoints
 
 ####### getCollectionDescriptions function (Advanced)
 # Get HTML-formatted descriptions of collections and their DOIs
 
 def getCollectionDescriptions(api_url = "", format = ""):
+    """
+    All parameters are optional.
+    Gets HTML-formatted descriptions of collections and their DOIs
+    """
     endpoint = "getCollectionDescriptions"
     options = {}
 
     data = queryData(endpoint, options, api_url, format)
     return data
 
 ####### getCollectionPatientCounts function (Advanced)
 # Get patient counts by collection from Advanced API
 
 def getCollectionPatientCounts(api_url = "", format = ""):
-
+    """
+    All parameters are optional.
+    Gets counts of Patient by collection from Advanced API
+    """
     endpoint = "getCollectionValuesAndCounts"
     options = {}
 
     data = queryData(endpoint, options, api_url, format)
     return data
 
 ####### getModalityCounts function (Advanced)
 # Get counts of Modality metadata from Advanced API
 # Allows filtering by collection and bodyPart
 
 def getModalityCounts(collection = "",
                       bodyPart = "",
                       api_url = "",
                       format = ""):
-
+    """
+    All parameters are optional.
+    Gets counts of Modality metadata from Advanced API
+    Allows filtering by collection and bodyPart
+    """
     endpoint = "getModalityValuesAndCounts"
 
     # create options dict to construct URL
     options = {}
 
     if collection:
         options['Collection'] = collection
@@ -947,15 +1060,19 @@
 # Get counts of Body Part metadata from Advanced API
 # Allows filtering by collection and modality
 
 def getBodyPartCounts(collection = "",
                       modality = "",
                       api_url = "",
                       format = ""):
-
+    """
+    All parameters are optional.
+    Gets counts of Body Part metadata from Advanced API
+    Allows filtering by collection and modality
+    """
     endpoint = "getBodyPartValuesAndCounts"
 
     # create options dict to construct URL
     options = {}
 
     if collection:
         options['Collection'] = collection
@@ -970,15 +1087,19 @@
 # Allows filtering by collection, body part and modality
 
 def getManufacturerCounts(collection = "",
                       modality = "",
                       bodyPart = "",
                       api_url = "",
                       format = ""):
-
+    """
+    All parameters are optional.
+    Gets counts of Manufacturer metadata from Advanced API
+    Allows filtering by collection, body part and modality
+    """
     endpoint = "getManufacturerValuesAndCounts"
 
     # create options dict to construct URL
     options = {}
 
     if collection:
         options['Collection'] = collection
@@ -992,15 +1113,20 @@
 
 ####### getSeriesList function (Advanced)
 # Get series metadata from Advanced API
 # Allows submission of a list of UIDs
 # Returns result as dataframe and CSV
 
 def getSeriesList(list, api_url = "", csv_filename = ""):
-
+    """
+    Optional: api_url, csv_filename
+    Get series metadata from Advanced API
+    Allows submission of a list of UIDs
+    Returns result as dataframe and CSV
+    """
     uids = ",".join(list)
     param = {'list': uids}
     endpoint = "getSeriesMetadata2"
 
     # set base_url
     base_url = setApiUrl(endpoint, api_url)
 
@@ -1040,15 +1166,18 @@
 
 ####### getDicomTags function (Advanced)
 # Gets DICOM tag metadata for a given series UID (scan)
 
 def getDicomTags(seriesUid,
                  api_url = "",
                  format = ""):
-
+    """
+    Optional: api_url, format
+    Gets DICOM tag metadata for a given series UID (scan)
+    """
     endpoint = "getDicomTags"
 
     # create options dict to construct URL
     options = {}
     options['SeriesUID'] = seriesUid
 
     data = queryData(endpoint, options, api_url, format)
@@ -1118,15 +1247,19 @@
 ####### getDoiMetadata function
 # Gets a list of Collections or Series associated with a DOI
 # Requires a DOI URL and specification of Collection or Series UID output
 # Result includes whether the data are 3rd party analyses or not
 # Formats output as JSON by default with options for "df" (dataframe) and "csv"
 
 def getDoiMetadata(doi, output, api_url = "", format = ""):
-
+    """
+    Optional: output, api_url, format
+    Gets a list of Collections if output = "", or Series if output = "series", associated with a DOI.
+    The result includes whether the data are 3rd party analyses or not.
+    """
     param = {'DOI': doi,
              'CollectionOrSeries': output}
 
     endpoint = "getCollectionOrSeriesForDOI"
 
     # set base_url
     base_url = setApiUrl(endpoint, api_url)
@@ -1186,16 +1319,18 @@
     start = 0,
     size = 10,
     sortDirection = 'ascending',
     sortField = 'subject',
     api_url = "",
     format = ""):
     """
-    Takes the same parameters as the SimpleSearch GUI; using more parameters narrows
-    the number of subjects received.
+    All parameters are optional.
+    Takes the same parameters as the SimpleSearch GUI
+    Use more parameters to narrow the number of subjects received.
+    Note: This function only supports output of JSON format, please leave the format parameter as it.
 
     collections: list[str]   -- The DICOM collections of interest to you
     species: list[str]       -- Filter collections by species. Possible values are 'human', 'mouse', and 'dog'
     modalities: list[str]    -- Filter collections by modality
     modalityAnded: bool      -- If true, only return subjects with all requested modalities, as opposed to any
     minStudies: int          -- The minimum number of studies a collection must have to be included in the results
     manufacturers: list[str] -- Imaging device manufacturers, e.g. SIEMENS
@@ -1338,15 +1473,24 @@
 #    you must call getToken() with a user ID that has access to all UIDs before calling this function.
 # Specifying api_url is only necessary if you are using input_type = "manifest" or "list" with NLST data (e.g. api_url = "nlst") 
 # Specify format = "var" to return the report values as a dictionary
 # Access variables example after saving function output to report_data: subjects = report_data["subjects"]
 # Specify format = "file" to save the report to a file
 # Specify a filename parameter to set a filename if you don't want the default
 
-
+    """
+    Ingests JSON output from any function that returns series-level data and creates summary report
+    Specify input_type = "manifest" to ingest a *.TCIA manifest file or "list" for a python list of UIDs.
+    If input_type = "manifest" or "list" and there are series UIDs that are restricted, you must call getToken() with a user ID that has access to all UIDs before calling this function.
+    Specifying api_url is only necessary if you are using input_type = "manifest" or "list" with NLST data (e.g. api_url = "nlst").
+    Specify format = "var" to return the report values as a dictionary.
+    Access variables example after saving function output to report_data: subjects = report_data["subjects"].
+    Specify format = "file" to save the report to a file.
+    Specify a filename parameter to set a filename if you don't want the default filename.
+    """
     # if input_type is manifest convert it to a list
     if input_type == "manifest":
         series_data = manifestToList(series_data)
         
     # if input_type is a list or manifest download relevant metadata
     if input_type == "list" or input_type == "manifest":
         df = getSeriesList(series_data, api_url = "", csv_filename = "")
@@ -1432,15 +1576,19 @@
         _log.info(report)
 
 ####### manifestToList function
 # Ingests a TCIA manifest file and removes header
 # Returns a list of series UIDs
 
 def manifestToList(manifest):
-
+    """
+    Ingests a TCIA manifest file and removes header
+    Returns a list of series UIDs
+    Because it is primarily a helper function used by downloadSeries() and makeSeriesReport(), please do NOT use this function.
+    """
     # initialize variable
     data = []
 
     # open file and write lines to a list
     with open(manifest) as f:
         # verify this is a tcia manifest file
         first_line = f.readline()
@@ -1470,15 +1618,24 @@
 # TCIA links display the individual series described in each row
 # IDC links display the entire study (all scans from that time point)
 # IDC links may not work if they haven't mirrored the series from TCIA yet
 # This function only works with fully public datasets (no limited-access data)
 # Optionally accepts a csv_filename parameter if you'd like to export a CSV file
 
 def makeVizLinks(series_data, csv_filename=""):
-
+    """
+    Ingests JSON output of getSeries() or getSharedCart()
+    Creates URLs to visualize them in a browser
+    The links appear in the last 2 columns of the dataframe.
+    TCIA links display the individual series described in each row.
+    IDC links display the entire study (all scans from that time point).
+    IDC links may not work if they haven't mirrored the series from TCIA, yet.
+    This function only works with fully public datasets (no limited-access data).
+    Optionally accepts a csv_filename parameter if you'd like to export a CSV file.
+    """
     # set base urls for tcia/idc
     tciaVizUrl = "https://nbia.cancerimagingarchive.net/viewer/?series="
     idcVizUrl = "https://viewer.imaging.datacommons.cancer.gov/viewer/"
 
     # create dataframe and append base URLs to study/series UIDs
     df = pd.DataFrame(series_data)
     df['VisualizeSeriesOnTcia'] = tciaVizUrl + df['SeriesInstanceUID']
@@ -1496,15 +1653,20 @@
 # Visualize a Series (scan) you've downloaded in the notebook
 # Requires EITHER a seriesUid or path parameter
 # Leave seriesUid empty if you want to provide a custom path
 # The function assumes "tciaDownload/<seriesUid>/" as path if seriesUid is
 #   provided since this is where downloadSeries() saves data
 
 def viewSeries(seriesUid = "", path = ""):
-
+    """
+    Visualizes a Series (scan) you've downloaded in the notebook
+    Requires EITHER a seriesUid or path parameter
+    Leave seriesUid empty if you want to provide a custom path.
+    The function assumes "tciaDownload/<seriesUid>/" as path if seriesUid is provided since this is where downloadSeries() saves data.
+    """
     # set path where downloadSeries() saves the data if seriesUid is provided
     if seriesUid != "":
         path = "tciaDownload/" + seriesUid
 
     # error message function for when series doesn't exist or is invalid data
     def seriesInvalid(uid):
         if seriesUid:
```

### Comparing `tcia_utils-1.5/src/tcia_utils/pathdb.py` & `tcia_utils-1.5.1/src/tcia_utils/pathdb.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.5/.gitignore` & `tcia_utils-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.5/LICENSE` & `tcia_utils-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.5/README.md` & `tcia_utils-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.5/pyproject.toml` & `tcia_utils-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcia_utils"
-version = "1.5"
+version = "1.5.1"
 authors = [
   { name="Justin Kirby", email="justin.kirby@nih.gov" },
 ]
 description = "A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcia_utils-1.5/PKG-INFO` & `tcia_utils-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcia_utils
-Version: 1.5
+Version: 1.5.1
 Summary: A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python.
 Project-URL: Homepage, https://github.com/kirbyju/tcia_utils
 Project-URL: Bug Tracker, https://github.com/kirbyju/tcia_utils/issues
 Author-email: Justin Kirby <justin.kirby@nih.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

