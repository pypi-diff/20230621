# Comparing `tmp/turkanime_cli-7.0.5.tar.gz` & `tmp/turkanime_cli-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turkanime_cli-7.0.5.tar", max compression
+gzip compressed data, was "turkanime_cli-7.1.0.tar", max compression
```

## Comparing `turkanime_cli-7.0.5.tar` & `turkanime_cli-7.1.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    15036 2022-12-22 00:44:19.591641 turkanime_cli-7.0.5/LICENSE
--rw-r--r--   0        0        0     2885 2022-12-24 03:09:23.731077 turkanime_cli-7.0.5/README.md
--rw-r--r--   0        0        0     1080 2022-12-24 17:27:37.667975 turkanime_cli-7.0.5/pyproject.toml
--rw-r--r--   0        0        0     4214 2022-12-24 04:25:46.682991 turkanime_cli-7.0.5/turkanime_api/.cli/__pycache__/turkanime.cpython-39.pyc
--rwxr-xr-x   0        0        0     5802 2022-12-24 04:20:52.922997 turkanime_cli-7.0.5/turkanime_api/.cli/turkanime.py
--rw-r--r--   0        0        0      205 2022-12-24 02:13:34.363139 turkanime_cli-7.0.5/turkanime_api/__init__.py
--rw-r--r--   0        0        0     4921 2022-12-24 05:06:19.110946 turkanime_cli-7.0.5/turkanime_api/anime.py
--rw-r--r--   0        0        0     4188 2022-12-24 05:56:01.498890 turkanime_cli-7.0.5/turkanime_api/cli/__pycache__/turkanime.cpython-39.pyc
--rwxr-xr-x   0        0        0     5516 2022-12-24 05:55:50.554891 turkanime_cli-7.0.5/turkanime_api/cli/turkanime.py
--rw-r--r--   0        0        0     8068 2022-12-24 05:39:41.618909 turkanime_cli-7.0.5/turkanime_api/dosyalar.py
--rw-r--r--   0        0        0     7745 2022-12-24 03:47:29.751034 turkanime_cli-7.0.5/turkanime_api/players.py
--rw-r--r--   0        0        0     4571 2022-12-24 06:04:19.090881 turkanime_cli-7.0.5/turkanime_api/tools.py
--rw-r--r--   0        0        0     3843 1970-01-01 00:00:00.000000 turkanime_cli-7.0.5/setup.py
--rw-r--r--   0        0        0     4150 1970-01-01 00:00:00.000000 turkanime_cli-7.0.5/PKG-INFO
+-rw-r--r--   0        0        0    15036 2023-01-02 19:55:34.835687 turkanime_cli-7.1.0/LICENSE
+-rw-r--r--   0        0        0     3276 2023-06-21 14:58:11.139883 turkanime_cli-7.1.0/README.md
+-rw-r--r--   0        0        0     1160 2023-06-21 15:09:58.755876 turkanime_cli-7.1.0/pyproject.toml
+-rw-r--r--   0        0        0      296 2023-06-21 14:58:11.139883 turkanime_cli-7.1.0/turkanime_api/__init__.py
+-rw-r--r--   0        0        0     8058 2023-06-20 23:57:36.423935 turkanime_cli-7.1.0/turkanime_api/anime.py
+-rw-r--r--   0        0        0     4893 2023-06-21 15:13:08.415874 turkanime_cli-7.1.0/turkanime_api/cli/__pycache__/turkanime.cpython-39.pyc
+-rwxr-xr-x   0        0        0     6843 2023-06-21 14:58:11.139883 turkanime_cli-7.1.0/turkanime_api/cli/turkanime.py
+-rw-r--r--   0        0        0     8148 2023-06-20 23:57:36.423935 turkanime_cli-7.1.0/turkanime_api/dosyalar.py
+-rw-r--r--   0        0        0     7585 2023-01-02 22:09:10.059464 turkanime_cli-7.1.0/turkanime_api/players.py
+-rw-r--r--   0        0        0     4885 2023-01-02 21:51:18.303494 turkanime_cli-7.1.0/turkanime_api/tools.py
+-rw-r--r--   0        0        0     1571 2023-06-21 15:13:50.659874 turkanime_cli-7.1.0/turkanime_api/version.py
+-rw-r--r--   0        0        0     4212 1970-01-01 00:00:00.000000 turkanime_cli-7.1.0/setup.py
+-rw-r--r--   0        0        0     4534 1970-01-01 00:00:00.000000 turkanime_cli-7.1.0/PKG-INFO
```

### Comparing `turkanime_cli-7.0.5/LICENSE` & `turkanime_cli-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `turkanime_cli-7.0.5/README.md` & `turkanime_cli-7.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -10,31 +10,38 @@
  - İndirmelere kaldığı yerden devam edebilir
  
 #### Desteklenen kaynaklar:
 ```Sibnet, Odnoklassinki, Sendvid, Mail.ru, VK, Google+, Myvi, GoogleDrive, Yandisk, Vidmoly, Yourupload, Dailymotion```
 
 #### Yenilikler:
  - Seçim ekranı en son seçilen bölümden başlıyor, https://github.com/KebabLord/turkanime-indirici/discussions/35 https://github.com/KebabLord/turkanime-indirici/discussions/30
+ - Aynı anda birden fazla bölüm indirme özelliği https://github.com/KebabLord/turkanime-indirici/pull/49
  - Önceden indirilen veya izlenen animelere izlendi ikonu seçeneği
- - Gereksinimleri otomatik indirme sistemi basitleştirildi
- - Dosya yönetim sistemi eklendi
- - Minimalleştirmeler & Hata gidermeleri
+ - Gereksinimleri uygulama içinden otomatik indirme
+
 
 
 # Kurulum
 Önceden derlenmiş sürümleri [indirebilir](https://github.com/KebabLord/turkanime-indirici/releases/latest) ya da pip ile kolayca `pip install turkanime-cli` kurabilirsiniz. Pip ile kuruyorsanız, ya da scripti kaynak kodundan çalıştırıyorsanız mpv ve geckodriver'ın sisteminizde kurulu olduğundan ve sistem path'ında olduğundan emin olun. Konuya ilişkin rehber için [wiki sayfası](https://github.com/KebabLord/turkanime-indirici/wiki/Herhangi-bir-uygulamay%C4%B1-system-path'%C4%B1na-ekleme).
 
  ### İzleme ekranı
  ![indirme.gif](docs/ss_izle.gif)
 
  ### İndirme ekranı
  ![indirme.gif](docs/ss_indir.gif)
 
 ### Yapılacaklar:
- - Progress yaratılma satırı minimal bir class ile kısaltılacak.
- - ~~Domain güncellemesinden beridir kod stabil çalışmıyor, düzeltilecek.~~
- - ~~Kod çorba gibi, basitleştirilecek.~~
- - ~~Navigasyon  ve indirme algoritması http talepleriyle sağlanacak.~~
- - ~~Zaman bloğu olarak sleep'den kurtulunacak, elementin yüklenmesi beklenecek.~~
- - ~~Prompt kütüphanesi olarak berbat durumda olan PyInquirer'den Questionary'e geçilecek.~~
- - ~~Arama sonuçları da http talepleriyle getirilecek.~~
- - ~~Fansub seçme özelliği tekrar eklenecek.~~
+ - [ ] İndirme bitimi aksiyonları: bildirim veya bilgisayar kapatma.
+ - [ ] Maximum çözünürlüğe ulaş.
+ - [ ] Gui versiyon
+ - [ ] Youtube-dl yerine yt-dlp'ye geçilmeli.
+ - [ ] Selenium'dan kurtulma
+ - [x] ~~Yeni sürüm var mı uygulama açılışında kontrol et.~~
+ - [x] ~~Paralel anime indirme özelliği.~~
+ - [x] ~~Progress yaratılma satırı minimal bir class ile kısaltılacak.~~
+ - [x] ~~Domain güncellemesinden beridir kod stabil çalışmıyor, düzeltilecek.~~
+ - [x] ~~Kod çorba gibi, basitleştirilecek.~~
+ - [x] ~~Navigasyon ve indirme algoritması http talepleriyle sağlanacak.~~
+ - [x] ~~Zaman bloğu olarak sleep'den kurtulunacak, elementin yüklenmesi beklenecek.~~
+ - [x] ~~Prompt kütüphanesi olarak berbat durumda olan PyInquirer'den Questionary'e geçilecek.~~
+ - [x] ~~Arama sonuçları da http talepleriyle getirilecek.~~
+ - [x] ~~Fansub seçme özelliği tekrar eklenecek.~~
```

