# Comparing `tmp/robotframework-robotlog2db-1.3.7.tar.gz` & `tmp/robotframework-robotlog2db-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-robotlog2db-1.3.7.tar", last modified: Wed Jun 14 08:58:32 2023, max compression
+gzip compressed data, was "robotframework-robotlog2db-1.3.8.tar", last modified: Wed Jun 21 11:40:54 2023, max compression
```

## Comparing `robotframework-robotlog2db-1.3.7.tar` & `robotframework-robotlog2db-1.3.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:32.617748 robotframework-robotlog2db-1.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-06-14 08:58:32.617748 robotframework-robotlog2db-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:32.613748 robotframework-robotlog2db-1.3.7/RobotLog2DB/
--rw-r--r--   0 runner    (1001) docker     (123)    42027 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/RobotLog2DB/CDataBase.py
--rw-r--r--   0 runner    (1001) docker     (123)   595626 2023-06-14 08:58:32.000000 robotframework-robotlog2db-1.3.7/RobotLog2DB/RobotLog2DB.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/RobotLog2DB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/RobotLog2DB/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43119 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/RobotLog2DB/robotlog2db.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/RobotLog2DB/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:32.613748 robotframework-robotlog2db-1.3.7/RobotLog2DB/xsd/
--rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/RobotLog2DB/xsd/robot.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:58:32.617748 robotframework-robotlog2db-1.3.7/robotframework_robotlog2db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-06-14 08:58:32.000000 robotframework-robotlog2db-1.3.7/robotframework_robotlog2db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-14 08:58:32.000000 robotframework-robotlog2db-1.3.7/robotframework_robotlog2db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:58:32.000000 robotframework-robotlog2db-1.3.7/robotframework_robotlog2db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 08:58:32.000000 robotframework-robotlog2db-1.3.7/robotframework_robotlog2db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 08:58:32.000000 robotframework-robotlog2db-1.3.7/robotframework_robotlog2db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 08:58:32.000000 robotframework-robotlog2db-1.3.7/robotframework_robotlog2db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:58:32.617748 robotframework-robotlog2db-1.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-14 08:56:25.000000 robotframework-robotlog2db-1.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:54.965007 robotframework-robotlog2db-1.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-06-21 11:40:54.965007 robotframework-robotlog2db-1.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:54.965007 robotframework-robotlog2db-1.3.8/RobotLog2DB/
+-rw-r--r--   0 runner    (1001) docker     (123)    41226 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/RobotLog2DB/CDataBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)   595489 2023-06-21 11:40:53.000000 robotframework-robotlog2db-1.3.8/RobotLog2DB/RobotLog2DB.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/RobotLog2DB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/RobotLog2DB/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43282 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/RobotLog2DB/robotlog2db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/RobotLog2DB/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:54.965007 robotframework-robotlog2db-1.3.8/RobotLog2DB/xsd/
+-rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/RobotLog2DB/xsd/robot.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:40:54.965007 robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-06-21 11:40:54.000000 robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-21 11:40:54.000000 robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:40:54.000000 robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 11:40:54.000000 robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 11:40:54.000000 robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-21 11:40:54.000000 robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 11:40:54.965007 robotframework-robotlog2db-1.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-21 11:38:02.000000 robotframework-robotlog2db-1.3.8/setup.py
```

### Comparing `robotframework-robotlog2db-1.3.7/PKG-INFO` & `robotframework-robotlog2db-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robotlog2db
-Version: 1.3.7
+Version: 1.3.8
 Summary: Imports robot result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/robotframework-robotlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -296,15 +296,15 @@
 
 [Tran Hoang Nguyen](mailto:Nguyen.TranHoang@vn.bosch.com)
 
 [Holger Queckenstedt](mailto:Holger.Queckenstedt@de.bosch.com)
 
 ### License
 
