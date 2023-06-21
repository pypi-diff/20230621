# Comparing `tmp/asteria_openrgb-0.1.0.tar.gz` & `tmp/asteria_openrgb-0.2.0.tar.gz`

## Comparing `asteria_openrgb-0.1.0.tar` & `asteria_openrgb-0.2.0.tar`

### file list

```diff
@@ -1,1086 +1,32 @@
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria.service
--rw-r--r--   0        0        0    47959 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria_example.jpg
--rw-r--r--   0        0        0   149225 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria_example.xcf
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/bad_config.toml
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/config.toml
--rw-r--r--   0        0        0   648443 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/example.jpg
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/gah.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/notes.md
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/pre-commit
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/requirements.txt
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/sample_config.toml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0     8308 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/__future__.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/__future__.meta.json
--rw-r--r--   0        0        0   184751 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    54031 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19389 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0    21828 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    62693 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0  1075221 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   125953 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   110121 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0   142772 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0    64107 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0   136038 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/functools.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/functools.meta.json
--rw-r--r--   0        0        0    24281 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    88144 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    29610 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    92294 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    48629 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    80880 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   151153 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    15090 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    29717 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    52448 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0    26663 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/string.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/string.meta.json
--rw-r--r--   0        0        0   168143 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   147814 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0    46043 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0   239473 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   429692 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    71403 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    90386 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/asteria/instruments.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/asteria/instruments.meta.json
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/asteria/metrics.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/asteria/metrics.meta.json
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/asteria/scales.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/asteria/scales.meta.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/asteria/utils.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/asteria/utils.meta.json
--rw-r--r--   0        0        0   390387 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   134895 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    12819 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    24988 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9411 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    59295 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    32630 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6505 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    73907 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    68863 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    94447 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12437 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    16561 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/json/__init__.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/json/__init__.meta.json
--rw-r--r--   0        0        0    15533 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/json/decoder.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/json/decoder.meta.json
--rw-r--r--   0        0        0    11493 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/json/encoder.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/json/encoder.meta.json
--rw-r--r--   0        0        0   367395 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/tomli/__init__.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/tomli/__init__.meta.json
--rw-r--r--   0        0        0    54962 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/tomli/_parser.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/tomli/_parser.meta.json
--rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/tomli/_re.data.json
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/tomli/_re.meta.json
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/tomli/_types.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.mypy_cache/3.10/tomli/_types.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.pytest_cache/README.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/__init__.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/__main__.py
--rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/driver.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/instruments.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/metrics.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/scales.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/utils.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0     8308 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/__future__.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/__future__.meta.json
--rw-r--r--   0        0        0   184751 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    54031 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19389 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0    21828 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    62693 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0  1075221 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   125953 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   110121 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0   142772 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0    64107 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0   136038 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/functools.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/functools.meta.json
--rw-r--r--   0        0        0    24281 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    88144 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    29610 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    92294 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    48629 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    80880 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   151153 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    15090 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    29717 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    52448 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0    26663 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/string.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/string.meta.json
--rw-r--r--   0        0        0   168143 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   147814 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0    46043 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0   239473 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   429692 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    71403 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    90386 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/asteria/__init__.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/asteria/__init__.meta.json
--rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/asteria/driver.data.json
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/asteria/driver.meta.json
--rw-r--r--   0        0        0     9593 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/asteria/instruments.data.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/asteria/instruments.meta.json
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/asteria/metrics.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/asteria/metrics.meta.json
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/asteria/scales.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/asteria/scales.meta.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/asteria/utils.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/asteria/utils.meta.json
--rw-r--r--   0        0        0   390387 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   134895 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    12819 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    24988 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9411 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    59295 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    32630 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6505 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    73907 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    68863 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    94447 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12437 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    16561 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/json/__init__.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/json/__init__.meta.json
--rw-r--r--   0        0        0    15533 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/json/decoder.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/json/decoder.meta.json
--rw-r--r--   0        0        0    11493 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/json/encoder.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/json/encoder.meta.json
--rw-r--r--   0        0        0   367395 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/tomli/__init__.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/tomli/__init__.meta.json
--rw-r--r--   0        0        0    54962 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/tomli/_parser.data.json
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/tomli/_parser.meta.json
--rw-r--r--   0        0        0     6992 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/tomli/_re.data.json
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/tomli/_re.meta.json
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/tomli/_types.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.mypy_cache/3.10/tomli/_types.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/asteria/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/bin/Activate.ps1
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/bin/activate
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/bin/activate.csh
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/bin/activate.fish
--rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/bin/asteria
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/bin/pip
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/bin/pip3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/bin/pip3.10
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/bin/python -> /usr/bin/python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/bin/python3.10 -> python
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/distutils-precedence.pth
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/_distutils_hack/override.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria/__init__.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria/__main__.py
--rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria/driver.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria/instruments.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria/metrics.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria/scales.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria/utils.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria-0.1.dist-info/INSTALLER
--rw-r--r--   0        0        0    34455 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria-0.1.dist-info/LICENSE
--rw-r--r--   0        0        0    46073 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria-0.1.dist-info/METADATA
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria-0.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria-0.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria-0.1.dist-info/WHEEL
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria-0.1.dist-info/direct_url.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria-0.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria-0.1.dist-info/top_level.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/openrgb/__init__.py
--rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/openrgb/network.py
--rw-r--r--   0        0        0    22726 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/openrgb/orgb.py
--rw-r--r--   0        0        0    22137 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/openrgb/utils.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/openrgb_python-0.2.15.dist-info/INSTALLER
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/openrgb_python-0.2.15.dist-info/LICENSE.md
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/openrgb_python-0.2.15.dist-info/METADATA
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/openrgb_python-0.2.15.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/openrgb_python-0.2.15.dist-info/WHEEL
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/openrgb_python-0.2.15.dist-info/top_level.txt
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/py.typed
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0     9535 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0    10623 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    20912 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8020 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    12712 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    29985 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18172 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    30315 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12148 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     6307 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    20316 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37596 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    17552 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    24596 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0     9289 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     7456 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     5877 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    10490 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    12190 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7637 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    22962 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/install/legacy.py
--rw-r--r--   0        0        0    27379 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    16611 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17502 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    33506 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24045 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24129 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    18963 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    27878 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/distutils_args.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    21617 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0    75420 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   285222 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    13919 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    26797 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5260 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30068 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13280 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0        0        0    97792 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/t32.exe
--rw-r--r--   0        0        0   182784 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/t64-arm.exe
--rw-r--r--   0        0        0   107520 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0        0        0    91648 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/w32.exe
--rw-r--r--   0        0        0   168448 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/w64-arm.exe
--rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    48841 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12795 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44025 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0   204400 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34557 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pep517/__init__.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pep517/build.py
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pep517/check.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pep517/colorlog.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pep517/compat.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pep517/dirtools.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pep517/envbuild.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pep517/meta.py
--rw-r--r--   0        0        0    13429 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pep517/wrappers.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/__init__.py
--rw-r--r--   0        0        0    11201 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py
--rw-r--r--   0        0        0   108287 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/py31compat.py
--rw-r--r--   0        0        0    12831 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23408 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    32005 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6143 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40292 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35441 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21819 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    72083 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    52792 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213344 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35287 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33240 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    17592 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     5944 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9864 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    95885 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     7954 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14074 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11471 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0     8744 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    36576 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59746 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24224 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    26240 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    34697 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39515 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    44666 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    26060 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    18257 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20070 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39093 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    28156 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11034 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    16899 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22001 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip-22.2.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip-22.2.2.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip-22.2.2.dist-info/METADATA
--rw-r--r--   0        0        0    76116 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip-22.2.2.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip-22.2.2.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip-22.2.2.dist-info/WHEEL
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip-22.2.2.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pip-22.2.2.dist-info/top_level.txt
--rw-r--r--   0        0        0   108568 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/appdirs.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/zipp.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0   132569 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    18410 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213278 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9030 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39007 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25353 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10381 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23003 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_deprecation_warning.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_entry_points.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_imp.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_importlib.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_itertools.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_path.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_reqs.py
--rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/archive_util.py
--rw-r--r--   0        0        0    10875 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/build_meta.py
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/cli-32.exe
--rw-r--r--   0        0        0    74752 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/cli-64.exe
--rw-r--r--   0        0        0   137216 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/cli-arm64.exe
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/cli.exe
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/dep_util.py
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/depends.py
--rw-r--r--   0        0        0    20785 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/discovery.py
--rw-r--r--   0        0        0    45578 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/dist.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/errors.py
--rw-r--r--   0        0        0     5270 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/extension.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/glob.py
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/gui-32.exe
--rw-r--r--   0        0        0    75264 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/gui-64.exe
--rw-r--r--   0        0        0   137728 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/gui-arm64.exe
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/gui.exe
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/installer.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/launch.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/logging.py
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/monkey.py
--rw-r--r--   0        0        0    50561 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/msvc.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/namespaces.py
--rw-r--r--   0        0        0    40020 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/package_index.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/py34compat.py
--rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/sandbox.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/script.tmpl
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/version.py
--rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/wheel.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/windows_support.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/_collections.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/_functools.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/_macos_compat.py
--rw-r--r--   0        0        0    20662 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0        0        0     8601 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0        0        0    14515 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0        0        0    47023 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0        0        0    17943 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/cmd.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0        0        0    15157 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0        0        0     8023 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0        0        0    50131 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0        0        0    10248 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0        0        0    17781 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0        0        0     8092 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0        0        0    13683 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0        0        0    29873 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0        0        0    23279 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/py39compat.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0        0        0    18577 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0        0        0    12094 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0        0        0    15588 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0        0        0    18208 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0        0        0    39304 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_msi.py
--rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0        0        0    15683 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_wininst.py
--rw-r--r--   0        0        0     5593 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0        0        0    31359 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0        0        0    16552 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0        0        0    13131 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0        0        0    30191 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0        0        0    11764 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0        0        0    19237 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py
--rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/typing_extensions.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/zipp.py
--rw-r--r--   0        0        0    30130 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_text.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0   117959 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213278 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9030 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39007 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25353 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10381 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23003 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/_vendor/tomli/_types.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/__init__.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/alias.py
--rw-r--r--   0        0        0    16623 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/build.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0        0        0    13212 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/build_py.py
--rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/develop.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0        0        0    85662 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0        0        0    26216 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/install.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/register.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/rotate.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/sdist.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/setopt.py
--rw-r--r--   0        0        0     8133 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/test.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/upload.py
--rw-r--r--   0        0        0     7492 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/config/__init__.py
--rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/config/_apply_pyprojecttoml.py
--rw-r--r--   0        0        0    16779 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/config/expand.py
--rw-r--r--   0        0        0    18950 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/config/pyprojecttoml.py
--rw-r--r--   0        0        0    23009 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/config/setupcfg.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-r--r--   0        0        0   269900 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools-63.2.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools-63.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools-63.2.0.dist-info/METADATA
--rw-r--r--   0        0        0    37885 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools-63.2.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools-63.2.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools-63.2.0.dist-info/WHEEL
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools-63.2.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/setuptools-63.2.0.dist-info/top_level.txt
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/tomli/_types.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/tomli/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/tomli-2.0.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/tomli-2.0.1.dist-info/LICENSE
--rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/tomli-2.0.1.dist-info/METADATA
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/tomli-2.0.1.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/tomli-2.0.1.dist-info/WHEEL
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/tests/test_instruments.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/tests/test_metrics.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/tests/test_scales.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/tests/test_utils.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/.gitignore
--rw-r--r--   0        0        0    34455 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/LICENSE
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/README.md
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    46246 2020-02-02 00:00:00.000000 asteria_openrgb-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/CHANGELOG
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/asteria.service
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/asteria.service.bak
+-rw-r--r--   0        0        0    47959 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/asteria_example.jpg
+-rw-r--r--   0        0        0   149225 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/asteria_example.xcf
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/bad_config.toml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/config.toml
+-rw-r--r--   0        0        0   648443 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/example.jpg
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/morse_config.toml
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/notes.md
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/pre-commit
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/requirements.txt
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/sample_config.toml
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/asteria/__init__.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/asteria/__main__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/asteria/constants.py
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/asteria/driver.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/asteria/metrics.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/asteria/scales.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/asteria/utils.py
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/asteria/instruments/__init__.py
+-rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/asteria/instruments/morse.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/tests/test_instruments.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/tests/test_metrics.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/tests/test_scales.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/tests/test_utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/.gitignore
+-rw-r--r--   0        0        0    34455 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/README.md
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    47607 2020-02-02 00:00:00.000000 asteria_openrgb-0.2.0/PKG-INFO
```

