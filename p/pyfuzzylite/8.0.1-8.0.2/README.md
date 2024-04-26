# Comparing `tmp/pyfuzzylite-8.0.1.tar.gz` & `tmp/pyfuzzylite-8.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfuzzylite-8.0.1.tar", max compression
+gzip compressed data, was "pyfuzzylite-8.0.2.tar", max compression
```

## Comparing `pyfuzzylite-8.0.1.tar` & `pyfuzzylite-8.0.2.tar`

### file list

```diff
@@ -1,245 +1,245 @@
--rw-r--r--   0        0        0       71 2024-01-11 00:28:25.578881 pyfuzzylite-8.0.1/AUTHOR
--rw-r--r--   0        0        0      807 2024-01-11 00:28:25.578881 pyfuzzylite-8.0.1/CITATION.cff
--rw-r--r--   0        0        0      142 2024-01-11 00:28:25.578881 pyfuzzylite-8.0.1/LICENSE.FuzzyLite.txt
--rw-r--r--   0        0        0    35148 2024-01-11 00:28:25.578881 pyfuzzylite-8.0.1/LICENSE.GPL.txt
--rw-r--r--   0        0        0     7814 2024-01-11 00:28:25.578881 pyfuzzylite-8.0.1/README.md
--rw-r--r--   0        0        0     1082 2024-01-11 00:28:25.618882 pyfuzzylite-8.0.1/fuzzylite/__init__.py
--rw-r--r--   0        0        0    17447 2024-01-11 00:28:25.618882 pyfuzzylite-8.0.1/fuzzylite/activation.py
--rw-r--r--   0        0        0     7896 2024-01-11 00:28:25.618882 pyfuzzylite-8.0.1/fuzzylite/benchmark.py
--rw-r--r--   0        0        0    21720 2024-01-11 00:28:25.618882 pyfuzzylite-8.0.1/fuzzylite/defuzzifier.py
--rw-r--r--   0        0        0    24311 2024-01-11 00:28:25.618882 pyfuzzylite-8.0.1/fuzzylite/engine.py
--rw-r--r--   0        0        0      134 2024-01-11 00:28:25.618882 pyfuzzylite-8.0.1/fuzzylite/examples/__init__.py
--rw-r--r--   0        0        0       84 2024-01-11 00:28:25.618882 pyfuzzylite-8.0.1/fuzzylite/examples/hybrid/__init__.py
--rw-r--r--   0        0        0    36888 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/hybrid/obstacle_avoidance.fld
--rw-r--r--   0        0        0     1073 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/hybrid/obstacle_avoidance.fll
--rw-r--r--   0        0        0     2435 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/hybrid/obstacle_avoidance.py
--rw-r--r--   0        0        0    50840 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/hybrid/tipper.fld
--rw-r--r--   0        0        0     2103 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/hybrid/tipper.fll
--rw-r--r--   0        0        0     4431 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/hybrid/tipper.py
--rw-r--r--   0        0        0      347 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/__init__.py
--rw-r--r--   0        0        0    24605 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/all_terms.fld
--rw-r--r--   0        0        0     2986 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/all_terms.fll
--rw-r--r--   0        0        0     6258 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/all_terms.py
--rw-r--r--   0        0        0    49885 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/laundry.fld
--rw-r--r--   0        0        0     1645 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/laundry.fll
--rw-r--r--   0        0        0     5788 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/laundry.py
--rw-r--r--   0        0        0      142 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/__init__.py
--rw-r--r--   0        0        0    38421 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/mam21.fld
--rw-r--r--   0        0        0     1034 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/mam21.fll
--rw-r--r--   0        0        0     2392 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/mam21.py
--rw-r--r--   0        0        0    51228 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/mam22.fld
--rw-r--r--   0        0        0     1454 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/mam22.fll
--rw-r--r--   0        0        0     3206 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/mam22.py
--rw-r--r--   0        0        0    51731 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/shower.fld
--rw-r--r--   0        0        0     2101 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/shower.fll
--rw-r--r--   0        0        0     4507 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/shower.py
--rw-r--r--   0        0        0    38427 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tank.fld
--rw-r--r--   0        0        0     1211 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tank.fll
--rw-r--r--   0        0        0     2754 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tank.py
--rw-r--r--   0        0        0    38441 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tank2.fld
--rw-r--r--   0        0        0     1194 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tank2.fll
--rw-r--r--   0        0        0     2681 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tank2.py
--rw-r--r--   0        0        0    37749 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tipper.fld
--rw-r--r--   0        0        0      985 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tipper.fll
--rw-r--r--   0        0        0     2338 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tipper.py
--rw-r--r--   0        0        0    25357 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tipper1.fld
--rw-r--r--   0        0        0      766 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tipper1.fll
--rw-r--r--   0        0        0     1863 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tipper1.py
--rw-r--r--   0        0        0    24592 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/obstacle_avoidance.fld
--rw-r--r--   0        0        0      621 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/obstacle_avoidance.fll
--rw-r--r--   0        0        0     1501 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/obstacle_avoidance.py
--rw-r--r--   0        0        0      120 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/octave/__init__.py
--rw-r--r--   0        0        0    39013 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/octave/investment_portfolio.fld
--rw-r--r--   0        0        0     1209 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/octave/investment_portfolio.fll
--rw-r--r--   0        0        0     2616 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/octave/investment_portfolio.py
--rw-r--r--   0        0        0    50277 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fld
--rw-r--r--   0        0        0     1651 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fll
--rw-r--r--   0        0        0     3516 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.py
--rw-r--r--   0        0        0    24574 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer.fld
--rw-r--r--   0        0        0      765 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer.fll
--rw-r--r--   0        0        0     1862 2024-01-11 00:28:25.622882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer.py
--rw-r--r--   0        0        0    36859 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer_chained.fld
--rw-r--r--   0        0        0     1195 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer_chained.fll
--rw-r--r--   0        0        0     2723 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer_chained.py
--rw-r--r--   0        0        0    36859 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer_inverse.fld
--rw-r--r--   0        0        0     1195 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer_inverse.fll
--rw-r--r--   0        0        0     2723 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer_inverse.py
--rw-r--r--   0        0        0      215 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/__init__.py
--rw-r--r--   0        0        0    49859 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/approximation.fld
--rw-r--r--   0        0        0     1927 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/approximation.fll
--rw-r--r--   0        0        0     3984 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/approximation.py
--rw-r--r--   0        0        0      410 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/__init__.py
--rw-r--r--   0        0        0    38334 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fld
--rw-r--r--   0        0        0     2524 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fll
--rw-r--r--   0        0        0     4762 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.py
--rw-r--r--   0        0        0    38262 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fld
--rw-r--r--   0        0        0     6722 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fll
--rw-r--r--   0        0        0    13825 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/invkine1.py
--rw-r--r--   0        0        0    38259 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fld
--rw-r--r--   0        0        0     5133 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fll
--rw-r--r--   0        0        0    10674 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/invkine2.py
--rw-r--r--   0        0        0    37614 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/juggler.fld
--rw-r--r--   0        0        0     1751 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/juggler.fll
--rw-r--r--   0        0        0     3943 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/juggler.py
--rw-r--r--   0        0        0    38551 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fld
--rw-r--r--   0        0        0     1076 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fll
--rw-r--r--   0        0        0     2669 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/membrn1.py
--rw-r--r--   0        0        0    38522 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fld
--rw-r--r--   0        0        0     1705 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fll
--rw-r--r--   0        0        0     3939 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/membrn2.py
--rw-r--r--   0        0        0    38833 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slbb.fld
--rw-r--r--   0        0        0     3394 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slbb.fll
--rw-r--r--   0        0        0     6518 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slbb.py
--rw-r--r--   0        0        0    39172 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcp.fld
--rw-r--r--   0        0        0     3386 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcp.fll
--rw-r--r--   0        0        0     6512 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcp.py
--rw-r--r--   0        0        0    76882 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fld
--rw-r--r--   0        0        0     1103 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fll
--rw-r--r--   0        0        0     2302 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcp1.py
--rw-r--r--   0        0        0    13064 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fld
--rw-r--r--   0        0        0     2744 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fll
--rw-r--r--   0        0        0     5057 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.py
--rw-r--r--   0        0        0    50135 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fld
--rw-r--r--   0        0        0      816 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fll
--rw-r--r--   0        0        0     1891 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.py
--rw-r--r--   0        0        0    25487 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fld
--rw-r--r--   0        0        0      614 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fll
--rw-r--r--   0        0        0     1485 2024-01-11 00:28:25.626882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.py
--rw-r--r--   0        0        0    38427 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fld
--rw-r--r--   0        0        0     1145 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fll
--rw-r--r--   0        0        0     2693 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/tanksg.py
--rw-r--r--   0        0        0    37709 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fld
--rw-r--r--   0        0        0      986 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fll
--rw-r--r--   0        0        0     2338 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/tippersg.py
--rw-r--r--   0        0        0    24593 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fld
--rw-r--r--   0        0        0      620 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fll
--rw-r--r--   0        0        0     1501 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.py
--rw-r--r--   0        0        0      244 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/__init__.py
--rw-r--r--   0        0        0    26243 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fld
--rw-r--r--   0        0        0     2109 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fll
--rw-r--r--   0        0        0     3994 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.py
--rw-r--r--   0        0        0    39580 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fld
--rw-r--r--   0        0        0     2505 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fll
--rw-r--r--   0        0        0     5136 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.py
--rw-r--r--   0        0        0    37976 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fld
--rw-r--r--   0        0        0     1124 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fll
--rw-r--r--   0        0        0     2659 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.py
--rw-r--r--   0        0        0    64628 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fld
--rw-r--r--   0        0        0     2646 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fll
--rw-r--r--   0        0        0     5360 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.py
--rw-r--r--   0        0        0    24574 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/simple_dimmer.fld
--rw-r--r--   0        0        0      743 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/simple_dimmer.fll
--rw-r--r--   0        0        0     1840 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/simple_dimmer.py
--rw-r--r--   0        0        0      707 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/__init__.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/arc.fld
--rw-r--r--   0        0        0      818 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/arc.fll
--rw-r--r--   0        0        0     1837 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/arc.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/bell.fld
--rw-r--r--   0        0        0      833 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/bell.fll
--rw-r--r--   0        0        0     1855 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/bell.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/binary.fld
--rw-r--r--   0        0        0      824 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/binary.fll
--rw-r--r--   0        0        0     1856 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/binary.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/concave.fld
--rw-r--r--   0        0        0      830 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/concave.fll
--rw-r--r--   0        0        0     1853 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/concave.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/constant.fld
--rw-r--r--   0        0        0      835 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/constant.fll
--rw-r--r--   0        0        0     1857 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/constant.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/cosine.fld
--rw-r--r--   0        0        0      827 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/cosine.fll
--rw-r--r--   0        0        0     1853 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/cosine.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/discrete.fld
--rw-r--r--   0        0        0     3233 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/discrete.fll
--rw-r--r--   0        0        0    15622 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/discrete.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/function.fld
--rw-r--r--   0        0        0     1007 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/function.fll
--rw-r--r--   0        0        0     2274 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/function.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/gaussian.fld
--rw-r--r--   0        0        0      833 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/gaussian.fll
--rw-r--r--   0        0        0     1861 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/gaussian.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/gaussian_product.fld
--rw-r--r--   0        0        0      878 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/gaussian_product.fll
--rw-r--r--   0        0        0     1988 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/gaussian_product.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/linear.fld
--rw-r--r--   0        0        0      841 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/linear.fll
--rw-r--r--   0        0        0     1863 2024-01-11 00:28:25.630882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/linear.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/pi_shape.fld
--rw-r--r--   0        0        0      854 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/pi_shape.fll
--rw-r--r--   0        0        0     1952 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/pi_shape.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/ramp.fld
--rw-r--r--   0        0        0      821 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/ramp.fll
--rw-r--r--   0        0        0     1837 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/ramp.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/rectangle.fld
--rw-r--r--   0        0        0      836 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/rectangle.fll
--rw-r--r--   0        0        0     1861 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/rectangle.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/semi_ellipse.fld
--rw-r--r--   0        0        0      842 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/semi_ellipse.fll
--rw-r--r--   0        0        0     1869 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/semi_ellipse.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid.fld
--rw-r--r--   0        0        0      833 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid.fll
--rw-r--r--   0        0        0     1852 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid_difference.fld
--rw-r--r--   0        0        0      888 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid_difference.fll
--rw-r--r--   0        0        0     1988 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid_difference.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid_product.fld
--rw-r--r--   0        0        0      881 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid_product.fll
--rw-r--r--   0        0        0     1978 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid_product.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/spike.fld
--rw-r--r--   0        0        0      824 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/spike.fll
--rw-r--r--   0        0        0     1849 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/spike.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/trapezoid.fld
--rw-r--r--   0        0        0      860 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/trapezoid.fll
--rw-r--r--   0        0        0     1956 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/trapezoid.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/triangle.fld
--rw-r--r--   0        0        0      845 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/triangle.fll
--rw-r--r--   0        0        0     1942 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/triangle.py
--rw-r--r--   0        0        0    24575 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/zs_shape.fld
--rw-r--r--   0        0        0      828 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/zs_shape.fll
--rw-r--r--   0        0        0     1847 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/terms/zs_shape.py
--rw-r--r--   0        0        0       48 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/tsukamoto/__init__.py
--rw-r--r--   0        0        0    61997 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/tsukamoto/tsukamoto.fld
--rw-r--r--   0        0        0     1629 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/tsukamoto/tsukamoto.fll
--rw-r--r--   0        0        0     3722 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/examples/tsukamoto/tsukamoto.py
--rw-r--r--   0        0        0    27206 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/exporter.py
--rw-r--r--   0        0        0    24708 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/factory.py
--rw-r--r--   0        0        0    40263 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/hedge.py
--rw-r--r--   0        0        0    17083 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/importer.py
--rw-r--r--   0        0        0    15021 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/library.py
--rw-r--r--   0        0        0    23089 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/norm.py
--rw-r--r--   0        0        0    16996 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/operation.py
--rw-r--r--   0        0        0        0 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/py.typed
--rw-r--r--   0        0        0    34909 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/rule.py
--rw-r--r--   0        0        0   101160 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/term.py
--rw-r--r--   0        0        0      278 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/types.py
--rw-r--r--   0        0        0    17502 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/fuzzylite/variable.py
--rw-r--r--   0        0        0    17073 2024-01-11 00:28:25.618882 pyfuzzylite-8.0.1/fuzzylite.png
--rw-r--r--   0        0        0     5226 2024-01-11 00:28:25.634882 pyfuzzylite-8.0.1/noxfile.py
--rw-r--r--   0        0        0       48 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/poetry.toml
--rw-r--r--   0        0        0     8471 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/pyproject.toml
--rw-r--r--   0        0        0       29 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/__init__.py
--rw-r--r--   0        0        0     4150 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/assert_component.py
--rw-r--r--   0        0        0     8974 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/notebooks/Hedges.ipynb
--rw-r--r--   0        0        0     4683 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/notebooks/Norms.ipynb
--rw-r--r--   0        0        0     9050 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/notebooks/Terms.ipynb
--rw-r--r--   0        0        0    25527 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_activation.py
--rw-r--r--   0        0        0    12037 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_benchmark.py
--rw-r--r--   0        0        0     7820 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_benchmark_codspeed.py
--rw-r--r--   0        0        0     8366 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_benchmark_pytest.py
--rw-r--r--   0        0        0    32083 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_defuzzifier.py
--rw-r--r--   0        0        0     3008 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_documentation.py
--rw-r--r--   0        0        0    36694 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_engine.py
--rw-r--r--   0        0        0     6106 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_examples.py
--rw-r--r--   0        0        0    39909 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_exporter.py
--rw-r--r--   0        0        0    18414 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_factory.py
--rw-r--r--   0        0        0     5297 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_hedge.py
--rw-r--r--   0        0        0    13578 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_importer.py
--rw-r--r--   0        0        0     8354 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_library.py
--rw-r--r--   0        0        0    16869 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_norm.py
--rw-r--r--   0        0        0    18108 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_operation.py
--rw-r--r--   0        0        0    40319 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_rule.py
--rw-r--r--   0        0        0    88012 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_term.py
--rw-r--r--   0        0        0    30049 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_variable.py
--rw-r--r--   0        0        0     7933 2024-01-11 00:28:25.638882 pyfuzzylite-8.0.1/tests/test_vectorization.py
--rw-r--r--   0        0        0     9430 1970-01-01 00:00:00.000000 pyfuzzylite-8.0.1/PKG-INFO
+-rw-r--r--   0        0        0       71 2024-04-26 03:53:28.031707 pyfuzzylite-8.0.2/AUTHOR
+-rw-r--r--   0        0        0      807 2024-04-26 03:53:28.031707 pyfuzzylite-8.0.2/CITATION.cff
+-rw-r--r--   0        0        0      142 2024-04-26 03:53:28.031707 pyfuzzylite-8.0.2/LICENSE.FuzzyLite.txt
+-rw-r--r--   0        0        0    35148 2024-04-26 03:53:28.031707 pyfuzzylite-8.0.2/LICENSE.GPL.txt
+-rw-r--r--   0        0        0     8480 2024-04-26 03:53:28.031707 pyfuzzylite-8.0.2/README.md
+-rw-r--r--   0        0        0     1082 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/__init__.py
+-rw-r--r--   0        0        0    17447 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/activation.py
+-rw-r--r--   0        0        0     7896 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/benchmark.py
+-rw-r--r--   0        0        0    21720 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/defuzzifier.py
+-rw-r--r--   0        0        0    24441 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/engine.py
+-rw-r--r--   0        0        0      134 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/__init__.py
+-rw-r--r--   0        0        0       84 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/__init__.py
+-rw-r--r--   0        0        0    36888 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/obstacle_avoidance.fld
+-rw-r--r--   0        0        0     1073 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/obstacle_avoidance.fll
+-rw-r--r--   0        0        0     2435 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/obstacle_avoidance.py
+-rw-r--r--   0        0        0    50840 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/tipper.fld
+-rw-r--r--   0        0        0     2103 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/tipper.fll
+-rw-r--r--   0        0        0     4431 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/tipper.py
+-rw-r--r--   0        0        0      347 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/__init__.py
+-rw-r--r--   0        0        0    24605 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/all_terms.fld
+-rw-r--r--   0        0        0     2986 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/all_terms.fll
+-rw-r--r--   0        0        0     6258 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/all_terms.py
+-rw-r--r--   0        0        0    49885 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/laundry.fld
+-rw-r--r--   0        0        0     1645 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/laundry.fll
+-rw-r--r--   0        0        0     5788 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/laundry.py
+-rw-r--r--   0        0        0      142 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/__init__.py
+-rw-r--r--   0        0        0    38421 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam21.fld
+-rw-r--r--   0        0        0     1034 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam21.fll
+-rw-r--r--   0        0        0     2392 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam21.py
+-rw-r--r--   0        0        0    51228 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam22.fld
+-rw-r--r--   0        0        0     1454 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam22.fll
+-rw-r--r--   0        0        0     3206 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam22.py
+-rw-r--r--   0        0        0    51731 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/shower.fld
+-rw-r--r--   0        0        0     2101 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/shower.fll
+-rw-r--r--   0        0        0     4507 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/shower.py
+-rw-r--r--   0        0        0    38427 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank.fld
+-rw-r--r--   0        0        0     1211 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank.fll
+-rw-r--r--   0        0        0     2754 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank.py
+-rw-r--r--   0        0        0    38441 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank2.fld
+-rw-r--r--   0        0        0     1194 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank2.fll
+-rw-r--r--   0        0        0     2681 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank2.py
+-rw-r--r--   0        0        0    37749 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper.fld
+-rw-r--r--   0        0        0      985 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper.fll
+-rw-r--r--   0        0        0     2338 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper.py
+-rw-r--r--   0        0        0    25357 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper1.fld
+-rw-r--r--   0        0        0      766 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper1.fll
+-rw-r--r--   0        0        0     1863 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper1.py
+-rw-r--r--   0        0        0    24592 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/obstacle_avoidance.fld
+-rw-r--r--   0        0        0      621 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/obstacle_avoidance.fll
+-rw-r--r--   0        0        0     1501 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/obstacle_avoidance.py
+-rw-r--r--   0        0        0      120 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/__init__.py
+-rw-r--r--   0        0        0    39013 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/investment_portfolio.fld
+-rw-r--r--   0        0        0     1209 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/investment_portfolio.fll
+-rw-r--r--   0        0        0     2616 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/investment_portfolio.py
+-rw-r--r--   0        0        0    50277 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fld
+-rw-r--r--   0        0        0     1651 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fll
+-rw-r--r--   0        0        0     3516 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.py
+-rw-r--r--   0        0        0    24574 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer.fld
+-rw-r--r--   0        0        0      765 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer.fll
+-rw-r--r--   0        0        0     1862 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer.py
+-rw-r--r--   0        0        0    36859 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_chained.fld
+-rw-r--r--   0        0        0     1195 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_chained.fll
+-rw-r--r--   0        0        0     2723 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_chained.py
+-rw-r--r--   0        0        0    36859 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_inverse.fld
+-rw-r--r--   0        0        0     1195 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_inverse.fll
+-rw-r--r--   0        0        0     2723 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_inverse.py
+-rw-r--r--   0        0        0      215 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/__init__.py
+-rw-r--r--   0        0        0    49859 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/approximation.fld
+-rw-r--r--   0        0        0     1927 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/approximation.fll
+-rw-r--r--   0        0        0     3984 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/approximation.py
+-rw-r--r--   0        0        0      410 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/__init__.py
+-rw-r--r--   0        0        0    38334 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fld
+-rw-r--r--   0        0        0     2524 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fll
+-rw-r--r--   0        0        0     4762 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.py
+-rw-r--r--   0        0        0    38262 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fld
+-rw-r--r--   0        0        0     6722 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fll
+-rw-r--r--   0        0        0    13825 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine1.py
+-rw-r--r--   0        0        0    38259 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fld
+-rw-r--r--   0        0        0     5133 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fll
+-rw-r--r--   0        0        0    10674 2024-04-26 03:53:28.075707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine2.py
+-rw-r--r--   0        0        0    37614 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/juggler.fld
+-rw-r--r--   0        0        0     1751 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/juggler.fll
+-rw-r--r--   0        0        0     3943 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/juggler.py
+-rw-r--r--   0        0        0    38551 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fld
+-rw-r--r--   0        0        0     1076 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fll
+-rw-r--r--   0        0        0     2669 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn1.py
+-rw-r--r--   0        0        0    38522 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fld
+-rw-r--r--   0        0        0     1705 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fll
+-rw-r--r--   0        0        0     3939 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn2.py
+-rw-r--r--   0        0        0    38833 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slbb.fld
+-rw-r--r--   0        0        0     3394 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slbb.fll
+-rw-r--r--   0        0        0     6518 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slbb.py
+-rw-r--r--   0        0        0    39172 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp.fld
+-rw-r--r--   0        0        0     3386 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp.fll
+-rw-r--r--   0        0        0     6512 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp.py
+-rw-r--r--   0        0        0    76882 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fld
+-rw-r--r--   0        0        0     1103 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fll
+-rw-r--r--   0        0        0     2302 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp1.py
+-rw-r--r--   0        0        0    13064 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fld
+-rw-r--r--   0        0        0     2744 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fll
+-rw-r--r--   0        0        0     5057 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.py
+-rw-r--r--   0        0        0    50135 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fld
+-rw-r--r--   0        0        0      816 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fll
+-rw-r--r--   0        0        0     1891 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.py
+-rw-r--r--   0        0        0    25487 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fld
+-rw-r--r--   0        0        0      614 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fll
+-rw-r--r--   0        0        0     1485 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.py
+-rw-r--r--   0        0        0    38427 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fld
+-rw-r--r--   0        0        0     1145 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fll
+-rw-r--r--   0        0        0     2693 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tanksg.py
+-rw-r--r--   0        0        0    37709 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fld
+-rw-r--r--   0        0        0      986 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fll
+-rw-r--r--   0        0        0     2338 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tippersg.py
+-rw-r--r--   0        0        0    24593 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fld
+-rw-r--r--   0        0        0      620 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fll
+-rw-r--r--   0        0        0     1501 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.py
+-rw-r--r--   0        0        0      244 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/__init__.py
+-rw-r--r--   0        0        0    26243 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fld
+-rw-r--r--   0        0        0     2109 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fll
+-rw-r--r--   0        0        0     3994 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.py
+-rw-r--r--   0        0        0    39580 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fld
+-rw-r--r--   0        0        0     2505 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fll
+-rw-r--r--   0        0        0     5136 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.py
+-rw-r--r--   0        0        0    37976 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fld
+-rw-r--r--   0        0        0     1124 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fll
+-rw-r--r--   0        0        0     2659 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.py
+-rw-r--r--   0        0        0    64628 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fld
+-rw-r--r--   0        0        0     2646 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fll
+-rw-r--r--   0        0        0     5360 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.py
+-rw-r--r--   0        0        0    24574 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/simple_dimmer.fld
+-rw-r--r--   0        0        0      743 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/simple_dimmer.fll
+-rw-r--r--   0        0        0     1840 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/simple_dimmer.py
+-rw-r--r--   0        0        0      707 2024-04-26 03:53:28.079707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/__init__.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/arc.fld
+-rw-r--r--   0        0        0      818 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/arc.fll
+-rw-r--r--   0        0        0     1837 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/arc.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/bell.fld
+-rw-r--r--   0        0        0      833 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/bell.fll
+-rw-r--r--   0        0        0     1855 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/bell.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/binary.fld
+-rw-r--r--   0        0        0      824 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/binary.fll
+-rw-r--r--   0        0        0     1856 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/binary.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/concave.fld
+-rw-r--r--   0        0        0      830 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/concave.fll
+-rw-r--r--   0        0        0     1853 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/concave.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/constant.fld
+-rw-r--r--   0        0        0      835 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/constant.fll
+-rw-r--r--   0        0        0     1857 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/constant.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/cosine.fld
+-rw-r--r--   0        0        0      827 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/cosine.fll
+-rw-r--r--   0        0        0     1853 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/cosine.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/discrete.fld
+-rw-r--r--   0        0        0     3233 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/discrete.fll
+-rw-r--r--   0        0        0    15622 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/discrete.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/function.fld
+-rw-r--r--   0        0        0     1007 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/function.fll
+-rw-r--r--   0        0        0     2274 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/function.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian.fld
+-rw-r--r--   0        0        0      833 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian.fll
+-rw-r--r--   0        0        0     1861 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian_product.fld
+-rw-r--r--   0        0        0      878 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian_product.fll
+-rw-r--r--   0        0        0     1988 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian_product.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/linear.fld
+-rw-r--r--   0        0        0      841 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/linear.fll
+-rw-r--r--   0        0        0     1863 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/linear.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/pi_shape.fld
+-rw-r--r--   0        0        0      854 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/pi_shape.fll
+-rw-r--r--   0        0        0     1952 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/pi_shape.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/ramp.fld
+-rw-r--r--   0        0        0      821 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/ramp.fll
+-rw-r--r--   0        0        0     1837 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/ramp.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/rectangle.fld
+-rw-r--r--   0        0        0      836 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/rectangle.fll
+-rw-r--r--   0        0        0     1861 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/rectangle.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/semi_ellipse.fld
+-rw-r--r--   0        0        0      842 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/semi_ellipse.fll
+-rw-r--r--   0        0        0     1869 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/semi_ellipse.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid.fld
+-rw-r--r--   0        0        0      833 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid.fll
+-rw-r--r--   0        0        0     1852 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_difference.fld
+-rw-r--r--   0        0        0      888 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_difference.fll
+-rw-r--r--   0        0        0     1988 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_difference.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_product.fld
+-rw-r--r--   0        0        0      881 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_product.fll
+-rw-r--r--   0        0        0     1978 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_product.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/spike.fld
+-rw-r--r--   0        0        0      824 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/spike.fll
+-rw-r--r--   0        0        0     1849 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/spike.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/trapezoid.fld
+-rw-r--r--   0        0        0      860 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/trapezoid.fll
+-rw-r--r--   0        0        0     1956 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/trapezoid.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/triangle.fld
+-rw-r--r--   0        0        0      845 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/triangle.fll
+-rw-r--r--   0        0        0     1942 2024-04-26 03:53:28.083707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/triangle.py
+-rw-r--r--   0        0        0    24575 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/zs_shape.fld
+-rw-r--r--   0        0        0      828 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/zs_shape.fll
+-rw-r--r--   0        0        0     1847 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/examples/terms/zs_shape.py
+-rw-r--r--   0        0        0       48 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/examples/tsukamoto/__init__.py
+-rw-r--r--   0        0        0    61997 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/examples/tsukamoto/tsukamoto.fld
+-rw-r--r--   0        0        0     1629 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/examples/tsukamoto/tsukamoto.fll
+-rw-r--r--   0        0        0     3722 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/examples/tsukamoto/tsukamoto.py
+-rw-r--r--   0        0        0    27206 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/exporter.py
+-rw-r--r--   0        0        0    24708 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/factory.py
+-rw-r--r--   0        0        0    40263 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/hedge.py
+-rw-r--r--   0        0        0    17083 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/importer.py
+-rw-r--r--   0        0        0    15021 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/library.py
+-rw-r--r--   0        0        0    23089 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/norm.py
+-rw-r--r--   0        0        0    16996 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/operation.py
+-rw-r--r--   0        0        0        0 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/py.typed
+-rw-r--r--   0        0        0    34909 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/rule.py
+-rw-r--r--   0        0        0   101160 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/term.py
+-rw-r--r--   0        0        0      278 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/types.py
+-rw-r--r--   0        0        0    17502 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/fuzzylite/variable.py
+-rw-r--r--   0        0        0    17073 2024-04-26 03:53:28.071707 pyfuzzylite-8.0.2/fuzzylite.png
+-rw-r--r--   0        0        0     5163 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/noxfile.py
+-rw-r--r--   0        0        0       48 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/poetry.toml
+-rw-r--r--   0        0        0     8471 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/pyproject.toml
+-rw-r--r--   0        0        0       29 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     4150 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/assert_component.py
+-rw-r--r--   0        0        0     8974 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/notebooks/Hedges.ipynb
+-rw-r--r--   0        0        0     4683 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/notebooks/Norms.ipynb
+-rw-r--r--   0        0        0     9050 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/notebooks/Terms.ipynb
+-rw-r--r--   0        0        0    25527 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_activation.py
+-rw-r--r--   0        0        0    12037 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_benchmark.py
+-rw-r--r--   0        0        0     7820 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_benchmark_codspeed.py
+-rw-r--r--   0        0        0     8366 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_benchmark_pytest.py
+-rw-r--r--   0        0        0    32083 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_defuzzifier.py
+-rw-r--r--   0        0        0     3008 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_documentation.py
+-rw-r--r--   0        0        0    40351 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_engine.py
+-rw-r--r--   0        0        0     6106 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_examples.py
+-rw-r--r--   0        0        0    39909 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_exporter.py
+-rw-r--r--   0        0        0    18414 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_factory.py
+-rw-r--r--   0        0        0     5297 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_hedge.py
+-rw-r--r--   0        0        0    13578 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_importer.py
+-rw-r--r--   0        0        0     8354 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_library.py
+-rw-r--r--   0        0        0    16869 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_norm.py
+-rw-r--r--   0        0        0    18108 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_operation.py
+-rw-r--r--   0        0        0    40319 2024-04-26 03:53:28.087707 pyfuzzylite-8.0.2/tests/test_rule.py
+-rw-r--r--   0        0        0    88012 2024-04-26 03:53:28.091707 pyfuzzylite-8.0.2/tests/test_term.py
+-rw-r--r--   0        0        0    30049 2024-04-26 03:53:28.091707 pyfuzzylite-8.0.2/tests/test_variable.py
+-rw-r--r--   0        0        0     7933 2024-04-26 03:53:28.091707 pyfuzzylite-8.0.2/tests/test_vectorization.py
+-rw-r--r--   0        0        0    10096 1970-01-01 00:00:00.000000 pyfuzzylite-8.0.2/PKG-INFO
```

### Comparing `pyfuzzylite-8.0.1/CITATION.cff` & `pyfuzzylite-8.0.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/LICENSE.GPL.txt` & `pyfuzzylite-8.0.2/LICENSE.GPL.txt`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/README.md` & `pyfuzzylite-8.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,29 @@
-# pyfuzzylite 8.0.1
-
-***
+# pyfuzzylite 8.0.2
 
 <img src="https://fuzzylite.github.io/pyfuzzylite/image/fuzzylite.svg" align="left" alt="fuzzylite">
 
 ## A Fuzzy Logic Control Library in Python
 
 by [**Juan Rada-Vilela, PhD**](https://fuzzylite.com/about)
 
+<br>
+<br>
+
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://opensource.org/license/gpl-3-0/)
 [![License: Paid](https://img.shields.io/badge/License-proprietary-blue)](mailto:sales@fuzzylite.com)
-
-***
-
-[main branch](https://github.com/fuzzylite/pyfuzzylite/tree/main)  
-[![Build](
-https://github.com/fuzzylite/pyfuzzylite/actions/workflows/build.yml/badge.svg?branch=main)](
-https://github.com/fuzzylite/pyfuzzylite/actions/workflows/build.yml)  
 [![Coverage Status](
 https://coveralls.io/repos/github/fuzzylite/pyfuzzylite/badge.svg?branch=main)](
 https://coveralls.io/github/fuzzylite/pyfuzzylite?branch=main)
-
-[development branch](https://github.com/fuzzylite/pyfuzzylite/tree/development)  
-[![Build](
-https://github.com/fuzzylite/pyfuzzylite/actions/workflows/build.yml/badge.svg?branch=development)](
-https://github.com/fuzzylite/pyfuzzylite/actions/workflows/build.yml)  
-[![Coverage Status](
-https://coveralls.io/repos/github/fuzzylite/pyfuzzylite/badge.svg?branch=development)](
-https://coveralls.io/github/fuzzylite/pyfuzzylite?branch=development)
-
-***
+[![Build](https://github.com/fuzzylite/pyfuzzylite/actions/workflows/build.yml/badge.svg)](
+https://github.com/fuzzylite/pyfuzzylite/actions/workflows/build.yml)
+[![Test](https://github.com/fuzzylite/pyfuzzylite/actions/workflows/test.yml/badge.svg)](
+https://github.com/fuzzylite/pyfuzzylite/actions/workflows/test.yml)
+[![Publish](https://github.com/fuzzylite/pyfuzzylite/actions/workflows/publish.yml/badge.svg)](
+https://github.com/fuzzylite/pyfuzzylite/actions/workflows/publish.yml)
 
 ## <a name="fuzzylite">FuzzyLite</a>
 
 **The FuzzyLite Libraries for Fuzzy Logic Control** refer to [`fuzzylite`](https://github.com/fuzzylite/fuzzylite/)
 (C++), [`pyfuzzylite`](https://github.com/fuzzylite/pyfuzzylite/) (Python),
 and [`jfuzzylite`](https://github.com/fuzzylite/jfuzzylite/) (Java).
 
@@ -175,19 +165,45 @@
                 fl.Rule.create("if obstacle is right then mSteer is left"),
             ],
         )
     ],
 )
 ```
 
