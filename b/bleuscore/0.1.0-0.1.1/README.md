# Comparing `tmp/bleuscore-0.1.0.tar.gz` & `tmp/bleuscore-0.1.1.tar.gz`

## Comparing `bleuscore-0.1.0.tar` & `bleuscore-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,34 @@
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 bleuscore-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     5144 2024-04-23 05:45:38.000000 bleuscore-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      900 2024-04-23 05:45:38.000000 bleuscore-0.1.0/.github/workflows/doc.yml
--rw-r--r--   0     1001      127      456 2024-04-23 05:45:38.000000 bleuscore-0.1.0/.gitignore
--rw-r--r--   0     1001      127      360 2024-04-23 05:45:38.000000 bleuscore-0.1.0/CHANGELOG.md
--rw-r--r--   0     1001      127     1068 2024-04-23 05:45:38.000000 bleuscore-0.1.0/LICENSE
--rw-r--r--   0     1001      127      821 2024-04-23 05:45:38.000000 bleuscore-0.1.0/README.md
--rw-r--r--   0     1001      127      146 2024-04-23 05:45:38.000000 bleuscore-0.1.0/python/bleuscore/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-23 05:45:38.000000 bleuscore-0.1.0/python/bleuscore/py.typed
--rw-r--r--   0     1001      127     4807 2024-04-23 05:45:38.000000 bleuscore-0.1.0/src/bleu.rs
--rw-r--r--   0     1001      127     2815 2024-04-23 05:45:38.000000 bleuscore-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127     3614 2024-04-23 05:45:38.000000 bleuscore-0.1.0/src/ngram.rs
--rw-r--r--   0     1001      127     3729 2024-04-23 05:45:38.000000 bleuscore-0.1.0/src/tokenizer.rs
--rw-r--r--   0     1001      127      484 2024-04-23 05:45:38.000000 bleuscore-0.1.0/tests/conftest.py
--rw-r--r--   0     1001      127     4897 2024-04-23 05:45:38.000000 bleuscore-0.1.0/tests/py_bleu.py
--rw-r--r--   0     1001      127     3488 2024-04-23 05:45:38.000000 bleuscore-0.1.0/tests/py_token.py
--rw-r--r--   0     1001      127     4463 2024-04-23 05:45:38.000000 bleuscore-0.1.0/tests/test_bleu_score.py
--rw-r--r--   0     1001      127     1318 2024-04-23 05:45:38.000000 bleuscore-0.1.0/tests/test_tokenizer.py
--rw-r--r--   0     1001      127     1074 2024-04-23 05:45:38.000000 bleuscore-0.1.0/tests/util.py
--rw-r--r--   0     1001      127    14252 2024-04-23 05:45:42.000000 bleuscore-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127     1970 2024-04-23 05:45:38.000000 bleuscore-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2292 1970-01-01 00:00:00.000000 bleuscore-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 bleuscore-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      127      900 2024-04-26 07:51:00.000000 bleuscore-0.1.1/.github/workflows/doc.yml
+-rw-r--r--   0     1001      127     5153 2024-04-26 07:51:00.000000 bleuscore-0.1.1/.github/workflows/maturin.yml
+-rw-r--r--   0     1001      127     1374 2024-04-26 07:51:00.000000 bleuscore-0.1.1/.github/workflows/rust.yml
+-rw-r--r--   0     1001      127      456 2024-04-26 07:51:00.000000 bleuscore-0.1.1/.gitignore
+-rw-r--r--   0     1001      127      478 2024-04-26 07:51:00.000000 bleuscore-0.1.1/CHANGELOG.md
+-rw-r--r--   0     1001      127     1068 2024-04-26 07:51:00.000000 bleuscore-0.1.1/LICENSE
+-rw-r--r--   0     1001      127     2848 2024-04-26 07:51:00.000000 bleuscore-0.1.1/README.md
+-rw-r--r--   0     1001      127   302127 2024-04-26 07:51:00.000000 bleuscore-0.1.1/asset/benchmark/n_1.png
+-rw-r--r--   0     1001      127   110049 2024-04-26 07:51:00.000000 bleuscore-0.1.1/asset/benchmark/n_100.png
+-rw-r--r--   0     1001      127   136288 2024-04-26 07:51:00.000000 bleuscore-0.1.1/asset/benchmark/n_10000.png
+-rw-r--r--   0     1001      127   117831 2024-04-26 07:51:00.000000 bleuscore-0.1.1/asset/benchmark/n_100000.png
+-rw-r--r--   0     1001      127   351628 2024-04-26 07:51:00.000000 bleuscore-0.1.1/asset/benchmark/simple.png
+-rw-r--r--   0     1001      127      178 2024-04-26 07:51:00.000000 bleuscore-0.1.1/benchmark/bench.sh
+-rw-r--r--   0     1001      127      206 2024-04-26 07:51:00.000000 bleuscore-0.1.1/benchmark/simple/hf_evaluate.py
+-rw-r--r--   0     1001      127     8279 2024-04-26 07:51:00.000000 bleuscore-0.1.1/benchmark/simple/local_hf_bleu.py
+-rw-r--r--   0     1001      127      179 2024-04-26 07:51:00.000000 bleuscore-0.1.1/benchmark/simple/rs_bleuscore.py
+-rw-r--r--   0     1001      127      247 2024-04-26 07:51:00.000000 bleuscore-0.1.1/benchmark/simple/sacre_bleu.py
+-rw-r--r--   0     1001      127      223 2024-04-26 07:51:00.000000 bleuscore-0.1.1/benchmark/simple/simulation_data.py
+-rw-r--r--   0     1001      127      146 2024-04-26 07:51:00.000000 bleuscore-0.1.1/python/bleuscore/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-26 07:51:00.000000 bleuscore-0.1.1/python/bleuscore/py.typed
+-rw-r--r--   0     1001      127     4735 2024-04-26 07:51:00.000000 bleuscore-0.1.1/src/bleu.rs
+-rw-r--r--   0     1001      127     2819 2024-04-26 07:51:00.000000 bleuscore-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      127     3508 2024-04-26 07:51:00.000000 bleuscore-0.1.1/src/ngram.rs
+-rw-r--r--   0     1001      127     3862 2024-04-26 07:51:00.000000 bleuscore-0.1.1/src/tokenizer.rs
+-rw-r--r--   0     1001      127      484 2024-04-26 07:51:00.000000 bleuscore-0.1.1/tests/conftest.py
+-rw-r--r--   0     1001      127     4897 2024-04-26 07:51:00.000000 bleuscore-0.1.1/tests/py_bleu.py
+-rw-r--r--   0     1001      127     3488 2024-04-26 07:51:00.000000 bleuscore-0.1.1/tests/py_token.py
+-rw-r--r--   0     1001      127     4463 2024-04-26 07:51:00.000000 bleuscore-0.1.1/tests/test_bleu_score.py
+-rw-r--r--   0     1001      127     1318 2024-04-26 07:51:00.000000 bleuscore-0.1.1/tests/test_tokenizer.py
+-rw-r--r--   0     1001      127     1074 2024-04-26 07:51:00.000000 bleuscore-0.1.1/tests/util.py
+-rw-r--r--   0     1001      127    14179 2024-04-26 07:51:05.000000 bleuscore-0.1.1/Cargo.lock
+-rw-r--r--   0     1001      127     1983 2024-04-26 07:51:00.000000 bleuscore-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4373 1970-01-01 00:00:00.000000 bleuscore-0.1.1/PKG-INFO
```

### Comparing `bleuscore-0.1.0/Cargo.toml` & `bleuscore-0.1.1/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [package]
 name = "bleuscore"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 authors = ["Mathew Shen <datahonor@gmail.com>"]
 repository = "https://github.com/shenxiangzhuang/bleuscore"
 readme = "README.md"
 license = "MIT"
