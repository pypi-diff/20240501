# Comparing `tmp/servicing-0.0.7.tar.gz` & `tmp/servicing-0.0.8.tar.gz`

## Comparing `servicing-0.0.7.tar` & `servicing-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 servicing-0.0.7/Cargo.toml
--rw-r--r--   0     1001      127     3958 2024-04-24 16:47:43.000000 servicing-0.0.7/.github/workflows/cicd.yml
--rw-r--r--   0     1001      127      686 2024-04-24 16:47:43.000000 servicing-0.0.7/.gitignore
--rw-r--r--   0     1001      127      165 2024-04-24 16:47:43.000000 servicing-0.0.7/.vimspector.json
--rw-r--r--   0     1001      127      693 2024-04-24 16:47:43.000000 servicing-0.0.7/README.md
--rw-r--r--   0     1001      127      271 2024-04-24 16:47:43.000000 servicing-0.0.7/build.rs
--rw-r--r--   0     1001      127     3319 2024-04-24 16:47:43.000000 servicing-0.0.7/servicing.pyi
--rw-r--r--   0     1001      127    18648 2024-04-24 16:47:43.000000 servicing-0.0.7/src/dispatcher/mod.rs
--rw-r--r--   0     1001      127     1455 2024-04-24 16:47:43.000000 servicing-0.0.7/src/error/mod.rs
--rw-r--r--   0     1001      127     5892 2024-04-24 16:47:43.000000 servicing-0.0.7/src/helper/mod.rs
--rw-r--r--   0     1001      127      637 2024-04-24 16:47:43.000000 servicing-0.0.7/src/lib.rs
--rw-r--r--   0     1001      127     3883 2024-04-24 16:47:43.000000 servicing-0.0.7/src/models/mod.rs
--rw-r--r--   0     1001      127      302 2024-04-24 16:47:43.000000 servicing-0.0.7/template/service.yaml
--rw-r--r--   0     1001      127    43003 2024-04-24 16:47:43.000000 servicing-0.0.7/Cargo.lock
--rw-r--r--   0     1001      127      390 2024-04-24 16:47:43.000000 servicing-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 servicing-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 servicing-0.0.8/Cargo.toml
+-rw-r--r--   0     1001      127     3958 2024-05-01 16:09:52.000000 servicing-0.0.8/.github/workflows/cicd.yml
+-rw-r--r--   0     1001      127      686 2024-05-01 16:09:52.000000 servicing-0.0.8/.gitignore
+-rw-r--r--   0     1001      127      165 2024-05-01 16:09:52.000000 servicing-0.0.8/.vimspector.json
+-rw-r--r--   0     1001      127      693 2024-05-01 16:09:52.000000 servicing-0.0.8/README.md
+-rw-r--r--   0     1001      127      271 2024-05-01 16:09:52.000000 servicing-0.0.8/build.rs
+-rw-r--r--   0     1001      127     3432 2024-05-01 16:09:52.000000 servicing-0.0.8/servicing.pyi
+-rw-r--r--   0     1001      127    18688 2024-05-01 16:09:52.000000 servicing-0.0.8/src/dispatcher/mod.rs
+-rw-r--r--   0     1001      127     1455 2024-05-01 16:09:52.000000 servicing-0.0.8/src/error/mod.rs
+-rw-r--r--   0     1001      127     5892 2024-05-01 16:09:52.000000 servicing-0.0.8/src/helper/mod.rs
+-rw-r--r--   0     1001      127      637 2024-05-01 16:09:52.000000 servicing-0.0.8/src/lib.rs
+-rw-r--r--   0     1001      127     4284 2024-05-01 16:09:52.000000 servicing-0.0.8/src/models/mod.rs
+-rw-r--r--   0     1001      127      302 2024-05-01 16:09:52.000000 servicing-0.0.8/template/service.yaml
+-rw-r--r--   0     1001      127    43004 2024-05-01 16:09:52.000000 servicing-0.0.8/Cargo.lock
+-rw-r--r--   0     1001      127      390 2024-05-01 16:09:52.000000 servicing-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 servicing-0.0.8/PKG-INFO
```

### Comparing `servicing-0.0.7/Cargo.toml` & `servicing-0.0.8/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "servicing"
-version = "0.0.7"
+version = "0.0.8"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "servicing"
 crate-type = ["cdylib"]
```

### Comparing `servicing-0.0.7/.github/workflows/cicd.yml` & `servicing-0.0.8/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `servicing-0.0.7/.gitignore` & `servicing-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `servicing-0.0.7/README.md` & `servicing-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `servicing-0.0.7/servicing.pyi` & `servicing-0.0.8/servicing.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,28 @@
     :param port: the port on which the service should running
     :param replicas: the number of replicas of the service
     :param cloud: the cloud on which the service should running
     :param workdir: the working directory of the service
     :param disk_size: the disk size of the service
     :param cpu: the CPU upper bound of the service
     :param memory: the memory upper bound of the service
+    :param accelerators: the GPU upper bound of the service
     :param setup: the setup command of the service
     :param run: the run command of the service
     """
 
     def __init__(self,
                  port: Optional[int] = None,
                  replicas: Optional[int] = None,
                  cloud: Optional[str] = None,
                  workdir: Optional[str] = None,
                  disk_size: Optional[int] = None,
                  cpu: Optional[str] = None,
                  memory: Optional[str] = None,
+                 accelerators: Optional[str] = None,
                  setup: Optional[str] = None,
                  run: Optional[str] = None) -> None: ...
 
 
 class Dispatcher:
     """
     Dispatcher is a class that represents the service dispatcher, which is
```