+### `float` and vectorization
+
+```python
+# single `float` operation
+engine.input_variable("obstacle").value = 0.5
+engine.process()
+print("y =", engine.output_variable("mSteer").value)
+# > y = 0.5
+print("ỹ =", engine.output_variable("mSteer").fuzzy_value())
+# > ỹ = 0.500/left + 0.500/right
+
+# vectorization
+engine.input_variable("obstacle").value = fl.array([0, 0.25, 0.5, 0.75, 1.0])
+engine.process()
+print("y =", repr(engine.output_variable("mSteer").value))
+# > y = array([0.6666665 , 0.62179477, 0.5       , 0.37820523, 0.3333335 ])
+print("ỹ =", repr(engine.output_variable("mSteer").fuzzy_value()))
+# > ỹ = array(['0.000/left + 1.000/right',
+#              '0.250/left + 0.750/right',
+#              '0.500/left + 0.500/right',
+#              '0.750/left + 0.250/right',
+#              '1.000/left + 0.000/right'], dtype='<U26')
+```
+
+Please refer to the documentation for more
+information: [**fuzzylite.github.io/pyfuzzylite/**](https://fuzzylite.github.io/pyfuzzylite/)
+
 ## <a name="contributing">Contributing</a>
 
 All contributions are welcome, provided they follow the following guidelines:
 
-- Pull requests are made to the [development](https://github.com/fuzzylite/pyfuzzylite/tree/development) branch
 - Source code is consistent with standards in the library
 - Contribution is properly documented and tested, raising issues where appropriate
 - Contribution is licensed under the FuzzyLite License
 
 ## <a name="reference">Reference</a>
 
 If you are using the FuzzyLite Libraries, please cite the following reference in your article:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfuzzylite-8.0.1/fuzzylite/__init__.py` & `pyfuzzylite-8.0.2/fuzzylite/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/activation.py` & `pyfuzzylite-8.0.2/fuzzylite/activation.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/benchmark.py` & `pyfuzzylite-8.0.2/fuzzylite/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/defuzzifier.py` & `pyfuzzylite-8.0.2/fuzzylite/defuzzifier.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/engine.py` & `pyfuzzylite-8.0.2/fuzzylite/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,17 +319,17 @@
             | 2D array | sets each column of values to each input variable |
 
         Raises:
             RuntimeError: when there are no input variables
             ValueError: when the dimensionality of values is greater than 2
             ValueError: when the number of columns in the values is different from the number of input variables
         """
-        return np.atleast_2d(  # type:ignore
-            np.array([v.value for v in self.input_variables])
-        ).T
+        values = tuple(input_variable.value for input_variable in self.input_variables)
+        result = np.column_stack(values) if values else np.array(values)
+        return result
 
     @input_values.setter
     def input_values(self, values: ScalarArray) -> None:
         """Sets the input values of the engine.
 
         Args:
             values: input values of the engine.
@@ -375,17 +375,17 @@
     def output_values(self) -> ScalarArray:
         """Return a 2D array of output values (rows) for each output variable (columns).
 
         Returns:
             2D array of output values (rows) for each output variable (columns).
         """
         # TODO: Maybe a property setter like input_values.
-        return np.atleast_2d(  # type:ignore
-            np.array([v.value for v in self.output_variables])
-        ).T
+        values = tuple(output_variable.value for output_variable in self.output_variables)
+        result = np.column_stack(values) if values else np.array(values)
+        return result
 
     @property
     def values(self) -> ScalarArray:
         """Return a 2D array of current input and output values.
 
         Returns:
             2D array of current input and output values.
```

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/hybrid/obstacle_avoidance.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/obstacle_avoidance.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/hybrid/obstacle_avoidance.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/obstacle_avoidance.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/hybrid/obstacle_avoidance.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/obstacle_avoidance.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/hybrid/tipper.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/tipper.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/hybrid/tipper.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/tipper.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/hybrid/tipper.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/hybrid/tipper.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/all_terms.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/all_terms.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/all_terms.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/all_terms.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/all_terms.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/all_terms.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/laundry.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/laundry.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/laundry.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/laundry.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/laundry.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/laundry.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/mam21.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam21.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/mam21.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam21.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/mam21.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam21.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/mam22.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam22.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/mam22.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam22.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/mam22.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/mam22.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/shower.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/shower.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/shower.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/shower.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/shower.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/shower.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tank.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tank.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tank.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tank2.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank2.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tank2.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank2.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tank2.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tank2.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tipper.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tipper.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tipper.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tipper1.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper1.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tipper1.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper1.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/matlab/tipper1.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/matlab/tipper1.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/obstacle_avoidance.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/obstacle_avoidance.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/obstacle_avoidance.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/obstacle_avoidance.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/obstacle_avoidance.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/obstacle_avoidance.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/octave/investment_portfolio.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/investment_portfolio.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/octave/investment_portfolio.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/investment_portfolio.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/octave/investment_portfolio.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/investment_portfolio.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/octave/mamdani_tip_calculator.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer_chained.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_chained.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer_chained.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_chained.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer_chained.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_chained.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer_inverse.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_inverse.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer_inverse.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_inverse.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/mamdani/simple_dimmer_inverse.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/mamdani/simple_dimmer_inverse.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/approximation.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/approximation.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/approximation.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/approximation.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/approximation.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/approximation.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/fpeaks.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine1.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/invkine1.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine1.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine2.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/invkine2.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/invkine2.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/juggler.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/juggler.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/juggler.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/juggler.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/juggler.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/juggler.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn1.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/membrn1.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn1.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn2.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/membrn2.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/membrn2.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slbb.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slbb.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slbb.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slbb.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slbb.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slbb.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcp.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcp.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcp.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp1.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcp1.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcp1.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/slcpp1.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sltbu_fl.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/sugeno1.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tanksg.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/tanksg.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tanksg.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tippersg.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/matlab/tippersg.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/matlab/tippersg.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/obstacle_avoidance.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/cubic_approximator.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/heart_disease_risk.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/linear_tip_calculator.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/octave/sugeno_tip_calculator.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/simple_dimmer.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/simple_dimmer.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/simple_dimmer.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/simple_dimmer.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/takagi_sugeno/simple_dimmer.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/takagi_sugeno/simple_dimmer.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/__init__.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/arc.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/arc.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/arc.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/arc.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/arc.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/arc.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/bell.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/bell.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/bell.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/bell.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/bell.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/bell.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/binary.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/binary.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/binary.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/binary.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/binary.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/binary.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/concave.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/concave.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/concave.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/concave.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/concave.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/concave.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/constant.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/constant.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/constant.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/constant.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/constant.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/constant.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/cosine.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/cosine.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/cosine.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/cosine.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/cosine.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/cosine.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/discrete.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/discrete.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/discrete.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/discrete.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/discrete.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/discrete.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/function.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/function.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/function.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/function.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/function.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/function.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/gaussian.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/gaussian.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/gaussian.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/gaussian_product.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian_product.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/gaussian_product.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian_product.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/gaussian_product.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/gaussian_product.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/linear.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/linear.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/linear.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/linear.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/linear.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/linear.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/pi_shape.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/pi_shape.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/pi_shape.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/pi_shape.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/pi_shape.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/pi_shape.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/ramp.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/ramp.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/ramp.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/ramp.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/ramp.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/ramp.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/rectangle.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/rectangle.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/rectangle.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/rectangle.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/rectangle.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/rectangle.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/semi_ellipse.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/semi_ellipse.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/semi_ellipse.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/semi_ellipse.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/semi_ellipse.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/semi_ellipse.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid_difference.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_difference.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid_difference.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_difference.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid_difference.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_difference.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid_product.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_product.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid_product.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_product.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/sigmoid_product.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/sigmoid_product.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/spike.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/spike.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/spike.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/spike.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/spike.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/spike.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/trapezoid.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/trapezoid.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/trapezoid.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/trapezoid.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/trapezoid.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/trapezoid.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/triangle.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/triangle.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/triangle.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/triangle.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/triangle.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/triangle.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/zs_shape.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/zs_shape.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/zs_shape.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/zs_shape.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/terms/zs_shape.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/terms/zs_shape.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/tsukamoto/tsukamoto.fld` & `pyfuzzylite-8.0.2/fuzzylite/examples/tsukamoto/tsukamoto.fld`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/tsukamoto/tsukamoto.fll` & `pyfuzzylite-8.0.2/fuzzylite/examples/tsukamoto/tsukamoto.fll`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/examples/tsukamoto/tsukamoto.py` & `pyfuzzylite-8.0.2/fuzzylite/examples/tsukamoto/tsukamoto.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/exporter.py` & `pyfuzzylite-8.0.2/fuzzylite/exporter.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/factory.py` & `pyfuzzylite-8.0.2/fuzzylite/factory.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/hedge.py` & `pyfuzzylite-8.0.2/fuzzylite/hedge.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/importer.py` & `pyfuzzylite-8.0.2/fuzzylite/importer.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/library.py` & `pyfuzzylite-8.0.2/fuzzylite/library.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
     @property
     def version(self) -> str:
         """Automatic version of the library handled by poetry using `[tool.poetry_bumpversion.file."fuzzylite/library.py"]`.
 
         Returns:
             version of the library
         """
-        __version__ = "8.0.1"
+        __version__ = "8.0.2"
         return __version__
 
 
 information: Final = Information()
 
 
 class Representation(reprlib.Repr):
```

### Comparing `pyfuzzylite-8.0.1/fuzzylite/norm.py` & `pyfuzzylite-8.0.2/fuzzylite/norm.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/operation.py` & `pyfuzzylite-8.0.2/fuzzylite/operation.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/rule.py` & `pyfuzzylite-8.0.2/fuzzylite/rule.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/term.py` & `pyfuzzylite-8.0.2/fuzzylite/term.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite/variable.py` & `pyfuzzylite-8.0.2/fuzzylite/variable.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/fuzzylite.png` & `pyfuzzylite-8.0.2/fuzzylite.png`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/noxfile.py` & `pyfuzzylite-8.0.2/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 MARKDOWN_FILES = ["README.md", "THANKS.md", "docs/"]
 
 
 @nox.session(python=False)
 def check(session: nox.Session) -> None:
     """Check the `pyproject.toml` is valid."""
     session.run(*"poetry check".split(), external=True)
-    session.run(*"poetry check --lock".split(), external=True)
 
 
 @nox.session(python=False)
 def format(session: nox.Session) -> None:
     """Run code formatting."""
     files = PYTHON_FILES
```

### Comparing `pyfuzzylite-8.0.1/pyproject.toml` & `pyfuzzylite-8.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyfuzzylite"
-version = "8.0.1"
+version = "8.0.2"
 description = "a fuzzy logic control library in Python"
 license = "Proprietary"
 readme = "README.md"
 keywords = ["fuzzy logic control", "soft computing", "artificial intelligence"]
 authors = ["Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>"]
 maintainers = ["Juan Rada-Vilela, PhD <jcrada@fuzzylite.com>"]
 repository = "https://github.com/fuzzylite/pyfuzzylite.git"
```

### Comparing `pyfuzzylite-8.0.1/tests/assert_component.py` & `pyfuzzylite-8.0.2/tests/assert_component.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/notebooks/Hedges.ipynb` & `pyfuzzylite-8.0.2/tests/notebooks/Hedges.ipynb`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/notebooks/Norms.ipynb` & `pyfuzzylite-8.0.2/tests/notebooks/Norms.ipynb`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/notebooks/Terms.ipynb` & `pyfuzzylite-8.0.2/tests/notebooks/Terms.ipynb`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_activation.py` & `pyfuzzylite-8.0.2/tests/test_activation.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_benchmark.py` & `pyfuzzylite-8.0.2/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_benchmark_codspeed.py` & `pyfuzzylite-8.0.2/tests/test_benchmark_codspeed.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_benchmark_pytest.py` & `pyfuzzylite-8.0.2/tests/test_benchmark_pytest.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_defuzzifier.py` & `pyfuzzylite-8.0.2/tests/test_defuzzifier.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_documentation.py` & `pyfuzzylite-8.0.2/tests/test_documentation.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_engine.py` & `pyfuzzylite-8.0.2/tests/test_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -420,14 +420,105 @@
             fl.array([[1.0, 2.0, 3.0]]),
             raises=ValueError(
                 "expected an array with 2 columns (one for each input variable), "
                 "but got 3 columns: [[1. 2. 3.]]"
             ),
         )
 
+    def test_input_values(self) -> None:
+        """Test the engine.input_values."""
+        engine = fl.Engine("Test")
+        np.testing.assert_equal(fl.array([]), engine.input_values)
+
+        engine = fl.Engine("Test", input_variables=[fl.InputVariable("A")])
+        engine.input_variable(0).value = 0.6
+        np.testing.assert_equal(fl.array([[0.6]]), engine.input_values)
+
+        engine.input_variable(0).value = fl.array([0.6, 0.7])
+        np.testing.assert_equal(fl.array([[0.6], [0.7]]), engine.input_values)
+
+        engine = fl.Engine("Test", input_variables=[fl.InputVariable("A"), fl.InputVariable("B")])
+        engine.input_variable(0).value = 0.6
+        engine.input_variable(1).value = 0.2
+        np.testing.assert_equal(fl.array([[0.6, 0.2]]), engine.input_values)
+
+        engine.input_variable(0).value = fl.array([0.6, 0.7])
+        engine.input_variable(1).value = fl.array([0.2, 0.3])
+        np.testing.assert_equal(fl.array([[0.6, 0.2], [0.7, 0.3]]), engine.input_values)
+
+    def test_output_values(self) -> None:
+        """Test the engine.output_values."""
+        engine = fl.Engine("Test")
+        np.testing.assert_equal(fl.array([]), engine.output_values)
+
+        engine = fl.Engine("Test", output_variables=[fl.OutputVariable("A")])
+        engine.output_variable(0).value = 0.6
+        np.testing.assert_equal(fl.array([[0.6]]), engine.output_values)
+
+        engine.output_variable(0).value = fl.array([0.6, 0.7])
+        np.testing.assert_equal(fl.array([[0.6], [0.7]]), engine.output_values)
+
+        engine = fl.Engine(
+            "Test", output_variables=[fl.OutputVariable("A"), fl.OutputVariable("B")]
+        )
+        engine.output_variable(0).value = 0.6
+        engine.output_variable(1).value = 0.2
+        np.testing.assert_equal(fl.array([[0.6, 0.2]]), engine.output_values)
+
+        engine.output_variable(0).value = fl.array([0.6, 0.7])
+        engine.output_variable(1).value = fl.array([0.2, 0.3])
+        np.testing.assert_equal(fl.array([[0.6, 0.2], [0.7, 0.3]]), engine.output_values)
+
+    def test_input_values_manual_bug(self) -> None:
+        """Test the bug raised in https://github.com/fuzzylite/pyfuzzylite/issues/75."""
+        fll = """\
+Engine: ObstacleAvoidance
+InputVariable: obstacle
+  enabled: true
+  range: 0.000 1.000
+  lock-range: false
+  term: left Ramp 1.000 0.000
+  term: right Ramp 0.000 1.000
+InputVariable: obstacle2
+  enabled: true
+  range: 0.000 1.000
+  lock-range: false
+  term: left Ramp 1.000 0.000
+  term: right Ramp 0.000 1.000
+OutputVariable: tsSteer
+  enabled: true
+  range: 0.000 1.000
+  lock-range: false
+  aggregation: Maximum
+  defuzzifier: WeightedAverage
+  default: nan
+  lock-previous: false
+  term: right Linear 1 1 0
+  term: left Linear 0 1 1
+RuleBlock: takagiSugeno
+  enabled: true
+  conjunction: Minimum
+  disjunction: none
+  implication: none
+  activation: General
+  rule: if obstacle is left and obstacle2 is left then tsSteer is right
+  rule: if obstacle is left and obstacle2 is right then tsSteer is right"""
+        engine = fl.FllImporter().from_string(fll)
+        engine.input_variable(0).value = 0.2
+        engine.input_variable(1).value = 0.6
+        engine.process()
+        np.testing.assert_allclose(0.8, engine.output_values)
+        np.testing.assert_allclose(fl.array([[0.2, 0.6, 0.8]]), engine.values)
+
+        engine.input_variable(0).value = fl.array([0.2, 0.2])
+        engine.input_variable(1).value = fl.array([0.6, 0.6])
+        engine.process()
+        np.testing.assert_allclose(fl.array([[0.8], [0.8]]), engine.output_values)
+        np.testing.assert_allclose(fl.array([[0.2, 0.6, 0.8], [0.2, 0.6, 0.8]]), engine.values)
+
     def test_repr(self) -> None:
         """Tests repr."""
         code = fl.repr(SimpleDimmer().engine)
         engine = eval(code)
         engine.input_variables[0].value = 1 / 3
         engine.process()
         np.testing.assert_allclose(
```

### Comparing `pyfuzzylite-8.0.1/tests/test_examples.py` & `pyfuzzylite-8.0.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_exporter.py` & `pyfuzzylite-8.0.2/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_factory.py` & `pyfuzzylite-8.0.2/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_hedge.py` & `pyfuzzylite-8.0.2/tests/test_hedge.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_importer.py` & `pyfuzzylite-8.0.2/tests/test_importer.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_library.py` & `pyfuzzylite-8.0.2/tests/test_library.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 variable InputVariable OutputVariable Variable
 """
         self.assertSetEqual(set(expected.split()), set(vars(fl)))
 
     def test_library_vars(self) -> None:
         """Test the library variables."""
-        __version__ = "8.0.1"
+        __version__ = "8.0.2"
         self.assertEqual(fl.__name__, "fuzzylite")
         self.assertEqual(fl.__version__, __version__)
         self.assertEqual(fl.__doc__, fl.information.description)
 
     def test_context(self) -> None:
         """Tests the context."""
         # float_type
```

### Comparing `pyfuzzylite-8.0.1/tests/test_norm.py` & `pyfuzzylite-8.0.2/tests/test_norm.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_operation.py` & `pyfuzzylite-8.0.2/tests/test_operation.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_rule.py` & `pyfuzzylite-8.0.2/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_term.py` & `pyfuzzylite-8.0.2/tests/test_term.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_variable.py` & `pyfuzzylite-8.0.2/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/tests/test_vectorization.py` & `pyfuzzylite-8.0.2/tests/test_vectorization.py`

 * *Files identical despite different names*

### Comparing `pyfuzzylite-8.0.1/PKG-INFO` & `pyfuzzylite-8.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfuzzylite
-Version: 8.0.1
+Version: 8.0.2
 Summary: a fuzzy logic control library in Python
 Home-page: https://github.com/fuzzylite/pyfuzzylite.git
 License: Proprietary
 Keywords: fuzzy logic control,soft computing,artificial intelligence
 Author: Juan Rada-Vilela, PhD
 Author-email: jcrada@fuzzylite.com
 Maintainer: Juan Rada-Vilela, PhD
@@ -29,46 +29,36 @@
 Requires-Dist: numpy (>=1.20,<2.0)
 Project-URL: Bug Tracker, https://github.com/fuzzylite/pyfuzzylite/issues
 Project-URL: Documentation, https://fuzzylite.github.io/pyfuzzylite/
 Project-URL: Repository, https://github.com/fuzzylite/pyfuzzylite.git
 Project-URL: Source Code, https://github.com/fuzzylite/pyfuzzylite
 Description-Content-Type: text/markdown
 
-# pyfuzzylite 8.0.1
-
-***
+# pyfuzzylite 8.0.2
 
 <img src="https://fuzzylite.github.io/pyfuzzylite/image/fuzzylite.svg" align="left" alt="fuzzylite">
 
 ## A Fuzzy Logic Control Library in Python
 
 by [**Juan Rada-Vilela, PhD**](https://fuzzylite.com/about)
 
+<br>
+<br>
+
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://opensource.org/license/gpl-3-0/)
 [![License: Paid](https://img.shields.io/badge/License-proprietary-blue)](mailto:sales@fuzzylite.com)
-
-***
-
-[main branch](https://github.com/fuzzylite/pyfuzzylite/tree/main)  
-[![Build](
-https://github.com/fuzzylite/pyfuzzylite/actions/workflows/build.yml/badge.svg?branch=main)](
-https://github.com/fuzzylite/pyfuzzylite/actions/workflows/build.yml)  
 [![Coverage Status](
 https://coveralls.io/repos/github/fuzzylite/pyfuzzylite/badge.svg?branch=main)](
 https://coveralls.io/github/fuzzylite/pyfuzzylite?branch=main)
-
-[development branch](https://github.com/fuzzylite/pyfuzzylite/tree/development)  
-[![Build](
-https://github.com/fuzzylite/pyfuzzylite/actions/workflows/build.yml/badge.svg?branch=development)](
-https://github.com/fuzzylite/pyfuzzylite/actions/workflows/build.yml)  
-[![Coverage Status](
-https://coveralls.io/repos/github/fuzzylite/pyfuzzylite/badge.svg?branch=development)](
-https://coveralls.io/github/fuzzylite/pyfuzzylite?branch=development)
-
-***
+[![Build](https://github.com/fuzzylite/pyfuzzylite/actions/workflows/build.yml/badge.svg)](
+https://github.com/fuzzylite/pyfuzzylite/actions/workflows/build.yml)
+[![Test](https://github.com/fuzzylite/pyfuzzylite/actions/workflows/test.yml/badge.svg)](
+https://github.com/fuzzylite/pyfuzzylite/actions/workflows/test.yml)
+[![Publish](https://github.com/fuzzylite/pyfuzzylite/actions/workflows/publish.yml/badge.svg)](
+https://github.com/fuzzylite/pyfuzzylite/actions/workflows/publish.yml)
 
 ## <a name="fuzzylite">FuzzyLite</a>
 
 **The FuzzyLite Libraries for Fuzzy Logic Control** refer to [`fuzzylite`](https://github.com/fuzzylite/fuzzylite/)
 (C++), [`pyfuzzylite`](https://github.com/fuzzylite/pyfuzzylite/) (Python),
 and [`jfuzzylite`](https://github.com/fuzzylite/jfuzzylite/) (Java).
 
@@ -210,19 +200,45 @@
                 fl.Rule.create("if obstacle is right then mSteer is left"),
             ],
         )
     ],
 )
 ```
 
+### `float` and vectorization
+
+```python
+# single `float` operation
+engine.input_variable("obstacle").value = 0.5
+engine.process()
+print("y =", engine.output_variable("mSteer").value)
+# > y = 0.5
+print("ỹ =", engine.output_variable("mSteer").fuzzy_value())
+# > ỹ = 0.500/left + 0.500/right
+
+# vectorization
+engine.input_variable("obstacle").value = fl.array([0, 0.25, 0.5, 0.75, 1.0])
+engine.process()
+print("y =", repr(engine.output_variable("mSteer").value))
+# > y = array([0.6666665 , 0.62179477, 0.5       , 0.37820523, 0.3333335 ])
+print("ỹ =", repr(engine.output_variable("mSteer").fuzzy_value()))
+# > ỹ = array(['0.000/left + 1.000/right',
+#              '0.250/left + 0.750/right',
+#              '0.500/left + 0.500/right',
+#              '0.750/left + 0.250/right',
+#              '1.000/left + 0.000/right'], dtype='<U26')
+```
+
+Please refer to the documentation for more
+information: [**fuzzylite.github.io/pyfuzzylite/**](https://fuzzylite.github.io/pyfuzzylite/)
+
 ## <a name="contributing">Contributing</a>
 
 All contributions are welcome, provided they follow the following guidelines:
 
-- Pull requests are made to the [development](https://github.com/fuzzylite/pyfuzzylite/tree/development) branch
 - Source code is consistent with standards in the library
 - Contribution is properly documented and tested, raising issues where appropriate
 - Contribution is licensed under the FuzzyLite License
 
 ## <a name="reference">Reference</a>
 
 If you are using the FuzzyLite Libraries, please cite the following reference in your article:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

