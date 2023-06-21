# Comparing `tmp/webp3-0.6.0.tar.gz` & `tmp/webp3-0.7.0.tar.gz`

## Comparing `webp3-0.6.0.tar` & `webp3-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 webp3-0.6.0/apache/install-webp3.rst
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 webp3-0.6.0/apache/install-webp3.sh
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 webp3-0.6.0/apache/webp3.conf
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/__init__.py
--rwxr-xr-x   0        0        0      820 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/__main__.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/app.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/conf.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/exceptions.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/main_wsgi.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/pathutils.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/requestutils.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/webp3.wsgi
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/static/COPYING.WTFPL
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/static/base.tpl
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/static/favicon.png
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/static/player.js
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 webp3-0.6.0/webp3/static/style.css
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 webp3-0.6.0/.gitignore
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 webp3-0.6.0/COPYING.WTFPL
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 webp3-0.6.0/README.rst
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 webp3-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 webp3-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 webp3-0.7.0/apache/install-webp3.rst
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 webp3-0.7.0/apache/install-webp3.sh
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 webp3-0.7.0/apache/webp3.conf
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 webp3-0.7.0/webp3/__init__.py
+-rwxr-xr-x   0        0        0      978 2020-02-02 00:00:00.000000 webp3-0.7.0/webp3/__main__.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 webp3-0.7.0/webp3/app.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 webp3-0.7.0/webp3/conf.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 webp3-0.7.0/webp3/exceptions.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 webp3-0.7.0/webp3/main_wsgi.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 webp3-0.7.0/webp3/pathutils.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 webp3-0.7.0/webp3/requestutils.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 webp3-0.7.0/webp3/webp3.wsgi
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 webp3-0.7.0/webp3/static/COPYING.WTFPL
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 webp3-0.7.0/webp3/static/base.tpl
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 webp3-0.7.0/webp3/static/favicon.png
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 webp3-0.7.0/webp3/static/player.js
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 webp3-0.7.0/webp3/static/style.css
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 webp3-0.7.0/.gitignore
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 webp3-0.7.0/COPYING.WTFPL
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 webp3-0.7.0/README.rst
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 webp3-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 webp3-0.7.0/PKG-INFO
```

### Comparing `webp3-0.6.0/apache/install-webp3.sh` & `webp3-0.7.0/apache/install-webp3.sh`

 * *Files identical despite different names*

### Comparing `webp3-0.6.0/webp3/__main__.py` & `webp3-0.7.0/webp3/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 #!/usr/bin/env python3
 # SPDX-License-Identifier: WTFPL
 
 import argparse
 from pathlib import Path
+import os
 
 from . import conf
 
 
 def main():
 	from .app import bapp
 
 	parser = argparse.ArgumentParser()
 	parser.add_argument('folders', metavar='NAME=PATH', nargs='+', help='give access to PATH under /NAME/')
 	parser.add_argument('-p', '--port', metavar='PORT', default=8000, type=int, help='listen on PORT')
+	parser.add_argument('-b', '--base-url', help='Absolute URLs start at BASE_URL')
 	args = parser.parse_args()
 
 	conf.ROOTS = {}
 
 	for fstr in args.folders:
 		fdata = fstr.split('=', 1)
 		if len(fdata) != 2 or not all(fdata):
 			parser.error('folders must be with format NAME=PATH')
 		key = fdata[0]
 		if key in conf.ROOTS:
 			parser.error('roots can only be specified once: %s' % key)
 		conf.ROOTS[key] = Path(fdata[1])
 
+	conf.BASE_URL = args.base_url or os.environ.get("WEBP3_BASEURL")
+
 	bapp.run(host='', port=args.port, debug=True)
 
 
 if __name__ == '__main__':
 	main()
```

### Comparing `webp3-0.6.0/webp3/app.py` & `webp3-0.7.0/webp3/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,22 @@
 		'path': path,
 	}
 
 
 bapp = Bottle()
 
 
