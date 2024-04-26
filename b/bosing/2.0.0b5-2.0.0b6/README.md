# Comparing `tmp/bosing-2.0.0b5.tar.gz` & `tmp/bosing-2.0.0b6.tar.gz`

## Comparing `bosing-2.0.0b5.tar` & `bosing-2.0.0b6.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 bosing-2.0.0b5/Cargo.toml
--rw-r--r--   0     1001      127      505 2024-04-25 06:57:50.000000 bosing-2.0.0b5/.github/dependabot.yml
--rw-r--r--   0     1001      127     6307 2024-04-25 06:57:50.000000 bosing-2.0.0b5/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      696 2024-04-25 06:57:50.000000 bosing-2.0.0b5/.gitignore
--rw-r--r--   0     1001      127      972 2024-04-25 06:57:50.000000 bosing-2.0.0b5/.readthedocs.yaml
--rw-r--r--   0     1001      127     1068 2024-04-25 06:57:50.000000 bosing-2.0.0b5/LICENSE.txt
--rw-r--r--   0     1001      127     1348 2024-04-25 06:57:50.000000 bosing-2.0.0b5/README.md
--rw-r--r--   0     1001      127    10244 2024-04-25 06:57:50.000000 bosing-2.0.0b5/bosing.pyi
--rw-r--r--   0     1001      127      634 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/Makefile
--rw-r--r--   0     1001      127      175 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      127     1147 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/_templates/autosummary/module.rst
--rw-r--r--   0     1001      127       82 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/api.rst
--rw-r--r--   0     1001      127     1464 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/conf.py
--rw-r--r--   0     1001      127     1258 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/index.rst
--rw-r--r--   0     1001      127     1716 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/instruction.rst
--rw-r--r--   0     1001      127      765 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/make.bat
--rw-r--r--   0     1001      127      347 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/quickstart.rst
--rw-r--r--   0     1001      127       16 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/requirements.txt
--rw-r--r--   0     1001      127     5534 2024-04-25 06:57:50.000000 bosing-2.0.0b5/docs/schedule.rst
--rw-r--r--   0     1001      127     1138 2024-04-25 06:57:50.000000 bosing-2.0.0b5/example/flexible.py
--rw-r--r--   0     1001      127      521 2024-04-25 06:57:50.000000 bosing-2.0.0b5/example/hann.py
--rw-r--r--   0     1001      127      770 2024-04-25 06:57:50.000000 bosing-2.0.0b5/example/interp.py
--rw-r--r--   0     1001      127      682 2024-04-25 06:57:50.000000 bosing-2.0.0b5/example/overlap.py
--rw-r--r--   0     1001      127     2219 2024-04-25 06:57:50.000000 bosing-2.0.0b5/example/schedule.py
--rw-r--r--   0     1001      127     2028 2024-04-25 06:57:50.000000 bosing-2.0.0b5/example/schedule_stress.py
--rw-r--r--   0     1001      127     6064 2024-04-25 06:57:50.000000 bosing-2.0.0b5/ruff_defaults.toml
--rw-r--r--   0     1001      127     7351 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/executor.rs
--rw-r--r--   0     1001      127    62068 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/lib.rs
--rw-r--r--   0     1001      127    11167 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/pulse.rs
--rw-r--r--   0     1001      127     1667 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/quant.rs
--rw-r--r--   0     1001      127     2479 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/schedule/absolute.rs
--rw-r--r--   0     1001      127     7387 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/schedule/grid.rs
--rw-r--r--   0     1001      127     3311 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/schedule/play.rs
--rw-r--r--   0     1001      127     2349 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/schedule/repeat.rs
--rw-r--r--   0     1001      127     3944 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/schedule/simple.rs
--rw-r--r--   0     1001      127     5741 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/schedule/stack.rs
--rw-r--r--   0     1001      127    11082 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/schedule.rs
--rw-r--r--   0     1001      127     6649 2024-04-25 06:57:50.000000 bosing-2.0.0b5/src/shape.rs
--rw-r--r--   0     1001      127       14 2024-04-25 06:57:50.000000 bosing-2.0.0b5/stubtest-allowlist.txt
--rw-r--r--   0     1001      127        0 2024-04-25 06:57:50.000000 bosing-2.0.0b5/tests/__init__.py
--rw-r--r--   0     1001      127     1171 2024-04-25 06:57:50.000000 bosing-2.0.0b5/tests/test_basic.py
--rw-r--r--   0     1001      127    18030 2024-04-25 06:58:08.000000 bosing-2.0.0b5/Cargo.lock
--rw-r--r--   0     1001      127     1867 2024-04-25 06:57:50.000000 bosing-2.0.0b5/pyproject.toml
--rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 bosing-2.0.0b5/PKG-INFO
+-rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 bosing-2.0.0b6/Cargo.toml
+-rw-r--r--   0     1001      127      505 2024-04-26 03:57:23.000000 bosing-2.0.0b6/.github/dependabot.yml
+-rw-r--r--   0     1001      127     6323 2024-04-26 03:57:23.000000 bosing-2.0.0b6/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      696 2024-04-26 03:57:23.000000 bosing-2.0.0b6/.gitignore
+-rw-r--r--   0     1001      127      972 2024-04-26 03:57:23.000000 bosing-2.0.0b6/.readthedocs.yaml
+-rw-r--r--   0     1001      127     1068 2024-04-26 03:57:23.000000 bosing-2.0.0b6/LICENSE.txt
+-rw-r--r--   0     1001      127     1348 2024-04-26 03:57:23.000000 bosing-2.0.0b6/README.md
+-rw-r--r--   0     1001      127    10185 2024-04-26 03:57:23.000000 bosing-2.0.0b6/bosing.pyi
+-rw-r--r--   0     1001      127       78 2024-04-26 03:57:23.000000 bosing-2.0.0b6/clippy.toml
+-rw-r--r--   0     1001      127      634 2024-04-26 03:57:23.000000 bosing-2.0.0b6/docs/Makefile
+-rw-r--r--   0     1001      127      175 2024-04-26 03:57:23.000000 bosing-2.0.0b6/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      127     1147 2024-04-26 03:57:23.000000 bosing-2.0.0b6/docs/_templates/autosummary/module.rst
+-rw-r--r--   0     1001      127       82 2024-04-26 03:57:23.000000 bosing-2.0.0b6/docs/api.rst
+-rw-r--r--   0     1001      127     1464 2024-04-26 03:57:23.000000 bosing-2.0.0b6/docs/conf.py
+-rw-r--r--   0     1001      127     1258 2024-04-26 03:57:23.000000 bosing-2.0.0b6/docs/index.rst
+-rw-r--r--   0     1001      127     1716 2024-04-26 03:57:23.000000 bosing-2.0.0b6/docs/instruction.rst
+-rw-r--r--   0     1001      127      765 2024-04-26 03:57:23.000000 bosing-2.0.0b6/docs/make.bat
+-rw-r--r--   0     1001      127      347 2024-04-26 03:57:23.000000 bosing-2.0.0b6/docs/quickstart.rst
+-rw-r--r--   0     1001      127       22 2024-04-26 03:57:23.000000 bosing-2.0.0b6/docs/requirements.txt
+-rw-r--r--   0     1001      127     5534 2024-04-26 03:57:23.000000 bosing-2.0.0b6/docs/schedule.rst
+-rw-r--r--   0     1001      127     1179 2024-04-26 03:57:23.000000 bosing-2.0.0b6/example/flexible.py
+-rw-r--r--   0     1001      127      537 2024-04-26 03:57:23.000000 bosing-2.0.0b6/example/hann.py
+-rw-r--r--   0     1001      127      792 2024-04-26 03:57:23.000000 bosing-2.0.0b6/example/interp.py
+-rw-r--r--   0     1001      127      700 2024-04-26 03:57:23.000000 bosing-2.0.0b6/example/overlap.py
+-rw-r--r--   0     1001      127     2090 2024-04-26 03:57:23.000000 bosing-2.0.0b6/example/schedule.py
+-rw-r--r--   0     1001      127     1924 2024-04-26 03:57:23.000000 bosing-2.0.0b6/example/schedule_stress.py
+-rw-r--r--   0     1001      127     6064 2024-04-26 03:57:23.000000 bosing-2.0.0b6/ruff_defaults.toml
+-rw-r--r--   0     1001      127     7368 2024-04-26 03:57:23.000000 bosing-2.0.0b6/src/executor.rs
+-rw-r--r--   0     1001      127    62006 2024-04-26 03:57:23.000000 bosing-2.0.0b6/src/lib.rs
+-rw-r--r--   0     1001      127    12086 2024-04-26 03:57:23.000000 bosing-2.0.0b6/src/pulse.rs
+-rw-r--r--   0     1001      127     1667 2024-04-26 03:57:23.000000 bosing-2.0.0b6/src/quant.rs
+-rw-r--r--   0     1001      127     2481 2024-04-26 03:57:23.000000 bosing-2.0.0b6/src/schedule/absolute.rs
+-rw-r--r--   0     1001      127     7389 2024-04-26 03:57:23.000000 bosing-2.0.0b6/src/schedule/grid.rs
+-rw-r--r--   0     1001      127     3326 2024-04-26 03:57:23.000000 bosing-2.0.0b6/src/schedule/play.rs
+-rw-r--r--   0     1001      127     2350 2024-04-26 03:57:23.000000 bosing-2.0.0b6/src/schedule/repeat.rs
+-rw-r--r--   0     1001      127     3966 2024-04-26 03:57:23.000000 bosing-2.0.0b6/src/schedule/simple.rs
+-rw-r--r--   0     1001      127     5760 2024-04-26 03:57:23.000000 bosing-2.0.0b6/src/schedule/stack.rs
+-rw-r--r--   0     1001      127    11083 2024-04-26 03:57:23.000000 bosing-2.0.0b6/src/schedule.rs
+-rw-r--r--   0     1001      127     6649 2024-04-26 03:57:23.000000 bosing-2.0.0b6/src/shape.rs
+-rw-r--r--   0     1001      127       14 2024-04-26 03:57:23.000000 bosing-2.0.0b6/stubtest-allowlist.txt
+-rw-r--r--   0     1001      127        0 2024-04-26 03:57:23.000000 bosing-2.0.0b6/tests/__init__.py
+-rw-r--r--   0     1001      127     1204 2024-04-26 03:57:23.000000 bosing-2.0.0b6/tests/test_basic.py
+-rw-r--r--   0     1001      127    19274 2024-04-26 03:57:28.000000 bosing-2.0.0b6/Cargo.lock
+-rw-r--r--   0     1001      127     1867 2024-04-26 03:57:23.000000 bosing-2.0.0b6/pyproject.toml
+-rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 bosing-2.0.0b6/PKG-INFO
```

### Comparing `bosing-2.0.0b5/.github/workflows/ci.yml` & `bosing-2.0.0b6/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         platform:
           - runner: ubuntu-latest
             target: x86_64
     steps:
       - uses: actions/checkout@v4
       - name: Replace version in Cargo.toml
         shell: pwsh