### Comparing `asteria_openrgb-0.1.0/asteria_example.jpg` & `asteria_openrgb-0.2.0/asteria_example.jpg`

 * *Files identical despite different names*

### Comparing `asteria_openrgb-0.1.0/asteria_example.xcf` & `asteria_openrgb-0.2.0/asteria_example.xcf`

 * *Files identical despite different names*

### Comparing `asteria_openrgb-0.1.0/config.toml` & `asteria_openrgb-0.2.0/config.toml`

 * *Files identical despite different names*

### Comparing `asteria_openrgb-0.1.0/example.jpg` & `asteria_openrgb-0.2.0/example.jpg`

 * *Files identical despite different names*

### Comparing `asteria_openrgb-0.1.0/notes.md` & `asteria_openrgb-0.2.0/notes.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,7 +16,10 @@
         - Also profiles stored here, but not sure what they cover/how they're loaded--might need to adjust systemd unit to pick profile @ startup?
 
 
 # Packaging notes
 - Image in README doesn't show in PyPI (local link doesn't resolve)
     - Could point to `https://gitlab.com/JoshWVS/asteria/-/raw/master/asteria_example.jpg`, but don't love that either?
     - Just host it myself somewhere?
+
+# Systemd notes
+- USER UNITS CAN'T DEPEND ON SYSTEM UNITS WHYYYYY https://wiki.archlinux.org/title/Systemd/User (from https://unix.stackexchange.com/questions/147904/systemd-user-unit-that-depends-on-system-unit-sleep-target)
```

### Comparing `asteria_openrgb-0.1.0/asteria/__main__.py` & `asteria_openrgb-0.2.0/asteria/__main__.py`

 * *Files identical despite different names*

### Comparing `asteria_openrgb-0.1.0/asteria/driver.py` & `asteria_openrgb-0.2.0/asteria/driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from . import instruments, metrics, scales
 import logging
 from openrgb import OpenRGBClient