-description = "A fast bleu score calculator"
+description = "A fast(not yet :) bleu score calculator"
 keywords = ["NLP", "Tokenizer", "BLEU", "DeepLearning"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "bleuscore"
-crate-type = ["cdylib"]
+crate-type = ["cdylib", "rlib"]
 
 [dependencies]
-cached = "0.49.3"
+cached = "0.50.0"
 regex = "1.10.4"
 lazy_static = "1.4.0"
 counter = "0.5.7"
 
 [dependencies.pyo3]
 version = "0.21.1"
 # "abi3-py38" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.8
```

### Comparing `bleuscore-0.1.0/.github/workflows/CI.yml` & `bleuscore-0.1.1/.github/workflows/maturin.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # This file is autogenerated by maturin v1.5.1
 # To update, run
 #
 #    maturin generate-ci github --pytest
 #
-name: CI
+name: Maturin CI
 
 on:
   push:
     branches:
       - main
       - master
     tags:
@@ -57,14 +57,15 @@
         if: ${{ startsWith(matrix.platform.target, 'x86_64') }}
         shell: bash
         run: |
           set -e
           pip install bleuscore --find-links dist --force-reinstall
           pip install pytest hypothesis evaluate
           pytest --hypothesis-show-statistics tests
+
       - name: pytest
         if: ${{ !startsWith(matrix.platform.target, 'x86') && matrix.platform.target != 'ppc64' }}
         uses: uraimo/run-on-arch-action@v2.5.0
         with:
           arch: ${{ matrix.platform.target }}
           distro: ubuntu22.04
           githubToken: ${{ github.token }}
```

### Comparing `bleuscore-0.1.0/.github/workflows/doc.yml` & `bleuscore-0.1.1/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.0/LICENSE` & `bleuscore-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.0/src/bleu.rs` & `bleuscore-0.1.1/src/bleu.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,131 +1,135 @@
+use crate::ngram::get_token_ngram_counter;
+use crate::tokenizer::{Tokenizer, Tokenizer13a};
 use std::cmp::min;
 use std::collections::HashMap;
-use crate::ngram::{get_token_ngram_counter};
-use crate::tokenizer::{Tokenizer, Tokenizer13a};
-
 
 /// The BLEU score data struct
 #[derive(Debug, Default)]
 pub struct BleuScore {
     pub bleu: f64,
     pub precisions: Vec<f64>,
     pub brevity_penalty: f64,
     pub length_ratio: f64,
     pub translation_length: usize,
     pub reference_length: usize,
 }
 
-/// compute the BLEU score with `Tokenizer13a` as default tokenizer
+/// compute the BLEU score with `Tokenizer13a` as default tokenizer.
+/// The implementation is based on [huggingface/nmt](https://github.com/huggingface/evaluate/blob/main/metrics/bleu/bleu.py)
 pub fn compute_score(
     references: Vec<Vec<String>>,
     predictions: Vec<String>,
     max_order: usize,
     smooth: bool,
 ) -> BleuScore {
     // init
     let mut matches_by_order: Vec<usize> = vec![0; max_order];
     let mut possible_matches_by_order: Vec<usize> = vec![0; max_order];
     let mut reference_length: usize = 0;
     let mut translation_length: usize = 0;
     let tokenizer = Tokenizer13a::new();
-    
-    for (references, translation) in 
-        references.iter().zip(predictions.iter()) {
+
+    for (references, translation) in references.iter().zip(predictions.iter()) {
         // tokenize
         let translation_tokens = tokenizer.tokenize(translation);
-        let references_tokens: Vec<Vec<String>> = references.iter()
-                                                            .map(|x| tokenizer.tokenize(x))
-                                                            .collect();
+        let references_tokens: Vec<Vec<String>> =
+            references.iter().map(|x| tokenizer.tokenize(x)).collect();
         // lengths
         reference_length += references_tokens.iter().map(|x| x.len()).min().unwrap();
         translation_length += translation_tokens.len();
-        
+
         // ngram count
         let translation_ngram_counts = get_token_ngram_counter(&translation_tokens, max_order);
         let mut merged_ref_ngram_counts = HashMap::new();
         for reference_tokens in references_tokens {
             let reference_ngram_counts = get_token_ngram_counter(&reference_tokens, max_order);
             for (key, value) in reference_ngram_counts {
-                merged_ref_ngram_counts.entry(key).and_modify(|v| *v += value).or_insert(value);
+                merged_ref_ngram_counts
+                    .entry(key)
+                    .and_modify(|v| *v += value)
+                    .or_insert(value);
             }
         }
-        
+
         // overlap count
         let mut overlap_counts = HashMap::new();
         for (k, v) in translation_ngram_counts {
             let key = k.clone();
             if merged_ref_ngram_counts.contains_key(&key) {
                 overlap_counts.insert(k, min(merged_ref_ngram_counts[&key], v));
-            }
-            else { 
-                continue
+            } else {
+                continue;
             }
         }
         for key in overlap_counts.keys() {
             let (_, order) = key;
             matches_by_order[order - 1] += overlap_counts[&key];
         }
-        
+
         // possible match
         for order in 1..=max_order {
             let possible_matches = translation_tokens.len().saturating_sub(order - 1);
             if possible_matches > 0 {
                 possible_matches_by_order[order - 1] += possible_matches
             }
         }
     }
-    
+
     // precisions calculation
-    let mut precisions:Vec<f64> = vec![0.0; max_order];
+    let mut precisions: Vec<f64> = vec![0.0; max_order];
     for i in 0..max_order {
         match smooth {
             true => {
-                precisions[i] = (matches_by_order[i] as f64 + 1.0) / 
-                    (possible_matches_by_order[i] as f64 + 1.0);
-            },
+                precisions[i] = (matches_by_order[i] as f64 + 1.0)
+                    / (possible_matches_by_order[i] as f64 + 1.0);
+            }
             false => {
                 if possible_matches_by_order[i] > 0 {
-                    precisions[i] = (matches_by_order[i] as f64) / 
-                        (possible_matches_by_order[i] as f64)
-                }
-                else { 
+                    precisions[i] =
+                        (matches_by_order[i] as f64) / (possible_matches_by_order[i] as f64)
+                } else {
                     precisions[i] = 0.0;
                 }
             }
         }
     }
-    
+
     let mut geo_mean = 0.0;
-    
+
     if precisions.iter().fold(f64::INFINITY, |a, &b| a.min(b)) > 0.0 {
-        let p_log_sum: f64 = (1.0 / max_order as f64) * precisions.iter()
-                                                                  .map(|&x| x.ln())
-                                                                  .sum::<f64>();
+        let p_log_sum: f64 =
+            (1.0 / max_order as f64) * precisions.iter().map(|&x| x.ln()).sum::<f64>();
         geo_mean = p_log_sum.exp();
     }
 
     let length_ratio: f64 = translation_length as f64 / reference_length as f64;
     let mut brevity_penalty = 1.0;
     if length_ratio <= 1.0 {
         brevity_penalty = (1.0 - 1.0 / length_ratio).exp();
     }
     let bleu = geo_mean * brevity_penalty;
-    BleuScore{bleu, precisions, brevity_penalty, length_ratio, translation_length, reference_length}
+    BleuScore {
+        bleu,
+        precisions,
+        brevity_penalty,
+        length_ratio,
+        translation_length,
+        reference_length,
+    }
 }
 
-
 #[cfg(test)]
 mod test {
-    use crate::bleu::{compute_score};
+    use crate::bleu::compute_score;
     #[test]
     fn test_bleu() {
         let references: Vec<Vec<String>> = vec![vec!["Hello, World!".to_string()]];
         let predictions: Vec<String> = vec!["Yellow, World!".to_string()];
         let max_order: usize = 4;
         let smooth: bool = true;
         let res = compute_score(references, predictions, max_order, smooth);
         // (0.668740304976422, [0.8, 0.75, 0.6666666666666666, 0.5], 1.0, 1.0, 4, 4)
         println!("result: {:?}", res);
         assert!((res.bleu - 0.668740304976422).abs() < 1e-10);
     }
-}
+}
```

### Comparing `bleuscore-0.1.0/src/lib.rs` & `bleuscore-0.1.1/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -27,28 +27,27 @@
 // set the parameters:
 let max_order: usize = 4;
 let smooth: bool = true;
 
 // calculate the BLEU score:
 let res = compute_score(references, predictions, max_order, smooth);
 println!("result: {:?}", res);