-        run: (Get-Content -Path Cargo.toml -Raw) -replace 'version = ".*"', 'version = "${{ needs.release.outputs.version }}"' | Set-Content -Path Cargo.toml
+        run: (Get-Content -Path Cargo.toml) -replace '^version = "0.0.0-dev"$', 'version = "${{ needs.release.outputs.version }}"' | Set-Content -Path Cargo.toml
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.platform.target }}
@@ -118,15 +118,15 @@
             target: x64
           - runner: windows-latest
             target: x86
     steps:
       - uses: actions/checkout@v4
       - name: Replace version in Cargo.toml
         shell: pwsh
-        run: (Get-Content -Path Cargo.toml -Raw) -replace 'version = ".*"', 'version = "${{ needs.release.outputs.version }}"' | Set-Content -Path Cargo.toml
+        run: (Get-Content -Path Cargo.toml) -replace '^version = "0.0.0-dev"$', 'version = "${{ needs.release.outputs.version }}"' | Set-Content -Path Cargo.toml
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
           architecture: ${{ matrix.platform.target }}
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
@@ -149,15 +149,15 @@
             target: x86_64
           - runner: macos-14
             target: aarch64
     steps:
       - uses: actions/checkout@v4
       - name: Replace version in Cargo.toml
         shell: pwsh
-        run: (Get-Content -Path Cargo.toml -Raw) -replace 'version = ".*"', 'version = "${{ needs.release.outputs.version }}"' | Set-Content -Path Cargo.toml
+        run: (Get-Content -Path Cargo.toml) -replace '^version = "0.0.0-dev"$', 'version = "${{ needs.release.outputs.version }}"' | Set-Content -Path Cargo.toml
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON_VERSION }}
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.platform.target }}
@@ -172,15 +172,15 @@
   sdist:
     runs-on: ubuntu-latest
     needs: release
     steps:
       - uses: actions/checkout@v4
       - name: Replace version in Cargo.toml
         shell: pwsh
-        run: (Get-Content -Path Cargo.toml -Raw) -replace 'version = ".*"', 'version = "${{ needs.release.outputs.version }}"' | Set-Content -Path Cargo.toml
+        run: (Get-Content -Path Cargo.toml) -replace '^version = "0.0.0-dev"$', 'version = "${{ needs.release.outputs.version }}"' | Set-Content -Path Cargo.toml
       - name: Build sdist
         uses: PyO3/maturin-action@v1
         with:
           command: sdist
           args: --out dist
       - name: Upload sdist
         uses: actions/upload-artifact@v4
```

### Comparing `bosing-2.0.0b5/.gitignore` & `bosing-2.0.0b6/.gitignore`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b5/.readthedocs.yaml` & `bosing-2.0.0b6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b5/LICENSE.txt` & `bosing-2.0.0b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b5/README.md` & `bosing-2.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b5/bosing.pyi` & `bosing-2.0.0b6/bosing.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-from collections.abc import Iterable, Sequence
+from collections.abc import Iterable, Mapping, Sequence
 from typing import ClassVar, Literal, Self, TypeAlias, final
 
 import numpy as np
 import numpy.typing as npt
 
 @final
 class Channel:
     def __new__(
         cls,
-        name: str,
         base_freq: float,
         sample_rate: float,
         length: int,
         *,
         delay: float = ...,
         align_level: int = ...,
     ) -> Self: ...
     @property
-    def name(self) -> str: ...
-    @property
     def base_freq(self) -> float: ...
     @property
     def sample_rate(self) -> float: ...
     @property
     def length(self) -> int: ...
     @property
     def delay(self) -> float: ...
@@ -68,16 +65,16 @@
     @property
     def min_duration(self) -> float: ...
 
 @final
 class Play(Element):
     def __new__(
         cls,
-        channel_id: int,
-        shape_id: int | None,
+        channel_id: str,
+        shape_id: str | None,
         amplitude: float,
         width: float,
         *,
         plateau: float = ...,
         drag_coef: float = ...,
         frequency: float = ...,
         phase: float = ...,
@@ -86,17 +83,17 @@
         alignment: Literal["end", "start", "center", "stretch"] | Alignment | None = ...,
         phantom: bool = ...,
         duration: float | None = ...,
         max_duration: float = ...,
         min_duration: float = ...,
     ) -> Self: ...
     @property
-    def channel_id(self) -> int: ...
+    def channel_id(self) -> str: ...
     @property
-    def shape_id(self) -> int | None: ...
+    def shape_id(self) -> str | None: ...
     @property
     def amplitude(self) -> float: ...
     @property
     def width(self) -> float: ...
     @property
     def plateau(self) -> float: ...
     @property
@@ -108,119 +105,119 @@
     @property
     def flexible(self) -> bool: ...
 
 @final
 class ShiftPhase(Element):
     def __new__(
         cls,
-        channel_id: int,
+        channel_id: str,
         phase: float,
         *,
         margin: float | tuple[float, float] | None = ...,
         alignment: Literal["end", "start", "center", "stretch"] | Alignment | None = ...,
         phantom: bool = ...,
         duration: float | None = ...,
         max_duration: float = ...,
         min_duration: float = ...,
     ) -> Self: ...
     @property
-    def channel_id(self) -> int: ...
+    def channel_id(self) -> str: ...
     @property
     def phase(self) -> float: ...
 
 @final
 class SetPhase(Element):
     def __new__(
         cls,
-        channel_id: int,
+        channel_id: str,
         phase: float,
         *,
         margin: float | tuple[float, float] | None = ...,
         alignment: Literal["end", "start", "center", "stretch"] | Alignment | None = ...,
         phantom: bool = ...,
         duration: float | None = ...,
         max_duration: float = ...,
         min_duration: float = ...,
     ) -> Self: ...
     @property
-    def channel_id(self) -> int: ...
+    def channel_id(self) -> str: ...
     @property
     def phase(self) -> float: ...
 
 @final
 class ShiftFreq(Element):
     def __new__(
         cls,
-        channel_id: int,
+        channel_id: str,
         frequency: float,
         *,
         margin: float | tuple[float, float] | None = ...,
         alignment: Literal["end", "start", "center", "stretch"] | Alignment | None = ...,
         phantom: bool = ...,
         duration: float | None = ...,
         max_duration: float = ...,
         min_duration: float = ...,
     ) -> Self: ...
     @property
-    def channel_id(self) -> int: ...
+    def channel_id(self) -> str: ...
     @property
     def frequency(self) -> float: ...
 
 @final
 class SetFreq(Element):
     def __new__(
         cls,
-        channel_id: int,
+        channel_id: str,
         frequency: float,
         *,
         margin: float | tuple[float, float] | None = ...,
         alignment: Literal["end", "start", "center", "stretch"] | Alignment | None = ...,
         phantom: bool = ...,
         duration: float | None = ...,
         max_duration: float = ...,
         min_duration: float = ...,
     ) -> Self: ...
     @property
-    def channel_id(self) -> int: ...
+    def channel_id(self) -> str: ...
     @property
     def frequency(self) -> float: ...
 
 @final
 class SwapPhase(Element):
     def __new__(
         cls,
-        channel_id1: int,
-        channel_id2: int,
+        channel_id1: str,
+        channel_id2: str,
         *,
         margin: float | tuple[float, float] | None = ...,
         alignment: Literal["end", "start", "center", "stretch"] | Alignment | None = ...,
         phantom: bool = ...,
         duration: float | None = ...,
         max_duration: float = ...,
         min_duration: float = ...,
     ) -> Self: ...
     @property
-    def channel_id1(self) -> int: ...
+    def channel_id1(self) -> str: ...
     @property
-    def channel_id2(self) -> int: ...
+    def channel_id2(self) -> str: ...
 
 @final
 class Barrier(Element):
     def __new__(
         cls,
-        *channel_ids: int,
+        *channel_ids: str,
         margin: float | tuple[float, float] | None = ...,
         alignment: Literal["end", "start", "center", "stretch"] | Alignment | None = ...,
         phantom: bool = ...,
         duration: float | None = ...,
         max_duration: float = ...,
         min_duration: float = ...,
     ) -> Self: ...
     @property
-    def channel_ids(self) -> Sequence[int]: ...
+    def channel_ids(self) -> Sequence[str]: ...
 
 @final
 class Repeat(Element):
     def __new__(
         cls,
         child: Element,
         count: int,
@@ -349,17 +346,16 @@
     ) -> Grid: ...
     @property
     def children(self) -> Sequence[GridEntry]: ...
     @property
     def columns(self) -> Sequence[GridLength]: ...
 
 def generate_waveforms(
-    channels: Iterable[Channel],
-    shapes: Iterable[Shape],
+    channels: Mapping[str, Channel],
+    shapes: Mapping[str, Shape],
     schedule: Element,
     *,
     time_tolerance: float = ...,
     amp_tolerance: float = ...,
-    phase_tolerance: float = ...,
     allow_oversize: bool = ...,
-    crosstalk: npt.ArrayLike | None = ...,
+    crosstalk: tuple[npt.ArrayLike, Sequence[str]] | None = ...,
 ) -> dict[str, np.ndarray]: ...
```

