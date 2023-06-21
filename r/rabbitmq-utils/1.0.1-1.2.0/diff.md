# Comparing `tmp/rabbitmq-utils-1.0.1.tar.gz` & `tmp/rabbitmq-utils-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitmq-utils-1.0.1.tar", last modified: Thu Apr 27 12:02:02 2023, max compression
+gzip compressed data, was "rabbitmq-utils-1.2.0.tar", last modified: Wed Jun 21 09:51:26 2023, max compression
```

## Comparing `rabbitmq-utils-1.0.1.tar` & `rabbitmq-utils-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-04-27 12:02:02.860211 rabbitmq-utils-1.0.1/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     2815 2023-04-27 12:02:02.860211 rabbitmq-utils-1.0.1/PKG-INFO
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     1964 2023-04-27 12:01:58.000000 rabbitmq-utils-1.0.1/README.md
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-04-27 12:02:02.860211 rabbitmq-utils-1.0.1/rabbitmq_utils/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       78 2023-04-27 12:01:58.000000 rabbitmq-utils-1.0.1/rabbitmq_utils/__init__.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     2760 2023-04-27 12:01:58.000000 rabbitmq-utils-1.0.1/rabbitmq_utils/consumer.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     3084 2023-04-27 12:01:58.000000 rabbitmq-utils-1.0.1/rabbitmq_utils/producer.py
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       12 2023-04-27 12:01:58.000000 rabbitmq-utils-1.0.1/rabbitmq_utils/requirements.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       19 2023-04-27 12:01:58.000000 rabbitmq-utils-1.0.1/rabbitmq_utils/version.py
-drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-04-27 12:02:02.860211 rabbitmq-utils-1.0.1/rabbitmq_utils.egg-info/
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     2815 2023-04-27 12:02:02.000000 rabbitmq-utils-1.0.1/rabbitmq_utils.egg-info/PKG-INFO
--rw-rw-r--   0 sigma     (1000) sigma     (1000)      346 2023-04-27 12:02:02.000000 rabbitmq-utils-1.0.1/rabbitmq_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)        1 2023-04-27 12:02:02.000000 rabbitmq-utils-1.0.1/rabbitmq_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       12 2023-04-27 12:02:02.000000 rabbitmq-utils-1.0.1/rabbitmq_utils.egg-info/requires.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       25 2023-04-27 12:02:02.000000 rabbitmq-utils-1.0.1/rabbitmq_utils.egg-info/top_level.txt
--rw-rw-r--   0 sigma     (1000) sigma     (1000)       38 2023-04-27 12:02:02.860211 rabbitmq-utils-1.0.1/setup.cfg
--rw-rw-r--   0 sigma     (1000) sigma     (1000)     2016 2023-04-16 10:20:34.000000 rabbitmq-utils-1.0.1/setup.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-21 09:51:26.275294 rabbitmq-utils-1.2.0/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     6216 2023-06-21 09:51:26.271294 rabbitmq-utils-1.2.0/PKG-INFO
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     5365 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/README.md
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-21 09:51:26.271294 rabbitmq-utils-1.2.0/rabbitmq_utils/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      128 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/rabbitmq_utils/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3423 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/rabbitmq_utils/consumer.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3552 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/rabbitmq_utils/producer.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       12 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/rabbitmq_utils/requirements.txt
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-21 09:51:26.271294 rabbitmq-utils-1.2.0/rabbitmq_utils/rpc/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       59 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/rabbitmq_utils/rpc/__init__.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     3371 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/rabbitmq_utils/rpc/client.py
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     1876 2023-06-21 09:51:22.000000 rabbitmq-utils-1.2.0/rabbitmq_utils/rpc/server.py
+drwxrwxr-x   0 sigma     (1000) sigma     (1000)        0 2023-06-21 09:51:26.271294 rabbitmq-utils-1.2.0/rabbitmq_utils.egg-info/
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     6216 2023-06-21 09:51:26.000000 rabbitmq-utils-1.2.0/rabbitmq_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)      409 2023-06-21 09:51:26.000000 rabbitmq-utils-1.2.0/rabbitmq_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)        1 2023-06-21 09:51:26.000000 rabbitmq-utils-1.2.0/rabbitmq_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       12 2023-06-21 09:51:26.000000 rabbitmq-utils-1.2.0/rabbitmq_utils.egg-info/requires.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       25 2023-06-21 09:51:26.000000 rabbitmq-utils-1.2.0/rabbitmq_utils.egg-info/top_level.txt
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)       38 2023-06-21 09:51:26.275294 rabbitmq-utils-1.2.0/setup.cfg
+-rw-rw-r--   0 sigma     (1000) sigma     (1000)     2068 2023-06-21 09:46:18.000000 rabbitmq-utils-1.2.0/setup.py
```

### Comparing `rabbitmq-utils-1.0.1/rabbitmq_utils/consumer.py` & `rabbitmq-utils-1.2.0/rabbitmq_utils/consumer.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,37 @@
 """
 
 
 import pika
 import time
 
 def callback_test(ch, method, properties, body):
+    # GETTING MESSAGE
+    message = body.decode()
     print('==================================')
-    print(f'INFO: Received Message: \n\n{body.decode()}\n')
-    wait_sec = body.count(b'.')
+    print(f'INFO: Received Message: \n\n{message}\n')
+    
+    # PERFORM YOUR LOGIC HERE
+    import json
+    wait_sec = json.loads(message)['wait_time']
     print(f'INFO: Wating for {wait_sec} seconds.')
     time.sleep(wait_sec)
     print('INFO: Done waiting.')
+    
+    
+    # ACKNOWLEDGE WORK IS DONE
     ch.basic_ack(delivery_tag=method.delivery_tag)
     print("INFO: Acknowledgment Done.")
     print('==================================')
     print('\n\n')
     return None
 
 
 class RabbitMQConsumer():
-    def __init__(self, host, port, virtual_host, username, password, exchange, queue_name, routing_key, exchange_type='topic', callback_fun=callback_test) -> None:
+    def __init__(self, host, port, virtual_host, username, password, queue_name, routing_key, exchange='', exchange_type='topic', callback_fun=callback_test) -> None:
         """Constructor."""
         self.host = host
         self.port = port
         self.virtual_host = virtual_host
         self.username = username
         self.password = password
         self.exchange = exchange
@@ -53,18 +61,19 @@
         connection = pika.BlockingConnection(connection_params)
         self.channel = connection.channel()
         
         # DECLARE QUEUE
         self.channel.queue_declare(queue=self.queue_name, durable=True, exclusive=False, auto_delete=False)
         
         # DECLARE EXCHANGE
-        self.channel.exchange_declare(exchange=self.exchange, exchange_type=self.exchange_type, durable=True)
+        if self.exchange != '': # No delecration and binding is required for default exchange.
+            self.channel.exchange_declare(exchange=self.exchange, exchange_type=self.exchange_type, durable=True)
         
-        # BINDING QUEUE
-        self.channel.queue_bind(exchange=self.exchange, queue=self.queue_name, routing_key=self.routing_key)
+            # BINDING QUEUE
+            self.channel.queue_bind(exchange=self.exchange, queue=self.queue_name, routing_key=self.routing_key)
         return None
     
     def startReveiving(self):
         """Start the consumer consuming process."""
         self.channel.basic_qos(prefetch_count=1)
         self.channel.basic_consume(queue=self.queue_name, on_message_callback=self.callback_fun)
         self.channel.start_consuming()
@@ -73,8 +82,23 @@
     def receiveMessage(self):
         """Main function of the application."""
         # MAKING CONNECTION
         self.makeConnection()
         
         # STARTING CINSUMPTION
         self.startReveiving()
-        return None
+        return None
+
+if __name__ == "__main__":
+    # INFORMATION
+    host = 'localhost'
+    port = 9020
+    virtual_host = '/'
+    username = 'guest'
+    password = 'guest'
+    exchange = 'test_exc'
+    routing_key = 'test_key'
+    queue_name = 'test_que'
+    
+    # RECEIVING
+    consumer = RabbitMQConsumer(host, port, virtual_host, username, password, queue_name, routing_key, exchange)
+    consumer.receiveMessage()
```

### Comparing `rabbitmq-utils-1.0.1/rabbitmq_utils/producer.py` & `rabbitmq-utils-1.2.0/rabbitmq_utils/producer.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,27 +4,37 @@
 Project:	 rabbitmq-utils
 Description: Provide function to send the message to rabbitmq exchange.
 """
 
 import pika
 
 class RabbitMQProducer():