### Comparing `servicing-0.0.7/src/dispatcher/mod.rs` & `servicing-0.0.8/src/dispatcher/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -513,14 +513,15 @@
                     replicas: Some(5),
                     cloud: Some("aws".to_string()),
                     workdir: None,
                     setup: None,
                     run: None,
                     disk_size: None,
                     cpu: None,
+                    accelerators: None,
                     memory: None,
                 }),
             )
             .unwrap();
 
             // test the runtime... should NOT panic
             dis.rt.block_on(async { "" });
```

### Comparing `servicing-0.0.7/src/error/mod.rs` & `servicing-0.0.8/src/error/mod.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.7/src/helper/mod.rs` & `servicing-0.0.8/src/helper/mod.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.7/src/lib.rs` & `servicing-0.0.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.7/src/models/mod.rs` & `servicing-0.0.8/src/models/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     pub port: Option<u16>,
     pub replicas: Option<u16>,
     pub cloud: Option<String>,
     pub workdir: Option<String>,
     pub disk_size: Option<u16>,
     pub cpu: Option<String>,
     pub memory: Option<String>,
+    pub accelerators: Option<String>,
     pub setup: Option<String>,
     pub run: Option<String>,
 }
 
 #[pymethods]
 impl UserProvidedConfig {
     #[new]
@@ -23,25 +24,27 @@
         port: Option<u16>,
         replicas: Option<u16>,
         cloud: Option<String>,
         workdir: Option<String>,
         disk_size: Option<u16>,
         cpu: Option<String>,
         memory: Option<String>,
+        accelerators: Option<String>,
         setup: Option<String>,
         run: Option<String>,
     ) -> Self {
         UserProvidedConfig {
             port,
             replicas,
             cloud,
             workdir,
             disk_size,
             cpu,
             memory,
+            accelerators,
             setup,
             run,
         }
     }
 }
 
 #[derive(Serialize, Deserialize, Debug)]
@@ -72,14 +75,17 @@
         }
         if let Some(cpu) = &config.cpu {
             self.resources.cpus = cpu.clone();
         }
         if let Some(memory) = &config.memory {
             self.resources.memory = memory.clone();
         }
+        if let Some(accelerators) = &config.accelerators {
+            self.resources.accelerators = Some(accelerators.clone());
+        }
         if let Some(setup) = &config.setup {
             self.setup = setup.clone();
         }
         if let Some(run) = &config.run {
             self.run = run.clone();
         }
     }
@@ -99,27 +105,30 @@
 #[derive(Serialize, Deserialize, Debug)]
 pub struct Resources {
     pub ports: u16,
     pub cloud: String,
     pub cpus: String,
     pub memory: String,
     pub disk_size: u16,
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub accelerators: Option<String>,
 }
 
 impl Default for Configuration {
     fn default() -> Self {
         Configuration {
             service: Service {
                 readiness_probe: "/health".to_string(),
                 replicas: 2,
             },
             resources: Resources {
                 ports: 8080,
                 cpus: "4+".to_string(),
                 memory: "10+".to_string(),
+                accelerators: None,
                 cloud: "aws".to_string(),
                 disk_size: 100,
             },
             workdir: ".".to_string(),
             setup: "conda install cudatoolkit -y\n".to_string()
                 + "pip install poetry\n"
                 + "poetry install\n",
@@ -135,14 +144,15 @@
             readiness_probe: "/".to_string(),
             replicas: 1,
         },
         resources: Resources {
             ports: 8080,
             cpus: "4+".to_string(),
             memory: "10+".to_string(),
+            accelerators: None,
             cloud: "aws".to_string(),
             disk_size: 50,
         },
         setup: "".to_string(),
         workdir: ".".to_string(),
         run: "python -m http.server 8080\n".to_string(),
     }
```

### Comparing `servicing-0.0.7/Cargo.lock` & `servicing-0.0.8/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -93,17 +93,17 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
-version = "0.22.0"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
 
 [[package]]
 name = "bincode"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
@@ -132,17 +132,17 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
+checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -235,17 +235,17 @@
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
@@ -396,17 +396,17 @@
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
@@ -569,17 +569,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "libredox"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
 dependencies = [
@@ -591,17 +591,17 @@
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -741,33 +741,33 @@
 name = "option-ext"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
@@ -895,19 +895,19 @@
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "redox_users"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
@@ -1065,26 +1065,26 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.198"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
+checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.198"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
+checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -1121,15 +1121,15 @@
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
 
 [[package]]
 name = "servicing"
-version = "0.0.7"
+version = "0.0.8"
 dependencies = [
  "base64",
  "bincode",
  "dirs",
  "env_logger",
  "futures",
  "log",
@@ -1165,17 +1165,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "syn"
```

### Comparing `servicing-0.0.7/PKG-INFO` & `servicing-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: servicing
-Version: 0.0.7
+Version: 0.0.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 ### SERVICING: a small binary aimed at service configuration and cluster deployment for OPENAD
```

