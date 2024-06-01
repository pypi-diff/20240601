# Comparing `tmp/rekker-0.1.1.tar.gz` & `tmp/rekker-0.1.2.tar.gz`

## Comparing `rekker-0.1.1.tar` & `rekker-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 rekker-0.1.1/Cargo.toml
--rw-r--r--   0        0        0     1066 2024-05-26 12:08:46.000000 rekker-0.1.1/LICENSE
--rw-r--r--   0        0        0      469 2024-05-26 12:08:46.000000 rekker-0.1.1/README.md
--rw-r--r--   0        0        0      197 2024-05-26 12:08:46.000000 rekker-0.1.1/src/lib.rs
--rw-r--r--   0        0        0    10174 2024-05-26 12:08:46.000000 rekker-0.1.1/src/literal.rs
--rw-r--r--   0        0        0       99 2024-05-26 12:08:46.000000 rekker-0.1.1/src/pipe/mod.rs
--rw-r--r--   0        0        0      680 2024-05-26 12:08:46.000000 rekker-0.1.1/src/pipe/pipe.rs
--rw-r--r--   0        0        0     1966 2024-05-26 12:08:46.000000 rekker-0.1.1/src/pipe/py.rs
--rw-r--r--   0        0        0     7659 2024-05-26 12:08:46.000000 rekker-0.1.1/src/pipe/tcp.rs
--rw-r--r--   0        0        0     1356 2024-05-26 12:08:46.000000 rekker-0.1.1/src/pipe/tls.rs
--rw-r--r--   0        0        0      212 2024-05-26 12:08:46.000000 rekker-0.1.1/src/pipe/udp.rs
--rw-r--r--   0        0        0      312 2024-05-26 12:08:46.000000 rekker-0.1.1/src/py.rs
--rw-r--r--   0        0        0     2389 2024-05-26 12:08:46.000000 rekker-0.1.1/src/req.rs
--rw-r--r--   0        0        0    21723 2024-05-26 12:08:55.000000 rekker-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      387 2024-05-26 12:08:46.000000 rekker-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1056 1970-01-01 00:00:00.000000 rekker-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 rekker-0.1.2/Cargo.toml
+-rw-r--r--   0        0        0     1066 2024-06-01 21:35:52.000000 rekker-0.1.2/LICENSE
+-rw-r--r--   0        0        0      469 2024-06-01 21:35:52.000000 rekker-0.1.2/README.md
+-rw-r--r--   0        0        0      219 2024-06-01 21:35:52.000000 rekker-0.1.2/src/lib.rs
+-rw-r--r--   0        0        0    10174 2024-06-01 21:35:52.000000 rekker-0.1.2/src/literal.rs
+-rw-r--r--   0        0        0       99 2024-06-01 21:35:52.000000 rekker-0.1.2/src/pipe/mod.rs
+-rw-r--r--   0        0        0      964 2024-06-01 21:35:52.000000 rekker-0.1.2/src/pipe/pipe.rs
+-rw-r--r--   0        0        0     9817 2024-06-01 21:35:52.000000 rekker-0.1.2/src/pipe/py.rs
+-rw-r--r--   0        0        0     8313 2024-06-01 21:35:52.000000 rekker-0.1.2/src/pipe/tcp.rs
+-rw-r--r--   0        0        0     1356 2024-06-01 21:35:52.000000 rekker-0.1.2/src/pipe/tls.rs
+-rw-r--r--   0        0        0    10255 2024-06-01 21:35:52.000000 rekker-0.1.2/src/pipe/udp.rs
+-rw-r--r--   0        0        0      312 2024-06-01 21:35:52.000000 rekker-0.1.2/src/py.rs
+-rw-r--r--   0        0        0     2389 2024-06-01 21:35:52.000000 rekker-0.1.2/src/req.rs
+-rw-r--r--   0        0        0    21940 2024-06-01 21:36:00.000000 rekker-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      387 2024-06-01 21:35:52.000000 rekker-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1056 1970-01-01 00:00:00.000000 rekker-0.1.2/PKG-INFO
```

### Comparing `rekker-0.1.1/Cargo.toml` & `rekker-0.1.2/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 name = "rekker"
 description = "Attack library written for rust and python"
 authors = ["GlacierSG <iamglaciersg@gmail.com>"]
 repository = "https://github.com/GlacierSG/rekker"
 readme = "README.md"
 keywords = ["tcp","attack"]
 license = "MIT"