-// result: BleuScore { bleu: 0.668740304976422, precisions: [0.8, 0.75, 0.6666666666666666, 0.5], 
+// result: BleuScore { bleu: 0.668740304976422, precisions: [0.8, 0.75, 0.6666666666666666, 0.5],
 // brevity_penalty: 1.0, length_ratio: 1.0, translation_length: 4, reference_length: 4 }
 ```
 !*/
 mod tokenizer;
 pub use crate::tokenizer::{Tokenizer, Tokenizer13a, TokenizerRegex};
-mod ngram;
 mod bleu;
-pub use crate::bleu::{BleuScore, compute_score};
+mod ngram;
+pub use crate::bleu::{compute_score, BleuScore};
 
 use pyo3::prelude::*;
 use pyo3::types::IntoPyDict;
 
-
 #[pyfunction]
 fn tokenizer_regex(line: &str) -> PyResult<Vec<String>> {
     let tokenizer_regex = tokenizer::TokenizerRegex::new();
     let res = tokenizer_regex.tokenize(line);
     Ok(res)
 }
 
@@ -66,27 +65,26 @@
     predictions: Vec<String>,
     max_order: usize,
     smooth: bool,
 ) -> PyResult<PyObject> {
     let bleu = compute_score(references, predictions, max_order, smooth);
     Python::with_gil(|py| {
         let bleu_dict = [
-            ("bleu", bleu.bleu.to_object(py)), 
+            ("bleu", bleu.bleu.to_object(py)),
             ("precisions", bleu.precisions.to_object(py)),
             ("brevity_penalty", bleu.brevity_penalty.to_object(py)),
             ("length_ratio", bleu.length_ratio.to_object(py)),
             ("translation_length", bleu.translation_length.to_object(py)),
             ("reference_length", bleu.reference_length.to_object(py)),
-        ].into_py_dict_bound(py);
+        ]
+        .into_py_dict_bound(py);
         Ok(bleu_dict.into())
     })
-
 }
 
-
 /// A Python module implemented in Rust.
 #[pymodule]
 fn bleuscore(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(tokenizer_regex, m)?)?;
     m.add_function(wrap_pyfunction!(tokenizer_13a, m)?)?;
     m.add_function(wrap_pyfunction!(compute, m)?)?;
     m.add("__version__", env!("CARGO_PKG_VERSION"))?;
```