### Comparing `turkanime_cli-7.0.5/pyproject.toml` & `turkanime_cli-7.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turkanime-cli"
-version = "7.0.5"
+version = "7.1.0"
 description = "Türkanime video oynatıcı ve indirici"
 authors = ["Junicchi <junicchi@waifu.club>"]
 readme = "README.md"
 license = "CC-BY-NC-ND-4.0"
 repository = "https://github.com/kebablord/turkanime-indirici"
 keywords = ["turkanime","turk","anime","downloader"]
 
@@ -34,10 +34,12 @@
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-# Publish sırasında buraya kopyalanmalı
-# ./turkanime.py -> turkanime_api/cli/turkanime.py
+# Publish sırasında yapılması gerekenler:
+#   cp ./turkanime.py turkanime_api/cli/turkanime.py
+#   turkanime_api/version.py dosyasındaki build, pip olarak değişmeli.
+
 turkanime = 'turkanime_api.cli.turkanime:run'
```

### Comparing `turkanime_cli-7.0.5/turkanime_api/.cli/turkanime.py` & `turkanime_cli-7.1.0/turkanime_api/cli/turkanime.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,148 +1,198 @@
-""" TürkAnimu Downloader v7 """
-from os import path,mkdir
+""" TürkAnimu Downloader """
+from os import path,mkdir,name,environ
 from sys import exit as kapat
 from time import sleep
 from atexit import register
 from selenium.common.exceptions import WebDriverException
-from rich.progress import Progress, BarColumn, SpinnerColumn
 from rich import print as rprint
-from questionary import select,autocomplete,checkbox
+from questionary import select,autocomplete,checkbox, text
 
-from turkanime_api import AnimeSorgula,Anime,DosyaManager,gereksinim_kontrol
-from turkanime_api import elementi_bekle,webdriver_hazirla,prompt_tema,clear
+from turkanime_api import (
+    AnimeSorgula,
+    Anime,
+    DosyaManager,
+    gereksinim_kontrol,
+    elementi_bekle,
+    webdriver_hazirla,
+    prompt_tema,
+    clear,
+    create_progress,
+    isGuncel,update_type,__build__
+)
 
-def main():
-    with Progress(SpinnerColumn(), '[progress.description]{task.description}', BarColumn(bar_width=40)) as progress:
-        task = progress.add_task("[cyan]Sürücü başlatılıyor..", start=False)
-        gereksinim_kontrol(progress)
-        driver = webdriver_hazirla(progress)
-        register(lambda: (print("Program kapatılıyor..",end="\r") or driver.quit()))
-    
-        progress.update(task, description="[cyan]TürkAnime'ye bağlanılıyor..")
-        try:
-            driver.get("https://turkanime.co/kullanici/anonim")
-            elementi_bekle(".navbar-nav",driver)
-        except (ConnectionError,WebDriverException):
-            progress.update(task,visible=False)
-            rprint("[red][strong]TürkAnime'ye ulaşılamıyor.[/strong][red]")
-            kapat(1)
-        sorgu = AnimeSorgula(driver)
+# Uygulama path'ını işletim sistemine uygun olarak script'e importla
+dosya = DosyaManager()
+SEP = ";" if name=="nt" else ":"
+environ["PATH"] +=  SEP + dosya.ROOT + SEP
+
+# Güncelleme varsa uyarı ver.
+if not isGuncel:
+    rprint(f"[red]!)[/red] {update_type} güncellemesi mevcut!")
+    if __build__ == "pip":
+        print("  - Güncellemek için: pip install -U turkanime-cli")
+    elif __build__ == "exe":
+        print("  - Son sürümü github'daki releases bölümünden indirebilirsin")
+    print("\n")
+    sleep(3)
+else:
+    rprint(f"[green]*)[/green] Script'in güncel {__build__} sürümünü kullanıyorsunuz.")
+
+# Selenium'u başlat
+with create_progress() as progress:
+    task = progress.add_task("[cyan]Sürücü başlatılıyor..", start=False)
+    gereksinim_kontrol(progress)
+    driver = webdriver_hazirla(progress)
+    register(lambda: (print("Program kapatılıyor..",end="\r") or driver.quit()))
+
+    progress.update(task, description="[cyan]TürkAnime'ye bağlanılıyor..")
+    try:
+        driver.get("https://turkanime.co/kullanici/anonim")
+        elementi_bekle(".navbar-nav",driver)
+    except (ConnectionError,WebDriverException):
         progress.update(task,visible=False)
