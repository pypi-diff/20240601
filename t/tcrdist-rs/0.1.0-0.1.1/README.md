# Comparing `tmp/tcrdist_rs-0.1.0.tar.gz` & `tmp/tcrdist_rs-0.1.1.tar.gz`

## Comparing `tcrdist_rs-0.1.0.tar` & `tcrdist_rs-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 tcrdist_rs-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     3406 2024-05-01 23:47:44.000000 tcrdist_rs-0.1.0/.github/workflows/release_python.yml
--rw-r--r--   0     1001      127      114 2024-05-01 23:47:44.000000 tcrdist_rs-0.1.0/.gitignore
--rw-r--r--   0     1001      127     1064 2024-05-01 23:47:44.000000 tcrdist_rs-0.1.0/LICENSE
--rw-r--r--   0     1001      127     3839 2024-05-01 23:47:44.000000 tcrdist_rs-0.1.0/README.md
--rw-r--r--   0     1001      127    26855 2024-05-01 23:47:44.000000 tcrdist_rs-0.1.0/src/distance.rs
--rw-r--r--   0     1001      127    41138 2024-05-01 23:47:44.000000 tcrdist_rs-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127   617784 2024-05-01 23:47:44.000000 tcrdist_rs-0.1.0/src/match_table.rs
--rw-r--r--   0     1001      127    10614 2024-05-01 23:47:48.000000 tcrdist_rs-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127      592 2024-05-01 23:47:44.000000 tcrdist_rs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4410 1970-01-01 00:00:00.000000 tcrdist_rs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 tcrdist_rs-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      127     3406 2024-05-31 23:19:04.000000 tcrdist_rs-0.1.1/.github/workflows/release_python.yml
+-rw-r--r--   0     1001      127      114 2024-05-31 23:19:04.000000 tcrdist_rs-0.1.1/.gitignore
+-rw-r--r--   0     1001      127     1064 2024-05-31 23:19:04.000000 tcrdist_rs-0.1.1/LICENSE
+-rw-r--r--   0     1001      127     3822 2024-05-31 23:19:04.000000 tcrdist_rs-0.1.1/README.md
+-rw-r--r--   0     1001      127    30434 2024-05-31 23:19:04.000000 tcrdist_rs-0.1.1/src/distance.rs
+-rw-r--r--   0     1001      127    46514 2024-05-31 23:19:04.000000 tcrdist_rs-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      127   617784 2024-05-31 23:19:04.000000 tcrdist_rs-0.1.1/src/match_table.rs
+-rw-r--r--   0     1001      127    10614 2024-05-31 23:19:09.000000 tcrdist_rs-0.1.1/Cargo.lock
+-rw-r--r--   0     1001      127      592 2024-05-31 23:19:04.000000 tcrdist_rs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4393 1970-01-01 00:00:00.000000 tcrdist_rs-0.1.1/PKG-INFO
```

### Comparing `tcrdist_rs-0.1.0/Cargo.toml` & `tcrdist_rs-0.1.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "tcrdist_rs"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 license = "MIT"
 description = "Rust tcrdist routines, including SMID-accelerated edit distances from triple_accel."
 homepage = "https://github.com/zacmon/tcrdist_rs"
 repository = "https://github.com/zacmon/tcrdist_rs"
 readme = "README.md"
 keywords = ["tcrdist"]