-    def __init__(self, host, port, virtual_host, username, password, exchange, exchange_type='topic') -> None:
+    def __init__(self, host, port, virtual_host, username, password, exchange='', exchange_type='topic') -> None:
         """Constructor."""
         self.host = host
         self.port = port
         self.virtual_host = virtual_host
         self.username = username
         self.password = password
         self.exchange = exchange
         self.exchange_type = exchange_type
         
         # STATE VARIABLES
         self.channel = None
         self.connection = None
+        self._isSent = None
+        return None
+    
+    def isSent(self):
+        """Getting send status."""
+        return self._isSent
+    
+    def setSentStatus(self, status):
+        """Setting send status."""
+        self._isSent = status
         return None
     
     def getChannel(self):
         """Getting channel that have connection."""
         if self.channel is None:
             credentials = pika.credentials.PlainCredentials(self.username, self.password)
             connection_params = pika.ConnectionParameters(
@@ -33,65 +43,71 @@
                 virtual_host=self.virtual_host, 
                 credentials=credentials
                 )
             self.connection = pika.BlockingConnection(connection_params)
             self.channel = self.connection.channel()
             
             # DECLARE EXCHANGE
-            self.channel.exchange_declare(exchange=self.exchange, exchange_type=self.exchange_type, durable=True)
+            if self.exchange != '':
+                self.channel.exchange_declare(exchange=self.exchange, exchange_type=self.exchange_type, durable=True)
             
             # Turn on delivery confirmations
             self.channel.confirm_delivery()
         return self.channel
     
     def closeConnection(self):
         """Close the channel connection."""
         self.connection.close()
         return None
     