### Comparing `bleuscore-0.1.0/src/ngram.rs` & `bleuscore-0.1.1/src/ngram.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-use std::collections::HashMap;
 use counter::Counter;
-
+use std::collections::HashMap;
 
 /// Here the tokens' type is `&[String]` rather than `&Vec<String>`
 /// to fix `clippy::not_unsafe_ptr_arg_deref` error.
-pub fn get_token_ngram_counter(tokens: &[String], 
-                               max_order: usize,
-                              ) -> HashMap<(String, usize), usize> 
-{
+pub fn get_token_ngram_counter(
+    tokens: &[String],
+    max_order: usize,
+) -> HashMap<(String, usize), usize> {
     let mut count_map: HashMap<(String, usize), usize> = HashMap::new();
     for order in 1..=max_order {
         for start_index in 0..(tokens.len().saturating_sub(order - 1)) {
             // note: can not join with "", which will make 2-gram ('000', '00') = ('0000', '0')
             let ngram = tokens[start_index..(start_index + order)].join(" ");
-            count_map.entry((ngram, order))
-                     .and_modify(|counter| *counter += 1)
-                     .or_insert(1);
+            count_map
+                .entry((ngram, order))
+                .and_modify(|counter| *counter += 1)
+                .or_insert(1);
         }
     }
     count_map
 }
 
-
 /// TODO: change to use Counter to count ngram
 #[allow(dead_code)]
 fn get_ngram_counter(line: &str, max_order: usize) -> Counter<&str> {
     let mut counts: Counter<&str> = Counter::new();
     for order in 1..=max_order {
         for start_index in 0..(line.len().saturating_sub(order - 1)) {
             // println!("line: {}, start_index: {}, order: {}", line, start_index, order);
@@ -33,36 +32,37 @@
             // println!("ngram: {}", ngram);
             counts[&ngram] += 1;
         }
     }
     counts
 }
 
-
 #[cfg(test)]
 mod test {
     use crate::ngram::{get_ngram_counter, get_token_ngram_counter};
 
     #[test]
     fn test_get_token_ngram_short() {
         let tokens = vec!["a".to_string(), "b".to_string()];
-        let counter = get_token_ngram_counter(&tokens,4);
+        let counter = get_token_ngram_counter(&tokens, 4);
         assert_eq!(counter[&("a".to_string(), 1)], 1);
         assert_eq!(counter[&("b".to_string(), 1)], 1);
         assert_eq!(counter[&("a b".to_string(), 2)], 1);
     }
 
     #[test]
     fn test_get_token_ngram_long() {
         // aabc
-        let tokens: Vec<String> = vec!["a".to_string(),
-                                       "a".to_string(),
-                                       "b".to_string(),
-                                       "c".to_string()];
-        let counter = get_token_ngram_counter(&tokens,4);
+        let tokens: Vec<String> = vec![
+            "a".to_string(),
+            "a".to_string(),
+            "b".to_string(),
+            "c".to_string(),
+        ];
+        let counter = get_token_ngram_counter(&tokens, 4);
         assert_eq!(counter[&("a".to_string(), 1)], 2);
         assert_eq!(counter[&("b".to_string(), 1)], 1);
         assert_eq!(counter[&("c".to_string(), 1)], 1);
         assert_eq!(counter.get(&("d".to_string(), 1)), None);
 
         assert_eq!(counter[&("a a".to_string(), 2)], 1);
         assert_eq!(counter[&("a b".to_string(), 2)], 1);
@@ -72,15 +72,14 @@
         assert_eq!(counter[&("a a b".to_string(), 3)], 1);
         assert_eq!(counter[&("a b c".to_string(), 3)], 1);
         assert_eq!(counter[&("a a b c".to_string(), 4)], 1);
 
         assert_eq!(counter.len(), 9);
     }
 
-
     #[test]
     fn test_get_ngram_short() {
         let counter = get_ngram_counter("ab", 4);
         assert_eq!(counter[&"a"], 1);
         assert_eq!(counter[&"b"], 1);
         assert_eq!(counter[&"ab"], 1);
     }
@@ -97,8 +96,8 @@
         assert_eq!(counter[&"ab"], 1);
         assert_eq!(counter[&"bc"], 1);
         assert_eq!(counter[&"ac"], 0);
 
         assert_eq!(counter[&"aab"], 1);
         assert_eq!(counter[&"aabc"], 1);
     }
-}
+}
```

### Comparing `bleuscore-0.1.0/src/tokenizer.rs` & `bleuscore-0.1.1/src/tokenizer.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 use cached::proc_macro::cached;
 use lazy_static::lazy_static;
 use regex::Regex;
 
 lazy_static! {
     pub static ref REGEX_ARRAY: [(Regex, &'static str); 4] = [
-        (Regex::new(r"([\{-\~\[-\` -\&\(-\+\:-\@\/])").unwrap(),  r" $1 "),
+        (
+            Regex::new(r"([\{-\~\[-\` -\&\(-\+\:-\@\/])").unwrap(),
+            r" $1 "
+        ),
         (Regex::new(r"([^0-9])([\.,])").unwrap(), r"$1 $2 "),
         (Regex::new(r"([\.,])([^0-9])").unwrap(), r" $1 $2"),
         (Regex::new(r"([0-9])(-)").unwrap(), r"$1 $2 "),
     ];
 }
 
-
 /// tokenize function is used to tokenize the strings
 pub trait Tokenizer {
     fn signature(&self) -> &str;
     fn tokenize(&self, line: &str) -> Vec<String>;
 }
 
 /// Same implementation with [huggingface/sacrebleu](https://github.com/huggingface/evaluate/blob/main/metrics/bleu/tokenizer_13a.py)
 #[derive(Debug)]
 pub struct TokenizerRegex {
     pub signature: String,
 }
 
 impl Default for TokenizerRegex {
     fn default() -> Self {
-        Self {signature: "re".to_string()}
+        Self {
+            signature: "re".to_string(),
+        }
     }
 }
 
-
 impl TokenizerRegex {
     pub fn new() -> Self {
         Self::default()
     }
 }
 
-
-#[cached(size=65536)]
-fn regex_tokenize_cache(line: String) -> Vec<String>  {
+#[cached(size = 65536)]
+fn regex_tokenize_cache(line: String) -> Vec<String> {
     let mut res = line;
     for &(ref re_capture, re_replace) in REGEX_ARRAY.iter() {
         res = re_capture.replace_all(&res, re_replace).to_string();
     }
     res.split_whitespace().map(|x| x.to_string()).collect()
 }
 
@@ -52,84 +54,92 @@
         &self.signature
     }
     fn tokenize(&self, line: &str) -> Vec<String> {
         regex_tokenize_cache(line.to_string())
     }
 }
 
