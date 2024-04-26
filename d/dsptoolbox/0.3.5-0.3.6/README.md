# Comparing `tmp/dsptoolbox-0.3.5.tar.gz` & `tmp/dsptoolbox-0.3.6.tar.gz`

## Comparing `dsptoolbox-0.3.5.tar` & `dsptoolbox-0.3.6.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/.gitattributes
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/.readthedocs.yaml
--rw-r--r--   0        0        0    18324 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/CHANGELOG.rst
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/requirements.txt
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/Makefile
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/__rdme.rst
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/classes.rst
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/conf.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/index.rst
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/make.bat
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules.rst
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/readme.rst
--rw-r--r--   0        0        0   262622 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/logo/logo.png
--rw-r--r--   0        0        0   262793 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/logo/logo2.png
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.audio_io.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.beamforming.rst
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.distances.rst
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.effects.rst
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.filterbanks.rst
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.generators.rst
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.plots.rst
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.room_acoustics.rst
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.standard_functions.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.transfer_functions.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.transforms.rst
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/__init__.py
--rw-r--r--   0        0        0    37498 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/_general_helpers.py
--rw-r--r--   0        0        0    36355 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/_standard.py
--rw-r--r--   0        0        0    46103 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/standard_functions.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/audio_io/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/audio_io/_audio_io.py
--rw-r--r--   0        0        0    14939 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/audio_io/audio_io.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/beamforming/__init__.py
--rw-r--r--   0        0        0     9865 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/beamforming/_beamforming.py
--rw-r--r--   0        0        0    62886 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/beamforming/beamforming.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/__init__.py
--rw-r--r--   0        0        0    20948 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/_filter.py
--rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/_lattice_ladder_filter.py
--rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/_phaseLinearizer.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/_plots.py
--rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/_svfilter.py
--rw-r--r--   0        0        0    32846 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/filter_class.py
--rw-r--r--   0        0        0    29479 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/filterbank.py
--rw-r--r--   0        0        0    16030 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/multibandsignal.py
--rw-r--r--   0        0        0    57889 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/signal_class.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/distances/__init__.py
--rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/distances/_distances.py
--rw-r--r--   0        0        0    13049 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/distances/distances.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/effects/__init__.py
--rw-r--r--   0        0        0    18619 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/effects/_effects.py
--rw-r--r--   0        0        0    58609 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/effects/effects.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/filterbanks/__init__.py
--rw-r--r--   0        0        0    48939 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/filterbanks/_filterbank.py
--rw-r--r--   0        0        0    16152 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/filterbanks/filterbanks.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/generators/__init__.py
--rw-r--r--   0        0        0    18264 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/generators/generators.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/plots/__init__.py
--rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/plots/plots.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/room_acoustics/__init__.py
--rw-r--r--   0        0        0    43582 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/room_acoustics/_room_acoustics.py
--rw-r--r--   0        0        0    25842 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/room_acoustics/room_acoustics.py
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/transfer_functions/__init__.py
--rw-r--r--   0        0        0    10926 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/transfer_functions/_transfer_functions.py
--rw-r--r--   0        0        0    60900 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/transfer_functions/transfer_functions.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/transforms/__init__.py
--rw-r--r--   0        0        0    11056 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/transforms/_transforms.py
--rw-r--r--   0        0        0    30334 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/transforms/transforms.py
--rw-r--r--   0        0        0    46390 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/audio_io_module.ipynb
--rw-r--r--   0        0        0   369566 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/beamforming_module.ipynb
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/distances_module.ipynb
--rw-r--r--   0        0        0   409017 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/filterbanks_module.ipynb
--rw-r--r--   0        0        0  1013477 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/general.ipynb
--rw-r--r--   0        0        0   244031 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/generators_module.ipynb
--rw-r--r--   0        0        0   180489 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/room_acoustics_module.ipynb
--rw-r--r--   0        0        0    94731 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/standard_module.ipynb
--rw-r--r--   0        0        0   208870 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/transfer_function_module.ipynb
--rw-r--r--   0        0        0  1248737 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/transforms_module.ipynb
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/data/array.xml
--rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/data/chirp.wav
--rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/data/chirp_mono.wav
--rw-r--r--   0        0        0   768044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/data/chirp_stereo.wav
--rw-r--r--   0        0        0  1766444 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/data/fuer_elise.wav
--rw-r--r--   0        0        0    96044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/data/rir.wav
--rw-r--r--   0        0        0   187792 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/data/speech.flac
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_audio_io.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_beamforming.py
--rw-r--r--   0        0        0    34170 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_classes.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_distances.py
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_filterbanks.py
--rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_fx.py
--rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_generators.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_room_acoustics.py
--rw-r--r--   0        0        0    13083 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_standard.py
--rw-r--r--   0        0        0    17635 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_transfer_functions.py
--rw-r--r--   0        0        0     5930 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_transforms.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/LICENSE
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/README.rst
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/.gitattributes
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/.readthedocs.yaml
+-rw-r--r--   0        0        0    18569 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/CHANGELOG.rst
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/requirements.txt
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/Makefile
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/__rdme.rst
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/classes.rst
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/conf.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/index.rst
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/make.bat
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/modules.rst
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/readme.rst
+-rw-r--r--   0        0        0   262622 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/logo/logo.png
+-rw-r--r--   0        0        0   262793 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/logo/logo2.png
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/modules/dsptoolbox.audio_io.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/modules/dsptoolbox.beamforming.rst
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/modules/dsptoolbox.distances.rst
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/modules/dsptoolbox.effects.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/modules/dsptoolbox.filterbanks.rst
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/modules/dsptoolbox.generators.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/modules/dsptoolbox.plots.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/modules/dsptoolbox.room_acoustics.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/modules/dsptoolbox.standard_functions.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/modules/dsptoolbox.transfer_functions.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/docs/modules/dsptoolbox.transforms.rst
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/__init__.py
+-rw-r--r--   0        0        0    37498 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/_general_helpers.py
+-rw-r--r--   0        0        0    36355 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/_standard.py
+-rw-r--r--   0        0        0    47469 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/standard_functions.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/audio_io/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/audio_io/_audio_io.py
+-rw-r--r--   0        0        0    17827 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/audio_io/audio_io.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/beamforming/__init__.py
+-rw-r--r--   0        0        0     9865 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/beamforming/_beamforming.py
+-rw-r--r--   0        0        0    62886 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/beamforming/beamforming.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/classes/__init__.py
+-rw-r--r--   0        0        0    20948 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/classes/_filter.py
+-rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/classes/_lattice_ladder_filter.py
+-rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/classes/_phaseLinearizer.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/classes/_plots.py
+-rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/classes/_svfilter.py
+-rw-r--r--   0        0        0    32846 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/classes/filter_class.py
+-rw-r--r--   0        0        0    29479 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/classes/filterbank.py
+-rw-r--r--   0        0        0    16030 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/classes/multibandsignal.py
+-rw-r--r--   0        0        0    57835 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/classes/signal_class.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/distances/__init__.py
+-rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/distances/_distances.py
+-rw-r--r--   0        0        0    13049 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/distances/distances.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/effects/__init__.py
+-rw-r--r--   0        0        0    18619 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/effects/_effects.py
+-rw-r--r--   0        0        0    58609 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/effects/effects.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/filterbanks/__init__.py
+-rw-r--r--   0        0        0    48939 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/filterbanks/_filterbank.py
+-rw-r--r--   0        0        0    17996 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/filterbanks/filterbanks.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/generators/__init__.py
+-rw-r--r--   0        0        0    18264 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/generators/generators.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/plots/__init__.py
+-rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/plots/plots.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/room_acoustics/__init__.py
+-rw-r--r--   0        0        0    43582 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/room_acoustics/_room_acoustics.py
+-rw-r--r--   0        0        0    25842 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/room_acoustics/room_acoustics.py
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/transfer_functions/__init__.py
+-rw-r--r--   0        0        0    10926 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/transfer_functions/_transfer_functions.py
+-rw-r--r--   0        0        0    60900 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/transfer_functions/transfer_functions.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/transforms/__init__.py
+-rw-r--r--   0        0        0    11056 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/transforms/_transforms.py
+-rw-r--r--   0        0        0    30334 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/dsptoolbox/transforms/transforms.py
+-rw-r--r--   0        0        0    46390 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/audio_io_module.ipynb
+-rw-r--r--   0        0        0   369566 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/beamforming_module.ipynb
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/distances_module.ipynb
+-rw-r--r--   0        0        0   409017 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/filterbanks_module.ipynb
+-rw-r--r--   0        0        0  1013477 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/general.ipynb
+-rw-r--r--   0        0        0   244031 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/generators_module.ipynb
+-rw-r--r--   0        0        0   180489 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/room_acoustics_module.ipynb
+-rw-r--r--   0        0        0    94731 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/standard_module.ipynb
+-rw-r--r--   0        0        0   208870 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/transfer_function_module.ipynb
+-rw-r--r--   0        0        0  1248737 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/transforms_module.ipynb
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/data/array.xml
+-rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/data/chirp.wav
+-rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/data/chirp_mono.wav
+-rw-r--r--   0        0        0   768044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/data/chirp_stereo.wav
+-rw-r--r--   0        0        0  1766444 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/data/fuer_elise.wav
+-rw-r--r--   0        0        0    96044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/data/rir.wav
+-rw-r--r--   0        0        0   187792 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/examples/data/speech.flac
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/tests/test_audio_io.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/tests/test_beamforming.py
+-rw-r--r--   0        0        0    34170 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/tests/test_classes.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/tests/test_distances.py
+-rw-r--r--   0        0        0     9040 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/tests/test_filterbanks.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/tests/test_fx.py
+-rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/tests/test_generators.py
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/tests/test_room_acoustics.py
+-rw-r--r--   0        0        0    12211 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/tests/test_standard.py
+-rw-r--r--   0        0        0    17635 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/tests/test_transfer_functions.py
+-rw-r--r--   0        0        0     5930 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/tests/test_transforms.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/LICENSE
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/README.rst
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 dsptoolbox-0.3.6/PKG-INFO
```

### Comparing `dsptoolbox-0.3.5/.readthedocs.yaml` & `dsptoolbox-0.3.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/CHANGELOG.rst` & `dsptoolbox-0.3.6/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,26 @@
 
 `To Do's for future releases`_
 ------------------------------
 
 - Validation for results from tests in every module (so far many tests are
   only regarding functionality)
 
