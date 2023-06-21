# Comparing `tmp/edxbackup-3.1.1.tar.gz` & `tmp/edxbackup-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edxbackup-3.1.1.tar", last modified: Mon Jun  5 12:59:05 2023, max compression
+gzip compressed data, was "edxbackup-3.2.1.tar", last modified: Wed Jun 21 14:58:15 2023, max compression
```

## Comparing `edxbackup-3.1.1.tar` & `edxbackup-3.2.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.992704 edxbackup-3.1.1/
--rw-r--r--   0 snglth    (1000) users      (100)        8 2023-01-31 10:12:41.000000 edxbackup-3.1.1/.dockerignore
--rw-r--r--   0 snglth    (1000) users      (100)      395 2023-05-23 14:56:08.000000 edxbackup-3.1.1/.envrc
--rw-r--r--   0 snglth    (1000) users      (100)      125 2023-01-31 10:12:41.000000 edxbackup-3.1.1/.flake8
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.986704 edxbackup-3.1.1/.github/
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.988704 edxbackup-3.1.1/.github/workflows/
--rw-r--r--   0 snglth    (1000) users      (100)      809 2023-05-23 14:56:08.000000 edxbackup-3.1.1/.github/workflows/lint.yml
--rw-r--r--   0 snglth    (1000) users      (100)      100 2023-05-23 14:56:08.000000 edxbackup-3.1.1/.gitignore
--rw-r--r--   0 snglth    (1000) users      (100)      173 2023-01-31 10:12:41.000000 edxbackup-3.1.1/.isort.cfg
--rw-r--r--   0 snglth    (1000) users      (100)      598 2023-05-23 14:56:08.000000 edxbackup-3.1.1/.pre-commit-config.yaml
--rw-r--r--   0 snglth    (1000) users      (100)     1060 2023-05-23 14:56:08.000000 edxbackup-3.1.1/Dockerfile
--rw-r--r--   0 snglth    (1000) users      (100)    11357 2023-06-05 12:45:15.000000 edxbackup-3.1.1/LICENSE
--rw-r--r--   0 snglth    (1000) users      (100)     1132 2023-06-05 12:59:05.992704 edxbackup-3.1.1/PKG-INFO
--rw-r--r--   0 snglth    (1000) users      (100)      849 2023-05-23 14:56:08.000000 edxbackup-3.1.1/README.md
--rw-r--r--   0 snglth    (1000) users      (100)      876 2023-06-05 12:45:15.000000 edxbackup-3.1.1/README.rst
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.988704 edxbackup-3.1.1/contrib/
--rw-r--r--   0 snglth    (1000) users      (100)     1443 2023-05-23 14:56:08.000000 edxbackup-3.1.1/contrib/delete_old.py
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.990704 edxbackup-3.1.1/edxbackup/
--rw-r--r--   0 snglth    (1000) users      (100)       18 2023-06-05 12:58:04.000000 edxbackup-3.1.1/edxbackup/__init__.py
--rw-r--r--   0 snglth    (1000) users      (100)     1679 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/backup.py
--rw-r--r--   0 snglth    (1000) users      (100)      637 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/cli.py
--rw-r--r--   0 snglth    (1000) users      (100)      278 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/config.py
--rw-r--r--   0 snglth    (1000) users      (100)     2871 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/context.py
--rw-r--r--   0 snglth    (1000) users      (100)      837 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/info.py
--rw-r--r--   0 snglth    (1000) users      (100)     1831 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/mongo.py
--rw-r--r--   0 snglth    (1000) users      (100)     1857 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/mysql.py
--rw-r--r--   0 snglth    (1000) users      (100)      447 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/options.py
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.992704 edxbackup-3.1.1/edxbackup/restic/
--rw-r--r--   0 snglth    (1000) users      (100)      912 2023-06-05 12:56:46.000000 edxbackup-3.1.1/edxbackup/restic/backup.py
--rw-r--r--   0 snglth    (1000) users      (100)      587 2023-06-05 12:56:57.000000 edxbackup-3.1.1/edxbackup/restic/restore.py
--rw-r--r--   0 snglth    (1000) users      (100)     1189 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/restic/snapshot.py
--rw-r--r--   0 snglth    (1000) users      (100)     2664 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/restore.py
--rw-r--r--   0 snglth    (1000) users      (100)     1744 2023-06-05 12:45:15.000000 edxbackup-3.1.1/edxbackup/s3.py
--rw-r--r--   0 snglth    (1000) users      (100)      384 2023-05-23 14:56:08.000000 edxbackup-3.1.1/edxbackup/utils.py
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.990704 edxbackup-3.1.1/edxbackup.egg-info/
--rw-r--r--   0 snglth    (1000) users      (100)     1132 2023-06-05 12:59:05.000000 edxbackup-3.1.1/edxbackup.egg-info/PKG-INFO
--rw-r--r--   0 snglth    (1000) users      (100)      943 2023-06-05 12:59:05.000000 edxbackup-3.1.1/edxbackup.egg-info/SOURCES.txt
--rw-r--r--   0 snglth    (1000) users      (100)        1 2023-06-05 12:59:05.000000 edxbackup-3.1.1/edxbackup.egg-info/dependency_links.txt
--rw-r--r--   0 snglth    (1000) users      (100)       49 2023-06-05 12:59:05.000000 edxbackup-3.1.1/edxbackup.egg-info/entry_points.txt
--rw-r--r--   0 snglth    (1000) users      (100)       29 2023-06-05 12:59:05.000000 edxbackup-3.1.1/edxbackup.egg-info/requires.txt
--rw-r--r--   0 snglth    (1000) users      (100)       45 2023-06-05 12:59:05.000000 edxbackup-3.1.1/edxbackup.egg-info/top_level.txt
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.992704 edxbackup-3.1.1/example/
--rw-r--r--   0 snglth    (1000) users      (100)      560 2023-05-23 14:56:08.000000 edxbackup-3.1.1/example/edxbackup.json
--rw-r--r--   0 snglth    (1000) users      (100)      606 2023-06-05 12:55:53.000000 edxbackup-3.1.1/pyproject.toml
--rw-r--r--   0 snglth    (1000) users      (100)       37 2023-06-01 16:33:13.000000 edxbackup-3.1.1/pytest.ini
--rw-r--r--   0 snglth    (1000) users      (100)      495 2023-06-05 12:55:58.000000 edxbackup-3.1.1/requirements.txt
--rw-r--r--   0 snglth    (1000) users      (100)       38 2023-06-05 12:59:05.992704 edxbackup-3.1.1/setup.cfg
--rw-r--r--   0 snglth    (1000) users      (100)       98 2023-06-05 12:45:27.000000 edxbackup-3.1.1/shell.nix
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.992704 edxbackup-3.1.1/systemd/
--rw-r--r--   0 snglth    (1000) users      (100)      288 2023-05-23 14:56:08.000000 edxbackup-3.1.1/systemd/edxbackup.service
--rw-r--r--   0 snglth    (1000) users      (100)      131 2023-05-23 14:56:08.000000 edxbackup-3.1.1/systemd/edxbackup.timer
-drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-05 12:59:05.992704 edxbackup-3.1.1/tests/
--rw-r--r--   0 snglth    (1000) users      (100)       20 2023-05-23 14:56:08.000000 edxbackup-3.1.1/tests/README.md
--rw-r--r--   0 snglth    (1000) users      (100)     1180 2023-05-23 14:56:08.000000 edxbackup-3.1.1/tests/docker-compose.yml
--rw-r--r--   0 snglth    (1000) users      (100)      438 2023-05-23 14:56:08.000000 edxbackup-3.1.1/tests/edxbackup.json
--rwxr-xr-x   0 snglth    (1000) users      (100)      370 2023-05-23 14:56:08.000000 edxbackup-3.1.1/tests/integration.sh
--rw-r--r--   0 snglth    (1000) users      (100)     1157 2023-05-23 14:56:08.000000 edxbackup-3.1.1/tests/populate.sh
--rw-r--r--   0 snglth    (1000) users      (100)      330 2023-05-23 14:56:08.000000 edxbackup-3.1.1/tests/retention.py
--rw-r--r--   0 snglth    (1000) users      (100)      391 2023-05-23 14:56:08.000000 edxbackup-3.1.1/tests/testenv.sh
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-21 14:58:15.237336 edxbackup-3.2.1/
+-rw-r--r--   0 snglth    (1000) users      (100)        8 2023-01-31 10:12:41.000000 edxbackup-3.2.1/.dockerignore
+-rw-r--r--   0 snglth    (1000) users      (100)      395 2023-05-23 14:56:08.000000 edxbackup-3.2.1/.envrc
+-rw-r--r--   0 snglth    (1000) users      (100)      125 2023-01-31 10:12:41.000000 edxbackup-3.2.1/.flake8
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-21 14:58:15.227336 edxbackup-3.2.1/.github/
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-21 14:58:15.231336 edxbackup-3.2.1/.github/workflows/
+-rw-r--r--   0 snglth    (1000) users      (100)      809 2023-05-23 14:56:08.000000 edxbackup-3.2.1/.github/workflows/lint.yml
+-rw-r--r--   0 snglth    (1000) users      (100)      100 2023-05-23 14:56:08.000000 edxbackup-3.2.1/.gitignore
+-rw-r--r--   0 snglth    (1000) users      (100)      173 2023-01-31 10:12:41.000000 edxbackup-3.2.1/.isort.cfg
+-rw-r--r--   0 snglth    (1000) users      (100)      598 2023-05-23 14:56:08.000000 edxbackup-3.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 snglth    (1000) users      (100)     1163 2023-06-20 09:55:41.000000 edxbackup-3.2.1/Dockerfile
+-rw-r--r--   0 snglth    (1000) users      (100)    11357 2023-06-05 12:45:15.000000 edxbackup-3.2.1/LICENSE
+-rw-r--r--   0 snglth    (1000) users      (100)     2491 2023-06-21 14:58:15.237336 edxbackup-3.2.1/PKG-INFO
+-rw-r--r--   0 snglth    (1000) users      (100)     2235 2023-06-08 15:47:18.000000 edxbackup-3.2.1/README.rst
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-21 14:58:15.231336 edxbackup-3.2.1/contrib/
+-rw-r--r--   0 snglth    (1000) users      (100)     1443 2023-05-23 14:56:08.000000 edxbackup-3.2.1/contrib/delete_old.py
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-21 14:58:15.233336 edxbackup-3.2.1/edxbackup/
+-rw-r--r--   0 snglth    (1000) users      (100)       18 2023-06-21 14:56:49.000000 edxbackup-3.2.1/edxbackup/__init__.py
+-rw-r--r--   0 snglth    (1000) users      (100)     2139 2023-06-21 14:55:06.000000 edxbackup-3.2.1/edxbackup/backup.py
+-rw-r--r--   0 snglth    (1000) users      (100)      637 2023-05-23 14:56:08.000000 edxbackup-3.2.1/edxbackup/cli.py
+-rw-r--r--   0 snglth    (1000) users      (100)      367 2023-06-20 09:55:41.000000 edxbackup-3.2.1/edxbackup/config.py
+-rw-r--r--   0 snglth    (1000) users      (100)     3769 2023-06-20 10:13:43.000000 edxbackup-3.2.1/edxbackup/context.py
+-rw-r--r--   0 snglth    (1000) users      (100)      837 2023-05-23 14:56:08.000000 edxbackup-3.2.1/edxbackup/info.py
+-rw-r--r--   0 snglth    (1000) users      (100)     2187 2023-06-20 10:13:20.000000 edxbackup-3.2.1/edxbackup/mongo.py
+-rw-r--r--   0 snglth    (1000) users      (100)     1857 2023-06-07 22:23:58.000000 edxbackup-3.2.1/edxbackup/mysql.py
+-rw-r--r--   0 snglth    (1000) users      (100)      447 2023-05-23 14:56:08.000000 edxbackup-3.2.1/edxbackup/options.py
+-rw-r--r--   0 snglth    (1000) users      (100)     2098 2023-06-20 10:13:43.000000 edxbackup-3.2.1/edxbackup/postgresql.py
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-21 14:58:15.233336 edxbackup-3.2.1/edxbackup/restic/
+-rw-r--r--   0 snglth    (1000) users      (100)      912 2023-06-05 12:56:46.000000 edxbackup-3.2.1/edxbackup/restic/backup.py
+-rw-r--r--   0 snglth    (1000) users      (100)      587 2023-06-05 12:56:57.000000 edxbackup-3.2.1/edxbackup/restic/restore.py
+-rw-r--r--   0 snglth    (1000) users      (100)     1189 2023-05-23 14:56:08.000000 edxbackup-3.2.1/edxbackup/restic/snapshot.py
+-rw-r--r--   0 snglth    (1000) users      (100)     3462 2023-06-20 10:13:43.000000 edxbackup-3.2.1/edxbackup/restore.py
+-rw-r--r--   0 snglth    (1000) users      (100)     1744 2023-06-05 12:45:15.000000 edxbackup-3.2.1/edxbackup/s3.py
+-rw-r--r--   0 snglth    (1000) users      (100)      384 2023-05-23 14:56:08.000000 edxbackup-3.2.1/edxbackup/utils.py
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-21 14:58:15.233336 edxbackup-3.2.1/edxbackup.egg-info/
+-rw-r--r--   0 snglth    (1000) users      (100)     2491 2023-06-21 14:58:15.000000 edxbackup-3.2.1/edxbackup.egg-info/PKG-INFO
+-rw-r--r--   0 snglth    (1000) users      (100)      957 2023-06-21 14:58:15.000000 edxbackup-3.2.1/edxbackup.egg-info/SOURCES.txt
+-rw-r--r--   0 snglth    (1000) users      (100)        1 2023-06-21 14:58:15.000000 edxbackup-3.2.1/edxbackup.egg-info/dependency_links.txt
+-rw-r--r--   0 snglth    (1000) users      (100)       49 2023-06-21 14:58:15.000000 edxbackup-3.2.1/edxbackup.egg-info/entry_points.txt
+-rw-r--r--   0 snglth    (1000) users      (100)       29 2023-06-21 14:58:15.000000 edxbackup-3.2.1/edxbackup.egg-info/requires.txt
+-rw-r--r--   0 snglth    (1000) users      (100)       45 2023-06-21 14:58:15.000000 edxbackup-3.2.1/edxbackup.egg-info/top_level.txt
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-21 14:58:15.233336 edxbackup-3.2.1/example/
+-rw-r--r--   0 snglth    (1000) users      (100)      560 2023-05-23 14:56:08.000000 edxbackup-3.2.1/example/edxbackup.json
+-rw-r--r--   0 snglth    (1000) users      (100)      606 2023-06-05 12:55:53.000000 edxbackup-3.2.1/pyproject.toml
+-rw-r--r--   0 snglth    (1000) users      (100)       37 2023-06-01 16:33:13.000000 edxbackup-3.2.1/pytest.ini
+-rw-r--r--   0 snglth    (1000) users      (100)      495 2023-06-05 12:55:58.000000 edxbackup-3.2.1/requirements.txt
+-rw-r--r--   0 snglth    (1000) users      (100)       38 2023-06-21 14:58:15.237336 edxbackup-3.2.1/setup.cfg
+-rw-r--r--   0 snglth    (1000) users      (100)      159 2023-06-20 10:11:33.000000 edxbackup-3.2.1/shell.nix
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-21 14:58:15.235336 edxbackup-3.2.1/systemd/
+-rw-r--r--   0 snglth    (1000) users      (100)      288 2023-05-23 14:56:08.000000 edxbackup-3.2.1/systemd/edxbackup.service
+-rw-r--r--   0 snglth    (1000) users      (100)      131 2023-05-23 14:56:08.000000 edxbackup-3.2.1/systemd/edxbackup.timer
+drwxr-xr-x   0 snglth    (1000) users      (100)        0 2023-06-21 14:58:15.235336 edxbackup-3.2.1/tests/
+-rw-r--r--   0 snglth    (1000) users      (100)       20 2023-05-23 14:56:08.000000 edxbackup-3.2.1/tests/README.md
+-rw-r--r--   0 snglth    (1000) users      (100)     1376 2023-06-20 10:06:30.000000 edxbackup-3.2.1/tests/docker-compose.yml
+-rw-r--r--   0 snglth    (1000) users      (100)      531 2023-06-20 10:11:33.000000 edxbackup-3.2.1/tests/edxbackup.json
+-rwxr-xr-x   0 snglth    (1000) users      (100)      370 2023-05-23 14:56:08.000000 edxbackup-3.2.1/tests/integration.sh
+-rw-r--r--   0 snglth    (1000) users      (100)     1157 2023-06-20 10:08:17.000000 edxbackup-3.2.1/tests/populate.sh
+-rw-r--r--   0 snglth    (1000) users      (100)      330 2023-05-23 14:56:08.000000 edxbackup-3.2.1/tests/retention.py
+-rw-r--r--   0 snglth    (1000) users      (100)      450 2023-06-20 09:55:41.000000 edxbackup-3.2.1/tests/testenv.sh
```

### Comparing `edxbackup-3.1.1/.github/workflows/lint.yml` & `edxbackup-3.2.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.1/.pre-commit-config.yaml` & `edxbackup-3.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.1/Dockerfile` & `edxbackup-3.2.1/Dockerfile`

 * *Files 15% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 ARG mongodb_version=100.7.0
 ARG restic_version=0.15.1
 
 ENV MYDUMPER_VERSION=${mydumper_version}
 ENV MONGOTOOLS_VERSION=${mongodb_version}
 ENV RESTIC_VERSION=${restic_version}
 
-RUN apt-get update && apt-get install -y bzip2 curl
+RUN apt-get update && apt-get install -y bzip2 curl postgresql-client-common postgresql-client-13
 
 RUN curl -LO https://github.com/mydumper/mydumper/releases/download/v${MYDUMPER_VERSION}/mydumper_${MYDUMPER_VERSION}-zstd.bullseye_amd64.deb && \
     apt install -y ./mydumper*.deb && rm ./mydumper*.deb
 
 RUN curl -LO https://fastdl.mongodb.org/tools/db/mongodb-database-tools-debian11-x86_64-${MONGOTOOLS_VERSION}.deb && \
     apt install -y ./mongodb-database-tools*.deb && rm ./mongodb-database-tools*.deb
 
 RUN curl -L https://github.com/restic/restic/releases/download/v${RESTIC_VERSION}/restic_${RESTIC_VERSION}_linux_amd64.bz2 | \
 	bunzip2 > /usr/local/bin/restic && chmod +x /usr/local/bin/restic
 
 COPY requirements.txt pyproject.toml /app/
 COPY edxbackup /app/edxbackup
 
+COPY contrib/delete_old.py /usr/local/bin/delete_old.py
+
 RUN pip install -r /app/requirements.txt && pip install /app
```