-    
+        rprint("[red][strong]TürkAnime'ye ulaşılamıyor.[/strong][red]")
+        kapat(1)
+    sorgu = AnimeSorgula(driver)
+    progress.update(task,visible=False)
+
+# Kullanıcıyı karşıla
+clear()
+rprint("[green]!)[/green] Üst menülere dönmek için Ctrl+C kullanabilirsiniz.\n")
+sleep(2.5)
+
+# Ana menü
+while True:
     clear()
-    rprint("[green]!)[/green] Üst menülere dönmek için Ctrl+C kullanabilirsiniz.\n")
-    sleep(2.5)
-    
-    while True:
+    islem = select(
+        "İşlemi seç",
+        choices=['Anime izle',
+                'Anime indir',
+                'Ayarlar',
+                'Kapat'],
+        style=prompt_tema,
+        instruction=" "
+    ).ask()
+
+    if "Anime" in islem:
         clear()
-        islem = select(
-            "İşlemi seç",
-            choices=['Anime izle',
-                    'Anime indir',
-                    'Ayarlar',
-                    'Kapat'],
-            style=prompt_tema,
-            instruction=" "
-        ).ask()
-    
-        if "Anime" in islem:
-            clear()
-            try:
-                secilen_seri = autocomplete(
-                    'Animeyi yazın',
-                    choices=sorgu.get_seriler(),
-                    style=prompt_tema
-                ).ask()
-                seri_slug = sorgu.tamliste[secilen_seri]
-            except KeyError:
-                rprint("[red][strong]Aradığınız anime bulunamadı.[/strong][red]")
-                continue
-    
-            bolumler = sorgu.get_bolumler(secilen_seri)
-            set_prev = lambda x: [i for i in bolumler if i["value"]==x].pop()
-            previous = None
-            while True:
-                if "izle" in islem:
-                    sorgu.mark_bolumler(seri_slug,bolumler,islem="izlendi")
-                    previous = sorgu.son_bolum if previous == None else previous
-                    clear()
-                    secilen = select(
-                        message='Bölüm seç',
-                        choices=bolumler,
-                        style=prompt_tema,
-                        default=previous
-                    ).ask(kbi_msg="")
-                    if secilen:
-                        previous = set_prev(secilen)
-                else:
-                    sorgu.mark_bolumler(seri_slug,bolumler,islem="indirildi")
-                    previous = sorgu.son_bolum if previous == None else previous
-                    clear()
-                    secilen = checkbox(
-                        message = "Bölüm seç",
-                        choices=bolumler,
-                        style=prompt_tema,
-                        initial_choice=previous
-                    ).ask(kbi_msg="")
-                    if secilen:
-                        previous = set_prev(secilen[-1])
-    
-                # Bölüm seçim ekranı iptal edildiyse
-                if not secilen:
-                    break
-                anime = Anime(driver, sorgu.anime_ismi ,secilen)
-    
-                if islem=="Anime izle":
-                    anime.oynat()
-                else:
-                    anime.indir()
-    
-        elif "Ayarlar" in islem:
-            dosya = DosyaManager()
-            ayar = dosya.ayar
-            tr = lambda x: "AÇIK" if x else "KAPALI"
-            while True:
-                _otosub  = ayar.getboolean("TurkAnime","manuel fansub")
-                _watched = ayar.getboolean("TurkAnime","izlendi ikonu")
-                _otosave = ayar.getboolean("TurkAnime","izlerken kaydet")
-                ayarlar = [
-                    'İndirilenler klasörünü seç',
-                    f'İzlerken kaydet: {tr(_otosave)}',
-                    f'Manuel fansub seç: {tr(_otosub)}',
-                    f'İzlendi/İndirildi ikonu: {tr(_watched)}',
-                    'Geri dön'
-                ]
+        try:
+            secilen_seri = autocomplete(
+                'Animeyi yazın',
+                choices=sorgu.get_seriler(),
+                style=prompt_tema
+            ).ask()
+            seri_slug = sorgu.tamliste[secilen_seri]
+        except KeyError:
+            rprint("[red][strong]Aradığınız anime bulunamadı.[/strong][red]")
+            continue
+
+        bolumler = sorgu.get_bolumler(secilen_seri)
+        set_prev = lambda x: [i for i in bolumler if i["value"]==x].pop()
+        previous = None
+        while True:
+            if "izle" in islem:
+                sorgu.mark_bolumler(seri_slug,bolumler,islem="izlendi")
+                previous = sorgu.son_bolum if previous is None else previous
+                clear()
+                secilen = select(
+                    message='Bölüm seç',
+                    choices=bolumler,
+                    style=prompt_tema,
+                    default=previous
+                ).ask(kbi_msg="")
+                if secilen:
+                    previous = set_prev(secilen)
+            else:
+                sorgu.mark_bolumler(seri_slug,bolumler,islem="indirildi")
+                previous = sorgu.son_bolum if previous is None else previous
                 clear()