-version = "0.1.1"
+version = "0.1.2"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-pyo3 = { version = "0.21.2", features = ["extension-module"], optional = true}
+pyo3 = { version = "0.20.3", features = ["extension-module"], optional = true}
 colored = "2.1.0"
 rustls = "0.23.5"
 webpki-roots = "0.26.1"
 ctrlc = "3.4.4"
+regex = "1.10.4"
+humantime = "2.1.0"
 
 [lib]
 crate-type = ["cdylib", "lib"]
```

### Comparing `rekker-0.1.1/LICENSE` & `rekker-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rekker-0.1.1/src/literal.rs` & `rekker-0.1.2/src/literal.rs`

 * *Files identical despite different names*

### Comparing `rekker-0.1.1/src/pipe/pipe.rs` & `rekker-0.1.2/src/pipe/pipe.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 use std::io::Result;
+use std::time::Duration;
 
 pub trait Pipe {
     fn recv(&mut self, size: usize) -> Result<Vec<u8>>;
     fn recvn(&mut self, size: usize) -> Result<Vec<u8>>;
     fn recvline(&mut self) -> Result<Vec<u8>>;
     fn recvuntil(&mut self, suffix: impl AsRef<[u8]>) -> Result<Vec<u8>>;
     fn recvall(&mut self) -> Result<Vec<u8>>;
 
-    fn send(&mut self, msg: impl AsRef<[u8]>) -> Result<usize>;
-    fn sendline(&mut self, msg: impl AsRef<[u8]>) -> Result<usize>;
+    fn send(&mut self, msg: impl AsRef<[u8]>) -> Result<()>;
+    fn sendline(&mut self, msg: impl AsRef<[u8]>) -> Result<()>;
     fn sendlineafter(&mut self, suffix: impl AsRef<[u8]>, msg: impl AsRef<[u8]>) -> Result<Vec<u8>>;
+    
+    fn set_recv_timeout(&mut self, dur: Option<Duration>) -> Result<()>;
+    fn recv_timeout(&self) -> Result<Option<Duration>>;
+
+    fn set_send_timeout(&mut self, dur: Option<Duration>) -> Result<()>;
+    fn send_timeout(&self) -> Result<Option<Duration>>;
+
 
     fn debug(&mut self) -> Result<()>;
     fn interactive(&mut self) -> Result<()>;
     fn close(&mut self) -> Result<()>;
 }
```

### Comparing `rekker-0.1.1/src/pipe/tcp.rs` & `rekker-0.1.2/src/pipe/udp.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,119 +1,204 @@
-use std::net::TcpStream;
-use std::io::{self, Read, Write, Result, BufReader, BufRead};
+use std::net::UdpSocket;
+use std::io::{self, Read, Write, Result, Error};
 use std::time::Duration;
 use super::pipe::Pipe;
 use crate::{from_lit, to_lit_colored};
 use std::sync::atomic::{AtomicBool, Ordering};
 use colored::*;
 use std::sync::Arc;
