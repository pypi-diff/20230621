# Comparing `tmp/pem-21.2.0.tar.gz` & `tmp/pem-23.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pem-21.2.0.tar", last modified: Wed Apr  7 13:31:19 2021, max compression
+gzip compressed data, last modified: Wed Jun 21 10:09:26 2023, max compression
```

## Comparing `pem-21.2.0.tar` & `pem-23.1.0.tar`

### file list

```diff
@@ -1,47 +1,38 @@
-drwxr-xr-x   0 hynek      (501) staff       (20)        0 2021-04-07 13:31:19.889965 pem-21.2.0/
--rw-r--r--   0 hynek      (501) staff       (20)      553 2021-04-07 12:33:12.000000 pem-21.2.0/.pre-commit-config.yaml
--rw-r--r--   0 hynek      (501) staff       (20)      123 2019-03-19 20:59:13.000000 pem-21.2.0/.readthedocs.yml
--rw-r--r--   0 hynek      (501) staff       (20)      276 2021-01-22 08:56:15.000000 pem-21.2.0/AUTHORS.rst
--rw-r--r--   0 hynek      (501) staff       (20)     7012 2021-04-07 13:22:59.000000 pem-21.2.0/CHANGELOG.rst
--rw-r--r--   0 hynek      (501) staff       (20)     1064 2015-01-13 13:42:33.000000 pem-21.2.0/LICENSE
--rw-r--r--   0 hynek      (501) staff       (20)      245 2020-01-06 13:00:47.000000 pem-21.2.0/MANIFEST.in
--rw-r--r--   0 hynek      (501) staff       (20)     5763 2021-04-07 13:31:19.889661 pem-21.2.0/PKG-INFO
--rw-r--r--   0 hynek      (501) staff       (20)     2634 2021-02-12 07:07:07.000000 pem-21.2.0/README.rst
--rw-r--r--   0 hynek      (501) staff       (20)      175 2018-06-18 06:26:19.000000 pem-21.2.0/codecov.yml
--rw-r--r--   0 hynek      (501) staff       (20)      137 2018-06-16 08:02:18.000000 pem-21.2.0/conftest.py
-drwxr-xr-x   0 hynek      (501) staff       (20)        0 2021-04-07 13:31:19.880028 pem-21.2.0/docs/
--rw-r--r--   0 hynek      (501) staff       (20)     7397 2015-07-09 11:12:00.000000 pem-21.2.0/docs/Makefile
--rw-r--r--   0 hynek      (501) staff       (20)     1234 2021-04-07 12:31:07.000000 pem-21.2.0/docs/api.rst
--rw-r--r--   0 hynek      (501) staff       (20)      545 2015-07-10 09:57:01.000000 pem-21.2.0/docs/backward-compatibility.rst
--rw-r--r--   0 hynek      (501) staff       (20)       30 2016-02-04 14:17:19.000000 pem-21.2.0/docs/changelog.rst
--rw-r--r--   0 hynek      (501) staff       (20)     9372 2021-01-22 08:27:54.000000 pem-21.2.0/docs/conf.py
--rw-r--r--   0 hynek      (501) staff       (20)       60 2020-03-07 09:33:39.000000 pem-21.2.0/docs/contributing.rst
--rw-r--r--   0 hynek      (501) staff       (20)      677 2021-01-22 08:30:08.000000 pem-21.2.0/docs/core.rst
--rw-r--r--   0 hynek      (501) staff       (20)      528 2015-07-10 13:26:46.000000 pem-21.2.0/docs/index.rst
--rw-r--r--   0 hynek      (501) staff       (20)      315 2021-02-12 07:08:22.000000 pem-21.2.0/docs/license.rst
--rw-r--r--   0 hynek      (501) staff       (20)     7238 2015-07-09 11:12:00.000000 pem-21.2.0/docs/make.bat
--rw-r--r--   0 hynek      (501) staff       (20)     2030 2018-06-16 16:17:23.000000 pem-21.2.0/docs/twisted.rst
--rw-r--r--   0 hynek      (501) staff       (20)      350 2018-06-23 09:16:57.000000 pem-21.2.0/mypy.ini
--rw-r--r--   0 hynek      (501) staff       (20)      360 2021-01-21 10:20:01.000000 pem-21.2.0/pyproject.toml
--rw-r--r--   0 hynek      (501) staff       (20)       38 2021-04-07 13:31:19.890063 pem-21.2.0/setup.cfg
--rw-r--r--   0 hynek      (501) staff       (20)     3877 2021-01-22 08:26:12.000000 pem-21.2.0/setup.py
-drwxr-xr-x   0 hynek      (501) staff       (20)        0 2021-04-07 13:31:19.861605 pem-21.2.0/src/
-drwxr-xr-x   0 hynek      (501) staff       (20)        0 2021-04-07 13:31:19.882649 pem-21.2.0/src/pem/
--rw-r--r--   0 hynek      (501) staff       (20)     1150 2021-04-07 13:22:59.000000 pem-21.2.0/src/pem/__init__.py
--rw-r--r--   0 hynek      (501) staff       (20)      320 2020-11-03 11:27:44.000000 pem-21.2.0/src/pem/_compat.py
--rw-r--r--   0 hynek      (501) staff       (20)     6128 2021-04-07 12:31:07.000000 pem-21.2.0/src/pem/_core.py
--rw-r--r--   0 hynek      (501) staff       (20)        0 2018-06-23 09:16:57.000000 pem-21.2.0/src/pem/py.typed
--rw-r--r--   0 hynek      (501) staff       (20)     3515 2020-11-03 11:27:44.000000 pem-21.2.0/src/pem/twisted.py
-drwxr-xr-x   0 hynek      (501) staff       (20)        0 2021-04-07 13:31:19.885986 pem-21.2.0/src/pem.egg-info/
--rw-r--r--   0 hynek      (501) staff       (20)     5763 2021-04-07 13:31:19.000000 pem-21.2.0/src/pem.egg-info/PKG-INFO
--rw-r--r--   0 hynek      (501) staff       (20)      701 2021-04-07 13:31:19.000000 pem-21.2.0/src/pem.egg-info/SOURCES.txt
--rw-r--r--   0 hynek      (501) staff       (20)        1 2021-04-07 13:31:19.000000 pem-21.2.0/src/pem.egg-info/dependency_links.txt
--rw-r--r--   0 hynek      (501) staff       (20)        1 2016-02-04 14:19:16.000000 pem-21.2.0/src/pem.egg-info/not-zip-safe
--rw-r--r--   0 hynek      (501) staff       (20)      182 2021-04-07 13:31:19.000000 pem-21.2.0/src/pem.egg-info/requires.txt
--rw-r--r--   0 hynek      (501) staff       (20)        4 2021-04-07 13:31:19.000000 pem-21.2.0/src/pem.egg-info/top_level.txt
-drwxr-xr-x   0 hynek      (501) staff       (20)        0 2021-04-07 13:31:19.888639 pem-21.2.0/tests/
--rw-r--r--   0 hynek      (501) staff       (20)        0 2015-07-09 15:04:15.000000 pem-21.2.0/tests/__init__.py
--rw-r--r--   0 hynek      (501) staff       (20)    14543 2021-04-07 12:31:07.000000 pem-21.2.0/tests/data.py
--rw-r--r--   0 hynek      (501) staff       (20)    17419 2021-04-07 12:31:24.000000 pem-21.2.0/tests/test_core.py
--rw-r--r--   0 hynek      (501) staff       (20)     7719 2020-11-03 11:27:44.000000 pem-21.2.0/tests/test_twisted.py
--rw-r--r--   0 hynek      (501) staff       (20)     1754 2021-01-21 10:24:02.000000 pem-21.2.0/tox.ini
+-rw-r--r--   0        0        0      476 2023-06-21 10:09:26.000000 pem-23.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2023-06-21 10:09:26.000000 pem-23.1.0/.python-version
+-rw-r--r--   0        0        0      225 2023-06-21 10:09:26.000000 pem-23.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     7690 2023-06-21 10:09:26.000000 pem-23.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3115 2023-06-21 10:09:26.000000 pem-23.1.0/README.md
+-rw-r--r--   0        0        0     1697 2023-06-21 10:09:26.000000 pem-23.1.0/tox.ini
+-rw-r--r--   0        0        0     3167 2023-06-21 10:09:26.000000 pem-23.1.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     6769 2023-06-21 10:09:26.000000 pem-23.1.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       37 2023-06-21 10:09:26.000000 pem-23.1.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1360 2023-06-21 10:09:26.000000 pem-23.1.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      712 2023-06-21 10:09:26.000000 pem-23.1.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2023-06-21 10:09:26.000000 pem-23.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     3509 2023-06-21 10:09:26.000000 pem-23.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      749 2023-06-21 10:09:26.000000 pem-23.1.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1731 2023-06-21 10:09:26.000000 pem-23.1.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0     7397 2023-06-21 10:09:26.000000 pem-23.1.0/docs/Makefile
+-rw-r--r--   0        0        0     1383 2023-06-21 10:09:26.000000 pem-23.1.0/docs/api.rst
+-rw-r--r--   0        0        0       33 2023-06-21 10:09:26.000000 pem-23.1.0/docs/changelog.md
+-rw-r--r--   0        0        0     2078 2023-06-21 10:09:26.000000 pem-23.1.0/docs/conf.py
+-rw-r--r--   0        0        0      586 2023-06-21 10:09:26.000000 pem-23.1.0/docs/core.md
+-rw-r--r--   0        0        0      463 2023-06-21 10:09:26.000000 pem-23.1.0/docs/index.md
+-rw-r--r--   0        0        0     7238 2023-06-21 10:09:26.000000 pem-23.1.0/docs/make.bat
+-rw-r--r--   0        0        0     1947 2023-06-21 10:09:26.000000 pem-23.1.0/docs/twisted.md
+-rw-r--r--   0        0        0     2122 2023-06-21 10:09:26.000000 pem-23.1.0/src/pem/__init__.py
+-rw-r--r--   0        0        0     1770 2023-06-21 10:09:26.000000 pem-23.1.0/src/pem/_core.py
+-rw-r--r--   0        0        0     6634 2023-06-21 10:09:26.000000 pem-23.1.0/src/pem/_object_types.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:09:26.000000 pem-23.1.0/src/pem/py.typed
+-rw-r--r--   0        0        0     3830 2023-06-21 10:09:26.000000 pem-23.1.0/src/pem/twisted.py
+-rw-r--r--   0        0        0        0 2023-06-21 10:09:26.000000 pem-23.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    22052 2023-06-21 10:09:26.000000 pem-23.1.0/tests/data.py
+-rw-r--r--   0        0        0    20708 2023-06-21 10:09:26.000000 pem-23.1.0/tests/test_core.py
+-rw-r--r--   0        0        0     1318 2023-06-21 10:09:26.000000 pem-23.1.0/tests/test_packaging.py
+-rw-r--r--   0        0        0     7849 2023-06-21 10:09:26.000000 pem-23.1.0/tests/test_twisted.py
+-rw-r--r--   0        0        0      609 2023-06-21 10:09:26.000000 pem-23.1.0/tests/typing/api.py
+-rw-r--r--   0        0        0      144 2023-06-21 10:09:26.000000 pem-23.1.0/.gitignore
+-rw-r--r--   0        0        0     1084 2023-06-21 10:09:26.000000 pem-23.1.0/LICENSE
+-rw-r--r--   0        0        0     4306 2023-06-21 10:09:26.000000 pem-23.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5054 2023-06-21 10:09:26.000000 pem-23.1.0/PKG-INFO
```

### Comparing `pem-21.2.0/CHANGELOG.rst` & `pem-23.1.0/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,350 +1,205 @@
-.. :changelog:
+# Changelog
 
