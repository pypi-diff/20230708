# Comparing `tmp/VirxERLU_RLib-1.1.2.tar.gz` & `tmp/VirxERLU_RLib-1.2.0.tar.gz`

## Comparing `VirxERLU_RLib-1.1.2.tar` & `VirxERLU_RLib-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 VirxERLU_RLib-1.1.2/Cargo.toml
--rw-r--r--   0     1001      123    12715 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/Cargo.lock
--rw-r--r--   0     1001      123     3406 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/README.md
--rw-r--r--   0     1001      123      597 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/pyproject.toml
--rw-r--r--   0     1001      123     8684 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/air.rs
--rw-r--r--   0     1001      123    12054 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/analyzer.rs
--rw-r--r--   0     1001      123    20096 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/car.rs
--rw-r--r--   0     1001      123     2956 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/constants.rs
--rw-r--r--   0     1001      123     7931 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/ground.rs
--rw-r--r--   0     1001      123    19188 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/lib.rs
--rw-r--r--   0     1001      123    10833 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/pytypes.rs
--rw-r--r--   0     1001      123     8713 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/shot.rs
--rw-r--r--   0     1001      123     5677 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/utils.rs
--rw-r--r--   0     1001      123     4764 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/virx_erlu_rlib.pyi
--rw-r--r--   0        0        0     4211 1970-01-01 00:00:00.000000 VirxERLU_RLib-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 VirxERLU_RLib-1.2.0/Cargo.toml
+-rw-r--r--   0     1001      123    12486 2023-07-08 13:15:22.000000 VirxERLU_RLib-1.2.0/Cargo.lock
+-rw-r--r--   0     1001      123     3406 2023-07-08 13:15:22.000000 VirxERLU_RLib-1.2.0/README.md
+-rw-r--r--   0     1001      123      597 2023-07-08 13:15:22.000000 VirxERLU_RLib-1.2.0/pyproject.toml
+-rw-r--r--   0     1001      123     9510 2023-07-08 13:15:22.000000 VirxERLU_RLib-1.2.0/src/air.rs
+-rw-r--r--   0     1001      123    12810 2023-07-08 13:15:22.000000 VirxERLU_RLib-1.2.0/src/analyzer.rs
+-rw-r--r--   0     1001      123    20136 2023-07-08 13:15:22.000000 VirxERLU_RLib-1.2.0/src/car.rs
+-rw-r--r--   0     1001      123     3280 2023-07-08 13:15:22.000000 VirxERLU_RLib-1.2.0/src/constants.rs
+-rw-r--r--   0     1001      123     7975 2023-07-08 13:15:22.000000 VirxERLU_RLib-1.2.0/src/ground.rs
+-rw-r--r--   0     1001      123    19719 2023-07-08 13:15:22.000000 VirxERLU_RLib-1.2.0/src/lib.rs
+-rw-r--r--   0     1001      123    10991 2023-07-08 13:15:22.000000 VirxERLU_RLib-1.2.0/src/pytypes.rs
+-rw-r--r--   0     1001      123     8797 2023-07-08 13:15:22.000000 VirxERLU_RLib-1.2.0/src/shot.rs
+-rw-r--r--   0     1001      123     5837 2023-07-08 13:15:22.000000 VirxERLU_RLib-1.2.0/src/utils.rs
+-rw-r--r--   0     1001      123     4764 2023-07-08 13:15:22.000000 VirxERLU_RLib-1.2.0/virx_erlu_rlib.pyi
+-rw-r--r--   0        0        0     4211 1970-01-01 00:00:00.000000 VirxERLU_RLib-1.2.0/PKG-INFO
```

### Comparing `VirxERLU_RLib-1.1.2/Cargo.toml` & `VirxERLU_RLib-1.2.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "virx_erlu_rlib"
-version = "1.1.2"
+version = "1.2.0"
 edition = "2021"
 authors = ["VirxEC <virx@virxcase.dev>"]
 readme = "README.md"
 description = "Rust modules for VirxERLU"
 homepage = "https://github.com/VirxEC/VirxERLU-RLib"
 license = "MIT"
 include = ["/src", "pyproject.toml", "virx_erlu_rlib.pyi", "/README.md"]
@@ -31,23 +31,23 @@
 features = ["stable-compression", "standard", "dropshot", "hoops", "throwback"]
 
 [dependencies.glam]
 version = "0.24.0"
 features = ["fast-math"]
 
 [dependencies.pyo3]
-version = "0.18.1"
+version = "0.19.1"
 features = ["abi3-py37"]
 
 [features]
 default = ["pyo3/extension-module"]
 
 [profile.release]
 codegen-units = 1
 panic = "abort"
 lto = true
 strip = true
 
 [profile.release-with-debug]
 inherits = "release"
 strip = false