-                cevap = select(
-                    'İşlemi seç',
-                    ayarlar,
+                secilen = checkbox(
+                    message = "Bölüm seç",
+                    choices=bolumler,
                     style=prompt_tema,
-                    instruction=" "
-                    ).ask()
-                if cevap == ayarlar[0]:
-                    from easygui import diropenbox
-                    indirilenler_dizin=diropenbox()
-                    if indirilenler_dizin:
-                        ayar.set('TurkAnime','indirilenler',indirilenler_dizin)
-    
-                elif cevap == ayarlar[1]:
-                    ayar.set('TurkAnime','izlerken kaydet',str(not _otosave))
-                    if not path.isdir(path.join(".","Kayıtlar")):
-                        mkdir(path.join(".","Kayıtlar"))
-    
-                elif cevap == ayarlar[2]:
-                    ayar.set('TurkAnime','manuel fansub',str(not _otosub))
-    
-                elif cevap == ayarlar[3]:
-                    ayar.set('TurkAnime','izlendi ikonu',str(not _watched))
-    
+                    initial_choice=previous
+                ).ask(kbi_msg="")
+                if secilen:
+                    previous = set_prev(secilen[-1])
+
+            # Bölüm seçim ekranı iptal edildiyse
+            if not secilen:
+                break
+            anime = Anime(driver, sorgu.anime_ismi ,secilen)
+
+            if islem=="Anime izle":
+                anime.oynat()
+            else:
+                dosya = DosyaManager()
+                max_dl = dosya.ayar.getint("TurkAnime","aynı anda indirme sayısı")
+                if max_dl <= 1:
+                    anime.indir()
                 else:
-                    break
-                dosya.save_ayarlar()
-                sorgu.son_bolum=None
-    
-        elif "Kapat" in islem:
-            break
+                    rprint(f" [green]-[/green] Paralel indirme aktif. (max={max_dl})\n")
+                    anime.multi_indir(max_dl)
+
+
+    elif "Ayarlar" in islem:
+        dosya = DosyaManager()
+        ayar = dosya.ayar
+        tr = lambda x: "AÇIK" if x else "KAPALI"
+        while True:
+            _otosub  = ayar.getboolean("TurkAnime","manuel fansub")
+            _watched = ayar.getboolean("TurkAnime","izlendi ikonu")
+            _otosave = ayar.getboolean("TurkAnime","izlerken kaydet")
+            _max_dl  = ayar.get("TurkAnime","aynı anda indirme sayısı")
+            ayarlar = [
+                'İndirilenler klasörünü seç',
+                f'İzlerken kaydet: {tr(_otosave)}',
+                f'Manuel fansub seç: {tr(_otosub)}',
+                f'İzlendi/İndirildi ikonu: {tr(_watched)}',
+                f'Aynı anda indirme sayısı: {_max_dl}',
+                'Geri dön'
+            ]
+            clear()
+            cevap = select(
+                'İşlemi seç',
+                ayarlar,
+                style=prompt_tema,
+                instruction=" "
+                ).ask()
+            if cevap == ayarlar[0]:
+                from easygui import diropenbox
+                indirilenler_dizin=diropenbox()
+                if indirilenler_dizin:
+                    ayar.set('TurkAnime','indirilenler',indirilenler_dizin)
+
+            elif cevap == ayarlar[1]:
+                ayar.set('TurkAnime','izlerken kaydet',str(not _otosave))
+                if not path.isdir(path.join(".","Kayıtlar")):
+                    mkdir(path.join(".","Kayıtlar"))
+
+            elif cevap == ayarlar[2]:
+                ayar.set('TurkAnime','manuel fansub',str(not _otosub))
+
+            elif cevap == ayarlar[3]:
+                ayar.set('TurkAnime','izlendi ikonu',str(not _watched))
+
+            elif cevap == ayarlar[4]:
+                _max_dl = text(
+                    message = 'Maksimum eş zamanlı kaç bölüm indirilsin?',
+                    default = str(_max_dl),
+                    style = prompt_tema
+                ).ask(kbi_msg="")
+                ayar.set('TurkAnime','aynı anda indirme sayısı',_max_dl)
+
+            else:
+                break
+            dosya.save_ayarlar()
+            sorgu.son_bolum=None
+
+    elif "Kapat" in islem:
+        break
+
 
+""" Poetry script'leri de modül gibi çalışmaya zorladığından
+    limitasyonu aşmak için kirli bir çözüm.
+"""
+run = lambda: None
 if __name__=="__main__":
-    main()
+    run()
```

### Comparing `turkanime_cli-7.0.5/turkanime_api/anime.py` & `turkanime_cli-7.1.0/turkanime_api/anime.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 from os import system,path,mkdir,environ,name
+from time import sleep,perf_counter
+from subprocess import Popen, PIPE
+from concurrent.futures import ThreadPoolExecutor, as_completed
+from shlex import split as csplit
 import json
 from bs4 import BeautifulSoup as bs4
-from rich.progress import Progress, BarColumn, SpinnerColumn
 from rich import print as rprint
 
 from .players import url_getir
 from .dosyalar import DosyaManager
+from .tools import create_progress
 
 class AnimeSorgula():
+    """ İstenilen bölümü veya bölümleri dict olarak getir. """
     def __init__(self,driver=None):
         self.driver=driver
         self.anime_ismi=None
         self.tamliste=None
         self.son_bolum=None
         self.dosya=DosyaManager()
 
     def get_seriler(self):
         """ Sitedeki tüm animeleri [{name:*,value:*}..] formatında döndürür. """