-
 /// Same implementation with [huggingface/sacrebleu](https://github.com/huggingface/evaluate/blob/main/metrics/bleu/tokenizer_13a.py)
 #[derive(Debug)]
 pub struct Tokenizer13a {
     pub signature: String,
 }
 
 impl Default for Tokenizer13a {
     fn default() -> Self {
-        Self {signature: "13a".to_string()}
+        Self {
+            signature: "13a".to_string(),
+        }
     }
 }
 
 impl Tokenizer13a {
     pub fn new() -> Self {
         Self::default()
     }
 }
 
-
-#[cached(size=65536)]
-fn tokenize_13a_cache(line: String) -> Vec<String>  {
+#[cached(size = 65536)]
+fn tokenize_13a_cache(line: String) -> Vec<String> {
     let mut res = line;
-    res = res.replace("<skipped>", "")
-             .replace("-\n", "")
-             .replace('\n', " ");
+    res = res
+        .replace("<skipped>", "")
+        .replace("-\n", "")
+        .replace('\n', " ");
     if res.contains('&') {
-        res = res.replace("&quot;", "\"")
-                 .replace("&amp;", "&")
-                 .replace("&lt;", "<")
-                 .replace("&gt;", ">");
+        res = res
+            .replace("&quot;", "\"")
+            .replace("&amp;", "&")
+            .replace("&lt;", "<")
+            .replace("&gt;", ">");
     }
     TokenizerRegex::new().tokenize(&format!(" {res} "))
 }
 
 impl Tokenizer for Tokenizer13a {
     fn signature(&self) -> &str {
         &self.signature
     }
     fn tokenize(&self, line: &str) -> Vec<String> {
         tokenize_13a_cache(line.to_string())
     }
 }
 
-
-
 #[cfg(test)]
 mod test {
     use crate::tokenizer;
     use crate::tokenizer::Tokenizer;
 
     #[test]
     fn test_tokenize_regex() {
         let tokenizer_regex = tokenizer::TokenizerRegex::new();
         let mut line = "Hello, World!";
         let mut res = tokenizer_regex.tokenize(line);
         assert_eq!(res, vec!["Hello", ",", "World", "!"]);
-        
+
         line = "/usr/sbin/sendmail - 0 errors, 12 warnings";
         res = tokenizer_regex.tokenize(line);
-        assert_eq!(res, vec!["/", "usr", "/", "sbin", "/", "sendmail", 
-                             "-", "0", "errors", ",", "12", "warnings"])
+        assert_eq!(
+            res,
+            vec![
+                "/", "usr", "/", "sbin", "/", "sendmail", "-", "0", "errors", ",", "12", "warnings"
+            ]
+        )
     }
 
     #[test]
     fn test_tokenize_13a_regex() {
         let tokenizer_regex = tokenizer::Tokenizer13a::new();
         let mut line = "Hello, &quot;World!<skipped>";
         let mut res = tokenizer_regex.tokenize(line);
         assert_eq!(res, vec!["Hello", ",", "\"", "World", "!"]);
 
         line = "/usr/sbin/sendmail - 0 errors, 12 warnings";
         res = tokenizer_regex.tokenize(line);
-        assert_eq!(res, vec!["/", "usr", "/", "sbin", "/", "sendmail",
-                             "-", "0", "errors", ",", "12", "warnings"])
+        assert_eq!(
+            res,
+            vec![
+                "/", "usr", "/", "sbin", "/", "sendmail", "-", "0", "errors", ",", "12", "warnings"
+            ]
+        )
     }
-}
+}
```

### Comparing `bleuscore-0.1.0/tests/py_bleu.py` & `bleuscore-0.1.1/tests/py_bleu.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.0/tests/py_token.py` & `bleuscore-0.1.1/tests/py_token.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.0/tests/test_bleu_score.py` & `bleuscore-0.1.1/tests/test_bleu_score.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.0/tests/test_tokenizer.py` & `bleuscore-0.1.1/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.0/tests/util.py` & `bleuscore-0.1.1/tests/util.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.0/Cargo.lock` & `bleuscore-0.1.1/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -33,54 +33,54 @@
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bleuscore"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "cached",
  "counter",
  "lazy_static",
  "pyo3",
  "regex",
 ]
 
 [[package]]
 name = "cached"