```

### Comparing `tcrdist_rs-0.1.0/.github/workflows/release_python.yml` & `tcrdist_rs-0.1.1/.github/workflows/release_python.yml`

 * *Files identical despite different names*

### Comparing `tcrdist_rs-0.1.0/LICENSE` & `tcrdist_rs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tcrdist_rs-0.1.0/README.md` & `tcrdist_rs-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ```bash
 pip install maturin
 ```
 
 To compile tcrdist, run
 
 ```bash
-maturin develop --release -F py_binds,pyo3 --profile release
+maturin develop --release --profile release
 ```
 
 ## Example
 
 We use the same [settings](https://tcrdist3.readthedocs.io/en/latest/tcrdistances.html#i-want-complete-control) as Python tcrdist. Notably, the keyword `parallel` enables the use of all CPU cores when computing many distances. However, be mindful of enabling it and use it only when there are enough sequences such that the overhead of parallelizing is less costly than the actual computation.
 
 ```python
```

### Comparing `tcrdist_rs-0.1.0/src/distance.rs` & `tcrdist_rs-0.1.1/src/distance.rs`

 * *Files 6% similar despite different names*

```diff
@@ -612,15 +612,15 @@
                         .collect::<Vec<u16>>()
                 })
                 .collect()
         })
     }
 }
 
-/// Compute the full tcrdist between a CDR3-V gene allele array and many others.
+/// Compute the full tcrdist between a CDR3-V gene array and many others.
 pub fn tcrdist_gene_one_to_many(
     seq: [&str; 2],
     seqs: &[[&str; 2]],
     ntrim: usize,
     ctrim: usize,
     parallel: bool,
 ) -> Vec<u16> {
@@ -633,15 +633,15 @@
             seqs.par_iter()
                 .map(|&s| tcrdist_gene(seq, s, ntrim, ctrim))
                 .collect::<Vec<u16>>()
         })
     }
 }
 
-/// Compute the full tcrdist between many CDR3-V gene allele arrays and many others.
+/// Compute the full tcrdist between many CDR3-V gene arrays and many others.
 pub fn tcrdist_gene_many_to_many(
     seqs1: &[[&str; 2]],
     seqs2: &[[&str; 2]],
     ntrim: usize,
     ctrim: usize,
     parallel: bool,
 ) -> Vec<u16> {
@@ -669,14 +669,139 @@
                         .collect::<Vec<u16>>()
                 })
                 .collect()
         })
     }
 }
 
+/// Compute whether two CDR3-V gene arrays are tcrdist-gene neighbors.
+pub fn tcrdist_gene_neighbor(
+    s1: [&str; 2],
+    s2: [&str; 2],
+    threshold: u16,
+    ntrim: usize,
+    ctrim: usize,
+) -> bool {
+    let s1_bytes: &[u8] = s1[0].as_bytes();
+    let s2_bytes: &[u8] = s2[0].as_bytes();
+    let s1_len: usize = s1_bytes.len();
+    let s2_len: usize = s2_bytes.len();
+    let len_diff: u16 = if s1_len > s2_len {
+        (s1_len - s2_len) as u16
+    } else {
+        (s2_len - s1_len) as u16
+    };
+
+    // Gap penalty is 12. Stop computation if lengths are too different.
+    if len_diff * 12 > threshold {
+        return false;
+    }
+
+    // Stop computation if V gene distance and length difference are too different.
+    let v_gene_dist = match_table::gene_distance(s1[1].as_bytes(), s2[1].as_bytes());
+    if v_gene_dist + len_diff > threshold {
+        return false;
+    }
+
+    (v_gene_dist + 3 * tcrdist(s1_bytes, s2_bytes, 1, 4, ntrim, ctrim, false)) <= threshold
+}
+
+pub fn tcrdist_gene_neighbor_matrix(
+    seqs: &[[&str; 2]],
+    threshold: u16,
+    ntrim: usize,
+    ctrim: usize,
+    parallel: bool,
+) -> Vec<bool> {
+    if parallel == false {
+        let seqs_len: usize = seqs.len();
+        let num_combinations: usize = seqs_len * (seqs_len - 1) / 2;
+        let mut dists: Vec<bool> = vec![false; num_combinations];
+        let mut counter: usize = 0;
+
+        for (i, &s1) in seqs.iter().enumerate() {
+            for &s2 in seqs[i + 1..].iter() {
+                dists[counter] = tcrdist_gene_neighbor(s1, s2, threshold, ntrim, ctrim);
+                counter += 1;
+            }
+        }
+
+        dists
+    } else {
+        POOL.install(|| {
+            seqs.par_iter()
+                .enumerate()
+                .flat_map(|(i, &s1)| {
+                    seqs[i + 1..]
+                        .iter()
+                        .map(|&s2| tcrdist_gene_neighbor(s1, s2, threshold, ntrim, ctrim))
+                        .collect::<Vec<bool>>()
+                })
+                .collect()
+        })
+    }
+}
+
+pub fn tcrdist_gene_neighbor_one_to_many(
+    seq: [&str; 2],
+    seqs: &[[&str; 2]],
+    threshold: u16,
+    ntrim: usize,
+    ctrim: usize,
+    parallel: bool,
+) -> Vec<bool> {
+    if parallel == false {
+        seqs.iter()
+            .map(|&s| tcrdist_gene_neighbor(seq, s, threshold, ntrim, ctrim))
+            .collect()
+    } else {
+        POOL.install(|| {
+            seqs.par_iter()
+                .map(|&s| tcrdist_gene_neighbor(seq, s, threshold, ntrim, ctrim))
+                .collect::<Vec<bool>>()
+        })
+    }
+}
+
+pub fn tcrdist_gene_neighbor_many_to_many(
+    seqs1: &[[&str; 2]],
+    seqs2: &[[&str; 2]],
+    threshold: u16,
+    ntrim: usize,
+    ctrim: usize,
+    parallel: bool,
+) -> Vec<bool> {
+    if parallel == false {
+        let seqs1_len: usize = seqs1.len();
+        let seqs2_len: usize = seqs2.len();
+        let mut dists: Vec<bool> = vec![false; seqs1_len * seqs2_len];
+        let mut counter: usize = 0;
+
+        for &s1 in seqs1.iter() {
+            for &s2 in seqs2.iter() {
+                dists[counter] = tcrdist_gene_neighbor(s1, s2, threshold, ntrim, ctrim);
+                counter += 1;
+            }
+        }
+        dists
+    } else {
+        POOL.install(|| {
+            seqs1
+                .par_iter()
+                .flat_map(|&s1| {
+                    seqs2
+                        .iter()
+                        .map(|&s2| tcrdist_gene_neighbor(s1, s2, threshold, ntrim, ctrim))
+                        .collect::<Vec<bool>>()
+                })
+                .collect()
+        })
+    }
+}
+
 /// Compute the Hamming distance matrix on an iterable of strings.
 pub fn hamming_matrix(seqs: &[&str], parallel: bool) -> Vec<u32> {
     if parallel == false {
         let seqs_len: usize = seqs.len();
         let num_combinations: usize = seqs_len * (seqs_len - 1) / 2;
         let mut dists: Vec<u32> = vec![0; num_combinations];
         let mut counter: usize = 0;
```

### Comparing `tcrdist_rs-0.1.0/src/lib.rs` & `tcrdist_rs-0.1.1/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 //! # tcrdist_rs
 //!
 //! A library for computing the distances between immune cell receptors.
 mod distance;
 mod match_table;
-
 use crate::distance as _distance;
 
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 use pyo3::prelude::*;
 use triple_accel;
 
 pub use match_table::{
     amino_distances, cdr1_distances, cdr2_distances, gene_distance, phmc_distances,
 };
 
@@ -32,15 +31,15 @@
 ///     The Hamming distance between the two strings.
 ///
 /// Examples
 /// --------
 /// >>> s1 = "abcdefg"
 /// >>> s2 = "abddefg"
 /// >>> assert(hamming(s1, s2) == 1)
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
 fn hamming(s1: &str, s2: &str) -> PyResult<u32> {
     Ok(triple_accel::hamming(&s1.as_bytes(), &s2.as_bytes()))
 }
 
 /// Compute the Hamming distance matrix on an iterable of strings.
 ///
@@ -59,16 +58,17 @@
 /// list of int
 ///     The Hamming distances among the strings.
 ///
 /// Examples
 /// --------
 /// >>> seqs = ["abc", "abd", "fcd"]
 /// >>> assert(hamming_matrix(seqs, parallel=False) == [1, 3, 2])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seqs, parallel=false))]
 fn hamming_matrix(seqs: Vec<&str>, parallel: bool) -> PyResult<Vec<u32>> {
     Ok(_distance::hamming_matrix(&seqs, parallel))
 }
 
 /// Compute the Hamming distance between one string and many others.
 ///
 /// The strings being compared must have equal lengths or the program will terminate.
@@ -76,29 +76,30 @@
 ///
 /// Parameters
 /// ----------
 /// seq : str
 ///     The string against which all others will be compared.
 /// seqs : iterable of str
 ///     The other strings being compared.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The Hamming distances among the strings.
 ///
 /// Examples
 /// --------
 /// >>> seq = "abb"
 /// >>> seqs = ["abc", "abd", "fcd"]
 /// >>> assert(hamming_one_to_many(seq, seqs, parallel=False) == [1, 1, 3])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seq, seqs, parallel=false))]
 fn hamming_one_to_many(seq: &str, seqs: Vec<&str>, parallel: bool) -> PyResult<Vec<u32>> {
     Ok(_distance::hamming_one_to_many(&seq, &seqs, parallel))
 }
 
 /// Compute the Hamming distance between many strings and many others.
 ///
 /// The strings being compared must have equal lengths or the program will terminate.
@@ -106,29 +107,30 @@
 ///
 /// Parameters
 /// ----------
 /// seqs1 : iterable of str
 ///     The first iterable of strings.
 /// seqs2 : iterable of str
 ///     The other iterable of strings.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The Hamming distances among the strings.
 ///
 /// Examples
 /// --------
 /// >>> seqs1 = ["abb", "abc"]
 /// >>> seqs2 = ["abc", "abd", "fcd"]
 /// >>> assert(hamming_many_to_many(seqs1, seqs2, parallel=False) == [1, 1, 3, 0, 1, 3])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seqs1, seqs2, parallel=false))]
 fn hamming_many_to_many(seqs1: Vec<&str>, seqs2: Vec<&str>, parallel: bool) -> PyResult<Vec<u32>> {
     Ok(_distance::hamming_many_to_many(&seqs1, &seqs2, parallel))
 }
 
 /// Compute the Levenshtein distance between two strings.
 ///
 /// The strings must be representable as byte strings.
@@ -146,43 +148,44 @@
 ///     The Levenshtein distance between the two strings.
 ///
 /// Examples
 /// --------
 /// >>> s1 = "abcdefg"
 /// >>> s2 = "abdcd defgggg"
 /// >>> assert(levenshtein(s1, s2) == 6)
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
 fn levenshtein(s1: &str, s2: &str) -> PyResult<u32> {
     Ok(triple_accel::levenshtein(&s1.as_bytes(), &s2.as_bytes()))
 }
 
 /// Compute the Levenshtein distance matrix on an iterable of strings.
 ///
 /// The strings must be representable as byte strings.
 ///
 /// Parameters
 /// ----------
 /// seqs : iterable str
 ///     The strings to be compared. The must have an appropriate representation
 ///     as byte strings.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The Levenshtein distances among the strings.
 ///
 /// Examples
 /// --------
 /// >>> seqs = ["Monday", "Tuesday", "Wednesday", "Thursday"]
 /// >>> assert(levenshtein_matrix(seqs, parallel=False) == [4, 5, 5, 4, 2, 5])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seqs, parallel=false))]
 fn levenshtein_matrix(seqs: Vec<&str>, parallel: bool) -> PyResult<Vec<u32>> {
     Ok(_distance::levenshtein_matrix(&seqs, parallel))
 }
 
 /// Compute the Levenshtein distance between one string and many others.
 ///
 /// This returns the upper right triangle of the distance matrix.
@@ -190,58 +193,60 @@
 ///
 /// Parameters
 /// ----------
 /// seq : str
 ///     The string against which all others will be compared.
 /// seqs : iterable of str
 ///     The other strings being compared.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The Levenshtein distances among the strings.
 ///
 /// Examples
 /// --------
 /// >>> seq = "Sunday"
 /// >>> seqs = ["Monday", "Tuesday", "Wednesday", "Thursday"]
 /// >>> assert(levenshtein_one_to_many(seq, seqs, parallel=False) == [2, 3, 5, 4])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seq, seqs, parallel=false))]
 fn levenshtein_one_to_many(seq: &str, seqs: Vec<&str>, parallel: bool) -> PyResult<Vec<u32>> {
     Ok(_distance::levenshtein_one_to_many(&seq, &seqs, parallel))
 }
 
 /// Compute the Levenshtein distance between many strings and many others.
 ///
 /// The strings must be representable as byte strings.
 ///
 /// Parameters
 /// ----------
 /// seqs1 : iterable of str
 ///     The first iterable of strings.
 /// seqs : iterable of str
 ///     The second iterable of strings.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The Levenshtein distances among the strings.
 ///
 /// Examples
 /// --------
 /// >>> seqs1 = ["Sunday", "Saturday"]
 /// >>> seqs2 = ["Monday", "Tuesday", "Wednesday"]
 /// >>> assert(levenshtein_many_to_many(seqs1, seqs2, parallel=False) == [2, 3, 5, 5, 5, 6])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seqs1, seqs2, parallel=false))]
 fn levenshtein_many_to_many(
     seqs1: Vec<&str>,
     seqs2: Vec<&str>,
     parallel: bool,
 ) -> PyResult<Vec<u32>> {
     Ok(_distance::levenshtein_many_to_many(
         &seqs1, &seqs2, parallel,
@@ -267,15 +272,15 @@
 ///     The Levenshtein distance between the two strings.
 ///
 /// Examples
 /// --------
 /// >>> s1 = "abcdefg"
 /// >>> s2 = "abdcd defgggg"
 /// >>> assert(levenshtein_exp(s1, s2) == 6)
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
 fn levenshtein_exp(s1: &str, s2: &str) -> PyResult<u32> {
     Ok(triple_accel::levenshtein_exp(
         &s1.as_bytes(),
         &s2.as_bytes(),
     ))
 }
@@ -287,28 +292,29 @@
 /// levenshtein_exp_matrix when the number of edits is small.
 ///
 /// Parameters
 /// ----------
 /// seqs : iterable str
 ///     The strings to be compared. The must have an appropriate representation
 ///     as byte strings.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The Levenshtein distances among the strings.
 ///
 /// Examples
 /// --------
 /// >>> seqs = ["Monday", "Tuesday", "Wednesday", "Thursday"]
 /// >>> assert(levenshtein_exp_matrix(seqs, parallel=False) == [4, 5, 5, 4, 2, 5])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seqs, parallel=false))]
 fn levenshtein_exp_matrix(seqs: Vec<&str>, parallel: bool) -> PyResult<Vec<u32>> {
     Ok(_distance::levenshtein_exp_matrix(&seqs, parallel))
 }
 
 /// Compute the Levenshtein distance between one string and many others using exponential search.
 ///
 /// This returns the upper right triangle of the distance matrix.
@@ -318,29 +324,30 @@
 ///
 /// Parameters
 /// ----------
 /// seq : str
 ///     The string against which all others will be compared.
 /// seqs : iterable of str
 ///     The other strings being compared.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The Levenshtein distances among the strings.
 ///
 /// Examples
 /// --------
 /// >>> seq = "Sunday"
 /// >>> seqs = ["Monday", "Tuesday", "Wednesday", "Thursday"]
 /// >>> assert(levenshtein_one_to_many(seq, seqs, parallel=False) == [2, 3, 5, 4])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seq, seqs, parallel=false))]
 fn levenshtein_exp_one_to_many(seq: &str, seqs: Vec<&str>, parallel: bool) -> PyResult<Vec<u32>> {
     Ok(_distance::levenshtein_exp_one_to_many(
         &seq, &seqs, parallel,
     ))
 }
 
 /// Compute the Levenshtein distance between many strings and many others.
@@ -351,29 +358,30 @@
 ///
 /// Parameters
 /// ----------
 /// seqs1 : iterable of str
 ///     The first iterable of strings.
 /// seqs : iterable of str
 ///     The second iterable of strings.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The Levenshtein distances among the strings.
 ///
 /// Examples
 /// --------
 /// >>> seqs1 = ["Sunday", "Saturday"]
 /// >>> seqs2 = ["Monday", "Tuesday", "Wednesday"]
 /// >>> assert(levenshtein_many_to_many(seqs1, seqs2, parallel=False) == [2, 3, 5, 5, 5, 6])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seqs1, seqs2, parallel=false))]
 fn levenshtein_exp_many_to_many(
     seqs1: Vec<&str>,
     seqs2: Vec<&str>,
     parallel: bool,
 ) -> PyResult<Vec<u32>> {
     Ok(_distance::levenshtein_exp_many_to_many(
         &seqs1, &seqs2, parallel,
@@ -398,15 +406,15 @@
 ///     The distance between the two residues.
 ///
 /// Examples
 /// --------
 /// >>> s1 = "C"
 /// >>> s2 = "a"
 /// >>> assert(amino_acid_distance(s1, s2) == 4)
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
 fn amino_acid_distance(s1: &str, s2: &str) -> PyResult<u16> {
     Ok(amino_distances(&s1.as_bytes()[0], &s2.as_bytes()[0]))
 }
 
 /// Compute the distance between V genes using precomputed tcrdists.
 ///
@@ -423,15 +431,15 @@
 ///     The distance between two V genes.
 ///
 /// Examples
 /// --------
 /// >>> s1 = "C"
 /// >>> s2 = "a"
 /// >>> assert(amino_acid_distance(s1, s2) == 4)
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
 fn v_gene_distance(s1: &str, s2: &str) -> PyResult<u16> {
     Ok(gene_distance(&s1.as_bytes(), &s2.as_bytes()))
 }
 
 /// Compute the pMHC distance between V alleles using precomputed tcrdists.
 ///
@@ -451,15 +459,15 @@
 ///     The distance between the V alleles' pMHCs.
 ///
 /// Examples
 /// --------
 /// s1 = "TRBV2*01"
 /// s2 = "TRBV6-2*01"
 /// assert(phmc_distance(s1, s2) == 16)
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
 fn phmc_distance(s1: &str, s2: &str) -> PyResult<u16> {
     Ok(phmc_distances(s1.as_bytes(), s2.as_bytes()))
 }
 
 /// Compute the CDR1 distance between V alleles using precomputed tcrdists.
 ///
@@ -479,15 +487,15 @@
 ///     The distance between the V alleles' CDR1s.
 ///
 /// Examples
 /// --------
 /// s1 = "TRBV2*01"
 /// s2 = "TRBV6-2*01"
 /// assert(cdr1_distance(s1, s2) == 8)
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
 fn cdr1_distance(s1: &str, s2: &str) -> PyResult<u16> {
     Ok(cdr1_distances(s1.as_bytes(), s2.as_bytes()))
 }
 
 /// Compute the CDR2 distance between V alleles using precomputed tcrdists.
 ///
@@ -507,15 +515,15 @@
 ///     The distance between the V alleles' CDR2s.
 ///
 /// Examples
 /// --------
 /// >>> s1 = "TRBV2*01"
 /// >>> s2 = "TRBV6-2*01"
 /// >>> assert(cdr2_distance(s1, s2) == 24)
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
 fn cdr2_distance(s1: &str, s2: &str) -> PyResult<u16> {
     Ok(cdr2_distances(s1.as_bytes(), s2.as_bytes()))
 }
 
 /// Compute the tcrdist between two strings.
 ///
@@ -523,26 +531,26 @@
 ///
 /// Parameters
 /// ----------
 /// s1 : str
 ///     A string. Ideally, this should be a string of amino acid residues.
 /// s2 : str
 ///     A string. Ideally, this should be a string of amino acid residues.
-/// dist_weight : int
+/// dist_weight : int, default 1
 ///     A weight applied to the mismatch distances. This weight is not applied
 ///     to the gap penalties.
-/// gap_penalty : int
+/// gap_penalty : int, default 4
 ///     The penalty given to the difference in length of the strings.
-/// ntrim : int
+/// ntrim : int, default 3
 ///     The position at which the distance calculation will begin.
 ///     This parameter must be >= 0.
-/// ctrim : int
+/// ctrim : int, default 2
 ///     The position, counted from the end, at which the calculation will end.
 ///     This parameter must be >= 0.
-/// fixed_gappos : bool
+/// fixed_gappos : bool, default False
 ///     If True, insert gaps at a fixed position after the cysteine residue
 ///     starting the CDR3 (typically position 6). If False, find the "optimal"
 ///     position for inserting the gaps to make up the difference in length.
 ///
 /// Returns
 /// -------
 /// int
@@ -555,16 +563,17 @@
 /// >>> dist_weight = 1
 /// >>> gap_penalty = 4
 /// >>> ntrim = 3
 /// >>> ctrim = 2
 /// >>> fixed_gappos = False
 /// >>> dist = tcrdist(s1, s2, dist_weight, gap_penalty, ntrim, ctrim, fixed_gappos)
 /// >>> assert(dist == 40)
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (s1, s2, dist_weight=1, gap_penalty=4, ntrim=3, ctrim=2, fixed_gappos=false))]
 fn tcrdist(
     s1: &str,
     s2: &str,
     dist_weight: u16,
     gap_penalty: u16,
     ntrim: usize,
     ctrim: usize,
@@ -585,30 +594,30 @@
 ///
 /// The strings must be representable as byte strings.
 ///
 /// Parameters
 /// ----------
 /// seqs : iterable of str
 ///     Iterable of strings.
-/// dist_weight : int
+/// dist_weight : int, default 1
 ///     A weight applied to the mismatch distances. This weight is not applied
 ///     to the gap penalties.
-/// gap_penalty : int
+/// gap_penalty : int, default 4
 ///     The penalty given to the difference in length of the strings.
-/// ntrim : int
+/// ntrim : int, default 3
 ///     The position at which the distance calculation will begin.
 ///     This parameter must be >= 0.
-/// ctrim : int
+/// ctrim : int, default 2
 ///     The position, counted from the end, at which the calculation will end.
 ///     This parameter must be >= 0.
-/// fixed_gappos : bool
+/// fixed_gappos : bool, default False
 ///     If True, insert gaps at a fixed position after the cysteine residue
 ///     starting the CDR3 (typically position 6). If False, find the "optimal"
 ///     position for inserting the gaps to make up the difference in length.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The tcrdists among the strings.
 ///
@@ -619,16 +628,17 @@
 /// >>> gap_penalty = 4
 /// >>> ntrim = 3
 /// >>> ctrim = 2
 /// >>> fixed_gappos = False
 /// >>> dist = tcrdist_matrix(seqs, dist_weight, gap_penalty, ntrim, ctrim, fixed_gappos,
 /// parallel=False)
 /// >>> assert(dist == [40, 28, 28, 40, 40, 19])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seqs, dist_weight=1, gap_penalty=4, ntrim=3, ctrim=2, fixed_gappos=false, parallel=false))]
 fn tcrdist_matrix(
     seqs: Vec<&str>,
     dist_weight: u16,
     gap_penalty: u16,
     ntrim: usize,
     ctrim: usize,
     fixed_gappos: bool,
@@ -652,30 +662,30 @@
 ///
 /// Parameters
 /// ----------
 /// seq : str
 ///     The string against which all others will be compared.
 /// seqs : str
 ///     The other strings being compared.
-/// dist_weight : int
+/// dist_weight : int, default 1
 ///     A weight applied to the mismatch distances. This weight is not applied
 ///     to the gap penalties.
-/// gap_penalty : int
+/// gap_penalty : int, default 4
 ///     The penalty given to the difference in length of the strings.
-/// ntrim : int
+/// ntrim : int, default 3
 ///     The position at which the distance calculation will begin.
 ///     This parameter must be >= 0.
-/// ctrim : int
+/// ctrim : int, default 2
 ///     The position, counted from the end, at which the calculation will end.
 ///     This parameter must be >= 0.
-/// fixed_gappos : bool
+/// fixed_gappos : bool, default False
 ///     If True, insert gaps at a fixed position after the cysteine residue
 ///     starting the CDR3 (typically position 6). If False, find the "optimal"
 ///     position for inserting the gaps to make up the difference in length.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The tcrdists among the strings.
 ///
@@ -687,16 +697,17 @@
 /// >>> gap_penalty = 4
 /// >>> ntrim = 3
 /// >>> ctrim = 2
 /// >>> fixed_gappos = False
 /// >>> dist = tcrdist_one_to_many(seq, seqs, dist_weight, gap_penalty, ntrim, ctrim, fixed_gappos,
 /// parallel=False)
 /// >>> assert(dist == [52, 41, 52, 48])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seq, seqs, dist_weight=1, gap_penalty=4, ntrim=3, ctrim=2, fixed_gappos=false, parallel=false))]
 fn tcrdist_one_to_many(
     seq: &str,
     seqs: Vec<&str>,
     dist_weight: u16,
     gap_penalty: u16,
     ntrim: usize,
     ctrim: usize,
@@ -721,30 +732,30 @@
 ///
 /// Parameters
 /// ----------
 /// seqs1 : iterable of str
 ///     The first iterable of strings.
 /// seqs2 : iterable of str
 ///     The other iterable of strings.
-/// dist_weight : int
+/// dist_weight : int, default 1
 ///     A weight applied to the mismatch distances. This weight is not applied
 ///     to the gap penalties.
-/// gap_penalty : int
+/// gap_penalty : int, default 4
 ///     The penalty given to the difference in length of the strings.
-/// ntrim : int
+/// ntrim : int, default 3
 ///     The position at which the distance calculation will begin.
 ///     This parameter must be >= 0.
-/// ctrim : int
+/// ctrim : int, default 2
 ///     The position, counted from the end, at which the calculation will end.
 ///     This parameter must be >= 0.
-/// fixed_gappos : bool
+/// fixed_gappos : bool, default False
 ///     If True, insert gaps at a fixed position after the cysteine residue
 ///     starting the CDR3 (typically position 6). If False, find the "optimal"
 ///     position for inserting the gaps to make up the difference in length.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The tcrdists among the strings.
 ///
@@ -755,16 +766,17 @@
 /// >>> dist_weight = 1
 /// >>> gap_penalty = 4
 /// >>> ntrim = 3
 /// >>> ctrim = 2
 /// >>> fixed_gappos = False
 /// >>> dist = tcrdist_many_to_many(seqs1, seqs2, dist_weight, gap_penalty, ntrim, ctrim, fixed_gappos, parallel=False)
 /// >>> assert(dist == [52, 41, 52, 48])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seqs1, seqs2, dist_weight=1, gap_penalty=4, ntrim=3, ctrim=2, fixed_gappos=false, parallel=false))]
 fn tcrdist_many_to_many(
     seqs1: Vec<&str>,
     seqs2: Vec<&str>,
     dist_weight: u16,
     gap_penalty: u16,
     ntrim: usize,
     ctrim: usize,
@@ -778,41 +790,42 @@
         gap_penalty,
         ntrim,
         ctrim,
         fixed_gappos,
         parallel,
     ))
 }
+
 /// Compute the tcrdist between two CDR3-V allele pairs.
 ///
 /// This incorporates differences between the pMHC, CDR1, CDR2, and CDR3.
 ///
 /// Parameters
 /// ----------
 /// s1 : iterable of str
 ///     An iterable of the CDR3 amino acid sequence and V allele.
 /// s2 : iterable of str
 ///     An iterable of the CDR3 amino acid sequence and V allele.
-/// phmc_weight : int
+/// phmc_weight : int, default 1
 ///     How much the difference in pMHCs contributes to the distance.
-/// cdr1_weight : int
+/// cdr1_weight : int, default 1
 ///     How much the difference in CDR1s contributes to the distance.
-/// cdr2_weight : int
+/// cdr2_weight : int, default 1
 ///     How much the difference in CDR2s contributes to the distance.
-/// cdr3_weight : int
+/// cdr3_weight : int, default 3
 ///     How much the difference in CDR3s contributes to the distance.
-/// gap_penalty : int
+/// gap_penalty : int, default 4
 ///     The penalty given to the difference in length of the strings.
-/// ntrim : int
+/// ntrim : int, default 3
 ///     The position at which the distance calculation will begin.
 ///     This parameter must be >= 0.
-/// ctrim : int
+/// ctrim : int, default 2
 ///     The position, counted from the end, at which the calculation will end.
 ///     This parameter must be >= 0.
-/// fixed_gappos : bool
+/// fixed_gappos : bool, default False
 ///     If True, insert gaps at a fixed position after the cysteine residue
 ///     starting the CDR3 (typically position 6). If False, find the "optimal"
 ///     position for inserting the gaps to make up the difference in length.
 ///
 /// Returns
 /// -------
 /// int
@@ -828,16 +841,17 @@
 /// >>> cdr3_weight = 3
 /// >>> gap_penalty = 4
 /// >>> ntrim = 3
 /// >>> ctrim = 2
 /// >>> fixed_gappos = False
 /// >>> dist = tcrdist_allele(s1, s2, phmc_weight, cdr1_weight, cdr2_weight, cdr3_weight, gap_penalty, ntrim, ctrim, fixed_gappos)
 /// >>> assert(dist == 168)
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (s1, s2, phmc_weight=1, cdr1_weight=1, cdr2_weight=1, cdr3_weight=3, gap_penalty=4, ntrim=3, ctrim=2, fixed_gappos=false))]
 fn tcrdist_allele(
     s1: [&str; 2],
     s2: [&str; 2],
     phmc_weight: u16,
     cdr1_weight: u16,
     cdr2_weight: u16,
     cdr3_weight: u16,
@@ -865,35 +879,35 @@
 /// This returns the upper right triangle of the distance matrix.
 /// This incorporates differences between the pMHC, CDR1, CDR2, and CDR3.
 ///
 /// Parameters
 /// ----------
 /// seqs : iterable of iterable of str
 ///     An iterable containing iterables of CDR3 amino acid sequences and V alleles.
-/// phmc_weight : int
+/// phmc_weight : int, default 1
 ///     How much the difference in pMHCs contributes to the distance.
-/// cdr1_weight : int
+/// cdr1_weight : int, default 1
 ///     How much the difference in CDR1s contributes to the distance.
-/// cdr2_weight : int
+/// cdr2_weight : int, default 1
 ///     How much the difference in CDR2s contributes to the distance.
-/// cdr3_weight : int
+/// cdr3_weight : int, default 3
 ///     How much the difference in CDR3s contributes to the distance.
-/// gap_penalty : int
+/// gap_penalty : int, default 4
 ///     The penalty given to the difference in length of the strings.
-/// ntrim : int
+/// ntrim : int, default 3
 ///     The position at which the distance calculation will begin.
 ///     This parameter must be >= 0.
-/// ctrim : int
+/// ctrim : int, default 2
 ///     The position, counted from the end, at which the calculation will end.
 ///     This parameter must be >= 0.
-/// fixed_gappos : bool
+/// fixed_gappos : bool, default False
 ///     If True, insert gaps at a fixed position after the cysteine residue
 ///     starting the CDR3 (typically position 6). If False, find the "optimal"
 ///     position for inserting the gaps to make up the difference in length.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The tcrdists among the CDR3-V allele pairs.
 ///
@@ -906,16 +920,17 @@
 /// >>> cdr3_weight = 3
 /// >>> gap_penalty = 4
 /// >>> ntrim = 3
 /// >>> ctrim = 2
 /// >>> fixed_gappos = False
 /// >>> dist = tcrdist_allele_matrix(seqs, phmc_weight, cdr1_weight, cdr2_weight, cdr3_weight, gap_penalty, ntrim, ctrim, fixed_gappos, parallel=False)
 /// >>> assert(dist == [168, 142, 134, 203, 163, 169, 148, 116, 189, 198])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seqs, phmc_weight=1, cdr1_weight=1, cdr2_weight=1, cdr3_weight=3, gap_penalty=4, ntrim=3, ctrim=2, fixed_gappos=false, parallel=false))]
 fn tcrdist_allele_matrix(
     seqs: Vec<[&str; 2]>,
     phmc_weight: u16,
     cdr1_weight: u16,
     cdr2_weight: u16,
     cdr3_weight: u16,
     gap_penalty: u16,
@@ -944,34 +959,36 @@
 ///
 /// Parameters
 /// ----------
 /// s1 : iterable of str
 ///     An iterable containing a CDR3 amino acid sequence and V allele.
 /// seqs : iterable of iterable of str
 ///     An iterable of iterables containing pairs of CDR3 amino acid sequences and V alleles.
-/// phmc_weight : int
+/// phmc_weight : int, default 1
 ///     How much the difference in pMHCs contributes to the distance.
-/// cdr1_weight : int
+/// cdr1_weight : int, default 1
 ///     How much the difference in CDR1s contributes to the distance.
-/// cdr2_weight : int
+/// cdr2_weight : int, default 1
 ///     How much the difference in CDR2s contributes to the distance.
-/// cdr3_weight : int
+/// cdr3_weight : int, default 3
 ///     How much the difference in CDR3s contributes to the distance.
-/// gap_penalty : int
+/// gap_penalty : int, default 4
 ///     The penalty given to the difference in length of the strings.
-/// ntrim : int
+/// ntrim : int, default 3
 ///     The position at which the distance calculation will begin.
 ///     This parameter must be >= 0.
-/// ctrim : int
+/// ctrim : int, default 2
 ///     The position, counted from the end, at which the calculation will end.
 ///     This parameter must be >= 0.
-/// fixed_gappos : bool
+/// fixed_gappos : bool, False
 ///     If True, insert gaps at a fixed position after the cysteine residue
 ///     starting the CDR3 (typically position 6). If False, find the "optimal"
 ///     position for inserting the gaps to make up the difference in length.
+/// parallel: bool, default False
+///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The tcrdists among the CDR3-V allele sequences.
 ///
 /// Examples
@@ -984,16 +1001,17 @@
 /// >>> cdr3_weight = 3
 /// >>> gap_penalty = 4
 /// >>> ntrim = 3
 /// >>> ctrim = 2
 /// >>> fixed_gappos = False
 /// >>> dist = tcrdist_allele_one_to_many(seq, seqs, phmc_weight, cdr1_weight, cdr2_weight, cdr3_weight, gap_penalty, ntrim, ctrim, fixed_gappos, parallel=False)
 /// >>> assert(dist == [168, 142, 134, 203])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seq, seqs, phmc_weight=1, cdr1_weight=1, cdr2_weight=1, cdr3_weight=3, gap_penalty=4, ntrim=3, ctrim=2, fixed_gappos=false, parallel=false))]
 fn tcrdist_allele_one_to_many(
     seq: [&str; 2],
     seqs: Vec<[&str; 2]>,
     phmc_weight: u16,
     cdr1_weight: u16,
     cdr2_weight: u16,
     cdr3_weight: u16,
@@ -1024,35 +1042,35 @@
 ///
 /// Parameters
 /// ----------
 /// seqs1 : iterable of iterable of str
 ///     An iterable of iterables containing pairs of CDR3 amino acid sequences and V alleles.
 /// seqs2 : iterable of iterable of str
 ///     An iterable of iterables containing pairs of CDR3 amino acid sequences and V alleles.
-/// phmc_weight : int
+/// phmc_weight : int, default 1
 ///     How much the difference in pMHCs contributes to the distance.
-/// cdr1_weight : int
+/// cdr1_weight : int, default 1
 ///     How much the difference in CDR1s contributes to the distance.
-/// cdr2_weight : int
+/// cdr2_weight : int, default 1
 ///     How much the difference in CDR2s contributes to the distance.
-/// cdr3_weight : int
+/// cdr3_weight : int, default 3
 ///     How much the difference in CDR3s contributes to the distance.
-/// gap_penalty : int
+/// gap_penalty : int, default 4
 ///     The penalty given to the difference in length of the strings.
-/// ntrim : int
+/// ntrim : int, default 3
 ///     The position at which the distance calculation will begin.
 ///     This parameter must be >= 0.
-/// ctrim : int
+/// ctrim : int, default 2
 ///     The position, counted from the end, at which the calculation will end.
 ///     This parameter must be >= 0.
-/// fixed_gappos : bool
+/// fixed_gappos : bool, False
 ///     If True, insert gaps at a fixed position after the cysteine residue
 ///     starting the CDR3 (typically position 6). If False, find the "optimal"
 ///     position for inserting the gaps to make up the difference in length.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The tcrdists among the CDR3-V allele pairs.
 ///
@@ -1066,16 +1084,17 @@
 /// >>> cdr3_weight = 3
 /// >>> gap_penalty = 4
 /// >>> ntrim = 3
 /// >>> ctrim = 2
 /// >>> fixed_gappos = False
 /// >>> dist = tcrdist_allele_many_to_many(seqs1, seqs2, phmc_weight, cdr1_weight, cdr2_weight, cdr3_weight, gap_penalty, ntrim, ctrim, fixed_gappos, parallel=False)
 /// >>> assert(dist == [168, 142, 134, 203, 104, 125, 143, 121])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seqs1, seqs2, phmc_weight=1, cdr1_weight=1, cdr2_weight=1, cdr3_weight=3, gap_penalty=4, ntrim=3, ctrim=2, fixed_gappos=false, parallel=false))]
 fn tcrdist_allele_many_to_many(
     seqs1: Vec<[&str; 2]>,
     seqs2: Vec<[&str; 2]>,
     phmc_weight: u16,
     cdr1_weight: u16,
     cdr2_weight: u16,
     cdr3_weight: u16,
@@ -1104,71 +1123,73 @@
 ///
 /// Parameters
 /// ----------
 /// s1 : iterable of str
 ///     An iterable containing a CDR3 amino acid sequence and V gene pair.
 /// s2 : iterable of str
 ///     An iterable containing a CDR3 amino acid sequence and V gene pair.
-/// ntrim : int
+/// ntrim : int, default 3
 ///     The position at which the distance calculation will begin.
 ///     This parameter must be >= 0.
-/// ctrim : int
+/// ctrim : int, default 2
 ///     The position, counted from the end, at which the calculation will end.
 ///     This parameter must be >= 0.
 ///
 /// Returns
 /// -------
 /// int
 ///     The tcrdist between two CDR3-V gene pairs.
 ///
 /// Examples
 /// --------
-/// >>> s1 = ["CASRTGTVYEQYF", "TRBV2*01"]
-/// >>> s2 = ["CASSTLDRVYNSPLHF", "TRBV6-2*01"]
+/// >>> s1 = ["CASRTGTVYEQYF", "TRBV2"]
+/// >>> s2 = ["CASSTLDRVYNSPLHF", "TRBV6-2"]
 /// >>> ntrim = 3
 /// >>> ctrim = 2
 /// >>> dist = tcrdist_gene(s1, s2, ntrim, ctrim)
 /// >>> assert(dist == 168)
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (s1, s2, ntrim=3, ctrim=2))]
 fn tcrdist_gene(s1: [&str; 2], s2: [&str; 2], ntrim: usize, ctrim: usize) -> PyResult<u16> {
     Ok(_distance::tcrdist_gene(s1, s2, ntrim, ctrim))
 }
 
 /// Compute the tcrdist matrix on an iterable of CDR3-V gene pairs.
 ///
 /// This returns the upper right triangle of the distance matrix.
 ///
 /// Parameters
 /// ----------
 /// seqs : iterable of iterable of str
 ///     An iterable containing iterables of CDR3 amino acid sequence and V gene pairs.
-/// ntrim : int
+/// ntrim : int, default 3
 ///     The position at which the distance calculation will begin.
 ///     This parameter must be >= 0.
-/// ctrim : int
+/// ctrim : int, default 2
 ///     The position, counted from the end, at which the calculation will end.
 ///     This parameter must be >= 0.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The tcrdist among the CDR3-V gene pairs.
 ///
 /// Examples
 /// --------
 /// >>> seqs = [["CASRTGTVYEQYF", "TRBV2"], ["CASSTLDRVYNSPLHF", "TRBV6-2"], ["CASSESGGQVDTQYF", "TRBV6-4"], ["CASSPTGPTDTQYF", "TRBV18"], ["CASSYPIEGGRAFTGELFF", "TRBV6-5"]]
 /// >>> ntrim = 3
 /// >>> ctrim = 2
 /// >>> dist = tcrdist_gene_matrix(seqs, ntrim, ctrim, parallel=False)
 /// >>> assert(dist == [168, 142, 134, 203, 163, 169, 148, 116, 189, 198])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seqs, ntrim=3, ctrim=2, parallel=false))]
 fn tcrdist_gene_matrix(
     seqs: Vec<[&str; 2]>,
     ntrim: usize,
     ctrim: usize,
     parallel: bool,
 ) -> PyResult<Vec<u16>> {
     Ok(_distance::tcrdist_gene_matrix(
@@ -1180,21 +1201,21 @@
 ///
 /// Parameters
 /// ----------
 /// seq : iterable of str
 ///     An iterable containing a CDR3 amino acid sequence and V allele pair.
 /// seqs : iterable of iterable of str
 ///     An iterable containing iterables of CDR3 amino acid sequence and V gene pairs.
-/// ntrim : int
+/// ntrim : int, default 3
 ///     The position at which the distance calculation will begin.
 ///     This parameter must be >= 0.
-/// ctrim : int
+/// ctrim : int, default 2
 ///     The position, counted from the end, at which the calculation will end.
 ///     This parameter must be >= 0.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The tcrdists among the CDR3-V gene pairs.
 ///
@@ -1202,16 +1223,17 @@
 /// --------
 /// >>> seq = ["CASRTGTVYEQYF", "TRBV2"]
 /// >>> seqs = [["CASSTLDRVYNSPLHF", "TRBV6-2"], ["CASSESGGQVDTQYF", "TRBV6-4"], ["CASSPTGPTDTQYF", "TRBV18"], ["CASSYPIEGGRAFTGELFF", "TRBV6-5"]]
 /// >>> ntrim = 3
 /// >>> ctrim = 2
 /// >>> dist = tcrdist_gene_one_to_many(seq, seqs, ntrim, ctrim, parallel=False)
 /// >>> assert(dist == [168, 142, 134, 203])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seq, seqs, ntrim=3, ctrim=2, parallel=false))]
 fn tcrdist_gene_one_to_many(
     seq: [&str; 2],
     seqs: Vec<[&str; 2]>,
     ntrim: usize,
     ctrim: usize,
     parallel: bool,
 ) -> PyResult<Vec<u16>> {
@@ -1224,21 +1246,21 @@
 ///
 /// Parameters
 /// ----------
 /// seqs1 : iterable of iterable of str
 ///     An iterable containing iterables of CDR3 amino acid sequence and V gene pairs.
 /// seqs2 : iterable of iterable of str
 ///     An iterable containing iterables of CDR3 amino acid sequence and V gene pairs.
-/// ntrim : int
+/// ntrim : int, default 3
 ///     The position at which the distance calculation will begin.
 ///     This parameter must be >= 0.
-/// ctrim : int
+/// ctrim : int, default 2
 ///     The position, counted from the end, at which the calculation will end.
 ///     This parameter must be >= 0.
-/// parallel: bool
+/// parallel: bool, default False
 ///     Bool to specify if computation should be parallelized.
 ///
 /// Returns
 /// -------
 /// list of int
 ///     The tcrdists among the CDR3-V gene pairs.
 ///
@@ -1246,29 +1268,129 @@
 /// --------
 /// >>> seqs1 = [["CASRTGTVYEQYF", "TRBV2"], ["CASSYSEEPSSPLHF", "TRBV6-6"]]
 /// >>> seqs2 = [["CASSTLDRVYNSPLHF", "TRBV6-2"], ["CASSESGGQVDTQYF", "TRBV6-4"], ["CASSPTGPTDTQYF", "TRBV18"], ["CASSYPIEGGRAFTGELFF", "TRBV6-5"]]
 /// >>> ntrim = 3
 /// >>> ctrim = 2
 /// >>> dist = tcrdist_gene_many_to_many(seqs1, seqs2, ntrim, ctrim, parallel=False)
 /// >>> assert(dist == [168, 142, 134, 203, 104, 125, 143, 121])
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+#[cfg(all(feature = "pyo3"))]
 #[pyfunction]
+#[pyo3(signature = (seqs1, seqs2, ntrim=3, ctrim=2, parallel=false))]
 fn tcrdist_gene_many_to_many(
     seqs1: Vec<[&str; 2]>,
     seqs2: Vec<[&str; 2]>,
     ntrim: usize,
     ctrim: usize,
     parallel: bool,
 ) -> PyResult<Vec<u16>> {
     Ok(_distance::tcrdist_gene_many_to_many(
         &seqs1, &seqs2, ntrim, ctrim, parallel,
     ))
 }
-#[cfg(all(feature = "py_binds", feature = "pyo3"))]
+
+/// Compute whether two CDR3-V gene pairs are neighbors with tcrdist_gene.
+///
+/// This function is quicker than using the tcrdist_gene function since it computes
+/// whether the V genes are within the distance threshold and whether the difference
+/// in lengths won't incur a penalty larger than the distance threshold. With these
+/// two checks, many unnecessary calculations are avoided.
+///
+/// Parameters
+/// ----------
+/// s1 : iterable of str
+///     An iterable containing a CDR3 amino acid sequence and V gene pair.
+/// s2 : iterable of str
+///     An iterable containing a CDR3 amino acid sequence and V gene pair.
+/// threshold: int
+///     The distance threshold that will be used to call sequences neighbors.
+/// ntrim : int, default 3
+///     The position at which the distance calculation will begin.
+///     This parameter must be >= 0.
+/// ctrim : int, default 2
+///     The position, counted from the end, at which the calculation will end.
+    ///     This parameter must be >= 0.
+///
+/// Returns
+/// -------
+/// bool 
+///     Whether the two CDR3-V gene pairs are have tcrdist within the threshold.
+///
+/// Examples
+/// --------
+/// >>> s1 = ["CASRTGTVYEQYF", "TRBV2"]
+/// >>> s2 = ["CASSTLDRVYNSPLHF", "TRBV6-2"]
+/// >>> threshold = 20
+/// >>> ntrim = 3
+/// >>> ctrim = 2
+/// >>> are_neighbors = tcrdist_gene(s1, s2, threshold, ntrim, ctrim)
+/// >>> assert(are_neighbors == False)
+#[cfg(all(feature = "pyo3"))]
+#[pyfunction]
+#[pyo3(signature = (s1, s2, threshold, ntrim=3, ctrim=2))]
+fn tcrdist_gene_neighbor(
+    s1: [&str; 2],
+    s2: [&str; 2],
+    threshold: u16,
+    ntrim: usize,
+    ctrim: usize,
+) -> PyResult<bool> {
+    Ok(_distance::tcrdist_gene_neighbor(
+        s1, s2, threshold, ntrim, ctrim,
+    ))
+}
+
+#[cfg(all(feature = "pyo3"))]
+#[pyfunction]
+#[pyo3(signature = (seqs, threshold, ntrim=3, ctrim=2, parallel=false))]
+fn tcrdist_gene_neighbor_matrix(
+    seqs: Vec<[&str; 2]>,
+    threshold: u16,
+    ntrim: usize,
+    ctrim: usize,
+    parallel: bool,
+) -> PyResult<Vec<bool>> {
+    Ok(_distance::tcrdist_gene_neighbor_matrix(
+        &seqs, threshold, ntrim, ctrim, parallel,
+    ))
+}
+
+#[cfg(all(feature = "pyo3"))]
+#[pyfunction]
+#[pyo3(signature = (seq, seqs, threshold, ntrim=3, ctrim=2, parallel=false))]
+fn tcrdist_gene_neighbor_one_to_many(
+    seq: [&str; 2],
+    seqs: Vec<[&str; 2]>,
+    threshold: u16,
+    ntrim: usize,
+    ctrim: usize,
+    parallel: bool,
+) -> PyResult<Vec<bool>> {
+    Ok(_distance::tcrdist_gene_neighbor_one_to_many(
+        seq, &seqs, threshold, ntrim, ctrim, parallel,
+    ))
+}
+
+#[cfg(all(feature = "pyo3"))]
+#[pyfunction]
+#[pyo3(signature = (seqs1, seqs2, threshold, ntrim=3, ctrim=2, parallel=false))]
+fn tcrdist_gene_neighbor_many_to_many(
+    seqs1: Vec<[&str; 2]>,
+    seqs2: Vec<[&str; 2]>,
+    threshold: u16,
+    ntrim: usize,
+    ctrim: usize,
+    parallel: bool,
+) -> PyResult<Vec<bool>> {
+    Ok(_distance::tcrdist_gene_neighbor_many_to_many(
+        &seqs1, &seqs2, threshold, ntrim, ctrim, parallel,
+    ))
+}
+
 #[pymodule]
+#[pyo3(name = "tcrdist_rs")]
 pub fn tcrdist_rs(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(hamming, m)?)?;
     m.add_function(wrap_pyfunction!(hamming_matrix, m)?)?;
     m.add_function(wrap_pyfunction!(hamming_one_to_many, m)?)?;
     m.add_function(wrap_pyfunction!(hamming_many_to_many, m)?)?;
 
     m.add_function(wrap_pyfunction!(levenshtein_exp, m)?)?;
@@ -1297,9 +1419,15 @@
     m.add_function(wrap_pyfunction!(tcrdist_allele_one_to_many, m)?)?;
     m.add_function(wrap_pyfunction!(tcrdist_allele_many_to_many, m)?)?;
 
     m.add_function(wrap_pyfunction!(tcrdist_gene, m)?)?;
     m.add_function(wrap_pyfunction!(tcrdist_gene_matrix, m)?)?;
     m.add_function(wrap_pyfunction!(tcrdist_gene_one_to_many, m)?)?;
     m.add_function(wrap_pyfunction!(tcrdist_gene_many_to_many, m)?)?;
+
+    m.add_function(wrap_pyfunction!(tcrdist_gene_neighbor, m)?)?;
+    m.add_function(wrap_pyfunction!(tcrdist_gene_neighbor_matrix, m)?)?;
+    m.add_function(wrap_pyfunction!(tcrdist_gene_neighbor_one_to_many, m)?)?;
+    m.add_function(wrap_pyfunction!(tcrdist_gene_neighbor_many_to_many, m)?)?;
+
     Ok(())
 }
```

### Comparing `tcrdist_rs-0.1.0/src/match_table.rs` & `tcrdist_rs-0.1.1/src/match_table.rs`

 * *Files identical despite different names*

### Comparing `tcrdist_rs-0.1.0/Cargo.lock` & `tcrdist_rs-0.1.1/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "anyhow"
-version = "1.0.82"
+version = "1.0.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
+checksum = "b3d1d046238990b9cf5bcde22a3fb3584ee5cf65fb2765f454ed428c7a0063da"
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
@@ -43,23 +43,23 @@
 checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
 
 [[package]]
 name = "either"
-version = "1.11.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
@@ -73,17 +73,17 @@
 name = "inventory"
 version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f958d3d68f4167080a18141e10381e7634563984a537f2a49a30fd8e53ac5767"
 
 [[package]]
 name = "libc"
-version = "0.2.154"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "lock_api"
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
@@ -104,17 +104,17 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.2"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
@@ -133,17 +133,17 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.81"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
@@ -257,54 +257,54 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.60"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tcrdist_rs"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "once_cell",
  "pyo3",
  "rayon",
  "thiserror",
  "triple_accel",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.59"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.59"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
```

### Comparing `tcrdist_rs-0.1.0/pyproject.toml` & `tcrdist_rs-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tcrdist_rs-0.1.0/PKG-INFO` & `tcrdist_rs-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tcrdist_rs
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 Summary: Fast tcrdist routines between TCR sequences.
 Keywords: tcrdist
@@ -44,15 +44,15 @@
 ```bash
 pip install maturin
 ```
 
 To compile tcrdist, run
 
 ```bash
-maturin develop --release -F py_binds,pyo3 --profile release
+maturin develop --release --profile release
 ```
 
 ## Example
 
 We use the same [settings](https://tcrdist3.readthedocs.io/en/latest/tcrdistances.html#i-want-complete-control) as Python tcrdist. Notably, the keyword `parallel` enables the use of all CPU cores when computing many distances. However, be mindful of enabling it and use it only when there are enough sequences such that the overhead of parallelizing is less costly than the actual computation.
 
 ```python
```