+`0.3.6 <https://pypi.org/project/dsptoolbox/0.3.6>`_ - 
+---------------------
+
+Added
+~~~~~~~
+- `set_latency` and `set_blocksize` in ``audio_io``
+- `dither` in ``standard``
+
+Misc
+~~~~~~
+- general documentation and small performance improvements
+
 `0.3.5 <https://pypi.org/project/dsptoolbox/0.3.5>`_ - 
 ---------------------
 
 Added
 ~~~~~~~
 - `harmonic_distortion_analysis` in ``transfer_functions``
 - added possibility of scaling the spectrogram
```

### Comparing `dsptoolbox-0.3.5/docs/Makefile` & `dsptoolbox-0.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/docs/classes.rst` & `dsptoolbox-0.3.6/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/docs/conf.py` & `dsptoolbox-0.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/docs/index.rst` & `dsptoolbox-0.3.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/docs/make.bat` & `dsptoolbox-0.3.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/docs/modules.rst` & `dsptoolbox-0.3.6/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/docs/readme.rst` & `dsptoolbox-0.3.6/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/docs/logo/logo.png` & `dsptoolbox-0.3.6/docs/logo/logo.png`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/docs/logo/logo2.png` & `dsptoolbox-0.3.6/docs/logo/logo2.png`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/__init__.py` & `dsptoolbox-0.3.6/dsptoolbox/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     resample,
     load_pkl_object,
     erb_frequencies,
     detrend,
     rms,
     CalibrationData,
     envelope,