-version = "0.49.3"
+version = "0.50.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e8e463fceca5674287f32d252fb1d94083758b8709c160efae66d263e5f4eba"
+checksum = "10a7d38ed2761b8a13ce42bc44b09d5a052b88da2f9fead624c779f31ac0729a"
 dependencies = [
  "ahash",
  "cached_proc_macro",
  "cached_proc_macro_types",
  "hashbrown",
  "instant",
  "once_cell",
  "thiserror",
 ]
 
 [[package]]
 name = "cached_proc_macro"
-version = "0.20.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad9f16c0d84de31a2ab7fdf5f7783c14631f7075cf464eb3bb43119f61c9cb2a"
+checksum = "771aa57f3b17da6c8bcacb187bb9ec9bc81c8160e72342e67c329e0e1651a669"
 dependencies = [
  "darling",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn",
 ]
 
 [[package]]
 name = "cached_proc_macro_types"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ade8366b8bd5ba243f0a58f036cc0ca8a2f069cff1a2351ef1cac6b083e16fc0"
@@ -98,45 +98,45 @@
 checksum = "2d458e66999348f56fd3ffcfbb7f7951542075ca8359687c703de6500c1ddccd"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "darling"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
+checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
 dependencies = [
  "darling_core",
  "darling_macro",
 ]
 
 [[package]]
 name = "darling_core"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "109c1ca6e6b7f82cc233a97004ea8ed7ca123a9af07a8230878fcfda9b158bf0"
+checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim",
- "syn 1.0.109",
+ "syn",
 ]
 
 [[package]]
 name = "darling_macro"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4aab4dbc9f7611d8b55048a3a16d2d010c2c8334e46304b40ac1cc14bf3b48e"
+checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
 dependencies = [
  "darling_core",
  "quote",
- "syn 1.0.109",
+ "syn",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
@@ -188,17 +188,17 @@
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
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
 name = "memchr"
@@ -228,27 +228,27 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
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
  "windows-targets",
 ]
@@ -311,44 +311,44 @@
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.60",
+ "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.60",
+ "syn",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
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
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
 version = "1.10.4"
@@ -394,25 +394,14 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "syn"
-version = "1.0.109"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
-dependencies = [
- "proc-macro2",
- "quote",
- "unicode-ident",
-]
-
-[[package]]
-name = "syn"
 version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
@@ -437,15 +426,15 @@
 name = "thiserror-impl"
 version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn",
 ]
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
@@ -460,68 +449,75 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "windows-targets"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
+ "windows_i686_gnullvm",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.5"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "zerocopy"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
 dependencies = [
@@ -532,9 +528,9 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn",
 ]
```

### Comparing `bleuscore-0.1.0/pyproject.toml` & `bleuscore-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 dependencies = []
 
 [project.urls]
 Homepage = 'https://github.com/shenxiangzhuang/bleuscore'
 Source = 'https://github.com/shenxiangzhuang/bleuscore'
 
 [project.optional-dependencies]
-test = ["pytest", "pytest-sugar", "hypothesis", "evaluate"]
+test = ["pytest", "pytest-sugar", "hypothesis", "evaluate", "sacrebleu"]
 lint = ["black", "ruff~=0.3.7"]
 #docs = []
 #dev = []
 
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
```

