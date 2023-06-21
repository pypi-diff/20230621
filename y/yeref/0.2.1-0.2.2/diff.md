# Comparing `tmp/yeref-0.2.1.tar.gz` & `tmp/yeref-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.2.1.tar", last modified: Mon Jun 19 18:19:22 2023, max compression
+gzip compressed data, was "yeref-0.2.2.tar", last modified: Wed Jun 21 12:17:20 2023, max compression
```

## Comparing `yeref-0.2.1.tar` & `yeref-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-19 18:19:22.342320 yeref-0.2.1/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-19 18:19:22.342550 yeref-0.2.1/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-19 18:19:22.343498 yeref-0.2.1/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-19 18:18:30.000000 yeref-0.2.1/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-19 18:19:22.334951 yeref-0.2.1/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.1/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   557022 2023-06-19 17:17:09.000000 yeref-0.2.1/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   210940 2023-06-19 18:18:21.000000 yeref-0.2.1/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-19 18:19:22.341692 yeref-0.2.1/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-19 18:19:22.000000 yeref-0.2.1/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-19 18:19:22.000000 yeref-0.2.1/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-19 18:19:22.000000 yeref-0.2.1/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-19 18:19:22.000000 yeref-0.2.1/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-21 12:17:20.873908 yeref-0.2.2/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-21 12:17:20.874122 yeref-0.2.2/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-21 12:17:20.874973 yeref-0.2.2/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-21 12:16:57.000000 yeref-0.2.2/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-21 12:17:20.868009 yeref-0.2.2/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.2/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   558227 2023-06-21 12:16:57.000000 yeref-0.2.2/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   210940 2023-06-19 18:18:21.000000 yeref-0.2.2/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-21 12:17:20.873318 yeref-0.2.2/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-21 12:17:20.000000 yeref-0.2.2/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-21 12:17:20.000000 yeref-0.2.2/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-21 12:17:20.000000 yeref-0.2.2/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-21 12:17:20.000000 yeref-0.2.2/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.2.1/setup.py` & `yeref-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.2.01',
+      version='0.2.02',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -36,15 +36,14 @@
 # python setup.py install
 # python setup.py develop
 #
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
-
 # twine upload dist/*
 # freey.sitner.ya
 # cejwez-nosgin-vaVfe7
 
 # python3 -m pip install --upgrade yeref
 
 # python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.99-py3-none-any.whl
```

### Comparing `yeref-0.2.1/yeref/l_.py` & `yeref-0.2.2/yeref/l_.py`

 * *Files 1% similar despite different names*

```diff
@@ -1791,20 +1791,28 @@
     'ru': "<figure><img src='{0}'/><figcaption>Фото профиля: @{1}</figcaption></figure><blockquote>Лэндинг-блог для продвижения в <i>Telegram</i></blockquote>👩🏽‍💻 <b>бот:</b> {2}<br>[<b>id</b>={3}]<br><b>Био:</b> {4}<br><aside>Описание</aside>{5}",
     'en': "Profile photo: @{1}Landing blog for promotion in <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = {3}] <b>Bio:</b> {4}Description{5}",
     'es': "Foto de perfil: @{1}Blog de aterrizaje para promoción en <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = {3}] <b>Bio:</b> {4}Descripción{5}",
     'fr': "Photo de profil : @{1}Blog d'atterrissage pour la promotion dans <i>Telegram</i> 👩🏽‍💻 <b>bot :</b> {2}[<b>id</b> = {3}] <b>Bio :</b> {4}Description{5}",
     'zh': "个人资料照片：@{1}登陆博客以在<i>Telegram</i> 👩🏽‍💻<b>机器人中进行推广：</b> {2}[<b>id</b> = {3}]<b>简介：</b> {4}说明{5}",
     'ar': "صورة الملف الشخصي: @ {1} مدونة الهبوط للترويج في <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2} [<b>id</b> = {3}] <b>السيرة الذاتية:</b> {4} الوصف {5}",
 }