-    convert_into_lattice_filter,
+    dither,
 )
 from .classes import (
     Filter,
     FilterBank,
     Signal,
     MultiBandSignal,
 )
@@ -55,22 +55,22 @@
     "erb_frequencies",
     "load_pkl_object",
     "fractional_octave_frequencies",
     "detrend",
     "rms",
     "CalibrationData",
     "envelope",
-    "convert_into_lattice_filter",
+    "dither",
     # Modules
     "transfer_functions",
     "distances",
     "room_acoustics",
     "plots",
     "generators",
     "filterbanks",
     "transforms",
     "audio_io",
     "beamforming",
     "effects",
 ]
 
-__version__ = "0.3.5"
+__version__ = "0.3.6"
```

### Comparing `dsptoolbox-0.3.5/dsptoolbox/_general_helpers.py` & `dsptoolbox-0.3.6/dsptoolbox/_general_helpers.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/_standard.py` & `dsptoolbox-0.3.6/dsptoolbox/_standard.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/standard_functions.py` & `dsptoolbox-0.3.6/dsptoolbox/standard_functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,20 +16,14 @@
 
 from .classes import (
     Signal,
     MultiBandSignal,
     FilterBank,
     Filter,
 )
-from .classes._lattice_ladder_filter import (
-    LatticeLadderFilter,
-    _get_lattice_ladder_coefficients_iir,
-    _get_lattice_coefficients_fir,
-    _get_lattice_ladder_coefficients_iir_sos,
-)
 from ._standard import (
     _latency,
     _center_frequencies_fractional_octaves_iec,
     _exact_center_frequencies_fractional_octaves,
     # _kaiser_window_beta,
     _indices_above_threshold_dbfs,
     _detrend,
@@ -1278,50 +1272,91 @@
                 b, mode=mode, window_length_samples=window_length_samples
             )
         return rms_vec
     else:
         raise TypeError("Signal must be type Signal or MultiBandSignal")
 
 
-def convert_into_lattice_filter(filt: Filter) -> LatticeLadderFilter:
-    """Convert an IIR or FIR filter into its lattice-ladder filter
-    representation. Filtering is then done using the lattice coefficients.
-    If the filter uses second-order sections, the lattice-ladder coefficients
-    are also computed and used in second-order sections.
+def dither(
+    s: Signal,
+    mode: str = "triangular",
+    epsilon: float = float(np.finfo(np.float16).smallest_subnormal),
+    noise_shaping_filterbank: FilterBank | None = None,
+    truncate: bool = False,
+) -> Signal:
+    """
+    This function applies dither to the signal and, optionally, truncates the
+    time samples to 16-bits floating point representation.
 
     Parameters
     ----------
-    filt: `Filter`
-        Filter to convert into its lattice filter representation.
+    s : `Signal`
+        Signal to apply dither to.
+    mode : str, optional
+        Type of probability distribution to use noise from. Choose from
+        `"rectangular"`, `"triangular"`. See notes and references for details.
+        Default: `"triangular"`.
+    epsilon : float, optional
+        Value that represents the quantization step. The default value supposes
+        quantization to 16-bit floating point. It is obtained through numpy's
+        smallest subnormal for np.float16. See notes for the value concerning
+        the 24-bit case. Default: 6e-08.
+    noise_shaping_filterbank : `FilterBank`, `None`, optional
+        Noise can be arbitrarily shaped using a filter bank (in sequential
+        mode). Pass `None` to avoid any noise-shaping. Default: `None`.
+    truncate : bool, optional
+        When `True`, the time samples are truncated to np.float16 resolution.
+        `False` only applies dither noise to the signal without truncating.
+        Default: `False`.
 
     Returns
     -------
-    new_filt : `LatticeLadderFilter`
-        New filter representation.
+    new_s : `Signal`
+        Signal with dither.
 
     Notes
     -----