-
-pub struct Tcp {
-    pub stream: TcpStream
+use std::mem;
+use std::io::ErrorKind;
+use regex::Regex;
+
+pub struct Udp {
+    stream: Option<UdpSocket>,
+    buffer: Vec<u8>,
 }
 
-impl Tcp {
-    pub fn connect(addr: &str) -> std::io::Result<Tcp> {
-        Ok(Tcp {
-            stream: TcpStream::connect(addr)?
+#[macro_export]
+macro_rules! handle_stream_option {
+    ($stream:expr) => {
+        match $stream {
+            Some(stream) => stream,
+            None => return Err(Error::new(io::ErrorKind::Other, "UDP Socket is not connected")),
+        }
+    }
+}
+impl Udp {
+    pub fn connect(addr: &str) -> std::io::Result<Udp> {
+        let re = Regex::new(r"\s+").unwrap();
+        let addr = re.replace_all(addr.trim(), ":");
+
+        let stream = UdpSocket::bind("0.0.0.0:0")?; 
+        stream.connect(addr.as_ref())?;
+
+        Ok(Udp {
+            stream: Some(stream),
+            buffer: vec![0; 0]
         })
     }
 
+    fn add_to_buffer(&mut self) -> Result<usize> {
+        handle_stream_option!(&self.stream).set_nonblocking(true)?;
+        let mut total = 0;
+        loop {
+            match self.add_to_buffer_blocking() {
+                Ok(r) => {
+                    total += r;
+                },
+                Err(e) => {
+                    if e.kind() == ErrorKind::WouldBlock {
+                        break
+                    }
+                    else {
+                        handle_stream_option!(&self.stream).set_nonblocking(false)?;
+                        return Err(e);
+                    }
+                }
+            }
+        }
+        handle_stream_option!(&self.stream).set_nonblocking(false)?;
+
+        Ok(total)
+    }
+
+    fn add_to_buffer_blocking(&mut self) -> Result<usize> {
+        let mut temp_buf = vec![0; 65535];
+
+        match handle_stream_option!(&self.stream).recv(&mut temp_buf) {
+            Ok(r) => {
+                self.buffer.extend_from_slice(&temp_buf[..r]);
+                Ok(r)
+            },
+            Err(e) => Err(e)
+        }
+    }
 }
 
-impl Pipe for Tcp {
+impl Pipe for Udp {
     fn recv(&mut self, size: usize) -> Result<Vec<u8>> {
-        let mut buffer = vec![0; size];
-        let size = self.stream.read(&mut buffer)?;
-        Ok(buffer[..size].to_vec())
+        self.add_to_buffer()?;
+       
+        let l = if size < self.buffer.len() { size }
+                else { self.buffer.len() };
+
+        let out = self.buffer[..l].to_vec();
+        self.buffer.drain(..l);
+        Ok(out)
     }
-
     fn recvn(&mut self, size: usize) -> Result<Vec<u8>> {
-        let mut buffer = vec![0; size];
-        let _ = self.stream.read_exact(&mut buffer)?;
-        Ok(buffer)
-    }
+        while self.buffer.len() < size {
+            self.add_to_buffer()?;
+        }
 
+        let out = self.buffer[..size].to_vec();
+        self.buffer.drain(..size);
+        Ok(out)
+    }
     fn recvline(&mut self) -> Result<Vec<u8>> {
-        let mut buffer = Vec::new();
-        let mut reader = BufReader::new(&self.stream);
-
-        reader.read_until(10, &mut buffer)?;
+        let mut bi = 0;
+        loop {
+            for i in bi..self.buffer.len() {
+                if self.buffer[i] == 10 {
+                    let out = self.buffer[..i+1].to_vec();
+                    self.buffer.drain(..i+1);
+                    return Ok(out);
+                }
+            }
+            bi = self.buffer.len();
 
-        Ok(buffer)
+            self.add_to_buffer_blocking()?;
+        }
     }
-
     fn recvuntil(&mut self, suffix: impl AsRef<[u8]>) -> Result<Vec<u8>> {
         let suffix = suffix.as_ref();
         if suffix.len() == 0 {
             return Ok(vec![])
         }
-        let mut buffer = vec![];
 
-        let mut reader = BufReader::new(&self.stream);
+        let mut bi = suffix.len() - 1;
         loop {
-            let mut tmp_buffer = vec![];
-
-            let _ = reader.read_until(suffix[suffix.len()-1], &mut tmp_buffer)?;
-            buffer.extend(tmp_buffer);
-            if suffix.len() <= buffer.len() {
-                if &suffix[..] == &buffer[(buffer.len()-suffix.len())..] {
-                    return Ok(buffer);
+            if suffix.len() <= self.buffer.len() {
+                for i in bi..self.buffer.len() {
+                    if self.buffer[i] == suffix[suffix.len()-1] {
+                        if &suffix[..] == &self.buffer[i+1-suffix.len()..i+1] {
+                            let out = self.buffer[..i+1].to_vec();
+                            self.buffer.drain(..i+1);
+                            return Ok(out);
+                        }
+                    }
                 }
+                bi = self.buffer.len();
             }
+
+            self.add_to_buffer_blocking()?;
         }
     }
-
     fn recvall(&mut self) -> Result<Vec<u8>> {
-        let mut buffer = vec![];
-
-        let mut reader = BufReader::new(&self.stream);
-        let _ = reader.read_to_end(&mut buffer).unwrap();
-        Ok(buffer)
+        self.add_to_buffer()?;
+        Ok(mem::take(&mut self.buffer))
     }
 
-    fn send(&mut self, msg: impl AsRef<[u8]>) -> Result<usize> {
-        self.stream.write(msg.as_ref())
+    fn send(&mut self, msg: impl AsRef<[u8]>) -> Result<()> {
+        let msg = msg.as_ref();
+        let mut total = 0;
+        while total < msg.len() {
+            total += handle_stream_option!(&self.stream).send(&msg[total..])?;
+        }
+        Ok(())
     }
-
-    fn sendline(&mut self, msg: impl AsRef<[u8]>) -> Result<usize> {
-        let mut tmp: Vec<u8> = msg.as_ref().to_vec();
-        tmp.extend(b"\n");
-        self.send(tmp.as_slice())
+    fn sendline(&mut self, msg: impl AsRef<[u8]>) -> Result<()> {
+        let msg = msg.as_ref();
+        let _ = self.send(msg);
+        let _ = self.send(b"\n");
+        Ok(())
     }
-
     fn sendlineafter(&mut self, suffix: impl AsRef<[u8]>, msg: impl AsRef<[u8]>) -> Result<Vec<u8>> {
         let buf = self.recvuntil(suffix)?;
         self.sendline(msg)?;
         Ok(buf)
     }
 
+    fn recv_timeout(&self) -> Result<Option<Duration>> {
+        handle_stream_option!(&self.stream).read_timeout()
+    }
+    fn set_recv_timeout(&mut self, dur: Option<Duration>) -> Result<()> {
+        handle_stream_option!(&self.stream).set_read_timeout(dur)
+    }
+
+    fn send_timeout(&self) -> Result<Option<Duration>> {
+        handle_stream_option!(&self.stream).write_timeout()
+    }
+    fn set_send_timeout(&mut self, dur: Option<Duration>) -> Result<()> {
+        handle_stream_option!(&self.stream).set_write_timeout(dur)
+    }
+
     fn debug(&mut self) -> Result<()> {
         let go_up = "\x1b[1A";
         let clear_line = "\x1b[2K";
         let begin_line = "\r";
         fn prompt() { 
             print!("{} ", "$".red());
             io::stdout().flush().expect("Unable to flush stdout");
         }
         prompt();
         
         let running = Arc::new(AtomicBool::new(true));
         let thread_running = running.clone();
 
-
-        let old_read_timeout = self.stream.read_timeout()?;
-        self.stream.set_read_timeout(Some(Duration::from_millis(1)))?;
+        let old_recv_timeout = self.recv_timeout()?;
+        self.set_recv_timeout(Some(Duration::from_millis(1)))?;
 
 
-        let mut stream_clone = self.stream.try_clone()?;
+        let stream_clone = handle_stream_option!(&self.stream).try_clone()?;
         let receiver = std::thread::spawn(move || {
             let mut buffer = [0; 1024];
             loop {
-                match stream_clone.read(&mut buffer) {
+                match stream_clone.recv(&mut buffer) {
                     Ok(0) => {
                         println!("{}{}{}", begin_line, clear_line, "Pipe broke".red());
                         print!("{}", "Press Enter to continue".red());
                         io::stdout().flush().expect("Unable to flush stdout");
 
                         thread_running.store(false, Ordering::SeqCst);
                         break;
@@ -122,78 +207,75 @@
                         let response = &buffer[0..n];
                         print!("{}{}", begin_line, clear_line);
                         let lit = to_lit_colored(&response, |x| x.normal(), |x| x.yellow());
                         
                         println!("{}",lit);
                         prompt();
                     }
-                    Err(_) => {}
+                    Err(_) => {
+                    }
                 }
 
                 if !thread_running.load(Ordering::SeqCst) { break; }
             }
         });    
 
         let stdin = io::stdin();
         let handle = stdin.lock();
 
         let mut bytes = vec![0; 0];
         for byte_result in handle.bytes() {
-            bytes.push(byte_result?);
-            if bytes[bytes.len()-1] == 10 {
+            bytes.push(byte_result?); 
+            if bytes.len() != 0 && bytes[bytes.len()-1] == 10 {
                 if !running.load(Ordering::SeqCst) {
                     print!("{}{}{}", go_up, begin_line, clear_line,);
                     break;
                 }
-                let d;
-                if bytes.len() > 0 {
-                    d = from_lit(&bytes[..bytes.len()-1]);
-                }
-                else {
-                    d = from_lit(&bytes);
-                }
+                let d = from_lit(&bytes[..bytes.len()-1]);
                 match d {
                     Ok(x) => {
                         bytes = x;
                         let lit = to_lit_colored(&bytes, |x| x.normal(), |x| x.green());
-            
                         println!("{}{}{}", go_up, clear_line, lit);
                         prompt();
-                        self.stream.write_all(&bytes)?;
-                        self.stream.flush()?;
+                        self.send(&bytes)?;
+                    },
+                    Err(e) => {
+                        eprintln!("{}", e.red());
+                        print!("{}", "$ ".red());
+                        io::stdout().flush().expect("Unable to flush stdout");
                     },
-                    Err(e) => eprintln!("{}", e.red()),
                 }
 
                 bytes = vec![0; 0];
             }
         }
         running.store(false, Ordering::SeqCst);
         
-        self.stream.set_read_timeout(old_read_timeout)?;
+        self.set_recv_timeout(old_recv_timeout)?;
 
         receiver.join().unwrap();
         
         Ok(())
     }
 
     fn interactive(&mut self) -> Result<()> {
         let running = Arc::new(AtomicBool::new(true));
         let thread_running = running.clone();
 
 
-        let old_read_timeout = self.stream.read_timeout()?;
-        self.stream.set_read_timeout(Some(Duration::from_millis(1)))?;
+        let old_recv_timeout = self.recv_timeout()?;
+        self.set_recv_timeout(Some(Duration::from_millis(1)))?;
 
 
-        let mut stream_clone = self.stream.try_clone()?;
+        let stream_clone = handle_stream_option!(&self.stream).try_clone()?;
         let receiver = std::thread::spawn(move || {
             let mut buffer = [0; 1024];
             loop {
-                match stream_clone.read(&mut buffer) {
+                match stream_clone.recv(&mut buffer) {
                     Ok(0) => {
                         println!("{}", "Pipe broke".red());
                         print!("{}", "Press Enter to continue".red());
                         io::stdout().flush().expect("Unable to flush stdout");
 
                         thread_running.store(false, Ordering::SeqCst);
                         break;
@@ -217,31 +299,28 @@
         for byte_result in handle.bytes() {
             bytes.push(byte_result?);
             if bytes[bytes.len()-1] == 10 {
                 if !running.load(Ordering::SeqCst) {
                     break;
                 }
     
-                //print!("{}", String::from_utf8_lossy(&bytes));
-                //io::stdout().flush().expect("Unable to flush stdout");
-
-                self.stream.write_all(&bytes)?;
-                self.stream.flush()?;
+                self.send(&bytes)?;
 
                 bytes = vec![0; 0];
             }
         }
         running.store(false, Ordering::SeqCst);
         
-        self.stream.set_read_timeout(old_read_timeout)?;
+        self.set_recv_timeout(old_recv_timeout)?;
 
         receiver.join().unwrap();
         
         Ok(())
     }
 
 
     fn close(&mut self) -> Result<()> {
-        self.stream.shutdown(std::net::Shutdown::Both)
+        self.stream = None;
+        self.buffer.clear();
+        Ok(())
     }
 }
-
```

### Comparing `rekker-0.1.1/src/pipe/tls.rs` & `rekker-0.1.2/src/pipe/tls.rs`

 * *Files identical despite different names*

### Comparing `rekker-0.1.1/src/req.rs` & `rekker-0.1.2/src/req.rs`

 * *Files identical despite different names*

### Comparing `rekker-0.1.1/Cargo.lock` & `rekker-0.1.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "humantime"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
+
+[[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "itertools"
@@ -386,17 +392,17 @@
 checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -404,49 +410,49 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
@@ -496,19 +502,21 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rekker"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "colored",
  "ctrlc",
+ "humantime",
  "pyo3",
+ "regex",
  "rustls",
  "webpki-roots",
 ]
 
 [[package]]
 name = "ring"
 version = "0.17.8"
```

### Comparing `rekker-0.1.1/PKG-INFO` & `rekker-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rekker
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Attack library written for rust and python
 Keywords: tcp,attack
 Author: GlacierSG <iamglaciersg@gmail.com>
```