+l_no_permission_table = {
+    'ru': "👩🏽‍💻 <b>Нет прав</b> для записи в данную таблицу: {0}\n\n👩🏽‍💻 <b>Необходимо</b> заново добавить корректную ссылку на таблицу в @{1}-боте",
+    'en': "Profile photo: @{1}Landing blog for promotion in <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = {3}] <b>Bio:</b> {4}Description{5}",
+    'es': "Foto de perfil: @{1}Blog de aterrizaje para promoción en <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = {3}] <b>Bio:</b> {4}Descripción{5}",
+    'fr': "Photo de profil : @{1}Blog d'atterrissage pour la promotion dans <i>Telegram</i> 👩🏽‍💻 <b>bot :</b> {2}[<b>id</b> = {3}] <b>Bio :</b> {4}Description{5}",
+    'zh': "个人资料照片：@{1}登陆博客以在<i>Telegram</i> 👩🏽‍💻<b>机器人中进行推广：</b> {2}[<b>id</b> = {3}]<b>简介：</b> {4}说明{5}",
+    'ar': "صورة الملف الشخصي: @ {1} مدونة الهبوط للترويج في <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2} [<b>id</b> = {3}] <b>السيرة الذاتية:</b> {4} الوصف {5}",
+}
 # endregion
 
 
 # region extra bot
 l_show_admin_panel_md = {
-    'ru': "*👩🏽‍💻 Создание и редактирование блога*\n\n👩🏽‍💻 Вы зашли как *Администратор* и можете создавать и редактировать блоги, но не удалять их\n\n¹ Авторизация по ссылке в браузере:\n`{0}`\n\n² Перейди (в течение 10сек) по нужной ссылке для редактирования публикации (жми, чтобы скопировать):\n\n",
+    'ru': "*👩🏽‍💻 Создание и редактирование блога*\n\n👩🏽‍💻 Вы зашли как *Администратор* и можете создавать и редактировать блоги, но не удалять их\n\n¹ Авторизация (в течение 10сек) по ссылке в браузере:\n`{0}`\n\n² Перейди (в течение 10сек) по нужной ссылке для редактирования публикации (жми, чтобы скопировать):\n\n",
     'en': "*👩🏽‍💻 Creating and editing a blog*\n\n👩🏽‍💻 You are logged in as *Administrator* and can create and edit blogs, but not delete them\n\n¹ Authorization via link in browser:\n`{0 }`\n\n² Go (within 10 seconds) to the desired link to edit the post (click to copy):\n\n",
     'es': "*👩🏽‍💻 Crear y editar un blog*\n\n👩🏽‍💻 Ha iniciado sesión como *Administrador* y puede crear y editar blogs, pero no eliminarlos\n\n¹ Autorización a través de un enlace en el navegador:\n`{0 }`\n\n² Vaya (dentro de 10 segundos) al enlace deseado para editar la publicación (haga clic para copiar):\n\n",
     'fr': "*👩🏽‍💻 Créer et modifier un blog*\n\n👩🏽‍💻 Vous êtes connecté en tant qu'*administrateur* et vous pouvez créer et modifier des blogs, mais pas les supprimer\n\n¹ Autorisation via un lien dans le navigateur :\n`{0 }`\n\n² Accédez (dans les 10 secondes) au lien souhaité pour modifier le message (cliquez pour copier) :\n\n",
     'zh': "*👩🏽‍💻 创建和编辑博客*\n\n👩🏽‍💻 您以*管理员*身份登录，可以创建和编辑博客，但不能删除它们\n\n¹ 通过浏览器中的链接授权：\n`{0 }`\n\n²（在 10 秒内）转到所需的链接以编辑帖子（单击以复制）：\n\n",
     'ar': "* 👩🏽‍💻 إنشاء مدونة وتحريرها *\n\n👩🏽‍💻 تم تسجيل دخولك بصفتك * المسؤول * ويمكنك إنشاء المدونات وتحريرها ، ولكن لا يمكنك حذفها\n\n¹ التفويض عبر الارتباط في المستعرض:\n'{0}`\n\n² انتقل (في غضون 10 ثوانٍ) إلى الرابط المطلوب لتعديل المشاركة (انقر للنسخ):\n\n",
 }
 l_show_admin_panel_html = {
```

### Comparing `yeref-0.2.1/yeref/yeref.py` & `yeref-0.2.2/yeref/yeref.py`

 * *Files identical despite different names*