-        with Progress(SpinnerColumn(), '[progress.description]{task.description}', BarColumn(bar_width=40)) as progress:
+        with create_progress() as progress:
             task = progress.add_task("[cyan]Anime listesi getiriliyor..", start=False)
             if self.tamliste:
                 progress.update(task,visible=False)
                 return self.tamliste.keys()
 
             soup = bs4(
                 self.driver.execute_script("return $.get('/ajax/tamliste')"),
@@ -31,15 +36,15 @@
             for seri in raw_series:
                 self.tamliste[seri.text] = seri.findParent().get('href').split('anime/')[1]
             progress.update(task,visible=False)
             return [seri.text for seri in raw_series]
 
     def get_bolumler(self, isim):
         """ Animenin bölümlerini {bölüm,title} formatında döndürür. """
-        with Progress(SpinnerColumn(), '[progress.description]{task.description}', BarColumn(bar_width=40)) as progress:
+        with create_progress() as progress:
             task = progress.add_task("[cyan]Bölümler getiriliyor..", start=False)
             anime_slug=self.tamliste[isim]
             self.anime_ismi = anime_slug
             raw = self.driver.execute_script(f"return $.get('/anime/{anime_slug}')")
             soup = bs4(raw,"html.parser")
             anime_code = soup.find('meta',{'name':'twitter:image'}).get('content').split('lerb/')[1][:-4]
 
@@ -84,29 +89,102 @@
         self.dosya.tazele()
         dlfolder = self.dosya.ayar.get("TurkAnime","indirilenler")
 
         if not path.isdir(path.join(dlfolder,self.seri)):
             mkdir(path.join(dlfolder,self.seri))
 
         for i,bolum in enumerate(self.bolumler):
-            print(" "*50+f"\r\n{i+1}. bölüm indiriliyor:")
+            print(" "*50+f"\r\n{i+1}. video indiriliyor:")
             otosub = bool(len(self.bolumler)==1 and self.otosub)
             url = url_getir(bolum,self.driver,manualsub=otosub)
+            if not url:
+                rprint("[red]Bu fansuba veya bölüme ait çalışan bir player bulunamadı.[/red]")
+                sleep(3)
+                continue
             suffix="--referer https://video.sibnet.ru/" if "sibnet" in url else ""
-            system(f'youtube-dl --no-warnings -o "{path.join(dlfolder,self.seri,bolum)}.%(ext)s" "{url}" {suffix}')
+            output = path.join(dlfolder,self.seri,bolum)
+            system(f'youtube-dl --no-warnings -o "{output}.%(ext)s" "{url}" {suffix}')
             self.dosya.update_gecmis(self.seri,bolum,islem="indirildi")
         return True
 
+    def multi_indir(self, worker_count = 2):
+        self.dosya.tazele()
+        dlfolder = self.dosya.ayar.get("TurkAnime","indirilenler")
+
+        if not path.isdir(path.join(dlfolder,self.seri)):
+            mkdir(path.join(dlfolder,self.seri))
+
+        def find_urls(i, bolum):
+            print(" "*50+f"\r\n{i+1}. video hazırlanıyor:")
+            otosub = bool(len(self.bolumler)==1 and self.otosub)
+            url = url_getir(bolum,self.driver,manualsub=otosub)
+            if not url:
+                rprint("[red]Bu fansuba veya bölüme ait çalışan bir player bulunamadı.[/red]")
+                sleep(3)
+                return ()
+            suffix="--referer https://video.sibnet.ru/" if "sibnet" in url else ""
+            output = path.join(dlfolder,self.seri,bolum)
+            cmd = f'youtube-dl --no-warnings -o "{output}.%(ext)s" "{url}" {suffix}'
+            return (bolum, cmd)
+
+        def thread(bolum, cmd, i, progress):
+            task = None
+            p = Popen(csplit(cmd), stdout=PIPE)
+            b = False
+            output = b''
+            while p.poll() is None:
+                c = p.stdout.read(1)
+                if c == b'\r':
+                    if b:
+                        splited = output.split()
+                        yuzde, file_size, speed = splited[1].decode('UTF-8'), \
+                            splited[3].decode('UTF-8'), splited[5].decode('UTF-8')
+                        if not task:
+                            task = progress.add_task(
+                                f'[red]Seçilen {i}. bölüm indiriliyor. {file_size}',
+                                total=100, visible=False)
+                        else:
+                            progress.update(task, completed=float(yuzde[:-1]), visible=True,
+                                description=f'[red]Seçilen {i}. bölüm indiriliyor. {file_size} {speed}')
+                        b = not b
+                        output = b''
+                        continue
+                    b = not b
+                elif b:
+                    output += c
+            progress.update(task, completed=100, visible=True)
+            self.dosya.update_gecmis(self.seri, bolum,islem="indirildi")
+            return True
+
+        cmds = []
+        for i, bolum in enumerate(self.bolumler):
+            cmd = find_urls(i, bolum)
+            if cmd:
+                cmds.append(cmd)
+
+        with create_progress() as progress:
+            start = perf_counter()
+            with ThreadPoolExecutor(worker_count) as executor:
+                futures = {executor.submit(thread, t[0], t[1], i + 1, progress) for i, t in enumerate(cmds)}
+                for _ in as_completed(futures):
+                    pass
+            end = perf_counter()
+
+        rprint(f'İndirme işlemi {int(end - start)} saniye sürdü')
+        sleep(5)
+        return True
+
     def oynat(self):
         url = url_getir(self.bolumler,self.driver,manualsub=self.otosub)
 
         if not url:
             rprint("[red]Bu bölüme ait çalışan bir player bulunamadı.[/red]")
             return False
 
         suffix ="--referrer=https://video.sibnet.ru/ " if  "sibnet" in url else ""
         suffix+= "--msg-level=display-tags=no "
         if self.dosya.ayar.getboolean("TurkAnime","izlerken kaydet"):
-            suffix+="--stream-record={}.mp4 ".format(path.join(self.dosya.ROOT,"Kayıtlar",self.bolumler))
+            output = path.join(self.dosya.ROOT,"Kayıtlar",self.bolumler)
+            suffix+=f"--stream-record={output}.mp4 "
         system(f'mpv "{url}" {suffix} ')
         self.dosya.update_gecmis(self.seri,self.bolumler,islem="izlendi")
         return True
```

### Comparing `turkanime_cli-7.0.5/turkanime_api/dosyalar.py` & `turkanime_cli-7.1.0/turkanime_api/dosyalar.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 DownloadGereksinimler()
     - Gereksinimlerin indirilmesini ve paketten çıkarılmasını sağlar.
 """
 from os import path,mkdir,replace,rename,remove,system,getcwd
 from struct import calcsize
 from configparser import ConfigParser
 import json
-from py7zr import SevenZipFile
 from zipfile import ZipFile
 from concurrent.futures import ThreadPoolExecutor
 from urllib.request import urlopen
 import signal
 from shutil import rmtree
 from functools import partial
 import requests
+from py7zr import SevenZipFile
 
 from rich.progress import (
     Event,
     Progress,
     TextColumn,
     BarColumn,
     DownloadColumn,
@@ -33,19 +33,21 @@
     """
     def __init__(self):
         if path.isdir(".git"): # Git reposundan çalıştırıldığında.
             self.ROOT = getcwd()
         else: # Pip modülü veya Exe olarak çalıştırıldığında.
             self.ROOT = path.join(path.expanduser("~"), "TurkAnimu" )
 
+        # default ayarlar
         self.default = {
             "manuel fansub" : "False",
             "izlerken kaydet" : "False",
             "indirilenler" : ".",
-            "izlendi ikonu" : "True"
+            "izlendi ikonu" : "True",
+            "aynı anda indirme sayısı" : "3",
         }
         self.ayar_path = path.join(self.ROOT, "ayarlar.ini")
         self.gecmis_path = path.join(self.ROOT, "gecmis.json")
         self.verify_dosyalar()
         self.ayar = ConfigParser()
         self.ayar.read(self.ayar_path)
 
@@ -184,23 +186,23 @@
                 self.prog.start_task(task_id)
                 for data in iter(partial(response.read, 32768), b""):
                     dest_file.write(data)
                     self.prog.update(task_id, advance=len(data))
                     if self.done_event.is_set():
                         print("Başarısız")
                         return
-        except Exception as rr:
+        except Exception as err:
             self.prog.console.log("HATA:",str(err))
             self.status=False
             return
         self.prog.console.log(f"İndirildi: {dlpath}")
 
     def download(self, urls, dest_dir):
         """Birden fazla url'yi hedef dosyaya indir."""
-        urls = [urls] if not type(urls) is list else urls
+        urls = [urls] if not isinstance(urls,list) else urls
         with self.prog:
             with ThreadPoolExecutor(max_workers=3) as pool:
                 for url in urls:
                     filename = url.split("/")[-1]
                     dest_path = path.join(dest_dir, filename)
                     task_id = self.prog.add_task("download", filename=filename, start=False)
                     pool.submit(self.copy_url, task_id, url, dest_path)
```

### Comparing `turkanime_cli-7.0.5/turkanime_api/players.py` & `turkanime_cli-7.1.0/turkanime_api/players.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import re
 import subprocess as sp
 from time import time
 import base64
 from selenium.common.exceptions import NoSuchElementException,JavascriptException
-from rich.progress import Progress, BarColumn, SpinnerColumn
 from rich import print as rprint
 from questionary import select
 from bs4 import BeautifulSoup as bs4
-from .tools import prompt_tema
+from .tools import prompt_tema,create_progress
 from .dosyalar import DosyaManager
 
 desteklenen_players = [
     "SIBNET",
     "MAIL",
     "MYVI",
     "VK",
@@ -40,14 +39,19 @@
         raise ConnectionError("TürkAnime'ye ulaşılamıyor")
 
 def check_video(url):
     """ Video yaşıyor mu kontrol eder """
     if "_myvideo" in url:
         return False
     test = sp.Popen(f'youtube-dl --no-warnings -F "{url}"',stdout=sp.PIPE,shell=True)
+    try:
+        test.wait(30)
+    except sp.TimeoutExpired:
+        test.kill()
+        return False
     stdout = test.communicate()[0].decode()
     stdexit   = test.returncode
     if stdexit == 0 and "php" not in stdout:
         return True
     return False
 
 def fansub_sec(src):
@@ -132,26 +136,20 @@
         ve çalışan bir alternatif bulana dek bu listedeki playerları itere eder.
     """
     dosya, url = DosyaManager(), False
     key = base64.b64decode(
             dosya.ayar.get("TurkAnime","key")
         ).decode() if dosya.ayar.has_option("TurkAnime","key") else False
 
-    with Progress(
-        SpinnerColumn(),'[progress.description]{task.description}',
-        BarColumn(bar_width=40),transient=True) as progress:
+    with create_progress(transient=True) as progress:
         task = progress.add_task("[cyan]Bölüm sayfası getiriliyor..", start=False)
         bolum_src = driver.execute_script(f'return $.get("/video/{bolum}")')
 
     fansub_hash = fansub_sec(bolum_src) if manualsub else ""
-    with Progress(
-            SpinnerColumn(),
-            '[progress.description]{task.description}',
-            BarColumn(bar_width=40)
-        ) as progress:
+    with create_progress() as progress:
         task = progress.add_task("[cyan]Video url'si çözülüyor..", start=False)
 
         videos = []
         regex = re.search("videosec&b=(.*?)&", bolum_src)
 
         if regex:
             bolum_hash = regex.group()
```

### Comparing `turkanime_cli-7.0.5/turkanime_api/tools.py` & `turkanime_cli-7.1.0/turkanime_api/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,30 +10,40 @@
 import subprocess as sp
 from os import name,system
 from time import sleep
 from prompt_toolkit import styles
 from selenium import webdriver
 from selenium.webdriver.firefox.options import Options
 from selenium.common.exceptions import SessionNotCreatedException
+from rich.progress import Progress, BarColumn, SpinnerColumn
 from questionary import confirm
 
 from .dosyalar import DosyaManager,DownloadGereksinimler
 
 def clear():
     """ Daha kompakt görüntü için her prompt sonrası clear
         Debug yapacaksanız devre dışı bırakmanız önerilir.
     """
     system('cls' if name == 'nt' else 'clear')
 
+def create_progress(transient=False):
+    """ Progress animasyonu objesini döndürüyor. """
+    return Progress(
+        SpinnerColumn(),
+        '[progress.description]{task.description}',
+        BarColumn(bar_width=40),
+        transient=transient
+    )
+
 def gereksinim_kontrol(progress=None):
     """ Gereksinimlerin erişilebilir olup olmadığını kontrol eder """
     stdout, bulunmayan = "\n", []
     for gereksinim in ["geckodriver","youtube-dl","mpv"]:
         status = sp.Popen(f'{gereksinim} --version',stdout=sp.PIPE,stderr=sp.PIPE,shell=True).wait()
-        if status==1 or status==127:
+        if status in (1,127):
             stdout += f"x {gereksinim} bulunamadı.\n"
             bulunmayan.append(gereksinim)
         elif status==0:
             stdout += f"+ {gereksinim} bulundu.\n"
         else:
             stdout += f"x {gereksinim} bulundu ancak çalıştırılamadı.\n"
             if name=="nt" and gereksinim=="youtube-dl":
```

### Comparing `turkanime_cli-7.0.5/setup.py` & `turkanime_cli-7.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['turkanime_api', 'turkanime_api..cli', 'turkanime_api.cli']
+['turkanime_api', 'turkanime_api.cli']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['bs4>=0.0.1',
  'easygui>=0.98.2',
@@ -18,17 +18,17 @@
  'youtube_dl>=2021.0.0']
 
 entry_points = \
 {'console_scripts': ['turkanime = turkanime_api.cli.turkanime:run']}
 
 setup_kwargs = {
     'name': 'turkanime-cli',
-    'version': '7.0.5',
+    'version': '7.1.0',
     'description': 'Türkanime video oynatıcı ve indirici',
-    'long_description': "# TürkAnimu-Cli\n[![GitHub all releases](https://img.shields.io/github/downloads/kebablord/turkanime-indirici/total?style=flat-square)](https://github.com/KebabLord/turkanime-indirici/releases/latest)  [![GitHub release (latest by date)](https://img.shields.io/github/v/release/kebablord/turkanime-indirici?style=flat-square)](https://github.com/kebablord/turkanime-indirici/releases/latest/download/turkanimu.exe)  [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/kebablord/turkanime-indirici/.github/workflows/main.yml?style=flat-square)](https://github.com/KebabLord/turkanime-indirici/actions) [![Pypi version](https://img.shields.io/pypi/v/turkanime-cli?style=flat-square)](https://pypi.org/project/turkanime-cli/)\n\nTürkanime için terminal video oynatıcı ve indirici. İtinayla her bölümü indirir & oynatır.\n - Yığın bölüm indirebilir\n - Animu izleyebilir\n - Uygulama içinden arama yapabilir\n - Fansub seçtirebilir\n - Bir yandan izlerken bir yandan animeyi kaydedebilir\n - İndirmelere kaldığı yerden devam edebilir\n \n#### Desteklenen kaynaklar:\n```Sibnet, Odnoklassinki, Sendvid, Mail.ru, VK, Google+, Myvi, GoogleDrive, Yandisk, Vidmoly, Yourupload, Dailymotion```\n\n#### Yenilikler:\n - Seçim ekranı en son seçilen bölümden başlıyor, https://github.com/KebabLord/turkanime-indirici/discussions/35 https://github.com/KebabLord/turkanime-indirici/discussions/30\n - Önceden indirilen veya izlenen animelere izlendi ikonu seçeneği\n - Gereksinimleri otomatik indirme sistemi basitleştirildi\n - Dosya yönetim sistemi eklendi\n - Minimalleştirmeler & Hata gidermeleri\n\n\n# Kurulum\nÖnceden derlenmiş sürümleri [indirebilir](https://github.com/KebabLord/turkanime-indirici/releases/latest) ya da pip ile kolayca `pip install turkanime-cli` kurabilirsiniz. Pip ile kuruyorsanız, ya da scripti kaynak kodundan çalıştırıyorsanız mpv ve geckodriver'ın sisteminizde kurulu olduğundan ve sistem path'ında olduğundan emin olun. Konuya ilişkin rehber için [wiki sayfası](https://github.com/KebabLord/turkanime-indirici/wiki/Herhangi-bir-uygulamay%C4%B1-system-path'%C4%B1na-ekleme).\n\n ### İzleme ekranı\n ![indirme.gif](docs/ss_izle.gif)\n\n ### İndirme ekranı\n ![indirme.gif](docs/ss_indir.gif)\n\n### Yapılacaklar:\n - Progress yaratılma satırı minimal bir class ile kısaltılacak.\n - ~~Domain güncellemesinden beridir kod stabil çalışmıyor, düzeltilecek.~~\n - ~~Kod çorba gibi, basitleştirilecek.~~\n - ~~Navigasyon  ve indirme algoritması http talepleriyle sağlanacak.~~\n - ~~Zaman bloğu olarak sleep'den kurtulunacak, elementin yüklenmesi beklenecek.~~\n - ~~Prompt kütüphanesi olarak berbat durumda olan PyInquirer'den Questionary'e geçilecek.~~\n - ~~Arama sonuçları da http talepleriyle getirilecek.~~\n - ~~Fansub seçme özelliği tekrar eklenecek.~~\n",
+    'long_description': "# TürkAnimu-Cli\n[![GitHub all releases](https://img.shields.io/github/downloads/kebablord/turkanime-indirici/total?style=flat-square)](https://github.com/KebabLord/turkanime-indirici/releases/latest)  [![GitHub release (latest by date)](https://img.shields.io/github/v/release/kebablord/turkanime-indirici?style=flat-square)](https://github.com/kebablord/turkanime-indirici/releases/latest/download/turkanimu.exe)  [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/kebablord/turkanime-indirici/.github/workflows/main.yml?style=flat-square)](https://github.com/KebabLord/turkanime-indirici/actions) [![Pypi version](https://img.shields.io/pypi/v/turkanime-cli?style=flat-square)](https://pypi.org/project/turkanime-cli/)\n\nTürkanime için terminal video oynatıcı ve indirici. İtinayla her bölümü indirir & oynatır.\n - Yığın bölüm indirebilir\n - Animu izleyebilir\n - Uygulama içinden arama yapabilir\n - Fansub seçtirebilir\n - Bir yandan izlerken bir yandan animeyi kaydedebilir\n - İndirmelere kaldığı yerden devam edebilir\n \n#### Desteklenen kaynaklar:\n```Sibnet, Odnoklassinki, Sendvid, Mail.ru, VK, Google+, Myvi, GoogleDrive, Yandisk, Vidmoly, Yourupload, Dailymotion```\n\n#### Yenilikler:\n - Seçim ekranı en son seçilen bölümden başlıyor, https://github.com/KebabLord/turkanime-indirici/discussions/35 https://github.com/KebabLord/turkanime-indirici/discussions/30\n - Aynı anda birden fazla bölüm indirme özelliği https://github.com/KebabLord/turkanime-indirici/pull/49\n - Önceden indirilen veya izlenen animelere izlendi ikonu seçeneği\n - Gereksinimleri uygulama içinden otomatik indirme\n\n\n\n# Kurulum\nÖnceden derlenmiş sürümleri [indirebilir](https://github.com/KebabLord/turkanime-indirici/releases/latest) ya da pip ile kolayca `pip install turkanime-cli` kurabilirsiniz. Pip ile kuruyorsanız, ya da scripti kaynak kodundan çalıştırıyorsanız mpv ve geckodriver'ın sisteminizde kurulu olduğundan ve sistem path'ında olduğundan emin olun. Konuya ilişkin rehber için [wiki sayfası](https://github.com/KebabLord/turkanime-indirici/wiki/Herhangi-bir-uygulamay%C4%B1-system-path'%C4%B1na-ekleme).\n\n ### İzleme ekranı\n ![indirme.gif](docs/ss_izle.gif)\n\n ### İndirme ekranı\n ![indirme.gif](docs/ss_indir.gif)\n\n### Yapılacaklar:\n - [ ] İndirme bitimi aksiyonları: bildirim veya bilgisayar kapatma.\n - [ ] Maximum çözünürlüğe ulaş.\n - [ ] Gui versiyon\n - [ ] Youtube-dl yerine yt-dlp'ye geçilmeli.\n - [ ] Selenium'dan kurtulma\n - [x] ~~Yeni sürüm var mı uygulama açılışında kontrol et.~~\n - [x] ~~Paralel anime indirme özelliği.~~\n - [x] ~~Progress yaratılma satırı minimal bir class ile kısaltılacak.~~\n - [x] ~~Domain güncellemesinden beridir kod stabil çalışmıyor, düzeltilecek.~~\n - [x] ~~Kod çorba gibi, basitleştirilecek.~~\n - [x] ~~Navigasyon ve indirme algoritması http talepleriyle sağlanacak.~~\n - [x] ~~Zaman bloğu olarak sleep'den kurtulunacak, elementin yüklenmesi beklenecek.~~\n - [x] ~~Prompt kütüphanesi olarak berbat durumda olan PyInquirer'den Questionary'e geçilecek.~~\n - [x] ~~Arama sonuçları da http talepleriyle getirilecek.~~\n - [x] ~~Fansub seçme özelliği tekrar eklenecek.~~\n",
     'author': 'Junicchi',
     'author_email': 'junicchi@waifu.club',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kebablord/turkanime-indirici',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `turkanime_cli-7.0.5/PKG-INFO` & `turkanime_cli-7.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turkanime-cli
-Version: 7.0.5
+Version: 7.1.0
 Summary: Türkanime video oynatıcı ve indirici
 Home-page: https://github.com/kebablord/turkanime-indirici
 License: CC-BY-NC-ND-4.0
 Keywords: turkanime,turk,anime,downloader
 Author: Junicchi
 Author-email: junicchi@waifu.club
 Requires-Python: >=3.6,<4
@@ -44,32 +44,39 @@
  - İndirmelere kaldığı yerden devam edebilir
  
 #### Desteklenen kaynaklar:
 ```Sibnet, Odnoklassinki, Sendvid, Mail.ru, VK, Google+, Myvi, GoogleDrive, Yandisk, Vidmoly, Yourupload, Dailymotion```
 
 #### Yenilikler:
  - Seçim ekranı en son seçilen bölümden başlıyor, https://github.com/KebabLord/turkanime-indirici/discussions/35 https://github.com/KebabLord/turkanime-indirici/discussions/30
+ - Aynı anda birden fazla bölüm indirme özelliği https://github.com/KebabLord/turkanime-indirici/pull/49
  - Önceden indirilen veya izlenen animelere izlendi ikonu seçeneği
- - Gereksinimleri otomatik indirme sistemi basitleştirildi
- - Dosya yönetim sistemi eklendi
- - Minimalleştirmeler & Hata gidermeleri
+ - Gereksinimleri uygulama içinden otomatik indirme
+
 
 
 # Kurulum
 Önceden derlenmiş sürümleri [indirebilir](https://github.com/KebabLord/turkanime-indirici/releases/latest) ya da pip ile kolayca `pip install turkanime-cli` kurabilirsiniz. Pip ile kuruyorsanız, ya da scripti kaynak kodundan çalıştırıyorsanız mpv ve geckodriver'ın sisteminizde kurulu olduğundan ve sistem path'ında olduğundan emin olun. Konuya ilişkin rehber için [wiki sayfası](https://github.com/KebabLord/turkanime-indirici/wiki/Herhangi-bir-uygulamay%C4%B1-system-path'%C4%B1na-ekleme).
 
  ### İzleme ekranı
  ![indirme.gif](docs/ss_izle.gif)
 
  ### İndirme ekranı
  ![indirme.gif](docs/ss_indir.gif)
 
 ### Yapılacaklar:
- - Progress yaratılma satırı minimal bir class ile kısaltılacak.
- - ~~Domain güncellemesinden beridir kod stabil çalışmıyor, düzeltilecek.~~
- - ~~Kod çorba gibi, basitleştirilecek.~~
- - ~~Navigasyon  ve indirme algoritması http talepleriyle sağlanacak.~~
- - ~~Zaman bloğu olarak sleep'den kurtulunacak, elementin yüklenmesi beklenecek.~~
- - ~~Prompt kütüphanesi olarak berbat durumda olan PyInquirer'den Questionary'e geçilecek.~~
- - ~~Arama sonuçları da http talepleriyle getirilecek.~~
- - ~~Fansub seçme özelliği tekrar eklenecek.~~
+ - [ ] İndirme bitimi aksiyonları: bildirim veya bilgisayar kapatma.
+ - [ ] Maximum çözünürlüğe ulaş.
+ - [ ] Gui versiyon
+ - [ ] Youtube-dl yerine yt-dlp'ye geçilmeli.
+ - [ ] Selenium'dan kurtulma
+ - [x] ~~Yeni sürüm var mı uygulama açılışında kontrol et.~~
+ - [x] ~~Paralel anime indirme özelliği.~~
+ - [x] ~~Progress yaratılma satırı minimal bir class ile kısaltılacak.~~
+ - [x] ~~Domain güncellemesinden beridir kod stabil çalışmıyor, düzeltilecek.~~
+ - [x] ~~Kod çorba gibi, basitleştirilecek.~~
+ - [x] ~~Navigasyon ve indirme algoritması http talepleriyle sağlanacak.~~
+ - [x] ~~Zaman bloğu olarak sleep'den kurtulunacak, elementin yüklenmesi beklenecek.~~
+ - [x] ~~Prompt kütüphanesi olarak berbat durumda olan PyInquirer'den Questionary'e geçilecek.~~
+ - [x] ~~Arama sonuçları da http talepleriyle getirilecek.~~
+ - [x] ~~Fansub seçme özelliği tekrar eklenecek.~~
```