-    - Linear phase FIR filters produce unstable reflection coefficients and
-      can therefore not be converted into lattice filters. When trying to do
-      this, an assertion error is raised.
+    - The output signal has time samples with 16-bit precision, but the data
+      type of the array is `np.float64` for consistency.
+    - `"rectangular"` mode applies noise with samples coming from a uniform
+      distribution [-epsilon/2, epsilon/2]. `"triangular"` has a triangle shape
+      for the noise distribution with values between [-epsilon, epsilon]. See
+      [1] for more details on this.
+    - Dither might be only necessary when lowering the bit-depth down to 16
+      bits, though the 24-bit case might be relevant if the there are signal
+      components with very low volumes.
+    - 24-bit signed integers range from -8388608 to 8388607. The quantization
+      step is therefore `1/8388608=1.1920928955078125e-07`.
+
+    References
+    ----------
+    - [1]: Lerch, Weinzierl. Handbuch der Audiotechnik: Chapter 14.
 
     """
-    if filt.filter_type in ("iir", "biquad"):
-        if hasattr(filt, "sos"):
-            sos = filt.get_coefficients("sos")
-            k, c = _get_lattice_ladder_coefficients_iir_sos(sos)
-        else:
-            b, a = filt.get_coefficients("ba")
-            k, c = _get_lattice_ladder_coefficients_iir(b, a)
-        new_filt = LatticeLadderFilter(k, c, filt.sampling_rate_hz)
-    elif filt.filter_type == "fir":
-        b, a = filt.get_coefficients("ba")
-        b /= b[0]
-        k = _get_lattice_coefficients_fir(b)
-        assert np.all(np.abs(k) < 1), (
-            "Some reflection coefficient was "
-            + "equal or larger than zero, this is not supported"
+    mode = mode.lower()
+    shape = s.time_data.shape
+
+    if mode == "rectangular":
+        noise = np.random.uniform(-epsilon / 2, epsilon / 2, size=shape)
+    elif mode == "triangular":
+        noise = np.random.uniform(
+            -epsilon / 2, epsilon / 2, size=shape
+        ) + np.random.uniform(-epsilon / 2, epsilon / 2, size=shape)
+    else:
+        raise ValueError(f"{mode} is not supported.")
+
+    if noise_shaping_filterbank is not None:
+        noise_s = Signal(None, noise, s.sampling_rate_hz)
+        noise_s = noise_shaping_filterbank.filter_signal(
+            noise_s, mode="sequential"
         )
-        new_filt = LatticeLadderFilter(k, None, filt.sampling_rate_hz)
+        noise = noise_s.time_data
+
+    new_s = s.copy()
+
+    if truncate:
+        new_s.time_data = (
+            (new_s.time_data + noise).astype(np.float16)
+        ).astype(np.float64)
     else:
-        raise ValueError(f"Unsupported filter type: {filt.filter_type}")
-    return new_filt
+        new_s.time_data = new_s.time_data + noise
+    return new_s
```

### Comparing `dsptoolbox-0.3.5/dsptoolbox/audio_io/__init__.py` & `dsptoolbox-0.3.6/dsptoolbox/audio_io/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 are just wrappers around sounddevice's functions:
 
 Setting audio device:
 
 - `set_device()`
 - `print_device_info()`
 - `default_config`
+- `set_latency()`
+- `set_blocksize()`
 
 Playing audio:
 
 - `play()`
 - `play_through_stream()`
 - `play_and_record()`
 - `output_stream()`
@@ -29,34 +31,39 @@
 - `sleep()` (sleep while audio playback is finished)
 
 References
 ----------
 - https://pypi.org/project/sounddevice/
 
 """
+
 from .audio_io import (
     play,
     play_and_record,
     set_device,
     record,
     print_device_info,
     play_through_stream,
     CallbackStop,
     standard_callback,
     sleep,
     output_stream,
     default_config,
+    set_latency,
+    set_blocksize,
 )
 
 __all__ = [
     "play",
     "play_and_record",
     "set_device",
     "record",
     "print_device_info",
     "play_through_stream",
     "CallbackStop",
     "standard_callback",
     "sleep",
     "output_stream",
     "default_config",
+    "set_latency",
+    "set_blocksize",
 ]
```

### Comparing `dsptoolbox-0.3.5/dsptoolbox/audio_io/_audio_io.py` & `dsptoolbox-0.3.6/dsptoolbox/audio_io/_audio_io.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/audio_io/audio_io.py` & `dsptoolbox-0.3.6/dsptoolbox/audio_io/audio_io.py`

 * *Files 24% similar despite different names*

```diff
@@ -35,80 +35,171 @@
         return d
     else:
         d = sd.query_devices(device_number)
         print(d)
         return d
 
 
+def set_latency(input_low: bool, output_low: bool):
+    """
+    Set the desired latency (Default is high). This can vary for each device
+    and host. Sounddevice only allows for setting a low or a high latency.
+    High latency is more robust, but it might be too large for some
+    applications.
+
+    Parameters
+    ----------
+    input_low : bool
+        When `True`, low latency will be requested to the host for input
+        streams.
+    output_low : bool
+        When `True`, low latency will be requested to the host for output
+        streams.
+
+    """
+    sd.default.latency = (
+        "low" if input_low else "high",
+        "low" if output_low else "high",
+    )
+
+
+def set_blocksize(blocksize: int):
+    """
+    Set a default blocksize for any stream. This can lead to a stable latency
+    for most interfaces. Not setting it will lead to a default value.
+
+    Parameters
+    ----------
+    blocksize : int
+        Desired block size.
+
+    """
+    sd.default.blocksize = blocksize
+
+
 def set_device(
-    device_numbers: list | int | None = None,
+    device: list[int] | list[str] | str | int | None = None,
     sampling_rate_hz: int | None = None,
 ):
     """Takes in a device number to set it as the default for the input and the
     output. If `None` is passed, the available devices are first shown and
     then the user is asked for input to set the device two values separated by
     a comma "input_int, output_int".
 
     Parameters
     ----------
-    device_number : list with length 2, optional
+    device : list[int | str] with length 2, str, int, optional
         Sets the input and output devices from two integers, e.g. [1, 2].
-        Use `None` to be prompted with the options and pass only two values
-        separated by a comma, e.g., `1, 2`. Default: `None`.
+        Alternatively, two strings contained in the interface's name (or the
+        name itself) can be passed. The first interface to match will be taken.
+        If passing only one string or integer, the interface will be taken for
+        both input and output. Use `None` to be prompted with the options and
+        pass only two values separated by a comma, e.g., `1, 2`.
+        Default: `None`.
     sampling_rate_hz : int, optional
         Pass a default sampling rate to the devices. Pass `None` to ignore.
         Default: `None`.
 
     Returns
     -------
     device_list : `sounddevice.DeviceList`
         Device List with dictionaries containing information about each
-        available device.
+        available device if `device=None`.
 
     """
-    if device_numbers is None:
+    if device is None:
         txt = "List of available devices"
         print(txt + "\n" + "-" * len(txt))
         print(sd.query_devices())
         print("-" * len(txt))