+def build_absolute_url(req, name: str) -> str:
+	path = str(req.path)
+	if conf.BASE_URL:
+		return "/".join((conf.BASE_URL.rstrip("/"), req.tree, path, urlquote(name)))
+	else:
+		return urljoin(request.url, urlquote(name))
+
+
 @base_request
 def ls_dir(req: Request):
 	files = list(req.target.iterdir())
 
 	natural_sort_ci(files)
 
 	etag = gen_etag(files, path=req.target, weak=True)
@@ -50,15 +58,15 @@
 	files = [i['basename'] for i in items if is_audio(i['path'])]
 
 	if is_json_request():
 		response.headers['Content-Type'] = 'application/json'
 		body = json.dumps(items)
 	elif is_m3u_request():
 		response.headers['Content-Type'] = 'audio/x-mpegurl'
-		body = ''.join(urljoin(request.url, urlquote(f)) + '\n' for f in files)
+		body = ''.join(build_absolute_url(req, f) + '\n' for f in files)
 	else:
 		response.headers['Content-Type'] = 'text/html'
 		body = mako_template(
 			conf.TEMPLATE,
 			items=items,
 			files=files,
 			relpath=Path('/').joinpath(req.path),
```

### Comparing `webp3-0.6.0/webp3/main_wsgi.py` & `webp3-0.7.0/webp3/main_wsgi.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
 			if key in roots:
 				raise RuntimeError('duplicate key %r' % key)
 
 			roots[key] = Path(dest)
 		webp3.conf.ROOTS = roots
 
+	webp3.conf.BASE_URL = os.environ.get("WEBP3_BASEURL")
+
 
 def decorate(func):
 	def wrapper(environ, starter):
 		read_conf(environ)
 		return func(environ, starter)
 
 	return wrapper
```

### Comparing `webp3-0.6.0/webp3/pathutils.py` & `webp3-0.7.0/webp3/pathutils.py`

 * *Files identical despite different names*

### Comparing `webp3-0.6.0/webp3/requestutils.py` & `webp3-0.7.0/webp3/requestutils.py`

 * *Files identical despite different names*

### Comparing `webp3-0.6.0/webp3/webp3.wsgi` & `webp3-0.7.0/webp3/webp3.wsgi`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 
 			if key in roots:
 				raise RuntimeError('duplicate key %r' % key)
 
 			roots[key] = Path(dest)
 		webp3.conf.ROOTS = roots
 
+	webp3.conf.BASE_URL = os.environ.get("WEBP3_BASEURL")
+
 
 def decorate(func):
 	def wrapper(environ, starter):
 		read_conf(environ)
 		return func(environ, starter)
 
 	return wrapper
```

### Comparing `webp3-0.6.0/webp3/static/COPYING.WTFPL` & `webp3-0.7.0/webp3/static/COPYING.WTFPL`

 * *Files identical despite different names*

### Comparing `webp3-0.6.0/webp3/static/base.tpl` & `webp3-0.7.0/webp3/static/base.tpl`

 * *Files identical despite different names*

### Comparing `webp3-0.6.0/webp3/static/favicon.png` & `webp3-0.7.0/webp3/static/favicon.png`

 * *Files identical despite different names*

### Comparing `webp3-0.6.0/webp3/static/player.js` & `webp3-0.7.0/webp3/static/player.js`

 * *Files identical despite different names*

### Comparing `webp3-0.6.0/webp3/static/style.css` & `webp3-0.7.0/webp3/static/style.css`

 * *Files identical despite different names*

### Comparing `webp3-0.6.0/README.rst` & `webp3-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `webp3-0.6.0/pyproject.toml` & `webp3-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `webp3-0.6.0/PKG-INFO` & `webp3-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webp3
-Version: 0.6.0
+Version: 0.7.0
 Summary: Music player web app
 Project-URL: Homepage, https://gitlab.com/hydrargyrum/webp3
 Author-email: Hg <dev@indigo.re>
 License-Expression: WTFPL
 License-File: COPYING.WTFPL
 Keywords: audio,html5,music,player,server,web
 Classifier: Development Status :: 4 - Beta
```