-debug = true
+debug = true
```

### Comparing `VirxERLU_RLib-1.1.2/Cargo.lock` & `VirxERLU_RLib-1.2.0/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -54,28 +54,28 @@
 checksum = "38187dbbf076e5f2b85b5dd3e5fb37aa7ed99986e2b852bc08ea99e84c9d5ca8"
 dependencies = [
  "glam",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "glam"
-version = "0.24.0"
+version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad83ab008a4fa3b31dfa713dd41b5a9bdea1e94e4cf1e2fc274ffbd49b0271d3"
+checksum = "42218cb640844e3872cc3c153dc975229e080a6c4733b34709ef445610550226"
 
 [[package]]
 name = "include-flate"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c2e11569346406931d20276cc460215ee2826e7cad43aa986999cb244dd7adb0"
 dependencies = [
@@ -117,23 +117,23 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libflate"
-version = "1.3.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97822bf791bd4d5b403713886a5fbe8bf49520fe78e323b0dc480ca1a03e50b0"
+checksum = "5ff4ae71b685bbad2f2f391fe74f6b7659a34871c08b210fdc039e43bee07d18"
 dependencies = [
  "adler32",
  "crc32fast",
  "libflate_lz77",
 ]
 
 [[package]]
@@ -143,58 +143,58 @@
 checksum = "a52d3a8bfc85f250440e4424db7d857e241a3aebbbe301f3eb606ab15c39acbf"
 dependencies = [
  "rle-decode-fast",
 ]
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
@@ -203,86 +203,86 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.58"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radsort"
 version = "0.1.0"
@@ -317,26 +317,26 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rl_ball_sym"
-version = "3.1.0"
+version = "3.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a742f7f8f7b1b7d3f1a75bdc6ed151d86cd83cb35dbc201314d7bbaf3cc4be65"
+checksum = "bcbf8024d35e360f54930c6fab35b0243a5fd9d4c884c9792a1028dde45e1e7c"
 dependencies = [
  "byteorder",
  "combo_vec",
  "glam",
  "include-flate",
  "radsort",
 ]
@@ -351,50 +351,50 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "virx_erlu_rlib"
-version = "1.1.2"
+version = "1.2.0"
 dependencies = [
  "combo_vec",
  "dubins_paths",
  "glam",
  "pyo3",
  "rand",
  "rl_ball_sym",
@@ -403,71 +403,62 @@
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
-
-[[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `VirxERLU_RLib-1.1.2/README.md` & `VirxERLU_RLib-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `VirxERLU_RLib-1.1.2/pyproject.toml` & `VirxERLU_RLib-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `VirxERLU_RLib-1.1.2/src/air.rs` & `VirxERLU_RLib-1.2.0/src/air.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 use std::f32::consts::PI;
 
 use dubins_paths::{NoPathError, Result as DubinsResult};
-use glam::Vec3A;
+use glam::{Vec2, Vec3A};
 
 use crate::{
     car::{Car, State},
     constants::*,
     pytypes::{BasicShotInfo, ShotType},
     BoostAmount, Mutators,
 };
 
 #[inline]
 fn angle_3d(a: Vec3A, b: Vec3A) -> f32 {
-    a.dot(b).clamp(-1., 1.).acos()
+    a.dot(b).acos()
 }
 
 #[derive(Debug)]
 pub struct AerialTargetInfo {
     pub shot_vector: Vec3A,
     pub jump_type: AerialJumpType,
     pub final_target: Vec3A,
@@ -29,28 +29,36 @@
     pub const fn get_basic_shot_info(&self, time: f32) -> BasicShotInfo {
         BasicShotInfo::found(time, ShotType::Aerial, self.shot_vector, true, self.wait_for_land)
     }
 }
 
 /// Estimation of if a pre-established aerial shot is still possible
 #[must_use]
-pub fn partial_validate(target: Vec3A, xf: Vec3A, vf: Vec3A, boost_amount: BoostAmount, boost_accel: f32, car_boost: f32, time_remaining: f32) -> bool {
+pub fn partial_validate(
+    target: Vec3A,
+    xf: Vec3A,
+    vf: Vec3A,
+    boost_amount: BoostAmount,
+    boost_accel: f32,
+    car_boost: f32,
+    time_remaining: f32,
+) -> bool {
     let delta_x = target - xf;
     let Some(f) = delta_x.try_normalize() else {
         return true;
     };
 
-    let required_acc = delta_x.length() / time_remaining.powi(2);
+    let required_acc = 2. * delta_x.length() / time_remaining.powi(2);
     let ratio = required_acc / boost_accel;
     if ratio.abs() > 1. {
         return false;
     }
 
     let tau2 = time_remaining - time_remaining * (1. - ratio).sqrt();
-    if boost_amount != BoostAmount::Unlimited && (tau2.floor() * BOOST_CONSUMPTION).ceil() >= car_boost {
+    if boost_amount != BoostAmount::Unlimited && (tau2 * BOOST_CONSUMPTION).floor() >= car_boost {
         return false;
     }
 
     (vf + f * (boost_accel * tau2)).length() <= MAX_SPEED
 }
 
 #[derive(Debug)]
@@ -63,41 +71,55 @@
     time_remaining: f32,
 }
 
 impl BasicAerialInfo {
     /// Estimation of if the aerial is valid
     fn validate(&self, xf: Vec3A, vf: Vec3A, jump_type: AerialJumpType) -> Option<(AerialJumpType, f32)> {
         let delta_x = self.target - xf;
-        let f = delta_x.try_normalize()?;
+        let f = delta_x.normalize();
         let phi = angle_3d(f, self.car_forward);
 
-        let turn_time = 3. * (phi / 9.).sqrt();
+        let turn_time = if phi < 0.1 {
+            TURN_TIME_POLY_EST[7] * phi as f64 + TURN_TIME_POLY_EST[8]
+        } else {
+            let x = Vec2::new(delta_x.z.atan2(delta_x.x), delta_x.y.atan2(delta_x.x)).length() as f64;
+
+            if x < 0.2 {
+                TURN_TIME_POLY_EST[9] * x.powi(2) + TURN_TIME_POLY_EST[10] * x + TURN_TIME_POLY_EST[11]
+            } else {
+                TURN_TIME_POLY_EST[0] * x.powi(6)
+                    + TURN_TIME_POLY_EST[1] * x.powi(5)
+                    + TURN_TIME_POLY_EST[2] * x.powi(4)
+                    + TURN_TIME_POLY_EST[3] * x.powi(3)
+                    + TURN_TIME_POLY_EST[4] * x.powi(2)
+                    + TURN_TIME_POLY_EST[5] * x
+                    + TURN_TIME_POLY_EST[6]
+            }
+        } as f32;
+
         if turn_time > self.time_remaining {
             return None;
         }
 
-        // when we start boosting
-        let tau1 = turn_time * (1. - AERIAL_START_BOOST_ANGLE / phi.max(f32::EPSILON)).clamp(0., 1.);
-
-        let required_acc = 2. * delta_x.length() / (self.time_remaining - tau1).powi(2);
+        let required_acc = 2. * delta_x.length() / (self.time_remaining - turn_time).powi(2);
         let ratio = required_acc / self.boost_accel;
         if ratio.abs() >= 0.9 {
             return None;
         }
 
         // when we stop boosting
-        let tau2 = self.time_remaining - (self.time_remaining - tau1) * (1. - ratio.clamp(0., 1.)).sqrt();
+        let tau2 = self.time_remaining - (self.time_remaining - turn_time) * (1. - ratio).sqrt();
 
-        let boost_estimate = (tau2 - tau1).floor() * BOOST_CONSUMPTION;
+        let boost_estimate = (tau2 - turn_time).floor() * BOOST_CONSUMPTION;
         if self.boost_amount != BoostAmount::Unlimited && boost_estimate.ceil() >= self.car_boost {
             return None;
         }
 
         // velocity estimate
-        if (vf + f * (self.boost_accel * (tau2 - tau1))).length() >= MAX_SPEED * 0.9 {
+        if (vf + f * (self.boost_accel * (tau2 - turn_time))).length() >= MAX_SPEED * 0.9 {
             return None;
         }
 
         Some((jump_type, boost_estimate))
     }
 }
 
@@ -122,15 +144,19 @@
 ) -> DubinsResult<AerialTargetInfo> {
     let is_on_ground = car.car_state == State::Grounded || time_remaining > car.time_to_land;
 
     if is_on_ground && car.rotmat.z_axis.z >= 0. && time_remaining <= JUMP_MAX_DURATION {
         return Err(NoPathError);
     }
 
-    let land_time = if car.car_state != State::Grounded { car.time_to_land } else { car.last_landing_time };
+    let land_time = if car.car_state != State::Grounded {
+        car.time_to_land
+    } else {
+        car.last_landing_time
+    };
     if is_on_ground && land_time + ON_GROUND_WAIT_TIME > time_remaining {
         return Err(NoPathError);
     }
 
     let quick_speed_required = car.location.distance(target) / time_remaining;
     if quick_speed_required > MAX_SPEED {
         return Err(NoPathError);
@@ -144,16 +170,19 @@
     let mut found: Vec<(AerialJumpType, f32, bool)> = Vec::with_capacity(3);
 
     let boost_accel = mutators.boost_accel + AERIAL_THROTTLE_ACCEL;
 
     let vf_base = car.velocity + gravity * time_remaining;
     let xf_base = car.velocity * time_remaining + gravity * 0.5 * time_remaining.powi(2);
 
-    let target_angle_check =
-        |car_location: Vec3A| check_target_angle.map_or(true, |ball_location| angle_3d((car_location - ball_location).normalize(), -shot_vector) < PI / 2.);
+    let target_angle_check = |car_location: Vec3A| {
+        check_target_angle.map_or(true, |ball_location| {
+            angle_3d((car_location - ball_location).normalize(), -shot_vector) < PI / 2.
+        })
+    };
 
     let ground_time_remaining = time_remaining - car.time_to_land - car.wait_to_jump_time;
     if is_on_ground && ground_time_remaining > 0. && target_angle_check(car.landing_location) {
         const TOTAL_JUMP_ACC: f32 = JUMP_SPEED + JUMP_ACC * JUMP_MAX_DURATION;
 
         let basic_aerial_info = BasicAerialInfo {
             car_forward: car.landing_rotmat.x_axis,
@@ -164,15 +193,16 @@
             time_remaining: ground_time_remaining,
             // car,
         };
 
         if time_remaining > DOUBLE_JUMP_DURATION {
             const TOTAL_JUMP_ACC_2: f32 = JUMP_SPEED + TOTAL_JUMP_ACC;
             const PARITAL_JUMP_LOC: f32 = 2. * JUMP_SPEED + JUMP_ACC * JUMP_MAX_DURATION;
-            const JUMP_LOC_P2: f32 = -(JUMP_SPEED * JUMP_MAX_DURATION + 0.5 * JUMP_MAX_DURATION * JUMP_MAX_DURATION * JUMP_ACC);
+            const JUMP_LOC_P2: f32 =
+                -(JUMP_SPEED * JUMP_MAX_DURATION + 0.5 * JUMP_MAX_DURATION * JUMP_MAX_DURATION * JUMP_ACC);
 
             let vf = vf_base + car.rotmat.z_axis * TOTAL_JUMP_ACC_2;
             let xf = car.landing_location + xf_base + car.rotmat.z_axis * (time_remaining * PARITAL_JUMP_LOC + JUMP_LOC_P2);
 
             if let Some((jump_type, boost)) = basic_aerial_info.validate(xf, vf, AerialJumpType::Double) {
                 found.push((jump_type, boost, true));
             }
@@ -200,29 +230,36 @@
             target,
             time_remaining,
             // car,
         };
 
         if car.car_state != State::DoubleJumped
             && (!is_on_ground
-                || (car.car_state != State::Grounded && (car.velocity.z + gravity.z * car.time_to_land) + mutators.boost_accel * car.time_to_land + JUMP_SPEED > 0.))
+                || (car.car_state != State::Grounded
+                    && (car.velocity.z + gravity.z * car.time_to_land)
+                        + mutators.boost_accel * car.time_to_land
+                        + JUMP_SPEED
+                        > 0.))
         {
             let vf = vf_base + car.rotmat.z_axis * JUMP_SPEED;
             let xf = car.location + xf_base + car.rotmat.z_axis * (JUMP_SPEED * time_remaining);
 
             if let Some((jump_type, boost)) = basic_aerial_info.validate(xf, vf, AerialJumpType::Secondary) {
                 found.push((jump_type, boost, false));
             }
         }
 
         if !is_on_ground
             || car.rotmat.z_axis.z < 0.
-            || (car.car_state != State::Grounded && (car.velocity.z + gravity.z * car.time_to_land) + mutators.boost_accel * car.time_to_land > 0.)
+            || (car.car_state != State::Grounded
+                && (car.velocity.z + gravity.z * car.time_to_land) + mutators.boost_accel * car.time_to_land > 0.)
         {
-            if let Some((jump_type, boost)) = basic_aerial_info.validate(car.location + xf_base, vf_base, AerialJumpType::None) {
+            if let Some((jump_type, boost)) =
+                basic_aerial_info.validate(car.location + xf_base, vf_base, AerialJumpType::None)
+            {
                 found.push((jump_type, boost, false));
             }
         }
     }
 
     if found.is_empty() {
         return Err(NoPathError);
```

### Comparing `VirxERLU_RLib-1.1.2/src/analyzer.rs` & `VirxERLU_RLib-1.2.0/src/analyzer.rs`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,17 @@
             if self.may_shoot(Shot::Jump) {
                 return Ok(ShotType::Jump);
             }
         } else if target.z < self.car.max_double_jump_height && self.may_shoot(Shot::DoubleJump) {
             return Ok(ShotType::DoubleJump);
         }
 
-        if self.car.car_state != State::Grounded || self.car.wait_to_jump_time + self.car.last_landing_time < time_remaining && self.may_shoot(Shot::Aerial) {
+        if self.car.car_state != State::Grounded
+            || self.car.wait_to_jump_time + self.car.last_landing_time < time_remaining && self.may_shoot(Shot::Aerial)
+        {
             return Ok(ShotType::Aerial);
         }
 
         Err(NoPathError)
     }
 
     fn get_jump_info(
@@ -100,40 +102,54 @@
                         0. // for pre-aligned ground shots
                     } else {
                         distance // for non-aligned ground shots
                     },
                 )
             }
             ShotType::Jump => {
-                let time = self.car.jump_time_to_height(self.gravity.z, target.z - self.car.hitbox.height / 2.);
+                let time = self
+                    .car
+                    .jump_time_to_height(self.gravity.z, target.z - self.car.hitbox.height / 2.);
 
                 (Some(time), time * max_speed + 128.)
             }
             ShotType::DoubleJump => {
                 // if we need to do a double jump but we don't even have time for a normal jump
                 if time_remaining < self.car.max_jump_time {
                     return Err(NoPathError);
                 }
 
-                let time = self.car.double_jump_time_to_height(self.gravity.z, target.z - self.car.hitbox.height / 2.);
+                let time = self
+                    .car
+                    .double_jump_time_to_height(self.gravity.z, target.z - self.car.hitbox.height / 2.);
 
                 (Some(time), time * max_speed + 128.)
             }
             ShotType::Aerial => unreachable!(),
         })
     }
 
     #[inline]
     fn should_travel_forwards(&self, time_remaining: f32, shot_vector: Vec3A) -> bool {
         // it's easier for me to think about what I want the criteria to be for going backwards, so I did that then just took the opposite of it for is_forwards
-        let is_backwards = time_remaining < 4. && angle_2d(shot_vector, Vec3A::new(self.car.landing_yaw.cos(), self.car.landing_yaw.sin(), 0.)) > PI * (2. / 3.);
+        let is_backwards = time_remaining < 4.
+            && angle_2d(
+                shot_vector,
+                Vec3A::new(self.car.landing_yaw.cos(), self.car.landing_yaw.sin(), 0.),
+            ) > PI * (2. / 3.);
         self.forwards_only || !is_backwards
     }
 