-Changelog
-=========
+All notable changes to this project will be documented in this file.
 
-Versions are year-based with a strict backward compatibility policy.
-The third digit is only for regressions.
+The format is based on [*Keep a Changelog*](https://keepachangelog.com/en/1.0.0/) and this project adheres to [*Calendar Versioning*](https://calver.org/).
 
+The **first number** of the version is the year.
+The **second number** is incremented with each release, starting at 1 for each year.
+The **third number** is for emergencies when we need to start branches for older releases.
 
-21.2.0 (2021-04-07)
--------------------
+You can find our backwards-compatibility policy [here](https://github.com/hynek/pem/blob/main/.github/SECURITY.md).
 
-Backward-incompatible changes:
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+<!-- changelog follows -->
 
-*none*
+## [23.1.0](https://github.com/hynek/pem/compare/21.2.0...23.1.0) - 2023-06-21
 
+### Removed
 
-Deprecations:
-^^^^^^^^^^^^^
+- Support for Python 2.7, 3.5, and 3.6 has been dropped.
 
-*none*
 
+### Added
 
-Changes:
-^^^^^^^^
+- Support for RFC 4880 OpenPGP private & public keys: `pem.OpenPGPPublicKey` and `pem.OpenPGPPrivateKey`.
+  [#72](https://github.com/hynek/pem/issues/72)
+- Support for intra-payload headers like the ones used in OpenPGP keys using the `meta_headers` property.
+  [#75](https://github.com/hynek/pem/pull/75)
+- `pem.parse_file()` now accepts also [`pathlib.Path`](https://docs.python.org/3/library/pathlib.html#pathlib.Path) objects.
+- `pem.parse()` now also accepts `str`.
+- Added `text_payload`, `bytes_payload` and `decoded_payload` properties to all PEM objects that allow to directly access the payload without the envelope and possible headers.
+  [#74](https://github.com/hynek/pem/pull/74)
 
-- Added support for ``pem.OpenSSLTrustedCertificate`` (``-----BEGIN TRUSTED CERTIFICATE-----``), as defined in `openssl x509 manual <https://www.openssl.org/docs/man1.1.1/man1/x509.html>`_.
-  `#28 <https://github.com/hynek/pem/issues/28>`_
 
+## [21.2.0](https://github.com/hynek/pem/compare/21.1.0...21.2.0) - 2021-04-07
 
-----
+### Added
 
+- Added support for `pem.OpenSSLTrustedCertificate` (`-----BEGIN TRUSTED CERTIFICATE-----`), as defined in [openssl x509 manual](https://www.openssl.org/docs/man1.1.1/man1/x509.html).
+  [#28](https://github.com/hynek/pem/issues/28)
 
-21.1.0 (2021-01-22)
--------------------
 
+## [21.1.0](https://github.com/hynek/pem/compare/20.1.0...21.1.0) - 2021-01-22
 
-Backward-incompatible changes:
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### Added
 
-*none*
-
-
-Deprecations:
-^^^^^^^^^^^^^
-
-*none*
-
-
-Changes:
-^^^^^^^^
-
-- Added support for DSA private keys (``BEGIN DSA PRIVATE``).
+- Added support for DSA private keys (`BEGIN DSA PRIVATE`).
   This is also the OpenSSH legacy PEM format.
-  `#49 <https://github.com/hynek/pem/issues/49>`_
-- Added support for ``pem.SSHPublicKey`` (``---- BEGIN SSH2 PUBLIC KEY ----``), as defined in `RFC 4716 <https://tools.ietf.org/html/rfc4716>`_.
-  `#46 <https://github.com/hynek/pem/pull/46>`_
-- Added support for ``pem.SSHCOMPrivateKey`` (``---- BEGIN SSH2 ENCRYPTED PRIVATE KEY ----``), the SSH.com / Tectia private key format (plain or encrypted).
-  `#46 <https://github.com/hynek/pem/pull/46>`_
-
-
-----
-
-
-20.1.0 (2020-01-06)
--------------------
+  [#49](https://github.com/hynek/pem/issues/49)
+- Added support for `pem.SSHPublicKey` (`---- BEGIN SSH2 PUBLIC KEY ----`), as defined in [RFC 4716](https://datatracker.ietf.org/doc/html/rfc4716).
+  [#46](https://github.com/hynek/pem/pull/46)
+- Added support for `pem.SSHCOMPrivateKey` (`---- BEGIN SSH2 ENCRYPTED PRIVATE KEY ----`), the SSH.com / Tectia private key format (plain or encrypted).
+  [#46](https://github.com/hynek/pem/pull/46)
 
 
-Backward-incompatible changes:
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+## [20.1.0](https://github.com/hynek/pem/compare/19.3.0...20.1.0) - 2020-01-06
 
-*none*
+### Changed
 
+- Carriage returns (`\r`) are now stripped before hashing *pem* objects to provide consistent hashes across platforms.
+  [#40](https://github.com/hynek/pem/issues/40)
 
-Deprecations:
-^^^^^^^^^^^^^
 
-*none*
+## [19.3.0](https://github.com/hynek/pem/compare/19.2.0...19.3.0) - 2019-10-16
 
-
-Changes:
-^^^^^^^^
-
-- Carriage returns (``\r``) are now stripped before hashing *pem* objects to provide consistent hashes across platforms.
-  `#40 <https://github.com/hynek/pem/issues/40>`_
-
-
-----
-
-
-19.3.0 (2019-10-16)
--------------------
-
-
-Backward-incompatible changes:
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### Removed
 
 - Python 3.4 is not supported anymore.
   It has been unsupported by the Python core team for a while now and its PyPI downloads are negligible.
 
   It's very unlikely that *pem* will break under 3.4 anytime soon, but we don't test it anymore.
 
+### Added
 
-Deprecations:
-^^^^^^^^^^^^^
-
-*none*
-
-
-Changes:
-^^^^^^^^
-
-- Added support for ``pem.OpenSSHPrivateKey`` (``OPENSSH PRIVATE KEY``).
-  OpenSSH added a new ``BEGIN`` label when it switched to a proprietary key encoding.
-  `#39 <https://github.com/hynek/pem/pull/39>`_
-
-
-----
-
-
-19.2.0 (2019-08-06)
--------------------
-
-
-Backward-incompatible changes:
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-*none*
-
-
-Deprecations:
-^^^^^^^^^^^^^
-
-*none*
-
-
-Changes:
-^^^^^^^^
-
-- Added support for ``pem.ECPrivateKey`` (``EC PRIVATE KEY``).
-
-
-----
-
+- Added support for `pem.OpenSSHPrivateKey` (`OPENSSH PRIVATE KEY`).
+  OpenSSH added a new `BEGIN` label when it switched to a proprietary key encoding.
+  [#39](https://github.com/hynek/pem/pull/39)
 
-19.1.0 (2019-03-19)
--------------------
 
+## [19.2.0](https://github.com/hynek/pem/compare/19.1.0...19.2.0) - 2019-08-06
 
-Backward-incompatible changes:
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### Added
 
-*none*
+- Added support for `pem.ECPrivateKey` (`EC PRIVATE KEY`).
 
 
-Deprecations:
-^^^^^^^^^^^^^
+## [19.1.0](https://github.com/hynek/pem/compare/18.2.0...19.1.0) - 2019-03-19
 
-*none*
+### Added
 
+- You can now load encrypted PKCS#8 PEM key as `pem.Key`.
+- Added support for `pem.PublicKey` (`PUBLIC KEY`).
+- Added support for `pem.RSAPublicKey` (`RSA PUBLIC KEY`).
 
-Changes:
-^^^^^^^^
 
-- You can now load encrypted PKCS#8 PEM key as ``pem.Key``.
-- Added support for ``pem.PublicKey`` (``PUBLIC KEY``).
-- Added support for ``pem.RSAPublicKey`` (``RSA PUBLIC KEY``).
+## [18.2.0](https://github.com/hynek/pem/compare/18.1.0...18.2.0) - 2018-10-09
 
+### Added
 
-----
+- Added `pem.CertificateRevocationList` for certificate revocation lists (CRLs).
+  [#32](https://github.com/hynek/pem/pull/32)
 
 
-18.2.0 (2018-10-09)
--------------------
+## [18.1.0](https://github.com/hynek/pem/compare/17.1.0...18.1.0) - 2018-06-23
 
+### Removed
 
-Backward-incompatible changes:
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-*none*
-
-
-Deprecations:
-^^^^^^^^^^^^^
-
-*none*
-
-
-Changes:
-^^^^^^^^
-
-- Added ``pem.CertificateRevocationList`` for certificate revocation lists (CRLs).
-  `#32 <https://github.com/hynek/pem/pull/32>`_
-
-
-----
-
-
-18.1.0 (2018-06-23)
--------------------
-
-
-Backward-incompatible changes:
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-- ``pem.certificateOptionsFromFiles()`` and ``pem.certificateOptionsFromPEMs()`` have been removed after three years of deprecation.
-  Please use ``pem.twisted.certificateOptionsFromFiles()`` ``pem.twisted.certificateOptionsFromPEMs()`` instead.
+- `pem.certificateOptionsFromFiles()` and `pem.certificateOptionsFromPEMs()` have been removed after three years of deprecation.
+  Please use `pem.twisted.certificateOptionsFromFiles()` `pem.twisted.certificateOptionsFromPEMs()` instead.
 - Diffie-Hellman support for Twisted older than 14.0 has been removed.
 
 
-Deprecations:
-^^^^^^^^^^^^^
-
-*none*
-
-
-Changes:
-^^^^^^^^
-
-- *pem* now ships with typing information that can be used by type checkers like `mypy <http://mypy-lang.org>`_.
-- PEM objects now have an ``obj.sha1_hexdigest`` property with the SHA-1 digest of the stored bytes  as a native string.
-  This is the same digest as the one that is used by the PEM objects' ``__repr__``\ s.
-- PEM objects now have an ``obj.as_text()`` method that returns the PEM-encoded content as unicode, always.
-
+### Added
 
-----
+- *pem* now ships with typing information that can be used by type checkers like [Mypy](https://mypy-lang.org).
+- PEM objects now have an `obj.sha1_hexdigest` property with the SHA-1 digest of the stored bytes  as a native string.
+  This is the same digest as the one that is used by the PEM objects' `__repr__`s.
+- PEM objects now have an `obj.as_text()` method that returns the PEM-encoded content as unicode, always.
 
 
-17.1.0 (2017-08-10)
--------------------
+## [17.1.0](https://github.com/hynek/pem/compare/16.1.0...17.1.0) - 2017-08-10
 
+### Added
 
-Changes:
-^^^^^^^^
+- Added `pem.CertificateRequest` for [certificate signing requests](https://en.wikipedia.org/wiki/Certificate_signing_request).
+  [#29](https://github.com/hynek/pem/pull/29)
 
-- Added ``pem.CertificateRequest`` for `certificate signing requests <https://en.wikipedia.org/wiki/Certificate_signing_request>`_.
-  `#29 <https://github.com/hynek/pem/pull/29>`_
 
+## [16.1.0](https://github.com/hynek/pem/compare/16.0.0...16.1.0) - 2016-04-08
 
-----
+### Deprecated
 
-
-16.1.0 (2016-04-08)
--------------------
-
-Deprecations:
-^^^^^^^^^^^^^
-
-- Passing ``dhParameters`` to ``pem.twisted.certifateOptionsFromPEMs`` and ``certificateOptionsFromFiles`` is now deprecated;
+- Passing `dhParameters` to `pem.twisted.certifateOptionsFromPEMs` and `certificateOptionsFromFiles` is now deprecated;
   instead, include the DH parameters in the PEM objects or files.
 
-
-Backward-incompatible changes:
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### Removed
 
 - Python 3.3 and 2.6 aren't supported anymore.
   They may work by chance but any effort to keep them working has ceased.
 
   The last Python 2.6 release was on October 29, 2013 and isn't supported by the CPython core team anymore.
   Major Python packages like Django and Twisted dropped Python 2.6 a while ago already.
 
   Python 3.3 never had a significant user base and wasn't part of any distribution's LTS release.
 
+### Added
 
-Changes:
-^^^^^^^^
-
-- ``pem.twisted.certificateOptionsFromPEMs`` and ``certificateOptionsFromFiles`` will now load Ephemeral Diffie-Hellman parameters if found.
-  `#21 <https://github.com/hynek/pem/pull/21>`_
-- PEM objects now correctly handle being constructed with unicode and bytes on both Python 2 and 3.
-  `#24 <https://github.com/hynek/pem/pull/24>`_
-- PEM objects now have an ``as_bytes`` method that returns the PEM-encoded content as bytes, always.
-  `#24 <https://github.com/hynek/pem/pull/24>`_
-- PEM objects are now hashable and comparable for equality.
-  `#25 <https://github.com/hynek/pem/pull/25>`_
+- `pem.twisted.certificateOptionsFromPEMs` and `certificateOptionsFromFiles` will now load Ephemeral Diffie-Hellman parameters if found.
+  [#21](https://github.com/hynek/pem/pull/21)
+- PEM objects now have an `as_bytes` method that returns the PEM-encoded content as bytes, always.
+  [#24](https://github.com/hynek/pem/pull/24)
 
 
+### Fixed
 
-----
+- PEM objects now correctly handle being constructed with unicode and bytes on both Python 2 and 3.
+  [#24](https://github.com/hynek/pem/pull/24)
+- PEM objects are now hashable and comparable for equality.
+  [#25](https://github.com/hynek/pem/pull/25)
 
 
-16.0.0 (2016-02-05)
--------------------
+## [16.0.0](https://github.com/hynek/pem/compare/15.0.0...16.0.0) - 2016-02-05
 
-Changes:
-^^^^^^^^
+### Added
 
 - PKCS #8 keys are now supported.
-  `#14 <https://github.com/hynek/pem/pull/14>`_
+  [#14](https://github.com/hynek/pem/pull/14)
 - *pem* is now fully functional without installing Twisted.
-  `#16 <https://github.com/hynek/pem/pull/16>`_
+  [#16](https://github.com/hynek/pem/pull/16)
 
 
-----
+## [15.0.0](https://github.com/hynek/pem/compare/0.3.0...15.0.0) - 2015-07-10
 
-
-15.0.0 (2015-07-10)
--------------------
-
-Deprecations:
-^^^^^^^^^^^^^
+### Deprecated
 
 - The usage of Twisted helpers from the pem module is deprecated.
-  Use their pendants from the ``pem.twisted`` module now.
+  Use their pendants from the `pem.twisted` module now.
 - The usage of the backport of ephemeral Diffie-Hellman support is hereby deprecated.
   Nobody should use a Twisted release that is older than 14.0.0 because it contains essential SSL/TLS fixes.
 
-
-Changes:
-^^^^^^^^
+### Changed
 
 - Support PEM strings that do not end with a new line.
-  `#12 <https://github.com/hynek/pem/pull/12>`_
-- Support PEM strings that end with ``\r\n``.
-- The Twisted-related helpers have been moved to ``pem.twisted``.
-
-
-----
+  [#12](https://github.com/hynek/pem/pull/12)
+- Support PEM strings that end with `\r\n`.
+- The Twisted-related helpers have been moved to `pem.twisted`.
 
 
-0.3.0 (2014-04-15)
-------------------
+## [0.3.0](https://github.com/hynek/pem/compare/0.2.0...0.3.0) - 2014-04-15
 
-Changes:
-^^^^^^^^
+### Changed
 
-- Load PEM files as UTF-8 to allow for non-ASCII comments (like in certifi).
+- Load PEM files as UTF-8 to allow for non-ASCII comments (like in *certifi*).
 - Allow keys, primary certificates, and chain certificates to occur in any order.
 
 
-----
+## [0.2.0](https://github.com/hynek/pem/compare/v0.1.0...0.2.0) - 2014-03-13
 
-
-0.2.0 (2014-03-13)
-------------------
-
-Changes:
-^^^^^^^^
+### Added
 
 - Add forward-compatible support for DHE.
 
 
-----
-
-
-0.1.0 (2013-07-18)
-------------------
+## [0.1.0](https://github.com/hynek/pem/tree/v0.1.0) - 2013-07-18
 
 Initial release.
```

### Comparing `pem-21.2.0/LICENSE` & `pem-23.1.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2012-2015 Hynek Schlawack
+Copyright (c) 2013 Hynek Schlawack and the pem contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `pem-21.2.0/docs/Makefile` & `pem-23.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pem-21.2.0/docs/api.rst` & `pem-23.1.0/docs/api.rst`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Core
 ----
 
 .. currentmodule:: pem
 
 See :doc:`core` for examples.
 
+
 Parsers
 ^^^^^^^
 
 .. autofunction:: parse
 
 .. autofunction:: parse_file
 
@@ -34,22 +35,24 @@
 .. autoclass:: RSAPrivateKey(PrivateKey)
 .. autoclass:: RSAPublicKey(PublicKey)
 .. autoclass:: ECPrivateKey(PrivateKey)
 .. autoclass:: DSAPrivateKey(PrivateKey)
 .. autoclass:: OpenSSHPrivateKey(PrivateKey)
 .. autoclass:: SSHPublicKey(Key)
 .. autoclass:: SSHCOMPrivateKey(PrivateKey)
+.. autoclass:: OpenPGPPublicKey(PublicKey)
+.. autoclass:: OpenPGPPrivateKey(PrivateKey)
 .. autoclass:: DHParameters(AbstractPEMObject)
 .. autoclass:: CertificateRequest(AbstractPEMObject)
 .. autoclass:: CertificateRevocationList(AbstractPEMObject)
 
 Their shared provided API is minimal:
 
 .. autoclass:: AbstractPEMObject
-   :members: __str__, as_bytes, as_text, sha1_hexdigest
+   :members: __str__, as_bytes, as_text, sha1_hexdigest, bytes_payload, text_payload, decoded_payload, meta_headers
 
 
 Twisted
 -------
 
 .. currentmodule:: pem.twisted
```

### Comparing `pem-21.2.0/docs/make.bat` & `pem-23.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pem-21.2.0/docs/twisted.rst` & `pem-23.1.0/docs/twisted.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,59 @@
-Twisted
-=======
+# Twisted
 
-A typical use case in Twisted with the core API would be::
+A typical use case in Twisted with the core API would be:
 
-   import pem
+```
+import pem
 
-   from twisted.internet import ssl
+from twisted.internet import ssl
 
-   key = pem.parse_file("key.pem")
-   cert, chain = pem.parse_file("cert_and_chain.pem")
-   cert = ssl.PrivateCertificate.loadPEM(str(key) + str(cert))
-   chainCert = ssl.Certificate.loadPEM(str(chain))
-   dhParams = ssl.DiffieHellmanParameters(str(pem.parse_file("dhparams.pem")))
-
-   ctxFactory = ssl.CertificateOptions(
-         privateKey=cert.privateKey.original,
-         certificate=cert.original,
-         extraCertChain=[chainCert.original],
-         dhParameters=dhParams,
-   )
+key = pem.parse_file("key.pem")
+cert, chain = pem.parse_file("cert_and_chain.pem")
+cert = ssl.PrivateCertificate.loadPEM(str(key) + str(cert))
+chainCert = ssl.Certificate.loadPEM(str(chain))
+dhParams = ssl.DiffieHellmanParameters(str(pem.parse_file("dhparams.pem")))
+
+ctxFactory = ssl.CertificateOptions(
+      privateKey=cert.privateKey.original,
+      certificate=cert.original,
+      extraCertChain=[chainCert.original],
+      dhParameters=dhParams,
+)
+```
 
 Turns out, this is a major use case.
-Therefore it can be simplified to::
-
-   ctxFactory = pem.twisted.certificateOptionsFromFiles(
-      "key.pem", "cert_and_chain.pem", "dhparams.pem",
-   )
+Therefore it can be simplified to:
 
+```
+ctxFactory = pem.twisted.certificateOptionsFromFiles(
+   "key.pem", "cert_and_chain.pem", "dhparams.pem",
+)
+```
 
 There must be exactly one private key present.
 The certificate matching the private key will be used as the server certificate, the rest is passed as the chain.
 There must be no more than one set of DH parameters.
 You can pass as many PEM files as you like.
 Therefore you can distribute your key, certificate, chain certificates, and DH parameters over a arbitrary number of files.
-A ``ValueError`` is raised if more than one key, no key, or no certificate are found.
-Any further keyword arguments will be passed to CertificateOptions_.
-Passing ``dhParameters`` directly as a keyword argument is deprecated; pass these as part of the PEM files instead.
+A `ValueError` is raised if more than one key, no key, or no certificate are found.
+Any further keyword arguments will be passed to [CertificateOptions].
+Passing `dhParameters` directly as a keyword argument is deprecated; pass these as part of the PEM files instead.
 
 If you want to load your PEM data from somewhere else, you can also use
-:func:`pem.twisted.certificateOptionsFromPEMs` to do the same thing with already-loaded PEM objects, like so::
-
-    myPems = []
-    pems = pem.parse("""\
-    -----BEGIN RSA PRIVATE KEY-----
-    ...
-    -----END RSA PRIVATE KEY-----
-    -----BEGIN CERTIFICATE-----
-    ...
-    -----END CERTIFICATE-----
-    """)
+{func}`pem.twisted.certificateOptionsFromPEMs` to do the same thing with already-loaded PEM objects, like so:
 
-    ctxFactory = pem.twisted.certificateOptionsFromPEMs(pems)
+```
+myPems = []
+pems = pem.parse("""\
+-----BEGIN RSA PRIVATE KEY-----
+...
+-----END RSA PRIVATE KEY-----
+-----BEGIN CERTIFICATE-----
+...
+-----END CERTIFICATE-----
+""")
 
+ctxFactory = pem.twisted.certificateOptionsFromPEMs(pems)
+```
 
-.. _CertificateOptions: https://twistedmatrix.com/documents/current/api/twisted.internet.ssl.CertificateOptions.html
+[certificateoptions]: https://docs.twistedmatrix.com/en/stable/api/twisted.internet.ssl.CertificateOptions.html
```

### Comparing `pem-21.2.0/src/pem/_core.py` & `pem-23.1.0/src/pem/_object_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,276 +1,322 @@
-# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2013 Hynek Schlawack <hs@ox.cx>
+#
+# SPDX-License-Identifier: MIT
 
 """
-Framework agnostic PEM file parsing functions.
+All supported PEM object types.
 """
 
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
 import hashlib
-import re
 
-from ._compat import ABC, PY2, text_type
+from abc import ABCMeta
+from base64 import b64decode
+from functools import cached_property
+from typing import ClassVar
 
 
-# mypy hack: Import typing information without actually importing anything.
-MYPY = False
-if MYPY:  # pragma: nocover
-    from typing import Any, AnyStr, Dict, List, Optional, Type, Union  # noqa
-
-
-class AbstractPEMObject(ABC):
+class AbstractPEMObject(metaclass=ABCMeta):
     """
     Base class for parsed objects.
     """
 
-    def __init__(self, pem_bytes):
-        # type: (Union[text_type, bytes]) -> None
-        if isinstance(pem_bytes, text_type):
-            self._pem_bytes = pem_bytes.encode("ascii")  # type: bytes
-        else:
-            self._pem_bytes = pem_bytes
-        self._sha1_hexdigest = None  # type: Optional[str]
+    _pattern: ClassVar[tuple[bytes, ...]] = NotImplemented
+
+    _pem_bytes: bytes
 
-    def __str__(self):
-        # type: () -> str
+    def __init__(self, pem_bytes: bytes | str):
+        self._pem_bytes = (
+            pem_bytes.encode("ascii")
+            if isinstance(pem_bytes, str)
+            else pem_bytes
+        )
+
+        self._sha1_hexdigest = None
+
+    def __str__(self) -> str:
         """
         Return the PEM-encoded content as a native :obj:`str`.
         """
-        if not PY2:
-            return self._pem_bytes.decode("ascii")
-        return self._pem_bytes
+        return self._pem_bytes.decode("ascii")
 
-    def __repr__(self):
-        # type: () -> str
-        return "<{0}(PEM string with SHA-1 digest {1!r})>".format(
+    def __repr__(self) -> str:
+        return "<{}(PEM string with SHA-1 digest {!r})>".format(
             self.__class__.__name__, self.sha1_hexdigest
         )
 
-    @property
-    def sha1_hexdigest(self):
-        # type: () -> str
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, type(self)):
+            return NotImplemented
+
+        return (
+            type(self) == type(other) and self._pem_bytes == other._pem_bytes
+        )
+
+    def __hash__(self) -> int:
+        return hash(self._pem_bytes)
+
+    @cached_property
+    def sha1_hexdigest(self) -> str:
         """
         A SHA-1 digest of the whole object for easy differentiation.
 
         .. versionadded:: 18.1.0
         .. versionchanged:: 20.1.0
 
            Carriage returns are removed before hashing to give the same hashes
            on Windows and UNIX-like operating systems.
         """
-        if self._sha1_hexdigest is None:
-            self._sha1_hexdigest = hashlib.sha1(
-                self._pem_bytes.replace(b"\r", b"")
-            ).hexdigest()
-
-        return self._sha1_hexdigest
+        return hashlib.sha1(  # noqa[S324]
+            self._pem_bytes.replace(b"\r", b"")
+        ).hexdigest()
 
-    def as_bytes(self):
-        # type: () -> bytes
+    def as_bytes(self) -> bytes:
         """
         Return the PEM-encoded content as :obj:`bytes`.
 
         .. versionadded:: 16.1.0
         """
         return self._pem_bytes
 
-    def as_text(self):
-        # type: () -> text_type
+    def as_text(self) -> str:
         """
-        Return the PEM-encoded content as Unicode text.
+        Return the PEM-encoded content as text.
 
         .. versionadded:: 18.1.0
         """
         return self._pem_bytes.decode("utf-8")
 
-    def __eq__(self, other):
-        # type: (object) -> bool
-        if not isinstance(other, type(self)):
-            return NotImplemented
+    @cached_property
+    def bytes_payload(self) -> bytes:
+        """
+        The payload of the PEM-encoded content.
 
-        return (
-            type(self) == type(other) and self._pem_bytes == other._pem_bytes
+        Possible PEM headers are removed.
+
+        .. versionadded:: 23.1.0
+        """
+        return b"".join(
+            line
+            for line in self._pem_bytes.splitlines()[1:-1]
+            if b":" not in line  # remove headers
         )
 
-    def __ne__(self, other):
-        # type: (object) -> bool
-        if not isinstance(other, type(self)):
-            return NotImplemented
+    @cached_property
+    def text_payload(self) -> str:
+        """
+        The payload of the PEM-encoded content.
 
-        return type(self) != type(other) or self._pem_bytes != other._pem_bytes
+        Possible PEM headers are removed.
 
-    def __hash__(self):
-        # type: () -> int
-        return hash(self._pem_bytes)
+        .. versionadded:: 23.1.0
+        """
+        return self.bytes_payload.decode("utf-8")
+
+    @cached_property
+    def decoded_payload(self) -> bytes:
+        """
+        The base64-decoded payload of the PEM-encoded content.
+
+        Possible PEM headers are removed.
+
+        .. versionadded:: 23.1.0
+        """
+        return b64decode(self.bytes_payload)
+
+    @cached_property
+    def meta_headers(self) -> dict[str, str]:
+        """
+        Return a dictionary of payload headers.
+
+        If the value of a header is quoted, the quotes are removed.
+
+        .. versionadded:: 23.1.0
+        """
+        expl = {}
+        for line in self._pem_bytes.decode().splitlines()[1:-1]:
+            if ":" not in line:
+                break
+
+            key, val = line.split(": ", 1)
+
+            # Strip quotes if they're only at the beginning and end.
+            if val.count('"') == 2 and val[0] == '"' and val[-1] == '"':
+                val = val[1:-1]
+
+            expl[key] = val
+        else:
+            # XXX: necessary for Coverage.py!? This can't happen with non-empty
+            # PEM objects.
+            pass  # pragma: no cover
+
+        return expl
 
 
 class Certificate(AbstractPEMObject):
     """
     A certificate.
     """
 
+    _pattern = (b"CERTIFICATE",)
+
 
 class OpenSSLTrustedCertificate(Certificate):
     """
     An OpenSSL "trusted certificate".
 
     .. versionadded:: 21.2.0
     """
 
+    _pattern = (b"TRUSTED CERTIFICATE",)
+
 
 class CertificateRequest(AbstractPEMObject):
     """
     A certificate signing request.
 
     .. versionadded:: 17.1.0
     """
 
+    _pattern = (b"NEW CERTIFICATE REQUEST", b"CERTIFICATE REQUEST")
+
 
 class CertificateRevocationList(AbstractPEMObject):
     """
     A certificate revocation list.
 
     .. versionadded:: 18.2.0
     """
 
+    _pattern = (b"X509 CRL",)
+
 
 class Key(AbstractPEMObject):
     """
     A key of unknown type.
     """
 
+    # Key is special-cased later and is kind of abstract.
+
 
 class PrivateKey(Key):
     """
     A private key of unknown type.
 
     .. versionadded:: 19.1.0
     """
 
+    _pattern: ClassVar[tuple[bytes, ...]] = (
+        b"PRIVATE KEY",
+        b"ENCRYPTED PRIVATE KEY",
+    )
+
 
 class PublicKey(Key):
     """
     A public key of unknown type.
 
     .. versionadded:: 19.1.0
     """
 
+    _pattern = (b"PUBLIC KEY",)
+
 
 class RSAPrivateKey(PrivateKey):
     """
     A private RSA key.
     """
 
+    _pattern = (b"RSA PRIVATE KEY",)
+
 
 class RSAPublicKey(PublicKey):
     """
     A public RSA key.
 
     .. versionadded:: 19.1.0
     """
 
+    _pattern = (b"RSA PUBLIC KEY",)
+
 
 class ECPrivateKey(PrivateKey):
     """
     A private EC key.
 
     .. versionadded:: 19.2.0
     """
 
+    _pattern = (b"EC PRIVATE KEY",)
+
 
 class DSAPrivateKey(PrivateKey):
     """
     A private DSA key.
 
     Also private DSA key in OpenSSH legacy PEM format.
 
     .. versionadded:: 21.1.0
     """
 
+    _pattern = (b"DSA PRIVATE KEY",)
+
 
 class DHParameters(AbstractPEMObject):
     """
     Diffie-Hellman parameters for DHE.
     """
 
+    _pattern = (b"DH PARAMETERS",)
+
 
 class OpenSSHPrivateKey(PrivateKey):
     """
     OpenSSH private key format
 
     .. versionadded:: 19.3.0
     """
 
+    _pattern = (b"OPENSSH PRIVATE KEY",)
+
 
 class SSHPublicKey(PublicKey):
     """
-    A public key in SSH
-    `RFC 4716 <https://tools.ietf.org/html/rfc4716>`_ format.
+    A public key in SSH :rfc:`4716` format.
 
     The Secure Shell (SSH) Public Key File Format.
 
     .. versionadded:: 21.1.0
     """
 
+    _pattern = (b"SSH2 PUBLIC KEY",)
+
 
 class SSHCOMPrivateKey(PrivateKey):
     """
     A private key in SSH.COM / Tectia format.
 
     .. versionadded:: 21.1.0
     """
 
+    _pattern = (b"SSH2 ENCRYPTED PRIVATE KEY",)
+
+
+class OpenPGPPublicKey(PublicKey):
+    """
+    An :rfc:`4880` armored OpenPGP public key.
+
+    .. versionadded:: 23.1.0
+    """
 
-_PEM_TO_CLASS = {
-    b"CERTIFICATE": Certificate,
-    b"TRUSTED CERTIFICATE": OpenSSLTrustedCertificate,
-    b"PRIVATE KEY": PrivateKey,
-    b"PUBLIC KEY": PublicKey,
-    b"ENCRYPTED PRIVATE KEY": PrivateKey,
-    b"OPENSSH PRIVATE KEY": OpenSSHPrivateKey,
-    b"DSA PRIVATE KEY": DSAPrivateKey,
-    b"RSA PRIVATE KEY": RSAPrivateKey,
-    b"RSA PUBLIC KEY": RSAPublicKey,
-    b"EC PRIVATE KEY": ECPrivateKey,
-    b"DH PARAMETERS": DHParameters,
-    b"NEW CERTIFICATE REQUEST": CertificateRequest,
-    b"CERTIFICATE REQUEST": CertificateRequest,
-    b"SSH2 PUBLIC KEY": SSHPublicKey,
-    b"SSH2 ENCRYPTED PRIVATE KEY": SSHCOMPrivateKey,
-    b"X509 CRL": CertificateRevocationList,
-}  # type: Dict[bytes, Type[AbstractPEMObject]]
-
-# See https://tools.ietf.org/html/rfc1421
-# and https://tools.ietf.org/html/rfc4716 for space instead of fifth dash.
-_PEM_RE = re.compile(
-    b"----[- ]BEGIN ("
-    + b"|".join(_PEM_TO_CLASS.keys())
-    + b""")[- ]----\r?
-.+?\r?
-----[- ]END \\1[- ]----\r?\n?""",
-    re.DOTALL,
-)
-
-
-def parse(pem_str):
-    # type: (bytes) -> List[AbstractPEMObject]
-    """
-    Extract PEM-like objects from *pem_str*.
-
-    :param pem_str: String to parse.
-    :type pem_str: bytes
-    :return: list of :ref:`pem-objects`
-    """
-    return [
-        _PEM_TO_CLASS[match.group(1)](match.group(0))
-        for match in _PEM_RE.finditer(pem_str)
-    ]
+    _pattern = (b"PGP PUBLIC KEY BLOCK",)
 
 
-def parse_file(file_name):
-    # type: (str) -> List[AbstractPEMObject]
+class OpenPGPPrivateKey(PrivateKey):
     """
-    Read *file_name* and parse PEM objects from it using :func:`parse`.
+    An :rfc:`4880` armored OpenPGP private key.
+
+    .. versionadded:: 23.1.0
     """
-    with open(file_name, "rb") as f:
-        return parse(f.read())
+
+    _pattern = (b"PGP PRIVATE KEY BLOCK",)
```

### Comparing `pem-21.2.0/src/pem/twisted.py` & `pem-23.1.0/src/pem/twisted.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,107 +1,117 @@
-# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2013 Hynek Schlawack <hs@ox.cx>
+#
+# SPDX-License-Identifier: MIT
 
 """
 Twisted-specific convenience helpers.
 """
 
-from __future__ import absolute_import, division, print_function
+from __future__ import annotations
 
-from OpenSSL.SSL import FILETYPE_PEM
-from twisted.internet import ssl
+from typing import TYPE_CHECKING
 
-from ._core import Certificate, DHParameters, Key, parse_file
+from OpenSSL.crypto import FILETYPE_PEM
+from twisted.internet import ssl
 
+from ._core import parse_file
+from ._object_types import Certificate, DHParameters, Key
 
-# mypy hack: Import typing information without actually importing anything.
-MYPY = False
-if MYPY:  # pragma: nocover
-    from typing import Any, List
 
-    from ._core import AbstractPEMObject
+if TYPE_CHECKING:
+    from ._object_types import AbstractPEMObject
 
 
-def certificateOptionsFromPEMs(pemObjects, **kw):
-    # type: (List[AbstractPEMObject], **Any) -> ssl.CerticateOptions
+def certificateOptionsFromPEMs(
+    pemObjects: list[AbstractPEMObject], **kw: object
+) -> ssl.CertificateOptions:
     """
     Load a CertificateOptions from the given collection of PEM objects
     (already-loaded private keys and certificates).
 
     In those PEM objects, identify one private key and its corresponding
     certificate to use as the primary certificate.  Then use the rest of the
     certificates found as chain certificates.  Raise a ValueError if no
     certificate matching a private key is found.
 
-    :return: A TLS context factory using *pemObjects*
-    :rtype: `twisted.internet.ssl.CertificateOptions`_
+    Args:
+        pemObjects (list[AbstractPEMObject]): A list of PEM objects to load.
+
+    Returns:
+        `twisted.internet.ssl.CertificateOptions`_: A TLS context factory using *pemObjects*
 
-    .. _`twisted.internet.ssl.CertificateOptions`: \
-        https://twistedmatrix.com/documents/current/api/\
-        twisted.internet.ssl.CertificateOptions.html
+    .. _`twisted.internet.ssl.CertificateOptions`: https://docs.twistedmatrix.com/en/stable/api/twisted.internet.ssl.CertificateOptions.html
     """
     keys = [key for key in pemObjects if isinstance(key, Key)]
     if not len(keys):
-        raise ValueError("Supplied PEM file(s) does *not* contain a key.")
+        msg = "Supplied PEM file(s) does *not* contain a key."
+        raise ValueError(msg)
     if len(keys) > 1:
-        raise ValueError("Supplied PEM file(s) contains *more* than one key.")
+        msg = "Supplied PEM file(s) contains *more* than one key."
+        raise ValueError(msg)
 
-    privateKey = ssl.KeyPair.load(str(keys[0]), FILETYPE_PEM)
+    privateKey = ssl.KeyPair.load(str(keys[0]), FILETYPE_PEM)  # type: ignore[no-untyped-call]
 
     certs = [cert for cert in pemObjects if isinstance(cert, Certificate)]
     if not len(certs):
-        raise ValueError("*At least one* certificate is required.")
-    certificates = [ssl.Certificate.loadPEM(str(certPEM)) for certPEM in certs]
-
-    certificatesByFingerprint = dict(
-        [
-            (certificate.getPublicKey().keyHash(), certificate)
-            for certificate in certificates
-        ]
-    )
+        msg = "*At least one* certificate is required."
+        raise ValueError(msg)
+    certificates = [
+        ssl.Certificate.loadPEM(str(certPEM))  # type: ignore[no-untyped-call]
+        for certPEM in certs
+    ]
+
+    certificatesByFingerprint = {
+        certificate.getPublicKey().keyHash(): certificate
+        for certificate in certificates
+    }
 
     if privateKey.keyHash() not in certificatesByFingerprint:
-        raise ValueError(
-            "No certificate matching {fingerprint} found.".format(
-                fingerprint=privateKey.keyHash()
-            )
-        )
+        msg = f"No certificate matching {privateKey.keyHash()} found."
+        raise ValueError(msg)
 
     primaryCertificate = certificatesByFingerprint.pop(privateKey.keyHash())
 
     if "dhParameters" in kw:
-        raise TypeError(
-            "Passing DH parameters as a keyword argument instead of a "
-            "PEM object is not supported anymore."
-        )
+        msg = "Passing DH parameters as a keyword argument instead of a PEM object is not supported anymore."
+        raise TypeError(msg)
 
     dhparams = [o for o in pemObjects if isinstance(o, DHParameters)]
     if len(dhparams) > 1:
-        raise ValueError(
-            "Supplied PEM file(s) contain(s) *more* than one set of DH "
-            "parameters."
+        msg = "Supplied PEM file(s) contain(s) *more* than one set of DH parameters."
+        raise ValueError(msg)
+
+    if len(dhparams) == 1:
+        kw["dhParameters"] = ssl.DiffieHellmanParameters(  # type: ignore[no-untyped-call]
+            str(dhparams[0])
         )
-    elif len(dhparams) == 1:
-        kw["dhParameters"] = ssl.DiffieHellmanParameters(str(dhparams[0]))
 
-    ctxFactory = ssl.CertificateOptions(
+    return ssl.CertificateOptions(  # type: ignore[no-any-return]
         privateKey=privateKey.original,
         certificate=primaryCertificate.original,
         extraCertChain=[
             chain.original for chain in certificatesByFingerprint.values()
         ],
-        **kw
+        **kw,
     )
 
-    return ctxFactory
 
-
-def certificateOptionsFromFiles(*pemFiles, **kw):
-    # type: (*str, **Any) -> ssl.CertificateOptions
+def certificateOptionsFromFiles(
+    *pemFiles: str, **kw: object
+) -> ssl.CertificateOptions:
     """
     Read all files named by *pemFiles*, and parse them using
     :func:`certificateOptionsFromPEMs`.
+
+    Args:
+        pemFiles (str): All positional arguments are used as filenames to
+            read.
+
+    Returns:
+        `twisted.internet.ssl.CertificateOptions`_: A TLS context factory using
+         PEM objects from *pemFiles*.
     """
-    pems = []  # type: List[AbstractPEMObject]
+    pems: list[AbstractPEMObject] = []
     for pemFile in pemFiles:
         pems += parse_file(pemFile)
 
     return certificateOptionsFromPEMs(pems, **kw)
```

### Comparing `pem-21.2.0/tests/test_core.py` & `pem-23.1.0/tests/test_core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-# -*- coding: utf-8 -*-
-
-from __future__ import absolute_import, division, print_function
+# SPDX-FileCopyrightText: 2013 Hynek Schlawack <hs@ox.cx>
+#
+# SPDX-License-Identifier: MIT
 
 from itertools import combinations
 
 import certifi
 import pytest
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
 
 import pem
 
-from pem._compat import text_type
-
 from .data import (
     CERT_NO_NEW_LINE,
     CERT_PEM_OPENSSL_TRUSTED,
     CERT_PEMS,
     CERT_PEMS_NO_NEW_LINE,
     CRL_PEMS,
     DH_PEM,
     KEY_PEM_DSA_PRIVATE,
     KEY_PEM_EC_PRIVATE,
+    KEY_PEM_OPENPGP_PRIVATE,
+    KEY_PEM_OPENPGP_PUBLIC,
     KEY_PEM_OPENSSH,
     KEY_PEM_PKCS5_ENCRYPTED,
     KEY_PEM_PKCS5_UNENCRYPTED,
+    KEY_PEM_PKCS5_UNENCRYPTED_PAYLOAD,
     KEY_PEM_PKCS8_ENCRYPTED,
     KEY_PEM_PKCS8_UNENCRYPTED,
     KEY_PEM_PUBLIC,
     KEY_PEM_RFC4716_PUBLIC,
     KEY_PEM_RSA_PUBLIC,
     KEY_PEM_SSHCOM_PRIVATE,
 )
@@ -39,22 +40,22 @@
 # SHA-1 of "test"
 TEST_DIGEST = (
     "PEM string with SHA-1 digest "
     "'a94a8fe5ccb19ba61c4c0873d391e987982fbbd3'"
 )
 
 
-class TestPEMObjects(object):
+class TestPEMObjects:
     def test_cert_has_correct_repr(self):
         """
         Calling repr on a Certificate instance returns the proper string.
         """
         cert = pem.Certificate(b"test")
 
-        assert "<Certificate({0})>".format(TEST_DIGEST) == repr(cert)
+        assert f"<Certificate({TEST_DIGEST})>" == repr(cert)
 
     def test_cert_has_correct_str(self):
         """
         Calling str on a Certificate instance returns the proper string.
         """
         cert = pem.Certificate(b"test")
 
@@ -63,19 +64,17 @@
     def test_cert_req_has_correct_repr(self):
         """
         Calling repr on a CertificateRequest instance returns the proper
         string.
         """
         cert_req = pem.CertificateRequest(b"test")
 
-        assert "<CertificateRequest({0})>".format(TEST_DIGEST) == repr(
-            cert_req
-        )
+        assert f"<CertificateRequest({TEST_DIGEST})>" == repr(cert_req)
 
-    @pytest.mark.parametrize("pem_bytes", (b"test", b"test\r"))
+    @pytest.mark.parametrize("pem_bytes", [b"test", b"test\r"])
     def test_sha1_hexdigest(self, pem_bytes):
         """
         obj.sha1_digest contains the correct digest and caches it properly.
 
         CRs are ignored.
         """
         cert = pem.Certificate(pem_bytes)
@@ -89,15 +88,61 @@
     def test_as_text(self):
         """
         obj.as_text() returns the contents as Unicode.
         """
         cert_text = pem.Certificate(b"test").as_text()
 
         assert "test" == cert_text
-        assert isinstance(cert_text, text_type)
+        assert isinstance(cert_text, str)
+
+    def test_text_payload(self):
+        """
+        obj.text_payload is a base64-encoded payload as text.
+        """
+        payload = pem.parse(KEY_PEM_PKCS5_UNENCRYPTED)[0].text_payload
+
+        assert (
+            KEY_PEM_PKCS5_UNENCRYPTED_PAYLOAD.decode().replace("\n", "")
+            == payload
+        )
+        assert isinstance(payload, str)
+
+    @pytest.mark.parametrize(
+        ("bs", "forbidden"),
+        [
+            (KEY_PEM_SSHCOM_PRIVATE, b"Comment:"),
+            (KEY_PEM_OPENPGP_PUBLIC, b"Version:"),
+            (KEY_PEM_OPENPGP_PRIVATE, b"Comment:"),
+            (KEY_PEM_PKCS5_ENCRYPTED, b"Proc-Type:"),
+        ],
+    )
+    def test_payload_with_headers(self, bs, forbidden):
+        """
+        Headers are removed from the payload.
+        """
+        assert forbidden in bs
+
+        (cert,) = pem.parse(bs)
+
+        assert forbidden.decode() not in cert.text_payload
+        assert forbidden not in cert.bytes_payload
+
+    def test_decoded_payload(self):
+        """
+        obj.decoded_payload is a base64-decoded payload as bytes.
+        """
+        cert = """\
+-----BEGIN EC PRIVATE KEY-----
+cGF5bG9hZF9kYXRhMQ==
+-----END EC PRIVATE KEY-----"""
+
+        payload_bytes = pem.Certificate(cert).decoded_payload
+
+        assert b"payload_data1" == payload_bytes
+        assert isinstance(payload_bytes, bytes)
 
     def test_cert_req_has_correct_str(self):
         """
         Calling str on a CertificateRequest instance returns the proper string.
         """
         cert_req = pem.CertificateRequest(b"test")
 
@@ -105,15 +150,15 @@
 
     def test_key_has_correct_repr(self):
         """
         Calling repr on a Key instance returns the proper string.
         """
         key = pem.Key(b"test")
 
-        assert "<Key({0})>".format(TEST_DIGEST) == repr(key)
+        assert f"<Key({TEST_DIGEST})>" == repr(key)
 
     def test_key_has_correct_str(self):
         """
         Calling str on a Key instance returns the proper string.
         """
         key = pem.Key(b"test")
 
@@ -121,23 +166,23 @@
 
     def test_rsa_private_key_has_correct_repr(self):
         """
         Calling repr on a RSAPrivateKey instance returns the proper string.
         """
         key = pem.RSAPrivateKey(b"test")
 
-        assert "<RSAPrivateKey({0})>".format(TEST_DIGEST) == repr(key)
+        assert f"<RSAPrivateKey({TEST_DIGEST})>" == repr(key)
 
     def test_rsa_public_key_has_correct_repr(self):
         """
         Calling repr on a RSAPublicKey instance returns the proper string.
         """
         key = pem.RSAPublicKey(b"test")
 
-        assert "<RSAPublicKey({0})>".format(TEST_DIGEST) == repr(key)
+        assert f"<RSAPublicKey({TEST_DIGEST})>" == repr(key)
 
     def test_rsa_key_has_correct_str(self):
         """
         Calling str on a RSAPrivateKey instance returns the proper string.
         """
         key = pem.RSAPrivateKey(b"test")
 
@@ -145,15 +190,15 @@
 
     def test_dh_params_has_correct_repr(self):
         """
         Calling repr on a DHParameters instance returns the proper string.
         """
         params = pem.DHParameters(b"test")
 
-        assert "<DHParameters({0})>".format(TEST_DIGEST) == repr(params)
+        assert f"<DHParameters({TEST_DIGEST})>" == repr(params)
 
     def test_dh_params_has_correct_str(self):
         """
         Calling str on a DHParameters instance returns the proper string.
         """
         params = pem.DHParameters(b"test")
 
@@ -162,78 +207,76 @@
     def test_crl_has_correct_repr(self):
         """
         Calling repr on a CertificateRevocationList instance returns the proper
         string.
         """
         crl = pem.CertificateRevocationList(b"test")
 
-        assert "<CertificateRevocationList({0})>".format(TEST_DIGEST) == repr(
-            crl
-        )
+        assert f"<CertificateRevocationList({TEST_DIGEST})>" == repr(crl)
 
     def test_crl_has_correct_str(self):
         """
         Calling str on a CertificateRevocationList instance returns the proper
         string.
         """
         crl = pem.CertificateRevocationList(b"test")
 
         assert str(crl) == "test"
 
-    def test_certificate_unicode(self):
+    def test_certificate_text(self):
         """
         Passing unicode to Certificate encodes the string as ASCII.
         """
-        cert = pem.Certificate(u"a string")
+        cert = pem.Certificate("a string")
 
         assert cert.as_bytes() == b"a string"
         assert str(cert) == "a string"
 
     def test_certificate_request_unicode(self):
         """
         Passing unicode to CertificateRequest encodes the string as ASCII.
         """
-        cert_req = pem.CertificateRequest(u"a string")
+        cert_req = pem.CertificateRequest("a string")
 
         assert cert_req.as_bytes() == b"a string"
         assert str(cert_req) == "a string"
 
     def test_key_unicode(self):
         """
         Passing unicode to Key encodes the string as ASCII.
         """
-        key = pem.Key(u"a string")
+        key = pem.Key("a string")
 
         assert key.as_bytes() == b"a string"
         assert str(key) == "a string"
 
     def test_rsa_key_unicode(self):
         """
         Passing unicode to RSAPrivateKey encodes the string as ASCII.
         """
-        key = pem.RSAPrivateKey(u"a string")
+        key = pem.RSAPrivateKey("a string")
 
         assert key.as_bytes() == b"a string"
         assert str(key) == "a string"
 
     def test_dhparams_unicode_deprecated(self):
         """
         Passing unicode to DHParameters encodes the string as ASCII.
         """
-        params = pem.DHParameters(u"a string")
+        params = pem.DHParameters("a string")
 
         assert params.as_bytes() == b"a string"
         assert str(params) == "a string"
 
     def test_crl_unicode(self):
         """
         Passing unicode to CertificateRevocationList encodes the string as
         ASCII.
         """
-        crl = pem.CertificateRevocationList(u"a string")
+        crl = pem.CertificateRevocationList("a string")
 
         assert crl.as_bytes() == b"a string"
         assert str(crl) == "a string"
 
     def test_certs_equal(self):
         """
         Two Certificate instances with equal contents are equal.
@@ -347,49 +390,50 @@
             pem.CertificateRequest(c),
             pem.Key(c),
             pem.RSAPrivateKey(c),
             pem.CertificateRevocationList(c),
         ]
 
         for pem1, pem2 in combinations(pems, 2):
-            assert not pem1 == pem2
+            assert not pem1 == pem2  # noqa[SIM201]
             assert pem1 != pem2
 
     def test_incompatible_types(self):
         """
         A PEM object is not equal to some other arbitrary object.
         """
         cert = pem.Certificate(b"test")
 
-        assert not cert == object()
+        assert not cert == object()  # noqa[SIM201]
         assert cert != object()
         assert object() != cert
 
 
 def load_rsa_key(key, password=None):
     return serialization.load_pem_private_key(
         key.as_bytes(), password=password, backend=default_backend()
     )
 
 
-class TestParse(object):
+class TestParse:
     """
     Tests for parsing input with one or multiple PEM objects.
     """
 
     def test_key_pkcs5_unencrypted(self):
         """
         It can load an unencrypted PKCS#5 RSA key as PEM string
         as an RSAPrivateKey.
         """
         rv = pem.parse(KEY_PEM_PKCS5_UNENCRYPTED)
         (key,) = rv
 
         assert isinstance(key, pem.RSAPrivateKey)
         assert KEY_PEM_PKCS5_UNENCRYPTED == key.as_bytes()
+        assert KEY_PEM_PKCS5_UNENCRYPTED_PAYLOAD == key.bytes_payload
 
         crypto_key = load_rsa_key(key)
 
         assert isinstance(crypto_key, RSAPrivateKey)
         assert 512, crypto_key.key_size()
 
     def test_key_pkcs5_encrypted(self):
@@ -495,22 +539,26 @@
         list of corresponding CertificateRevocationLists
         """
         crls = pem.parse(b"".join(CRL_PEMS))
 
         assert all(isinstance(c, pem.CertificateRevocationList) for c in crls)
         assert CRL_PEMS == [crl.as_bytes() for crl in crls]
 
-    def test_file(self, tmpdir):
+    @pytest.mark.parametrize("use_path", [True, False])
+    def test_file(self, tmp_path, use_path):
         """
         A file with multiple certificate PEMs is parsed into a list of
         corresponding Certificates.
         """
-        certs_file = tmpdir.join("certs.pem")
-        certs_file.write(b"".join(CERT_PEMS))
-        certs = pem.parse_file(str(certs_file))
+        certs_file = tmp_path / "certs.pem"
+        certs_file.write_bytes(b"".join(CERT_PEMS))
+        if not use_path:
+            certs_file = str(certs_file)
+
+        certs = pem.parse_file(certs_file)
 
         assert all(isinstance(c, pem.Certificate) for c in certs)
         assert CERT_PEMS == [cert.as_bytes() for cert in certs]
 
     def test_loads_certifi(self):
         """
         Loading certifi returns a list of Certificates.
@@ -553,14 +601,22 @@
         Detects and loads EC private keys.
         """
         key = pem.parse(KEY_PEM_EC_PRIVATE)[0]
 
         assert isinstance(key, pem.ECPrivateKey)
         assert KEY_PEM_EC_PRIVATE == key.as_bytes()
 
+    def test_parse_str(self):
+        """ "
+        parse() accepts str too.
+        """
+        assert pem.parse(KEY_PEM_EC_PRIVATE) == pem.parse(
+            KEY_PEM_EC_PRIVATE.decode()
+        )
+
     def test_openshh_private_key(self):
         """
         Detects and loads private keys in the new OpenSSH private key format.
         """
         (key,) = pem.parse(KEY_PEM_OPENSSH)
 
         assert isinstance(key, pem.OpenSSHPrivateKey)
@@ -593,7 +649,62 @@
         """
         (key,) = pem.parse(
             b"PREAMBLE \n" + KEY_PEM_SSHCOM_PRIVATE + b"\n TRAILING"
         )
 
         assert isinstance(key, pem.SSHCOMPrivateKey)
         assert KEY_PEM_SSHCOM_PRIVATE == key.as_bytes()
+
+    def test_openpgp_public_key(self):
+        """
+        Detects and loads OpenPGP public keys.
+        """
+        (key,) = pem.parse(KEY_PEM_OPENPGP_PUBLIC)
+
+        assert isinstance(key, pem.OpenPGPPublicKey)
+        assert KEY_PEM_OPENPGP_PUBLIC == key.as_bytes()
+
+    def test_openpgp_private_key(self):
+        """
+        Detects and loads OpenPGP private keys.
+        """
+        (key,) = pem.parse(KEY_PEM_OPENPGP_PRIVATE)
+
+        assert isinstance(key, pem.OpenPGPPrivateKey)
+        assert KEY_PEM_OPENPGP_PRIVATE == key.as_bytes()
+
+    @pytest.mark.parametrize(
+        ("bs", "hdrs"),
+        [
+            (KEY_PEM_SSHCOM_PRIVATE, {"Comment": "rsa-key-20210120"}),
+            (
+                KEY_PEM_OPENPGP_PUBLIC,
+                {"Version": "Encryption Desktop 10.4.2 (Build 289)"},
+            ),
+            (
+                KEY_PEM_OPENPGP_PRIVATE,
+                {
+                    "Comment": "https://www.ietf.org/id/draft-bre-openpgp-samples-01.html"
+                },
+            ),
+            (
+                KEY_PEM_PKCS5_ENCRYPTED,
+                {
+                    "DEK-Info": "DES-EDE3-CBC,8A72BD2DC1C9092F",
+                    "Proc-Type": "4,ENCRYPTED",
+                },
+            ),
+        ],
+    )
+    def test_headers(self, bs, hdrs):
+        """
+        Headers are preserved.
+        """
+        assert hdrs == pem.parse(bs)[0].meta_headers
+
+    def test_no_headers(self):
+        """
+        No headers, no problem.
+        """
+        cert = pem.parse(CERT_PEM_OPENSSL_TRUSTED)[0]
+
+        assert {} == cert.meta_headers
```

### Comparing `pem-21.2.0/tests/test_twisted.py` & `pem-23.1.0/tests/test_twisted.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,52 @@
-# -*- coding: utf-8 -*-
-
-from __future__ import absolute_import, division, print_function
+# SPDX-FileCopyrightText: 2013 Hynek Schlawack <hs@ox.cx>
+#
+# SPDX-License-Identifier: MIT
 
 import pytest
 
 from OpenSSL import crypto
 from pretend import call, call_recorder, stub
-from twisted.internet import ssl
+
+
+try:
+    from twisted.internet import ssl
+except ImportError:
+    pytest.skip("Missing Twisted", allow_module_level=True)
 
 import pem
 
 from pem.twisted import certificateOptionsFromFiles
 
 from .data import CERT_PEMS, DH_PEM, KEY_PEM, KEY_PEM2
 
 
-@pytest.fixture
-def keyCertChainDHFile(tmpdir):
+@pytest.fixture(name="keyCertChainDHFile")
+def _keyCertChainDHFile(tmpdir):
     """
     Returns a file containing the key, three certificates, and DH parameters.
     """
     pemFile = tmpdir.join("key_cert_and_chain_and_params.pem")
     pemFile.write(KEY_PEM + b"".join(CERT_PEMS) + DH_PEM)
 
     return pemFile
 
 
-@pytest.fixture
-def keyCertChainFile(tmpdir):
+@pytest.fixture(name="keyCertChainFile")
+def _keyCertChainFile(tmpdir):
     """
     Returns a file containing the key and three certificates.
     """
     pemFile = tmpdir.join("key_cert_and_chain.pem")
     pemFile.write(KEY_PEM + b"".join(CERT_PEMS))
 
     return pemFile
 
 
-class TestCertificateOptionsFromFiles(object):
+class TestCertificateOptionsFromFiles:
     def test_worksWithoutChain(self, tmpdir):
         """
         Creating CO without chain certificates works.
         """
         keyFile = tmpdir.join("key.pem")
         keyFile.write(KEY_PEM)
         certFile = tmpdir.join("cert.pem")
@@ -194,15 +199,15 @@
 
         with pytest.raises(TypeError, match="Passing DH parameters"):
             certificateOptionsFromFiles(
                 str(keyCertChainFile), dhParameters=fakeParameters
             )
 
 
-class _TestForwardCompatibleDHE(object):
+class _TestForwardCompatibleDHE:
     def test_realDHParameterFileSupport(self, monkeypatch, keyCertChainDHFile):
         """
         Pass DH parameters loaded from a file directly to CertificateOptions if
         the installed version of Twisted supports it.
         """
         fakeCtxFactory = object()
         recorder = call_recorder(lambda *a, **kw: fakeCtxFactory)
```

### Comparing `pem-21.2.0/tox.ini` & `pem-23.1.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,76 @@
-[pytest]
-addopts = -ra
-testpaths = tests
-filterwarnings =
-    once::Warning
-
-
-[gh-actions]
-python =
-    2.7: py27
-    3.5: py35
-    3.6: py36
-    3.7: py37, docs
-    3.8: py38, mypy, lint
-    3.9: py39, manifest
+[tox]
+min_version = 4
+env_list =
+    pre-commit,
+    mypy-{pkg,api},
+    py3{8,9,10,11,12}{,-twisted},
+    docs,
+    coverage-report
 
 
-[tox]
-envlist = lint, mypy, {py27,py35,py36,py37,py38,py39}{-twisted,}, manifest, docs, pypi-description, coverage-report
-isolated_build = true
+[testenv]
+package = wheel
+wheel_build_env = .pkg
+pass_env =
+    NO_COLOR
+    FORCE_COLOR
+extras = tests
+deps = twisted: twisted[tls]
+commands = coverage run -m pytest {posargs}
 
 
-[testenv:lint]
+[testenv:pre-commit]
 description = Run all pre-commit hooks.
-basepython = python3.8
 skip_install = true
 deps = pre-commit
-passenv = HOMEPATH  # needed on Windows
 commands = pre-commit run --all-files
 
 
-[testenv]
-description = Run tests and measure coverage.
-extras = tests
-deps = twisted: twisted[tls]
-commands =
-    {py27,py38}{-twisted,}: coverage run -m pytest {posargs}
-    {py35,py36,py37,py39}{-twisted,}: python -m pytest {posargs}
+[testenv:mypy-api]
+description = Type-check our public API.
+extras = types
+commands = mypy tests/typing
 
 
-[testenv:mypy]
-description = Check types
-basepython = python3.8
-extras = tests
-deps = mypy
+[testenv:mypy-pkg]
+description = Type-check the package.
+extras = types
 commands = mypy src
 
 
-[testenv:manifest]
-description = Ensure MANIFEST.in is up to date.
-deps = check-manifest
-commands = check-manifest
-
-
 [testenv:docs]
 description = Build docs and run doctests.
-basepython = python3.7
+# Keep base_python in sync with .readthedocs.yaml & ci.yml/docs
+base_python = py311
 extras = docs
-deps = twisted[tls]
 commands =
-    sphinx-build -W -b html -d {envtmpdir}/doctrees docs docs/_build/html
+    sphinx-build -W -n -a --jobs auto -b html -d {envtmpdir}/doctrees docs docs/_build/html
     sphinx-build -W -b doctest -d {envtmpdir}/doctrees docs docs/_build/html
 
-
-[testenv:pypi-description]
-description = Ensure README.rst renders on PyPI.
-basepython = python3.8
-skip_install = true
-deps =
-    twine
-    pip >= 18.0.0
+[testenv:docs-serve]
+package = editable
+base_python = {[testenv:docs]base_python}
+extras = {[testenv:docs]extras}
+deps = watchfiles
 commands =
-    pip wheel -w {envtmpdir}/build --no-deps .
-    twine check {envtmpdir}/build/*
+    watchfiles \
+        --ignore-paths docs/_build/ \
+        'sphinx-build -W -n --jobs auto -b html -d {envtmpdir}/doctrees docs docs/_build/html' \
+        src \
+        docs
+
+
+[testenv:docs-linkcheck]
+package = editable
+base_python = {[testenv:docs]base_python}
+extras = {[testenv:docs]extras}
+commands = sphinx-build -W -b linkcheck -d {envtmpdir}/doctrees docs docs/_build/html
 
 
 [testenv:coverage-report]
 description = Report coverage over all test runs.
-basepython = python3.8
 deps = coverage[toml]>=5.0.2
 skip_install = true
 commands =
     coverage combine
     coverage report
```