-    def sendMessage(self, message, routing_key):
+    def sendMessage(self, message, routing_key, close_connection=True, **kwargs):
         """Send the message to rabbitmq."""
         # GETTING CHANNEL
         channel = self.getChannel()
         
         # SENDING MESSAGE
         is_sent = False
         try:
             channel.basic_publish(
                 exchange=self.exchange,
                 routing_key=routing_key,
                 body=message,
                 mandatory=True,
                 properties=pika.BasicProperties(
                     content_type='text/plain',
-                    delivery_mode=pika.DeliveryMode.Transient
+                    delivery_mode=pika.DeliveryMode.Transient,
+                    **kwargs
                 )
             )
             is_sent = True
         except pika.exceptions.UnroutableError:
             is_sent = False
+            
+        # UDATING STATUS
+        self.setSentStatus(is_sent)
         
         # CLOSING CONNECTION
-        self.closeConnection()
+        if close_connection:
+            self.closeConnection()
         return is_sent
 
 
 if __name__ == "__main__":
     # INFORMATION
     host = 'localhost'
-    port = 5672
+    port = 9020
     virtual_host = '/'
     username = 'guest'
     password = 'guest'
-    exchange = ''
-    routing_key = 'test'
+    exchange = 'test_exc'
+    routing_key = 'test_key'
     
     # DEFINING MESSAGE
     import json
-    message = json.dumps({'hello': 'world'})
+    message = json.dumps({'wait_time': 2})
     
     # SENDING
     producer = RabbitMQProducer(host, port, virtual_host, username, password, exchange)
     is_sent = producer.sendMessage(
         message,
         routing_key
     )
```

### Comparing `rabbitmq-utils-1.0.1/setup.py` & `rabbitmq-utils-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from setuptools import setup, find_namespace_packages
 from pathlib import Path
 
+from rabbitmq_utils import __version__
+
 # README FILE CONTENT
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # GETTING PACKAGES LIST
 def get_packages_list():
     """Getting list of packages using requirements file."""
@@ -12,25 +14,25 @@
     package_list = []
     for package in requirements_file.read_text().split('\n'):
         if package == '':
             continue
         package_list.append(package)
     return package_list
 
-def get_version():
-    """Getting version of the package."""
-    version_file = this_directory / 'rabbitmq_utils' / 'version.py'
-    with open(version_file, "rb") as source_file:
-        code = compile(source_file.read(), version_file, "exec")
-    exec(code)
-    return locals().get('__version__')
+# def get_version():
+#     """Getting version of the package."""
+#     version_file = this_directory / 'rabbitmq_utils' / 'version.py'
+#     with open(version_file, "rb") as source_file:
+#         code = compile(source_file.read(), version_file, "exec")
+#     exec(code)
+#     return locals().get('__version__')
 
 setup(
     name='rabbitmq-utils',
-    version=get_version(),
+    version=__version__,
     description='Provide easy connection to rabbitmq server.',
 
     long_description=long_description,
     long_description_content_type='text/markdown',
     # url='https://hello.com',
 
     author='Tahir Rafique',
```