-    pub fn no_target(&self, ball: &Ball, mut time_remaining: f32, slice_num: usize, shot_type: ShotType) -> DubinsResult<GroundTargetInfo> {
+    pub fn no_target(
+        &self,
+        ball: &Ball,
+        mut time_remaining: f32,
+        slice_num: usize,
+        shot_type: ShotType,
+    ) -> DubinsResult<GroundTargetInfo> {
         let max_speed = self.get_max_speed(slice_num);
 
         time_remaining -= self.car.time_to_land;
         assert!(time_remaining > 0.);
         let car_location = flatten(self.car.landing_location);
         let max_distance = time_remaining * max_speed + self.car_front_length + ball.radius();
 
@@ -143,15 +159,22 @@
         }
 
         let car_to_ball = (ball.location - self.car.location).normalize_or_zero();
 
         let (jump_time, end_distance) = if shot_type == ShotType::Ground {
             (None, 0.)
         } else {
-            self.get_jump_info(ball.location, ball.location, car_to_ball, max_speed, time_remaining, shot_type)?
+            self.get_jump_info(
+                ball.location,
+                ball.location,
+                car_to_ball,
+                max_speed,
+                time_remaining,
+                shot_type,
+            )?
         };
 
         if let Some(jump_time) = jump_time {
             // if we have enough time for just the jump
             if jump_time > time_remaining {
                 return Err(NoPathError);
             }
@@ -167,15 +190,22 @@
                 if should_turn_left {
                     -self.car.landing_rotmat.y_axis
                 } else {
                     self.car.landing_rotmat.y_axis
                 } * rho,
             );
 
-        let (turn_target, turn_target_2) = get_turn_exit_tanget(self.car, flatten(ball.location), center_of_turn, rho, target_is_forwards, is_forwards);
+        let (turn_target, turn_target_2) = get_turn_exit_tanget(
+            self.car,
+            flatten(ball.location),
+            center_of_turn,
+            rho,
+            target_is_forwards,
+            is_forwards,
+        );
 
         // check if the exit point is in the field
         if !self.car.field.is_point_in(turn_target) {
             return Err(NoPathError);
         }
 
         // compute the distance of each path, validating that it is within our current maximum travel distance (returning an error if neither are)
@@ -207,15 +237,19 @@
 
         let turn_arc_distance = turn_angle * rho;
 
         if turn_final_distance + turn_arc_distance > max_distance {
             return Err(NoPathError);
         }
 
-        let enter_yaw = if is_forwards { self.car.landing_yaw } else { mod2pi(self.car.landing_yaw + PI) };
+        let enter_yaw = if is_forwards {
+            self.car.landing_yaw
+        } else {
+            mod2pi(self.car.landing_yaw + PI)
+        };
 
         // construct a path so we can easily follow our defined turn arc
         let path = DubinsPath {
             qi: PosRot::new(car_location, enter_yaw),
             rho,
             type_: if direction_turn_left { PathType::RSL } else { PathType::LSR },
             param: [turn_angle, 0., 0.],
@@ -231,42 +265,58 @@
             is_forwards,
             shot_vector,
             turn_targets: Some((turn_target, turn_target_2)),
             wait_for_land: self.car.car_state != State::Grounded,
         })
     }
 