### Comparing `edxbackup-3.1.1/LICENSE` & `edxbackup-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.1/contrib/delete_old.py` & `edxbackup-3.2.1/contrib/delete_old.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.1/edxbackup/backup.py` & `edxbackup-3.2.1/edxbackup/backup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from edxbackup.config import EdxbackupConfig
 from edxbackup.mongo import dump_mongo_db
 from edxbackup.mysql import dump_mysql_db
+from edxbackup.postgresql import dump_postgresql_db
 from edxbackup.options import backup_time_option
 from edxbackup.options import config_path_option
 from edxbackup.s3 import dump_s3_bucket
 from edxbackup.utils import log_failure
 from edxbackup.utils import log_success
 
 import click
@@ -35,14 +36,24 @@
         if dump_mysql_db(mysql_config, config.prefix, backup_id, time):
             log_success(f"edxbackup backed up mysql database: {mysql_config.database}")
         else:
             log_failure(
                 f"edxbackup failed to backup mysql database: {mysql_config.database}"
             )
 
+    for postgresql_config in config.postgresql:
+        if dump_postgresql_db(postgresql_config, config.prefix, backup_id, time):
+            log_success(
+                f"edxbackup backed up postgresql database: {postgresql_config.database}"
+            )
+        else:
+            log_failure(
+                f"edxbackup failed to backup postgresql database: {postgresql_config.database}"
+            )
+
     for s3_config in config.s3:
         if dump_s3_bucket(s3_config, config.prefix, backup_id, time):
             log_success(f"edxbackup backed up S3 bucket: {s3_config.bucket}")
         else:
             log_failure(f"edxbackup failed to backup S3 bucket: {s3_config.bucket}")
 
     log_success(f"edxbackup backup finished\n{backup_id}")