-        device_numbers = input(
+        device = input(
             "Which device should be set as default? Between "
             + f"0 and {len(sd.query_devices()) - 1}: "
         )
-        device_numbers = [int(d) for d in device_numbers.split(",")]
-        if len(device_numbers) == 1:
-            device_numbers = device_numbers[0]
+        device = [int(d) for d in device.split(",")]
+        if len(device) == 1:
+            device = device[0]
     device_list = sd.query_devices()
-    if type(device_numbers) is int:
-        d = device_list[device_numbers]["name"]
+    if type(device) is int:
+        d = device_list[device]["name"]
         print(f"""{d} will be used for input and output!""")
-        sd.default.device = device_numbers
-    elif type(device_numbers) is list:
-        assert (
-            len(device_numbers) == 2
-        ), "List with device numbers must be exactly 2"
-        d = device_list[device_numbers[0]]["name"]
-        print(f"""{d} will be used for input!""")
-
-        d = device_list[device_numbers[1]]["name"]
-        print(f"""{d} will be used for output!""")
-        sd.default.device = device_numbers
+        sd.default.device = device
+    elif type(device) is str:
+        d_id, d_name = get_interface_number_by_name(device, device_list)
+        print(f"{d_name} will be used for input and output!")
+        sd.default.device = d_id
+    elif type(device) is list:
+        assert len(device) == 2, "List with device numbers must be exactly 2"
+
+        if type(device[0]) is int and type(device[1]) is int:
+            d = device_list[device[0]]["name"]
+            print(f"{d} will be used for input!")
+
+            d = device_list[device[1]]["name"]
+            print(f"{d} will be used for output!")
+            sd.default.device = device
+        elif type(device[0]) is str and type(device[1]) is str:
+            d_id_in, d_name_in = get_interface_number_by_name(
+                device[0], device_list
+            )
+            print(f"{d_name_in} will be used for input!")
+
+            d_id_out, d_name_out = get_interface_number_by_name(
+                device[1], device_list
+            )
+            print(f"{d_name_out} will be used for output!")
+            sd.default.device = [d_id_in, d_id_out]
+        else:
+            raise TypeError(
+                "device must be either a homogenouos list of int and "
+                + "str, or an int or a str"
+            )
     else:
-        raise TypeError("device_number must be either a list or an int")
+        raise TypeError(
+            "device must be either a homogenouos list of int and "
+            + "str, or an int or a str"
+        )
 
     # Sampling rate
     if sampling_rate_hz is not None:
         sd.default.samplerate = sampling_rate_hz
     return sd.query_devices()
 
 
+def get_interface_number_by_name(
+    name: str, device_list: sd.DeviceList
+) -> tuple[int, str]:
+    """
+    Return the interface ID (number) by looking at its name.
+
+    Parameters
+    ----------
+    name : str
+        Name of the interface or string contained in the name (the first
+        interface to match will be returned). The comparison is case-invariant.
+
+    Returns
+    -------
+    ind : int
+        Interface ID
+    full_name : str
+        Interface's full name
+
+    """
+    for ind, d in enumerate(device_list):
+        full_name: str = d["name"]
+        if name.lower() in full_name.lower():
+            return ind, full_name
+    raise ValueError(f"No device was found with name {name}")
+
+
 def play_and_record(
     signal: Signal,
     duration_seconds: float | None = None,
-    normalized_dbfs: float = -6,
+    normalized_dbfs: float | None = -6,
     device: str | None = None,
     play_channels=None,
     rec_channels=[1],
 ) -> Signal:
     """Play and record using some available device. Note that the channel
     numbers start here with 1.
 
@@ -181,16 +272,16 @@
         + f"({duration_seconds:.1f} s)..."
     )
     rec_time_data = sd.playrec(
         data=play_data,
         samplerate=signal.sampling_rate_hz,
         input_mapping=rec_channels,
         output_mapping=play_channels,
+        blocking=True,
     )
-    sd.wait()
     print("Playback and recording have ended\n")
 
     rec_sig = Signal(None, rec_time_data, signal.sampling_rate_hz)
     return rec_sig
 
 
 def record(
@@ -232,16 +323,16 @@
         sd.default.device = device
 
     print(f"\nRecording started ({duration_seconds:.1f} s)...")
     rec_time_data = sd.rec(
         frames=int(duration_seconds * sampling_rate_hz),
         samplerate=sampling_rate_hz,
         mapping=rec_channels,
+        blocking=True,
     )
-    sd.wait()
     print("Recording has ended\n")
 
     rec_sig = Signal(None, rec_time_data, sampling_rate_hz)
     return rec_sig
 
 
 def play(
@@ -298,16 +389,16 @@
         sd.default.device = device
 
     print(f"Playback started ({duration_seconds:.1f} s)...")
     sd.play(
         data=play_data,
         samplerate=signal.sampling_rate_hz,
         mapping=play_channels,
+        blocking=True,
     )
-    sd.wait()
     print("Playback has ended\n")
 
 
 def play_through_stream(
     signal: Signal,
     blocksize: int = 2048,
     audio_callback=standard_callback,
```

### Comparing `dsptoolbox-0.3.5/dsptoolbox/beamforming/__init__.py` & `dsptoolbox-0.3.6/dsptoolbox/beamforming/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/beamforming/_beamforming.py` & `dsptoolbox-0.3.6/dsptoolbox/beamforming/_beamforming.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/beamforming/beamforming.py` & `dsptoolbox-0.3.6/dsptoolbox/beamforming/beamforming.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/classes/__init__.py` & `dsptoolbox-0.3.6/dsptoolbox/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/classes/_filter.py` & `dsptoolbox-0.3.6/dsptoolbox/classes/_filter.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/classes/_lattice_ladder_filter.py` & `dsptoolbox-0.3.6/dsptoolbox/classes/_lattice_ladder_filter.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/classes/_phaseLinearizer.py` & `dsptoolbox-0.3.6/dsptoolbox/classes/_phaseLinearizer.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/classes/_plots.py` & `dsptoolbox-0.3.6/dsptoolbox/classes/_plots.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/classes/_svfilter.py` & `dsptoolbox-0.3.6/dsptoolbox/classes/_svfilter.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/classes/filter_class.py` & `dsptoolbox-0.3.6/dsptoolbox/classes/filter_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,17 +74,17 @@
             - order (int): Filter order
             - freqs (float, array-like): array with len 2 when 'bandpass'
               or 'bandstop'.
             - type_of_pass (str): 'bandpass', 'lowpass', 'highpass',
               'bandstop'.
             - filter_design_method (str): Default: 'butter'. Supported methods
               are: 'butter', 'bessel', 'ellip', 'cheby1', 'cheby2'.
-            - bandpass ripple (float): maximum bandpass ripple in dB for
+            - bandpass_ripple (float): maximum bandpass ripple in dB for
               'ellip' and 'cheby1'.
-            - stopband ripple (float): maximum stopband ripple in dB for
+            - stopband_ripple (float): maximum stopband ripple in dB for
               'ellip' and 'cheby2'.
 
         For `fir`:
             Keys: order, freqs, type_of_pass, filter_design_method (optional),
             width (optional, necessary for 'kaiser'), filter_id (optional).
 
             - order (int): Filter order, i.e., number of taps - 1.
```

### Comparing `dsptoolbox-0.3.5/dsptoolbox/classes/filterbank.py` & `dsptoolbox-0.3.6/dsptoolbox/classes/filterbank.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/classes/multibandsignal.py` & `dsptoolbox-0.3.6/dsptoolbox/classes/multibandsignal.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/classes/signal_class.py` & `dsptoolbox-0.3.6/dsptoolbox/classes/signal_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -1089,15 +1089,14 @@
             Figure.
         ax : `matplotlib.axes.Axes`
             Axes.
 
         Notes
         -----
         - All values are clipped to be at least -800 dBFS.
-        - No time averaging is done in this function.
         - If it is an analytic signal and normalization is applied, the peak
           value of the real part is used as the normalization factor.
         - If the time window is not 0, effects at the edges of the signal might
           be present due to zero-padding.
 
         """
         td_squared = self.time_data**2
```

### Comparing `dsptoolbox-0.3.5/dsptoolbox/distances/_distances.py` & `dsptoolbox-0.3.6/dsptoolbox/distances/_distances.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/distances/distances.py` & `dsptoolbox-0.3.6/dsptoolbox/distances/distances.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/effects/__init__.py` & `dsptoolbox-0.3.6/dsptoolbox/effects/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/effects/_effects.py` & `dsptoolbox-0.3.6/dsptoolbox/effects/_effects.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/effects/effects.py` & `dsptoolbox-0.3.6/dsptoolbox/effects/effects.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/filterbanks/__init__.py` & `dsptoolbox-0.3.6/dsptoolbox/filterbanks/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,40 +17,47 @@
 
 Other:
 
 - `qmf_crossover()`: Quadrature mirror filters crossover.
 - `fractional_octave_bands()`: Butterworth bandpass filter bank with signal
   energy conservation.
 - `weightning_filter()`: A- or C-Weightning filter.
-- `fir_complementary()`: Create a complementary FIR filter from a linear-phase
-  FIR prototype.
+- `complementary_fir_filter()`: Create a complementary FIR filter from a
+  linear-phase FIR prototype.
 - `LatticeLadderFilter()`: Filter with lattice-ladder topology.
-- `PhaseLinearizer()`: Design FIR that linearize a phase spectrum.
+- `PhaseLinearizer()`: Design an FIR filter that linearizes a phase spectrum
+  or matches a target group delay.
+- `StateVariableFilter()`: SV-Filter discretized with a topology-preserving
+  transform.
+- `convert_into_lattice_filter()`: Turns a conventional filter into its
+  lattice/ladder representation.
 
 """
 
 from .filterbanks import (
     linkwitz_riley_crossovers,
     reconstructing_fractional_octave_bands,
     auditory_filters_gammatone,
     fractional_octave_bands,
     qmf_crossover,
     weightning_filter,
     complementary_fir_filter,
+    convert_into_lattice_filter,
 )
 
 from ..classes._lattice_ladder_filter import LatticeLadderFilter
 from ..classes._phaseLinearizer import PhaseLinearizer
 from ..classes._svfilter import StateVariableFilter
 
 __all__ = [
     "linkwitz_riley_crossovers",
     "reconstructing_fractional_octave_bands",
     "fractional_octave_bands",
     "auditory_filters_gammatone",
     "qmf_crossover",
     "weightning_filter",
     "complementary_fir_filter",
+    "convert_into_lattice_filter",
     "LatticeLadderFilter",
     "PhaseLinearizer",
     "StateVariableFilter",
 ]
```

### Comparing `dsptoolbox-0.3.5/dsptoolbox/filterbanks/_filterbank.py` & `dsptoolbox-0.3.6/dsptoolbox/filterbanks/_filterbank.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/filterbanks/filterbanks.py` & `dsptoolbox-0.3.6/dsptoolbox/filterbanks/filterbanks.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 import warnings
 from .. import (
     Filter,
     FilterBank,
     fractional_octave_frequencies,
     erb_frequencies,
 )
+from ..classes._lattice_ladder_filter import (
+    LatticeLadderFilter,
+    _get_lattice_ladder_coefficients_iir,
+    _get_lattice_coefficients_fir,
+    _get_lattice_ladder_coefficients_iir_sos,
+)
 from ._filterbank import LRFilterBank, GammaToneFilterBank, QMFCrossover
 from .._standard import _kaiser_window_fractional
 
 
 def linkwitz_riley_crossovers(
     crossover_frequencies_hz, order, sampling_rate_hz: int
 ) -> LRFilterBank:
@@ -474,7 +480,52 @@
         b[impulse_index] += 1
     else:
         h = np.sinc(np.arange(-len(b) // 2 + 1, len(b) // 2 + 1) - 0.5)
         b = h * _kaiser_window_fractional(len(h), 60, 0.5) - b
 
     fir_complementary = Filter("other", {"ba": [b, [1]]}, fir.sampling_rate_hz)
     return fir_complementary
+
+
+def convert_into_lattice_filter(filt: Filter) -> LatticeLadderFilter:
+    """Convert an IIR or FIR filter into its lattice-ladder filter
+    representation. Filtering is then done using the lattice coefficients.
+    If the filter uses second-order sections, the lattice-ladder coefficients
+    are also computed and used in second-order sections.
+
+    Parameters
+    ----------
+    filt: `Filter`
+        Filter to convert into its lattice filter representation.
+
+    Returns
+    -------
+    new_filt : `LatticeLadderFilter`
+        New filter representation.
+
+    Notes
+    -----
+    - Linear phase FIR filters produce unstable reflection coefficients and
+      can therefore not be converted into lattice filters. When trying to do
+      this, an assertion error is raised.
+
+    """
+    if filt.filter_type in ("iir", "biquad"):
+        if hasattr(filt, "sos"):
+            sos = filt.get_coefficients("sos")
+            k, c = _get_lattice_ladder_coefficients_iir_sos(sos)
+        else:
+            b, a = filt.get_coefficients("ba")
+            k, c = _get_lattice_ladder_coefficients_iir(b, a)
+        new_filt = LatticeLadderFilter(k, c, filt.sampling_rate_hz)
+    elif filt.filter_type == "fir":
+        b, a = filt.get_coefficients("ba")
+        b /= b[0]
+        k = _get_lattice_coefficients_fir(b)
+        assert np.all(np.abs(k) < 1), (
+            "Some reflection coefficient was "
+            + "equal or larger than zero, this is not supported"
+        )
+        new_filt = LatticeLadderFilter(k, None, filt.sampling_rate_hz)
+    else:
+        raise ValueError(f"Unsupported filter type: {filt.filter_type}")
+    return new_filt
```

### Comparing `dsptoolbox-0.3.5/dsptoolbox/generators/generators.py` & `dsptoolbox-0.3.6/dsptoolbox/generators/generators.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/plots/plots.py` & `dsptoolbox-0.3.6/dsptoolbox/plots/plots.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/room_acoustics/__init__.py` & `dsptoolbox-0.3.6/dsptoolbox/room_acoustics/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/room_acoustics/_room_acoustics.py` & `dsptoolbox-0.3.6/dsptoolbox/room_acoustics/_room_acoustics.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/room_acoustics/room_acoustics.py` & `dsptoolbox-0.3.6/dsptoolbox/room_acoustics/room_acoustics.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/transfer_functions/__init__.py` & `dsptoolbox-0.3.6/dsptoolbox/transfer_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/transfer_functions/_transfer_functions.py` & `dsptoolbox-0.3.6/dsptoolbox/transfer_functions/_transfer_functions.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/transfer_functions/transfer_functions.py` & `dsptoolbox-0.3.6/dsptoolbox/transfer_functions/transfer_functions.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/transforms/__init__.py` & `dsptoolbox-0.3.6/dsptoolbox/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/transforms/_transforms.py` & `dsptoolbox-0.3.6/dsptoolbox/transforms/_transforms.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/dsptoolbox/transforms/transforms.py` & `dsptoolbox-0.3.6/dsptoolbox/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/audio_io_module.ipynb` & `dsptoolbox-0.3.6/examples/audio_io_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/beamforming_module.ipynb` & `dsptoolbox-0.3.6/examples/beamforming_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/distances_module.ipynb` & `dsptoolbox-0.3.6/examples/distances_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/filterbanks_module.ipynb` & `dsptoolbox-0.3.6/examples/filterbanks_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/general.ipynb` & `dsptoolbox-0.3.6/examples/general.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/generators_module.ipynb` & `dsptoolbox-0.3.6/examples/generators_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/room_acoustics_module.ipynb` & `dsptoolbox-0.3.6/examples/room_acoustics_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/standard_module.ipynb` & `dsptoolbox-0.3.6/examples/standard_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/transfer_function_module.ipynb` & `dsptoolbox-0.3.6/examples/transfer_function_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/transforms_module.ipynb` & `dsptoolbox-0.3.6/examples/transforms_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/data/array.xml` & `dsptoolbox-0.3.6/examples/data/array.xml`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/data/chirp.wav` & `dsptoolbox-0.3.6/examples/data/chirp.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/data/chirp_mono.wav` & `dsptoolbox-0.3.6/examples/data/chirp_mono.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/data/chirp_stereo.wav` & `dsptoolbox-0.3.6/examples/data/chirp_stereo.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/data/fuer_elise.wav` & `dsptoolbox-0.3.6/examples/data/fuer_elise.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/data/rir.wav` & `dsptoolbox-0.3.6/examples/data/rir.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/examples/data/speech.flac` & `dsptoolbox-0.3.6/examples/data/speech.flac`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/tests/test_beamforming.py` & `dsptoolbox-0.3.6/tests/test_beamforming.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/tests/test_classes.py` & `dsptoolbox-0.3.6/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/tests/test_distances.py` & `dsptoolbox-0.3.6/tests/test_distances.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/tests/test_filterbanks.py` & `dsptoolbox-0.3.6/tests/test_filterbanks.py`

 * *Files 10% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         gd *= ir.sampling_rate_hz
         pl = dsp.filterbanks.PhaseLinearizer(
             np.ones(len(gd)), len(ir), fs_hz, gd.squeeze()
         )
         pl.get_filter_as_ir()
         pl.get_filter()
 
-    def test_VSFilter(self):
+    def test_SVFilter(self):
         fs_hz = 10_000
         f = dsp.filterbanks.StateVariableFilter(500, np.sqrt(2), fs_hz)
 
         n = dsp.generators.noise(sampling_rate_hz=fs_hz)
         f.filter_signal(n)
 
         n = dsp.generators.noise(number_of_channels=3, sampling_rate_hz=fs_hz)
@@ -225,7 +225,46 @@
 
         k, c = _get_lattice_ladder_coefficients_iir(self.b / 10, self.a)
 
         f = dsp.filterbanks.LatticeLadderFilter(k, c, sampling_rate_hz=200)
         out = f.filter_signal(n)
         out = out.time_data.squeeze()
         assert np.all(np.isclose(expected, out))
+
+    def test_convert_lattice_filter(self):
+        fs = 44100
+        # Second-order sections
+        n = dsp.generators.noise(sampling_rate_hz=fs)
+        f = dsp.Filter(
+            "iir",
+            {
+                "filter_design_method": "bessel",
+                "order": 9,
+                "type_of_pass": "lowpass",
+                "freqs": 1000,
+            },
+            sampling_rate_hz=fs,
+        )
+        new_f = dsp.filterbanks.convert_into_lattice_filter(f)
+        n1 = f.filter_signal(n).time_data.squeeze()
+        n2 = new_f.filter_signal(n).time_data.squeeze()
+        assert np.all(np.isclose(n1, n2))
+
+        # BA
+        b, a = f.get_coefficients("ba")
+        f2 = dsp.Filter("other", {"ba": [b, a]}, f.sampling_rate_hz)
+        new_f = dsp.filterbanks.convert_into_lattice_filter(f2)
+        n1 = f2.filter_signal(n).time_data.squeeze()
+        n2 = new_f.filter_signal(n).time_data.squeeze()
+        assert np.all(np.isclose(n1, n2))
+
+        # FIR
+        n = dsp.generators.noise(sampling_rate_hz=fs)
+        f = dsp.Filter(
+            "other",
+            {"ba": [[1, 13 / 24, 5 / 8, 1 / 3], [1]]},
+            sampling_rate_hz=fs,
+        )
+        new_f = dsp.filterbanks.convert_into_lattice_filter(f)
+        n1 = f.filter_signal(n).time_data.squeeze()
+        n2 = new_f.filter_signal(n).time_data.squeeze()
+        assert np.all(np.isclose(n1, n2))
```

### Comparing `dsptoolbox-0.3.5/tests/test_fx.py` & `dsptoolbox-0.3.6/tests/test_fx.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/tests/test_generators.py` & `dsptoolbox-0.3.6/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/tests/test_room_acoustics.py` & `dsptoolbox-0.3.6/tests/test_room_acoustics.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/tests/test_standard.py` & `dsptoolbox-0.3.6/tests/test_standard.py`

 * *Files 10% similar despite different names*

```diff
@@ -337,45 +337,22 @@
 
         fb = dsp.filterbanks.auditory_filters_gammatone(
             [500, 1000], 1, s.sampling_rate_hz
         )
         ss = fb.filter_signal(s)
         dsp.envelope(ss)
 
-    def test_convert_lattice_filter(self):
-        fs = 44100
-        # Second-order sections
-        n = dsp.generators.noise(sampling_rate_hz=fs)
-        f = dsp.Filter(
-            "iir",
-            {
-                "filter_design_method": "bessel",
-                "order": 9,
-                "type_of_pass": "lowpass",
-                "freqs": 1000,
-            },
-            sampling_rate_hz=fs,
-        )
-        new_f = dsp.convert_into_lattice_filter(f)
-        n1 = f.filter_signal(n).time_data.squeeze()
-        n2 = new_f.filter_signal(n).time_data.squeeze()
-        assert np.all(np.isclose(n1, n2))
-
-        # BA
-        b, a = f.get_coefficients("ba")
-        f2 = dsp.Filter("other", {"ba": [b, a]}, f.sampling_rate_hz)
-        new_f = dsp.convert_into_lattice_filter(f2)
-        n1 = f2.filter_signal(n).time_data.squeeze()
-        n2 = new_f.filter_signal(n).time_data.squeeze()
-        assert np.all(np.isclose(n1, n2))
+    def test_dither(self):
+        # Functionality
+        dsp.dither(self.audio_multi)
 
-        # FIR
-        n = dsp.generators.noise(sampling_rate_hz=fs)
-        f = dsp.Filter(
-            "other",
-            {"ba": [[1, 13 / 24, 5 / 8, 1 / 3], [1]]},
-            sampling_rate_hz=fs,
+        fb = dsp.FilterBank(
+            [
+                dsp.Filter(
+                    "biquad",
+                    {"freqs": 500, "q": 1, "gain": 2, "eq_type": "peaking"},
+                    self.audio_multi.sampling_rate_hz,
+                )
+            ]
         )
-        new_f = dsp.convert_into_lattice_filter(f)
-        n1 = f.filter_signal(n).time_data.squeeze()
-        n2 = new_f.filter_signal(n).time_data.squeeze()
-        assert np.all(np.isclose(n1, n2))
+        dsp.dither(self.audio_multi, noise_shaping_filterbank=fb)
+        dsp.dither(self.audio_multi, truncate=False)
```

### Comparing `dsptoolbox-0.3.5/tests/test_transfer_functions.py` & `dsptoolbox-0.3.6/tests/test_transfer_functions.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/tests/test_transforms.py` & `dsptoolbox-0.3.6/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/LICENSE` & `dsptoolbox-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/README.rst` & `dsptoolbox-0.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/pyproject.toml` & `dsptoolbox-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.5/PKG-INFO` & `dsptoolbox-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsptoolbox
-Version: 0.3.5
+Version: 0.3.6
 Summary: Collection of dsp algorithms to be used for analysis of audio signals
 Project-URL: Homepage, https://github.com/nico-franco-gomez/dsptoolbox
 Project-URL: Bug Tracker, https://github.com/nico-franco-gomez/dsptoolbox/issues
 Project-URL: Documentation, https://dsptoolbox.readthedocs.io/en/latest/
 Author: Nicolas Franco-Gomez
 License-Expression: MIT
 License-File: LICENSE
```