-    pub fn target(&self, ball: &Ball, shot_vector: Vec3A, mut time_remaining: f32, slice_num: usize, shot_type: ShotType) -> DubinsResult<GroundTargetInfo> {
+    pub fn target(
+        &self,
+        ball: &Ball,
+        shot_vector: Vec3A,
+        mut time_remaining: f32,
+        slice_num: usize,
+        shot_type: ShotType,
+    ) -> DubinsResult<GroundTargetInfo> {
         let offset_target = ball.location - (shot_vector * ball.radius());
         let car_front_length = (self.car.hitbox_offset.x + self.car.hitbox.length) / 2.;
 
         let max_speed = self.get_max_speed(slice_num);
 
         time_remaining -= self.car.time_to_land;
         assert!(time_remaining > 0.);
         let car_location = self.car.landing_location;
         let max_distance = time_remaining * max_speed + car_front_length;
 
         // check if a simplified path is longer than the longest distance we can possibly travel
         if flatten(car_location).distance(flatten(offset_target)) > max_distance {
             return Err(NoPathError);
         }
-        let (jump_time, end_distance) = self.get_jump_info(ball.location, offset_target, shot_vector, max_speed, time_remaining, shot_type)?;
+        let (jump_time, end_distance) = self.get_jump_info(
+            ball.location,
+            offset_target,
+            shot_vector,
+            max_speed,
+            time_remaining,
+            shot_type,
+        )?;
 
         if let Some(jump_time) = jump_time {
             // if we have enough time for just the jump
             if jump_time > time_remaining {
                 return Err(NoPathError);
             }
         }
 
         let exit_turn_target = flatten(offset_target) - (flatten(shot_vector).normalize_or_zero() * end_distance);
 
         // check if the exit point is in the field, and make sure a simplified version of the path isn't longer than the longest distance we can travel
-        if !self.car.field.is_point_in(flatten(exit_turn_target)) || flatten(car_location).distance(exit_turn_target) + end_distance > max_distance {
+        if !self.car.field.is_point_in(flatten(exit_turn_target))
+            || flatten(car_location).distance(exit_turn_target) + end_distance > max_distance
+        {
             return Err(NoPathError);
         }
 
         // calculate and return the dubin's path
 
         let target_angle = shot_vector.y.atan2(shot_vector.x);
         let mut starting_yaw = self.car.landing_yaw;
@@ -279,15 +329,20 @@
 
         let q0 = PosRot::new(flatten(car_location), starting_yaw);
         let q1 = PosRot::new(flatten(exit_turn_target), target_angle);
 
         let path = shortest_path_in_validate(q0, q1, self.get_max_turn_radius(slice_num), &self.car.field, max_distance)?;
 
         let offset_distance = end_distance - car_front_length;
-        let distances = [path.segment_length(0), path.segment_length(1), path.segment_length(2), offset_distance];
+        let distances = [
+            path.segment_length(0),
+            path.segment_length(1),
+            path.segment_length(2),
+            offset_distance,
+        ];
 
         Ok(GroundTargetInfo {
             distances,
             shot_type,
             path,
             jump_time,
             is_forwards,
@@ -302,10 +357,18 @@
         &self,
         mutators: Mutators,
         target: Vec3A,
         shot_vector: Vec3A,
         time_remaining: f32,
         check_target_angle: Option<Vec3A>,
     ) -> DubinsResult<AerialTargetInfo> {
-        aerial_shot_is_viable(self.car, mutators, self.gravity, target, shot_vector, time_remaining, check_target_angle)
+        aerial_shot_is_viable(
+            self.car,
+            mutators,
+            self.gravity,
+            target,
+            shot_vector,
+            time_remaining,
+            check_target_angle,
+        )
     }
 }
```

### Comparing `VirxERLU_RLib-1.1.2/src/car.rs` & `VirxERLU_RLib-1.2.0/src/car.rs`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,19 @@
         // so we'll just ignore that edge case
 
         // this is the vertex of the equation, which also happens to be the apex of the trajectory
         let h = self.velocity.z / -gravity;
         let k = self.velocity.z * self.velocity.z / -gravity;
 
         let normal_gravity = gravity < 0.;
-        let fall_distance = if normal_gravity { self.location.z - 17. } else { 2030. - self.location.z };
+        let fall_distance = if normal_gravity {
+            self.location.z - 17.
+        } else {
+            2030. - self.location.z
+        };
 
         let terminal_velocity = 2300. - flatten(self.velocity).length();
         let time_until_tv = terminal_velocity / -gravity;
         let distance_until_tv = self.velocity.z * time_until_tv + -gravity * (time_until_tv * time_until_tv) / 2.;
 
         if fall_distance <= distance_until_tv {
             let (time1, time2) = vertex_quadratic_solve_for_x(gravity, h, k, -fall_distance);
```

### Comparing `VirxERLU_RLib-1.1.2/src/constants.rs` & `VirxERLU_RLib-1.2.0/src/constants.rs`

 * *Files 21% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 pub const START_THROTTLE_ACCEL_M: f32 = -36. / 35.;
 pub const START_THROTTLE_ACCEL_B: f32 = 1600.;
 pub const END_THROTTLE_ACCEL_M: f32 = -16.;
 pub const END_THROTTLE_ACCEL_B: f32 = 160.;
 
 pub const AERIAL_THROTTLE_ACCEL: f32 = 100. * (2. / 3.);
 pub const BOOST_ACCEL: f32 = 991. + 2. / 3.;
-pub const AERIAL_START_BOOST_ANGLE: f32 = 0.5;
 
 pub const MIN_BOOST_CONSUMPTION: f32 = BOOST_CONSUMPTION * MIN_BOOST_TIME;
 pub const BOOST_CONSUMPTION_DT: f32 = BOOST_CONSUMPTION * SIMULATION_DT;
 pub const BRAKE_ACC_DT: f32 = BRAKE_ACC * SIMULATION_DT;
 
 pub const BRAKE_COAST_TRANSITION: f32 = -(0.45 * BRAKE_ACC + 0.55 * COAST_ACC);
 pub const COASTING_THROTTLE_TRANSITION: f32 = -0.5 * COAST_ACC;
@@ -37,15 +36,16 @@
 pub const ON_GROUND_WAIT_TIME: f32 = 0.6;
 
 pub type NoGamePyErr = exceptions::PyNameError;
 pub const NO_GAME_ERR: &str = "GAME is unset. Call a function like load_soccar first.";
 pub type NoCarPyErr = exceptions::PyIndexError;
 pub const NO_CAR_ERR: &str = "No car at the provided index.";
 pub type NoSlicesPyErr = exceptions::PyValueError;
-pub const NO_SLICES_ERR: &str = "Ball prediction struct has not been initialized yet. Try calling a function like tick() first.";
+pub const NO_SLICES_ERR: &str =
+    "Ball prediction struct has not been initialized yet. Try calling a function like tick() first.";
 pub type NoTargetPyErr = exceptions::PyIndexError;
 pub const NO_TARGET_ERR: &str = "Target no longer exists.";
 pub type NoShotPyErr = exceptions::PyLookupError;
 pub const NO_SHOT_ERR: &str = "Specified target has no found shot.";
 pub type BallChangedPyErr = exceptions::PyAssertionError;
 pub const BALL_CHANGED_ERR: &str = "Ball has changed too much from the original prediction.";
 pub type NoShotSelectedPyErr = exceptions::PyAssertionError;
@@ -57,7 +57,24 @@
 pub type StrayedFromPathPyErr = exceptions::PyAssertionError;
 pub const STRAYED_FROM_PATH_ERR: &str = "Car has strayed from the path.";
 
 pub const STICKY_FORCE: f32 = -325.;
 pub const STICKY_TIMER: f32 = SIMULATION_DT * 3.;
 pub const HOLD_BONUS: f32 = 292. * 5.;
 pub const MAX_HOLD_TIME: f32 = 0.2;
+
+// magic numbers from the gods themselves
+// aka scipy.optimize.curve_fit
+pub const TURN_TIME_POLY_EST: [f64; 12] = [
+    -1.87039867e-03,
+    2.89665376e-02,
+    -1.79716410e-01,
+    5.88462548e-01,
+    -1.10170154e+00,
+    1.30438381e+00,
+    2.31720904e-02,
+    3.43119958e-10,
+    8.33333398e-03,
+    -1.00249604e+01,
+    4.97746568e+00,
+    -3.68316625e-01,
+];
```

### Comparing `VirxERLU_RLib-1.1.2/src/ground.rs` & `VirxERLU_RLib-1.2.0/src/ground.rs`

 * *Files 8% similar despite different names*

```diff
@@ -16,20 +16,30 @@
     let circle_center_to_target = target - circle_center;
     let b = circle_center_to_target.length();
     let th = (radius / b).acos();
     let d = circle_center_to_target.y.atan2(circle_center_to_target.x);
     let (d1s, d1c) = (d + th).sin_cos();
     let (d2s, d2c) = (d - th).sin_cos();
 
-    (circle_center + radius * Vec3A::new(d1c, d1s, 0.), circle_center + radius * Vec3A::new(d2c, d2s, 0.))
+    (
+        circle_center + radius * Vec3A::new(d1c, d1s, 0.),
+        circle_center + radius * Vec3A::new(d2c, d2s, 0.),
+    )
 }
 
 /// Get the exit turn point on a circle where the car will face the target
 #[must_use]
-pub fn get_turn_exit_tanget(car: &Car, target: Vec3A, circle_center: Vec3A, rho: f32, mut target_is_forwards: bool, travel_forwards: bool) -> (Vec3A, Vec3A) {
+pub fn get_turn_exit_tanget(
+    car: &Car,
+    target: Vec3A,
+    circle_center: Vec3A,
+    rho: f32,
+    mut target_is_forwards: bool,
+    travel_forwards: bool,
+) -> (Vec3A, Vec3A) {
     let (t1, t2) = get_turn_exit_tangets(target, circle_center, rho);
     let (mut t1_local, mut t2_local) = (car.localize_2d_location(t1), car.localize_2d_location(t2));
 
     if !travel_forwards {
         t1_local.x *= -1.;
         t2_local.x *= -1.;
         target_is_forwards = !target_is_forwards;
@@ -53,24 +63,37 @@
         (t2, t1)
     }
 }
 
 #[inline]
 #[must_use]
 pub fn angle_2d(vec1: Vec3A, vec2: Vec3A) -> f32 {
-    flatten(vec1).normalize_or_zero().dot(flatten(vec2).normalize_or_zero()).clamp(-1., 1.).acos()
+    flatten(vec1)
+        .normalize_or_zero()
+        .dot(flatten(vec2).normalize_or_zero())
+        .acos()
 }
 
-pub fn shortest_path_in_validate(q0: PosRot, q1: PosRot, rho: f32, car_field: &FieldRect, max_distance: f32) -> DubinsResult<DubinsPath> {
+pub fn shortest_path_in_validate(
+    q0: PosRot,
+    q1: PosRot,
+    rho: f32,
+    car_field: &FieldRect,
+    max_distance: f32,
+) -> DubinsResult<DubinsPath> {
     let mut best_cost = INFINITY;
     let mut best_path = None;
 
     let intermediate_results = Intermediate::from(q0, q1, rho);
 
-    for (i, param) in PathType::ALL.into_iter().flat_map(|path_type| intermediate_results.word(path_type)).enumerate() {
+    for (i, param) in PathType::ALL
+        .into_iter()
+        .flat_map(|path_type| intermediate_results.word(path_type))
+        .enumerate()
+    {
         let cost = param[0] + param[1] + param[2];
         if cost < best_cost && cost * rho <= max_distance {
             let path = DubinsPath {
                 qi: q0,
                 rho,
                 param,
                 type_: PathType::ALL[i],
@@ -104,35 +127,34 @@
     pub turn_targets: Option<(Vec3A, Vec3A)>,
     pub wait_for_land: bool,
 }
 
 impl GroundTargetInfo {
     pub fn can_reach(&self, car: &Car, max_time: f32, mutators: Mutators) -> Result<f32, CantReachError> {
         let is_curved = PathType::CCC.contains(&self.path.type_);
-
         let total_d = self.distances.iter().sum::<f32>();
-
-        let middle_range = {
-            let start = self.distances[0];
-            let end = start + self.distances[1];
-
-            start..end
-        };
-
+        let middle_range = self.distances[0]..self.distances[0] + self.distances[1];
         let direction = if self.is_forwards { 1. } else { -1. };
 
         let mut d = total_d;
         let mut t_r = max_time;
-        let b_s = f32::from(car.boost.min(12));
-        let mut b = f32::from(car.boost) - b_s;
+        let mut b = f32::from(car.boost - car.boost.min(12));
         let mut v = flatten(car.landing_velocity).length() * direction;
 
-        let boost_accel = if mutators.boost_amount == BoostAmount::NoBoost { 0. } else { mutators.boost_accel };
+        let boost_accel = if mutators.boost_amount == BoostAmount::NoBoost {
+            0.
+        } else {
+            mutators.boost_accel
+        };
 
-        let boost_consumption_dt = if mutators.boost_amount == BoostAmount::Unlimited { 0. } else { BOOST_CONSUMPTION_DT };
+        let boost_consumption_dt = if mutators.boost_amount == BoostAmount::Unlimited {
+            0.
+        } else {
+            BOOST_CONSUMPTION_DT
+        };
 
         loop {
             if self.distances[3] < f32::EPSILON && d < 1. {
                 return Ok(t_r.max(0.));
             }
 
             if t_r <= 0. {
@@ -180,17 +202,15 @@
 
             if t <= 0. {
                 boost = false;
             }
 
             throttle *= 1f32.copysign(v);
 
-            let mut accel = 0.;
-
-            accel += if throttle == 0. {
+            let mut accel = if throttle == 0. {
                 COAST_ACC * SIMULATION_DT * 1f32.copysign(-v)
             } else if throttle * v >= 0. {
                 throttle_accel * SIMULATION_DT * throttle
             } else {
                 BRAKE_ACC_DT.copysign(throttle)
             };
 
@@ -201,18 +221,16 @@
 
             if !(is_middle_straight || d < self.distances[3]) {
                 accel -= self.path.rho / E * SIMULATION_DT;
                 accel = accel.min(2295. - v);
             }
 
             v += accel;
-
             t_r -= SIMULATION_DT;
-            let d_delta = (v * direction) * SIMULATION_DT;
-            d -= d_delta;
+            d -= v * direction * SIMULATION_DT;
         }
 
         Ok(t_r)
     }
 
     #[inline]
     #[must_use]
@@ -221,22 +239,28 @@
     }
 }
 
 fn get_throttle_and_boost(throttle_accel: f32, b: f32, t: f32, boost_accel: f32) -> (f32, bool) {
     let acceleration = t / REACTION_TIME;
 
     if acceleration <= BRAKE_COAST_TRANSITION {
-        (-1., false)
-    } else if BRAKE_COAST_TRANSITION < acceleration && acceleration < COASTING_THROTTLE_TRANSITION {
-        (0., false)
+        return (-1., false);
+    } else if (BRAKE_COAST_TRANSITION..COASTING_THROTTLE_TRANSITION).contains(&acceleration) {
+        return (0., false);
+    }
+
+    let throttle_boost_transition = throttle_accel + 0.5 * boost_accel;
+    if (COASTING_THROTTLE_TRANSITION..throttle_boost_transition).contains(&acceleration) {
+        (
+            if throttle_accel == 0. {
+                1.
+            } else {
+                (acceleration / throttle_accel).clamp(0.02, 1.)
+            },
+            false,
+        )
+    } else if throttle_boost_transition < acceleration {
+        (1., b >= MIN_BOOST_CONSUMPTION && t > 0.)
     } else {
-        let throttle_boost_transition = throttle_accel + 0.5 * boost_accel;
-        if (COASTING_THROTTLE_TRANSITION..throttle_boost_transition).contains(&acceleration) {
-            let throttle = if throttle_accel == 0. { 1. } else { (acceleration / throttle_accel).clamp(0.02, 1.) };
-            (throttle, false)
-        } else if throttle_boost_transition < acceleration {
-            (1., b >= MIN_BOOST_CONSUMPTION && t > 0.)
-        } else {
-            (0., false)
-        }
+        (0., false)
     }
 }
```

### Comparing `VirxERLU_RLib-1.1.2/src/lib.rs` & `VirxERLU_RLib-1.2.0/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -218,26 +218,33 @@
 
 #[pyfunction]
 pub fn get_num_ball_slices() -> usize {
     BALL_STRUCT.read().unwrap().len()
 }
 
 #[pyfunction]
-pub fn new_target(left_target: [f32; 3], right_target: [f32; 3], car_index: usize, options: Option<TargetOptions>) -> PyResult<usize> {
+pub fn new_target(
+    left_target: [f32; 3],
+    right_target: [f32; 3],
+    car_index: usize,
+    options: Option<TargetOptions>,
+) -> PyResult<usize> {
     let num_slices = BALL_STRUCT.read().unwrap().len();
 
     if num_slices == 0 {
         return Err(PyErr::new::<NoSlicesPyErr, _>(NO_SLICES_ERR));
     }
 
     let options = Options::new(options, num_slices);
 
     {
         let mut cars = CARS.write().unwrap();
-        let car = cars.get_mut(car_index).ok_or_else(|| PyErr::new::<NoCarPyErr, _>(NO_CAR_ERR))?;
+        let car = cars
+            .get_mut(car_index)
+            .ok_or_else(|| PyErr::new::<NoCarPyErr, _>(NO_CAR_ERR))?;
         car.init(GRAVITY.read().unwrap().z, num_slices, *MUTATORS.read().unwrap());
     }
 
     let target = Some(Target::new(left_target.into(), right_target.into(), car_index, options));
     let mut targets = TARGETS.write().unwrap();
 
     let target_position = targets.iter().position(Option::is_none);
@@ -260,15 +267,17 @@
         return Err(PyErr::new::<NoSlicesPyErr, _>(NO_SLICES_ERR));
     }
 
     let options = Options::new(options, num_slices);
 
     {
         let mut cars = CARS.write().unwrap();
-        let car = cars.get_mut(car_index).ok_or_else(|| PyErr::new::<NoCarPyErr, _>(NO_CAR_ERR))?;
+        let car = cars
+            .get_mut(car_index)
+            .ok_or_else(|| PyErr::new::<NoCarPyErr, _>(NO_CAR_ERR))?;
         car.init(GRAVITY.read().unwrap().z, num_slices, *MUTATORS.read().unwrap());
     }
 
     let target = Some(Target::new_any(car_index, options));
     let mut targets = TARGETS.write().unwrap();
 
     let target_position = targets.iter().position(Option::is_none);
@@ -329,48 +338,66 @@
 }
 
 #[pyfunction]
 pub fn get_targets_length() -> usize {
     TARGETS.read().unwrap().len()
 }
 
-fn analyze_shot(analyzer: &Analyzer, balls: &Predictions, target: &Target, mutators: Mutators, temporary: bool, game_time: f32) -> Option<(Shot, BasicShotInfo)> {
+fn analyze_shot(
+    analyzer: &Analyzer,
+    balls: &Predictions,
+    target: &Target,
+    mutators: Mutators,
+    temporary: bool,
+    game_time: f32,
+) -> Option<(Shot, BasicShotInfo)> {
     let mut shot = None;
 
     for (i, ball) in balls[target.options.min_slice..target.options.max_slice].iter().enumerate() {
         if ball.location.y.abs() > 5120. + ball.collision_radius() {
             break;
         }
 
         let max_time_remaining = ball.time - game_time;
 
         let Ok(shot_type) = analyzer.get_shot_type(ball.location, max_time_remaining) else {
             continue;
         };
 
         if let Some(target_location) = &target.location {
-            let post_info = PostCorrection::new(ball.location, ball.collision_radius(), target_location.left, target_location.right);
+            let post_info = PostCorrection::new(
+                ball.location,
+                ball.collision_radius(),
+                target_location.left,
+                target_location.right,
+            );
 
             if !post_info.fits {
                 continue;
             }
 
             let shot_vector = post_info.get_shot_vector_target(analyzer.car.landing_location, ball.location);
 
             if shot_type == ShotType::Aerial {
                 let ball_edge = ball.location - flatten(shot_vector) * ball.radius();
-                let target_location = ball_edge - Vec3A::new(0., 0., shot_vector.z) * (analyzer.car.hitbox_offset.x + analyzer.car.hitbox.length) / 2.;
+                let target_location = ball_edge
+                    - Vec3A::new(0., 0., shot_vector.z) * (analyzer.car.hitbox_offset.x + analyzer.car.hitbox.length) / 2.;
 
                 let Ok(target_info) = analyzer.aerial_shot(mutators, target_location, shot_vector, max_time_remaining, Some(ball.location)) else {
                     continue;
                 };
 
                 if shot.is_none() {
                     let basic_shot_info = target_info.get_basic_shot_info(ball.time);
-                    let found_shot = if temporary { AirBasedShot::default() } else { AirBasedShot::new(ball, &target_info) }.into();
+                    let found_shot = if temporary {
+                        AirBasedShot::default()
+                    } else {
+                        AirBasedShot::new(ball, &target_info)
+                    }
+                    .into();
                     shot = Some((found_shot, basic_shot_info));
 
                     if !target.options.all {
                         break;
                     }
                 }
 
@@ -396,25 +423,31 @@
                 shot = Some((found_shot, basic_shot_info));
 
                 if !target.options.all {
                     break;
                 }
             }
         } else if shot_type == ShotType::Aerial {
-            let ball_edge = ball.location - flatten(ball.location - analyzer.car.location).normalize_or_zero() * ball.radius();
+            let ball_edge =
+                ball.location - flatten(ball.location - analyzer.car.location).normalize_or_zero() * ball.radius();
             let shot_vector = (ball_edge - analyzer.car.location).normalize_or_zero();
             let target_location = ball_edge - shot_vector * (analyzer.car.hitbox_offset.x + analyzer.car.hitbox.length) / 2.;
 
             let Ok(target_info) = analyzer.aerial_shot(mutators, target_location, shot_vector, max_time_remaining, None) else {
                 continue;
             };
 
             if shot.is_none() {
                 let basic_shot_info = target_info.get_basic_shot_info(ball.time);
-                let found_shot = if temporary { AirBasedShot::default() } else { AirBasedShot::new(ball, &target_info) }.into();
+                let found_shot = if temporary {
+                    AirBasedShot::default()
+                } else {
+                    AirBasedShot::new(ball, &target_info)
+                }
+                .into();
                 shot = Some((found_shot, basic_shot_info));
 
                 if !target.options.all {
                     break;
                 }
             }
         } else if let Ok(target_info) = analyzer.no_target(ball, max_time_remaining, i, shot_type) {
@@ -477,17 +510,22 @@
         let target = targets_gaurd
             .get(target_index)
             .ok_or_else(|| PyErr::new::<NoTargetPyErr, _>(NO_TARGET_ERR))?
             .as_ref()
             .ok_or_else(|| PyErr::new::<NoTargetPyErr, _>(NO_TARGET_ERR))?;
 
         let cars = CARS.read().unwrap();
-        let car = cars.get(target.car_index).ok_or_else(|| PyErr::new::<NoCarPyErr, _>(NO_CAR_ERR))?;
-
-        if car.car_state == State::Demolished || balls.is_empty() || car.time_to_land >= balls.last().map(|slice| slice.time).unwrap_or_default() {
+        let car = cars
+            .get(target.car_index)
+            .ok_or_else(|| PyErr::new::<NoCarPyErr, _>(NO_CAR_ERR))?;
+
+        if car.car_state == State::Demolished
+            || balls.is_empty()
+            || car.time_to_land >= balls.last().map(|slice| slice.time).unwrap_or_default()
+        {
             return Ok(BasicShotInfo::not_found());
         }
 
         let (max_speed, max_turn_radius) = if target.options.use_absolute_max_values {
             (Some(MAX_SPEED), Some(turn_radius(MAX_SPEED)))
         } else {
             (None, None)
@@ -527,36 +565,42 @@
 pub fn get_data_for_shot_with_target(target_index: usize) -> PyResult<AdvancedShotInfo> {
     let targets_gaurd = TARGETS.read().unwrap();
     let target = targets_gaurd
         .get(target_index)
         .ok_or_else(|| PyErr::new::<NoTargetPyErr, _>(NO_TARGET_ERR))?
         .as_ref()
         .ok_or_else(|| PyErr::new::<NoTargetPyErr, _>(NO_TARGET_ERR))?;
-    let shot = target.shot.as_ref().ok_or_else(|| PyErr::new::<NoShotPyErr, _>(NO_SHOT_ERR))?;
+    let shot = target
+        .shot
+        .as_ref()
+        .ok_or_else(|| PyErr::new::<NoShotPyErr, _>(NO_SHOT_ERR))?;
 
     let time_remaining = shot.time() - *GAME_TIME.read().unwrap();
 
     if time_remaining < 0. {
         return Err(PyErr::new::<NoTimeRemainingPyErr, _>(NO_TIME_REMAINING_ERR));
     }
 
     let cars_guard = CARS.read().unwrap();
-    let car = cars_guard.get(target.car_index).ok_or_else(|| PyErr::new::<NoCarPyErr, _>(NO_CAR_ERR))?;
+    let car = cars_guard
+        .get(target.car_index)
+        .ok_or_else(|| PyErr::new::<NoCarPyErr, _>(NO_CAR_ERR))?;
 
     let ball_struct = BALL_STRUCT.read().unwrap();
     let slice_num = ((time_remaining * TPS).round() as usize).clamp(1, ball_struct.len()) - 1;
     let ball = ball_struct[slice_num];
 
     if ball.location.distance(shot.ball_location()) > car.hitbox.width {
         return Err(PyErr::new::<BallChangedPyErr, _>(BALL_CHANGED_ERR));
     }
 
     match shot {
         Shot::GroundBased(shot_details) => {
-            let shot_info = AdvancedShotInfo::get_from_ground(car, shot_details).ok_or_else(|| PyErr::new::<StrayedFromPathPyErr, _>(STRAYED_FROM_PATH_ERR))?;
+            let shot_info = AdvancedShotInfo::get_from_ground(car, shot_details)
+                .ok_or_else(|| PyErr::new::<StrayedFromPathPyErr, _>(STRAYED_FROM_PATH_ERR))?;
 
             if car.max_speed[slice_num] * (time_remaining + 0.1) >= shot_info.get_distance_remaining() {
                 Ok(shot_info)
             } else {
                 Err(PyErr::new::<BadAccelerationPyErr, _>(BAD_ACCELERATION_ERR))
             }
         }
```

### Comparing `VirxERLU_RLib-1.1.2/src/pytypes.rs` & `VirxERLU_RLib-1.2.0/src/pytypes.rs`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,21 @@
     pub forwards_only: Option<bool>,
 }
 
 #[pymethods]
 impl TargetOptions {
     #[new]
     #[inline]
-    const fn __new__(min_slice: Option<usize>, max_slice: Option<usize>, use_absolute_max_values: Option<bool>, all: Option<bool>, forwards_only: Option<bool>) -> Self {
+    const fn __new__(
+        min_slice: Option<usize>,
+        max_slice: Option<usize>,
+        use_absolute_max_values: Option<bool>,
+        all: Option<bool>,
+        forwards_only: Option<bool>,
+    ) -> Self {
         Self {
             min_slice,
             max_slice,
             use_absolute_max_values,
             all,
             forwards_only,
         }
@@ -341,15 +347,18 @@
     fn __str__(&self) -> String {
         if let Some(required_jump_time) = self.required_jump_time {
             format!(
                 "Final target: {:?}, distance remaining: {:.0}, required jump time: {:.1}, num_jumps: {:?}",
                 self.final_target, self.distance_remaining, required_jump_time, self.num_jumps
             )
         } else {
-            format!("Final target: {:?}, distance remaining: {:.0}", self.final_target, self.distance_remaining)
+            format!(
+                "Final target: {:?}, distance remaining: {:.0}",
+                self.final_target, self.distance_remaining
+            )
         }
     }
 }
 
 impl AdvancedShotInfo {
     pub fn get_from_ground(car: &Car, shot: &GroundBasedShot) -> Option<Self> {
         let (segment, pre_index) = shot.find_min_distance_index(car.location);
@@ -372,15 +381,20 @@
 
             shot.path_endpoint.pos + additional_space
         } else {
             shot.path.sample(distance_along + distance).pos
         };
 
         // get all the samples from the vec after index
-        let samples = shot.all_samples.iter().skip(index / GroundBasedShot::ALL_STEP).copied().collect();
+        let samples = shot
+            .all_samples
+            .iter()
+            .skip(index / GroundBasedShot::ALL_STEP)
+            .copied()
+            .collect();
 
         Some(Self {
             final_target: get_tuple_from_vec3(flatten(target)),
             distance_remaining: distance_to_ball,
             path_samples: samples,
             required_jump_time: shot.jump_time,
             current_path_point: get_tuple_from_vec3(flatten(current_path_point)),
```

### Comparing `VirxERLU_RLib-1.1.2/src/shot.rs` & `VirxERLU_RLib-1.2.0/src/shot.rs`

 * *Files 1% similar despite different names*

```diff
@@ -106,16 +106,20 @@
                 target.path.segment_length(0) + target.path.segment_length(1),
                 target.path.length(),
             ];
 
             // the samples for each subpath
             let raw_samples = [
                 target.path.sample_many_range(Self::STEP_DISTANCE, 0f32..segment_distances[0]),
-                target.path.sample_many_range(Self::STEP_DISTANCE, segment_distances[0]..segment_distances[1]),
-                target.path.sample_many_range(Self::STEP_DISTANCE, segment_distances[1]..segment_distances[2]),
+                target
+                    .path
+                    .sample_many_range(Self::STEP_DISTANCE, segment_distances[0]..segment_distances[1]),
+                target
+                    .path
+                    .sample_many_range(Self::STEP_DISTANCE, segment_distances[1]..segment_distances[2]),
                 get_samples_from_line(path_endpoint, direction, target.distances[3], Self::STEP_DISTANCE),
             ];
 
             (
                 raw_samples[0]
                     .iter()
                     .map(posrot_to_xy_tuple)
```

### Comparing `VirxERLU_RLib-1.1.2/src/utils.rs` & `VirxERLU_RLib-1.2.0/src/utils.rs`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,19 @@
     Right,
 }
 
 fn clamp_index(s: Vec3A, start: Vec3A, end: Vec3A) -> ClampDirection {
     let right = s.dot(end.cross(-Vec3A::Z)) < 0.;
     let left = s.dot(start.cross(-Vec3A::Z)) > 0.;
 
-    let return_original = if end.dot(start.cross(-Vec3A::Z)) > 0. { right && left } else { right || left };
+    let return_original = if end.dot(start.cross(-Vec3A::Z)) > 0. {
+        right && left
+    } else {
+        right || left
+    };
 
     if return_original {
         ClampDirection::Middle
     } else if start.dot(s) < end.dot(s) {
         ClampDirection::Right
     } else {
         ClampDirection::Left
@@ -90,17 +94,27 @@
     #[must_use]
     pub fn new(ball_location: Vec3A, ball_radius: f32, target_left: Vec3A, target_right: Vec3A) -> Self {
         let goal_line_perp = (target_right - target_left).cross(Vec3A::Z);
 
         let left_adjusted = (target_left - ball_location).normalize().cross(-Vec3A::Z) * ball_radius;
         let right_adjusted = (target_right - ball_location).normalize().cross(Vec3A::Z) * ball_radius;
 
-        let left_corrected = target_left + if left_adjusted.dot(goal_line_perp) > 0. { Vec3A::ZERO } else { left_adjusted };
-
-        let right_corrected = target_right + if right_adjusted.dot(goal_line_perp) > 0. { Vec3A::ZERO } else { right_adjusted };
+        let left_corrected = target_left
+            + if left_adjusted.dot(goal_line_perp) > 0. {
+                Vec3A::ZERO
+            } else {
+                left_adjusted
+            };
+
+        let right_corrected = target_right
+            + if right_adjusted.dot(goal_line_perp) > 0. {
+                Vec3A::ZERO
+            } else {
+                right_adjusted
+            };
 
         let left_to_right = right_corrected - left_corrected;
         let new_goal_line = left_to_right.normalize();
         let new_goal_width = left_to_right.length();
 
         let new_goal_perp = new_goal_line.cross(Vec3A::Z);
         let goal_center = left_corrected + new_goal_line * new_goal_width * 0.5;
```

### Comparing `VirxERLU_RLib-1.1.2/virx_erlu_rlib.pyi` & `VirxERLU_RLib-1.2.0/virx_erlu_rlib.pyi`

 * *Files identical despite different names*

### Comparing `VirxERLU_RLib-1.1.2/PKG-INFO` & `VirxERLU_RLib-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VirxERLU-RLib
-Version: 1.1.2
+Version: 1.2.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