-Copyright 2020-2022 Robert Bosch GmbH
+Copyright 2020-2023 Robert Bosch GmbH
 
 Licensed under the Apache License, Version 2.0 (the \"License\"); you
 may not use this file except in compliance with the License. You may
 obtain a copy of the License at
 
 > [![License: Apache
 > v2](https://img.shields.io/pypi/l/robotframework.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)
```

### Comparing `robotframework-robotlog2db-1.3.7/README.rst` & `robotframework-robotlog2db-1.3.8/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 -  `Sourcecode Documentation <#sourcecode-documentation>`__
 -  `Feedback <#feedback>`__
 -  `About <#about>`__
 
    -  `Maintainers <#maintainers>`__
    -  `Contributors <#contributors>`__
    -  `License <#license>`__
-   
+
 Getting Started
 ---------------
 
-**RobotLog2DB** is a command-line tool that enables you to import `Robot 
-Framework XML result`_ files into TestResultWebApp_'s database for 
-presenting an overview about the whole test execution and detail of each test 
+**RobotLog2DB** is a command-line tool that enables you to import `Robot
+Framework XML result`_ files into TestResultWebApp_'s database for
+presenting an overview about the whole test execution and detail of each test
 result.
 
-**RobotLog2DB** tool is operating system independent and only works with 
+**RobotLog2DB** tool is operating system independent and only works with
 Python 3.
 
 How to install
 ~~~~~~~~~~~~~~
 
 **RobotLog2DB** can be installed in two different ways.
 
@@ -82,26 +82,26 @@
 
    * Use the following command to install **RobotLog2DB**:
 
      .. code::
 
         python setup.py install
 
-After succesful installation, the executable file **RobotLog2DB** 
-will be available (under *Scripts* folder of Python on Windows 
+After succesful installation, the executable file **RobotLog2DB**
+will be available (under *Scripts* folder of Python on Windows
 and *~/.local/bin/* folder on Linux).
 
-In case above location is added to **PATH** environment variable 
+In case above location is added to **PATH** environment variable
 then you can run it directly as operation system's command.
 
 Usage
 -----
 
-**RobotLog2DB** requires the Robot Framework result file(s) which contains the 
-output result in XML format (default name is ``output.xml``) and 
+**RobotLog2DB** requires the Robot Framework result file(s) which contains the
+output result in XML format (default name is ``output.xml``) and
 TestResultWebApp_'s database information for importing.
 
 Use below command to get tools's usage
 
 ::
 
    RobotLog2DB -h
@@ -131,15 +131,15 @@
    --append             is used in combination with --UUID <UUID>.If set, allow to append new result(s) to existing execution result UUID in --UUID argument.
    --UUID UUID          UUID used to identify the import and version ID on webapp. If not provided RobotLog2DB will generate an UUID for the whole import.
    --variant VARIANT    variant name to be set for this import.
    --versions VERSIONS  metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).
    --config CONFIG      configuration json file for component mapping information.
 
 
-The below command is simple usage with all required arguments to import 
+The below command is simple usage with all required arguments to import
 Robot Framework results into TestResultWebApp's database:
 
 ::
 
    RobotLog2DB <resultxmlfile> <server> <user> <password> <database>
 
 Besides the executable file, you can also run tool as a Python module
@@ -148,20 +148,20 @@
 
    python -m RobotLog2DB <resultxmlfile> <server> <user> <password> <database>
 
 
 Example
 -------
 
-In order the import the Robot Framework result(s) to TestResultWebApp's database, 
+In order the import the Robot Framework result(s) to TestResultWebApp's database,
 we need the Robot Framework result file (``output.xml``).
 
 So, firstly execute the Robot Framework testcase(s) to get the Robot Framework result file.
 
-Sample Robot Framework testcase which contains neccessary information for importing into 
+Sample Robot Framework testcase which contains neccessary information for importing into
 TestResultWebApp's database:
 
 ::
 
    *** Settings ***
    # Test execution level
    Metadata   project        ROBFW              # Project/Variant
@@ -186,69 +186,69 @@
       [Tags]   ISSUE-RTC-003   TCID-1002   FID-113
       Log   	This is Testcase 01
 
 
 Notes:
 ~~~~~~
 
-   In case you are using RobotFramework AIO, these below ``Metadata`` 
-   definitions will be handled implicitly by `RobotFramework Testsuites 
-   Management`_ library within Suite Setup. 
+   In case you are using RobotFramework AIO, these below ``Metadata``
+   definitions will be handled implicitly by `RobotFramework Testsuites
+   Management`_ library within Suite Setup.
 
    * project
    * version_sw
    * version_hw
    * version_test
    * machine
    * tester
    * testtool
 
    So that you do not need to define them in your Robot Framework testcase(s).
 
-   However, if these ``Metadata`` definitions are already missing in the 
+   However, if these ``Metadata`` definitions are already missing in the
    Robot Framework output result file, you can specific them when executing the
    **RobotLog2DB** tool with the optional arguments:
 
    * ``--variant VARIANT``: Project definitions
    * ``--versions VERSIONS``: Versions (Software;Hardware;Test) definitions.
    * ``--config CONFIG``: Project, versions or component mapping definitions.
 
    Please refer to `RobotLog2DB tool’s Documentation`_ for more detail about
    these optional arguments.
 
-After getting Robot Framework result file (``output.xml``), use below sample 
-command to  import that result into TestResultWebApp's database which is hosted 
+After getting Robot Framework result file (``output.xml``), use below sample
+command to  import that result into TestResultWebApp's database which is hosted
 at *localhost* as below sample command
 
 ::
 
    RobotLog2DB output.xml localhost test_user test_pw test_db
 
-Then, open TestResultWebApp with your favourite browser and you will see how 
+Then, open TestResultWebApp with your favourite browser and you will see how
 wonderful the execution result is displayed as below figures:
 
 Dashboard view:
 
 .. image:: https://github.com/test-fullautomation/robotframework-robotlog2db/blob/develop/packagedoc/additional_docs/pictures/Dashboard.png?raw=true
    :alt: Dashboard view
 
 Datatable view:
 
 .. image:: https://github.com/test-fullautomation/robotframework-robotlog2db/blob/develop/packagedoc/additional_docs/pictures/Datatable.png?raw=true
    :alt: Datatable view
 
 Contribution
 ------------
-We are always searching support and you are cordially invited to help to improve 
+We are always searching support and you are cordially invited to help to improve
 **RobotLog2DB** tool.
 
 Sourcecode Documentation
 ------------------------
 To understand more detail about the tool's features, parameters and how Robot Framework
-testcase information will be displayed on TestResultWebApp, please refer to 
+testcase information will be displayed on TestResultWebApp, please refer to
 `RobotLog2DB tool’s Documentation`_.
 
 Feedback
 --------
 Please feel free to give any feedback to us via
 
 Email to: `Thomas Pollerspöck`_
@@ -274,15 +274,15 @@
 `Tran Hoang Nguyen`_
 
 `Holger Queckenstedt`_
 
 License
 ~~~~~~~
 
-Copyright 2020-2022 Robert Bosch GmbH
+Copyright 2020-2023 Robert Bosch GmbH
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     |License: Apache v2|
```

### Comparing `robotframework-robotlog2db-1.3.7/RobotLog2DB/CDataBase.py` & `robotframework-robotlog2db-1.3.8/RobotLog2DB/CDataBase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2023 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,58 +16,58 @@
 # File: CDataBase.py
 #
 # Initialy created by Pollerspoeck Thomas (CM/PJ-CMD) / June 2016
 #
 # This class provides methods to interact with TestResultWebApp's database.
 #
 # History:
-# 
+#
 # June 2016:
 #  - initial version
-# 
+#
 # February 2022:
 #  - update sourcecode document
-# 
+#
 # *******************************************************************************
 
 import MySQLdb as db
 
 class CDataBase(object):
    """
-CDataBase class play a role as mysqlclient and provide methods to interact  
+CDataBase class play a role as mysqlclient and provide methods to interact
 with TestResultWebApp's database.
    """
    __single = None
-   
+
    __NUM_BUFFERD_ELEMENTS_FOR_EXECUTEMANY=100
-   
+
    #make the CDataBase to singleton
    #! __new__ requires inheritance from "object" !
    def __new__(classtype, *args, **kwargs):
       """
-Create object method to make singleton class ``CDataBase``. 
+Create object method to make singleton class ``CDataBase``.
       """
       # Check to see if a __single exists already for this class
       # Compare class types instead of just looking for None so
       # that subclasses will create their own __single objects
       if classtype != type(classtype.__single):
          classtype.__single = object.__new__(classtype)
       return classtype.__single
 
    def __init__(self):
       """
 Initializer of class ``CDataBase``.
       """
-      con      = None  
-      db       = None 
+      con      = None
+      db       = None
       self.lTestCases = []
-      
+
    def __del__(self):
       pass
-  
+
    def connect(self,host        = None,
                     user        = None,
                     passwd      = None,
                     database    = None,
                     charset     = 'utf8',
                     use_unicode = True):
       """
@@ -105,121 +105,121 @@
 
    The connection character set.
 
 *  ``use_unicode``
 
    / *Condition*: optional / *Type*: bool / *Default*: True /
 
-   If True, CHAR and VARCHAR and TEXT columns are returned as Unicode strings, 
+   If True, CHAR and VARCHAR and TEXT columns are returned as Unicode strings,
    using the configured character set.
 
 **Returns:**
 
 (*no returns*)
       """
 
       if (host==None or user==None or passwd==None or database==None):
          raise Exception("host, user, passwd and database need to be provided!")
-   
+
       self.db = database
-      
-      # default encoding of python is latin-1, 
+
+      # default encoding of python is latin-1,
       # therefore we force mysql to convert to encode to utf8.
       self.con = db.connect(host,user,passwd,db=database,charset=charset,use_unicode=use_unicode)
       #for test purpose activate autocommit with (True)
       self.con.autocommit(False)
       print("Successfully connected to: %s@%s" % (self.db, host))
-  
+
    def disconnect(self):
       """
-Disconnect from TestResultWebApp's database. 
+Disconnect from TestResultWebApp's database.
 
 **Arguments:**
 
 (*no arguments*)
 
 **Returns:**
 
 (*no returns*)
       """
       self.con.commit()
       self.con.close()
-       
+
    def cleanAllTables(self):
       """
 Delete all table data. Please be careful before calling this method.
 
 **Arguments:**
 
 (*no arguments*)
 
 **Returns:**
 
 (*no returns*)
       """
       print(">> Deleting all table data!")
       sql="""delete from """ + self.db + """.evtbl_result_main where test_result_id!="" """
-      self.__arExec(sql) 
+      self.__arExec(sql)
       sql="""delete from """ + self.db + """.evtbl_failed_unknown_per_component where test_result_id!="" """
-      self.__arExec(sql) 
+      self.__arExec(sql)
       sql="""delete from """ + self.db + """.tbl_usr_case where test_case_id>0"""
-      self.__arExec(sql) 
+      self.__arExec(sql)
       sql="""delete from """ + self.db + """.tbl_usr_case_history where test_case_id>0"""
       self.__arExec(sql)
       sql="""delete from """ + self.db + """.tbl_usr_comments where test_case_id>0"""
       self.__arExec(sql)
       sql="""delete from """ + self.db + """.tbl_usr_links where test_case_id>0"""
       self.__arExec(sql)
       sql="""delete from """ + self.db + """.tbl_usr_result where test_result_id!="" """
       self.__arExec(sql)
       sql="""delete from """ + self.db + """.tbl_usr_result_history where test_result_id!="" """
       self.__arExec(sql)
-      
+
       sql="""delete from """ + self.db + """.tbl_file_header where file_id>0"""
-      self.__arExec(sql)   
+      self.__arExec(sql)
       sql="""delete from """ + self.db + """.tbl_case where test_case_id>0"""
-      self.__arExec(sql) 
+      self.__arExec(sql)
       sql="""delete from """ + self.db + """.tbl_file where file_id>0"""
       self.__arExec(sql)
       sql="""delete from """ + self.db + """.tbl_result where test_result_id!="" """
       self.__arExec(sql)
       sql="""delete from """ + self.db + """.tbl_prj where project<>"a" """
       self.__arExec(sql)
       self.con.commit()
-           
+
    def __arExec(self, command, values=None, bHasResponse=False, bReturnInsertedID=False):
       """
 Execute a query. By default don't try to fetch a result.
 
 **Arguments:**
 
 *  ``command``
 
    / *Condition*: required / *Type*: str /
-   
+
    Query need to be executed.
 
 *  ``values``
 
    / *Condition*: optional / *Type*: list / *Default*: None /
-   
+
    Sequence of parameters to be used with the query.
 
 *  ``bHasResponse``
 
    / *Condition*: optional / *Type*: bool / *Default*: False /
-   
+
    If True, respsonse is expected.
 
 *  ``bReturnInsertedID``
 
    / *Condition*: optional / *Type*: bool / *Default*: False /
-   
+
    If True, the lastrowid will be returned.
-      
+
 **Returns:**
 
 *  ``arRes``
 
    / *Type*: list /
 
    List of reponse data (or lastrowid if bReturnInsertedID is set).
@@ -228,15 +228,15 @@
       c = self.con.cursor()
       c.execute(command,values)
       if bHasResponse:
          arRes = c.fetchall()
       elif bReturnInsertedID:
          arRes = c.lastrowid
       c.close()
-      return arRes     
+      return arRes
 
    def __vExecMany(self, command, values=None):
       """
 Execute a query for bulk insert of many elements. No response expected.
 
 **Arguments:**
 
@@ -245,69 +245,69 @@
    / *Condition*: required / *Type*: str /
 
    Query need to be executed.
 
 *  ``values``
 
    / *Condition*: optional / *Type*: list / *Default*: None /
-   
+
    Sequence of parameters to be used with the query.
-      
+
 **Returns:**
 
-(*no returns*)      
+(*no returns*)
       """
       c = self.con.cursor()
       c.executemany(command,values)
       c.close()
-      
+
    def __nGetLastInsertID(self, tbl):
       """
 Return the last_insert_id of a given table.
 
 **Arguments:**
 
 *  ``tbl``
 
    / *Condition*: required / *Type*: str /
-   
+
    Table name to get the last_insert_id.
-      
+
 **Returns:**
 
 *  ``res``
 
    / *Type*: str /
 
-   The last_insert_id.      
+   The last_insert_id.
       """
-      # "select last_insert_id from table" returns as result a one column table 
-      # where the number of rows is the length of the full table. 
+      # "select last_insert_id from table" returns as result a one column table
+      # where the number of rows is the length of the full table.
       # Each row has the same value of the last_insert_id.
-      # This causes dramatic performance problems. 
+      # This causes dramatic performance problems.
       # Anyhow we need only one element, therefore we limit here to 1
       sql = """select last_insert_id() from """ + self.db + "." + tbl + " limit 1"
       res = self.__arExec(sql,bHasResponse=True)[0][0]
       return res
-       
+
    def sCreateNewTestResult(self, _tbl_prj_project,
                                   _tbl_prj_variant,
                                   _tbl_prj_branch,
                                   _tbl_test_result_id,
                                   _tbl_result_interpretation,
                                   _tbl_result_time_start,
                                   _tbl_result_time_end,
                                   _tbl_result_version_sw_target,
                                   _tbl_result_version_sw_test,
                                   _tbl_result_version_target,
                                   _tbl_result_jenkinsurl,
                                   _tbl_result_reporting_qualitygate
                             ):
       """
-Creates a new test result in ``tbl_result``. This is the main table which is 
+Creates a new test result in ``tbl_result``. This is the main table which is
 linked to all other data by means of ``test_result_id``.
 
 **Arguments:**
 
 *  ``_tbl_prj_project``
 
    / *Condition*: required / *Type*: str /
@@ -375,58 +375,58 @@
    Jenkinsurl in case test result is executed by jenkins.
 
 *  ``_tbl_result_reporting_qualitygate``
 
    / *Condition*: required / *Type*: str /
 
    Qualitygate information for reporting.
-      
+
 **Returns:**
 
 *  ``_tbl_test_result_id``
 
    / *Type*: str /
 
    ``test_result_id`` of new test result.
       """
-      sql,sqlval = """select count(*) from """ + self.db + """.tbl_prj where 
+      sql,sqlval = """select count(*) from """ + self.db + """.tbl_prj where
                (project=%s and variant=%s and branch=%s)""", (_tbl_prj_project,
                                                               _tbl_prj_variant,
                                                               _tbl_prj_branch)
       res = self.__arExec(sql,sqlval,True)[0][0]
       if res == 0:
-         sql,sqlval = """insert into """ + self.db + """.tbl_prj 
+         sql,sqlval = """insert into """ + self.db + """.tbl_prj
          ( variant,project, branch) values (%s, %s, %s)""" , (_tbl_prj_variant,
                                                               _tbl_prj_project,
                                                               _tbl_prj_branch)
-         self.__arExec(sql,sqlval) 
-         
-      sql,sqlval = """insert into """ + self.db + """.tbl_result (test_result_id, 
-         variant,project,branch, time_start,time_end, version_sw_target, 
-         version_sw_test,version_hardware,jenkinsurl,reporting_qualitygate,result_state) 
+         self.__arExec(sql,sqlval)
+
+      sql,sqlval = """insert into """ + self.db + """.tbl_result (test_result_id,
+         variant,project,branch, time_start,time_end, version_sw_target,
+         version_sw_test,version_hardware,jenkinsurl,reporting_qualitygate,result_state)
          values (%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s)""" , (_tbl_test_result_id,
                                                             _tbl_prj_variant,
                                                             _tbl_prj_project,
                                                             _tbl_prj_branch,
                                                             _tbl_result_time_start,
                                                             _tbl_result_time_end,
                                                             _tbl_result_version_sw_target,
                                                             _tbl_result_version_sw_test,
                                                             _tbl_result_version_target,
                                                             _tbl_result_jenkinsurl,
                                                             _tbl_result_reporting_qualitygate,
                                                             "in progress")
-      self.__arExec(sql,sqlval) 
-      
+      self.__arExec(sql,sqlval)
+
       if _tbl_result_interpretation!='':
-         sql,sqlval = """update """ + self.db + """.tbl_result set interpretation=%s 
+         sql,sqlval = """update """ + self.db + """.tbl_result set interpretation=%s
             where test_result_id='""" + _tbl_test_result_id + "'", (_tbl_result_interpretation,)
-         self.__arExec(sql,sqlval)  
-         
-      return _tbl_test_result_id                           
+         self.__arExec(sql,sqlval)
+
+      return _tbl_test_result_id
 
    def nCreateNewFile(self,_tbl_file_name,
                            _tbl_file_tester_account,
                            _tbl_file_tester_machine,
                            _tbl_file_time_start,
                            _tbl_file_time_end,
                            _tbl_test_result_id,
@@ -473,62 +473,62 @@
    UUID of test result for linking to `tbl_result` table.
 
 *  ``_tbl_file_origin``
 
    / *Condition*: required / *Type*: str /
 
    Origin (test framework) of test file. Deafult is "ROBFW"
-      
+
 **Returns:**
 
 *  ``iInsertedID``
-   
+
    / *Type*: int /
-   
+
    ID of new entry.
       """
       sql,sqlval ="""insert into """ + self.db + """.tbl_file (name,tester_account,
-                     tester_machine,time_start,time_end,test_result_id,origin) 
+                     tester_machine,time_start,time_end,test_result_id,origin)
                      values (%s,%s,%s,%s,%s,%s,%s)""" , ( _tbl_file_name,
                                                          _tbl_file_tester_account,
                                                          _tbl_file_tester_machine,
                                                          _tbl_file_time_start,
                                                          _tbl_file_time_end,
                                                          _tbl_test_result_id,
-                                                         _tbl_file_origin) 
-      iInsertedID = self.__arExec(sql,sqlval, bReturnInsertedID=True)                                                                                                      
+                                                         _tbl_file_origin)
+      iInsertedID = self.__arExec(sql,sqlval, bReturnInsertedID=True)
       return iInsertedID
 
    def vCreateNewHeader(self, _tbl_file_id,
                               _tbl_header_testtoolconfiguration_testtoolname,
                               _tbl_header_testtoolconfiguration_testtoolversionstring,
                               _tbl_header_testtoolconfiguration_projectname,
                               _tbl_header_testtoolconfiguration_logfileencoding,
                               _tbl_header_testtoolconfiguration_pythonversion,
                               _tbl_header_testtoolconfiguration_testfile,
                               _tbl_header_testtoolconfiguration_logfilepath,
                               _tbl_header_testtoolconfiguration_logfilemode,
                               _tbl_header_testtoolconfiguration_ctrlfilepath,
                               _tbl_header_testtoolconfiguration_configfile,
                               _tbl_header_testtoolconfiguration_confname,
-                              
+
                               _tbl_header_testfileheader_author,
                               _tbl_header_testfileheader_project,
                               _tbl_header_testfileheader_testfiledate,
                               _tbl_header_testfileheader_version_major,
                               _tbl_header_testfileheader_version_minor,
                               _tbl_header_testfileheader_version_patch,
                               _tbl_header_testfileheader_keyword,
                               _tbl_header_testfileheader_shortdescription,
                               _tbl_header_testexecution_useraccount,
                               _tbl_header_testexecution_computername,
-                              
+
                               _tbl_header_testrequirements_documentmanagement,
                               _tbl_header_testrequirements_testenvironment,
-                              
+
                               _tbl_header_testbenchconfig_name,
                               _tbl_header_testbenchconfig_data,
                               _tbl_header_preprocessor_filter,
                               _tbl_header_preprocessor_parameters ):
       """
 Create a new header entry in ``tbl_file_header`` table which is linked with the file.
 
@@ -697,54 +697,54 @@
    Preprocessor filter information.
 
 *  ``_tbl_header_preprocessor_parameters``
 
    / *Condition*: required / *Type*: str /
 
    Preprocessor parameters definition.
-      
+
 **Returns:**
 
 (*no returns*)
-      """   
-      sql,sqlval ="""insert into """ + self.db + """.tbl_file_header 
+      """
+      sql,sqlval ="""insert into """ + self.db + """.tbl_file_header
                         ( file_id,
                           testtoolconfiguration_testtoolname,
                           testtoolconfiguration_testtoolversionstring,
                           testtoolconfiguration_projectname,
                           testtoolconfiguration_logfileencoding,
                           testtoolconfiguration_pythonversion,
                           testtoolconfiguration_testfile,
                           testtoolconfiguration_logfilepath,
                           testtoolconfiguration_logfilemode,
                           testtoolconfiguration_ctrlfilepath,
                           testtoolconfiguration_configfile,
                           testtoolconfiguration_confname,
-                          
+
                           testfileheader_author,
                           testfileheader_project,
                           testfileheader_testfiledate,
                           testfileheader_version_major,
                           testfileheader_version_minor,
                           testfileheader_version_patch,
                           testfileheader_keyword,
                           testfileheader_shortdescription,
                           testexecution_useraccount,
                           testexecution_computername,
-                          
+
                           testrequirements_documentmanagement,
                           testrequirements_testenvironment,
-                          
+
                           testbenchconfig_name,
                           testbenchconfig_data,
-                          preprocessor_filter, 
-                          preprocessor_parameters) 
-                  values ( %s, %s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s, %s, 
+                          preprocessor_filter,
+                          preprocessor_parameters)
+                  values ( %s, %s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s, %s,
                            %s, %s, %s,%s,%s,%s,%s,%s,%s,%s,%s,%s)""" , \
-                        ( _tbl_file_id, 
+                        ( _tbl_file_id,
                           _tbl_header_testtoolconfiguration_testtoolname,
                           _tbl_header_testtoolconfiguration_testtoolversionstring,
                           _tbl_header_testtoolconfiguration_projectname,
                           _tbl_header_testtoolconfiguration_logfileencoding,
                           _tbl_header_testtoolconfiguration_pythonversion,
                           _tbl_header_testtoolconfiguration_testfile,
                           _tbl_header_testtoolconfiguration_logfilepath,
@@ -766,17 +766,17 @@
 
                           _tbl_header_testrequirements_documentmanagement,
                           _tbl_header_testrequirements_testenvironment,
 
                           _tbl_header_testbenchconfig_name,
                           _tbl_header_testbenchconfig_data,
                           _tbl_header_preprocessor_filter,
-                          _tbl_header_preprocessor_parameters) 
-      self.__arExec(sql,sqlval)                                                                       
-   
+                          _tbl_header_preprocessor_parameters)
+      self.__arExec(sql,sqlval)
+
    def nCreateNewSingleTestCase(self,
                                 _tbl_case_name,
                                 _tbl_case_issue,
                                 _tbl_case_tcid,
                                 _tbl_case_fid,
                                 _tbl_case_testnumber,
                                 _tbl_case_repeatcount,
@@ -831,15 +831,15 @@
 
    Test case repeatition count.
 
 *  ``_tbl_case_component``
 
    / *Condition*: required / *Type*: str /
 
-   Component which test case is belong to. 
+   Component which test case is belong to.
 
 *  ``_tbl_case_time_start``
 
    / *Condition*: required / *Type*: str /
 
    Test case start time as format ``%Y-%m-%d %H:%M:%S``.
 
@@ -873,34 +873,34 @@
 
    Traceback information when test case is failed.
 
 *  ``_tbl_test_result_id``
 
    / *Condition*: required / *Type*: str /
 
-   UUID of test result for linking to file in ``tbl_result`` table. 
+   UUID of test result for linking to file in ``tbl_result`` table.
 
 *  ``_tbl_file_id``
 
    / *Condition*: required / *Type*: int /
 
-   Test file ID for linking to file in ``tbl_file`` table. 
-      
+   Test file ID for linking to file in ``tbl_file`` table.
+
 **Returns:**
 
 *  ``iInsertedID``
-   
+
    / *Type*: int /
-   
+
    ID of new entry.
       """
       if _tbl_case_lastlog == "":
          _tbl_case_lastlog = None
-      sql = """insert into """ + self.db + """.tbl_case (name, issue, tcid, fid, 
-               testnumber, repeatcount, component, time_start, result_main, result_state, 
+      sql = """insert into """ + self.db + """.tbl_case (name, issue, tcid, fid,
+               testnumber, repeatcount, component, time_start, result_main, result_state,
                result_return, counter_resets, lastlog, test_result_id, file_id)
                values (%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s)"""
       sqlval = (_tbl_case_name,
                 _tbl_case_issue,
                 _tbl_case_tcid,
                 _tbl_case_fid,
                 _tbl_case_testnumber,
@@ -916,16 +916,16 @@
                 _tbl_file_id
                )
       iInsertedTestID = self.__arExec(sql, sqlval, bReturnInsertedID=True)
       return iInsertedTestID
 
    #
    # create a new test case entry:
-   # 
-   #         
+   #
+   #
    def nCreateNewTestCase(self,
                           _tbl_case_name,
                           _tbl_case_issue,
                           _tbl_case_tcid,
                           _tbl_case_fid,
                           _tbl_case_testnumber,
                           _tbl_case_repeatcount,
@@ -982,15 +982,15 @@
 
    Test case repeatition count.
 
 *  ``_tbl_case_component``
 
    / *Condition*: required / *Type*: str /
 
-   Component which test case is belong to. 
+   Component which test case is belong to.
 
 *  ``_tbl_case_time_start``
 
    / *Condition*: required / *Type*: str /
 
    Test case start time as format ``%Y-%m-%d %H:%M:%S``.
 
@@ -1024,22 +1024,22 @@
 
    Traceback information when test case is failed.
 
 *  ``_tbl_test_result_id``
 
    / *Condition*: required / *Type*: str /
 
-   UUID of test result for linking to file in `tbl_result` table. 
+   UUID of test result for linking to file in `tbl_result` table.
 
 *  ``_tbl_file_id``
 
    / *Condition*: required / *Type*: int /
 
-   Test file ID for linking to file in ``tbl_file`` table. 
-      
+   Test file ID for linking to file in ``tbl_file`` table.
+
 **Returns:**
 
 (*no returns*)
       """
       if _tbl_case_lastlog == "":
          _tbl_case_lastlog = None
       sqlval = (_tbl_case_name,
@@ -1052,24 +1052,24 @@
                 _tbl_case_time_start,
                 _tbl_case_result_main,
                 _tbl_case_result_state,
                 _tbl_case_result_return,
                 _tbl_case_counter_resets,
                 _tbl_test_result_id,
                 _tbl_file_id,
-                _tbl_case_lastlog,                
-                )         
+                _tbl_case_lastlog,
+                )
       self.lTestCases.append(sqlval)
       if len(self.lTestCases) >= CDataBase.__NUM_BUFFERD_ELEMENTS_FOR_EXECUTEMANY:
          self.vEnableForeignKeyCheck(False)
          self.__vUploadTestCaseListToDb(self.lTestCases)
          self.vEnableForeignKeyCheck(True)
          # Clear test cases list
          self.lTestCases = []
-   
+
    def __vUploadTestCaseListToDb(self, lTestCases):
       """
 Bulk insert test case results.
 
 **Arguments:**
 
 *  ``lTestCases``
@@ -1078,20 +1078,20 @@
 
    List of test case for creation.
 
 **Returns:**
 
 (*no returns*)
       """
-      sql = """insert into """ + self.db + """.tbl_case (name, issue, tcid, fid, 
-            testnumber, repeatcount, component, time_start, result_main, result_state, 
-            result_return, counter_resets, test_result_id, file_id, lastlog) 
+      sql = """insert into """ + self.db + """.tbl_case (name, issue, tcid, fid,
+            testnumber, repeatcount, component, time_start, result_main, result_state,
+            result_return, counter_resets, test_result_id, file_id, lastlog)
             values (%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s)"""
       self.__vExecMany(sql, lTestCases)
-       
+
    def vCreateTags(self, _tbl_test_result_id, _tbl_usr_result_tags):
       """
 Create tag entries.
 
 **Arguments:**
 
 *  ``_tbl_test_result_id``
@@ -1106,18 +1106,18 @@
 
    User tags information.
 
 **Returns:**
 
 (*no returns*)
       """
-      sql,sqlval="""insert into """ + self.db + """.tbl_usr_result (test_result_id, tags) 
+      sql,sqlval="""insert into """ + self.db + """.tbl_usr_result (test_result_id, tags)
                     values (%s,%s)""", (_tbl_test_result_id , _tbl_usr_result_tags)
-      self.__arExec(sql,sqlval) 
-   
+      self.__arExec(sql,sqlval)
+
    def vSetCategory(self, _tbl_test_result_id, tbl_result_category_main):
       """
 Create category entry.
 
 **Arguments:**
 
 *  ``_tbl_test_result_id``
@@ -1135,16 +1135,16 @@
 **Returns:**
 
 (*no returns*)
       """
       sql="""update """ + self.db + """.tbl_result set category_main='""" + \
                   tbl_result_category_main + """' where test_result_id='""" + \
                   _tbl_test_result_id + "'"
-      self.__arExec(sql)  
-        
+      self.__arExec(sql)
+
    def vUpdateStartEndTime(self, _tbl_test_result_id, _tbl_result_time_start, _tbl_result_time_end):
       """
 Create start-end time entry.
 
 **Arguments:**
 
 *  ``_tbl_test_result_id``
@@ -1165,45 +1165,45 @@
 
    Result end time as format ``%Y-%m-%d %H:%M:%S``.
 
 **Returns:**
 
 (*no returns*)
       """
-      sql,sqlval="""update """ + self.db + """.tbl_result set time_start=%s, time_end=%s 
+      sql,sqlval="""update """ + self.db + """.tbl_result set time_start=%s, time_end=%s
                   where test_result_id='""" + _tbl_test_result_id + "'" , \
                   (_tbl_result_time_start, _tbl_result_time_end)
-      self.__arExec(sql,sqlval)         
-        
+      self.__arExec(sql,sqlval)
+
    def arGetCategories(self):
       """
 Get existing categories.
 
 **Arguments:**
 
 (*no arguments*)
 
 **Returns:**
 
 *  ``arCategories``
 
    / *Type*: list /
-   
+
    List of exsiting categories.
       """
       sql="""select category from """ + self.db + """.tbl_result_categories"""
       res=self.__arExec(sql, bHasResponse=True)
       arCategories=[]
       for cat in res:
-         arCategories.append(cat[0])       
+         arCategories.append(cat[0])
       return arCategories
-    
+
    #
    # create abort reason entry
-   #    
+   #
    def vCreateAbortReason(self,
                           _tbl_test_result_id,
                           _tbl_abort_reason,
                           _tbl_abort_message
                            ):
       """
 Create abort reason entry.
@@ -1228,22 +1228,22 @@
 
    Detail message of abort.
 
 **Returns:**
 
 (*no returns*)
       """
-      sql,sqlval = """insert into """ + self.db + """.tbl_abort 
+      sql,sqlval = """insert into """ + self.db + """.tbl_abort
                            (test_result_id, abort_reason, msg_detail)
                            values (%s,%s,%s)""" , (_tbl_test_result_id,
                                                    _tbl_abort_reason,
                                                    _tbl_abort_message,
-                                                   )                         
-      self.__arExec(sql,sqlval)      
-   
+                                                   )
+      self.__arExec(sql,sqlval)
+
    def vCreateReanimation(self, _tbl_test_result_id, _tbl_num_of_reanimation):
       """
 Create reanimation entry.
 
 **Arguments:**
 
 *  ``_tbl_test_result_id``
@@ -1258,15 +1258,15 @@
 
    Counter of target reanimation during execution.
 
 **Returns:**
 
 (*no returns*)
       """
-      sql, sqlval = """update """ + self.db + """.tbl_result set num_of_reanimation=%s where 
+      sql, sqlval = """update """ + self.db + """.tbl_result set num_of_reanimation=%s where
                         test_result_id='""" + _tbl_test_result_id + "'", (_tbl_num_of_reanimation)
       self.__arExec(sql, sqlval)
 
    def vCreateCCRdata(self, _tbl_test_case_id, lCCRdata):
       """
 Create CCR data per test case.
 
@@ -1286,15 +1286,15 @@
 
 **Returns:**
 
 (*no returns*)
       """
       sql = """insert into """ + self.db + """.tbl_ccr (test_case_id, timestamp, MEM, CPU) values(%s,%s,%s,%s)"""
       sqlVals = []
-      for row in lCCRdata: 
+      for row in lCCRdata:
          row.insert(0, _tbl_test_case_id)
          sqlVals.append(tuple(row))
       self.__vExecMany(sql, sqlVals)
 
    def vFinishTestResult(self,_tbl_test_result_id):
       """
 Finish upload:
@@ -1314,33 +1314,33 @@
 
 (*no returns*)
       """
       if len(self.lTestCases) > 0:
          self.vEnableForeignKeyCheck(False)
          self.__vUploadTestCaseListToDb(self.lTestCases)
          self.vEnableForeignKeyCheck(True)
-      sql="""update """ + self.db + """.tbl_result set result_state="new report" 
+      sql="""update """ + self.db + """.tbl_result set result_state="new report"
                   where test_result_id='""" + _tbl_test_result_id + "'"
-      self.__arExec(sql)  
-          
+      self.__arExec(sql)
+
    def vUpdateEvtbls(self):
       """
 Call ``update_evtbls`` stored procedure.
 
 **Arguments:**
 
 (*no arguments*)
 
 **Returns:**
 
 (*no returns*)
       """
-      sql="""call """ + self.db + """.update_evtbls();""" 
-      self.__arExec(sql)   
- 
+      sql="""call """ + self.db + """.update_evtbls();"""
+      self.__arExec(sql)
+
    def vUpdateEvtbl(self, _tbl_test_result_id):
       """
 Call ``update_evtbl`` stored procedure to update provided ``test_result_id``.
 
 **Arguments:**
 
 *  ``_tbl_test_result_id``
@@ -1350,16 +1350,16 @@
    UUID of test result.
 
 **Returns:**
 
 (*no returns*)
       """
       sql="""call """ + self.db + """.update_evtbl('%s');"""%_tbl_test_result_id
-      self.__arExec(sql)  
-  
+      self.__arExec(sql)
+
    def vEnableForeignKeyCheck(self, enable=True):
       """
 Switch ``foreign_key_checks`` flag.
 
 **Arguments:**
 
 *  ``enable``
@@ -1369,16 +1369,16 @@
    If True, enable foreign key constraint.
 
 **Returns:**
 
 (*no returns*)
       """
       sql = "SET FOREIGN_KEY_CHECKS=%s;" %str(int(enable))
-      self.__arExec(sql)        
-       
+      self.__arExec(sql)
+
    def sGetLatestFileID(self, _tbl_test_result_id):
       """
 Get latest file ID from ``tbl_file`` table.
 
 **Arguments:**
 
 *  ``_tbl_test_result_id``
@@ -1444,30 +1444,30 @@
 
 **Returns:**
 
 (*no returns*)
       """
       sql = "UPDATE %s.tbl_result SET time_end='%s' WHERE test_result_id='%s'"%(self.db, _tbl_result_time_end, _tbl_test_result_id)
       self.__arExec(sql)
-   
+
    def bExistingResultID(self, _tbl_test_result_id):
       """
 Verify the given test result UUID is existing in ``tbl_result`` table or not.
 
 **Arguments:**
 
 *  ``_tbl_test_result_id``
 
    / *Condition*: required / *Type*: str /
 
    Result UUID to be verified.
 
 **Returns:**
 
-*  ``bExisting`` 
+*  ``bExisting``
 
    / *Type*: bool /
 
    True if test result UUID is already existing.
       """
       sql = "SELECT test_result_id FROM %s.tbl_result WHERE test_result_id='%s'"%(self.db, _tbl_test_result_id)
       res = self.__arExec(sql, bHasResponse=True)
@@ -1494,9 +1494,9 @@
 
    None if test result UUID is not existing, else the tuple which contains project and version_sw: (project, variant) is returned.
       """
       sql = "SELECT project, version_sw_target FROM %s.tbl_result WHERE test_result_id='%s'"%(self.db, _tbl_test_result_id)
       res = self.__arExec(sql, bHasResponse=True)
       if res and len(res)>0:
          return res[0]
-      
-      return None
+
+      return None
```

### Comparing `robotframework-robotlog2db-1.3.7/RobotLog2DB/RobotLog2DB.pdf` & `robotframework-robotlog2db-1.3.8/RobotLog2DB/RobotLog2DB.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 6% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 RobotLog2DB
-v. 1.3.7
+v. 1.3.8
 Tran Duy Ngoan
-14.06.2023
+21.06.2023
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -2115,19 +2115,19 @@
 
 Name
 
 RobotLog2DB
 
 Version
 
-1.3.7
+1.3.8
 
 Date
 
-14.06.2023
+21.06.2023
 
 Description
 
 Imports robot result(s) to TestResultWebApp database
 
 Package URL
 
@@ -2251,14 +2251,20 @@
 
 Update README with new instruction for installation and image’s links
 
 32
 
 CHAPTER 6. HISTORY
 
+1.3.8
+
+21.06.2023
+
+Fix issue with suite.starttime at root suite is N/A
+
 RobotLog2DB.pdf
-Created at 14.06.2023 - 08:58:27
+Created at 21.06.2023 - 11:40:49
 by GenPackageDoc v. 0.40.3
 
 33
```

### Comparing `robotframework-robotlog2db-1.3.7/RobotLog2DB/__init__.py` & `robotframework-robotlog2db-1.3.8/RobotLog2DB/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2023 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
-#  limitations under the License.
+#  limitations under the License.
```

### Comparing `robotframework-robotlog2db-1.3.7/RobotLog2DB/__main__.py` & `robotframework-robotlog2db-1.3.8/RobotLog2DB/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2023 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,8 +10,8 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from .robotlog2db import RobotLog2DB
 
 if __name__ == "__main__":
-   RobotLog2DB()
+   RobotLog2DB()
```

### Comparing `robotframework-robotlog2db-1.3.7/RobotLog2DB/robotlog2db.py` & `robotframework-robotlog2db-1.3.8/RobotLog2DB/robotlog2db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2020-2022 Robert Bosch Car Multimedia GmbH
+#  Copyright 2020-2023 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,28 +15,28 @@
 #
 # File: robotlog2db.py
 #
 # Initialy created by Tran Duy Ngoan(RBVH/ECM11) / November 2020
 #
 # This tool is used to parse the robot framework results output.xml
 # then import them into TestResultWebApp's database
-#  
+#
 # History:
-# 
+#
 # 2020-11-26:
 #  - initial version
 #
 # 2021-05-20:
 #  - Correct regex for tags and testtool.
 #  - Add file description information as suite.doc.
 #  - Add new command line arguments:
 #    + -UUID: to specify the uuid of test result.
 #    + --variant: to specify project/variant of test result.
 #    + --versions: to specify versions information (Software;Hardware;Test)
-#    + --config: configuration(component, variant, version_sw) json file for 
+#    + --config: configuration(component, variant, version_sw) json file for
 #                the import.
 #  - Try to extract metadata from suites incase many suite levels in result.
 #
 # 2023-02-28:
 #  - Rename key to 'components' in configuration json file (--config).
 #
 # ******************************************************************************
@@ -163,34 +163,34 @@
    Color style for the message.
 
 *  ``indent``
 
    / *Condition*: optional / *Type*: int / *Default*: 0 /
 
    Offset indent.
-      
+
 **Returns:**
 
 (*no returns*)
       """
       if color==None:
          color = cls.color_normal
       if cls.output_console:
-         print(cls.prefix_all + cls.color_reset + color + " "*indent + msg + 
+         print(cls.prefix_all + cls.color_reset + color + " "*indent + msg +
                cls.color_reset)
       if cls.output_logfile!=None and os.path.isfile(cls.output_logfile):
          with open(cls.output_logfile, 'a') as f:
             f.write(" "*indent + msg)
       return
 
    @classmethod
    def log_warning(cls, msg):
       """
 Write warning message to console/file output.
-      
+
 **Arguments:**
 
 *  ``msg``
 
    / *Condition*: required / *Type*: str /
 
    Warning message which is written to output.
@@ -238,21 +238,21 @@
 Collect all valid Robot xml result file in given path.
 
 **Arguments:**
 
 *  ``path``
 
    / *Condition*: required / *Type*: str /
-   
+
    Path to Robot result folder or file to be searched.
 
 *  ``search_recursive``
 
    / *Condition*: optional / *Type*: bool / *Default*: False /
-   
+
    If set, the given path is searched recursively for xml result files.
 
 **Returns:**
 
 *  ``lFoundFiles``
 
    / *Type*: list /
@@ -296,27 +296,27 @@
 Verify the given xml result file is valid or not.
 
 **Arguments:**
 
 *  ``xml_result``
 
    / *Condition*: required / *Type*: str /
-   
+
    Path to Robot result file.
 
 *  ``xsd_schema``
 
    / *Condition*: optional / *Type*: str / *Default*: <installed_folder>\/xsd\/robot.xsd /
-   
+
    Path to Robot schema *.xsd file.
 
 *  ``exit_on_failure``
 
    / *Condition*: optional / *Type*: bool / *Default*: True /
-   
+
    If set, exit with fatal error if the schema validation of given xml file failed.
 
 **Returns:**
 
 *  / *Type*: bool /
 
    True if the given xml result is valid with the provided schema *.xsd.
@@ -343,21 +343,21 @@
 Verify the given UUID is valid or not.
 
 **Arguments:**
 
 *  ``uuid_to_test``
 
    / *Condition*: required / *Type*: str /
-   
+
    UUID to be verified.
 
 *  ``version``
 
    / *Condition*: optional / *Type*: int / *Default*: 4 /
-   
+
    UUID version.
 
 **Returns:**
 
 *  ``bValid``
 
    / *Type*: bool /
@@ -365,18 +365,18 @@
    True if the given UUID is valid.
    """
    bValid = False
    try:
       uuid_obj = uuid.UUID(uuid_to_test, version=version)
    except:
       return bValid
-   
+
    if str(uuid_obj) == uuid_to_test:
       bValid = True
-   
+
    return bValid
 
 def is_valid_config(dConfig, dSchema=CONFIG_SCHEMA, bExitOnFail=True):
    """
 Validate the json configuration base on given schema.
 
 Default schema supports below information:
@@ -430,31 +430,31 @@
                bValid = False
          # Fixed type
          else:
             if type(dConfig[key]) != dSchema[key]:
                bValid = False
 
          if not bValid:
-            Logger.log_error(f"Value of '{key}' has wrong type '{type(dConfig[key])}' in configuration json file.", 
+            Logger.log_error(f"Value of '{key}' has wrong type '{type(dConfig[key])}' in configuration json file.",
                              fatal_error=bExitOnFail)
             break
 
       else:
          bValid = False
-         Logger.log_error(f"Information '{key}' is not supported in configuration json file.", 
+         Logger.log_error(f"Information '{key}' is not supported in configuration json file.",
                           fatal_error=bExitOnFail)
          break
-   
+
    return bValid
 
 def get_from_tags(lTags, reInfo):
    """
 Extract testcase information from tags.
 
-Example: 
+Example:
    ``TCID-xxxx``, ``FID-xxxx``, ...
 
 **Arguments:**
 
 *  ``lTags``
 
    / *Condition*: required / *Type*: list /
@@ -468,15 +468,15 @@
    Regex to get the expectated info (ID) from tag info.
 
 **Returns:**
 
 *  ``lInfo``
 
    / *Type*: list /
-   
+
    List of expected information (ID)
    """
    lInfo = []
    if len(lTags) != 0:
       for tag in lTags:
          oMatch = re.search(reInfo, tag, re.I)
          if oMatch:
@@ -485,26 +485,26 @@
 
 def get_branch_from_swversion(sw_version):
    """
 Get branch name from software version information.
 
 Convention of branch information in suffix of software version:
 
-*  All software version with .0F is the main/freature branch. 
+*  All software version with .0F is the main/freature branch.
    The leading number is the current year. E.g. ``17.0F03``
-*  All software version with ``.1S``, ``.2S``, ... is a stabi branch. 
+*  All software version with ``.1S``, ``.2S``, ... is a stabi branch.
    The leading number is the year of branching out for stabilization.
    The number before "S" is the order of branching out in the year.
-   
+
 **Arguments:**
 
 *  ``sw_version``
 
    / *Condition*: required / *Type*: str /
-   
+
    Software version.
 
 **Returns:**
 
 *  ``branch_name``
 
    / *Type*: str /
@@ -537,16 +537,19 @@
 
 *  ``sFormatedTime``
 
    / *Type*: str /
 
    TestResultWebApp's time as format ``%Y-%m-%d %H:%M:%S``.
    """
-
-   sFormatedTime = sTime[0:4]+"-"+sTime[4:6]+"-"+sTime[6:]
+   try:
+      sFormatedTime = sTime[0:4]+"-"+sTime[4:6]+"-"+sTime[6:]
+   except Exception as reason:
+      Logger.log_error(f"Cannot convert given time '{sTime}' to TestResultWebApp's time format.\nReason: {reason}",
+                        fatal_error=True)
    return sFormatedTime
 
 def __process_commandline():
    """
 Process provided argument(s) from command line.
 
 Avalable arguments in command line:
@@ -577,52 +580,52 @@
    """
    PROG_NAME = "RobotLog2DB (RobotXMLResult to TestResultWebApp importer)"
    PROG_DESC = "RobotLog2DB imports XML result files (default: output.xml) "+\
                "generated by the Robot Framework into a WebApp database."
 
    cmdParser = argparse.ArgumentParser(prog=PROG_NAME, description=PROG_DESC)
 
-   cmdParser.add_argument('-v', '--version', action='version', 
+   cmdParser.add_argument('-v', '--version', action='version',
                            version=f'v{VERSION} ({VERSION_DATE})',
                            help='version of the RobotLog2DB importer.')
-   cmdParser.add_argument('resultxmlfile', type=str, 
+   cmdParser.add_argument('resultxmlfile', type=str,
                            help='absolute or relative path to the result file or directory of result files to be imported.')
-   cmdParser.add_argument('server', type=str, 
+   cmdParser.add_argument('server', type=str,
                            help='server which hosts the database (IP or URL).')
-   cmdParser.add_argument('user', type=str, 
+   cmdParser.add_argument('user', type=str,
                            help='user for database login.')
-   cmdParser.add_argument('password', type=str, 
+   cmdParser.add_argument('password', type=str,
                            help='password for database login.')
-   cmdParser.add_argument('database', type=str, 
+   cmdParser.add_argument('database', type=str,
                            help='database schema for database login.')
-   cmdParser.add_argument('--recursive', action="store_true", 
+   cmdParser.add_argument('--recursive', action="store_true",
                            help='if set, then the path is searched recursively for output files to be imported.')
-   cmdParser.add_argument('--dryrun', action="store_true", 
+   cmdParser.add_argument('--dryrun', action="store_true",
                            help='if set, then verify all input arguments (includes DB connection) and show what would be done.')
-   cmdParser.add_argument('--append', action="store_true", 
+   cmdParser.add_argument('--append', action="store_true",
                            help='is used in combination with --UUID <UUID>.'+\
                                 'If set, allow to append new result(s) to existing execution result UUID in --UUID argument.')
-   cmdParser.add_argument('--UUID', type=str, 
+   cmdParser.add_argument('--UUID', type=str,
                            help='UUID used to identify the import and version ID on webapp. '+\
                                 'If not provided RobotLog2DB will generate an UUID for the whole import.')
-   cmdParser.add_argument('--variant', type=str, 
+   cmdParser.add_argument('--variant', type=str,
                            help='variant name to be set for this import.')
-   cmdParser.add_argument('--versions', type=str, 
+   cmdParser.add_argument('--versions', type=str,
                            help='metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).')
-   cmdParser.add_argument('--config', type=str, 
+   cmdParser.add_argument('--config', type=str,
                            help='configuration json file for component mapping information.')
 
    return cmdParser.parse_args()
 
 def process_suite_metadata(suite, default_metadata=DEFAULT_METADATA):
    """
 Try to find metadata information from all suite levels.
 
 Metadata at top suite level has a highest priority.
-   
+
 **Arguments:**
 
 *  ``suite``
 
    / *Condition*: required / *Type*: `TestSuite` object /
 
    Robot suite object.
@@ -644,15 +647,15 @@
    dMetadata = dict(default_metadata)
    # Try to get metadata from first child of suite - multiple log files
    if suite.suites != None and len(list(suite.suites)) > 0:
       dMetadata = process_suite_metadata(suite.suites[0], dMetadata)
    # The higher suite level metadata have higher priority
    if suite.metadata != None:
       dMetadata = process_metadata(suite.metadata, dMetadata)
-   
+
    return dMetadata
 
 def process_metadata(metadata, default_metadata=DEFAULT_METADATA):
    """
 Extract metadata from suite result bases on DEFAULT_METADATA.
 
 **Arguments:**
@@ -668,18 +671,18 @@
    / *Condition*: optional / *Type*: dict / *Default*: DEFAULT_METADATA /
 
    Initial Metadata information for updating.
 
 **Returns:**
 
 *  ``dMetadata``
-   
+
    / *Type*: dict /
-   
-   Dictionary of Metadata information.  
+
+   Dictionary of Metadata information.
    """
    dMetadata = dict(default_metadata)
    for key in dMetadata.keys():
       if key in metadata:
          if metadata[key] != None:
             dMetadata[key] = metadata[key]
 
@@ -722,19 +725,19 @@
 
    / *Condition*: required / *Type*: dict / *Default*: None /
 
    Configuration data which is parsed from given json configuration file.
 
 **Returns:**
 
-(*no returns*)  
+(*no returns*)
    """
    if len(list(suite.suites)) > 0:
       for subsuite in suite.suites:
-         process_suite(db, subsuite, _tbl_test_result_id, root_metadata, 
+         process_suite(db, subsuite, _tbl_test_result_id, root_metadata,
                        dConfig)
    else:
       # File metadata
       metadata_info = process_metadata(suite.metadata, root_metadata)
       _tbl_file_name = suite.source
       _tbl_file_tester_account = metadata_info['tester']
       if dConfig != None and 'tester' in dConfig:
@@ -751,47 +754,47 @@
          # process component mapping if provided in config file
          if dConfig != None and 'components' in dConfig:
             if isinstance(dConfig['components'], dict):
                for cmpt_name in dConfig['components']:
                   if isinstance(dConfig['components'][cmpt_name], list):
                      bFound = False
                      for path in dConfig['components'][cmpt_name]:
-                        if (normalize_path(path) in 
+                        if (normalize_path(path) in
                             normalize_path(_tbl_file_name)):
                            metadata_info['component'] = cmpt_name
                            bFound = True
                            break
                      if bFound:
                         break
                   elif isinstance(dConfig['components'][cmpt_name], str):
                      cmpt_path = normalize_path(dConfig['components'][cmpt_name])
                      if cmpt_path in normalize_path(_tbl_file_name):
                         metadata_info['component'] = cmpt_name
                         break
-            elif (isinstance(dConfig['components'], str) and 
+            elif (isinstance(dConfig['components'], str) and
                   dConfig['components'].strip() != ""):
                metadata_info['component'] = dConfig['components']
-      
+
       # New test file
       if not Logger.dryrun:
          try:
             _tbl_file_id = db.nCreateNewFile(_tbl_file_name,
                                              _tbl_file_tester_account,
                                              _tbl_file_tester_machine,
                                              _tbl_file_time_start,
                                              _tbl_file_time_end,
                                              _tbl_test_result_id)
          except Exception as reason:
             Logger.log_error(f"Cannot create new test file result for file '{_tbl_file_name}' in database.\nReason: {reason}",
                              fatal_error=True)
       else:
          _tbl_file_id = "file id for dryrun"
-      Logger.log(f"Created test file result for file '{_tbl_file_name}' successfully: {str(_tbl_file_id)}", 
+      Logger.log(f"Created test file result for file '{_tbl_file_name}' successfully: {str(_tbl_file_id)}",
                  indent=2)
-      
+
       _tbl_header_testtoolname    = ""
       _tbl_header_testtoolversion = ""
       _tbl_header_pythonversion   = ""
       sTestTool = metadata_info['testtool']
       if dConfig != None and 'testtool' in dConfig:
          sTestTool = dConfig['testtool']
       if sTestTool != "":
@@ -806,29 +809,29 @@
       _tbl_header_logfileencoding = "UTF-8"
       _tbl_header_testfile    = _tbl_file_name
       _tbl_header_logfilepath = ""
       _tbl_header_logfilemode = ""
       _tbl_header_ctrlfilepath= ""
       _tbl_header_configfile  = metadata_info['configfile']
       _tbl_header_confname    = ""
-   
+
       _tbl_header_author        = metadata_info['author']
       _tbl_header_project       = metadata_info['project']
       _tbl_header_testfiledate  = ""
       _tbl_header_version_major = ""
       _tbl_header_version_minor = ""
       _tbl_header_version_patch = ""
       _tbl_header_keyword       = ""
       _tbl_header_shortdescription = suite.doc
       _tbl_header_useraccount   = metadata_info['tester']
       _tbl_header_computername  = metadata_info['machine']
 
       _tbl_header_testrequirements_documentmanagement = ""
       _tbl_header_testrequirements_testenvironment    = ""
-      
+
       _tbl_header_testbenchconfig_name    = ""
       _tbl_header_testbenchconfig_data    = ""
       _tbl_header_preprocessor_filter     = ""
       _tbl_header_preprocessor_parameters = ""
 
       if not Logger.dryrun:
          try:
@@ -858,23 +861,23 @@
 
                               _tbl_header_testrequirements_documentmanagement,
                               _tbl_header_testrequirements_testenvironment,
 
                               _tbl_header_testbenchconfig_name,
                               _tbl_header_testbenchconfig_data,
                               _tbl_header_preprocessor_filter,
-                              _tbl_header_preprocessor_parameters 
+                              _tbl_header_preprocessor_parameters
                               )
          except Exception as reason:
-            Logger.log_error(f"Cannot create new test file header result for file '{_tbl_file_name}' in database.\nReason: {reason}", 
+            Logger.log_error(f"Cannot create new test file header result for file '{_tbl_file_name}' in database.\nReason: {reason}",
                              fatal_error=True)
       if len(list(suite.tests)) > 0:
          test_number = 1
          for test in suite.tests:
-            process_test(db, test, _tbl_file_id, _tbl_test_result_id, 
+            process_test(db, test, _tbl_file_id, _tbl_test_result_id,
                          metadata_info, test_number)
             test_number = test_number + 1
 
 def process_test(db, test, file_id, test_result_id, metadata_info, test_number):
    """
 Process test case data and create new test case record.
 
@@ -936,24 +939,24 @@
    if _tbl_case_component not in dComponentCounter:
       dComponentCounter[_tbl_case_component] = 0
    try:
       _tbl_case_result_main = DRESULT_MAPPING[test.status]
    except Exception:
       Logger.log_error(f"Invalid Robotframework result state '{test.status}' of test '{_tbl_case_name}'.")
       return
-   _tbl_case_result_state   = "complete" 
+   _tbl_case_result_state   = "complete"
    _tbl_case_result_return  = 11
    _tbl_case_counter_resets = 0
    try:
       _tbl_case_lastlog = base64.b64encode(test.message.encode())
    except:
       _tbl_case_lastlog = None
    _tbl_test_result_id = test_result_id
    _tbl_file_id = file_id
-   
+
    if not Logger.dryrun:
       try:
          tbl_case_id = db.nCreateNewSingleTestCase(_tbl_case_name,
                                                    _tbl_case_issue,
                                                    _tbl_case_tcid,
                                                    _tbl_case_fid,
                                                    _tbl_case_testnumber,
@@ -979,29 +982,29 @@
    Logger.log(f"Created test case result for test '{_tbl_case_name}' successfully: {str(tbl_case_id)}{component_msg}", indent=4)
 
 def process_config_file(config_file):
    """
 Parse information from configuration file:
 
 *  ``component``:
-   
+
    .. code:: python
 
       {
          "components" : {
             "componentA" : "componentA/path/to/testcase",
             "componentB" : "componentB/path/to/testcase",
             "componentC" : [
                "componentC1/path/to/testcase",
                "componentC2/path/to/testcase"
             ]
          }
       }
 
-   Then all testcases which their paths contain ``componentA/path/to/testcase`` 
+   Then all testcases which their paths contain ``componentA/path/to/testcase``
    will be belong to ``componentA``, ...
 
 *  ``variant``, ``version_sw``: configuration file has low priority than command line.
 
 **Arguments:**
 
 *  ``config_file``
@@ -1011,27 +1014,27 @@
    Path to configuration file.
 
 **Returns:**
 
 *  ``dConfig``
 
    / *Type*: dict /
-   
+
    Configuration object.
    """
 
    with open(config_file, encoding='utf-8') as f:
       try:
          dConfig = json.load(f)
       except Exception as reason:
-         Logger.log_error(f"Cannot parse the json file '{config_file}'. Reason: {reason}", 
+         Logger.log_error(f"Cannot parse the json file '{config_file}'. Reason: {reason}",
                           fatal_error=True)
 
    if not is_valid_config(dConfig, bExitOnFail=False):
-      Logger.log_error(f"Error in configuration file '{config_file}'.", 
+      Logger.log_error(f"Error in configuration file '{config_file}'.",
                        fatal_error=True)
    return dConfig
 
 def normalize_path(sPath):
    """
 Normalize path file.
 
@@ -1040,36 +1043,36 @@
 *  ``sPath``
 
    / *Condition*: required / *Type*: str /
 
    Path file to be normalized.
 
 *  ``sNPath``
-   
+
    / *Type*: str /
-   
+
    Normalized path file.
    """
    if sPath.strip()=='':
       return ''
-   
+
    #make all backslashes to slash, but mask
    #UNC indicator \\ before and restore after.
    sNPath=re.sub(r"\\\\",r"#!#!#",sPath.strip())
    sNPath=re.sub(r"\\",r"/",sNPath)
    sNPath=re.sub(r"#!#!#",r"\\\\",sNPath)
-   
+
    return sNPath
 
 
 def RobotLog2DB(args=None):
    """
 Import robot results from ``output.xml`` to TestResultWebApp's database.
 
-Flow to import Robot results to database: 
+Flow to import Robot results to database:
 
 1. Process provided arguments from command line.
 2. Parse Robot results.
 3. Connect to database.
 4. Import results into database.
 5. Disconnect from database.
 
@@ -1111,15 +1114,15 @@
 
    # get metadata from top level of testsuite
    metadata_info = {}
    if result.suite != None:
       metadata_info = process_suite_metadata(result.suite)
 
    else:
-      Logger.log_error("Could not get suite data from xml result file", 
+      Logger.log_error("Could not get suite data from xml result file",
                        fatal_error=True)
 
    # Validate provided UUID
    if args.UUID!=None:
       if is_valid_uuid(args.UUID):
          pass
       else:
@@ -1127,70 +1130,70 @@
 
    # Validate provided versions info (software;hardware;test)
    arVersions = []
    if args.versions!=None and args.versions.strip() != "":
       arVersions=args.versions.split(";")
       arVersions=[x.strip() for x in arVersions]
       if len(arVersions)>3:
-         Logger.log_error(f"The provided versions information is not valid: '{str(args.versions)}'", 
+         Logger.log_error(f"The provided versions information is not valid: '{str(args.versions)}'",
                           fatal_error=True)
 
    # Validate provided configuration file (component, variant, version_sw)
    dConfig = None
    if args.config != None:
       if os.path.isfile(args.config):
          dConfig = process_config_file(args.config)
       else:
-         Logger.log_error(f"The provided config file is not existing: '{args.config}'" , 
+         Logger.log_error(f"The provided config file is not existing: '{args.config}'" ,
                           fatal_error=True)
 
    # 3. Connect to database
    db=CDataBase()
    try:
       db.connect(args.server,
                  args.user,
                  args.password,
                  args.database,
                  "utf8mb4")
    except Exception as reason:
-      Logger.log_error(f"Could not connect to database: '{reason}'", 
+      Logger.log_error(f"Could not connect to database: '{reason}'",
                        fatal_error=True)
 
    # 4. Import results into database
    #    Create new execution result in database
    #    |
    #    '---Create new file result(s)
    #        |
-   #        '---Create new test result(s) 
+   #        '---Create new test result(s)
    try:
       bUseDefaultPrjVariant = True
       bUseDefaultVersionSW  = True
       sMsgVarirantSetBy = sMsgVersionSWSetBy = "default value"
 
       # Process project/variant info
       sVariant = metadata_info['project']
       if args.variant!=None and args.variant.strip() != "":
          bUseDefaultPrjVariant = False
          sMsgVarirantSetBy = "from --variant commandline argument"
          sVariant = args.variant.strip()
       elif dConfig != None and 'variant' in dConfig:
          bUseDefaultPrjVariant = False
-         sMsgVarirantSetBy = f"from configuration '{args.config}' file provided by --config"  
+         sMsgVarirantSetBy = f"from configuration '{args.config}' file provided by --config"
          sVariant = dConfig['variant']
       _tbl_prj_project = _tbl_prj_variant = sVariant
 
       # Process versions info
       sVersionSW = metadata_info['version_sw']
       sVersionHW  = metadata_info['version_hw']
       sVersionTest   = metadata_info['version_test']
       if len(arVersions) > 0:
          bUseDefaultVersionSW = False
          sMsgVersionSWSetBy = "from --versions commandline argument"
          if len(arVersions)==1 or len(arVersions)==2 or len(arVersions)==3:
-            sVersionSW = arVersions[0] 
+            sVersionSW = arVersions[0]
          if len(arVersions)==2 or len(arVersions)==3:
             sVersionHW = arVersions[1]
          if len(arVersions)==3:
             sVersionTest = arVersions[2]
       elif dConfig != None:
          if 'version_sw' in dConfig:
             bUseDefaultVersionSW = False
@@ -1200,42 +1203,46 @@
             sVersionHW = dConfig['version_hw']
          if 'version_test' in dConfig:
             sVersionTest = dConfig['version_test']
       _tbl_result_version_sw_target = sVersionSW
       _tbl_result_version_hardware  = sVersionHW
       _tbl_result_version_sw_test   = sVersionTest
 
+      # Process start/end time info
+      sSuiteStarttime = result.suite.starttime
+      sSuiteEndtime   = result.suite.endtime
+
+      # Get start and end time of suite a as min and max time incase multiple suite results
+      if (len(sources) > 1) or (len(result.suite.suites) > 0):
+         sSuiteStarttime = min([suite.starttime for suite in result.suite.suites])
+         sSuiteEndtime   = max([suite.endtime for suite in result.suite.suites])
+
+      _tbl_result_time_start = format_time(sSuiteStarttime)
+      _tbl_result_time_end   = format_time(sSuiteEndtime)
+
       # Set version as start time of the execution if not provided in metadata
       # Format: %Y%m%d_%H%M%S
       if _tbl_result_version_sw_target=="":
          bUseDefaultVersionSW = True
-         _tbl_result_version_sw_target = re.sub(r'(\d{8})\s(\d{2}):(\d{2}):(\d{2})\.\d+', 
-                                                r'\1_\2\3\4', result.suite.starttime)
+         _tbl_result_version_sw_target = re.sub(r'(\d{8})\s(\d{2}):(\d{2}):(\d{2})\.\d+',
+                                                r'\1_\2\3\4', sSuiteStarttime)
       if not args.append:
          Logger.log(f"Set project/variant to '{sVariant}' ({sMsgVarirantSetBy})")
          Logger.log(f"Set version_sw to '{_tbl_result_version_sw_target}' ({sMsgVersionSWSetBy})")
 
       # Process branch info from software version
       _tbl_prj_branch = get_branch_from_swversion(_tbl_result_version_sw_target)
 
       # Process UUID info
       if args.UUID != None:
          _tbl_test_result_id = args.UUID
       else:
          _tbl_test_result_id = str(uuid.uuid4())
          if args.append:
             Logger.log_error("'--append' argument should be used in combination with '--UUID <UUID>` argument.", fatal_error=True)
-      
-      # Process start/end time info
-      if len(sources) > 1:
-         _tbl_result_time_start = format_time(min([suite.starttime for suite in result.suite.suites]))
-         _tbl_result_time_end   = format_time(max([suite.endtime for suite in result.suite.suites]))
-      else:
-         _tbl_result_time_start = format_time(result.suite.starttime)
-         _tbl_result_time_end   = format_time(result.suite.endtime)
 
       # Process other info
       _tbl_result_interpretation = ""
       _tbl_result_jenkinsurl     = ""
       _tbl_result_reporting_qualitygate = ""
 
       # Check the UUID is existing or not
@@ -1244,28 +1251,28 @@
       if _db_result_info:
          if args.append:
             # Check given variant/project and version_sw (not default values) with existing values in db
             _db_prj_variant = _db_result_info[0]
             _db_version_sw  = _db_result_info[1]
             if not bUseDefaultPrjVariant and _tbl_prj_variant != _db_prj_variant:
                Logger.log_error(f"Given project/variant '{_tbl_prj_variant}' ({sMsgVarirantSetBy}) is different with existing value '{_db_prj_variant}' in database.", fatal_error=True)
-            elif not bUseDefaultVersionSW and _tbl_result_version_sw_target != _db_version_sw: 
+            elif not bUseDefaultVersionSW and _tbl_result_version_sw_target != _db_version_sw:
                Logger.log_error(f"Given version software '{_tbl_result_version_sw_target}' ({sMsgVersionSWSetBy}) is different with existing value '{_db_version_sw}' in database.", fatal_error=True)
             else:
                Logger.log(f"Append to existing test execution result for variant '{_db_prj_variant}' - version '{_db_version_sw}' - UUID '{_tbl_test_result_id}'.")
          else:
             Logger.log_error(f"Execution result with UUID '{_tbl_test_result_id}' is already existing. \
                \n{error_indent}Please use other UUID (or remove '--UUID' argument from your command) for new execution result. \
-               \n{error_indent}Or add '--append' argument in your command to append new result(s) to this existing UUID.", 
+               \n{error_indent}Or add '--append' argument in your command to append new result(s) to this existing UUID.",
                fatal_error=True)
       else:
          if args.append:
             Logger.log_error(f"Execution result with UUID '{_tbl_test_result_id}' is not existing for appending.\
                \n{error_indent}Please use an existing UUID to append new result(s) to that UUID. \
-               \n{error_indent}Or remove '--append' argument in your command to create new execution result with given UUID.", 
+               \n{error_indent}Or remove '--append' argument in your command to create new execution result with given UUID.",
                fatal_error=True)
          else:
             # Process new test result
             if not Logger.dryrun:
                db.sCreateNewTestResult(_tbl_prj_project,
                                        _tbl_prj_variant,
                                        _tbl_prj_branch,
@@ -1289,16 +1296,16 @@
       db.vFinishTestResult(_tbl_test_result_id)
       if args.append:
          db.vUpdateEvtbl(_tbl_test_result_id)
 
    # 5. Disconnect from database
    db.disconnect()
    import_mode_msg = "append" if args.append else "written"
-   testcnt_msg = f"All {iTotalTestcase}" 
-   extended_msg = "" 
+   testcnt_msg = f"All {iTotalTestcase}"
+   extended_msg = ""
    if (iTotalTestcase>iSuccessTestcase):
       testcnt_msg  = f"{iSuccessTestcase} of {iTotalTestcase}"
       extended_msg = f" {iTotalTestcase-iSuccessTestcase} test cases are skipped because of errors."
    Logger.log()
    Logger.log(f"{testcnt_msg} test cases are {import_mode_msg} to database successfully.{extended_msg}")
 
    # Components's statistics
```

### Comparing `robotframework-robotlog2db-1.3.7/RobotLog2DB/version.py` & `robotframework-robotlog2db-1.3.8/RobotLog2DB/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **************************************************************************************************************
 #
-#  Copyright 2020-2022 Robert Bosch GmbH
+#  Copyright 2020-2023 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,9 +14,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of RobotLog2DB
 #
-VERSION      = "1.3.7"
-VERSION_DATE = "14.06.2023"
+VERSION      = "1.3.8"
+VERSION_DATE = "21.06.2023"
```

### Comparing `robotframework-robotlog2db-1.3.7/RobotLog2DB/xsd/robot.xsd` & `robotframework-robotlog2db-1.3.8/RobotLog2DB/xsd/robot.xsd`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.3.7/robotframework_robotlog2db.egg-info/PKG-INFO` & `robotframework-robotlog2db-1.3.8/robotframework_robotlog2db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robotlog2db
-Version: 1.3.7
+Version: 1.3.8
 Summary: Imports robot result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/robotframework-robotlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -296,15 +296,15 @@
 
 [Tran Hoang Nguyen](mailto:Nguyen.TranHoang@vn.bosch.com)
 
 [Holger Queckenstedt](mailto:Holger.Queckenstedt@de.bosch.com)
 
 ### License
 
-Copyright 2020-2022 Robert Bosch GmbH
+Copyright 2020-2023 Robert Bosch GmbH
 
 Licensed under the Apache License, Version 2.0 (the \"License\"); you
 may not use this file except in compliance with the License. You may
 obtain a copy of the License at
 
 > [![License: Apache
 > v2](https://img.shields.io/pypi/l/robotframework.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)
```

### Comparing `robotframework-robotlog2db-1.3.7/setup.py` & `robotframework-robotlog2db-1.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **************************************************************************************************************
 #
-#  Copyright 2020-2022 Robert Bosch GmbH
+#  Copyright 2020-2023 Robert Bosch GmbH
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