+from openrgb.utils import RGBColor
 import tomli
 import time
 
 
 MIN_SLEEP_MS = 100  # Always sleep at least this long between iterations
 QUANTUM_MS = 500  # TODO: move into driver (with safety assertion)?
+# Displayed if an instrument encounters an unhandled exception
+ERROR_COLOUR = RGBColor.fromHEX("#FF0000")
 
 
 class OpenRgbDriver:
     def __init__(
         self, config, address, port, termination_event, shut_off_on_disconnect=True
     ):
         self.address = address
@@ -141,17 +144,22 @@
         for zone, instruments in self.zone_mapping.items():
             zone_len = len(zone.leds)
             colours = []
             num_leds = zone_len // len(instruments)
             num_leftover_leds = zone_len % len(instruments)
             for i, instrument in enumerate(instruments):
                 # Assign one extra "leftover" LED to each instrument until we run out
-                output = instrument.display(
-                    num_leds + (1 if i < num_leftover_leds else 0)
-                )
+                num_instrument_leds = num_leds + (1 if i < num_leftover_leds else 0)
+                try:
+                    output = instrument.display(num_instrument_leds)
+                except Exception as e:
+                    logging.warn(
+                        f"Observed exception when running instrument '{instrument}': {e}"
+                    )
+                    output = [ERROR_COLOUR] * num_instrument_leds
                 colours.extend(output)
 
             assert zone_len == len(colours)
             zone.set_colors(colours)
 
     def run(self):
         while not self.finished.is_set():
