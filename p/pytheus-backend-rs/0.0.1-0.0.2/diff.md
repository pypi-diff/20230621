# Comparing `tmp/pytheus_backend_rs-0.0.1.tar.gz` & `tmp/pytheus_backend_rs-0.0.2.tar.gz`

## Comparing `pytheus_backend_rs-0.0.1.tar` & `pytheus_backend_rs-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.1/Cargo.toml
--rw-r--r--   0     1001      123     2792 2023-06-18 13:40:52.000000 pytheus_backend_rs-0.0.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-18 13:40:52.000000 pytheus_backend_rs-0.0.1/.gitignore
--rw-r--r--   0     1001      123      378 2023-06-18 13:40:52.000000 pytheus_backend_rs-0.0.1/pyproject.toml
--rw-r--r--   0     1001      123     1987 2023-06-18 13:40:52.000000 pytheus_backend_rs-0.0.1/src/lib.rs
--rw-r--r--   0     1001      123     7431 2023-06-18 13:40:59.000000 pytheus_backend_rs-0.0.1/Cargo.lock
--rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      299 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.2/Cargo.toml
+-rw-r--r--   0     1001      123     2792 2023-06-20 22:55:30.000000 pytheus_backend_rs-0.0.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-20 22:55:30.000000 pytheus_backend_rs-0.0.2/.gitignore
+-rw-r--r--   0     1001      123      620 2023-06-20 22:55:30.000000 pytheus_backend_rs-0.0.2/pyproject.toml
+-rw-r--r--   0     1001      123     9686 2023-06-20 22:55:30.000000 pytheus_backend_rs-0.0.2/src/lib.rs
+-rw-r--r--   0     1001      123    11135 2023-06-20 22:55:38.000000 pytheus_backend_rs-0.0.2/Cargo.lock
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 pytheus_backend_rs-0.0.2/PKG-INFO
```

### Comparing `pytheus_backend_rs-0.0.1/.github/workflows/CI.yml` & `pytheus_backend_rs-0.0.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pytheus_backend_rs-0.0.1/.gitignore` & `pytheus_backend_rs-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytheus_backend_rs-0.0.1/Cargo.lock` & `pytheus_backend_rs-0.0.2/Cargo.lock`

 * *Files 24% similar despite different names*

```diff
@@ -11,26 +11,82 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bytes"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "combine"
+version = "4.6.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "35ed6e9d84f0b51a7f52daf1c7d71dd136fd7a3f41a8462b8cdb8c78d920fad4"
+dependencies = [
+ "bytes",
+ "memchr",
+]
+
+[[package]]
+name = "either"
+version = "1.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+
+[[package]]
+name = "form_urlencoded"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
+dependencies = [
+ "percent-encoding",
+]
+
+[[package]]
+name = "idna"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
+dependencies = [
+ "unicode-bidi",
+ "unicode-normalization",
+]
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "itertools"
+version = "0.10.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
+dependencies = [
+ "either",
+]
+
+[[package]]
+name = "itoa"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+
+[[package]]
 name = "libc"
 version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "lock_api"
@@ -39,14 +95,20 @@
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
+name = "memchr"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
+
+[[package]]
 name = "memoffset"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
@@ -77,14 +139,20 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
+name = "percent-encoding"
+version = "2.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
@@ -147,44 +215,72 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pytheus-backend-rs"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
+ "itertools",
  "pyo3",
+ "redis",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "redis"
+version = "0.23.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3ea8c51b5dc1d8e5fd3350ec8167f464ec0995e79f2e90a075b63371500d557f"
+dependencies = [
+ "combine",
+ "itoa",
+ "percent-encoding",
+ "ryu",
+ "sha1_smol",
+ "url",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "ryu"
+version = "1.0.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
+name = "sha1_smol"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ae1a47186c03a32177042e55dbc5fd5aee900b8e0069a8d70fba96a9375cd012"
+
+[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "syn"
@@ -200,26 +296,67 @@
 [[package]]
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
+name = "tinyvec"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
+dependencies = [
+ "tinyvec_macros",
+]
+
+[[package]]
+name = "tinyvec_macros"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
+
+[[package]]
+name = "unicode-bidi"
+version = "0.3.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
+name = "unicode-normalization"
+version = "0.1.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+dependencies = [
+ "tinyvec",
+]
+
+[[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "url"
+version = "2.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
+dependencies = [
+ "form_urlencoded",
+ "idna",
+ "percent-encoding",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
```

