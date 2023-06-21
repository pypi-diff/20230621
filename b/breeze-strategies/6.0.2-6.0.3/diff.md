# Comparing `tmp/breeze_strategies-6.0.2.tar.gz` & `tmp/breeze_strategies-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-6.0.2.tar", last modified: Mon Jun 19 08:38:13 2023, max compression
+gzip compressed data, was "breeze_strategies-6.0.3.tar", last modified: Wed Jun 21 06:02:16 2023, max compression
```

## Comparing `breeze_strategies-6.0.2.tar` & `breeze_strategies-6.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 08:38:13.112002 breeze_strategies-6.0.2/
--rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-6.0.2/LICENSE
--rw-rw-rw-   0        0        0     1135 2023-06-19 08:38:13.111005 breeze_strategies-6.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-06-19 08:37:30.000000 breeze_strategies-6.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 08:38:13.056948 breeze_strategies-6.0.2/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0.2/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    18070 2023-06-19 08:36:51.000000 breeze_strategies-6.0.2/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:38:13.109002 breeze_strategies-6.0.2/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1135 2023-06-19 08:38:12.000000 breeze_strategies-6.0.2/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-19 08:38:12.000000 breeze_strategies-6.0.2/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 08:38:12.000000 breeze_strategies-6.0.2/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-19 08:38:12.000000 breeze_strategies-6.0.2/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-19 08:38:12.000000 breeze_strategies-6.0.2/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 08:38:13.113004 breeze_strategies-6.0.2/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-06-19 08:37:27.000000 breeze_strategies-6.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 06:02:16.142026 breeze_strategies-6.0.3/
+-rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-6.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1135 2023-06-21 06:02:16.140004 breeze_strategies-6.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-06-19 10:01:44.000000 breeze_strategies-6.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-21 06:02:16.051430 breeze_strategies-6.0.3/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-6.0.3/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    18286 2023-06-21 05:54:42.000000 breeze_strategies-6.0.3/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-21 06:02:16.136210 breeze_strategies-6.0.3/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1135 2023-06-21 06:02:15.000000 breeze_strategies-6.0.3/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-21 06:02:15.000000 breeze_strategies-6.0.3/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 06:02:15.000000 breeze_strategies-6.0.3/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-21 06:02:15.000000 breeze_strategies-6.0.3/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-21 06:02:15.000000 breeze_strategies-6.0.3/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 06:02:16.142026 breeze_strategies-6.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      817 2023-06-19 10:01:32.000000 breeze_strategies-6.0.3/setup.py
```

### Comparing `breeze_strategies-6.0.2/LICENSE` & `breeze_strategies-6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-6.0.2/PKG-INFO` & `breeze_strategies-6.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze_strategies
-Version: 6.0.2
+Version: 6.0.3
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.2
+pip install breeze_strategies==6.0.3
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.2/README.md` & `breeze_strategies-6.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.2
+pip install breeze_strategies==6.0.3
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.2/breeze_strategies/breeze_strategies.py` & `breeze_strategies-6.0.3/breeze_strategies/breeze_strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,21 @@
                             validity=validity,
                             stoploss="0",
                             quantity=quantity,
                             price=price,
                             validity_date=validity_date,
                             trade_password="",
                             disclosed_quantity="0")
+        response = None
+        if(data['Status'] == 200):
+            response = data['Success']['message']
+        else:
+            response = data['Error']
         