### Comparing `bosing-2.0.0b5/docs/Makefile` & `bosing-2.0.0b6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b5/docs/_templates/autosummary/module.rst` & `bosing-2.0.0b6/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b5/docs/conf.py` & `bosing-2.0.0b6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b5/docs/index.rst` & `bosing-2.0.0b6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b5/docs/instruction.rst` & `bosing-2.0.0b6/docs/instruction.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b5/docs/make.bat` & `bosing-2.0.0b6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b5/docs/schedule.rst` & `bosing-2.0.0b6/docs/schedule.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b5/example/flexible.py` & `bosing-2.0.0b6/example/flexible.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import matplotlib.pyplot as plt
 
 from bosing import Barrier, Channel, Grid, Hann, Play, Repeat, Stack, generate_waveforms
 
-channels = [Channel("xy", 30e6, 2e9, 1000), Channel("u", 0, 2e9, 1000)]
-shapes = [Hann()]
+channels = {
+    "xy": Channel(30e6, 2e9, 1000),
+    "u": Channel(0, 2e9, 1000),
+}
+shapes = {
+    "hann": Hann(),
+}
 grid = Grid(columns=[40e-9, "auto", 40e-9]).with_children(
     # flexible u pulse spanning 3 columns
     (
         Play(
-            channel_id=1,
-            shape_id=0,
+            channel_id="u",
+            shape_id="hann",
             amplitude=0.5,
             width=60e-9,
             alignment="stretch",
             flexible=True,
         ),
         0,
         3,
     ),
     # xy pulse in the middle column
     (
         Repeat(
             Play(
-                channel_id=0,
-                shape_id=0,
+                channel_id="xy",
+                shape_id="hann",
                 amplitude=0.3,
                 width=60e-9,
             ),
             count=3,
             spacing=30e-9,
         ),
         1,
```

### Comparing `bosing-2.0.0b5/example/hann.py` & `bosing-2.0.0b6/example/hann.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import matplotlib.pyplot as plt
 
 from bosing import Barrier, Channel, Hann, Play, Stack, generate_waveforms
 
-channels = [Channel("xy", 30e6, 2e9, 1000)]
-shapes = [Hann()]
+channels = {"xy": Channel(30e6, 2e9, 1000)}
+shapes = {"hann": Hann()}
 schedule = Stack(duration=500e-9).with_children(
     Play(
-        channel_id=0,
-        shape_id=0,
+        channel_id="xy",
+        shape_id="hann",
         amplitude=0.3,
         width=100e-9,
         plateau=200e-9,
     ),
     Barrier(duration=10e-9),
 )
 result = generate_waveforms(channels, shapes, schedule)
```

### Comparing `bosing-2.0.0b5/example/interp.py` & `bosing-2.0.0b6/example/interp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.interpolate import make_interp_spline
 
 from bosing import Barrier, Channel, Interp, Play, Stack, generate_waveforms
 
-channels = [Channel("xy", 0, 2e9, 1000)]
+channels = {"xy": Channel(0, 2e9, 1000)}
 # x should be in the range [-0.5, 0.5]
 x = np.linspace(-0.5, 0.5, 20)
 y = np.cos(np.pi * x)
 interp = make_interp_spline(x, y)
 knots = interp.t
 controls = interp.c
 degree = interp.k
-shapes = [Interp(knots, controls, degree)]
+shapes = {"halfcos": Interp(knots, controls, degree)}
 schedule = Stack(duration=500e-9).with_children(
     Play(
-        channel_id=0,
-        shape_id=0,
+        channel_id="xy",
+        shape_id="halfcos",
         amplitude=0.3,
         width=100e-9,
     ),
     Barrier(duration=10e-9),
 )
 result = generate_waveforms(channels, shapes, schedule)
 w = result["xy"]
```

### Comparing `bosing-2.0.0b5/example/overlap.py` & `bosing-2.0.0b6/example/overlap.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import matplotlib.pyplot as plt
 
 from bosing import Absolute, Barrier, Channel, Hann, Play, Stack, generate_waveforms
 
-channels = [Channel("m", 0, 2e9, 1000)]
-shapes = [Hann()]
+channels = {"m": Channel(30e6, 2e9, 1000)}
+shapes = {"hann": Hann()}
 measure = Absolute().with_children(
     *[
         Play(
-            channel_id=0,
-            shape_id=0,
+            channel_id="m",
+            shape_id="hann",
             amplitude=0.3,
             width=100e-9,
             plateau=300e-9,
             frequency=40e6 * i + 60e6,
         )
         for i in range(2)
     ]
```

### Comparing `bosing-2.0.0b5/example/schedule.py` & `bosing-2.0.0b6/example/schedule.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,42 +4,40 @@
 from matplotlib import pyplot as plt
 from scipy.interpolate import make_interp_spline
 
 from bosing import Absolute, Barrier, Channel, Grid, Hann, Interp, Play, Repeat, ShiftPhase, Stack, generate_waveforms
 
 if __name__ == "__main__":
     length = 100000
-    channels = [
-        Channel("xy0", 0, 2e9, length),
-        Channel("xy1", 0, 2e9, length),
-        Channel("u0", 0, 2e9, length),
-        Channel("u1", 0, 2e9, length),
-        Channel("m0", 0, 2e9, length),
-    ]
-    c = {ch.name: i for i, ch in enumerate(channels)}
+    channels = {
+        "xy0": Channel(0, 2e9, length),
+        "xy1": Channel(0, 2e9, length),
+        "u0": Channel(0, 2e9, length),
+        "u1": Channel(0, 2e9, length),
+        "m0": Channel(0, 2e9, length),
+    }
     halfcos = np.sin(np.linspace(0, np.pi, 10))
     interp = make_interp_spline(np.linspace(-0.5, 0.5, 10), halfcos)
-    shapes = [
-        Hann(),
-        Interp(interp.t, interp.c, interp.k),
-    ]
-    s = {"hann": 0, "rect": None, "halfcos": 1}
+    shapes = {
+        "hann": Hann(),
+        "halfcos": Interp(interp.t, interp.c, interp.k),
+    }
 
     measure = Absolute(
-        Play(c["m0"], s["hann"], 0.1, 30e-9, plateau=1e-6, frequency=123e6),
-        Play(c["m0"], s["hann"], 0.15, 30e-9, plateau=1e-6, frequency=-233e6),
+        Play("m0", "hann", 0.1, 30e-9, plateau=1e-6, frequency=123e6),
+        Play("m0", "hann", 0.15, 30e-9, plateau=1e-6, frequency=-233e6),
     )
     c01 = Stack(
-        Play(c["u0"], s["rect"], 0.5, 50e-9),
-        Play(c["u1"], s["rect"], 0.5, 50e-9),
-        ShiftPhase(c["xy0"], 0.1),
-        ShiftPhase(c["xy1"], 0.2),
+        Play("u0", None, 0.5, 50e-9),
+        Play("u1", None, 0.5, 50e-9),
+        ShiftPhase("xy0", 0.1),
+        ShiftPhase("xy1", 0.2),
     )
-    x0 = Play(c["xy0"], s["hann"], 0.3, 50e-9, drag_coef=5e-10)
-    x1 = Play(c["xy1"], s["hann"], 0.4, 100e-9, drag_coef=3e-10)
+    x0 = Play("xy0", "hann", 0.3, 50e-9, drag_coef=5e-10)
+    x1 = Play("xy1", "hann", 0.4, 100e-9, drag_coef=3e-10)
     x_group = Grid(
         Stack(x0, alignment="center"),
         Stack(x1, alignment="center"),
     )
 
     schedule = Stack(duration=50e-6).with_children(
         Repeat(
```

### Comparing `bosing-2.0.0b5/example/schedule_stress.py` & `bosing-2.0.0b6/example/schedule_stress.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,33 +11,31 @@
 
 def gen_n(n: int):
     t0 = time.perf_counter()
     nxy = 64
     nu = 2 * nxy
     nm = nxy // 8
     channels = (
-        [Channel(f"xy{i}", 3e6 * i, 2e9, 100000) for i in range(nxy)]
-        + [Channel(f"u{i}", 0, 2e9, 100000) for i in range(nu)]
-        + [Channel(f"m{i}", 0, 2e9, 100000) for i in range(nm)]
+        {f"xy{i}": Channel(3e6 * i, 2e9, 100000) for i in range(nxy)}
+        | {f"u{i}": Channel(0, 2e9, 100000) for i in range(nu)}
+        | {f"m{i}": Channel(0, 2e9, 100000) for i in range(nm)}
     )
-    c = {ch.name: i for i, ch in enumerate(channels)}
     halfcos = np.sin(np.linspace(0, np.pi, 10))
     spline = make_interp_spline(np.linspace(-0.5, 0.5, 10), halfcos)
-    shapes = [
-        Hann(),
-        Interp(spline.t, spline.c, spline.k),
-    ]
-    s = {"hann": 0, "rect": None, "halfcos": 1}
+    shapes = {
+        "hann": Hann(),
+        "halfcos": Interp(spline.t, spline.c, spline.k),
+    }
 
     measure = Absolute().with_children(
-        *(Play(c[f"m{i}"], s["hann"], 0.1, 30e-9, plateau=1e-6, frequency=20e6 * i) for i in range(nm))
+        *(Play(f"m{i}", "hann", 0.1, 30e-9, plateau=1e-6, frequency=20e6 * i) for i in range(nm))
     )
-    c_group = Stack().with_children(*(Play(c[f"u{i}"], s["halfcos"], 0.01 * (i + 1), 50e-9) for i in range(nu)))
+    c_group = Stack().with_children(*(Play(f"u{i}", "halfcos", 0.01 * (i + 1), 50e-9) for i in range(nu)))
     x_group = Stack().with_children(
-        *(Play(c[f"xy{i}"], s["hann"], 0.01 * (i + 1), 50e-9, drag_coef=5e-10) for i in range(nxy))
+        *(Play(f"xy{i}", "hann", 0.01 * (i + 1), 50e-9, drag_coef=5e-10) for i in range(nxy))
     )
 
     schedule = Stack(duration=50e-6).with_children(
         *(
             Stack().with_children(
                 x_group,
                 Barrier(duration=15e-9),
@@ -46,18 +44,19 @@
             )
             for _ in range(n)
         ),
         measure,
         Barrier(duration=15e-9),
     )
 
-    crosstalk = np.eye(len(channels), dtype=np.float64)
-    crosstalk[c["u0"] : c["u0"] + nu, c["u0"] : c["u0"] + nu] += 0.1
+    ct_matrix = np.eye(nu, dtype=np.float64)
+    ct_matrix += 0.1
+    ct_names = [f"u{i}" for i in range(nu)]
 
-    _ = generate_waveforms(channels, shapes, schedule, crosstalk=crosstalk)
+    _ = generate_waveforms(channels, shapes, schedule, crosstalk=(ct_matrix, ct_names))
 
     t1 = time.perf_counter()
     print(f"Time: {t1-t0:.3f}s")
 
 
 def main():
     for i in cycle(range(349, 350)):
```

### Comparing `bosing-2.0.0b5/ruff_defaults.toml` & `bosing-2.0.0b6/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b5/src/executor.rs` & `bosing-2.0.0b6/src/executor.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,53 @@
+use hashbrown::HashMap;
+
 use crate::{
     pulse::{Envelope, PulseList, PulseListBuilder},
     quant::{Frequency, Time},
     schedule::{self, ArrangedElement, ElementVariant},
     shape::Shape,
 };
 
 #[derive(Debug, Clone)]
 pub struct Executor {
-    channels: Vec<Channel>,
-    shapes: Vec<Shape>,
+    channels: HashMap<String, Channel>,
+    shapes: HashMap<String, Shape>,
     amp_tolerance: f64,
     time_tolerance: f64,
 }
 
 impl Executor {
     pub fn new(amp_tolerance: f64, time_tolerance: f64) -> Self {
         Self {
-            channels: vec![],
-            shapes: vec![],
+            channels: HashMap::new(),
+            shapes: HashMap::new(),
             amp_tolerance,
             time_tolerance,
         }
     }
 
-    pub fn add_channel(&mut self, base_freq: f64) {
-        self.channels.push(Channel::new(
-            base_freq,
-            self.amp_tolerance,
-            self.time_tolerance,
-        ));
+    pub fn add_channel(&mut self, name: String, base_freq: f64) {
+        self.channels.insert(
+            name,
+            Channel::new(base_freq, self.amp_tolerance, self.time_tolerance),
+        );
     }
 
-    pub fn add_shape(&mut self, shape: Shape) {
-        self.shapes.push(shape);
+    pub fn add_shape(&mut self, name: String, shape: Shape) {
+        self.shapes.insert(name, shape);
     }
 
     pub fn execute(&mut self, element: &ArrangedElement) {
         self.execute_dispatch(element, 0.0);
     }
 
-    pub fn into_result(self) -> Vec<PulseList> {
+    pub fn into_result(self) -> HashMap<String, PulseList> {
         self.channels
             .into_iter()
-            .map(|c| c.pulses.build())
+            .map(|(n, b)| (n, b.pulses.build()))
             .collect()
     }
 
     fn execute_dispatch(&mut self, element: &ArrangedElement, time: f64) {
         if element.element().common().phantom() {
             return;
         }
@@ -82,55 +83,51 @@
         let amplitude = element.amplitude();
         let drag_coef = element.drag_coef();
         let freq = element.frequency();
         let phase = element.phase();
         let time = Time::new(time).unwrap();
         let width = Time::new(width).unwrap();
         let plateau = Time::new(plateau).unwrap();
-        let channel = &mut self.channels[element.channel_id()];
+        let channel = self.channels.get_mut(element.channel_id()).unwrap();
         channel.add_pulse(
             shape, time, width, plateau, amplitude, drag_coef, freq, phase,
         );
     }
 
     fn execute_shift_phase(&mut self, element: &schedule::ShiftPhase) {
         let delta_phase = element.phase();
-        let channel = &mut self.channels[element.channel_id()];
+        let channel = self.channels.get_mut(element.channel_id()).unwrap();
         channel.shift_phase(delta_phase);
     }
 
     fn execute_set_phase(&mut self, element: &schedule::SetPhase, time: f64) {
         let phase = element.phase();
-        let channel = &mut self.channels[element.channel_id()];
+        let channel = self.channels.get_mut(element.channel_id()).unwrap();
         channel.set_phase(phase, time);
     }
 
     fn execute_shift_freq(&mut self, element: &schedule::ShiftFreq, time: f64) {
         let delta_freq = element.frequency();
-        let channel = &mut self.channels[element.channel_id()];
+        let channel = self.channels.get_mut(element.channel_id()).unwrap();
         channel.shift_freq(delta_freq, time);
     }
 
     fn execute_set_freq(&mut self, element: &schedule::SetFreq, time: f64) {
         let freq = element.frequency();
-        let channel = &mut self.channels[element.channel_id()];
+        let channel = self.channels.get_mut(element.channel_id()).unwrap();
         channel.set_freq(freq, time);
     }
 
     fn execute_swap_phase(&mut self, element: &schedule::SwapPhase, time: f64) {
         let ch1 = element.channel_id1();
         let ch2 = element.channel_id2();
-        // Workaround for unstable get_many_mut
         if ch1 == ch2 {
             return;
         }
-        let (ch1, ch2) = if ch1 < ch2 { (ch1, ch2) } else { (ch2, ch1) };
-        let (a, b) = self.channels.split_at_mut(ch2);
-        let channel = &mut a[ch1];
-        let other = &mut b[0];
+        let [channel, other] = self.channels.get_many_mut([ch1, ch2]).unwrap();
         channel.swap_phase(other, time);
     }
 
     fn execute_repeat(
         &mut self,
         element: &schedule::Repeat,
         child: &ArrangedElement,
```

### Comparing `bosing-2.0.0b5/src/lib.rs` & `bosing-2.0.0b6/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 //! Although Element struct may contains [`Py<Element>`] as children, it is not
 //! possible to create cyclic references because we don't allow mutate the
 //! children after creation.
 
+use hashbrown::HashMap;
 use mimalloc::MiMalloc;
 use numpy::prelude::*;
 use numpy::{AllowTypeChange, Complex64, PyArray1, PyArrayLike2};
 use pyo3::exceptions::{PyRuntimeError, PyTypeError, PyValueError};
 use pyo3::prelude::*;
-use std::{collections::HashMap, sync::Arc};
+use std::sync::Arc;
 
 use crate::executor::Executor;
 use crate::pulse::Sampler;
 use crate::quant::{Frequency, Time};
 use schedule::ElementCommonBuilder;
 
 mod executor;
@@ -26,45 +27,35 @@
 /// Channel configuration.
 ///
 /// `align_level` is the time axis alignment granularity. With sampling interval
 /// :math:`\Delta t` and `align_level` :math:`n`, start of pulse is aligned to
 /// the nearest multiple of :math:`2^n \Delta t`.
 ///
 /// Args:
-///     name (str): Name of the channel.
 ///     base_freq (float): Base frequency of the channel.
 ///     sample_rate (float): Sample rate of the channel.
 ///     length (int): Length of the waveform.
 ///     delay (float): Delay of the channel. Defaults to 0.0.
 ///     align_level (int): Time axis alignment granularity. Defaults to -10.
 #[pyclass(get_all, frozen)]
 #[derive(Debug, Clone)]
 struct Channel {
-    name: String,
     base_freq: f64,
     sample_rate: f64,
     length: usize,
     delay: f64,
     align_level: i32,
 }
 
 #[pymethods]
 impl Channel {
     #[new]
-    #[pyo3(signature = (name, base_freq, sample_rate, length, *, delay=0.0, align_level=-10))]
-    fn new(
-        name: String,
-        base_freq: f64,
-        sample_rate: f64,
-        length: usize,
-        delay: f64,
-        align_level: i32,
-    ) -> Self {
+    #[pyo3(signature = (base_freq, sample_rate, length, *, delay=0.0, align_level=-10))]
+    fn new(base_freq: f64, sample_rate: f64, length: usize, delay: f64, align_level: i32) -> Self {
         Channel {
-            name,
             base_freq,
             sample_rate,
             length,
             delay,
             align_level,
         }
     }
@@ -401,16 +392,16 @@
 ///
 /// .. caution::
 ///
 ///     The unit of phase is number of cycles, not radians. For example, a phase
 ///     of :math:`0.5` means a phase shift of :math:`\pi` radians.
 ///
 /// Args:
-///     channel_id (int): Target channel ID.
-///     shape_id (int | None): Shape ID of the pulse. If ``None``, the pulse is
+///     channel_id (str): Target channel ID.
+///     shape_id (str | None): Shape ID of the pulse. If ``None``, the pulse is
 ///         a rectangular pulse.
 ///     amplitude (float): Amplitude of the pulse.
 ///     width (float): Width of the pulse.
 ///     plateau (float): Plateau length of the pulse. Defaults to 0.
 ///     drag_coef (float): Drag coefficient of the pulse. If the pulse is a
 ///         rectangular pulse, the drag coefficient is ignored. Defaults to 0.
 ///     frequency (float): Additional frequency of the pulse on top of channel
@@ -442,16 +433,16 @@
         phantom=false,
         duration=None,
         max_duration=f64::INFINITY,
         min_duration=0.0,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
-        channel_id: usize,
-        shape_id: Option<usize>,
+        channel_id: String,
+        shape_id: Option<String>,
         amplitude: f64,
         width: f64,
         plateau: f64,
         drag_coef: f64,
         frequency: f64,
         phase: f64,
         flexible: bool,
@@ -488,39 +479,39 @@
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     #[getter]
-    fn channel_id(slf: &Bound<'_, Self>) -> PyResult<usize> {
+    fn channel_id(slf: &Bound<'_, Self>) -> PyResult<String> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_play()
             .ok_or(PyValueError::new_err(
                 "Failed to get the play variant from the element.",
             ))?
             .channel_id();
-        Ok(ret)
+        Ok(ret.to_string())
     }
 
     #[getter]
-    fn shape_id(slf: &Bound<'_, Self>) -> PyResult<Option<usize>> {
+    fn shape_id(slf: &Bound<'_, Self>) -> PyResult<Option<String>> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_play()
             .ok_or(PyValueError::new_err(
                 "Failed to get the play variant from the element.",
             ))?
             .shape_id();
-        Ok(ret)
+        Ok(ret.map(|x| x.to_string()))
     }
 
     #[getter]
     fn amplitude(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
@@ -625,15 +616,15 @@
 ///
 /// .. caution::
 ///
 ///     The unit of phase is number of cycles, not radians. For example, a phase
 ///     of :math:`0.5` means a phase shift of :math:`\pi` radians.
 ///
 /// Args:
-///     channel_id (int): Target channel ID.
+///     channel_id (str): Target channel ID.
 ///     phase (float): Phase shift in **cycles**.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct ShiftPhase;
 
 #[pymethods]
 impl ShiftPhase {
@@ -647,15 +638,15 @@
         phantom=false,
         duration=None,
         max_duration=f64::INFINITY,
         min_duration=0.0,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
-        channel_id: usize,
+        channel_id: String,
         phase: f64,
         margin: Option<&Bound<'_, PyAny>>,
         alignment: Option<&Bound<'_, PyAny>>,
         phantom: bool,
         duration: Option<f64>,
         max_duration: f64,
         min_duration: f64,
@@ -673,25 +664,25 @@
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     #[getter]
-    fn channel_id(slf: &Bound<'_, Self>) -> PyResult<usize> {
+    fn channel_id(slf: &Bound<'_, Self>) -> PyResult<String> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_shift_phase()
             .ok_or(PyValueError::new_err(
                 "Failed to get the shift_phase variant from the element.",
             ))?
             .channel_id();
-        Ok(ret)
+        Ok(ret.to_string())
     }
 
     #[getter]
     fn phase(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
@@ -720,15 +711,15 @@
 ///
 /// .. caution::
 ///
 ///     The unit of phase is number of cycles, not radians. For example, a phase
 ///     of :math:`0.5` means a phase shift of :math:`\pi` radians.
 ///
 /// Args:
-///     channel_id (int): Target channel ID.
+///     channel_id (str): Target channel ID.
 ///     phase (float): Target phase value in **cycles**.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct SetPhase;
 
 #[pymethods]
 impl SetPhase {
@@ -742,15 +733,15 @@
         phantom=false,
         duration=None,
         max_duration=f64::INFINITY,
         min_duration=0.0,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
-        channel_id: usize,
+        channel_id: String,
         phase: f64,
         margin: Option<&Bound<'_, PyAny>>,
         alignment: Option<&Bound<'_, PyAny>>,
         phantom: bool,
         duration: Option<f64>,
         max_duration: f64,
         min_duration: f64,
@@ -768,25 +759,25 @@
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     #[getter]
-    fn channel_id(slf: &Bound<'_, Self>) -> PyResult<usize> {
+    fn channel_id(slf: &Bound<'_, Self>) -> PyResult<String> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_set_phase()
             .ok_or(PyValueError::new_err(
                 "Failed to get the set_phase variant from the element.",
             ))?
             .channel_id();
-        Ok(ret)
+        Ok(ret.to_string())
     }
 
     #[getter]
     fn phase(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
@@ -803,15 +794,15 @@
 /// A frequency shift element.
 ///
 /// Frequency shift will be added to the channel frequency shift :math:`\Delta
 /// f` and the channel phase offset :math:`\phi_c` will be adjusted such that
 /// the phase is continuous at the scheduled time point.
 ///
 /// Args:
-///     channel_id (int): Target channel ID.
+///     channel_id (str): Target channel ID.
 ///     frequency (float): Delta frequency.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct ShiftFreq;
 
 #[pymethods]
 impl ShiftFreq {
@@ -825,15 +816,15 @@
         phantom=false,
         duration=None,
         max_duration=f64::INFINITY,
         min_duration=0.0,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
-        channel_id: usize,
+        channel_id: String,
         frequency: f64,
         margin: Option<&Bound<'_, PyAny>>,
         alignment: Option<&Bound<'_, PyAny>>,
         phantom: bool,
         duration: Option<f64>,
         max_duration: f64,
         min_duration: f64,
@@ -851,25 +842,25 @@
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     #[getter]
-    fn channel_id(slf: &Bound<'_, Self>) -> PyResult<usize> {
+    fn channel_id(slf: &Bound<'_, Self>) -> PyResult<String> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_shift_freq()
             .ok_or(PyValueError::new_err(
                 "Failed to get the shift_freq variant from the element.",
             ))?
             .channel_id();
-        Ok(ret)
+        Ok(ret.to_string())
     }
 
     #[getter]
     fn frequency(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
@@ -887,15 +878,15 @@
 ///
 /// The channel frequency shift :math:`\Delta f` will be set to the provided
 /// `frequency` parameter and the channel phase offset :math:`\phi_c` will be
 /// adjusted such that the phase is continuous at the scheduled time point.
 /// The channel base frequency :math:`f_0` will not be changed.
 ///
 /// Args:
-///     channel_id (int): Target channel ID.
+///     channel_id (str): Target channel ID.
 ///     frequency (float): Target frequency.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct SetFreq;
 
 #[pymethods]
 impl SetFreq {
@@ -909,15 +900,15 @@
         phantom=false,
         duration=None,
         max_duration=f64::INFINITY,
         min_duration=0.0,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
-        channel_id: usize,
+        channel_id: String,
         frequency: f64,
         margin: Option<&Bound<'_, PyAny>>,
         alignment: Option<&Bound<'_, PyAny>>,
         phantom: bool,
         duration: Option<f64>,
         max_duration: f64,
         min_duration: f64,
@@ -935,25 +926,25 @@
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     #[getter]
-    fn channel_id(slf: &Bound<'_, Self>) -> PyResult<usize> {
+    fn channel_id(slf: &Bound<'_, Self>) -> PyResult<String> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_set_freq()
             .ok_or(PyValueError::new_err(
                 "Failed to get the set_freq variant from the element.",
             ))?
             .channel_id();
-        Ok(ret)
+        Ok(ret.to_string())
     }
 
     #[getter]
     fn frequency(slf: &Bound<'_, Self>) -> PyResult<f64> {
         let ret = slf
             .downcast::<Element>()?
             .get()
@@ -973,16 +964,16 @@
 /// base frequency :math:`f_0` and the channel frequency shift :math:`\Delta f`
 /// will be considered. At the scheduled time point, the phase to be swapped
 /// is calculated as
 ///
 /// .. math:: \phi(t) = (f_0 + \Delta f) t + \phi_c
 ///
 /// Args:
-///     channel_id1 (int): Target channel ID 1.
-///     channel_id2 (int): Target channel ID 2.
+///     channel_id1 (str): Target channel ID 1.
+///     channel_id2 (str): Target channel ID 2.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct SwapPhase;
 
 #[pymethods]
 impl SwapPhase {
     #[new]
@@ -995,16 +986,16 @@
         phantom=false,
         duration=None,
         max_duration=f64::INFINITY,
         min_duration=0.0,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
-        channel_id1: usize,
-        channel_id2: usize,
+        channel_id1: String,
+        channel_id2: String,
         margin: Option<&Bound<'_, PyAny>>,
         alignment: Option<&Bound<'_, PyAny>>,
         phantom: bool,
         duration: Option<f64>,
         max_duration: f64,
         min_duration: f64,
     ) -> PyResult<(Self, Element)> {
@@ -1020,53 +1011,53 @@
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     #[getter]
-    fn channel_id1(slf: &Bound<'_, Self>) -> PyResult<usize> {
+    fn channel_id1(slf: &Bound<'_, Self>) -> PyResult<String> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_swap_phase()
             .ok_or(PyValueError::new_err(
                 "Failed to get the swap_phase variant from the element.",
             ))?
             .channel_id1();
-        Ok(ret)
+        Ok(ret.to_string())
     }
 
     #[getter]
-    fn channel_id2(slf: &Bound<'_, Self>) -> PyResult<usize> {
+    fn channel_id2(slf: &Bound<'_, Self>) -> PyResult<String> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_swap_phase()
             .ok_or(PyValueError::new_err(
                 "Failed to get the swap_phase variant from the element.",
             ))?
             .channel_id2();
-        Ok(ret)
+        Ok(ret.to_string())
     }
 }
 
 /// A barrier element.
 ///
 /// A barrier element is a no-op element. Useful for aligning elements on
 /// different channels and adding space between elements in a :class:`Stack`
 /// layout.
 ///
 /// If no channel IDs are provided, the layout system will arrange the barrier
 /// element as if it occupies all channels in its parent.
 ///
 /// Args:
-///     *channel_ids (int): Channel IDs. Defaults to empty.
+///     *channel_ids (str): Channel IDs. Defaults to empty.
 #[pyclass(extends=Element, frozen)]
 #[derive(Debug, Clone)]
 struct Barrier;
 
 #[pymethods]
 impl Barrier {
     #[new]
@@ -1076,15 +1067,15 @@
         alignment=None,
         phantom=false,
         duration=None,
         max_duration=f64::INFINITY,
         min_duration=0.0,
     ))]
     fn new(
-        channel_ids: Vec<usize>,
+        channel_ids: Vec<String>,
         margin: Option<&Bound<'_, PyAny>>,
         alignment: Option<&Bound<'_, PyAny>>,
         phantom: bool,
         duration: Option<f64>,
         max_duration: f64,
         min_duration: f64,
     ) -> PyResult<(Self, Element)> {
@@ -1100,15 +1091,15 @@
                 max_duration,
                 min_duration,
             )?,
         ))
     }
 
     #[getter]
-    fn channel_ids(slf: &Bound<'_, Self>) -> PyResult<Vec<usize>> {
+    fn channel_ids(slf: &Bound<'_, Self>) -> PyResult<Vec<String>> {
         let ret = slf
             .downcast::<Element>()?
             .get()
             .0
             .try_get_barrier()
             .ok_or(PyValueError::new_err(
                 "Failed to get the barrier variant from the element.",
@@ -1945,41 +1936,40 @@
         Ok(ret)
     }
 }
 
 /// Generate waveforms from a schedule.
 ///
 /// Args:
-///     channels (Iterable[Channel]): Information of the channels.
-///     shapes (Iterable[Shape]): Shapes used in the schedule.
+///     channels (Mapping[str, Channel]): Information of the channels.
+///     shapes (Mapping[str, Shape]): Shapes used in the schedule.
 ///     schedule (Element): Root element of the schedule.
 ///     time_tolerance (float): Tolerance for time comparison. Default is 1e-12.
 ///     amp_tolerance (float): Tolerance for amplitude comparison. Default is
 ///         0.1 / 2^16.
-///     phase_tolerance (float): Tolerance for phase comparison. Default is
-///         1e-4.
 ///     allow_oversize (bool): Allow oversize elements. Default is ``False``.
-///     crosstalk (array_like | None): Crosstalk matrix. Default is ``None``.
+///     crosstalk (tuple[array_like, Sequence[str]] | None): Crosstalk matrix
+///         with corresponding channel ids. Default is ``None``.
 /// Returns:
 ///     Dict[str, numpy.ndarray]: Waveforms of the channels. The key is the
 ///         channel name and the value is the waveform.
 /// Raises:
 ///     ValueError: If some input is invalid.
 ///     TypeError: If some input has an invalid type.
 ///     RuntimeError: If waveform generation fails.
 /// Example:
 ///     .. code-block:: python
 ///
 ///         from bosing import Barrier, Channel, Hann, Play, Stack, generate_waveforms
-///         channels = [Channel("xy", 30e6, 2e9, 1000)]
-///         shapes = [Hann()]
+///         channels = {"xy": Channel(30e6, 2e9, 1000)}
+///         shapes = {"hann": Hann()}
 ///         schedule = Stack(duration=500e-9).with_children(
 ///             Play(
-///                 channel_id=0,
-///                 shape_id=0,
+///                 channel_id="xy",
+///                 shape_id="hann",
 ///                 amplitude=0.3,
 ///                 width=100e-9,
 ///                 plateau=200e-9,
 ///             ),
 ///             Barrier(duration=10e-9),
 ///         )
 ///         result = generate_waveforms(channels, shapes, schedule)
@@ -1987,82 +1977,79 @@
 #[pyo3(signature = (
     channels,
     shapes,
     schedule,
     *,
     time_tolerance=1e-12,
     amp_tolerance=0.1 / 2f64.powi(16),
-    phase_tolerance=1e-4,
     allow_oversize=false,
     crosstalk=None,
 ))]
 #[allow(clippy::too_many_arguments)]
 fn generate_waveforms(
     py: Python<'_>,
-    channels: Vec<Channel>,
-    shapes: Vec<Py<Shape>>,
+    channels: HashMap<String, Channel>,
+    shapes: HashMap<String, Py<Shape>>,
     schedule: &Bound<'_, Element>,
     time_tolerance: f64,
     amp_tolerance: f64,
-    phase_tolerance: f64,
     allow_oversize: bool,
-    crosstalk: Option<PyArrayLike2<'_, f64, AllowTypeChange>>,
+    crosstalk: Option<(PyArrayLike2<'_, f64, AllowTypeChange>, Vec<String>)>,
 ) -> PyResult<HashMap<String, Py<PyArray1<Complex64>>>> {
-    // TODO: use the tolerances
-    let _ = phase_tolerance;
-    if let Some(crosstalk) = &crosstalk {
+    if let Some((crosstalk, names)) = &crosstalk {
         if crosstalk.ndim() != 2 {
             return Err(PyValueError::new_err("Crosstalk must be a 2D array."));
         }
         if crosstalk.shape()[0] != crosstalk.shape()[1] {
             return Err(PyValueError::new_err("Crosstalk must be a square matrix."));
         }
-        if crosstalk.shape()[0] != channels.len() {
+        if crosstalk.shape()[0] != names.len() {
             return Err(PyValueError::new_err(
-                "The size of the crosstalk matrix must be the same as the number of channels.",
+                "The size of the crosstalk matrix must be the same as the number of names.",
             ));
         }
     }
 
     let root = schedule.downcast::<Element>()?.get().0.clone();
     let measured = schedule::measure(root, f64::INFINITY);
     let arrange_options = schedule::ScheduleOptions {
         time_tolerance,
         allow_oversize,
     };
     let arranged = schedule::arrange(&measured, 0.0, measured.duration(), &arrange_options)
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
     let mut executor = Executor::new(amp_tolerance, time_tolerance);
-    for c in channels.iter() {
-        executor.add_channel(c.base_freq);
+    for (n, c) in &channels {
+        executor.add_channel(n.clone(), c.base_freq);
     }
-    for s in shapes.iter() {
+    for (n, s) in &shapes {
         let s = s.bind(py);
-        executor.add_shape(Shape::get_rust_shape(s)?);
+        executor.add_shape(n.clone(), Shape::get_rust_shape(s)?);
     }
     executor.execute(&arranged);
     let results = executor.into_result();
     let mut sampler = Sampler::new();
-    for (c, pl) in channels.iter().zip(results) {
+    for (n, pl) in results {
+        let c = &channels[&n];
         sampler.add_channel(
+            n,
             pl,
             c.length,
             Frequency::new(c.sample_rate).unwrap(),
             Time::new(c.delay).unwrap(),
             c.align_level,
         );
     }
-    if let Some(crosstalk) = &crosstalk {
-        sampler.set_crosstalk(crosstalk.as_array());
+    if let Some((crosstalk, names)) = &crosstalk {
+        sampler.set_crosstalk(crosstalk.as_array(), names.clone());
     }
     let waveforms = sampler.sample(time_tolerance);
-    let dict = channels
+    let dict = waveforms
         .into_iter()
-        .zip(waveforms)
-        .map(|(c, w)| (c.name, PyArray1::from_vec_bound(py, w).unbind()))
+        .map(|(n, w)| (n, PyArray1::from_vec_bound(py, w).unbind()))
         .collect();
     Ok(dict)
 }
 
 /// Generates microwave pulses for superconducting quantum computing
 /// experiments.
 ///
```

### Comparing `bosing-2.0.0b5/src/pulse.rs` & `bosing-2.0.0b6/src/pulse.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 use std::{
-    collections::HashMap,
     f64::consts::TAU,
     ops::{Add, Mul},
     sync::Arc,
 };
 
 use cached::proc_macro::cached;
 use float_cmp::approx_eq;
+use hashbrown::HashMap;
 use itertools::{izip, Itertools};
-use ndarray::ArrayView2;
+use ndarray::{ArrayView2, Axis};
 use numpy::Complex64;
+use rayon::prelude::*;
 
 use crate::{
     quant::{AlignedIndex, Frequency, Time},
     shape::Shape,
 };
 
 /// A pulse envelope
@@ -82,78 +83,105 @@
 }
 
 #[derive(Debug, Clone)]
 pub struct PulseList {
     items: HashMap<ListBin, Vec<(Time, PulseAmplitude)>>,
 }
 
+#[derive(Debug, Clone)]
+pub struct Crosstalk<'a> {
+    matrix: ArrayView2<'a, f64>,
+    names: Vec<String>,
+}
+
+impl<'a> Crosstalk<'a> {
+    pub fn new(matrix: ArrayView2<'a, f64>, names: Vec<String>) -> Self {
+        Self { matrix, names }
+    }
+}
+
 #[derive(Debug, Clone, Default)]
 pub struct Sampler<'a> {
-    channels: Vec<Channel>,
-    crosstalk: Option<ArrayView2<'a, f64>>,
+    channels: HashMap<String, Channel>,
+    crosstalk: Option<Crosstalk<'a>>,
 }
 
 impl<'a> Sampler<'a> {
     pub fn new() -> Self {
         Self::default()
     }
 
     pub fn add_channel(
         &mut self,
+        name: String,
         pulses: PulseList,
         length: usize,
         sample_rate: Frequency,
         delay: Time,
         align_level: i32,
     ) {
-        self.channels.push(Channel {
-            pulses,
-            length,
-            sample_rate,
-            align_level,
-            delay,
-        });
+        self.channels.insert(
+            name,
+            Channel {
+                pulses,
+                length,
+                sample_rate,
+                align_level,
+                delay,
+            },
+        );
     }
 
-    pub fn set_crosstalk(&mut self, crosstalk: ArrayView2<'a, f64>) {
-        self.crosstalk = Some(crosstalk);
+    pub fn set_crosstalk(&mut self, crosstalk: ArrayView2<'a, f64>, names: Vec<String>) {
+        self.crosstalk = Some(Crosstalk::new(crosstalk, names));
     }
 
-    pub fn sample(&self, time_tolerance: f64) -> Vec<Vec<Complex64>> {
-        if let Some(crosstalk) = self.crosstalk {
+    pub fn sample(&self, time_tolerance: f64) -> HashMap<String, Vec<Complex64>> {
+        if let Some(crosstalk) = &self.crosstalk {
             crosstalk
-                .columns()
-                .into_iter()
-                .zip(&self.channels)
-                .map(|(column, output)| {
-                    let lists = column
-                        .iter()
-                        .copied()
-                        .zip(&self.channels)
-                        .map(|(multiplier, input)| (multiplier, &input.pulses));
-                    merge_and_sample(
-                        lists,
-                        output.length,
-                        output.sample_rate,
-                        output.delay,
-                        output.align_level,
-                        time_tolerance,
+                .matrix
+                .axis_iter(Axis(0))
+                .into_par_iter()
+                .zip(&crosstalk.names)
+                .map(|(row, out_name)| {
+                    let out_channel = &self.channels[out_name];
+                    let lists =
+                        row.iter()
+                            .copied()
+                            .zip(&crosstalk.names)
+                            .map(|(multiplier, in_name)| {
+                                let in_channel = &self.channels[in_name];
+                                (multiplier, &in_channel.pulses)
+                            });
+                    (
+                        out_name.clone(),
+                        merge_and_sample(
+                            lists,
+                            out_channel.length,
+                            out_channel.sample_rate,
+                            out_channel.delay,
+                            out_channel.align_level,
+                            time_tolerance,
+                        ),
                     )
                 })
                 .collect()
         } else {
             self.channels
-                .iter()
-                .map(|c| {
+                .par_iter()
+                .map(|(n, c)| {
                     let list = c
                         .pulses
                         .items
                         .iter()
                         .map(|(bin, items)| (bin.clone(), items.iter().copied()));
-                    sample_pulse_list(list, c.length, c.sample_rate, c.delay, c.align_level)
+                    (
+                        n.clone(),
+                        sample_pulse_list(list, c.length, c.sample_rate, c.delay, c.align_level),
+                    )
                 })
                 .collect()
         }
     }
 }
 
 #[derive(Debug, Clone)]
```

### Comparing `bosing-2.0.0b5/src/quant.rs` & `bosing-2.0.0b6/src/quant.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b5/src/schedule/absolute.rs` & `bosing-2.0.0b6/src/schedule/absolute.rs`

 * *Files 2% similar despite different names*

```diff
@@ -25,30 +25,30 @@
         Ok(self)
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct Absolute {
     children: Vec<AbsoluteEntry>,
-    channel_ids: Vec<usize>,
+    channel_ids: Vec<String>,
 }
 
 impl Absolute {
     pub fn new() -> Self {
         Self {
             children: vec![],
             channel_ids: vec![],
         }
     }
 
     pub fn with_children(mut self, children: Vec<AbsoluteEntry>) -> Self {
         let channel_ids = children
             .iter()
             .flat_map(|e| e.element.variant.channels())
-            .copied()
+            .cloned()
             .unique()
             .collect();
         self.children = children;
         self.channel_ids = channel_ids;
         self
     }
 }
@@ -79,11 +79,11 @@
             .collect::<Result<_>>()?;
         Ok(ArrangeResult(
             context.final_duration,
             ArrangeResultVariant::Multiple(arranged_children),
         ))
     }
 
-    fn channels(&self) -> &[usize] {
+    fn channels(&self) -> &[String] {
         &self.channel_ids
     }
 }
```

### Comparing `bosing-2.0.0b5/src/schedule/grid.rs` & `bosing-2.0.0b6/src/schedule/grid.rs`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct Grid {
     children: Vec<GridEntry>,
     columns: Vec<GridLength>,
-    channel_ids: Vec<usize>,
+    channel_ids: Vec<String>,
 }
 
 impl Grid {
     pub fn new() -> Self {
         Self {
             children: vec![],
             columns: vec![GridLength::star(1.0).unwrap()],
@@ -60,15 +60,15 @@
         self
     }
 
     pub fn with_children(mut self, children: Vec<GridEntry>) -> Self {
         let channel_ids = children
             .iter()
             .flat_map(|e| e.element.variant.channels())
-            .copied()
+            .cloned()
             .unique()
             .collect();
         self.children = children;
         self.channel_ids = channel_ids;
         self
     }
 
@@ -194,15 +194,15 @@
             .collect::<Result<_>>()?;
         Ok(ArrangeResult(
             context.final_duration,
             ArrangeResultVariant::Multiple(arranged_children),
         ))
     }
 
-    fn channels(&self) -> &[usize] {
+    fn channels(&self) -> &[String] {
         &self.channel_ids
     }
 }
 
 fn expand_col_by_ratio(
     col_sizes: &mut [f64],
     start: usize,
```

### Comparing `bosing-2.0.0b5/src/schedule/play.rs` & `bosing-2.0.0b6/src/schedule/play.rs`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 use super::{
     ArrangeContext, ArrangeResult, ArrangeResultVariant, MeasureContext, MeasureResult,
     MeasureResultVariant, Schedule,
 };
 
 #[derive(Debug, Clone)]
 pub struct Play {
-    channel_id: [usize; 1],
-    shape_id: Option<usize>,
+    channel_id: [String; 1],
+    shape_id: Option<String>,
     amplitude: f64,
     width: f64,
     plateau: f64,
     drag_coef: f64,
     frequency: f64,
     phase: f64,
     flexible: bool,
 }
 
 impl Play {
     pub fn new(
-        channel_id: usize,
-        shape_id: Option<usize>,
+        channel_id: String,
+        shape_id: Option<String>,
         amplitude: f64,
         width: f64,
     ) -> Result<Self> {
         if !amplitude.is_finite() {
             bail!("Invalid amplitude {}", amplitude);
         }
         if !width.is_finite() || width < 0.0 {
@@ -77,20 +77,20 @@
     }
 
     pub fn with_flexible(mut self, flexible: bool) -> Self {
         self.flexible = flexible;
         self
     }
 
-    pub fn channel_id(&self) -> usize {
-        self.channel_id[0]
+    pub fn channel_id(&self) -> &str {
+        &self.channel_id[0]
     }
 
-    pub fn shape_id(&self) -> Option<usize> {
-        self.shape_id
+    pub fn shape_id(&self) -> Option<&str> {
+        self.shape_id.as_deref()
     }
 
     pub fn amplitude(&self) -> f64 {
         self.amplitude
     }
 
     pub fn width(&self) -> f64 {
@@ -133,11 +133,11 @@
             context.final_duration
         } else {
             self.width + self.plateau
         };
         Ok(ArrangeResult(arranged, ArrangeResultVariant::Simple))
     }
 
-    fn channels(&self) -> &[usize] {
+    fn channels(&self) -> &[String] {
         &self.channel_id
     }
 }
```

### Comparing `bosing-2.0.0b5/src/schedule/repeat.rs` & `bosing-2.0.0b6/src/schedule/repeat.rs`

 * *Files 5% similar despite different names*

```diff
@@ -67,11 +67,11 @@
         let arranged = arranged_child.inner_duration * n + self.spacing * (n - 1.0);
         Ok(ArrangeResult(
             arranged,
             ArrangeResultVariant::Multiple(vec![arranged_child]),
         ))
     }
 
-    fn channels(&self) -> &[usize] {
+    fn channels(&self) -> &[String] {
         self.child.variant.channels()
     }
 }
```

### Comparing `bosing-2.0.0b5/src/schedule/simple.rs` & `bosing-2.0.0b6/src/schedule/simple.rs`

 * *Files 26% similar despite different names*

```diff
@@ -2,202 +2,202 @@
 
 use super::{
     ArrangeContext, ArrangeResult, ArrangeResultVariant, MeasureContext, MeasureResult,
     MeasureResultVariant, Schedule,
 };
 
 trait SimpleElement {
-    fn channels(&self) -> &[usize];
+    fn channels(&self) -> &[String];
 }
 
 impl<T> Schedule for T
 where
     T: SimpleElement,
 {
     fn measure(&self, _context: &MeasureContext) -> MeasureResult {
         MeasureResult(0.0, MeasureResultVariant::Simple)
     }
 
     fn arrange(&self, _context: &ArrangeContext) -> Result<ArrangeResult> {
         Ok(ArrangeResult(0.0, ArrangeResultVariant::Simple))
     }
 
-    fn channels(&self) -> &[usize] {
+    fn channels(&self) -> &[String] {
         self.channels()
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct ShiftPhase {
-    channel_id: [usize; 1],
+    channel_id: [String; 1],
     phase: f64,
 }
 
 impl ShiftPhase {
-    pub fn new(channel_id: usize, phase: f64) -> Result<Self> {
+    pub fn new(channel_id: String, phase: f64) -> Result<Self> {
         if !phase.is_finite() {
             bail!("Invalid phase {}", phase);
         }
         Ok(Self {
             channel_id: [channel_id],
             phase,
         })
     }
 
-    pub fn channel_id(&self) -> usize {
-        self.channel_id[0]
+    pub fn channel_id(&self) -> &str {
+        &self.channel_id[0]
     }
 
     pub fn phase(&self) -> f64 {
         self.phase
     }
 }
 
 impl SimpleElement for ShiftPhase {
-    fn channels(&self) -> &[usize] {
+    fn channels(&self) -> &[String] {
         &self.channel_id
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct SetPhase {
-    channel_id: [usize; 1],
+    channel_id: [String; 1],
     phase: f64,
 }
 
 impl SetPhase {
-    pub fn new(channel_id: usize, phase: f64) -> Result<Self> {
+    pub fn new(channel_id: String, phase: f64) -> Result<Self> {
         if !phase.is_finite() {
             bail!("Invalid phase {}", phase);
         }
         Ok(Self {
             channel_id: [channel_id],
             phase,
         })
     }
 
-    pub fn channel_id(&self) -> usize {
-        self.channel_id[0]
+    pub fn channel_id(&self) -> &str {
+        &self.channel_id[0]
     }
 
     pub fn phase(&self) -> f64 {
         self.phase
     }
 }
 
 impl SimpleElement for SetPhase {
-    fn channels(&self) -> &[usize] {
+    fn channels(&self) -> &[String] {
         &self.channel_id
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct ShiftFreq {
-    channel_id: [usize; 1],
+    channel_id: [String; 1],
     frequency: f64,
 }
 
 impl ShiftFreq {
-    pub fn new(channel_id: usize, frequency: f64) -> Result<Self> {
+    pub fn new(channel_id: String, frequency: f64) -> Result<Self> {
         if !frequency.is_finite() {
             bail!("Invalid frequency {}", frequency);
         }
         Ok(Self {
             channel_id: [channel_id],
             frequency,
         })
     }
 
-    pub fn channel_id(&self) -> usize {
-        self.channel_id[0]
+    pub fn channel_id(&self) -> &str {
+        &self.channel_id[0]
     }
 
     pub fn frequency(&self) -> f64 {
         self.frequency
     }
 }
 
 impl SimpleElement for ShiftFreq {
-    fn channels(&self) -> &[usize] {
+    fn channels(&self) -> &[String] {
         &self.channel_id
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct SetFreq {
-    channel_id: [usize; 1],
+    channel_id: [String; 1],
     frequency: f64,
 }
 
 impl SetFreq {
-    pub fn new(channel_id: usize, frequency: f64) -> Result<Self> {
+    pub fn new(channel_id: String, frequency: f64) -> Result<Self> {
         if !frequency.is_finite() {
             bail!("Invalid frequency {}", frequency);
         }
         Ok(Self {
             channel_id: [channel_id],
             frequency,
         })
     }
 
-    pub fn channel_id(&self) -> usize {
-        self.channel_id[0]
+    pub fn channel_id(&self) -> &str {
+        &self.channel_id[0]
     }
 
     pub fn frequency(&self) -> f64 {
         self.frequency
     }
 }
 
 impl SimpleElement for SetFreq {
-    fn channels(&self) -> &[usize] {
+    fn channels(&self) -> &[String] {
         &self.channel_id
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct SwapPhase {
-    channel_ids: [usize; 2],
+    channel_ids: [String; 2],
 }
 
 impl SwapPhase {
-    pub fn new(channel_id1: usize, channel_id2: usize) -> Self {
+    pub fn new(channel_id1: String, channel_id2: String) -> Self {
         Self {
             channel_ids: [channel_id1, channel_id2],
         }
     }
 
-    pub fn channel_id1(&self) -> usize {
-        self.channel_ids[0]
+    pub fn channel_id1(&self) -> &str {
+        &self.channel_ids[0]
     }
 
-    pub fn channel_id2(&self) -> usize {
-        self.channel_ids[1]
+    pub fn channel_id2(&self) -> &str {
+        &self.channel_ids[1]
     }
 }
 
 impl SimpleElement for SwapPhase {
-    fn channels(&self) -> &[usize] {
+    fn channels(&self) -> &[String] {
         &self.channel_ids
     }
 }
 
 #[derive(Debug, Clone)]
 pub struct Barrier {
-    channel_ids: Vec<usize>,
+    channel_ids: Vec<String>,
 }
 
 impl Barrier {
-    pub fn new(channel_ids: Vec<usize>) -> Self {
+    pub fn new(channel_ids: Vec<String>) -> Self {
         Self { channel_ids }
     }
 
-    pub fn channel_ids(&self) -> &[usize] {
+    pub fn channel_ids(&self) -> &[String] {
         &self.channel_ids
     }
 }
 
 impl SimpleElement for Barrier {
-    fn channels(&self) -> &[usize] {
+    fn channels(&self) -> &[String] {
         &self.channel_ids
     }
 }
```

### Comparing `bosing-2.0.0b5/src/schedule/stack.rs` & `bosing-2.0.0b6/src/schedule/stack.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 use anyhow::{bail, Result};
+use hashbrown::HashMap;
 use itertools::{Either, Itertools as _};
-use std::collections::HashMap;
 
 use super::{
     arrange, measure, ArrangeContext, ArrangeResult, ArrangeResultVariant, ElementRef,
     MeasureContext, MeasureResult, MeasureResultVariant, MeasuredElement, Schedule,
 };
 use crate::Direction;
 
 #[derive(Debug, Clone)]
 pub struct Stack {
     children: Vec<ElementRef>,
     direction: Direction,
-    channel_ids: Vec<usize>,
+    channel_ids: Vec<String>,
 }
 
 impl Stack {
     pub fn new() -> Self {
         Self {
             children: vec![],
             direction: Direction::Backward,
@@ -29,15 +29,15 @@
         self
     }
 
     pub fn with_children(mut self, children: Vec<ElementRef>) -> Self {
         let channel_ids = children
             .iter()
             .flat_map(|e| e.variant.channels())
-            .copied()
+            .cloned()
             .unique()
             .collect();
         self.children = children;
         self.channel_ids = channel_ids;
         self
     }
 
@@ -47,15 +47,15 @@
 }
 
 impl Schedule for Stack {
     fn measure(&self, context: &MeasureContext) -> MeasureResult {
         let mut used_duration = if self.channel_ids.is_empty() {
             Either::Left(0.0)
         } else {
-            Either::Right(HashMap::<usize, f64>::new())
+            Either::Right(HashMap::<String, f64>::new())
         };
         let mapper = |child: &ElementRef| {
             let child_channels = child.variant.channels();
             let channel_used_duration = get_channel_usage(&used_duration, child_channels);
             let child_available_duration = context.max_duration - channel_used_duration;
             let measured_child = measure(child.clone(), child_available_duration);
             let channel_used_duration = channel_used_duration + measured_child.duration;
@@ -87,15 +87,15 @@
         )
     }
 
     fn arrange(&self, context: &ArrangeContext) -> Result<ArrangeResult> {
         let mut used_duration = if self.channel_ids.is_empty() {
             Either::Left(0.0)
         } else {
-            Either::Right(HashMap::<usize, f64>::new())
+            Either::Right(HashMap::<String, f64>::new())
         };
         let measured_children = match &context.measured_self.data {
             MeasureResultVariant::Multiple(v) => v,
             _ => bail!("Invalid measure data"),
         };
         let mapper = |child: &MeasuredElement| {
             let child_channels = child.element.variant.channels();
@@ -126,35 +126,38 @@
         }
         Ok(ArrangeResult(
             context.final_duration,
             ArrangeResultVariant::Multiple(arranged_children),
         ))
     }
 
-    fn channels(&self) -> &[usize] {
+    fn channels(&self) -> &[String] {
         &self.channel_ids
     }
 }
 
 fn update_channel_usage(
-    used_duration: &mut Either<f64, HashMap<usize, f64>>,
+    used_duration: &mut Either<f64, HashMap<String, f64>>,
     new_duration: f64,
-    channels: &[usize],
+    channels: &[String],
 ) {
     match used_duration {
         Either::Left(v) => *v = new_duration,
         Either::Right(d) => {
-            for &ch in channels {
-                d.insert(ch, new_duration);
+            for ch in channels {
+                d.insert(ch.clone(), new_duration);
             }
         }
     }
 }
 
-fn get_channel_usage(used_duration: &Either<f64, HashMap<usize, f64>>, channels: &[usize]) -> f64 {
+fn get_channel_usage(
+    used_duration: &Either<f64, HashMap<String, f64>>,
+    channels: &[String],
+) -> f64 {
     match used_duration {
         Either::Left(v) => *v,
         Either::Right(d) => (if channels.is_empty() {
             d.values().max_by(|a, b| a.total_cmp(b))
         } else {
             channels
                 .iter()
```

### Comparing `bosing-2.0.0b5/src/schedule.rs` & `bosing-2.0.0b6/src/schedule.rs`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 #[enum_dispatch]
 trait Schedule {
     /// Measure the element and return desired inner size and measured children.
     fn measure(&self, context: &MeasureContext) -> MeasureResult;
     /// Arrange the element and return final inner size and arranged children.
     fn arrange(&self, context: &ArrangeContext) -> Result<ArrangeResult>;
     /// Channels used by this element. Empty means all of parent's channels.
-    fn channels(&self) -> &[usize];
+    fn channels(&self) -> &[String];
 }
 
 fn clamp_duration(duration: f64, min_duration: f64, max_duration: f64) -> f64 {
     duration.min(max_duration).max(min_duration)
 }
 
 pub fn measure(element: ElementRef, available_duration: f64) -> MeasuredElement {
```

### Comparing `bosing-2.0.0b5/src/shape.rs` & `bosing-2.0.0b6/src/shape.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b5/tests/test_basic.py` & `bosing-2.0.0b6/tests/test_basic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import numpy as np
 
 import bosing
 
 
 def test_basic():
-    channels = [bosing.Channel("xy0", 100e6, 2e9, 100000)]
-    shapes = [bosing.Hann()]
-    schedule = bosing.Stack(duration=49.9e-6).with_children(bosing.Play(0, 0, 0.1, 100e-9))
+    channels = {"xy0": bosing.Channel(100e6, 2e9, 100000)}
+    shapes = {"hann": bosing.Hann()}
+    schedule = bosing.Stack(duration=49.9e-6).with_children(bosing.Play("xy0", "hann", 0.1, 100e-9))
     result = bosing.generate_waveforms(channels, shapes, schedule)
     assert "xy0" in result
     w = result["xy0"]
     assert len(w) == 100000
     assert w[0] == 0
     assert w[-1] == 0
     assert np.any(w != 0)
 
 
 def test_mixing():
-    shapes = [bosing.Hann()]
+    shapes = {"hann": bosing.Hann()}
     schedule = bosing.Stack(duration=500e-9).with_children(
         bosing.Play(
-            channel_id=0,
+            channel_id="xy",
+            shape_id="hann",
             amplitude=0.3,
-            shape_id=0,
             width=100e-9,
             plateau=200e-9,
         ),
         bosing.Barrier(duration=10e-9),
     )
     freq = 30e6
 
-    channels = [bosing.Channel("xy", freq, 2e9, 1000)]
+    channels = {"xy": bosing.Channel(freq, 2e9, 1000)}
     result = bosing.generate_waveforms(channels, shapes, schedule)
     w1 = result["xy"]
 
-    channels = [bosing.Channel("xy", 0, 2e9, 1000)]
+    channels = {"xy": bosing.Channel(0, 2e9, 1000)}
     result = bosing.generate_waveforms(channels, shapes, schedule)
     w2 = result["xy"]
     w2 = w2 * np.exp(1j * (2 * np.pi * freq * np.arange(1000) / 2e9))
 
     assert np.allclose(w1, w2)
```

### Comparing `bosing-2.0.0b5/Cargo.lock` & `bosing-2.0.0b6/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -36,28 +36,30 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bosing"
-version = "2.0.0-beta.5"
+version = "2.0.0-beta.6"
 dependencies = [
  "anyhow",
  "bspline",
  "cached",
  "enum_dispatch",
  "float-cmp",
+ "hashbrown",
  "itertools",
  "mimalloc",
  "ndarray",
  "num",
  "numpy",
  "ordered-float",
  "pyo3",
+ "rayon",
 ]
 
 [[package]]
 name = "bspline"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af7483eaaefe53f63b5b140f639c5ed6749f8e545768803dc5b89f43acb8ee84"
@@ -108,14 +110,39 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "crossbeam-deque"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
+dependencies = [
+ "crossbeam-epoch",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-epoch"
+version = "0.9.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
+dependencies = [
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-utils"
+version = "0.8.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+
+[[package]]
 name = "darling"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
 dependencies = [
  "darling_core",
  "darling_macro",
@@ -183,14 +210,15 @@
 name = "hashbrown"
 version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 dependencies = [
  "ahash",
  "allocator-api2",
+ "rayon",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
@@ -286,14 +314,15 @@
 checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
 dependencies = [
  "matrixmultiply",
  "num-complex",
  "num-integer",
  "num-traits",
  "rawpointer",
+ "rayon",
 ]
 
 [[package]]
 name = "num"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
@@ -438,14 +467,15 @@
 [[package]]
 name = "pyo3"
 version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
+ "hashbrown",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
@@ -510,14 +540,34 @@
 [[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
+name = "rayon"
+version = "1.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
+dependencies = [
+ "either",
+ "rayon-core",
+]
+
+[[package]]
+name = "rayon-core"
+version = "1.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
+dependencies = [
+ "crossbeam-deque",
+ "crossbeam-utils",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
```

### Comparing `bosing-2.0.0b5/pyproject.toml` & `bosing-2.0.0b6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b5/PKG-INFO` & `bosing-2.0.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bosing
-Version: 2.0.0b5
+Version: 2.0.0b6
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
```