```

### Comparing `edxbackup-3.1.1/edxbackup/cli.py` & `edxbackup-3.2.1/edxbackup/cli.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.1/edxbackup/info.py` & `edxbackup-3.2.1/edxbackup/info.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.1/edxbackup/mongo.py` & `edxbackup-3.2.1/edxbackup/mongo.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,44 +9,58 @@
 from edxbackup.restic.restore import restore_stream
 from pydantic import BaseModel
 
 
 class MongoConfig(BaseModel):
     host: str
     port: int
-    user: str
-    password: str
+    user: str | None
+    password: str | None
     database: str
 
     def to_backup_options(self) -> list[str]:
         """
         Return a Popen args list to be used with mongodump CLI tool
         """
-        return [
+        options = [
             "--archive",
             f"--host={self.host}:{self.port}",
-            f"--username={self.user}",
-            f"--password={self.password}",
             f"--db={self.database}",
-            "--authenticationDatabase=admin",
         ]
 
+        has_auth = self.user is not None and self.password is not None
+        if has_auth:
+            options += [
+                f"--username={self.user}",
+                f"--password={self.password}",
+                "--authenticationDatabase=admin",
+            ]
+
+        return options
+
     def to_restore_options(self) -> list[str]:
         """
         Return a Popen args list to be used with mongorestore CLI tool
         """
-        return [
+        options = [
             "--archive",
             "--drop",
             f"--host={self.host}:{self.port}",
-            f"--username={self.user}",
-            f"--password={self.password}",
-            "--authenticationDatabase=admin",
         ]
 
+        has_auth = self.user is not None and self.password is not None
+        if has_auth:
+            options += [
+                f"--username={self.user}",
+                f"--password={self.password}",
+                "--authenticationDatabase=admin",
+            ]
+
+        return options
+
 
 def dump_mongo_db(
     mongo_info: MongoConfig, prefix: str, backup_id: str, backup_time: datetime
 ) -> bool:
     backup_args = ["mongodump", "--archive"] + mongo_info.to_backup_options()
 
     return backup_stdin(
```

### Comparing `edxbackup-3.1.1/edxbackup/mysql.py` & `edxbackup-3.2.1/edxbackup/mysql.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.1/edxbackup/restic/backup.py` & `edxbackup-3.2.1/edxbackup/restic/backup.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.1/edxbackup/restic/restore.py` & `edxbackup-3.2.1/edxbackup/restic/restore.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.1/edxbackup/restic/snapshot.py` & `edxbackup-3.2.1/edxbackup/restic/snapshot.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.1/edxbackup/restore.py` & `edxbackup-3.2.1/edxbackup/restore.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from edxbackup.config import EdxbackupConfig
 from edxbackup.context import build_context
 from edxbackup.context import get_mongo_target
 from edxbackup.context import get_mysql_target
+from edxbackup.context import get_postgresql_target
 from edxbackup.context import get_s3_target
 from edxbackup.mongo import restore_mongo_db
 from edxbackup.mysql import restore_mysql_db
 from edxbackup.options import config_path_option
+from edxbackup.postgresql import restore_postgresql_db
 from edxbackup.restic.snapshot import list_snapshots
 from edxbackup.s3 import restore_s3_bucket
 from edxbackup.utils import log_failure
 from edxbackup.utils import log_success
 
 import click
 
@@ -49,14 +51,29 @@
             else:
                 log_failure(f"edxbackup failed to restore mysql database: {mysql_db}")
         else:
             log_failure(
                 f"edxbackup failed to restore mysql database (no snapshot): {mysql_db}"
             )
 
+    for postgresql_config in config.postgresql:
+        postgresql_db = postgresql_config.database
+        postgresql_target = get_postgresql_target(backup_context, postgresql_db)
+        if postgresql_target is not None:
+            if restore_postgresql_db(postgresql_config, postgresql_target):
+                log_success(f"edxbackup restored postgresql database: {postgresql_db}")
+            else:
+                log_failure(
+                    f"edxbackup failed to restore postgresql database: {postgresql_db}"
+                )
+        else:
+            log_failure(
+                f"edxbackup failed to restore postgresql database (no snapshot): {postgresql_db}"
+            )
+
     for s3_config in config.s3:
         s3_bucket = s3_config.bucket
         s3_target = get_s3_target(backup_context, s3_config.bucket)
         if s3_target is not None:
             if restore_s3_bucket(s3_config, s3_target):
                 log_success(f"edxbackup restored S3 bucket: {s3_bucket}")
             else:
```

### Comparing `edxbackup-3.1.1/edxbackup/s3.py` & `edxbackup-3.2.1/edxbackup/s3.py`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.1/edxbackup.egg-info/SOURCES.txt` & `edxbackup-3.2.1/edxbackup.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 .envrc
 .flake8
 .gitignore
 .isort.cfg
 .pre-commit-config.yaml
 Dockerfile
 LICENSE
-README.md
 README.rst
 pyproject.toml
 pytest.ini
 requirements.txt
 shell.nix
 .github/workflows/lint.yml
 contrib/delete_old.py
@@ -19,14 +18,15 @@
 edxbackup/cli.py
 edxbackup/config.py
 edxbackup/context.py
 edxbackup/info.py
 edxbackup/mongo.py
 edxbackup/mysql.py
 edxbackup/options.py
+edxbackup/postgresql.py
 edxbackup/restore.py
 edxbackup/s3.py
 edxbackup/utils.py
 edxbackup.egg-info/PKG-INFO
 edxbackup.egg-info/SOURCES.txt
 edxbackup.egg-info/dependency_links.txt
 edxbackup.egg-info/entry_points.txt
```

### Comparing `edxbackup-3.1.1/example/edxbackup.json` & `edxbackup-3.2.1/example/edxbackup.json`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.1/pyproject.toml` & `edxbackup-3.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edxbackup-3.1.1/tests/docker-compose.yml` & `edxbackup-3.2.1/tests/docker-compose.yml`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,22 @@
       - "127.0.0.1:13306:3306"
     healthcheck:
       test: ["CMD", "mysqladmin" ,"ping", "-h", "localhost", "-uroot", "-p${MYSQL_PASSWORD}"]
       interval: 5s
       timeout: 5s
       retries: 20
 
+  postgresql:
+    image: "postgres:13.4-alpine"
+    environment:
+      POSTGRES_USER: "${POSTGRES_USER}"
+      POSTGRES_PASSWORD: "${POSTGRES_PASSWORD}"
+    ports:
+      - "127.0.0.1:55432:5432"
+
   minio:
     image: "quay.io/minio/minio:RELEASE.2023-04-07T05-28-58Z"
     environment:
       MINIO_ACCESS_KEY: "${MINIO_ACCESS_KEY}"
       MINIO_SECRET_KEY: "${MINIO_SECRET_KEY}"
     command: "server --address 0.0.0.0:9000 --console-address 0.0.0.0:9001 /data"
     ports:
```

### Comparing `edxbackup-3.1.1/tests/populate.sh` & `edxbackup-3.2.1/tests/populate.sh`

 * *Files identical despite different names*

