# Comparing `tmp/field-compression-benchmark-0.0.2.tar.gz` & `tmp/field-compression-benchmark-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "field-compression-benchmark-0.0.2.tar", last modified: Tue Apr  2 09:27:31 2024, max compression
+gzip compressed data, was "field-compression-benchmark-0.0.3.tar", last modified: Fri Apr 26 07:38:08 2024, max compression
```

## Comparing `field-compression-benchmark-0.0.2.tar` & `field-compression-benchmark-0.0.3.tar`

### file list

```diff
@@ -1,316 +1,325 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.738675 field-compression-benchmark-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/.cargo/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/.cargo/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)    88816 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-04-02 09:27:31.738675 field-compression-benchmark-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.698675 field-compression-benchmark-0.0.2/codecs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/bit-round/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/bit-round/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/bit-round/src/
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/bit-round/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/bit-transpose/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/bit-transpose/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/bit-transpose/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/bit-transpose/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/build/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/build/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/build/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/build/src/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/build/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/core/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/core/src/
--rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core/src/buffer.rs
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core/src/casts.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core/src/map.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core/src/slice.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7816 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core/src/ty.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/core-host/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-host/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.706675 field-compression-benchmark-0.0.2/codecs/core-host/src/
--rw-r--r--   0 runner    (1001) docker     (127)    11816 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-host/src/codec.rs
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-host/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-host/src/plugin.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/core-wasm/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-wasm/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/core-wasm/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-wasm/src/config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-wasm/src/convert.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/core-wasm/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/frontend/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/frontend/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/frontend/src/codec.rs
--rw-r--r--   0 runner    (1001) docker     (127)    21585 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/frontend/src/engine.rs
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/frontend/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/frontend/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)    24426 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/frontend/src/template.rs
--rw-r--r--   0 runner    (1001) docker     (127)    44331 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/frontend/src/transform.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/identity/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/identity/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/identity/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/identity/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/linear-quantize/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/linear-quantize/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/linear-quantize/src/
--rw-r--r--   0 runner    (1001) docker     (127)    18818 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/linear-quantize/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/log/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/log/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/log/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/log/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/reinterpret/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/reinterpret/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/reinterpret/src/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/reinterpret/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/sz3/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/sz3/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.710675 field-compression-benchmark-0.0.2/codecs/sz3/src/
--rw-r--r--   0 runner    (1001) docker     (127)     8951 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/sz3/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/uniform-noise/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/uniform-noise/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/uniform-noise/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/uniform-noise/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/wit/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/wit/world.wit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/zfp/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/zfp/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/zfp/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/zfp/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)    13336 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/zfp/src/zfp.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/zlib/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/zlib/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/zlib/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/zlib/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/zstd/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/zstd/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/codecs/zstd/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/codecs/zstd/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.702675 field-compression-benchmark-0.0.2/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/core/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/core/benchmark/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/case.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/goodness.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/measuring.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/performance.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/report.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/reporter.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/benchmark/src/settings.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/core/compressor/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/core/compressor/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.714675 field-compression-benchmark-0.0.2/core/compressor/src/codec/
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/codec/config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/codec/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10939 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/compress.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/compressor/src/compressor/
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/compressor/config.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/compressor/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/numcodecs.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/compressor/src/parameter/
--rw-r--r--   0 runner    (1001) docker     (127)    11429 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/parameter/config.rs
--rw-r--r--   0 runner    (1001) docker     (127)    24245 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/compressor/src/parameter/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/dataset/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/dataset/src/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/dataset/config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/dataset/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)    29862 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/units.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/dataset/src/variable/
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/variable/config.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/dataset/src/variable/derivative/
--rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/variable/derivative/config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/variable/derivative/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/dataset/src/variable/dimension/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/dataset/src/variable/dimension/config/
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/variable/dimension/config/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/variable/dimension/config/slice.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/variable/dimension/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/dataset/src/variable/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/error/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/error/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/error/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/error/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/goodness/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/goodness/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/goodness/src/
--rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/goodness/src/bit_information.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/goodness/src/correlation.rs
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/goodness/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/goodness/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/goodness/src/pca.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/goodness/src/uniformity.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.718675 field-compression-benchmark-0.0.2/core/measure/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/measure/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/core/measure/src/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/measure/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/measure/src/measurement.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/measure/src/stats.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/core/model/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/core/model/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/core/model/src/boundary/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/boundary/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/boundary/noop.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/boundary/periodic.rs
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/boundary/zero.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/core/model/src/extrapolation/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/extrapolation/direct.rs
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/extrapolation/euler_smoothing.rs
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/extrapolation/leapfrog.rs
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/extrapolation/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/extrapolation/runge_kutta.rs
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/core/model/src/model/
--rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/model/any.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/model/linadv.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/model/lorenz_63.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/model/lorenz_96.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/model/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/model/onedsw.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/model/twodsw.rs
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/core/model/src/num.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.702675 field-compression-benchmark-0.0.2/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/data/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/data/codecs/wasmtime.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.722675 field-compression-benchmark-0.0.2/fcbench/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/fcbench/fcbench/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/fcbench/fcbench/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/benchmark/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/codecs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/fcbench/fcbench/compressor/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/compressor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/compressor/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/fcbench/fcbench/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/dataset/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/fcbench/fcbench/model/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/model/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    29660 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/fcbench/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/fcbench/src/
--rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/src/benchmark.rs
--rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/src/compressor.rs
--rw-r--r--   0 runner    (1001) docker     (127)    21741 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/src/dataclass.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11940 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/src/dataset.rs
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)    26212 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fcbench/src/model.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/field_compression_benchmark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-04-02 09:27:31.000000 field-compression-benchmark-0.0.2/field_compression_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-02 09:27:31.000000 field-compression-benchmark-0.0.2/field_compression_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:27:31.000000 field-compression-benchmark-0.0.2/field_compression_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-02 09:27:31.000000 field-compression-benchmark-0.0.2/field_compression_benchmark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 09:27:31.000000 field-compression-benchmark-0.0.2/field_compression_benchmark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/fork/
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/fork/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/src/fork.rs
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/fork/src/reaper/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/src/reaper/canary.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/src/reaper/handler.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/src/reaper/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/src/reaper/worker.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/fork/src/work.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/rust-toolchain
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/rustfmt.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 09:27:31.738675 field-compression-benchmark-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/src/args.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/src/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/src/benchmarking/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/src/benchmarking/prepare.rs
--rw-r--r--   0 runner    (1001) docker     (127)    15158 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/src/benchmarking/report.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/src/fcpy.rs
--rw-r--r--   0 runner    (1001) docker     (127)    18774 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.702675 field-compression-benchmark-0.0.2/wasi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/build/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/build/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/build/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/build/src/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/build/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/cli/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/cli/src/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/cli/src/environment.rs
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/cli/src/exit.rs
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/cli/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/cli/src/stdio.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/cli/src/terminal.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/clocks/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/clocks/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/clocks/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/clocks/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/filesystem/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/filesystem/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/filesystem/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.726675 field-compression-benchmark-0.0.2/wasi/io/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/io/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/io/src/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/io/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/io/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/io/src/poll.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/io/src/streams.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/random/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/random/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/random/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/random/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/wit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.702675 field-compression-benchmark-0.0.2/wasi/wit/deps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/command.wit
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/environment.wit
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/exit.wit
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/imports.wit
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/run.wit
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/stdio.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/cli/terminal.wit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/wit/deps/clocks/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/clocks/monotonic-clock.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/clocks/wall-clock.wit
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/clocks/world.wit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/wit/deps/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/filesystem/preopens.wit
--rw-r--r--   0 runner    (1001) docker     (127)    27621 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/filesystem/types.wit
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/filesystem/world.wit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.730675 field-compression-benchmark-0.0.2/wasi/wit/deps/http/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/http/handler.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/http/proxy.wit
--rw-r--r--   0 runner    (1001) docker     (127)    24187 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/http/types.wit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/wasi/wit/deps/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/io/error.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/io/poll.wit
--rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/io/streams.wit
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/io/world.wit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/wasi/wit/deps/random/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/random/insecure-seed.wit
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/random/insecure.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/random/random.wit
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/random/world.wit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:27:31.734675 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/instance-network.wit
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/ip-name-lookup.wit
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/network.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/tcp-create-socket.wit
--rw-r--r--   0 runner    (1001) docker     (127)    20199 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/tcp.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/udp-create-socket.wit
--rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/udp.wit
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/deps/sockets/world.wit
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-02 09:27:23.000000 field-compression-benchmark-0.0.2/wasi/wit/world.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.562685 field-compression-benchmark-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.534684 field-compression-benchmark-0.0.3/.cargo/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/.cargo/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    94295 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-04-26 07:38:08.562685 field-compression-benchmark-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.526684 field-compression-benchmark-0.0.3/codecs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.534684 field-compression-benchmark-0.0.3/codecs/bit-round/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/bit-round/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.534684 field-compression-benchmark-0.0.3/codecs/bit-round/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/bit-round/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.534684 field-compression-benchmark-0.0.3/codecs/bit-transpose/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/bit-transpose/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.534684 field-compression-benchmark-0.0.3/codecs/bit-transpose/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/bit-transpose/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.534684 field-compression-benchmark-0.0.3/codecs/build/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/build/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8281 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/build/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.534684 field-compression-benchmark-0.0.3/codecs/build/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/build/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.534684 field-compression-benchmark-0.0.3/codecs/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.538684 field-compression-benchmark-0.0.3/codecs/core/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core/src/buffer.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core/src/casts.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core/src/map.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core/src/slice.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core/src/slice_mut.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9013 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core/src/ty.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.534684 field-compression-benchmark-0.0.3/codecs/core-host/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core-host/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.534684 field-compression-benchmark-0.0.3/codecs/core-host/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    14012 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core-host/src/codec.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core-host/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core-host/src/plugin.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core-host/src/store.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.534684 field-compression-benchmark-0.0.3/codecs/core-wasm/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core-wasm/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core-wasm/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.538684 field-compression-benchmark-0.0.3/codecs/core-wasm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core-wasm/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core-wasm/src/convert.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core-wasm/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.538684 field-compression-benchmark-0.0.3/codecs/core-wasm/wit/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core-wasm/wit/deps.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/core-wasm/wit/world.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.538684 field-compression-benchmark-0.0.3/codecs/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/frontend/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/frontend/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.538684 field-compression-benchmark-0.0.3/codecs/frontend/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    14884 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/frontend/src/codec.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    22181 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/frontend/src/engine.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/frontend/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/frontend/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/frontend/src/logging.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/frontend/src/stdio.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/frontend/src/template.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.538684 field-compression-benchmark-0.0.3/codecs/frontend/src/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/frontend/src/transform/instcnt.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/frontend/src/transform/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    39257 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/frontend/src/transform/nan.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.538684 field-compression-benchmark-0.0.3/codecs/frontend/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/frontend/tests/sz3.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.538684 field-compression-benchmark-0.0.3/codecs/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/identity/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.538684 field-compression-benchmark-0.0.3/codecs/identity/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/identity/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/linear-quantize/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/linear-quantize/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/linear-quantize/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    18818 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/linear-quantize/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/log/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/log/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/log/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/reinterpret/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/reinterpret/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/reinterpret/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/reinterpret/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/round/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/round/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/round/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/round/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/running-standardize/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/running-standardize/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/running-standardize/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/running-standardize/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/sz3/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/sz3/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/sz3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/sz3/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/uniform-noise/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/uniform-noise/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/uniform-noise/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/uniform-noise/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/wit/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/wit/codec.wit
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/wit/world.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/zfp/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/zfp/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/zfp/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/zfp/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    13435 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/zfp/src/zfp.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/zlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/zlib/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/zlib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/zlib/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/zstd/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/zstd/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/codecs/zstd/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/codecs/zstd/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.530684 field-compression-benchmark-0.0.3/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.542684 field-compression-benchmark-0.0.3/core/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/benchmark/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.546685 field-compression-benchmark-0.0.3/core/benchmark/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/benchmark/src/case.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/benchmark/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/benchmark/src/goodness.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/benchmark/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/benchmark/src/measuring.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/benchmark/src/performance.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/benchmark/src/report.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/benchmark/src/reporter.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/benchmark/src/settings.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.546685 field-compression-benchmark-0.0.3/core/compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/compressor/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.546685 field-compression-benchmark-0.0.3/core/compressor/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.546685 field-compression-benchmark-0.0.3/core/compressor/src/codec/
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/compressor/src/codec/config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/compressor/src/codec/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/compressor/src/compress.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.546685 field-compression-benchmark-0.0.3/core/compressor/src/compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/compressor/src/compressor/config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/compressor/src/compressor/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/compressor/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/compressor/src/numcodecs.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.546685 field-compression-benchmark-0.0.3/core/compressor/src/parameter/
+-rw-r--r--   0 runner    (1001) docker     (127)    11429 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/compressor/src/parameter/config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    24245 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/compressor/src/parameter/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.546685 field-compression-benchmark-0.0.3/core/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/dataset/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.546685 field-compression-benchmark-0.0.3/core/dataset/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.546685 field-compression-benchmark-0.0.3/core/dataset/src/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/dataset/src/dataset/config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/dataset/src/dataset/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/dataset/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    29862 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/dataset/src/units.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.546685 field-compression-benchmark-0.0.3/core/dataset/src/variable/
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/dataset/src/variable/config.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.546685 field-compression-benchmark-0.0.3/core/dataset/src/variable/derivative/
+-rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/dataset/src/variable/derivative/config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/dataset/src/variable/derivative/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.546685 field-compression-benchmark-0.0.3/core/dataset/src/variable/dimension/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.546685 field-compression-benchmark-0.0.3/core/dataset/src/variable/dimension/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/dataset/src/variable/dimension/config/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/dataset/src/variable/dimension/config/slice.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/dataset/src/variable/dimension/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/dataset/src/variable/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.550685 field-compression-benchmark-0.0.3/core/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/error/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.550685 field-compression-benchmark-0.0.3/core/error/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/error/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.550685 field-compression-benchmark-0.0.3/core/goodness/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/goodness/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.550685 field-compression-benchmark-0.0.3/core/goodness/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    14488 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/goodness/src/bit_information.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/goodness/src/correlation.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/goodness/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/goodness/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/goodness/src/pca.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/goodness/src/uniformity.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.550685 field-compression-benchmark-0.0.3/core/measure/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/measure/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.550685 field-compression-benchmark-0.0.3/core/measure/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/measure/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/measure/src/measurement.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/measure/src/stats.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.550685 field-compression-benchmark-0.0.3/core/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.550685 field-compression-benchmark-0.0.3/core/model/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.550685 field-compression-benchmark-0.0.3/core/model/src/boundary/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/boundary/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/boundary/noop.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/boundary/periodic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/boundary/zero.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.550685 field-compression-benchmark-0.0.3/core/model/src/extrapolation/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/extrapolation/direct.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/extrapolation/euler_smoothing.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/extrapolation/leapfrog.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/extrapolation/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/extrapolation/runge_kutta.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.554685 field-compression-benchmark-0.0.3/core/model/src/model/
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/model/any.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/model/linadv.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/model/lorenz_63.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/model/lorenz_96.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/model/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/model/onedsw.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/model/twodsw.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/core/model/src/num.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.530684 field-compression-benchmark-0.0.3/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.554685 field-compression-benchmark-0.0.3/data/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/data/codecs/wasmtime.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.554685 field-compression-benchmark-0.0.3/fcbench/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.562685 field-compression-benchmark-0.0.3/fcbench/fcbench/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/fcbench/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.562685 field-compression-benchmark-0.0.3/fcbench/fcbench/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/fcbench/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/fcbench/benchmark/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/fcbench/codecs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.562685 field-compression-benchmark-0.0.3/fcbench/fcbench/compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/fcbench/compressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/fcbench/compressor/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.562685 field-compression-benchmark-0.0.3/fcbench/fcbench/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/fcbench/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/fcbench/dataset/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.562685 field-compression-benchmark-0.0.3/fcbench/fcbench/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/fcbench/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/fcbench/model/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29660 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/fcbench/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.554685 field-compression-benchmark-0.0.3/fcbench/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/src/benchmark.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/src/compressor.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    21741 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/src/dataclass.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11940 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/src/dataset.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    27608 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fcbench/src/model.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.562685 field-compression-benchmark-0.0.3/field_compression_benchmark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-04-26 07:38:08.000000 field-compression-benchmark-0.0.3/field_compression_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-04-26 07:38:08.000000 field-compression-benchmark-0.0.3/field_compression_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 07:38:08.000000 field-compression-benchmark-0.0.3/field_compression_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-26 07:38:08.000000 field-compression-benchmark-0.0.3/field_compression_benchmark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-26 07:38:08.000000 field-compression-benchmark-0.0.3/field_compression_benchmark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.554685 field-compression-benchmark-0.0.3/fork/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fork/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.554685 field-compression-benchmark-0.0.3/fork/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fork/src/fork.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fork/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.554685 field-compression-benchmark-0.0.3/fork/src/reaper/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fork/src/reaper/canary.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fork/src/reaper/handler.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fork/src/reaper/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fork/src/reaper/worker.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/fork/src/work.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/rust-toolchain
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/rustfmt.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 07:38:08.562685 field-compression-benchmark-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.554685 field-compression-benchmark-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/src/args.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.554685 field-compression-benchmark-0.0.3/src/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/src/benchmarking/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/src/benchmarking/prepare.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    15158 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/src/benchmarking/report.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/src/fcpy.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    18774 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.530684 field-compression-benchmark-0.0.3/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.554685 field-compression-benchmark-0.0.3/utils/wit-deps/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/utils/wit-deps/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/utils/wit-deps/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.554685 field-compression-benchmark-0.0.3/utils/wit-deps/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/utils/wit-deps/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.530684 field-compression-benchmark-0.0.3/wasi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.558685 field-compression-benchmark-0.0.3/wasi/build/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/build/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/build/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.558685 field-compression-benchmark-0.0.3/wasi/build/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/build/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.558685 field-compression-benchmark-0.0.3/wasi/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/cli/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/cli/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.558685 field-compression-benchmark-0.0.3/wasi/cli/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/cli/src/environment.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/cli/src/exit.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/cli/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/cli/src/stdio.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/cli/src/terminal.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.558685 field-compression-benchmark-0.0.3/wasi/cli/wit/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/cli/wit/deps.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/cli/wit/world.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.558685 field-compression-benchmark-0.0.3/wasi/clocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/clocks/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/clocks/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.558685 field-compression-benchmark-0.0.3/wasi/clocks/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/clocks/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.558685 field-compression-benchmark-0.0.3/wasi/clocks/wit/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/clocks/wit/deps.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/clocks/wit/world.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.558685 field-compression-benchmark-0.0.3/wasi/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/filesystem/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/filesystem/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.558685 field-compression-benchmark-0.0.3/wasi/filesystem/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/filesystem/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.558685 field-compression-benchmark-0.0.3/wasi/filesystem/wit/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/filesystem/wit/deps.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/filesystem/wit/world.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.558685 field-compression-benchmark-0.0.3/wasi/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/io/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/io/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.558685 field-compression-benchmark-0.0.3/wasi/io/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/io/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/io/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/io/src/poll.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/io/src/streams.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.562685 field-compression-benchmark-0.0.3/wasi/io/wit/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/io/wit/deps.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/io/wit/world.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.562685 field-compression-benchmark-0.0.3/wasi/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/random/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/random/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.562685 field-compression-benchmark-0.0.3/wasi/random/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/random/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.562685 field-compression-benchmark-0.0.3/wasi/random/wit/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/random/wit/deps.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/random/wit/world.wit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 07:38:08.562685 field-compression-benchmark-0.0.3/wasi/wit/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-26 07:38:00.000000 field-compression-benchmark-0.0.3/wasi/wit/world.wit
```

### Comparing `field-compression-benchmark-0.0.2/Cargo.lock` & `field-compression-benchmark-0.0.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -86,25 +86,31 @@
 dependencies = [
  "anstyle",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.81"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
+checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 
 [[package]]
 name = "arbitrary"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d5a26814d8dcb93b0e5a0ff3c6d80a8843bafb21b39e8e18a6f05471870e110"
 
 [[package]]
+name = "arc-swap"
+version = "1.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "69f7f8c3906b62b754cd5326047894316021dcfe5a194c8ea52bdd94934a3457"
+
+[[package]]
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "autocfg"
@@ -115,20 +121,14 @@
 [[package]]
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
-name = "beef"
-version = "0.5.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3a8241f3ebb85c056b509d4327ad0358fbbba6ffb340bf388f26350aeda225b1"
-
-[[package]]
 name = "bincode"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
@@ -148,38 +148,38 @@
  "peeking_take_while",
  "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn 2.0.55",
+ "syn 2.0.60",
  "which",
 ]
 
 [[package]]
 name = "bindgen"
 version = "0.69.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a00dc851838a2120612785d195287475a3ac45514741da670b735818822129a0"
 dependencies = [
  "bitflags 2.5.0",
  "cexpr",
  "clang-sys",
- "itertools",
+ "itertools 0.12.1",
  "lazy_static",
  "lazycell",
  "log",
  "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn 2.0.55",
+ "syn 2.0.60",
  "which",
 ]
 
 [[package]]
 name = "bit-round-codec"
 version = "0.1.0"
 dependencies = [
@@ -263,23 +263,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "51670c3aa053938b0ee3bd67c3817e471e626151131b934038e83c5bf8de48f5"
 dependencies = [
  "once_cell",
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
  "syn_derive",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "byte-unit"
 version = "5.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ac19bdf0b2665407c39d82dbc937e951e7e2001609f0fb32edd0af45a2d63e"
 dependencies = [
@@ -326,20 +326,21 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cexpr"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
@@ -397,15 +398,15 @@
 version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck 0.5.0",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
@@ -425,24 +426,38 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67ba02a97a2bd10f4b59b25c7973101c79642302776489e030cd13cdab09ed15"
 
 [[package]]
 name = "codecs-build"
 version = "0.1.0"
 dependencies = [
+ "bit-round-codec",
+ "bit-transpose-codec",
  "flate2",
+ "identity-codec",
+ "linear-quantize-codec",
+ "log-codec",
+ "reinterpret-codec",
+ "round-codec",
+ "running-standardize-codec",
+ "sz3-codec",
  "tar",
- "wit-component 0.202.0",
+ "uniform-noise-codec",
+ "wit-component 0.205.0",
+ "zfp-codec",
+ "zlib-codec",
+ "zstd-codec",
 ]
 
 [[package]]
 name = "codecs-core"
 version = "0.1.0"
 dependencies = [
  "serde",
+ "thiserror",
 ]
 
 [[package]]
 name = "codecs-core-host"
 version = "0.1.0"
 dependencies = [
  "anyhow",
@@ -457,55 +472,71 @@
 
 [[package]]
 name = "codecs-core-wasm"
 version = "0.1.0"
 dependencies = [
  "codecs-core",
  "format_serde_error",
+ "log",
  "serde",
  "serde_json",
+ "wasi-logger",
  "wit-bindgen",
+ "wit-deps",
 ]
 
 [[package]]
 name = "codecs-frontend"
 version = "0.1.0"
 dependencies = [
  "anyhow",
+ "codecs-build",
  "codecs-core",
  "codecs-core-host",
  "convert_case",
  "core-error",
  "indexmap 2.2.6",
+ "log",
  "numpy",
  "polonius-the-crab",
  "pyo3",
  "pyodide-webassembly-runtime-layer",
  "semver",
+ "simple_logger",
  "thiserror",
- "topological-sort",
  "vecmap-rs",
  "virtual-wasi-build",
- "wac-parser",
+ "wac-graph",
  "walrus",
  "wasm_component_layer",
  "wasm_runtime_layer",
- "wasmparser 0.202.0",
+ "wasmparser 0.205.0",
  "wasmtime",
- "wit-component 0.202.0",
- "wit-parser 0.202.0",
+ "wasmtime_runtime_layer",
+ "wit-component 0.205.0",
+ "wit-parser 0.205.0",
 ]
 
 [[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
+name = "colored"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cbf2150cce219b664a8a70df7a1f933836724b503f8a413af9365b4dcc4d90b8"
+dependencies = [
+ "lazy_static",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "convert_case"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec182b0ca2f35d8fc196cf3404988fd8b8c739a4d270ff118a398feb0cbec1ca"
 dependencies = [
  "unicode-segmentation",
 ]
@@ -596,14 +627,15 @@
  "thiserror",
 ]
 
 [[package]]
 name = "core-model"
 version = "0.1.0"
 dependencies = [
+ "dyn-clone",
  "ndarray",
  "num-traits",
  "rand",
  "rand_distr",
  "serde",
 ]
 
@@ -614,119 +646,129 @@
 checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "cranelift-bforest"
-version = "0.105.3"
+version = "0.105.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16d5521e2abca66bbb1ddeecbb6f6965c79160352ae1579b39f8c86183895c24"
+checksum = "496c993b62bdfbe9b4c518b8b3e1fdba9f89ef89fcccc050ab61d91dfba9fbaf"
 dependencies = [
- "cranelift-entity",
+ "cranelift-entity 0.105.4",
 ]
 
 [[package]]
 name = "cranelift-codegen"
-version = "0.105.3"
+version = "0.105.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef40a4338a47506e832ac3e53f7f1375bc59351f049a8379ff736dd02565bd95"
+checksum = "96b922abb6be41fc383f5e9da65b58d32d0d0a32c87dfe3bbbcb61a09119506c"
 dependencies = [
  "bumpalo",
  "cranelift-bforest",
  "cranelift-codegen-meta",
  "cranelift-codegen-shared",
  "cranelift-control",
- "cranelift-entity",
+ "cranelift-entity 0.105.4",
  "cranelift-isle",
  "gimli 0.28.1",
  "hashbrown 0.14.3",
  "log",
  "regalloc2",
  "smallvec",
  "target-lexicon",
 ]
 
 [[package]]
 name = "cranelift-codegen-meta"
-version = "0.105.3"
+version = "0.105.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d24cd5d85985c070f73dfca07521d09086362d1590105ba44b0932bf33513b61"
+checksum = "634c2ed9ef8a04ca42535a3e2e7917e4b551f2f306f4df2d935a6e71e346c167"
 dependencies = [
  "cranelift-codegen-shared",
 ]
 
 [[package]]
 name = "cranelift-codegen-shared"
-version = "0.105.3"
+version = "0.105.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0584c4363e3aa0a3c7cb98a778fbd5326a3709f117849a727da081d4051726c"
+checksum = "00cde1425b4da28bb0d5ff010030ea9cc9be7aded342ae099b394284f17cefce"
 
 [[package]]
 name = "cranelift-control"
-version = "0.105.3"
+version = "0.105.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f25ecede098c6553fdba362a8e4c9ecb8d40138363bff47f9712db75be7f0571"
+checksum = "1622125c99f1864aaf44e57971770c4a918d081d4b4af0bb597bdf624660ed66"
 dependencies = [
  "arbitrary",
 ]
 
 [[package]]
 name = "cranelift-entity"
-version = "0.105.3"
+version = "0.105.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea081a42f25dc4c5b248b87efdd87dcd3842a1050a37524ec5391e6172058cb"
+checksum = "ea97887aca1c0cbe7f8513874dc3603e9744fb1cfa78840ca8897bd2766bd35b"
+dependencies = [
+ "serde",
+ "serde_derive",
+]
+
+[[package]]
+name = "cranelift-entity"
+version = "0.106.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f1930946836da6f514da87625cd1a0331f3908e0de454628c24a0b97b130c4d4"
 dependencies = [
  "serde",
  "serde_derive",
 ]
 
 [[package]]
 name = "cranelift-frontend"
-version = "0.105.3"
+version = "0.105.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9796e712f5af797e247784f7518e6b0a83a8907d73d51526982d86ecb3a58b68"
+checksum = "4cdade4c14183fe41482071ed77d6a38cb95a17c7a0a05e629152e6292c4f8cb"
 dependencies = [
  "cranelift-codegen",
  "log",
  "smallvec",
  "target-lexicon",
 ]
 
 [[package]]
 name = "cranelift-isle"
-version = "0.105.3"
+version = "0.105.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4a66ccad5782f15c80e9dd5af0df4acfe6e3eee98e8f7354a2e5c8ec3104bdd"
+checksum = "dbbe4d3ad7bd4bf4a8d916c8460b441cf92417f5cdeacce4dd1d96eee70b18a2"
 
 [[package]]
 name = "cranelift-native"
-version = "0.105.3"
+version = "0.105.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "285e80df1d9b79ded9775b285df68b920a277b84f88a7228d2f5bc31fcdc58eb"
+checksum = "c46be4ed1fc8f36df4e2a442b8c30a39d8c03c1868182978f4c04ba2c25c9d4f"
 dependencies = [
  "cranelift-codegen",
  "libc",
  "target-lexicon",
 ]
 
 [[package]]
 name = "cranelift-wasm"
-version = "0.105.3"
+version = "0.105.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4135b0ab01fd16aa8f8821196e9e2fe15953552ccaef8ba5153be0ced04ef757"
+checksum = "a1d4c4a785a7866da89d20df159e3c4f96a5f14feb83b1f5998cfd5fe2e74d06"
 dependencies = [
  "cranelift-codegen",
- "cranelift-entity",
+ "cranelift-entity 0.105.4",
  "cranelift-frontend",
- "itertools",
+ "itertools 0.10.5",
  "log",
  "smallvec",
  "wasmparser 0.121.2",
- "wasmtime-types",
+ "wasmtime-types 18.0.4",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
@@ -793,24 +835,30 @@
 dependencies = [
  "libc",
  "redox_users",
  "winapi",
 ]
 
 [[package]]
+name = "dyn-clone"
+version = "1.0.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
+
+[[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "encoding_rs"
-version = "0.8.33"
+version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
+checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "env_logger"
 version = "0.10.2"
@@ -862,26 +910,28 @@
 name = "fastrand"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
 
 [[package]]
 name = "fcbench"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
  "codecs-build",
  "codecs-frontend",
  "core-benchmark",
  "core-compressor",
  "core-dataset",
  "core-error",
  "core-model",
+ "dyn-clone",
  "ndarray",
  "numpy",
  "pyo3",
+ "pyo3-log",
  "pythonize",
  "rand",
  "rand_chacha",
  "rand_distr",
  "serde",
  "serde-reflection",
  "serde_path_to_error",
@@ -934,14 +984,26 @@
  "cfg-if",
  "libc",
  "redox_syscall",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "fixedbitset"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
+
+[[package]]
+name = "flagset"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cdeb3aa5e95cf9aabc17f060cfa0ced7b83f042390760ca53bf09df9968acaa1"
+
+[[package]]
 name = "flate2"
 version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
@@ -1019,17 +1081,17 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
@@ -1253,24 +1315,33 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
-version = "0.1.28"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -1307,32 +1378,31 @@
 [[package]]
 name = "libloading"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "libredox"
-version = "0.0.1"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85c833ca1e66078851dba29046874e38f08b2c883700aa29a03ddd3b23814ee8"
+checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
 dependencies = [
  "bitflags 2.5.0",
  "libc",
- "redox_syscall",
 ]
 
 [[package]]
 name = "linear-quantize-codec"
 version = "0.1.0"
 dependencies = [
  "codecs-core",
@@ -1370,47 +1440,14 @@
 dependencies = [
  "codecs-core",
  "codecs-core-wasm",
  "serde",
 ]
 
 [[package]]
-name = "logos"
-version = "0.14.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "161971eb88a0da7ae0c333e1063467c5b5727e7fb6b710b8db4814eade3a42e8"
-dependencies = [
- "logos-derive",
-]
-
-[[package]]
-name = "logos-codegen"
-version = "0.14.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e31badd9de5131fdf4921f6473d457e3dd85b11b7f091ceb50e4df7c3eeb12a"
-dependencies = [
- "beef",
- "fnv",
- "lazy_static",
- "proc-macro2",
- "quote",
- "regex-syntax",
- "syn 2.0.55",
-]
-
-[[package]]
-name = "logos-derive"
-version = "0.14.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c2a69b3eb68d5bd595107c9ee58d7e07fe2bb5e360cc85b0f084dedac80de0a"
-dependencies = [
- "logos-codegen",
-]
-
-[[package]]
 name = "mach"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b823e83b2affd8f40a9ee8c29dbc56404c1e34cd2710921f2801e2cf29527afa"
 dependencies = [
  "libc",
 ]
@@ -1446,38 +1483,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "miette"
-version = "7.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4edc8853320c2a0dab800fbda86253c8938f6ea88510dc92c5f1ed20e794afc1"
-dependencies = [
- "cfg-if",
- "miette-derive",
- "serde",
- "thiserror",
- "unicode-width",
-]
-
-[[package]]
-name = "miette-derive"
-version = "7.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dcf09caffaac8068c346b6df2a7fc27a177fd20b39421a39ce0a211bde679a6c"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.55",
-]
-
-[[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
@@ -1637,14 +1650,24 @@
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
+name = "petgraph"
+version = "0.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1d3afd2628e69da2be385eb6f2fd57c8ac7977ceeff6dc166ff1657b0e386a9"
+dependencies = [
+ "fixedbitset",
+ "indexmap 2.2.6",
+]
+
+[[package]]
 name = "pkg-config"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
 name = "polonius-the-crab"
@@ -1686,20 +1709,20 @@
 dependencies = [
  "env_logger",
  "log",
 ]
 
 [[package]]
 name = "prettyplease"
-version = "0.2.17"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8d3928fb5db768cb86f891ff014f0144589297e3c6a1aba6ed7cecfdace270c7"
+checksum = "5ac2cf0f2e4f42b49f5ffd07dae8d746508ef7526c13940e5f524012ae6c6550"
 dependencies = [
  "proc-macro2",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "proc-macro-crate"
 version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
@@ -1728,17 +1751,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "psm"
 version = "0.1.21"
@@ -1766,17 +1789,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "puruspe"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c6778a7ae74b21f07fc5b9d550b1fdc212d719ec76d03cd2940c41002247c8a"
+checksum = "06a1eed715f625eaa95fba5e049dcf7bc06fa396d6d2e55015b3764e234dfd3f"
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
@@ -1810,45 +1833,57 @@
 checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
+name = "pyo3-log"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4c10808ee7250403bedb24bc30c32493e93875fef7ba3e4292226fe924f398bd"
+dependencies = [
+ "arc-swap",
+ "log",
+ "pyo3",
+]
+
+[[package]]
 name = "pyo3-macros"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyodide-webassembly-runtime-layer"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38c50baf5fe8876a5dbd044875621dd47c3d5f0af182ae176dcbdd3e2006e275"
+checksum = "4c4516e325e63c802de7fb7ca463f14e0559db7bf6cbcd24e443a2342178c10f"
 dependencies = [
  "anyhow",
+ "flagset",
  "fxhash",
  "pyo3",
  "wasm_runtime_layer",
  "wasmparser 0.201.0",
  "wobbly",
 ]
 
@@ -1859,17 +1894,17 @@
 dependencies = [
  "pyo3",
  "serde",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -1941,17 +1976,17 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_users"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a18479200779601e498ada4e8c1e1f50e3ee19deb0259c25825a98b5603b2cb4"
+checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
 dependencies = [
  "getrandom",
  "libredox",
  "thiserror",
 ]
 
 [[package]]
@@ -1967,15 +2002,15 @@
 name = "ref-cast-impl"
 version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5fddb4f8d99b0a2ebafc65a87a69a7b9875e4b1ae1f00db265d300ef7f28bccc"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "regalloc2"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad156d539c879b7a24a363a2016d77961786e71f48f2e2fc8302a92abd2429a6"
@@ -2060,14 +2095,43 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "rolling-stats"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bb8b4ded7f5dde5c7ecdc992adc38dd88b999424c0ce6d081ed79ed5db508326"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
+name = "round-codec"
+version = "0.1.0"
+dependencies = [
+ "codecs-core",
+ "codecs-core-wasm",
+ "serde",
+]
+
+[[package]]
+name = "running-standardize-codec"
+version = "0.1.0"
+dependencies = [
+ "codecs-core",
+ "codecs-core-wasm",
+ "num-traits",
+ "rolling-stats",
+ "serde",
+]
+
+[[package]]
 name = "rust_decimal"
 version = "1.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1790d1c4c0ca81211399e0e0af16333276f375209e71a37b67698a373db5b47a"
 dependencies = [
  "arrayvec",
  "borsh",
@@ -2083,17 +2147,17 @@
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
@@ -2123,17 +2187,17 @@
 checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-name"
 version = "0.2.1"
@@ -2152,28 +2216,28 @@
  "once_cell",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2184,21 +2248,21 @@
 dependencies = [
  "itoa",
  "serde",
 ]
 
 [[package]]
 name = "serde_repr"
-version = "0.1.18"
+version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b2e6b945e9d3df726b65d6ee24060aff8e3533d431f677a9695db04eff9dfdb"
+checksum = "6c64451ba24fc7a6a2d60fc75dd9c83c90903b19028d4eff35e88fc1e86564e9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "serde_spanned"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eb3622f419d1296904700073ea6cc23ad690adbd66f13ea683df73298736f0c1"
@@ -2231,28 +2295,39 @@
 dependencies = [
  "libc",
  "signal-hook-registry",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
+name = "simple_logger"
+version = "4.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e7e46c8c90251d47d08b28b8a419ffb4aede0f87c2eea95e17d1d5bacbf3ef1"
+dependencies = [
+ "colored",
+ "log",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "siphasher"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56199f7ddabf13fe5074ce809e7d3f42b42ae711800501b5b16ea82ad029c39d"
 
 [[package]]
 name = "slab"
@@ -2300,34 +2375,34 @@
 name = "stable_deref_trait"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8f112729512f8e442d81f95a8a7ddf2b7c6b8a1a6f509a95864142b30cab2d3"
 
 [[package]]
 name = "strsim"
-version = "0.11.0"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ee073c9e4cd00e28217186dbe12796d692868f432bf2e97ee73bed0c56dfa01"
+checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
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
 name = "syn"
-version = "2.0.55"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2335,21 +2410,21 @@
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1329189c02ff984e9736652b1631330da25eaa6bc639089ed4915d25446cbe7b"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "sz3"
 version = "0.1.0+3.1.5.3"
-source = "git+https://github.com/juntyr/sz3-rs.git?rev=475d6e0#475d6e0d1b0a0c94b7647bc96eeff4ac79bc16a8"
+source = "git+https://github.com/juntyr/sz3-rs.git?rev=37622dd#37622ddca12b005f0e20d89ffb6fd6573efe57e0"
 dependencies = [
  "sz3-sys",
  "thiserror",
 ]
 
 [[package]]
 name = "sz3-codec"
@@ -2362,15 +2437,15 @@
  "sz3",
  "zstd-sys",
 ]
 
 [[package]]
 name = "sz3-sys"
 version = "0.1.0+SZ3-3.1.5.3"
-source = "git+https://github.com/juntyr/sz3-rs.git?rev=475d6e0#475d6e0d1b0a0c94b7647bc96eeff4ac79bc16a8"
+source = "git+https://github.com/juntyr/sz3-rs.git?rev=37622dd#37622ddca12b005f0e20d89ffb6fd6573efe57e0"
 dependencies = [
  "bindgen 0.68.1",
  "cc",
  "zstd-sys",
 ]
 
 [[package]]
@@ -2414,30 +2489,30 @@
 checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
@@ -2466,15 +2541,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e9dd1545e8208b4a5af1aa9bbd0b4cf7e9ea08fabc5d0a5c67fcaafa17433aa3"
 dependencies = [
  "indexmap 2.2.6",
  "serde",
  "serde_spanned",
  "toml_datetime",
- "toml_edit 0.22.9",
+ "toml_edit 0.22.12",
 ]
 
 [[package]]
 name = "toml_datetime"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
@@ -2491,32 +2566,26 @@
  "indexmap 2.2.6",
  "toml_datetime",
  "winnow 0.5.40",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.22.9"
+version = "0.22.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e40bb779c5187258fd7aad0eb68cb8706a0a81fa712fbea808ab43c4b8374c4"
+checksum = "d3328d4f68a705b2a4498da1d580585d39a6510f98318a2cec3018a7ec61ddef"
 dependencies = [
  "indexmap 2.2.6",
  "serde",
  "serde_spanned",
  "toml_datetime",
- "winnow 0.6.5",
+ "winnow 0.6.6",
 ]
 
 [[package]]
-name = "topological-sort"
-version = "0.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea68304e134ecd095ac6c3574494fc62b909f416c4fca77e440530221e549d3d"
-
-[[package]]
 name = "twofloat"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f50e81cdb4bbf8e77982b0fb55b3956fd9490d4a3fc172234b393ade7d928cc5"
 dependencies = [
  "hexf",
  "libm",
@@ -2553,34 +2622,28 @@
 [[package]]
 name = "unicode-segmentation"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
 
 [[package]]
-name = "unicode-width"
-version = "0.1.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
-
-[[package]]
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
 [[package]]
 name = "uniform-noise-codec"
 version = "0.1.0"
 dependencies = [
  "codecs-core",
  "codecs-core-wasm",
  "rand",
- "rand_chacha",
  "serde",
+ "wyhash",
 ]
 
 [[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
@@ -2633,71 +2696,95 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "virtual-wasi-build"
 version = "0.1.0"
 dependencies = [
- "wit-component 0.202.0",
+ "virtual-wasi-cli",
+ "virtual-wasi-clocks",
+ "virtual-wasi-filesystem",
+ "virtual-wasi-io",
+ "virtual-wasi-random",
+ "wit-component 0.205.0",
 ]
 
 [[package]]
 name = "virtual-wasi-cli"
 version = "0.1.0"
 dependencies = [
  "wit-bindgen",
+ "wit-deps",
 ]
 
 [[package]]
 name = "virtual-wasi-clocks"
 version = "0.1.0"
 dependencies = [
  "wit-bindgen",
+ "wit-deps",
 ]
 
 [[package]]
 name = "virtual-wasi-filesystem"
 version = "0.1.0"
 dependencies = [
  "wit-bindgen",
+ "wit-deps",
 ]
 
 [[package]]
 name = "virtual-wasi-io"
 version = "0.1.0"
 dependencies = [
  "wit-bindgen",
+ "wit-deps",
 ]
 
 [[package]]
 name = "virtual-wasi-random"
 version = "0.1.0"
 dependencies = [
  "rand_core",
  "rand_pcg",
  "wit-bindgen",
+ "wit-deps",
 ]
 
 [[package]]
-name = "wac-parser"
+name = "wac-graph"
 version = "0.1.0"
-source = "git+https://github.com/peterhuene/wac.git?rev=7b2f728#7b2f7283d3b3044419eafbc5c82d9877d8b0dc60"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0590b997892dc9d7e19884e7a1525263aec6069094775bd5f933858770e045f8"
 dependencies = [
  "anyhow",
  "id-arena",
  "indexmap 2.2.6",
  "log",
- "logos",
- "miette",
+ "petgraph",
  "semver",
- "serde",
  "thiserror",
- "wasm-encoder 0.201.0",
- "wasm-metadata 0.201.0",
- "wasmparser 0.201.0",
+ "wac-types",
+ "wasm-encoder 0.202.0",
+ "wasm-metadata 0.202.0",
+ "wasmparser 0.202.0",
+]
+
+[[package]]
+name = "wac-types"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "670f97b1f3b730df47e4c914e78b5ca0d140ed5656203bb7525bf3684c4616f4"
+dependencies = [
+ "anyhow",
+ "id-arena",
+ "indexmap 2.2.6",
+ "semver",
+ "wasm-encoder 0.202.0",
+ "wasmparser 0.202.0",
 ]
 
 [[package]]
 name = "walrus"
 version = "0.20.3"
 source = "git+https://github.com/rustwasm/walrus.git?rev=4efdb5c#4efdb5c8951a83deb64d02a8822f9442948a6401"
 dependencies = [
@@ -2715,24 +2802,34 @@
 name = "walrus-macro"
 version = "0.19.0"
 source = "git+https://github.com/rustwasm/walrus.git?rev=4efdb5c#4efdb5c8951a83deb64d02a8822f9442948a6401"
 dependencies = [
  "heck 0.3.3",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
+name = "wasi-logger"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "90ea08d42625ef5ef0cfec4451e9b74f14c39f5fa2234bbdbe911962703f5e7c"
+dependencies = [
+ "log",
+ "wit-bindgen",
+]
+
+[[package]]
 name = "wasm-bindgen"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
@@ -2745,15 +2842,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2767,15 +2864,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -2815,14 +2912,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfd106365a7f5f7aa3c1916a98cbb3ad477f5ff96ddb130285a91c6e7429e67a"
 dependencies = [
  "leb128",
 ]
 
 [[package]]
+name = "wasm-encoder"
+version = "0.205.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "90e95b3563d164f33c1cfb0a7efbd5940c37710019be10cd09f800fdec8b0e5c"
+dependencies = [
+ "leb128",
+]
+
+[[package]]
 name = "wasm-metadata"
 version = "0.200.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c31b8cc0c21f46d55b0aaa419cacce1eadcf28eaebd0e1488d6a6313ee71a586"
 dependencies = [
  "anyhow",
  "indexmap 2.2.6",
@@ -2832,73 +2938,71 @@
  "spdx",
  "wasm-encoder 0.200.0",
  "wasmparser 0.200.0",
 ]
 
 [[package]]
 name = "wasm-metadata"
-version = "0.201.0"
+version = "0.202.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fd83062c17b9f4985d438603cde0a5e8c5c8198201a6937f778b607924c7da2"
+checksum = "094aea3cb90e09f16ee25a4c0e324b3e8c934e7fd838bfa039aef5352f44a917"
 dependencies = [
  "anyhow",
  "indexmap 2.2.6",
  "serde",
  "serde_derive",
  "serde_json",
  "spdx",
- "wasm-encoder 0.201.0",
- "wasmparser 0.201.0",
+ "wasm-encoder 0.202.0",
+ "wasmparser 0.202.0",
 ]
 
 [[package]]
 name = "wasm-metadata"
-version = "0.202.0"
+version = "0.205.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "094aea3cb90e09f16ee25a4c0e324b3e8c934e7fd838bfa039aef5352f44a917"
+checksum = "e9855ad6dd4d099fa8505f01fb0b84c7e3efd5f555207329e3ad938d5f394fe7"
 dependencies = [
  "anyhow",
  "indexmap 2.2.6",
  "serde",
  "serde_derive",
  "serde_json",
  "spdx",
- "wasm-encoder 0.202.0",
- "wasmparser 0.202.0",
+ "wasm-encoder 0.205.0",
+ "wasmparser 0.205.0",
 ]
 
 [[package]]
 name = "wasm_component_layer"
 version = "0.1.16"
-source = "git+https://github.com/juntyr/wasm_component_layer.git?rev=0d6d5e5#0d6d5e5d5a261a88756f36fb0d1da3377a6b17a3"
+source = "git+https://github.com/juntyr/wasm_component_layer.git?rev=6667c30#6667c3040b4b88d160fd52eb3fec040a54a89544"
 dependencies = [
  "anyhow",
  "bytemuck",
  "fxhash",
  "id-arena",
  "ref-cast",
  "semver",
  "slab",
  "wasm_runtime_layer",
- "wasmtime-environ",
+ "wasmtime-environ 19.0.2",
  "wit-component 0.200.0",
  "wit-parser 0.200.0",
 ]
 
 [[package]]
 name = "wasm_runtime_layer"
 version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8780c443079ea2ac14ed85f168f95e0854758d780909f242d5db4e6bd41c83b"
+source = "git+https://github.com/juntyr/wasm_runtime_layer.git?rev=d8ea0c5#d8ea0c55b8c91b8f1487f8b29e05d227a17b1d74"
 dependencies = [
  "anyhow",
  "fxhash",
  "ref-cast",
  "smallvec",
- "wasmtime",
 ]
 
 [[package]]
 name = "wasmparser"
 version = "0.100.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "64b20236ab624147dfbb62cf12a19aaf66af0e41b8398838b66e997d07d269d4"
@@ -2948,28 +3052,49 @@
 dependencies = [
  "bitflags 2.5.0",
  "indexmap 2.2.6",
  "semver",
 ]
 
 [[package]]
+name = "wasmparser"
+version = "0.205.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1d457bb52804242e09d55a306e53ddbc65d1d29ed83db6a4eea3ed412ee0cfdf"
+dependencies = [
+ "bitflags 2.5.0",
+ "indexmap 2.2.6",
+ "semver",
+]
+
+[[package]]
 name = "wasmprinter"
 version = "0.2.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60e73986a6b7fdfedb7c5bf9e7eb71135486507c8fbc4c0c42cffcb6532988b7"
 dependencies = [
  "anyhow",
  "wasmparser 0.121.2",
 ]
 
 [[package]]
+name = "wasmprinter"
+version = "0.201.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a67e66da702706ba08729a78e3c0079085f6bfcb1a62e4799e97bbf728c2c265"
+dependencies = [
+ "anyhow",
+ "wasmparser 0.201.0",
+]
+
+[[package]]
 name = "wasmtime"
-version = "18.0.3"
+version = "18.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8106d7d22d63d1bcb940e22dcc7b03e46f0fc8bfbaf2fd7b6cb8f448f9449774"
+checksum = "69472708b96ee90579a482bdbb908ce97e53a9e5ebbcab59cc29c3977bcab512"
 dependencies = [
  "anyhow",
  "bincode",
  "bumpalo",
  "cfg-if",
  "encoding_rs",
  "gimli 0.28.1",
@@ -2983,37 +3108,37 @@
  "serde",
  "serde_derive",
  "serde_json",
  "target-lexicon",
  "wasmparser 0.121.2",
  "wasmtime-cache",
  "wasmtime-component-macro",
- "wasmtime-component-util",
+ "wasmtime-component-util 18.0.4",
  "wasmtime-cranelift",
- "wasmtime-environ",
+ "wasmtime-environ 18.0.4",
  "wasmtime-jit-icache-coherence",
  "wasmtime-runtime",
  "wasmtime-winch",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "wasmtime-asm-macros"
-version = "18.0.3"
+version = "18.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3b0cf02cea951ace34ee3b0e64b7f446c3519d1c95ad75bc5330f405e275ee8f"
+checksum = "86292d6a9bf30c669582a40c4a4b8e0b8640e951f3635ee8e0acf7f87809961e"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "wasmtime-cache"
-version = "18.0.3"
+version = "18.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3249204a71d728d53fb3eea18afd0473f87e520445707a4d567ac4da0bb3eb5d"
+checksum = "8a180017db1233c902b992fea9484640d265f2fedf03db60eed57894cb2effcc"
 dependencies = [
  "anyhow",
  "base64",
  "bincode",
  "directories-next",
  "log",
  "rustix",
@@ -3023,114 +3148,144 @@
  "toml 0.5.11",
  "windows-sys 0.52.0",
  "zstd 0.11.2+zstd.1.5.2",
 ]
 
 [[package]]
 name = "wasmtime-component-macro"
-version = "18.0.3"
+version = "18.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d3786c0531565ec6c9852c0e46299f06cb6e4b58d36e30f3c234cfa69bde376"
+checksum = "dc6aca484581f9651886dca45f9dea893e105713b58623d14b06c56d8fe3f3f1"
 dependencies = [
  "anyhow",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
- "wasmtime-component-util",
+ "syn 2.0.60",
+ "wasmtime-component-util 18.0.4",
  "wasmtime-wit-bindgen",
  "wit-parser 0.13.2",
 ]
 
 [[package]]
 name = "wasmtime-component-util"
-version = "18.0.3"
+version = "18.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81eae2ec98027ee0b3950da83bc320120a23087ac4d39b3d59201cb5ebf52777"
+checksum = "0aa907cc97ad039c43f98525d772f4841c2ce69a0c11eeec2a3a9c77fc730e87"
+
+[[package]]
+name = "wasmtime-component-util"
+version = "19.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0dd17dc1ebc0b28fd24b6b9d07638f55b82ae908918ff08fd221f8b0fefa9125"
 
 [[package]]
 name = "wasmtime-cranelift"
-version = "18.0.3"
+version = "18.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "595abdb067acdc812ab0f21d8d46d5aa4022392aa7c3e0632c20bff9ec49ffb4"
+checksum = "b57d58e220ae223855c5d030ef20753377bc716d0c81b34c1fe74c9f44268774"
 dependencies = [
  "anyhow",
  "cfg-if",
  "cranelift-codegen",
  "cranelift-control",
- "cranelift-entity",
+ "cranelift-entity 0.105.4",
  "cranelift-frontend",
  "cranelift-native",
  "cranelift-wasm",
  "gimli 0.28.1",
  "log",
  "object",
  "target-lexicon",
  "thiserror",
  "wasmparser 0.121.2",
  "wasmtime-cranelift-shared",
- "wasmtime-environ",
+ "wasmtime-environ 18.0.4",
  "wasmtime-versioned-export-macros",
 ]
 
 [[package]]
 name = "wasmtime-cranelift-shared"
-version = "18.0.3"
+version = "18.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e8c24c1fdea167b992d82ebe76471fd1cbe7b0b406bc72f9250f86353000134e"
+checksum = "1ba2cfdfdbde42f0f3baeddb62f3555524dee9f836c96da8d466e299f75f5eee"
 dependencies = [
  "anyhow",
  "cranelift-codegen",
  "cranelift-control",
  "cranelift-native",
  "gimli 0.28.1",
  "object",
  "target-lexicon",
- "wasmtime-environ",
+ "wasmtime-environ 18.0.4",
 ]
 
 [[package]]
 name = "wasmtime-environ"
-version = "18.0.3"
+version = "18.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3279d510005358141550d8a90a5fc989d7e81748e5759d582fe6bfdcbf074a04"
+checksum = "abbf3075d9ee7eb1263dc67949aced64d0f0bf27be8098d34d8e5826cf0ff0f2"
 dependencies = [
  "anyhow",
  "bincode",
- "cranelift-entity",
+ "cranelift-entity 0.105.4",
  "gimli 0.28.1",
  "indexmap 2.2.6",
  "log",
  "object",
  "serde",
  "serde_derive",
  "target-lexicon",
  "thiserror",
  "wasm-encoder 0.41.2",
  "wasmparser 0.121.2",
- "wasmprinter",
- "wasmtime-component-util",
- "wasmtime-types",
+ "wasmprinter 0.2.80",
+ "wasmtime-component-util 18.0.4",
+ "wasmtime-types 18.0.4",
+]
+
+[[package]]
+name = "wasmtime-environ"
+version = "19.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d7e3f2aa72dbb64c19708646e1ff97650f34e254598b82bad5578ea9c80edd30"
+dependencies = [
+ "anyhow",
+ "bincode",
+ "cranelift-entity 0.106.2",
+ "gimli 0.28.1",
+ "indexmap 2.2.6",
+ "log",
+ "object",
+ "serde",
+ "serde_derive",
+ "target-lexicon",
+ "thiserror",
+ "wasm-encoder 0.201.0",
+ "wasmparser 0.201.0",
+ "wasmprinter 0.201.0",
+ "wasmtime-component-util 19.0.2",
+ "wasmtime-types 19.0.2",
 ]
 
 [[package]]
 name = "wasmtime-jit-icache-coherence"
-version = "18.0.3"
+version = "18.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "866634605089b4632b32226b54aa3670d72e1849f9fc425c7e50b3749c2e6df3"
+checksum = "dacd2aa30fb20fd8cd0eb4e664024a1ab28a02958529fa05bf52117532a098fc"
 dependencies = [
  "cfg-if",
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "wasmtime-runtime"
-version = "18.0.3"
+version = "18.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e11185c88cadf595d228f5ae4ff9b4badbf9ca98dcb37b0310c36e31fa74867f"
+checksum = "d14e97c4bb36d91bcdd194745446d595e67ce8b89916806270fdbee640c747fd"
 dependencies = [
  "anyhow",
  "cc",
  "cfg-if",
  "encoding_rs",
  "indexmap 2.2.6",
  "libc",
@@ -3140,78 +3295,104 @@
  "memoffset",
  "paste",
  "psm",
  "rustix",
  "sptr",
  "wasm-encoder 0.41.2",
  "wasmtime-asm-macros",
- "wasmtime-environ",
+ "wasmtime-environ 18.0.4",
  "wasmtime-versioned-export-macros",
  "wasmtime-wmemcheck",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "wasmtime-types"
-version = "18.0.3"
+version = "18.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f32377cbd827bee06fcb2f6bf97b0477fdcc86888bbe6db7b9cab8e644082e0a"
+checksum = "530b94c627a454d24f520173d3145112d1b807c44c82697a57e1d8e28390cde4"
 dependencies = [
- "cranelift-entity",
+ "cranelift-entity 0.105.4",
  "serde",
  "serde_derive",
  "thiserror",
  "wasmparser 0.121.2",
 ]
 
 [[package]]
+name = "wasmtime-types"
+version = "19.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cebe297aa063136d9d2e5b347c1528868aa43c2c8d0e1eb0eec144567e38fe0f"
+dependencies = [
+ "cranelift-entity 0.106.2",
+ "serde",
+ "serde_derive",
+ "thiserror",
+ "wasmparser 0.201.0",
+]
+
+[[package]]
 name = "wasmtime-versioned-export-macros"
-version = "18.0.3"
+version = "18.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ab8d7566d206c42f8cf1d4ac90c5e40d3582e8eabad9b3b67e9e73c61fc47a1"
+checksum = "5399c175ddba4a471b9da45105dea3493059d52b2d54860eadb0df04c813948d"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "wasmtime-winch"
-version = "18.0.3"
+version = "18.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba5a97bfccc241d1769cef75eb16f472a893982704d5f3c9c71c431c1484344a"
+checksum = "729dff119cfd2e2333504b52db6661e49278314c83276a01d15a2a86e566e614"
 dependencies = [
  "anyhow",
  "cranelift-codegen",
  "gimli 0.28.1",
  "object",
  "target-lexicon",
  "wasmparser 0.121.2",
  "wasmtime-cranelift-shared",
- "wasmtime-environ",
+ "wasmtime-environ 18.0.4",
  "winch-codegen",
 ]
 
 [[package]]
 name = "wasmtime-wit-bindgen"
-version = "18.0.3"
+version = "18.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "faf2c76781a27e07802669f6f0e11eb4441546407eb65be60c3d862200988b92"
+checksum = "6945fc6cfee04ba81016e9723bea77a2b913108e03904a4d901daedf208365f5"
 dependencies = [
  "anyhow",
  "heck 0.4.1",
  "indexmap 2.2.6",
  "wit-parser 0.13.2",
 ]
 
 [[package]]
 name = "wasmtime-wmemcheck"
-version = "18.0.3"
+version = "18.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3847d969bd203b8cd239f89581e52432a0f00b8c5c9bc917be2fccd7542c4f2f"
+checksum = "e1711f429111e782fac0537e0b3eb2ab6f821613cf1ec3013f2a0ff3fde41745"
+
+[[package]]
+name = "wasmtime_runtime_layer"
+version = "18.0.0"
+source = "git+https://github.com/juntyr/wasm_runtime_layer.git?rev=d8ea0c5#d8ea0c55b8c91b8f1487f8b29e05d227a17b1d74"
+dependencies = [
+ "anyhow",
+ "fxhash",
+ "ref-cast",
+ "smallvec",
+ "wasm_runtime_layer",
+ "wasmtime",
+]
 
 [[package]]
 name = "which"
 version = "4.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87ba24419a2078cd2b0f2ede2691b6c66d8e47836da3b6db8265ebad47afbfc7"
 dependencies = [
@@ -3250,26 +3431,26 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "winch-codegen"
-version = "0.16.3"
+version = "0.16.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e0bd4d6cac8d69525d475d0ce1e0801eb6f314d42e764a52bd497ed3cb9c371"
+checksum = "433cafb378ad01cd839974846204f56257ec34fc9d7db309ce1e34f24923fa6a"
 dependencies = [
  "anyhow",
  "cranelift-codegen",
  "gimli 0.28.1",
  "regalloc2",
  "smallvec",
  "target-lexicon",
  "wasmparser 0.121.2",
- "wasmtime-environ",
+ "wasmtime-environ 18.0.4",
 ]
 
 [[package]]
 name = "windows"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
@@ -3288,15 +3469,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -3308,182 +3489,189 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winnow"
 version = "0.5.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winnow"
-version = "0.6.5"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dffa400e67ed5a4dd237983829e66475f0a4a26938c4b04c21baede6262215b8"
+checksum = "f0c976aaaa0e1f90dbb21e9587cdaf1d9679a1cde8875c0d6bd83ab96a208352"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "wit-bindgen"
-version = "0.23.0"
+version = "0.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "041a3276f25dce240b10f5b34d9d490b007f18e8ead05984ae7948b283b4059e"
+checksum = "9fb4e7653763780be47e38f479e9aa83c768aa6a3b2ed086dc2826fdbbb7e7f5"
 dependencies = [
  "wit-bindgen-rt",
  "wit-bindgen-rust-macro",
 ]
 
 [[package]]
 name = "wit-bindgen-core"
-version = "0.23.0"
+version = "0.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0834150cd852e64e1eddcff4fea9524b788161b4111d83a94c9eda715f8f442"
+checksum = "9b67e11c950041849a10828c7600ea62a4077c01e8af72e8593253575428f91b"
 dependencies = [
  "anyhow",
  "wit-parser 0.202.0",
 ]
 
 [[package]]
 name = "wit-bindgen-rt"
-version = "0.23.0"
+version = "0.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6ccd4c6a69667c75474ddb30c36773c5e70cdca099ec2e293005458886ac81b"
+checksum = "3b0780cf7046630ed70f689a098cd8d56c5c3b22f2a7379bbdb088879963ff96"
 dependencies = [
  "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "wit-bindgen-rust"
-version = "0.23.0"
+version = "0.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60620df421d4c787e2660f0159fd58f2ae6998dc42ccf2e09b8d9d96d16885a9"
+checksum = "30acbe8fb708c3a830a33c4cb705df82659bf831b492ec6ca1a17a369cfeeafb"
 dependencies = [
  "anyhow",
  "heck 0.4.1",
  "indexmap 2.2.6",
  "wasm-metadata 0.202.0",
  "wit-bindgen-core",
  "wit-component 0.202.0",
 ]
 
 [[package]]
 name = "wit-bindgen-rust-macro"
-version = "0.23.0"
+version = "0.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96e875e7dd09a0d2acc1a27df6a4b0586288741d940b40a717e2daed3bc3d979"
+checksum = "2b1b06eae85feaecdf9f2854f7cac124e00d5a6e5014bfb02eb1ecdeb5f265b9"
 dependencies = [
  "anyhow",
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
  "wit-bindgen-core",
  "wit-bindgen-rust",
 ]
 
 [[package]]
 name = "wit-component"
 version = "0.200.0"
@@ -3519,14 +3707,37 @@
  "wasm-encoder 0.202.0",
  "wasm-metadata 0.202.0",
  "wasmparser 0.202.0",
  "wit-parser 0.202.0",
 ]
 
 [[package]]
+name = "wit-component"
+version = "0.205.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "74841e17b2c2bfbd8ca8c45190ef85dff1c5e8659f0e2d164802ffc87dfb18c3"
+dependencies = [
+ "anyhow",
+ "bitflags 2.5.0",
+ "indexmap 2.2.6",
+ "log",
+ "serde",
+ "serde_derive",
+ "serde_json",
+ "wasm-encoder 0.205.0",
+ "wasm-metadata 0.205.0",
+ "wasmparser 0.205.0",
+ "wit-parser 0.205.0",
+]
+
+[[package]]
+name = "wit-deps"
+version = "0.1.0"
+
+[[package]]
 name = "wit-parser"
 version = "0.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "316b36a9f0005f5aa4b03c39bc3728d045df136f8c13a73b7db4510dec725e08"
 dependencies = [
  "anyhow",
  "id-arena",
@@ -3572,20 +3783,47 @@
  "serde_derive",
  "serde_json",
  "unicode-xid",
  "wasmparser 0.202.0",
 ]
 
 [[package]]
+name = "wit-parser"
+version = "0.205.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a3db34c7688c161ed7bd1b2f8055dca9fb2c15201db58754e9c48a0805f32e5f"
+dependencies = [
+ "anyhow",
+ "id-arena",
+ "indexmap 2.2.6",
+ "log",
+ "semver",
+ "serde",
+ "serde_derive",
+ "serde_json",
+ "unicode-xid",
+ "wasmparser 0.205.0",
+]
+
+[[package]]
 name = "wobbly"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "10c47ee6b4260f6a7cee6cd6b7a34edf5b3e16ce2f309b5168d6fdb6c0dbbdd6"
 
 [[package]]
+name = "wyhash"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "baf6e163c25e3fac820b4b453185ea2dea3b6a3e0a721d4d23d75bd33734c295"
+dependencies = [
+ "rand_core",
+]
+
+[[package]]
 name = "wyz"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
  "tap",
 ]
@@ -3603,15 +3841,15 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.55",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "zfp-codec"
 version = "0.1.0"
 dependencies = [
  "codecs-core",
```

### Comparing `field-compression-benchmark-0.0.2/Cargo.toml` & `field-compression-benchmark-0.0.3/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,22 +5,23 @@
     "wasi/random",
     "core/benchmark", "core/compressor", "core/dataset", "core/error",
     "core/goodness", "core/measure", "core/model",
     "codecs/build", "codecs/core", "codecs/core-host", "codecs/core-wasm",
     "codecs/frontend",
     "codecs/bit-round", "codecs/bit-transpose", "codecs/identity",
     "codecs/linear-quantize", "codecs/log", "codecs/reinterpret",
-    "codecs/sz3", "codecs/uniform-noise", "codecs/zfp", "codecs/zlib",
-    "codecs/zstd",
+    "codecs/round", "codecs/sz3", "codecs/uniform-noise", "codecs/zfp",
+    "codecs/zlib", "codecs/zstd",
     "fcbench",
+    "utils/wit-deps",
 ]
 
 [workspace.lints.rust]
 unsafe_code = "deny"
-unstable_features = "deny"
+unstable_features = "forbid"
 
 [workspace.lints.clippy]
 complexity = "deny"
 correctness = "deny"
 nursery = "warn"
 pedantic = "warn"
 perf = "deny"
@@ -75,7 +76,11 @@
 vecmap-rs = { version = "0.2", default-features = false, features = ["serde"] }
 
 [lints]
 workspace = true
 
 [package.metadata.cargo-udeps.ignore]
 normal = ["codecs-build"]
+
+[patch.crates-io]
+# FIXME: update once wasm_runtime_layer v0.4.0 has been released
+wasm_runtime_layer = { git = "https://github.com/juntyr/wasm_runtime_layer.git", rev = "d8ea0c5", default-features = false }
```

### Comparing `field-compression-benchmark-0.0.2/LICENSE-APACHE` & `field-compression-benchmark-0.0.3/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/LICENSE-MIT` & `field-compression-benchmark-0.0.3/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/PKG-INFO` & `field-compression-benchmark-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: field-compression-benchmark
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data compression methods and benchmarks for Cli/Met datasets
 Author-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 Maintainer-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `field-compression-benchmark-0.0.2/README.md` & `field-compression-benchmark-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/codecs/bit-round/src/lib.rs` & `field-compression-benchmark-0.0.3/codecs/bit-round/src/lib.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/codecs/bit-transpose/src/lib.rs` & `field-compression-benchmark-0.0.3/codecs/bit-transpose/src/lib.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/codecs/build/build.rs` & `field-compression-benchmark-0.0.3/codecs/build/build.rs`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
     for (crate_name, codec_name) in [
         ("bit-round-codec", "bit-round"),
         ("bit-transpose-codec", "bit-transpose"),
         ("identity-codec", "identity"),
         ("linear-quantize-codec", "linear-quantize"),
         ("log-codec", "log"),
         ("reinterpret-codec", "reinterpret"),
+        ("round-codec", "round"),
+        ("running-standardize-codec", "running-standardize"),
         ("sz3-codec", "sz3"),
         ("uniform-noise-codec", "uniform-noise"),
         ("zfp-codec", "zfp"),
         ("zlib-codec", "zlib"),
         ("zstd-codec", "zstd"),
     ] {
         let wasm = build_wasm_codec(&wasi_sdk_path, &target_dir, crate_name)?;
```

### Comparing `field-compression-benchmark-0.0.2/codecs/core/src/buffer.rs` & `field-compression-benchmark-0.0.3/codecs/core/src/buffer.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-use alloc::{vec, vec::Vec};
-
 use crate::{
     map::HigherOrderMap,
     map_with,
     slice::BufferSlice,
+    slice_mut::BufferSliceMut,
     ty::{BufferTy, BufferTyBound},
 };
 
 #[allow(clippy::module_name_repetitions)]
 #[non_exhaustive]
 pub enum BufferVec<B: OwnedBuffer = VecBuffer> {
     U8(B::Buffer<u8>),
@@ -128,25 +127,18 @@
             Self::I64(b) => map.map::<i64>(b),
             Self::F32(b) => map.map::<f32>(b),
             Self::F64(b) => map.map::<f64>(b),
         }
     }
 
     #[must_use]
-    pub fn as_bytes_mut(&mut self) -> &mut [u8] {
-        self.map_ref_mut(map_with!(for<'a, T> |v: &'a mut [T]| -> &'a mut [u8] {
-            let (data, len) = (v.as_mut_ptr().cast::<u8>(), core::mem::size_of_val(v));
-            #[allow(unsafe_code)]
-            // Safety:
-            // - we have a mutable reference to self
-            // - all slice element types can be modified on a per-byte basis
-            unsafe {
-                core::slice::from_raw_parts_mut(data, len)
-            }
-        }))
+    pub fn as_slice_mut(&mut self) -> BufferSliceMut {
+        self.map_ref_mut(map_with!(
+            for<'a, T> |v: &'a mut [T]| -> BufferSliceMut<'a> { BufferSliceMut::from(v) }
+        ))
     }
 }
 
 impl BufferVec<VecBuffer> {
     #[must_use]
     pub fn zeros_with_ty_len(ty: BufferTy, len: usize) -> Self {
         ty.map(
```

### Comparing `field-compression-benchmark-0.0.2/codecs/core/src/lib.rs` & `field-compression-benchmark-0.0.3/codecs/core/src/lib.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 #![allow(clippy::missing_errors_doc)]
-#![no_std]
 
 #[doc(hidden)]
-pub extern crate alloc;
-#[doc(hidden)]
 pub extern crate core;
 
-use alloc::{string::String, vec::Vec};
-
 mod buffer;
 mod slice;
+mod slice_mut;
 mod ty;
 
 #[doc(hidden)]
 pub mod casts;
 pub mod map;
 
 pub use crate::{
     buffer::{BufferVec, OwnedBuffer, OwnedBufferImpl, VecBuffer},
     slice::BufferSlice,
+    slice_mut::BufferSliceMut,
     ty::{BufferTy, BufferTyBound},
 };
 
 pub trait Codec: 'static + Clone {
     const CODEC_ID: &'static str;
 
     type EncodedBuffer: OwnedBuffer;
```

### Comparing `field-compression-benchmark-0.0.2/codecs/core/src/map.rs` & `field-compression-benchmark-0.0.3/codecs/core/src/map.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/codecs/core/src/slice.rs` & `field-compression-benchmark-0.0.3/codecs/core/src/slice.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-use alloc::vec::Vec;
-use core::alloc::Layout;
+use std::alloc::Layout;
 
 use crate::{
     buffer::BufferVec,
     map::HigherOrderMap,
     map_with,
     ty::{BufferTy, BufferTyBound},
 };
```

### Comparing `field-compression-benchmark-0.0.2/codecs/core-host/Cargo.toml` & `field-compression-benchmark-0.0.3/codecs/core-host/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 [dependencies]
 anyhow = { version = "1.0", default-features = false }
 codecs-core = { path = "../core", default-features = false }
 core-error = { path = "../../core/error", default-features = false }
 semver = { version = "1.0", default-features = false }
 serde = { version = "1.0", default-features = false, features = ["alloc", "derive"] }
 thiserror = { version = "1.0", default-features = false }
-wasm_component_layer = { git = "https://github.com/juntyr/wasm_component_layer.git", rev = "0d6d5e5", version = "0.1", default-features = false }
+wasm_component_layer = { git = "https://github.com/juntyr/wasm_component_layer.git", rev = "6667c30", version = "0.1", default-features = false }
 wasm_runtime_layer = { version = "0.3", default-features = false }
 
 [lints]
 workspace = true
```

### Comparing `field-compression-benchmark-0.0.2/codecs/core-host/src/codec.rs` & `field-compression-benchmark-0.0.3/codecs/core-host/src/codec.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,243 @@
-use std::{borrow::BorrowMut, marker::PhantomData};
+use std::borrow::BorrowMut;
 
 use wasm_component_layer::{
-    List, ListType, RecordType, ResourceOwn, Value, ValueType, Variant, VariantCase, VariantType,
+    List, ListType, Record, RecordType, ResourceOwn, Value, ValueType, Variant, VariantCase,
+    VariantType,
 };
-use wasm_runtime_layer::backend::WasmEngine;
 
-use codecs_core::{casts::u32_as_usize, BufferSlice, ShapedBuffer, VecBuffer};
+use codecs_core::{casts::u32_as_usize, BufferSlice, BufferSliceMut, ShapedBuffer, VecBuffer};
 use core_error::LocationError;
 
 use crate::{plugin::CodecPlugin, Error};
 
 #[allow(clippy::module_name_repetitions)]
-pub struct WasmCodec<E: WasmEngine, P: BorrowMut<CodecPlugin<E>>> {
+pub struct WasmCodec<P: BorrowMut<CodecPlugin> = CodecPlugin> {
     pub(crate) resource: ResourceOwn,
     pub(crate) plugin: P,
     pub(crate) instruction_counter: u64,
-    pub(crate) _marker: PhantomData<E>,
 }
 
-impl<E: WasmEngine, P: BorrowMut<CodecPlugin<E>>> WasmCodec<E, P> {
+impl<P: BorrowMut<CodecPlugin>> WasmCodec<P> {
     #[must_use]
     pub const fn instruction_counter(&self) -> u64 {
         self.instruction_counter
     }
 
-    #[allow(clippy::type_complexity, clippy::too_many_lines)]
-    fn process(
+    #[allow(clippy::type_complexity)]
+    pub fn encode(
+        &mut self,
+        buf: BufferSlice,
+        shape: &[usize],
+    ) -> Result<Result<ShapedBuffer<VecBuffer>, String>, LocationError<Error>> {
+        self.process(
+            buf,
+            shape,
+            |plugin, arguments, results| plugin.ctx.call_func(&plugin.encode, arguments, results),
+            |buffer, shape| {
+                Ok(ShapedBuffer {
+                    buffer: buffer.to_vec(),
+                    shape,
+                })
+            },
+        )
+    }
+
+    #[allow(clippy::type_complexity)]
+    pub fn encode_into(
+        &mut self,
+        buf: BufferSlice,
+        shape: &[usize],
+        mut buf_out: BufferSliceMut,
+        shape_out: &[usize],
+    ) -> Result<Result<(), String>, LocationError<Error>> {
+        self.process(
+            buf,
+            shape,
+            |plugin, arguments, results| plugin.ctx.call_func(&plugin.encode, arguments, results),
+            |buffer, shape| {
+                if shape != shape_out {
+                    return Err(LocationError::from2(anyhow::Error::msg(format!(
+                        "encode result has shape {shape:?} but expected {shape_out:?}"
+                    ))));
+                }
+                buf_out
+                    .copy_from(buffer)
+                    .map_err(anyhow::Error::new)
+                    .map_err(LocationError::from2)?;
+                Ok(())
+            },
+        )
+    }
+
+    #[allow(clippy::type_complexity)]
+    pub fn decode(
         &mut self,
         buf: BufferSlice,
         shape: &[usize],
-        process: impl FnOnce(&mut CodecPlugin<E>, &[Value], &mut [Value]) -> anyhow::Result<()>,
     ) -> Result<Result<ShapedBuffer<VecBuffer>, String>, LocationError<Error>> {
-        let plugin: &mut CodecPlugin<E> = self.plugin.borrow_mut();
+        self.process(
+            buf,
+            shape,
+            |plugin, arguments, results| plugin.ctx.call_func(&plugin.decode, arguments, results),
+            |buffer, shape| {
+                Ok(ShapedBuffer {
+                    buffer: buffer.to_vec(),
+                    shape,
+                })
+            },
+        )
+    }
 
-        let resource = self
-            .resource
-            .borrow(&mut plugin.ctx)
+    #[allow(clippy::type_complexity)]
+    pub fn decode_into(
+        &mut self,
+        buf: BufferSlice,
+        shape: &[usize],
+        mut buf_out: BufferSliceMut,
+        shape_out: &[usize],
+    ) -> Result<Result<(), String>, LocationError<Error>> {
+        self.process(
+            buf,
+            shape,
+            |plugin, arguments, results| plugin.ctx.call_func(&plugin.decode, arguments, results),
+            |buffer, shape| {
+                if shape != shape_out {
+                    return Err(LocationError::from2(anyhow::Error::msg(format!(
+                        "decode result has shape {shape:?} but expected {shape_out:?}"
+                    ))));
+                }
+                buf_out
+                    .copy_from(buffer)
+                    .map_err(anyhow::Error::new)
+                    .map_err(LocationError::from2)?;
+                Ok(())
+            },
+        )
+    }
+
+    pub fn get_config(&mut self) -> Result<Result<String, String>, LocationError<Error>> {
+        let plugin: &mut CodecPlugin = self.plugin.borrow_mut();
+
+        let resource = plugin
+            .ctx
+            .borrow_resource(&self.resource)
             .map_err(LocationError::from2)?;
 
+        let arg = Value::Borrow(resource);
+        let mut result = Value::U8(0);
+
+        plugin
+            .ctx
+            .call_func(
+                &plugin.get_config,
+                std::slice::from_ref(&arg),
+                std::slice::from_mut(&mut result),
+            )
+            .map_err(LocationError::from2)?;
+
+        match result {
+            Value::Result(result) => match &*result {
+                Ok(Some(Value::String(config))) => Ok(Ok(String::from(&**config))),
+                Err(Some(Value::String(err))) => Ok(Err(String::from(&**err))),
+                result => Err(LocationError::from2(anyhow::Error::msg(format!(
+                    "unexpected get-config result value {result:?}"
+                )))),
+            },
+            value => Err(LocationError::from2(anyhow::Error::msg(format!(
+                "unexpected get-config result value {value:?}"
+            )))),
+        }
+    }
+
+    pub fn drop(mut self) -> Result<(), LocationError<Error>> {
+        let plugin: &mut CodecPlugin = self.plugin.borrow_mut();
+
+        let result = plugin
+            .ctx
+            .drop_resource(&self.resource)
+            .map_err(LocationError::from2);
+
+        // We need to forget here instead of using ManuallyDrop since we need
+        //  both a mutable borrow to self.plugin and an immutable borrow to
+        //  self.resource at the same time
+        std::mem::forget(self);
+
+        result
+    }
+}
+
+impl<P: BorrowMut<CodecPlugin>> WasmCodec<P> {
+    #[allow(clippy::type_complexity)]
+    fn process<O>(
+        &mut self,
+        buf: BufferSlice,
+        shape: &[usize],
+        process: impl FnOnce(&mut CodecPlugin, &[Value], &mut [Value]) -> anyhow::Result<()>,
+        with_result: impl for<'a> FnOnce(BufferSlice<'a>, Vec<usize>) -> Result<O, LocationError<Error>>,
+    ) -> Result<Result<O, String>, LocationError<Error>> {
+        let plugin: &mut CodecPlugin = self.plugin.borrow_mut();
+
+        let resource = plugin
+            .ctx
+            .borrow_resource(&self.resource)
+            .map_err(LocationError::from2)?;
+
+        let buffer_ty = Self::buffer_ty()?;
+        let buffer = Self::buffer_slice_into_wasm_variant(buf, buffer_ty.clone())?;
+        let shape = Self::shape_into_wasm_list(shape)?;
+
+        let instruction_counter_pre = plugin
+            .ctx
+            .call_typed_u64_func(&plugin.instruction_counter)
+            .map_err(LocationError::from2)?;
+
+        let mut result = Value::U8(0);
+
+        process(
+            plugin,
+            &[
+                Value::Borrow(resource),
+                Value::Variant(buffer),
+                Value::List(shape),
+            ],
+            std::slice::from_mut(&mut result),
+        )
+        .map_err(LocationError::from2)?;
+
+        let instruction_counter_post = plugin
+            .ctx
+            .call_typed_u64_func(&plugin.instruction_counter)
+            .map_err(LocationError::from2)?;
+        self.instruction_counter += instruction_counter_post - instruction_counter_pre;
+
+        match result {
+            Value::Result(result) => match &*result {
+                Ok(Some(Value::Record(record)))
+                    if record.ty() == Self::shaped_buffer_ty(buffer_ty)? =>
+                {
+                    Self::with_buffer_slice_from_wasm_record(record, |buffer| {
+                        Ok(Ok(with_result(
+                            buffer,
+                            Self::shape_from_wasm_record(record)?,
+                        )?))
+                    })
+                },
+                Err(Some(Value::String(err))) => Ok(Err(String::from(&**err))),
+                result => Err(LocationError::from2(anyhow::Error::msg(format!(
+                    "unexpected process result value {result:?}"
+                )))),
+            },
+            value => Err(LocationError::from2(anyhow::Error::msg(format!(
+                "unexpected process result value {value:?}"
+            )))),
+        }
+    }
+
+    fn buffer_ty() -> Result<VariantType, LocationError<Error>> {
         let buffer_ty = VariantType::new(
             None,
             [
                 VariantCase::new("u8", Some(ValueType::List(ListType::new(ValueType::U8)))),
                 VariantCase::new("u16", Some(ValueType::List(ListType::new(ValueType::U16)))),
                 VariantCase::new("u32", Some(ValueType::List(ListType::new(ValueType::U32)))),
                 VariantCase::new("u64", Some(ValueType::List(ListType::new(ValueType::U64)))),
@@ -51,23 +247,34 @@
                 VariantCase::new("i64", Some(ValueType::List(ListType::new(ValueType::S64)))),
                 VariantCase::new("f32", Some(ValueType::List(ListType::new(ValueType::F32)))),
                 VariantCase::new("f64", Some(ValueType::List(ListType::new(ValueType::F64)))),
             ],
         )
         .map_err(LocationError::from2)?;
 
+        Ok(buffer_ty)
+    }
+
+    fn shaped_buffer_ty(buffer_ty: VariantType) -> Result<RecordType, LocationError<Error>> {
         let shaped_buffer_ty = RecordType::new(
             None,
             [
-                ("buffer", ValueType::Variant(buffer_ty.clone())),
+                ("buffer", ValueType::Variant(buffer_ty)),
                 ("shape", ValueType::List(ListType::new(ValueType::U32))),
             ],
         )
         .map_err(LocationError::from2)?;
 
+        Ok(shaped_buffer_ty)
+    }
+
+    fn buffer_slice_into_wasm_variant(
+        buf: BufferSlice,
+        buffer_ty: VariantType,
+    ) -> Result<Variant, LocationError<Error>> {
         let buffer = match buf {
             BufferSlice::U8(buf) => Variant::new(buffer_ty, 0, Some(Value::List(List::from(buf)))),
             BufferSlice::U16(buf) => Variant::new(buffer_ty, 1, Some(Value::List(List::from(buf)))),
             BufferSlice::U32(buf) => Variant::new(buffer_ty, 2, Some(Value::List(List::from(buf)))),
             BufferSlice::U64(buf) => Variant::new(buffer_ty, 3, Some(Value::List(List::from(buf)))),
             BufferSlice::I8(buf) => Variant::new(buffer_ty, 4, Some(Value::List(List::from(buf)))),
             BufferSlice::I16(buf) => Variant::new(buffer_ty, 5, Some(Value::List(List::from(buf)))),
@@ -78,197 +285,81 @@
             buf => Err(anyhow::Error::msg(format!(
                 "unknown buffer type {}",
                 buf.ty()
             ))),
         }
         .map_err(LocationError::from2)?;
 
+        Ok(buffer)
+    }
+
+    fn shape_into_wasm_list(shape: &[usize]) -> Result<List, LocationError<Error>> {
         let shape = shape
             .iter()
             .map(|s| u32::try_from(*s).map_err(anyhow::Error::new))
             .collect::<Result<Vec<_>, _>>()
             .map_err(LocationError::from2)?;
-
-        let instruction_counter_pre = plugin
-            .instruction_counter
-            .call(&mut plugin.ctx, ())
-            .map_err(LocationError::from2)?;
-
-        let args = [
-            Value::Borrow(resource),
-            Value::Variant(buffer),
-            Value::List(List::from(shape.as_slice())),
-        ];
-        let mut result = Value::U8(0);
-
-        process(plugin, &args, std::slice::from_mut(&mut result)).map_err(LocationError::from2)?;
-
-        let instruction_counter_post = plugin
-            .instruction_counter
-            .call(&mut plugin.ctx, ())
-            .map_err(LocationError::from2)?;
-
-        self.instruction_counter += instruction_counter_post - instruction_counter_pre;
-
-        match result {
-            Value::Result(result) => match &*result {
-                Ok(Some(Value::Record(record))) if record.ty() == shaped_buffer_ty => {
-                    let Some(Value::Variant(variant)) = record.field("buffer") else {
-                        return Err(LocationError::from2(anyhow::Error::msg(format!(
-                            "process result record {record:?} is missing buffer field"
-                        ))));
-                    };
-                    let buffer = match (variant.discriminant(), variant.value()) {
-                        (0, Some(Value::List(list))) => {
-                            BufferSlice::from(list.typed::<u8>().map_err(LocationError::from2)?)
-                                .to_vec()
-                        },
-                        (1, Some(Value::List(list))) => {
-                            BufferSlice::from(list.typed::<u16>().map_err(LocationError::from2)?)
-                                .to_vec()
-                        },
-                        (2, Some(Value::List(list))) => {
-                            BufferSlice::from(list.typed::<u32>().map_err(LocationError::from2)?)
-                                .to_vec()
-                        },
-                        (3, Some(Value::List(list))) => {
-                            BufferSlice::from(list.typed::<u64>().map_err(LocationError::from2)?)
-                                .to_vec()
-                        },
-                        (4, Some(Value::List(list))) => {
-                            BufferSlice::from(list.typed::<i8>().map_err(LocationError::from2)?)
-                                .to_vec()
-                        },
-                        (5, Some(Value::List(list))) => {
-                            BufferSlice::from(list.typed::<i16>().map_err(LocationError::from2)?)
-                                .to_vec()
-                        },
-                        (6, Some(Value::List(list))) => {
-                            BufferSlice::from(list.typed::<i32>().map_err(LocationError::from2)?)
-                                .to_vec()
-                        },
-                        (7, Some(Value::List(list))) => {
-                            BufferSlice::from(list.typed::<i64>().map_err(LocationError::from2)?)
-                                .to_vec()
-                        },
-                        (8, Some(Value::List(list))) => {
-                            BufferSlice::from(list.typed::<f32>().map_err(LocationError::from2)?)
-                                .to_vec()
-                        },
-                        (9, Some(Value::List(list))) => {
-                            BufferSlice::from(list.typed::<f64>().map_err(LocationError::from2)?)
-                                .to_vec()
-                        },
-                        (discriminant, value) => {
-                            return Err(LocationError::from2(anyhow::Error::msg(format!(
-                                "process result buffer has an invalid variant \
-                                 [{discriminant}]:{value:?}"
-                            ))))
-                        },
-                    };
-
-                    let Some(Value::List(shape)) = record.field("shape") else {
-                        return Err(LocationError::from2(anyhow::Error::msg(format!(
-                            "process result record {record:?} is missing shape field"
-                        ))));
-                    };
-                    let shape = shape
-                        .typed::<u32>()
-                        .map_err(LocationError::from2)?
-                        .iter()
-                        .copied()
-                        .map(u32_as_usize)
-                        .collect();
-
-                    Ok(Ok(ShapedBuffer { buffer, shape }))
-                },
-                Err(Some(Value::String(err))) => Ok(Err(String::from(&**err))),
-                result => Err(LocationError::from2(anyhow::Error::msg(format!(
-                    "unexpected process result value {result:?}"
-                )))),
-            },
-            value => Err(LocationError::from2(anyhow::Error::msg(format!(
-                "unexpected process result value {value:?}"
-            )))),
-        }
+        Ok(List::from(shape.as_slice()))
     }
 
-    #[allow(clippy::type_complexity)]
-    pub fn encode(
-        &mut self,
-        buf: BufferSlice,
-        shape: &[usize],
-    ) -> Result<Result<ShapedBuffer<VecBuffer>, String>, LocationError<Error>> {
-        self.process(buf, shape, |plugin, arguments, results| {
-            plugin.encode.call(&mut plugin.ctx, arguments, results)
-        })
-    }
-
-    #[allow(clippy::type_complexity)]
-    pub fn decode(
-        &mut self,
-        buf: BufferSlice,
-        shape: &[usize],
-    ) -> Result<Result<ShapedBuffer<VecBuffer>, String>, LocationError<Error>> {
-        self.process(buf, shape, |plugin, arguments, results| {
-            plugin.decode.call(&mut plugin.ctx, arguments, results)
-        })
+    fn shape_from_wasm_record(record: &Record) -> Result<Vec<usize>, LocationError<Error>> {
+        let Some(Value::List(shape)) = record.field("shape") else {
+            return Err(LocationError::from2(anyhow::Error::msg(format!(
+                "process result record {record:?} is missing shape field"
+            ))));
+        };
+        let shape = shape
+            .typed::<u32>()
+            .map_err(LocationError::from2)?
+            .iter()
+            .copied()
+            .map(u32_as_usize)
+            .collect::<Vec<_>>();
+        Ok(shape)
     }
 
-    pub fn get_config(&mut self) -> Result<Result<String, String>, LocationError<Error>> {
-        let plugin: &mut CodecPlugin<E> = self.plugin.borrow_mut();
-
-        let resource = self
-            .resource
-            .borrow(&mut plugin.ctx)
-            .map_err(LocationError::from2)?;
-
-        let arg = Value::Borrow(resource);
-        let mut result = Value::U8(0);
-
-        plugin
-            .get_config
-            .call(
-                &mut plugin.ctx,
-                std::slice::from_ref(&arg),
-                std::slice::from_mut(&mut result),
-            )
-            .map_err(LocationError::from2)?;
-
-        match result {
-            Value::Result(result) => match &*result {
-                Ok(Some(Value::String(config))) => Ok(Ok(String::from(&**config))),
-                Err(Some(Value::String(err))) => Ok(Err(String::from(&**err))),
-                result => Err(LocationError::from2(anyhow::Error::msg(format!(
-                    "unexpected get-config result value {result:?}"
-                )))),
+    fn with_buffer_slice_from_wasm_record<O>(
+        record: &Record,
+        with: impl for<'a> FnOnce(BufferSlice<'a>) -> Result<O, LocationError<Error>>,
+    ) -> Result<O, LocationError<Error>> {
+        let Some(Value::Variant(variant)) = record.field("buffer") else {
+            return Err(LocationError::from2(anyhow::Error::msg(format!(
+                "process result record {record:?} is missing buffer field"
+            ))));
+        };
+        let Some(Value::List(list)) = variant.value() else {
+            return Err(LocationError::from2(anyhow::Error::msg(format!(
+                "process result buffer has an invalid variant type {:?}",
+                variant.value().map(|v| v.ty())
+            ))));
+        };
+
+        let buffer = match variant.discriminant() {
+            0 => BufferSlice::from(list.typed::<u8>().map_err(LocationError::from2)?),
+            1 => BufferSlice::from(list.typed::<u16>().map_err(LocationError::from2)?),
+            2 => BufferSlice::from(list.typed::<u32>().map_err(LocationError::from2)?),
+            3 => BufferSlice::from(list.typed::<u64>().map_err(LocationError::from2)?),
+            4 => BufferSlice::from(list.typed::<i8>().map_err(LocationError::from2)?),
+            5 => BufferSlice::from(list.typed::<i16>().map_err(LocationError::from2)?),
+            6 => BufferSlice::from(list.typed::<i32>().map_err(LocationError::from2)?),
+            7 => BufferSlice::from(list.typed::<i64>().map_err(LocationError::from2)?),
+            8 => BufferSlice::from(list.typed::<f32>().map_err(LocationError::from2)?),
+            9 => BufferSlice::from(list.typed::<f64>().map_err(LocationError::from2)?),
+            discriminant => {
+                return Err(LocationError::from2(anyhow::Error::msg(format!(
+                    "process result buffer has an invalid variant [{discriminant}]:{:?}",
+                    variant.value().map(|v| v.ty())
+                ))))
             },
-            value => Err(LocationError::from2(anyhow::Error::msg(format!(
-                "unexpected get-config result value {value:?}"
-            )))),
-        }
-    }
-
-    pub fn drop(mut self) -> Result<(), LocationError<Error>> {
-        let plugin: &mut CodecPlugin<E> = self.plugin.borrow_mut();
+        };
 
-        let result = self
-            .resource
-            .drop(&mut plugin.ctx)
-            .map_err(LocationError::from2);
-
-        // We need to forget here instead of using ManuallyDrop since we need
-        //  both a mutable borrow to self.plugin and an immutable borrow to
-        //  self.resource at the same time
-        std::mem::forget(self);
-
-        result
+        with(buffer)
     }
 }
 
-impl<E: WasmEngine, P: BorrowMut<CodecPlugin<E>>> Drop for WasmCodec<E, P> {
+impl<P: BorrowMut<CodecPlugin>> Drop for WasmCodec<P> {
     fn drop(&mut self) {
-        let plugin: &mut CodecPlugin<E> = self.plugin.borrow_mut();
+        let plugin: &mut CodecPlugin = self.plugin.borrow_mut();
 
-        std::mem::drop(self.resource.drop(&mut plugin.ctx));
+        std::mem::drop(plugin.ctx.drop_resource(&self.resource));
     }
 }
```

### Comparing `field-compression-benchmark-0.0.2/codecs/core-host/src/plugin.rs` & `field-compression-benchmark-0.0.3/codecs/core-host/src/plugin.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,43 @@
-use std::{borrow::BorrowMut, marker::PhantomData};
+use std::{borrow::BorrowMut, sync::OnceLock};
 
 use semver::Version;
 use wasm_component_layer::{
     ComponentList, ExportInstance, Func, Instance, InterfaceIdentifier, PackageIdentifier,
     PackageName, Store, TypedFunc, Value,
 };
 use wasm_runtime_layer::backend::WasmEngine;
 
 use core_error::LocationError;
 
-use crate::{codec::WasmCodec, Error};
+use crate::{codec::WasmCodec, store::ErasedWasmStore, Error};
 
 #[allow(clippy::type_complexity, clippy::module_name_repetitions)]
-pub struct CodecPlugin<E: WasmEngine> {
+pub struct CodecPlugin {
     // FIXME: make typed instead
     from_config: Func,
     pub(crate) encode: Func,
     pub(crate) decode: Func,
     codec_id: TypedFunc<(), String>,
     signature: TypedFunc<(), String>,
     documentation: TypedFunc<(), String>,
     pub(crate) get_config: Func,
     pub(crate) instruction_counter: TypedFunc<(), u64>,
     instance: Instance,
-    pub(crate) ctx: Store<(), E>,
+    pub(crate) ctx: Box<dyn Send + Sync + ErasedWasmStore>,
 }
 
-impl<E: WasmEngine> CodecPlugin<E> {
-    pub fn new(instance: Instance, ctx: Store<(), E>) -> Result<Self, LocationError<Error>> {
+impl CodecPlugin {
+    pub fn new<E: WasmEngine>(
+        instance: Instance,
+        ctx: Store<(), E>,
+    ) -> Result<Self, LocationError<Error>>
+    where
+        Store<(), E>: Send + Sync,
+    {
         fn load_func(interface: &ExportInstance, name: &str) -> Result<Func, LocationError<Error>> {
             let Some(func) = interface.func(name) else {
                 return Err(LocationError::from2(anyhow::Error::msg(format!(
                     "WASM component interface does not contain a function named `{name}`"
                 ))));
             };
 
@@ -43,114 +49,102 @@
             name: &str,
         ) -> Result<TypedFunc<P, R>, LocationError<Error>> {
             load_func(interface, name)?
                 .typed()
                 .map_err(LocationError::from2)
         }
 
-        let codecs_interface_id = InterfaceIdentifier::new(
-            PackageIdentifier::new(
-                PackageName::new("fcbench", "codec"),
-                Some(Version::new(0, 1, 0)),
-            ),
-            "codecs",
-        );
-        let Some(codecs_interface) = instance.exports().instance(&codecs_interface_id) else {
+        let interfaces = CodecPluginInterfaces::get();
+
+        let Some(codecs_interface) = instance.exports().instance(&interfaces.codecs) else {
             return Err(LocationError::from2(anyhow::Error::msg(format!(
-                "WASM component does not contain an interface named `{codecs_interface_id}`"
+                "WASM component does not contain an interface named `{}`",
+                interfaces.codecs
             ))));
         };
-
-        let perf_interface_id = InterfaceIdentifier::new(
-            PackageIdentifier::new(
-                PackageName::new("wasi", "perf"),
-                Some(Version::new(0, 1, 0)),
-            ),
-            "perf",
-        );
-        let Some(perf_interface) = instance.exports().instance(&perf_interface_id) else {
+        let Some(perf_interface) = instance.exports().instance(&interfaces.perf) else {
             return Err(LocationError::from2(anyhow::Error::msg(format!(
-                "WASM component does not contain an interface named `{perf_interface_id}`"
+                "WASM component does not contain an interface named `{}`",
+                interfaces.perf
             ))));
         };
 
         Ok(Self {
             from_config: load_func(codecs_interface, "[static]codec.from-config")?,
             encode: load_func(codecs_interface, "[method]codec.encode")?,
             decode: load_func(codecs_interface, "[method]codec.decode")?,
             codec_id: load_typed_func(codecs_interface, "codec-id")?,
             signature: load_typed_func(codecs_interface, "signature")?,
             documentation: load_typed_func(codecs_interface, "documentation")?,
             get_config: load_func(codecs_interface, "[method]codec.get-config")?,
-            instruction_counter: load_typed_func(perf_interface, "instruction-counter")?,
+            instruction_counter: load_typed_func(perf_interface, &interfaces.instruction_counter)?,
             instance,
-            ctx,
+            ctx: Box::new(ctx),
         })
     }
 
     pub fn codec_id(&mut self) -> Result<String, LocationError<Error>> {
-        self.codec_id
-            .call(&mut self.ctx, ())
+        self.ctx
+            .call_typed_str_func(&self.codec_id)
             .map_err(LocationError::from2)
     }
 
     pub fn signature(&mut self) -> Result<String, LocationError<Error>> {
-        self.signature
-            .call(&mut self.ctx, ())
+        self.ctx
+            .call_typed_str_func(&self.signature)
             .map_err(LocationError::from2)
     }
 
     pub fn documentation(&mut self) -> Result<String, LocationError<Error>> {
-        self.documentation
-            .call(&mut self.ctx, ())
+        self.ctx
+            .call_typed_str_func(&self.documentation)
             .map_err(LocationError::from2)
     }
 
     #[allow(clippy::type_complexity)]
     pub fn from_config<P: BorrowMut<Self>>(
         mut plugin: P,
         config: &str,
-    ) -> Result<Result<WasmCodec<E, P>, String>, LocationError<Error>> {
+    ) -> Result<Result<WasmCodec<P>, String>, LocationError<Error>> {
         let plugin_borrow: &mut Self = plugin.borrow_mut();
 
         let args = Value::String(config.into());
         let mut result = Value::U8(0);
 
         plugin_borrow
-            .from_config
-            .call(
-                &mut plugin_borrow.ctx,
+            .ctx
+            .call_func(
+                &plugin_borrow.from_config,
                 std::slice::from_ref(&args),
                 std::slice::from_mut(&mut result),
             )
             .map_err(LocationError::from2)?;
 
         match result {
             Value::Result(result) => match &*result {
                 Ok(Some(Value::Own(resource))) => Ok(Ok(WasmCodec {
                     resource: resource.clone(),
                     plugin,
                     instruction_counter: 0,
-                    _marker: PhantomData::<E>,
                 })),
                 Err(Some(Value::String(err))) => Ok(Err(String::from(&**err))),
                 result => Err(LocationError::from2(anyhow::Error::msg(format!(
                     "unexpected from-config result value {result:?}"
                 )))),
             },
             value => Err(LocationError::from2(anyhow::Error::msg(format!(
                 "unexpected from-config result value {value:?}"
             )))),
         }
     }
 
     pub fn drop(mut self) -> Result<(), LocationError<Error>> {
         let result = self
-            .instance
-            .drop(&mut self.ctx)
+            .ctx
+            .drop_instance(&self.instance)
             .map_err(LocationError::from2);
 
         // We need to forget here instead of using ManuallyDrop since we need
         //  both a mutable borrow to self.plugin and an immutable borrow to
         //  self.resource at the same time
         std::mem::forget(self);
 
@@ -166,12 +160,44 @@
                 .map(|err| format!("{err:#}"))
                 .collect::<Vec<_>>()
                 .join(" || "),
         ))))
     }
 }
 
-impl<E: WasmEngine> Drop for CodecPlugin<E> {
+impl Drop for CodecPlugin {
     fn drop(&mut self) {
-        std::mem::drop(self.instance.drop(&mut self.ctx));
+        std::mem::drop(self.ctx.drop_instance(&self.instance));
+    }
+}
+
+#[non_exhaustive]
+pub struct CodecPluginInterfaces {
+    pub codecs: InterfaceIdentifier,
+    pub perf: InterfaceIdentifier,
+    pub instruction_counter: String,
+}
+
+impl CodecPluginInterfaces {
+    #[must_use]
+    pub fn get() -> &'static Self {
+        static CODEC_PLUGIN_INTERFACES: OnceLock<CodecPluginInterfaces> = OnceLock::new();
+
+        CODEC_PLUGIN_INTERFACES.get_or_init(|| Self {
+            codecs: InterfaceIdentifier::new(
+                PackageIdentifier::new(
+                    PackageName::new("numcodecs", "abc"),
+                    Some(Version::new(0, 1, 0)),
+                ),
+                "codec",
+            ),
+            perf: InterfaceIdentifier::new(
+                PackageIdentifier::new(
+                    PackageName::new("fcbench", "perf"),
+                    Some(Version::new(0, 1, 0)),
+                ),
+                "perf",
+            ),
+            instruction_counter: String::from("instruction-counter"),
+        })
     }
 }
```

### Comparing `field-compression-benchmark-0.0.2/codecs/core-wasm/Cargo.toml` & `field-compression-benchmark-0.0.3/codecs/core-wasm/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 name = "codecs-core-wasm"
 version = "0.1.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
+log = { version = "0.4", default-features = false }
+wasi-logger = { version = "0.1", default-features = false }
 codecs-core = { path = "../core" }
 format_serde_error = { version = "0.3", default-features = false, features = ["serde_json"] }
 serde = { version = "1.0", default-features = false, features = ["alloc", "derive"] }
 serde_json = { version = "1.0", default-features = false, features = ["alloc"] }
-wit-bindgen = { version = "0.23", default-features = false, features = ["macros", "realloc"] }
+wit-bindgen = { version = "0.24", default-features = false, features = ["macros", "realloc"] }
+
+[build-dependencies]
+wit-deps = { path = "../../utils/wit-deps" }
 
 [lints]
 workspace = true
```

### Comparing `field-compression-benchmark-0.0.2/codecs/core-wasm/src/config.rs` & `field-compression-benchmark-0.0.3/codecs/core-wasm/src/config.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/codecs/core-wasm/src/convert.rs` & `field-compression-benchmark-0.0.3/codecs/core-wasm/src/convert.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use codecs_core::{BufferSlice, BufferVec, OwnedBuffer, OwnedBufferImpl};
 
-use crate::bindings::exports::fcbench::codec::codecs::Buffer as WitBuffer;
+use crate::bindings::exports::numcodecs::abc::codec::Buffer as WitBuffer;
 
 #[must_use]
 pub fn wit_buffer_to_codecs(buffer: &WitBuffer) -> BufferSlice {
     match buffer {
         WitBuffer::U8(data) => BufferSlice::from(data.as_slice()),
         WitBuffer::U16(data) => BufferSlice::from(data.as_slice()),
         WitBuffer::U32(data) => BufferSlice::from(data.as_slice()),
```

### Comparing `field-compression-benchmark-0.0.2/codecs/frontend/Cargo.toml` & `field-compression-benchmark-0.0.3/codecs/frontend/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,34 +8,40 @@
 [dependencies]
 anyhow = { version = "1.0", default-features = false }
 codecs-core = { path = "../core", default-features = false }
 codecs-core-host = { path = "../core-host", default-features = false }
 core-error = { path = "../../core/error", default-features = false }
 convert_case = { version = "0.6", default-features = false }
 indexmap = { version = "2.1", default-features = false, features = ["std"] }
+log = { version = "0.4", default-features = false }
 numpy = { version = "0.20", default-features = false }
 polonius-the-crab = { version = "0.4", default-features = false }
-pyodide-webassembly-runtime-layer = { version = ">=0.2.1", default-features = false, optional = true }
+pyodide-webassembly-runtime-layer = { version = ">=0.2.2", default-features = false, optional = true }
 pyo3 = { version = "0.20", default-features = false, features = ["abi3"] }
 semver = { version = "1.0", default-features = false }
 thiserror = { version = "1.0", default-features = false }
-topological-sort = { version = "0.2", default-features = false }
-wac-parser = { git = "https://github.com/peterhuene/wac.git", rev = "7b2f728", version = "0.1", default-features = false }
+wac-graph = { version = "0.1", default-features = false }
 walrus = { git = "https://github.com/rustwasm/walrus.git", rev = "4efdb5c", version = "0.20", default-features = false }
-wasm_component_layer = { git = "https://github.com/juntyr/wasm_component_layer.git", rev = "0d6d5e5", version = "0.1", default-features = false }
+wasm_component_layer = { git = "https://github.com/juntyr/wasm_component_layer.git", rev = "6667c30", version = "0.1", default-features = false }
 wasm_runtime_layer = { version = "0.3", default-features = false }
-wasmparser = { version = "0.202", default-features = false }
+wasmparser = { version = "0.205", default-features = false }
 # wasmtime requires `component-model` feature since wasm_component_layer
 #  enables the feature in the common wasmtime-environ dependency
 wasmtime = { version = "18.0", default-features = false, features = ["runtime", "cranelift", "cache", "component-model"], optional = true }
-wit-component = { version = "0.202", default-features = false }
-wit-parser = { version = "0.202", default-features = false }
+# FIXME: update once wasm_runtime_layer v0.4.0 has been released
+wasmtime_runtime_layer = { git = "https://github.com/juntyr/wasm_runtime_layer.git", rev = "d8ea0c5", default-features = false, optional = true }
+wit-component = { version = "0.205", default-features = false }
+wit-parser = { version = "0.205", default-features = false }
 vecmap-rs = { version = "0.2", default-features = false }
 virtual-wasi-build = { path = "../../wasi/build" }
 
+[dev-dependencies]
+codecs-build = { path = "../build", default-features = false }
+simple_logger = { version = "4.3", default-features = false, features = ["colors"] }
+
 [features]
 default = []
-wasmtime = ["dep:wasmtime", "wasm_runtime_layer/backend_wasmtime"]
+wasmtime = ["dep:wasmtime", "dep:wasmtime_runtime_layer"]
 pyodide = ["dep:pyodide-webassembly-runtime-layer"]
 
 [lints]
 workspace = true
```

### Comparing `field-compression-benchmark-0.0.2/codecs/frontend/src/engine.rs` & `field-compression-benchmark-0.0.3/codecs/frontend/src/engine.rs`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
         AsContext, AsContextMut, Export, Extern, Imports, Value, WasmEngine, WasmExternRef,
         WasmFunc, WasmGlobal, WasmInstance, WasmMemory, WasmModule, WasmStore, WasmStoreContext,
         WasmStoreContextMut, WasmTable,
     },
     ExportType, ExternType, FuncType, GlobalType, ImportType, MemoryType, TableType,
 };
 
-use crate::transform::{InstructionCounterInjecter, NaNCanonicaliser};
+use crate::transform::{instcnt::InstructionCounterInjecter, nan::NaNCanonicaliser};
 
 #[derive(Clone)]
 #[repr(transparent)]
 pub struct ValidatedEngine<E: WasmEngine>(E);
 
 impl<E: WasmEngine> WasmEngine for ValidatedEngine<E> {
     type ExternRef = ValidatedExternRef<E>;
@@ -23,18 +23,16 @@
     type Store<T> = ValidatedStore<T, E>;
     type StoreContext<'a, T: 'a> = ValidatedStoreContext<'a, T, E>;
     type StoreContextMut<'a, T: 'a> = ValidatedStoreContextMut<'a, T, E>;
     type Table = ValidatedTable<E>;
 }
 
 impl<E: WasmEngine> ValidatedEngine<E> {
-    cfg_single_wasm! {
-        pub const fn new(engine: E) -> Self {
-            Self(engine)
-        }
+    pub const fn new(engine: E) -> Self {
+        Self(engine)
     }
 
     const fn as_ref(&self) -> &E {
         &self.0
     }
 
     const fn from_ref(engine: &E) -> &Self {
@@ -270,93 +268,113 @@
             ctx.as_context_mut().as_inner_context_mut(),
             offset,
             buffer,
         )
     }
 }
 
+pub const DETERMINISTIC_WASM_MODULE_FEATURES: wasmparser::WasmFeaturesInflated =
+    wasmparser::WasmFeaturesInflated {
+        // MUST: mutable globals do not introduce non-determinism, as long
+        //       as the host does not change their value to be non-
+        //       deterministic
+        mutable_global: true,
+        // OK: saturating float -> int conversions only produce finite values
+        saturating_float_to_int: true,
+        // MUST: arithmetic sign extension operators are deterministic
+        sign_extension: true,
+        // (unsure): disabled for now, needs further research
+        reference_types: false,
+        // OK: returning multiple values does not interact with determinism
+        multi_value: true,
+        // MUST: operations like memcpy and memset are deterministic
+        bulk_memory: true,
+        // (ok): fixed-width SIMD replicates scalar float semantics
+        simd: true,
+        // BAD: exposes platform-dependent behaviour and non-determinism
+        relaxed_simd: false,
+        // BAD: allows non-deterministic concurrency and race conditions
+        threads: false,
+        // BAD: allows non-deterministic concurrency and race conditions
+        shared_everything_threads: false,
+        // (ok): using tail calls does not interact with determinism
+        //       but support is not universal yet:
+        //       https://webassembly.org/features/
+        tail_call: false,
+        // BAD: float operations can introduce non-deterministic NaNs
+        floats: false,
+        // MUST: using multiple memories does not interact with determinism
+        multi_memory: true,
+        // (unsure): disabled for now, needs further research
+        exceptions: false,
+        // (nope): using a 64bit memory space does not interact with
+        //         determinism but encourages large memory usage
+        memory64: false,
+        // (ok): const i[32|64] add, sub, and mul are deterministic
+        //       but support is not universal yet:
+        //       https://webassembly.org/features/
+        extended_const: false,
+        // NO-CORE: components must have been translated into core WASM
+        //          modules by now
+        component_model: false,
+        // (unsure): disabled for now, needs further research
+        function_references: false,
+        // (unsure): disabled for now, needs further research
+        memory_control: false,
+        // (unsure): disabled for now, needs further research
+        gc: false,
+        // (ok): statically declaring a custom page size is deterministic
+        //       and could reduce resource consumption
+        //       but there is no support yet
+        custom_page_sizes: false,
+        // NO-CORE: components must have been translated into core WASM
+        //          modules by now
+        component_model_values: false,
+        // NO-CORE: components must have been translated into core WASM
+        //          modules by now
+        component_model_nested_names: false,
+    };
+
 #[derive(Clone)]
 #[repr(transparent)]
 pub struct ValidatedModule<E: WasmEngine>(E::Module);
 
 impl<E: WasmEngine> WasmModule<ValidatedEngine<E>> for ValidatedModule<E> {
     fn new(engine: &ValidatedEngine<E>, mut stream: impl std::io::Read) -> anyhow::Result<Self> {
         let mut bytes = Vec::new();
         stream.read_to_end(&mut bytes)?;
 
-        wasmparser::Validator::new_with_features(wasmparser::WasmFeatures {
-            // MUST: mutable globals do not introduce non-determinism, as long
-            //       as the host does not change their value to be non-
-            //       deterministic
-            mutable_global: true,
-            // OK: saturating float -> int conversions only produce finite values
-            saturating_float_to_int: true,
-            // MUST: arithmetic sign extension operators are deterministic
-            sign_extension: true,
-            // (unsure): disabled for now, needs further research
-            reference_types: false,
-            // OK: returning multiple values does not interact with determinism
-            multi_value: true,
-            // MUST: operations like memcpy and memset are deterministic
-            bulk_memory: true,
-            // (ok): fixed-width SIMD replicates scalar float semantics
-            simd: true,
-            // BAD: exposes platform-dependent behaviour and non-determinism
-            relaxed_simd: false,
-            // BAD: allows non-deterministic concurrency and race conditions
-            threads: false,
-            // (ok): using tail calls does not interact with determinism
-            //       but support is not universal yet:
-            //       https://webassembly.org/features/
-            tail_call: false,
-            // MUST: float operations can introduce non-deterministic NaNs
-            floats: true,
-            // MUST: using multiple memories does not interact with determinism
-            // TODO: support is not universal yet, fail gracefully:
-            //       https://webassembly.org/features/
-            multi_memory: true,
-            // (unsure): disabled for now, needs further research
-            exceptions: false,
-            // (nope): using a 64bit memory space does not interact with
-            //         determinism but encourages large memory usage
-            memory64: false,
-            // (ok): const i[32|64] add, sub, and mul are deterministic
-            //       but support is not universal yet:
-            //       https://webassembly.org/features/
-            extended_const: false,
-            // NO-CORE: components must have been translated into core WASM
-            //          modules by now
-            component_model: false,
-            // (unsure): disabled for now, needs further research
-            function_references: false,
-            // (unsure): disabled for now, needs further research
-            memory_control: false,
-            // (unsure): disabled for now, needs further research
-            gc: false,
-            // NO-CORE: components must have been translated into core WASM
-            //          modules by now
-            component_model_values: false,
-            // NO-CORE: components must have been translated into core WASM
-            //          modules by now
-            component_model_nested_names: false,
-        })
+        wasmparser::Validator::new_with_features(
+            wasmparser::WasmFeaturesInflated {
+                // MUST: floats are required and we are running the NaN
+                //       canonicalisation transform to make them deterministic
+                floats: true,
+                ..DETERMINISTIC_WASM_MODULE_FEATURES
+            }
+            .into(),
+        )
         .validate_all(&bytes)?;
 
         let mut module = walrus::Module::from_buffer(&bytes)?;
 
         // Normalise NaNs to ensure floating point operations are deterministic
         NaNCanonicaliser::apply_to_module(&mut module)?;
 
         // Inject an instruction counter into the WASM module
         let instruction_counter = InstructionCounterInjecter::inject_into_module(&mut module);
 
-        if let Ok(func) = module
-            .exports
-            .get_func("wasi:perf/perf@0.1.0#instruction-counter")
-        {
+        if let Ok(func) = module.exports.get_func({
+            let codecs_core_host::CodecPluginInterfaces {
+                perf: perf_interface,
+                instruction_counter,
+                ..
+            } = codecs_core_host::CodecPluginInterfaces::get();
+
+            format!("{perf_interface}#{instruction_counter}")
+        }) {
             module.replace_exported_func(func, |(builder, _arg_locals)| {
                 builder.global_get(instruction_counter);
             })?;
         }
 
         let bytes = module.emit_wasm();
```

### Comparing `field-compression-benchmark-0.0.2/codecs/frontend/src/error.rs` & `field-compression-benchmark-0.0.3/codecs/frontend/src/error.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/codecs/frontend/src/transform.rs` & `field-compression-benchmark-0.0.3/codecs/frontend/src/transform/nan.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,149 +1,7 @@
-pub struct InstructionCounterInjecter {
-    instruction_counter: walrus::GlobalId,
-}
-
-impl InstructionCounterInjecter {
-    pub fn inject_into_module(module: &mut walrus::Module) -> walrus::GlobalId {
-        let (instruction_counter, _import) =
-            module.add_import_global("fcbench", "instruction-counter", walrus::ValType::I64, true);
-
-        for (_, func) in module.funcs.iter_local_mut() {
-            let entry = func.entry_block();
-
-            walrus::ir::dfs_pre_order_mut(
-                &mut Self {
-                    instruction_counter,
-                },
-                func,
-                entry,
-            );
-        }
-
-        instruction_counter
-    }
-
-    const fn instruction_needs_counter_update(instr: &walrus::ir::Instr) -> bool {
-        #[allow(clippy::match_same_arms)]
-        match instr {
-            walrus::ir::Instr::Block(_)
-            | walrus::ir::Instr::Loop(_)
-            | walrus::ir::Instr::Br(_)
-            | walrus::ir::Instr::BrIf(_)
-            | walrus::ir::Instr::IfElse(_)
-            | walrus::ir::Instr::BrTable(_)
-            | walrus::ir::Instr::Return(_) => true,
-            // calls must return control flow to continue,
-            //  so no counter-saving is necessary
-            walrus::ir::Instr::Call(_) | walrus::ir::Instr::CallIndirect(_) => false,
-            // unreachable control flow doesn't need to care
-            //  about instruction counting
-            walrus::ir::Instr::Unreachable(_) => false,
-            // no control flow occurs
-            walrus::ir::Instr::LocalGet(_)
-            | walrus::ir::Instr::LocalSet(_)
-            | walrus::ir::Instr::LocalTee(_)
-            | walrus::ir::Instr::GlobalGet(_)
-            | walrus::ir::Instr::GlobalSet(_)
-            | walrus::ir::Instr::Const(_)
-            | walrus::ir::Instr::Binop(_)
-            | walrus::ir::Instr::Unop(_)
-            | walrus::ir::Instr::Select(_)
-            | walrus::ir::Instr::Drop(_)
-            | walrus::ir::Instr::MemorySize(_)
-            | walrus::ir::Instr::MemoryGrow(_)
-            | walrus::ir::Instr::MemoryInit(_)
-            | walrus::ir::Instr::DataDrop(_)
-            | walrus::ir::Instr::MemoryCopy(_)
-            | walrus::ir::Instr::MemoryFill(_)
-            | walrus::ir::Instr::Load(_)
-            | walrus::ir::Instr::Store(_)
-            | walrus::ir::Instr::AtomicRmw(_)
-            | walrus::ir::Instr::Cmpxchg(_)
-            | walrus::ir::Instr::AtomicNotify(_)
-            | walrus::ir::Instr::AtomicWait(_)
-            | walrus::ir::Instr::AtomicFence(..)
-            | walrus::ir::Instr::TableGet(_)
-            | walrus::ir::Instr::TableSet(_)
-            | walrus::ir::Instr::TableGrow(_)
-            | walrus::ir::Instr::TableSize(_)
-            | walrus::ir::Instr::TableFill(_)
-            | walrus::ir::Instr::RefNull(_)
-            | walrus::ir::Instr::RefIsNull(_)
-            | walrus::ir::Instr::RefFunc(_)
-            | walrus::ir::Instr::V128Bitselect(_)
-            | walrus::ir::Instr::I8x16Swizzle(_)
-            | walrus::ir::Instr::I8x16Shuffle(_)
-            | walrus::ir::Instr::LoadSimd(_)
-            | walrus::ir::Instr::TableInit(_)
-            | walrus::ir::Instr::ElemDrop(_)
-            | walrus::ir::Instr::TableCopy(_) => false,
-        }
-    }
-
-    fn generate_instruction_counter_update(
-        &self,
-        delta: i64,
-    ) -> impl IntoIterator<Item = (walrus::ir::Instr, walrus::ir::InstrLocId)> {
-        [
-            (
-                walrus::ir::Instr::GlobalGet(walrus::ir::GlobalGet {
-                    global: self.instruction_counter,
-                }),
-                walrus::ir::InstrLocId::default(),
-            ),
-            (
-                walrus::ir::Instr::Const(walrus::ir::Const {
-                    value: walrus::ir::Value::I64(delta),
-                }),
-                walrus::ir::InstrLocId::default(),
-            ),
-            (
-                walrus::ir::Instr::Binop(walrus::ir::Binop {
-                    op: walrus::ir::BinaryOp::I64Add,
-                }),
-                walrus::ir::InstrLocId::default(),
-            ),
-            (
-                walrus::ir::Instr::GlobalSet(walrus::ir::GlobalSet {
-                    global: self.instruction_counter,
-                }),
-                walrus::ir::InstrLocId::default(),
-            ),
-        ]
-    }
-}
-
-impl walrus::ir::VisitorMut for InstructionCounterInjecter {
-    fn start_instr_seq_mut(&mut self, instr_seq: &mut walrus::ir::InstrSeq) {
-        let mut i = 0;
-
-        let mut counter: i64 = 0;
-
-        while let Some((instr, _)) = instr_seq.get(i) {
-            counter += 1;
-
-            if Self::instruction_needs_counter_update(instr) {
-                for new_instr in self.generate_instruction_counter_update(counter) {
-                    instr_seq.insert(i, new_instr);
-                    i += 1;
-                }
-
-                counter = 0;
-            }
-
-            i += 1;
-        }
-
-        if counter > 0 {
-            instr_seq.extend(self.generate_instruction_counter_update(counter));
-        }
-    }
-}
-
 /// Adapted from cranelift's NaN canonicalisation codegen pass
 /// <https://github.com/bytecodealliance/wasmtime/blob/ead6c7cc5dbb876437acbdf429a9190f25b96755/cranelift/codegen/src/nan_canonicalization.rs>
 /// Released under the Apache-2.0 WITH LLVM-exception License
 ///
 /// Implementation written referencing:
 /// - WebAssembly Core Specification v2 <https://www.w3.org/TR/2024/WD-wasm-core-2-20240219>
 /// - The "WebAssembly 128-bit packed SIMD Extension" Specification: <https://github.com/WebAssembly/spec/blob/f8114686035f6ffc358771c822ede3c96bf54cd9/proposals/simd/SIMD.md>
```

### Comparing `field-compression-benchmark-0.0.2/codecs/identity/src/lib.rs` & `field-compression-benchmark-0.0.3/codecs/identity/src/lib.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/codecs/linear-quantize/Cargo.toml` & `field-compression-benchmark-0.0.3/codecs/linear-quantize/Cargo.toml`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/codecs/linear-quantize/src/lib.rs` & `field-compression-benchmark-0.0.3/codecs/linear-quantize/src/lib.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/codecs/log/src/lib.rs` & `field-compression-benchmark-0.0.3/codecs/log/src/lib.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/codecs/reinterpret/src/lib.rs` & `field-compression-benchmark-0.0.3/codecs/reinterpret/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                 let mut buffer =
                     codecs_core::BufferVec::zeros_with_ty_len(ty, v.len() / ty.layout().size());
                 #[allow(unsafe_code)]
                 // Safety: buffer is v.len() bytes long and propely aligned for ty
                 unsafe {
                     std::ptr::copy_nonoverlapping(
                         v.as_ptr(),
-                        buffer.as_bytes_mut().as_mut_ptr().cast(),
+                        buffer.as_slice_mut().as_bytes_mut().as_mut_ptr().cast(),
                         v.len(),
                     );
                 }
                 (buffer, shape)
             },
             (codecs_core::BufferSlice::U16(v), codecs_core::BufferTy::I16) => (
                 codecs_core::BufferVec::I16(
```

### Comparing `field-compression-benchmark-0.0.2/codecs/sz3/Cargo.toml` & `field-compression-benchmark-0.0.3/codecs/zfp/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 [package]
-name = "sz3-codec"
+name = "zfp-codec"
 version = "0.1.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 crate-type = ["cdylib"]
 
 [dependencies]
 codecs-core = { path = "../core", default-features = false }
 codecs-core-wasm = { path = "../core-wasm", default-features = false }
-postcard = { version = "1.0", default-features = false }
 serde = { version = "1.0", default-features = false, features = ["std", "derive"] }
-sz3 = { git = "https://github.com/juntyr/sz3-rs.git", rev = "475d6e0", version = "0.1", default-features = false }
-# sz3-sys/zstd-sys@2.0.10 breaks compilation with XXH_STATIC_ASSERT=0
-zstd-sys = { version = "=2.0.9", default-features = false }
+zfp-sys = { version = ">=0.1.15", default-features = false, features = ["static"] }
 
 [lints]
 workspace = true
```

### Comparing `field-compression-benchmark-0.0.2/codecs/sz3/src/lib.rs` & `field-compression-benchmark-0.0.3/codecs/sz3/src/lib.rs`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,20 @@
         // Since they carry no information for Sz3 and we already encode them
         //  in our custom header, we just skip them here
         if *length > 1 {
             builder = builder.dim(*length).map_err(|err| format!("{err}"))?;
         }
     }
 
+    if data.len() == 1 {
+        // If there is only one element, all dimensions will have been skipped,
+        //  so we explicitly encode one dimension of size 1 here
+        builder = builder.dim(1).map_err(|err| format!("{err}"))?;
+    }
+
     let data = builder.finish().map_err(|err| format!("{err}"))?;
 
     let error_bound = match bound {
         ErrorBound::AbsoluteAndRelative { abs, rel } => sz3::ErrorBound::AbsoluteAndRelative {
             absolute_bound: *abs,
             relative_bound: *rel,
         },
@@ -46,14 +52,18 @@
         },
         ErrorBound::Absolute { abs } => sz3::ErrorBound::Absolute(*abs),
         ErrorBound::Relative { rel } => sz3::ErrorBound::Relative(*rel),
         ErrorBound::PS2NR { psnr } => sz3::ErrorBound::PSNR(*psnr),
         ErrorBound::L2Norm { l2 } => sz3::ErrorBound::L2Norm(*l2),
     };
 
+    // FIXME: Sz3 seems to have a UB bug that impacts the last few bytes but is
+    //        somehow gone if we use stdio first ... aaaaaaaah
+    std::mem::drop(std::io::Read::read(&mut std::io::stdin(), &mut []));
+
     // TODO: avoid extra allocation here
     let compressed = sz3::compress(&data, error_bound).map_err(|err| format!("{err}"))?;
     encoded.extend_from_slice(&compressed);
 
     Ok(encoded)
 }
 
@@ -286,8 +296,31 @@
             decoded.buffer.as_slice(),
             codecs_core::BufferSlice::I32(&[1, 2, 3, 4])
         );
         assert_eq!(decoded.shape, vec![2, 1, 2, 1]);
 
         Ok(())
     }
+
+    #[test]
+    fn small_state() -> Result<(), String> {
+        for data in [
+            &[][..],
+            &[0.0],
+            &[0.0, 1.0],
+            &[0.0, 1.0, 0.0],
+            &[0.0, 1.0, 0.0, 1.0],
+        ] {
+            let encoded = compress::<f64>(data, &[data.len()], &ErrorBound::Absolute { abs: 0.0 })?;
+            let decoded = decompress(&encoded)?;
+
+            assert_eq!(decoded.buffer.as_slice().ty(), codecs_core::BufferTy::F64);
+            assert_eq!(
+                decoded.buffer.as_slice(),
+                codecs_core::BufferSlice::F64(data)
+            );
+            assert_eq!(decoded.shape, vec![data.len()]);
+        }
+
+        Ok(())
+    }
 }
```

### Comparing `field-compression-benchmark-0.0.2/codecs/uniform-noise/Cargo.toml` & `field-compression-benchmark-0.0.3/codecs/uniform-noise/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 [lib]
 crate-type = ["cdylib"]
 
 [dependencies]
 codecs-core = { path = "../core", default-features = false }
 codecs-core-wasm = { path = "../core-wasm", default-features = false }
 rand = { version = "0.8", default-features = false }
-rand_chacha = { version = "0.3", default-features = false }
+wyhash = { version = "0.5", default-features = false }
 serde = { version = "1.0", default-features = false, features = ["std", "derive"] }
 
 [lints]
 workspace = true
```

### Comparing `field-compression-benchmark-0.0.2/codecs/uniform-noise/src/lib.rs` & `field-compression-benchmark-0.0.3/codecs/uniform-noise/src/lib.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,64 @@
 #![cfg_attr(not(test), no_main)]
 
-use std::sync::Mutex;
+use std::hash::{Hash, Hasher};
 
 use rand::{
     distributions::{Distribution, Open01},
-    Rng, SeedableRng,
+    SeedableRng,
 };
-use rand_chacha::ChaChaRng;
+use wyhash::{WyHash, WyRng};
 
 #[must_use]
-pub fn add_uniform_noise<T: Float>(data: &[T], rng: &mut impl Rng, scale: T) -> Vec<T>
+pub fn add_uniform_noise<T: Float>(data: &[T], shape: &[usize], scale: T, seed: u64) -> Vec<T>
 where
     Open01: Distribution<T>,
 {
+    let mut hasher = WyHash::with_seed(seed);
+    // hashing the shape provides a prefix for the flattened data
+    shape.hash(&mut hasher);
+    data.iter().copied().for_each(|x| x.hash_bits(&mut hasher));
+    let seed = hasher.finish();
+
+    let mut rng: WyRng = WyRng::seed_from_u64(seed);
+
     data.iter()
-        .map(|x| Open01.sample(rng).mul_add(scale, *x))
+        .map(|x| Open01.sample(&mut rng).mul_add(scale, *x))
         .collect()
 }
 
+#[derive(Clone, serde::Serialize, serde::Deserialize)]
 pub struct UniformNoiseCodec {
-    rng: Mutex<ChaChaRng>,
-    config: UniformNoiseCodecConfig,
-}
-
-impl Clone for UniformNoiseCodec {
-    fn clone(&self) -> Self {
-        Self {
-            #[allow(clippy::unwrap_used)] // FIXME
-            rng: Mutex::new(self.rng.try_lock().unwrap().clone()),
-            config: self.config.clone(),
-        }
-    }
+    scale: f64,
+    seed: u64,
 }
 
 impl codecs_core::Codec for UniformNoiseCodec {
     type DecodedBuffer = codecs_core::VecBuffer;
     type EncodedBuffer = codecs_core::VecBuffer;
 
     const CODEC_ID: &'static str = "uniform-noise";
 
     fn from_config<'de, D: serde::Deserializer<'de>>(config: D) -> Result<Self, D::Error> {
-        let config: UniformNoiseCodecConfig = serde::Deserialize::deserialize(config)?;
-
-        Ok(Self {
-            rng: Mutex::new(ChaChaRng::seed_from_u64(config.seed)),
-            config,
-        })
+        serde::Deserialize::deserialize(config)
     }
 
     fn encode(
         &self,
         buf: codecs_core::BufferSlice,
         shape: &[usize],
     ) -> Result<codecs_core::ShapedBuffer<Self::EncodedBuffer>, String> {
-        let Ok(mut rng) = self.rng.lock() else {
-            return Err(String::from("UniformNoise::encode cannot use poisoned rng"));
-        };
-
         let encoded =
             match buf {
                 #[allow(clippy::cast_possible_truncation)]
                 codecs_core::BufferSlice::F32(data) => codecs_core::BufferVec::F32(
-                    add_uniform_noise(data, &mut *rng, self.config.scale as f32),
+                    add_uniform_noise(data, shape, self.scale as f32, self.seed),
                 ),
                 codecs_core::BufferSlice::F64(data) => codecs_core::BufferVec::F64(
-                    add_uniform_noise(data, &mut *rng, self.config.scale),
+                    add_uniform_noise(data, shape, self.scale, self.seed),
                 ),
                 buf => {
                     return Err(format!(
                         "UniformNoise::encode does not support the buffer dtype `{}`",
                         buf.ty(),
                     ))
                 },
@@ -99,49 +89,53 @@
         Ok(codecs_core::ShapedBuffer {
             shape: Vec::from(shape),
             buffer: decoded,
         })
     }
 
     fn get_config<S: serde::Serializer>(&self, serializer: S) -> Result<S::Ok, S::Error> {
-        serde::Serialize::serialize(&self.config, serializer)
+        serde::Serialize::serialize(self, serializer)
     }
 }
 
 codecs_core_wasm::export_codec! {
     /// Uniform noise codec which adds U(-scale/2, scale/2) uniform random
     /// noise to the input on encoding and passes through the input unchanged
     /// during decoding.
     ///
-    /// Note that this code has interior mutable state and encoding the same
-    /// data twice will not produce the same result. To encode reproducibly,
-    /// create a new codec with the same seed before every encoding.
+    /// This codec first hashes the input and its shape to then seed a pseudo-
+    /// random number generator that generates the uniform noise. Therefore,
+    /// encoding the same data with the same seed will produce the same noise
+    /// and thus the same encoded data.
     ///
     /// Args:
     ///     scale (float): Scale/width of the uniform noise to add on encoding.
     ///     seed (int): Seed for the random number generator.
     UniformNoiseCodec(scale, seed)
 }
 
-#[derive(Clone, serde::Serialize, serde::Deserialize)]
-#[serde(rename = "UniformNoiseCodec")]
-struct UniformNoiseCodecConfig {
-    scale: f64,
-    seed: u64,
-}
-
 pub trait Float: Copy {
     #[must_use]
     fn mul_add(self, a: Self, b: Self) -> Self;
+
+    fn hash_bits<H: Hasher>(self, hasher: &mut H);
 }
 
 impl Float for f32 {
     fn mul_add(self, a: Self, b: Self) -> Self {
         Self::mul_add(self, a, b)
     }
+
+    fn hash_bits<H: Hasher>(self, hasher: &mut H) {
+        hasher.write_u32(self.to_bits());
+    }
 }
 
 impl Float for f64 {
     fn mul_add(self, a: Self, b: Self) -> Self {
         Self::mul_add(self, a, b)
     }
+
+    fn hash_bits<H: Hasher>(self, hasher: &mut H) {
+        hasher.write_u64(self.to_bits());
+    }
 }
```

### Comparing `field-compression-benchmark-0.0.2/codecs/wit/world.wit` & `field-compression-benchmark-0.0.3/codecs/wit/codec.wit`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-package fcbench:codec@0.1.0;
+package numcodecs:abc@0.1.0;
 
-interface codecs {
+interface codec {
   variant buffer {
     %u8(list<u8>),
     %u16(list<u16>),
     %u32(list<u32>),
     %u64(list<u64>),
     i8(list<s8>),
     i16(list<s16>),
@@ -28,11 +28,7 @@
     get-config: func() -> result<string, string>;
   }
 
   codec-id: func() -> string;
   signature: func() -> string;
   documentation: func() -> string;
 }
-
-world fcbench-codec {
-  export codecs;
-}
```

### Comparing `field-compression-benchmark-0.0.2/codecs/zfp/Cargo.toml` & `field-compression-benchmark-0.0.3/core/measure/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [package]
-name = "zfp-codec"
+name = "core-measure"
 version = "0.1.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
-[lib]
-crate-type = ["cdylib"]
-
 [dependencies]
-codecs-core = { path = "../core", default-features = false }
-codecs-core-wasm = { path = "../core-wasm", default-features = false }
-serde = { version = "1.0", default-features = false, features = ["std", "derive"] }
-zfp-sys = { version = ">=0.1.15", default-features = false, features = ["static"] }
+core-error = { path = "../error", default-features = false }
+human_bytes = { version = "0.4", default-features = false, features = ["si-units"] }
+rand = { version = "0.8", default-features = false }
+serde = { version = "1.0", default-features = false, features = ["derive"] }
+serde-name = { version = "0.2", default-features = false }
+thiserror = { version = "1.0", default-features = false }
 
 [lints]
 workspace = true
```

### Comparing `field-compression-benchmark-0.0.2/codecs/zfp/src/lib.rs` & `field-compression-benchmark-0.0.3/codecs/zfp/src/lib.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/codecs/zfp/src/zfp.rs` & `field-compression-benchmark-0.0.3/codecs/zfp/src/zfp.rs`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,19 @@
 
         let mut decompressed =
             codecs_core::BufferVec::zeros_with_ty_len(field_type, shape.iter().product());
 
         unsafe {
             zfp_sys::zfp_field_set_pointer(
                 self.field,
-                decompressed.as_bytes_mut().as_mut_ptr().cast(),
+                decompressed
+                    .as_slice_mut()
+                    .as_bytes_mut()
+                    .as_mut_ptr()
+                    .cast(),
             );
         }
 
         if unsafe { zfp_sys::zfp_decompress(self.stream, self.field) } == 0 {
             return Err(String::from("Zfp decompression failed"));
         }
```

### Comparing `field-compression-benchmark-0.0.2/codecs/zlib/Cargo.toml` & `field-compression-benchmark-0.0.3/codecs/zlib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/codecs/zlib/src/lib.rs` & `field-compression-benchmark-0.0.3/codecs/zlib/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,16 @@
 
 pub fn decompress(data: &[u8]) -> Result<(codecs_core::BufferVec, Vec<usize>), String> {
     let (header, data) = postcard::take_from_bytes::<CompressionHeader>(data)
         .map_err(|err| format!("Zlib::decode failed to read header: {err}"))?;
 
     let mut decoded =
         codecs_core::BufferVec::zeros_with_ty_len(header.dtype, header.shape.iter().product());
-    let decoded_bytes = decoded.as_bytes_mut();
+    let mut decoded_bytes = decoded.as_slice_mut();
+    let decoded_bytes = decoded_bytes.as_bytes_mut();
 
     let flags = miniz_oxide::inflate::core::inflate_flags::TINFL_FLAG_PARSE_ZLIB_HEADER
         | miniz_oxide::inflate::core::inflate_flags::TINFL_FLAG_USING_NON_WRAPPING_OUTPUT_BUF;
 
     let mut decomp = Box::<miniz_oxide::inflate::core::DecompressorOxide>::default();
 
     let (status, in_consumed, out_consumed) =
```

### Comparing `field-compression-benchmark-0.0.2/codecs/zstd/Cargo.toml` & `field-compression-benchmark-0.0.3/codecs/zstd/Cargo.toml`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/codecs/zstd/src/lib.rs` & `field-compression-benchmark-0.0.3/codecs/zstd/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,16 @@
         };
 
         let (header, data) = postcard::take_from_bytes::<CompressionHeader>(data)
             .map_err(|err| format!("Zstd failed to read header: {err}"))?;
 
         let mut decoded =
             codecs_core::BufferVec::zeros_with_ty_len(header.dtype, header.shape.iter().product());
-        let mut decoded_bytes = decoded.as_bytes_mut();
+        let mut decoded_bytes = decoded.as_slice_mut();
+        let mut decoded_bytes = decoded_bytes.as_bytes_mut();
 
         zstd::stream::copy_decode(data, &mut decoded_bytes).map_err(|err| format!("{err}"))?;
 
         if !decoded_bytes.is_empty() {
             return Err(String::from("Zstd::decode did not produce enough data"));
         }
```

### Comparing `field-compression-benchmark-0.0.2/core/benchmark/Cargo.toml` & `field-compression-benchmark-0.0.3/core/benchmark/Cargo.toml`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/benchmark/src/case.rs` & `field-compression-benchmark-0.0.3/core/benchmark/src/case.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/benchmark/src/error.rs` & `field-compression-benchmark-0.0.3/core/benchmark/src/error.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/benchmark/src/goodness.rs` & `field-compression-benchmark-0.0.3/core/benchmark/src/goodness.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/benchmark/src/lib.rs` & `field-compression-benchmark-0.0.3/core/benchmark/src/lib.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/benchmark/src/measuring.rs` & `field-compression-benchmark-0.0.3/core/benchmark/src/measuring.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/benchmark/src/performance.rs` & `field-compression-benchmark-0.0.3/core/benchmark/src/performance.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/benchmark/src/report.rs` & `field-compression-benchmark-0.0.3/core/benchmark/src/report.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/benchmark/src/reporter.rs` & `field-compression-benchmark-0.0.3/core/benchmark/src/reporter.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/benchmark/src/settings.rs` & `field-compression-benchmark-0.0.3/core/benchmark/src/settings.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/compressor/Cargo.toml` & `field-compression-benchmark-0.0.3/core/compressor/Cargo.toml`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/compressor/src/codec/config.rs` & `field-compression-benchmark-0.0.3/core/compressor/src/codec/config.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/compressor/src/codec/mod.rs` & `field-compression-benchmark-0.0.3/core/compressor/src/codec/mod.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/compressor/src/compress.rs` & `field-compression-benchmark-0.0.3/core/compressor/src/compress.rs`

 * *Files 2% similar despite different names*

```diff
@@ -211,18 +211,18 @@
     py: Python<'py>,
     array: &'py PyUntypedArray,
     codecs: Vec<&'py crate::numcodecs::Codec>,
     tracker: &mut CompressorPerformanceTracker,
 ) -> Result<&'py PyUntypedArray, PyErr> {
     // pre-obtain methods that are needed in the hot encode and decode loops
     let numpy = py.import(intern!(py, "numpy"))?;
-    let ensure_contiguous_ndarray_like = py
+    let ensure_ndarray_like = py
         .import(intern!(py, "numcodecs"))?
         .getattr(intern!(py, "compat"))?
-        .getattr(intern!(py, "ensure_contiguous_ndarray_like"))?;
+        .getattr(intern!(py, "ensure_ndarray_like"))?;
     let nbytes = intern!(py, "nbytes");
     let empty = numpy.getattr(intern!(py, "empty"))?;
     let reshape = intern!(py, "reshape");
     let instruction_counter = intern!(py, "instruction_counter");
 
     let mut silhouettes = Vec::with_capacity(codecs.len());
 
@@ -237,17 +237,20 @@
                 .getattr(instruction_counter)
                 .and_then(PyAny::extract)
                 .ok();
             let encode_start = match WallTime::start() {
                 Ok(encode_start) => encode_start,
                 Err(err) => err.infallible(),
             };
-            let encoded: &PyUntypedArray = ensure_contiguous_ndarray_like
+            let encoded: &PyUntypedArray = ensure_ndarray_like
                 .call1((codec.encode(encoded)?,))?
                 .extract()?;
+            if !encoded.is_contiguous() {
+                return Err(PyErr::from(numpy::NotContiguousError));
+            }
             let encode_timing = match WallTime::end(encode_start) {
                 Ok(encode_timing) => encode_timing,
                 Err(err) => err.infallible(),
             };
             let post_instructions: Option<u64> = codec
                 .as_ref()
                 .getattr(instruction_counter)
```

### Comparing `field-compression-benchmark-0.0.2/core/compressor/src/compressor/config.rs` & `field-compression-benchmark-0.0.3/core/compressor/src/compressor/config.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/compressor/src/compressor/mod.rs` & `field-compression-benchmark-0.0.3/core/compressor/src/compressor/mod.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/compressor/src/numcodecs.rs` & `field-compression-benchmark-0.0.3/core/compressor/src/numcodecs.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/compressor/src/parameter/config.rs` & `field-compression-benchmark-0.0.3/core/compressor/src/parameter/config.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/compressor/src/parameter/mod.rs` & `field-compression-benchmark-0.0.3/core/compressor/src/parameter/mod.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/dataset/Cargo.toml` & `field-compression-benchmark-0.0.3/core/dataset/Cargo.toml`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/dataset/src/dataset/config.rs` & `field-compression-benchmark-0.0.3/core/dataset/src/dataset/config.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/dataset/src/dataset/mod.rs` & `field-compression-benchmark-0.0.3/core/dataset/src/dataset/mod.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/dataset/src/units.rs` & `field-compression-benchmark-0.0.3/core/dataset/src/units.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/dataset/src/variable/config.rs` & `field-compression-benchmark-0.0.3/core/dataset/src/variable/config.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/dataset/src/variable/derivative/config.rs` & `field-compression-benchmark-0.0.3/core/dataset/src/variable/derivative/config.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/dataset/src/variable/derivative/mod.rs` & `field-compression-benchmark-0.0.3/core/dataset/src/variable/derivative/mod.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/dataset/src/variable/dimension/config/mod.rs` & `field-compression-benchmark-0.0.3/core/dataset/src/variable/dimension/config/mod.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/dataset/src/variable/dimension/config/slice.rs` & `field-compression-benchmark-0.0.3/core/dataset/src/variable/dimension/config/slice.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/dataset/src/variable/dimension/mod.rs` & `field-compression-benchmark-0.0.3/core/dataset/src/variable/dimension/mod.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/dataset/src/variable/mod.rs` & `field-compression-benchmark-0.0.3/core/dataset/src/variable/mod.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/error/src/lib.rs` & `field-compression-benchmark-0.0.3/core/error/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -85,14 +85,24 @@
         LocationError {
             inner: Box::new(LocationErrorInner {
                 error: map(self.inner.error),
                 location: self.inner.location,
             }),
         }
     }
+
+    #[must_use]
+    pub fn map_ref<'a, F: Error>(&'a self, map: impl FnOnce(&'a E) -> F) -> LocationError<F> {
+        LocationError {
+            inner: Box::new(LocationErrorInner {
+                error: map(&self.inner.error),
+                location: self.inner.location.clone(),
+            }),
+        }
+    }
 }
 
 impl<E: Error + Into<std::convert::Infallible>> LocationError<E> {
     pub fn infallible(self) -> ! {
         #[allow(unreachable_code)]
         match self.into_error().into() {}
     }
```

### Comparing `field-compression-benchmark-0.0.2/core/goodness/Cargo.toml` & `field-compression-benchmark-0.0.3/core/goodness/Cargo.toml`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/goodness/src/bit_information.rs` & `field-compression-benchmark-0.0.3/core/goodness/src/bit_information.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/goodness/src/correlation.rs` & `field-compression-benchmark-0.0.3/core/goodness/src/correlation.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/goodness/src/error.rs` & `field-compression-benchmark-0.0.3/core/goodness/src/error.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/goodness/src/lib.rs` & `field-compression-benchmark-0.0.3/core/goodness/src/lib.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/goodness/src/pca.rs` & `field-compression-benchmark-0.0.3/core/goodness/src/pca.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/goodness/src/uniformity.rs` & `field-compression-benchmark-0.0.3/core/goodness/src/uniformity.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/measure/Cargo.toml` & `field-compression-benchmark-0.0.3/codecs/sz3/Cargo.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [package]
-name = "core-measure"
+name = "sz3-codec"
 version = "0.1.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
+[lib]
+crate-type = ["cdylib"]
+
 [dependencies]
-core-error = { path = "../error", default-features = false }
-human_bytes = { version = "0.4", default-features = false, features = ["si-units"] }
-rand = { version = "0.8", default-features = false }
-serde = { version = "1.0", default-features = false, features = ["derive"] }
-serde-name = { version = "0.2", default-features = false }
-thiserror = { version = "1.0", default-features = false }
+codecs-core = { path = "../core", default-features = false }
+codecs-core-wasm = { path = "../core-wasm", default-features = false }
+postcard = { version = "1.0", default-features = false }
+serde = { version = "1.0", default-features = false, features = ["std", "derive"] }
+sz3 = { git = "https://github.com/juntyr/sz3-rs.git", rev = "37622dd", version = "0.1", default-features = false }
+# sz3-sys/zstd-sys@2.0.10 breaks compilation with XXH_STATIC_ASSERT=0
+zstd-sys = { version = "=2.0.9", default-features = false }
 
 [lints]
 workspace = true
```

### Comparing `field-compression-benchmark-0.0.2/core/measure/src/lib.rs` & `field-compression-benchmark-0.0.3/core/measure/src/lib.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/measure/src/measurement.rs` & `field-compression-benchmark-0.0.3/core/measure/src/measurement.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/measure/src/stats.rs` & `field-compression-benchmark-0.0.3/core/measure/src/stats.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/model/Cargo.toml` & `field-compression-benchmark-0.0.3/core/model/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 name = "core-model"
 version = "0.1.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
+dyn-clone = { version = "1.0", default-features = false }
 ndarray = { version = "0.15", default-features = false, features = ["std"] }
 num-traits = { version = "0.2", default-features = false }
 rand = { version = "0.8", default-features = false }
 rand_distr = { version = "0.4", default-features = false }
 serde = { version = "1.0", default-features = false, features = ["std", "derive"] }
 
 [lints]
```

### Comparing `field-compression-benchmark-0.0.2/core/model/src/boundary/periodic.rs` & `field-compression-benchmark-0.0.3/core/model/src/boundary/periodic.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 use ndarray::{SliceArg, SliceInfo, SliceInfoElem};
 
 use crate::{
     boundary::BoundaryCondition,
     model::{Model, StateViewMut},
 };
 
+#[derive(Clone, Copy)]
 pub struct PeriodicBoundary<const N: usize>;
 
 impl<L: ?Sized + Model, const N: usize> BoundaryCondition<L> for PeriodicBoundary<N>
 where
     for<'a> SliceInfo<&'a [SliceInfoElem], L::Dimension, L::Dimension>: SliceArg<L::Dimension>,
 {
     fn apply(&mut self, model: &mut L) {
```

### Comparing `field-compression-benchmark-0.0.2/core/model/src/boundary/zero.rs` & `field-compression-benchmark-0.0.3/core/model/src/boundary/zero.rs`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 use num_traits::Zero;
 
 use crate::{
     boundary::BoundaryCondition,
     model::{Model, StateViewMut},
 };
 
+#[derive(Clone, Copy)]
 pub struct ZeroBoundary<const N: usize>;
 
 impl<L: ?Sized + Model, const N: usize> BoundaryCondition<L> for ZeroBoundary<N>
 where
     L::Dimension: RemoveAxis,
 {
     fn apply(&mut self, model: &mut L) {
```

### Comparing `field-compression-benchmark-0.0.2/core/model/src/extrapolation/euler_smoothing.rs` & `field-compression-benchmark-0.0.3/core/model/src/extrapolation/euler_smoothing.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use crate::{
     extrapolation::TimeExtrapolation,
     model::{Model, State, StateView, StateViewMut},
     num::half,
 };
 
+#[derive(Clone, Copy)]
 pub struct EulerSmoothing;
 
 impl<L: ?Sized + Model> TimeExtrapolation<L> for EulerSmoothing {
     fn step(&mut self, model: &mut L, ext: &mut L::Ext, dt: L::Dtype) {
         // X_n
         let x_n = model.state().to_owned();
         // model.state = X_n
```

### Comparing `field-compression-benchmark-0.0.2/core/model/src/extrapolation/leapfrog.rs` & `field-compression-benchmark-0.0.3/core/model/src/extrapolation/leapfrog.rs`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,22 @@
 impl<L: ?Sized + Model> LeapFrog<L> {
     #[must_use]
     pub const fn new(state_prev: L::State) -> Self {
         Self { state_prev }
     }
 }
 
+impl<L: ?Sized + Model> Clone for LeapFrog<L> {
+    fn clone(&self) -> Self {
+        Self {
+            state_prev: self.state_prev.clone(),
+        }
+    }
+}
+
 impl<L: ?Sized + Model> TimeExtrapolation<L> for LeapFrog<L> {
     fn step(&mut self, model: &mut L, ext: &mut L::Ext, dt: L::Dtype) {
         // model.state = X_n
         // self.state_prev = X_(n-1)
 
         // X_(n+1) = X_(n-1) + 2 * X'_n * dt
         let mut x_np1 = model.tendencies(ext);
```

### Comparing `field-compression-benchmark-0.0.2/core/model/src/extrapolation/runge_kutta.rs` & `field-compression-benchmark-0.0.3/core/model/src/extrapolation/runge_kutta.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use crate::{
     extrapolation::TimeExtrapolation,
     model::{Model, State, StateViewMut},
     num::{half, two},
 };
 
+#[derive(Clone, Copy)]
 pub struct RungeKutta4;
 
 impl<L: ?Sized + Model> TimeExtrapolation<L> for RungeKutta4 {
     fn step(&mut self, model: &mut L, ext: &mut L::Ext, dt: L::Dtype) {
         // model.state = X_n
 
         // k1 = X'(X_n)
```

### Comparing `field-compression-benchmark-0.0.2/core/model/src/model/any.rs` & `field-compression-benchmark-0.0.3/core/model/src/model/any.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use std::any::{Any, TypeId};
 
+use dyn_clone::DynClone;
 use ndarray::{ArrayView, ArrayViewMut, IxDyn, NdFloat};
 
 use crate::model::{Model, State, StateView, StateViewMut};
 
 pub struct AnyModel<F: NdFloat> {
     model: Box<dyn 'static + ErasedModel<Dtype = F> + Send + Sync>,
 }
@@ -12,15 +13,15 @@
     #[must_use]
     pub fn new<L: 'static + Model<Dtype = F> + Send + Sync>(
         model: L,
         ext: Box<L::Ext>,
     ) -> (Self, AnyExt)
     where
         L::State: 'static + Send + Sync,
-        L::Ext: 'static + Sized + Send + Sync,
+        L::Ext: 'static + Sized + Send + Sync + Clone,
     {
         (
             Self {
                 model: Box::new(model),
             },
             AnyExt { ext },
         )
@@ -189,17 +190,29 @@
     // Safety: lifetime extension to 'static is only used to reveal the TypeId
     NonStaticAny::get_type_id(unsafe {
         std::mem::transmute::<&dyn NonStaticAny, &(dyn NonStaticAny + 'static)>(&phantom_data)
     })
 }
 
 pub struct AnyExt {
-    ext: Box<dyn 'static + AnyTypeName + Send + Sync>,
+    ext: Box<dyn 'static + ErasedExt + Send + Sync>,
 }
 
+impl Clone for AnyExt {
+    fn clone(&self) -> Self {
+        Self {
+            ext: dyn_clone::clone_box(&*self.ext),
+        }
+    }
+}
+
+trait ErasedExt: AnyTypeName + DynClone {}
+
+impl<T: AnyTypeName + DynClone> ErasedExt for T {}
+
 pub struct AnyState<F: NdFloat> {
     state: Box<dyn 'static + ErasedState<Dtype = F> + Send + Sync>,
 }
 
 impl<F: NdFloat> Clone for AnyState<F> {
     fn clone(&self) -> Self {
         ErasedState::clone(&*self.state)
```

### Comparing `field-compression-benchmark-0.0.2/core/model/src/model/linadv.rs` & `field-compression-benchmark-0.0.3/core/model/src/model/linadv.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/model/src/model/lorenz_63.rs` & `field-compression-benchmark-0.0.3/core/model/src/model/lorenz_63.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/model/src/model/lorenz_96.rs` & `field-compression-benchmark-0.0.3/core/model/src/model/lorenz_96.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use std::marker::PhantomData;
 
+use dyn_clone::DynClone;
 use ndarray::{Array, Array1, ArrayView, ArrayViewMut, Ix1, NdFloat};
 use rand::RngCore;
 use rand_distr::Distribution;
 
 use crate::model::Model;
 
 pub struct Lorenz96<F: NdFloat, S: ForcingSampler<Dtype = F>> {
@@ -48,15 +49,15 @@
     fn tendencies_for_state(
         &self,
         state: ArrayView<Self::Dtype, Self::Dimension>,
         ext: &mut Self::Ext,
     ) -> Array<Self::Dtype, Self::Dimension> {
         let Lorenz96Parameters { k: _, forcing } = &self.parameters;
 
-        let mut tendencies = Array1::zeros(state.dim());
+        let mut tendencies = state.to_owned();
 
         for (((x_k, &x_kp1), &x_km1), &x_km2) in tendencies
             .iter_mut()
             .zip(state.iter().cycle().skip(1))
             .zip(state.iter().cycle().skip(state.len() - 1))
             .zip(state.iter().cycle().skip(state.len() - 2))
         {
@@ -160,13 +161,54 @@
             _marker: PhantomData::<F>,
         }
     }
 }
 
 impl<F: NdFloat, D: Distribution<F> + Clone> ForcingSampler for Distr<F, D> {
     type Dtype = F;
-    type Ext = Box<dyn 'static + RngCore + Send + Sync>;
+    type Ext = AnyRng;
 
     fn sample(&self, ext: &mut Self::Ext) -> Self::Dtype {
-        self.distr.sample(&mut **ext)
+        self.distr.sample(ext)
     }
 }
+
+pub struct AnyRng {
+    rng: Box<dyn 'static + ClonableRngCore + Send + Sync>,
+}
+
+impl AnyRng {
+    #[must_use]
+    pub fn new(rng: impl 'static + RngCore + Clone + Send + Sync) -> Self {
+        Self { rng: Box::new(rng) }
+    }
+}
+
+impl Clone for AnyRng {
+    fn clone(&self) -> Self {
+        Self {
+            rng: dyn_clone::clone_box(&*self.rng),
+        }
+    }
+}
+
+impl RngCore for AnyRng {
+    fn next_u32(&mut self) -> u32 {
+        self.rng.next_u32()
+    }
+
+    fn next_u64(&mut self) -> u64 {
+        self.rng.next_u64()
+    }
+
+    fn fill_bytes(&mut self, dest: &mut [u8]) {
+        self.rng.fill_bytes(dest);
+    }
+
+    fn try_fill_bytes(&mut self, dest: &mut [u8]) -> Result<(), rand::Error> {
+        self.rng.try_fill_bytes(dest)
+    }
+}
+
+trait ClonableRngCore: RngCore + DynClone {}
+
+impl<T: RngCore + DynClone> ClonableRngCore for T {}
```

### Comparing `field-compression-benchmark-0.0.2/core/model/src/model/mod.rs` & `field-compression-benchmark-0.0.3/core/model/src/model/mod.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/model/src/model/onedsw.rs` & `field-compression-benchmark-0.0.3/core/model/src/model/onedsw.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/core/model/src/model/twodsw.rs` & `field-compression-benchmark-0.0.3/core/model/src/model/twodsw.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/fcbench/Cargo.toml` & `field-compression-benchmark-0.0.3/fcbench/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [package]
 name = "fcbench"
-version = "0.0.2"
+version = "0.0.3"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "fcbench"
 crate-type = ["cdylib"]
 
 [dependencies]
 codecs-build = { path = "../codecs/build", default-features = false }
 core-benchmark = { path = "../core/benchmark", default-features = false }
 core-compressor = { path = "../core/compressor", default-features = false }
 core-dataset = { path = "../core/dataset", default-features = false }
 core-error = { path = "../core/error", default-features = false }
 core-model = { path = "../core/model", default-features = false }
+dyn-clone = { version = "1.0", default-features = false }
 ndarray = { version = "0.15", default-features = false, features = ["std"] }
 numpy = { version = "0.20", default-features = false }
 pyo3 = { version = "0.20", default-features = false, features = ["macros", "abi3", "extension-module"] }
+pyo3-log = { version = "0.9", default-features = false }
 pythonize = { git = "https://github.com/juntyr/pythonize", rev = "3a1fb05", version = "0.20", default-features = false }
 rand = { version = "0.8", default-features = false }
 rand_chacha = { version = "0.3", default-features = false }
 rand_distr = { version = "0.4", default-features = false, features = ["serde1"] }
 serde = { version = "1.0", default-features = false, features = ["std"] }
 serde_path_to_error = { version = "0.1", default-features = false }
 serde-reflection = { git = "https://github.com/juntyr/serde-reflection.git", rev = "4490f20", version = "0.3", default-features = false }
```

### Comparing `field-compression-benchmark-0.0.2/fcbench/fcbench/__init__.py` & `field-compression-benchmark-0.0.3/fcbench/fcbench/__init__.py`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/fcbench/fcbench/codecs.py` & `field-compression-benchmark-0.0.3/fcbench/fcbench/codecs.py`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/fcbench/fcbench/plot.py` & `field-compression-benchmark-0.0.3/fcbench/fcbench/plot.py`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/fcbench/src/benchmark.rs` & `field-compression-benchmark-0.0.3/fcbench/src/benchmark.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/fcbench/src/compressor.rs` & `field-compression-benchmark-0.0.3/fcbench/src/compressor.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/fcbench/src/dataclass.rs` & `field-compression-benchmark-0.0.3/fcbench/src/dataclass.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/fcbench/src/dataset.rs` & `field-compression-benchmark-0.0.3/fcbench/src/dataset.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/fcbench/src/model.rs` & `field-compression-benchmark-0.0.3/fcbench/src/model.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use dyn_clone::DynClone;
 use pyo3::{intern, prelude::*, types::PyTuple};
 use serde::Deserialize;
 
 use crate::dataclass::{Dataclass, DataclassRegistry};
 
 /// Create a [`PyModule`] with name "model" that exports the [`Model`],
 /// [`TimeExtrapolation`], and [`Boundary`].
@@ -44,19 +45,14 @@
 }
 
 #[allow(clippy::unwrap_used)] // FIXME
 fn standard_normal() -> rand_distr::Normal<f64> {
     rand_distr::Normal::new(0.0, 1.0).unwrap()
 }
 
-type DynTimeExtrapolation =
-    dyn Send + core_model::extrapolation::TimeExtrapolation<core_model::model::any::AnyModel<f64>>;
-type DynBoundaryCondition =
-    dyn Send + core_model::boundary::BoundaryCondition<core_model::model::any::AnyModel<f64>>;
-
 #[pyclass(module = "fcbench.model")]
 /// A generalised multi-variable and multi-dimensional numerical model that
 /// provides mutable views into its state as the model is advanced each step.
 ///
 /// Use one of the following constructors to create a new
 /// Shallow-Water-[`Model`]:
 ///
@@ -93,16 +89,16 @@
 /// for state in model:
 ///     inspect_model_state(state)
 /// ```
 pub struct Model {
     #[allow(clippy::struct_field_names)]
     model: core_model::model::any::AnyModel<f64>,
     ext: core_model::model::any::AnyExt,
-    extrapolation: Box<DynTimeExtrapolation>,
-    boundary: Box<DynBoundaryCondition>,
+    extrapolation: Box<dyn AnyTimeExtrapolation>,
+    boundary: Box<dyn AnyBoundaryCondition>,
     dt: f64,
 }
 
 #[pymethods]
 impl Model {
     #[getter]
     /// A mutable view into the current model state.
@@ -160,14 +156,31 @@
     /// [SIGNATURE]: # "(self, /, dt: Optional[float] = None)"
     pub fn step(&mut self, dt: Option<f64>) {
         self.extrapolation
             .step(&mut self.model, &mut self.ext, dt.unwrap_or(self.dt));
         self.boundary.apply(&mut self.model);
     }
 
+    #[getter]
+    /// The default timestep `$\Delta t$` that the model uses to advance.
+    ///
+    /// [SIGNATURE]: # "(self) -> float"
+    #[must_use]
+    pub const fn dt(&self) -> f64 {
+        self.dt
+    }
+
+    /// Create a deep copy of the model.
+    ///
+    /// [SIGNATURE]: # "(self) -> Model"
+    #[must_use]
+    pub fn deepcopy(&self) -> Self {
+        Clone::clone(self)
+    }
+
     /// Use the model as a stream to iterate over the future timesteps.
     ///
     /// Each iteration of the returned iterator advances the model by a single
     /// timestep using the model's default timestep `$\Delta t$`.
     ///
     /// This method can be used to pull the next model states out of the
     /// advancing model in a for loop.
@@ -326,15 +339,15 @@
         >,
         extrapolation: &TimeExtrapolation,
         dt: f64,
         seed: u64,
     ) -> Self {
         let (model, ext) = core_model::model::any::AnyModel::new(
             core_model::model::lorenz_96::Lorenz96::new(*params),
-            Box::new(Box::new(
+            Box::new(core_model::model::lorenz_96::AnyRng::new(
                 <rand_chacha::ChaChaRng as rand_chacha::rand_core::SeedableRng>::seed_from_u64(
                     seed,
                 ),
             )),
         );
         let extrapolation = extrapolation.as_boxed(&model);
 
@@ -532,14 +545,31 @@
             extrapolation,
             boundary,
             dt,
         }
     }
 }
 
+impl Clone for Model {
+    fn clone(&self) -> Self {
+        Self {
+            model: core_model::model::Model::with_state(
+                &self.model,
+                core_model::model::StateView::to_owned(&core_model::model::Model::state(
+                    &self.model,
+                )),
+            ),
+            ext: self.ext.clone(),
+            extrapolation: dyn_clone::clone_box(&*self.extrapolation),
+            boundary: dyn_clone::clone_box(&*self.boundary),
+            dt: self.dt,
+        }
+    }
+}
+
 #[pyclass(module = "fcbench.model", frozen)]
 /// The `TimeExtrapolation` enum specifies the time extrapolation scheme that
 /// is used to advance the model by one timestep.
 ///
 /// The following options are supported:
 ///
 /// - [`TimeExtrapolation::Direct`]: The model is advanced using the direct /
@@ -640,15 +670,18 @@
     /// The model is advanced using the 4th order Runge-Kutta method, which
     /// averages the estimates of the first derivative tendencies of a field
     /// `$F$` at `$t$`, `$t + 0.5 \cdot \Delta t$`, and `$t + \Delta t$`.
     RungeKutta4,
 }
 
 impl TimeExtrapolation {
-    fn as_boxed(&self, model: &core_model::model::any::AnyModel<f64>) -> Box<DynTimeExtrapolation> {
+    fn as_boxed(
+        &self,
+        model: &core_model::model::any::AnyModel<f64>,
+    ) -> Box<dyn AnyTimeExtrapolation> {
         match self {
             Self::Direct => Box::new(core_model::extrapolation::Direct),
             Self::EulerSmoothing => Box::new(core_model::extrapolation::EulerSmoothing),
             Self::LeapFrog => Box::new(core_model::extrapolation::LeapFrog::new(
                 core_model::model::StateView::to_owned(&core_model::model::Model::state(model)),
             )),
             Self::RungeKutta4 => Box::new(core_model::extrapolation::RungeKutta4),
@@ -677,15 +710,15 @@
     /// produce a periodic domain.
     Periodic,
     /// The boundary values are constant zero.
     Zero,
 }
 
 impl Boundary {
-    fn as_boxed(&self) -> Box<DynBoundaryCondition> {
+    fn as_boxed(&self) -> Box<dyn AnyBoundaryCondition> {
         match self {
             Self::Zero => Box::new(core_model::boundary::ZeroBoundary::<1>),
             Self::Periodic => Box::new(core_model::boundary::PeriodicBoundary::<1>),
         }
     }
 }
 
@@ -700,14 +733,42 @@
     type Ext = ();
 
     fn sample(&self, _ext: &mut Self::Ext) -> Self::Dtype {
         42.0
     }
 }
 
+trait AnyTimeExtrapolation:
+    Send
+    + core_model::extrapolation::TimeExtrapolation<core_model::model::any::AnyModel<f64>>
+    + DynClone
+{
+}
+
+impl<
+        T: Send
+            + core_model::extrapolation::TimeExtrapolation<core_model::model::any::AnyModel<f64>>
+            + DynClone,
+    > AnyTimeExtrapolation for T
+{
+}
+
+trait AnyBoundaryCondition:
+    Send + core_model::boundary::BoundaryCondition<core_model::model::any::AnyModel<f64>> + DynClone
+{
+}
+
+impl<
+        T: Send
+            + core_model::boundary::BoundaryCondition<core_model::model::any::AnyModel<f64>>
+            + DynClone,
+    > AnyBoundaryCondition for T
+{
+}
+
 #[cfg(test)]
 mod tests {
     #[test]
     fn dataclass_registry() {
         let _ = super::dataclass_registry();
     }
 }
```

### Comparing `field-compression-benchmark-0.0.2/field_compression_benchmark.egg-info/PKG-INFO` & `field-compression-benchmark-0.0.3/field_compression_benchmark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: field-compression-benchmark
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data compression methods and benchmarks for Cli/Met datasets
 Author-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 Maintainer-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `field-compression-benchmark-0.0.2/fork/Cargo.toml` & `field-compression-benchmark-0.0.3/fork/Cargo.toml`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/fork/src/fork.rs` & `field-compression-benchmark-0.0.3/fork/src/fork.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/fork/src/reaper/canary.rs` & `field-compression-benchmark-0.0.3/fork/src/reaper/canary.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/fork/src/reaper/handler.rs` & `field-compression-benchmark-0.0.3/fork/src/reaper/handler.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/fork/src/reaper/mod.rs` & `field-compression-benchmark-0.0.3/fork/src/reaper/mod.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/fork/src/reaper/worker.rs` & `field-compression-benchmark-0.0.3/fork/src/reaper/worker.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/fork/src/work.rs` & `field-compression-benchmark-0.0.3/fork/src/work.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/pyproject.toml` & `field-compression-benchmark-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel", "setuptools-rust"]
 
 [project]
 name = "field-compression-benchmark"
-version = "0.0.2"
+version = "0.0.3"
 requires-python = ">=3.10"
 description = "Data compression methods and benchmarks for Cli/Met datasets"
 license = { file = "LICENSE-APACHE" }
 authors = [
     { name = "Juniper Tyree", email = "juniper.tyree@helsinki.fi" }
 ]
 maintainers = [
@@ -48,15 +48,15 @@
 [[tool.setuptools-rust.ext-modules]]
 target = "fcbench._fcbench"
 path = "fcbench/Cargo.toml"
 binding = "PyO3"
 
 [tool.poetry]
 name = "field-compression-benchmark"
-version = "0.0.2"
+version = "0.0.3"
 description = "field-compression-benchmark Python environment"
 authors = ["Juniper Tyree <juniper.tyree@helsinki.fi>"]
 package-mode = false
 
 [tool.poetry.dependencies]
 python = "~3.11"
 cfgrib = "0.9.10.4"
```

### Comparing `field-compression-benchmark-0.0.2/setup.py` & `field-compression-benchmark-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/src/args.rs` & `field-compression-benchmark-0.0.3/src/args.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/src/benchmarking/mod.rs` & `field-compression-benchmark-0.0.3/src/benchmarking/mod.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/src/benchmarking/prepare.rs` & `field-compression-benchmark-0.0.3/src/benchmarking/prepare.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/src/benchmarking/report.rs` & `field-compression-benchmark-0.0.3/src/benchmarking/report.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/src/fcpy.rs` & `field-compression-benchmark-0.0.3/src/fcpy.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/src/main.rs` & `field-compression-benchmark-0.0.3/src/main.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/wasi/build/build.rs` & `field-compression-benchmark-0.0.3/wasi/build/build.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/wasi/cli/src/stdio.rs` & `field-compression-benchmark-0.0.3/wasi/cli/src/stdio.rs`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,30 @@
     bindings::{
         exports::wasi::cli::{
             stderr::Guest as WasiCliStderr, stdin::Guest as WasiCliStdin,
             stdout::Guest as WasiCliStdout,
         },
         wasi::{
             io::streams::{InputStream, OutputStream},
-            virt::null_io::{closed_input, output_sink},
+            null::io::{closed_input, stderr, stdout},
         },
     },
     VirtCli,
 };
 
 impl WasiCliStdin for VirtCli {
     fn get_stdin() -> InputStream {
         closed_input()
     }
 }
 
 impl WasiCliStdout for VirtCli {
     fn get_stdout() -> OutputStream {
-        output_sink()
+        stdout()
     }
 }
 
 impl WasiCliStderr for VirtCli {
     fn get_stderr() -> OutputStream {
-        output_sink()
+        stderr()
     }
 }
```

### Comparing `field-compression-benchmark-0.0.2/wasi/cli/src/terminal.rs` & `field-compression-benchmark-0.0.3/wasi/cli/src/terminal.rs`

 * *Files identical despite different names*

### Comparing `field-compression-benchmark-0.0.2/wasi/clocks/src/lib.rs` & `field-compression-benchmark-0.0.3/wasi/clocks/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,25 @@
 use std::sync::atomic::{AtomicU64, Ordering};
 
 use crate::bindings::{
     exports::wasi::clocks::{
         monotonic_clock::{Duration, Guest as WasiClocksMonotonicClock, Instant},
         wall_clock::{Datetime, Guest as WasiClocksWallClock},
     },
-    wasi::{io::poll::Pollable, virt::null_io::ready_pollable},
+    wasi::{io::poll::Pollable, null::io::ready_pollable},
 };
 
 #[allow(clippy::missing_safety_doc, clippy::transmute_int_to_bool)]
 mod bindings {
-    wit_bindgen::generate!({
-        path: "../wit",
-        world: "virtual-wasi-clocks",
-    });
+    wit_bindgen::generate!("fcbench:wasi/virtual-clocks");
 }
 
 pub enum VirtClock {}
 
+#[cfg(target_arch = "wasm32")]
 #[allow(unsafe_code)]
 mod export {
     use crate::VirtClock;
     crate::bindings::export!(VirtClock with_types_in crate::bindings);
 }
 
 static CLOCK_NS: AtomicU64 = AtomicU64::new(0);
```

### Comparing `field-compression-benchmark-0.0.2/wasi/filesystem/src/lib.rs` & `field-compression-benchmark-0.0.3/wasi/filesystem/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,20 @@
         error::Error,
         streams::{InputStream, OutputStream},
     },
 };
 
 #[allow(clippy::missing_safety_doc, clippy::transmute_int_to_bool)]
 mod bindings {
-    wit_bindgen::generate!({
-        path: "../wit",
-        world: "virtual-wasi-filesystem",
-    });
+    wit_bindgen::generate!("fcbench:wasi/virtual-filesystem");
 }
 
 pub enum VirtFilesystem {}
 
+#[cfg(target_arch = "wasm32")]
 #[allow(unsafe_code)]
 mod export {
     use crate::VirtFilesystem;
     crate::bindings::export!(VirtFilesystem with_types_in crate::bindings);
 }
 
 pub enum VirtDescriptor {}
```

### Comparing `field-compression-benchmark-0.0.2/wasi/io/src/lib.rs` & `field-compression-benchmark-0.0.3/wasi/io/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 #![cfg_attr(not(test), no_main)]
 
 use crate::bindings::exports::wasi::{
     io::{
         poll::Pollable,
         streams::{InputStream, OutputStream},
     },
-    virt::null_io::Guest as WasiVirtNullIO,
+    null::io::Guest as WasiVirtNullIO,
 };
 
 pub mod error;
 pub mod poll;
 pub mod streams;
 
 #[allow(clippy::missing_safety_doc)]
 mod bindings {
-    wit_bindgen::generate!({
-        path: "../wit",
-        world: "virtual-wasi-io",
-    });
+    wit_bindgen::generate!("fcbench:wasi/virtual-io");
 }
 
 pub enum VirtIO {}
 
+#[cfg(target_arch = "wasm32")]
 #[allow(unsafe_code)]
 mod export {
     use crate::VirtIO;
     crate::bindings::export!(VirtIO with_types_in crate::bindings);
 }
 
 impl WasiVirtNullIO for VirtIO {
@@ -36,8 +34,16 @@
     fn closed_input() -> InputStream {
         streams::VirtInputStream::closed()
     }
 
     fn output_sink() -> OutputStream {
         streams::VirtOutputStream::sink()
     }
+
+    fn stdout() -> OutputStream {
+        streams::VirtOutputStream::stdout()
+    }
+
+    fn stderr() -> OutputStream {
+        streams::VirtOutputStream::stderr()
+    }
 }
```

### Comparing `field-compression-benchmark-0.0.2/wasi/io/src/poll.rs` & `field-compression-benchmark-0.0.3/wasi/io/src/poll.rs`

 * *Files 17% similar despite different names*

```diff
@@ -9,25 +9,28 @@
     type Pollable = VirtPollable;
 
     fn poll(r#in: Vec<PollableBorrow>) -> Vec<u32> {
         (0..).take(r#in.len()).collect()
     }
 }
 
-pub struct VirtPollable;
+#[non_exhaustive]
+pub enum VirtPollable {
+    Ready,
+}
 
 impl GuestPollable for VirtPollable {
     fn ready(&self) -> bool {
         true
     }
 
     fn block(&self) {
         // no-op
     }
 }
 
 impl VirtPollable {
     #[must_use]
     pub fn ready() -> Pollable {
-        Pollable::new(Self)
+        Pollable::new(Self::Ready)
     }
 }
```

### Comparing `field-compression-benchmark-0.0.2/wasi/random/src/lib.rs` & `field-compression-benchmark-0.0.3/wasi/random/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,20 @@
     exports::wasi::random::{
         insecure::Guest as WasiRandomInsecure, insecure_seed::Guest as WasiRandomInsecureSeed,
     },
     // wasi::random::insecure_seed::insecure_seed as insecure_seed_host,
 };
 
 mod bindings {
-    wit_bindgen::generate!({
-        path: "../wit",
-        world: "virtual-wasi-random",
-    });
+    wit_bindgen::generate!("fcbench:wasi/virtual-random");
 }
 
 pub enum VirtRandom {}
 
+#[cfg(target_arch = "wasm32")]
 #[allow(unsafe_code)]
 mod export {
     use crate::VirtRandom;
     crate::bindings::export!(VirtRandom with_types_in crate::bindings);
 }
 
 fn rng() -> MutexGuard<'static, Pcg64> {
```