```

### Comparing `asteria_openrgb-0.1.0/asteria/instruments.py` & `asteria_openrgb-0.2.0/asteria/instruments/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from openrgb.utils import RGBColor
 
-from .utils import clamp
+from ..utils import clamp
 
 LED_OFF = RGBColor.fromHEX("#000000")
 
 
 class Instrument(ABC):
     """An Instrument determines how the LEDs under its control should be illuminated
 
@@ -87,7 +87,15 @@
         filled = [self.colour] * num_filled
         empty = [LED_OFF] * (num_leds - num_filled)
 
         if self.bottom_up:
             return empty + filled
         else:
             return filled + empty
+
+
+# Beware of circular imports! The morse module needs to import the Instrument
+# class we define here, and I want to import the MorseCode class here so that
+# it's available as `asteria.instruments.MorseCode`. If you move this import
+# _before_ the definition of Instrument, that's a circular import and
+# everything will explode.
+from .morse import MorseCode
```

### Comparing `asteria_openrgb-0.1.0/asteria/metrics.py` & `asteria_openrgb-0.2.0/asteria/metrics.py`

 * *Files identical despite different names*

### Comparing `asteria_openrgb-0.1.0/asteria/scales.py` & `asteria_openrgb-0.2.0/asteria/scales.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from .utils import clamp
 
+
 # This looks a little silly, but at time of writing, a scale is required when
 # configuring an instrument--this just makes the intent obvious when the metric
 # doesn't require any rescaling
 def identity(f):
     """Return f unchanged."""
     return lambda: f()
 
 
 def linear(f, lower, upper):
     """Map f to the range [0, 1] using linear interpolation."""
     # TODO: assert upper > lower?
     range = upper - lower
+
     # TODO: support passing arguments to f (not needed for now)
     def calculate_percentage():
         # TODO: warn if metric value is outside [lower, upper]?
         percentage = (f() - lower) / range
         return clamp(percentage)
 
     return calculate_percentage
```

### Comparing `asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria-0.1.dist-info/LICENSE` & `asteria_openrgb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asteria_openrgb-0.1.0/test-venv/lib/python3.10/site-packages/asteria-0.1.dist-info/METADATA` & `asteria_openrgb-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
-Name: asteria
-Version: 0.1
+Name: asteria-openrgb
+Version: 0.2.0
 Summary: A framework to automatically control LEDs via OpenRGB
-Author-email: josh@simpsonian.ca
-License: GNU AFFERO GENERAL PUBLIC LICENSE
+Project-URL: Homepage, https://gitlab.com/JoshWVS/asteria
+Author-email: Joshua Simpson <josh@simpsonian.ca>
+License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
                                     Preamble
@@ -660,22 +661,23 @@
         solutions will be better for different programs; see section 13 for the
         specific requirements.
         
           You should also get your employer (if you work as a programmer) or school,
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
-        
-Project-URL: Homepage, https://gitlab.com/JoshWVS/asteria
-Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tomli (>2)
-Requires-Dist: openrgb-python (>0.2)
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3
+Requires-Dist: openrgb-python>0.2
+Requires-Dist: tomli>2
 Provides-Extra: test
-Requires-Dist: pytest (>7) ; extra == 'test'
+Requires-Dist: pytest>7; extra == 'test'
+Description-Content-Type: text/markdown
 
 # Asteria - a simple [OpenRGB](https://openrgb.org/) driver
 
 OpenRGB is a great tool for controlling your LEDs, but if you want something more than a static pattern, you'll probably
 outgrow its GUI relatively quickly. Fortunately, OpenRGB also offers an SDK that allows programmatic access to your
 LEDs. **Asteria is a framework to faciliate automatically updating your LEDs (via OpenRGB) in response to various
 conditions.** To make that more concrete, let's look at an example.
@@ -693,19 +695,28 @@
 sewers&hellip;):
 
 ![](asteria_example.jpg)
 
 Asteria automatically scales the configured instruments to fit the available LEDs, and periodically updates them (every
 500ms by default). Of course, this is only scratching the surface of what's possible&mdash;what will you come up with?
 
+## Installation
+
+Available on PyPI as
+[`asteria-openrgb`](https://pypi.org/project/asteria-openrgb/) (i.e. `pip
+install asteria-openrgb`).
+
 ## Usage
 
-Invoke the main Asteria driver with `python -m asteria CONFIG_FILE`. Add `--help` for further options.
+Invoke the main Asteria driver with `asteria CONFIG_FILE`. Add `--help` for further options.
+
+For an (overly long-winded) tutorial on how to run Asteria via systemd, see
+[this blog
+post](https://simpsonian.ca/blog/unleash-die-blinkenlights/#part-3-daily-scheduling-with-systemd-services-timers).
 
-**TODO: expand on this; add systemd user unit**
 
 ## Concepts
 
 Here are the key concepts in Astoria:
 
 - The `Driver` is the core Asteria application loop. It's responsible for polling the configured `Instrument`s to get
   their desired LED outputs, and making the OpenRGB SDK calls to set them accordingly. **Note:** generally, users should
@@ -780,30 +791,57 @@
 `LinearHueRange` offers the lighting effect we're interested in (gradually switching from one colour to another).
 There's just one problem: when we read our CPU temperature, we'll probably get a value like `42` (degrees Celsius), but
 `LinearHueRange` expects a value in the range [0, 1]. Fortunately, `scales.linear` handles that type of
 conversion&mdash;we'll just need to tell it what our low and high temperatures thresholds are. Here's what that would
 look like in a config file:
 
 ```toml
-# The header has two levels: the OpenRGB device and zone
-# to which this instrument should be applied
-# Note: each zone could have multiple effects, so the double
-# brackets are required (this is a TOML array of tables)
+# An Asteria config is a TOML array of tables. It defines a mapping like this:
+#
+# {OpenRGB device: {OpenRGB zone: [Asteria instrument(s), ...]}}
+#
+# where each Asteria instrument can optionally have a metric, and that metric
+# can optionally have a scale.
+#
+# Said in words: you have one or more OpenRGB devices (if not, Asteria won't do
+# much...). Each device has one or more OpenRGB zones. Zero or more Asteria
+# instruments can be displayed in each zone.
+
+# We begin by starting our array of tables. Under this header, we'll be adding
+# Asteria instruments to be displayed on device "MSI PRO B550M", in zone
+# "JRAINBOW1".
 [["MSI PRO B550M-VC WIFI (MS-7C95)"."JRAINBOW1"]]
 
-# First, our instrument...
+# Here's our first instrument...
 ["MSI PRO B550M-VC WIFI (MS-7C95)"."JRAINBOW1".instrument]
 type = "LinearHueRange"
 # That's hue as in "HSV hue"
 args = { lower_hue = 180, upper_hue = 360 }
 
-# ...next, our metric...
+# ...which needs a metric...
 ["MSI PRO B550M-VC WIFI (MS-7C95)"."JRAINBOW1".metric]
 type = "get_sensor"
 # Path to my CPU temperature--see metrics.get_sensor for details
 args = { keys = ["k10temp-pci-00c3", "Tctl", "temp1_input"] }
 
-# ...and finally, our scale.
+# ...and also a scale.
 ["MSI PRO B550M-VC WIFI (MS-7C95)"."JRAINBOW1".scale]
 type = "linear"
+# i.e., map a value <= 40 to 0, >= 100 to 1, and use
+# linear interpolation between the two endpoints
 args = { lower = 40, upper = 100 }
+
+
+# We add another instrument by adding another entry to the array.
+# Asteria will divide the LEDs between your effects as evenly as possible.
+[["MSI PRO B550M-VC WIFI (MS-7C95)"."JRAINBOW1"]]
+
+# Here's an instrument that doesn't use a metric or a scale; it just displays a
+# static colour.
+["MSI PRO B550M-VC WIFI (MS-7C95)"."JRAINBOW1".instrument]
+type = "StaticColour"
+args = { hex_colour = "#FF00FF" }
+
+
+# So, overall: with this config, Asteria will set the top half of the LEDs to
+# match my CPU temperature, and the bottom half will stay a solid hot pink.
 ```
```

### Comparing `asteria_openrgb-0.1.0/tests/test_metrics.py` & `asteria_openrgb-0.2.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `asteria_openrgb-0.1.0/tests/test_scales.py` & `asteria_openrgb-0.2.0/tests/test_scales.py`

 * *Files identical despite different names*

### Comparing `asteria_openrgb-0.1.0/README.md` & `asteria_openrgb-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -18,19 +18,28 @@
 sewers&hellip;):
 
 ![](asteria_example.jpg)
 
 Asteria automatically scales the configured instruments to fit the available LEDs, and periodically updates them (every
 500ms by default). Of course, this is only scratching the surface of what's possible&mdash;what will you come up with?
 
+## Installation
+
+Available on PyPI as
+[`asteria-openrgb`](https://pypi.org/project/asteria-openrgb/) (i.e. `pip
+install asteria-openrgb`).
+
 ## Usage
 
-Invoke the main Asteria driver with `python -m asteria CONFIG_FILE`. Add `--help` for further options.
+Invoke the main Asteria driver with `asteria CONFIG_FILE`. Add `--help` for further options.
+
+For an (overly long-winded) tutorial on how to run Asteria via systemd, see
+[this blog
+post](https://simpsonian.ca/blog/unleash-die-blinkenlights/#part-3-daily-scheduling-with-systemd-services-timers).
 
-**TODO: expand on this; add systemd user unit**
 
 ## Concepts
 
 Here are the key concepts in Astoria:
 
 - The `Driver` is the core Asteria application loop. It's responsible for polling the configured `Instrument`s to get
   their desired LED outputs, and making the OpenRGB SDK calls to set them accordingly. **Note:** generally, users should
@@ -105,30 +114,57 @@
 `LinearHueRange` offers the lighting effect we're interested in (gradually switching from one colour to another).
 There's just one problem: when we read our CPU temperature, we'll probably get a value like `42` (degrees Celsius), but
 `LinearHueRange` expects a value in the range [0, 1]. Fortunately, `scales.linear` handles that type of
 conversion&mdash;we'll just need to tell it what our low and high temperatures thresholds are. Here's what that would
 look like in a config file:
 
 ```toml
-# The header has two levels: the OpenRGB device and zone
-# to which this instrument should be applied
-# Note: each zone could have multiple effects, so the double
-# brackets are required (this is a TOML array of tables)
+# An Asteria config is a TOML array of tables. It defines a mapping like this:
+#
+# {OpenRGB device: {OpenRGB zone: [Asteria instrument(s), ...]}}
+#
+# where each Asteria instrument can optionally have a metric, and that metric
+# can optionally have a scale.
+#
+# Said in words: you have one or more OpenRGB devices (if not, Asteria won't do
+# much...). Each device has one or more OpenRGB zones. Zero or more Asteria
+# instruments can be displayed in each zone.
+
+# We begin by starting our array of tables. Under this header, we'll be adding
+# Asteria instruments to be displayed on device "MSI PRO B550M", in zone
+# "JRAINBOW1".
 [["MSI PRO B550M-VC WIFI (MS-7C95)"."JRAINBOW1"]]
 
-# First, our instrument...
+# Here's our first instrument...
 ["MSI PRO B550M-VC WIFI (MS-7C95)"."JRAINBOW1".instrument]
 type = "LinearHueRange"
 # That's hue as in "HSV hue"
 args = { lower_hue = 180, upper_hue = 360 }
 
-# ...next, our metric...
+# ...which needs a metric...
 ["MSI PRO B550M-VC WIFI (MS-7C95)"."JRAINBOW1".metric]
 type = "get_sensor"
 # Path to my CPU temperature--see metrics.get_sensor for details
 args = { keys = ["k10temp-pci-00c3", "Tctl", "temp1_input"] }
 
-# ...and finally, our scale.
+# ...and also a scale.
 ["MSI PRO B550M-VC WIFI (MS-7C95)"."JRAINBOW1".scale]
 type = "linear"
+# i.e., map a value <= 40 to 0, >= 100 to 1, and use
+# linear interpolation between the two endpoints
 args = { lower = 40, upper = 100 }
+
+
+# We add another instrument by adding another entry to the array.
+# Asteria will divide the LEDs between your effects as evenly as possible.
+[["MSI PRO B550M-VC WIFI (MS-7C95)"."JRAINBOW1"]]
+
+# Here's an instrument that doesn't use a metric or a scale; it just displays a
+# static colour.
+["MSI PRO B550M-VC WIFI (MS-7C95)"."JRAINBOW1".instrument]
+type = "StaticColour"
+args = { hex_colour = "#FF00FF" }
+
+
+# So, overall: with this config, Asteria will set the top half of the LEDs to
+# match my CPU temperature, and the bottom half will stay a solid hot pink.
 ```
```

### Comparing `asteria_openrgb-0.1.0/pyproject.toml` & `asteria_openrgb-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "asteria-openrgb"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     { name = "Joshua Simpson", email = "josh@simpsonian.ca" }
 ]
 description = "A framework to automatically control LEDs via OpenRGB"
 readme = "README.md"
 requires-python = ">=3"
 license = { file = "LICENSE" }
```