-        print(f"square off status of {right} is",data)
+        print(f"square off status of {right} is",response)
         
     def get_date_format(self,expiry_date):
         month_names = {
                             '01': 'Jan',
                             '02': 'Feb',
                             '03': 'Mar',
                             '04': 'Apr',
@@ -72,15 +77,15 @@
         month = expiry_date[5:7]
         day = expiry_date[8:10]
         formatted_date = f"{day}-{month_names[month]}-{year}"
         return(formatted_date)
         
     def trigger(self,product_type, rightval, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution,put_execution):
         net_gain_loss = (self.currentcall + self.currentput)*int(quantity)
-        print(f"net gain/loss  : {round(net_gain_loss,2)}/- Rs")
+        print(f"P&L (NET): {round(net_gain_loss,2)}/- Rs")
         print("-------------------------------------------------------------------")
         formatted_date = self.get_date_format(expiry_date)
 
         if(net_gain_loss > 0 and net_gain_loss >= self.maxprofit):
             print("maxprofit has reached...")
             print("SquareOff operation on both contracts call and put begins....")
             
@@ -111,23 +116,23 @@
         
         def on_ticks(data):
             
             value = data
             
             if(value['right'] == "Call"):
                 self.currentcall = round(float(value['last']) - float(call_execution), 2)
-                print(f"P & L (CALL)  : {self.currentcall * int(self.quantity)}/- Rs")
-                print("-------------------------------------------------------------------")
+                print(f"P&L (CALL)  : {round(self.currentcall * int(self.quantity),2)}/- Rs")
+                #print("-------------------------------------------------------------------")
                 if(self.flag == False):
                     self.trigger(product_type, "Call", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution)
             
             if(value['right'] == "Put"):
                 self.currentput = round(float(value['last']) - float(put_execution), 2)
-                print(f"P & L (PUT) :  {self.currentput * int(self.quantity)}/- Rs")
-                print("-------------------------------------------------------------------")
+                print(f"P&L (PUT) :  {round(self.currentput * int(self.quantity),2)}/- Rs")
+                #print("-------------------------------------------------------------------")
                 if(self.flag == False):
                     self.trigger(product_type, "Put", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution)
             
         self.client.on_ticks = on_ticks
         self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Call", get_exchange_quotes=True, get_market_depth=False)
         self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Put", get_exchange_quotes=True, get_market_depth=False) 
 
@@ -181,30 +186,30 @@
         t2 = threading.Thread(target = place_order_method,args = (stock_code,exchange_code,"options","buy",order_type,stoploss,qty,put_price,validity,validity_date,expiry_date,"Put",strike_price,res_queue))
         t2.start()
         t2.join()
         secondresponse = res_queue.get()
         
         
         #if one of the order fails then cancel the other one which is successfull
-        if(firstresponse.get('Success',None)!=None and secondresponse.get('Success',None)==None):
+        if(firstresponse.get('Status')==200 and secondresponse.get('Status')==500):
             print("Put Order Failed....")
             order_id = firstresponse['Success']['order_id']
             data  = self.client.cancel_order(exchange_code=exchange_code,
                     order_id = order_id)
 
             if(data.get("Success",None) == None):
                 print("Call Order Cancellation has not been successfull")
                 print("----------END-------------------")
             else:
                 print("Call Order Cancellation has  been successfull")
                 print("----------END-------------------")
             
             
         
-        elif(secondresponse.get('Success',None)!=None and firstresponse.get('Success',None)==None):
+        elif(secondresponse.get('Status')==200 and firstresponse.get('Status')==500):
             print("Call order failed....")
             order_id = secondresponse['Success']['order_id']
             
             data = self.client.cancel_order(exchange_code=exchange_code,
                     order_id = order_id)
             
             if(data.get("Success",None) == None):
@@ -281,20 +286,21 @@
             else:
                 print("Call order got executed at price :{0} Rs and Put Order got executed at price : {1} Rs".format(call_execution,put_execution))
                 self.profit_and_loss(product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution)
             
     def stop(self):
 
         print("squaring off the contract and exiting strategy...")
+        self.client.ws_disconnect()
         self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Call", action = "sell")
         self.squareoff(exchange_code = self.exchange_code, stock_code = self.stock_code, product_type = self.product_type , expiry_date = self.expiry_date , strike_price = self.strike_price , order_type = self.order_type, validity = self.validity, stoploss = self.stoploss, quantity = self.quantity, price = "", validity_date = self.validity_date, trade_password = "", disclosed_quantity="0",right = "Put", action = "sell")
 
-        self.client.ws_disconnect()
+        
 
     def get_pnl(self):
         print("- Negative indicates loss")
-        print(f" P & L(CALL):  {self.currentcall}/- Rs")
-        print(f" P & L(PUT):  {self.currentput}/- Rs")
+        print(f"P&L (CALL):  {round(self.currentcall*int(self.quantity),2)}/- Rs")
+        print(f"P&L (PUT):  {round(self.currentput*int(self.quantity),2)}/- Rs")
         outcome = (self.currentcall + self.currentput)*int(self.quantity)
-        print(f"Total Profit/Loss for {self.quantity} is {outcome}/- Rs")
+        print(f"P&L (NET) for QUANTITY = {self.quantity} is {outcome}/- Rs")
 
         print("------------------------------------------------------------------------------")
```

### Comparing `breeze_strategies-6.0.2/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-6.0.3/breeze_strategies.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breeze-strategies
-Version: 6.0.2
+Version: 6.0.3
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==6.0.2
+pip install breeze_strategies==6.0.3
 
 ```
 
 
 ## code usage
 
 ```python
```

### Comparing `breeze_strategies-6.0.2/setup.py` & `breeze_strategies-6.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="6.0.2",
+    version="6.0.3",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

